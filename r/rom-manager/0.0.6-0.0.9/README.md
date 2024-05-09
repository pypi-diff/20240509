# Comparing `tmp/rom_manager-0.0.6-py2.py3-none-any.whl.zip` & `tmp/rom_manager-0.0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 6096 bytes, number of entries: 9
--rw-r--r--  2.0 unx      313 b- defN 24-Feb-11 06:20 rom_manager/__init__.py
--rw-r--r--  2.0 unx     5831 b- defN 24-Feb-11 06:46 rom_manager/rom_manager.py
--rw-r--r--  2.0 unx      116 b- defN 24-Feb-11 06:46 rom_manager/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Feb-11 06:46 rom_manager-0.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     4079 b- defN 24-Feb-11 06:46 rom_manager-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Feb-11 06:46 rom_manager-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 24-Feb-11 06:46 rom_manager-0.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-Feb-11 06:46 rom_manager-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      746 b- defN 24-Feb-11 06:46 rom_manager-0.0.6.dist-info/RECORD
-9 files, 12337 bytes uncompressed, 4802 bytes compressed:  61.1%
+Zip file size: 53640 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      358 b- defN 24-Feb-11 10:54 rom_manager/__init__.py
+-rw-r--r--  2.0 unx   151059 b- defN 24-Feb-11 09:43 rom_manager/game_codes.py
+-rw-r--r--  2.0 unx    10328 b- defN 24-Feb-11 10:54 rom_manager/rom_manager.py
+-rw-r--r--  2.0 unx      116 b- defN 24-Feb-11 10:54 rom_manager/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Feb-11 10:55 rom_manager-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4549 b- defN 24-Feb-11 10:55 rom_manager-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Feb-11 10:55 rom_manager-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 24-Feb-11 10:55 rom_manager-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-Feb-11 10:55 rom_manager-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      831 b- defN 24-Feb-11 10:55 rom_manager-0.0.9.dist-info/RECORD
+10 files, 168493 bytes uncompressed, 52220 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: rom_manager/__init__.py
 Comment: 
 
+Filename: rom_manager/game_codes.py
+Comment: 
+
 Filename: rom_manager/rom_manager.py
 Comment: 
 
 Filename: rom_manager/version.py
 Comment: 
 
-Filename: rom_manager-0.0.6.dist-info/LICENSE
+Filename: rom_manager-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: rom_manager-0.0.6.dist-info/METADATA
+Filename: rom_manager-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: rom_manager-0.0.6.dist-info/WHEEL
+Filename: rom_manager-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: rom_manager-0.0.6.dist-info/entry_points.txt
+Filename: rom_manager-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: rom_manager-0.0.6.dist-info/top_level.txt
+Filename: rom_manager-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: rom_manager-0.0.6.dist-info/RECORD
+Filename: rom_manager-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rom_manager/__init__.py

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 # coding: utf-8
 from rom_manager.version import __version__, __author__, __credits__
+from rom_manager.game_codes import psx_codes
 from rom_manager.rom_manager import rom_manager, main, RomManager
 """
 rom-manager
 
 Create chd files for your compatible ROMs
 """
```

## rom_manager/rom_manager.py

```diff
@@ -3,88 +3,157 @@
 
 import os
 import sys
 import getopt
 import platform
 import subprocess
 import patoolib
+import glob
 import shutil
 from multiprocessing import Pool
-from rom_manager.version import __version__, __author__, __credits__
+try:
+    from version import __version__, __author__, __credits__
+    from game_codes import psx_codes
+except Exception:
+    from rom_manager.version import __version__, __author__, __credits__
+    from rom_manager.game_codes import psx_codes
 
 
 class RomManager:
     def __init__(self):
         self.silent = False
         self.chd_commands = []
         self.directory = os.path.curdir
         self.supported_types = [".iso", ".cue", ".gdi"]
         self.archive_formats = ['7z', 'zip', 'tar.gz', 'gz', 'gzip', 'bz2', 'bzip2', 'rar', 'tar']
         self.extracted_directories = []
+        self.processed_files = []
 
     def parallel_process_archives(self, cpu_count=None):
         if not cpu_count:
             cpu_count = os.cpu_count()
         pool = Pool(processes=cpu_count)
         try:
-            pool.map(self.process_archive, get_files(directory=self.directory, extensions=self.archive_formats))
+            files = self.get_files(directory=self.directory, extensions=self.archive_formats)
+            pool.map(self.process_archive, files)
         finally:
             pool.close()
             pool.join()
+        print("Extracting All Archives Complete!")
+        self.processed_files = files
+        for file in files:
+            extracted_directory = os.path.join(os.path.dirname(file), os.path.splitext(os.path.basename(file))[0])
+            self.extracted_directories.append(extracted_directory)
 
-    def process_archive(self, archive):
-        archive_directory = os.path.splitext(os.path.basename(archive))[0]
-        print(f"Extracting {archive} to {archive_directory}...")
-        os.makedirs(archive_directory, exist_ok=True)
-        patoolib.extract_archive(archive, outdir=archive_directory)
-        self.extracted_directories.append(archive_directory)
-        print(f"Finished Extracting {archive} to {archive_directory}")
-
-    def cleanup_extracted_archives(self):
+    def cleanup(self, deep_clean=False):
         for extracted_directory in self.extracted_directories:
             print(f"Cleaning {extracted_directory}...")
+            for file_path in self.get_files(directory=extracted_directory, extensions=[".chd"]):
+                parent_directory = os.path.dirname(os.path.dirname(file_path))
+                new_file_path = os.path.join(parent_directory, os.path.basename(file_path))
+                shutil.move(f"{file_path}", f"{new_file_path}")
             shutil.rmtree(extracted_directory)
             print(f"Finished Cleaning {extracted_directory}")
 
-    def build_commands(self):
-        for file in get_files(directory=self.directory, extensions=self.supported_types):
+        if deep_clean:
+            for file in self.processed_files:
+                if os.path.exists(file):
+                    os.remove(file)
+                    print(f"The file {file} has been deleted.")
+                else:
+                    print(f"The file {file} does not exist.")
+
+    def build_commands(self, force=False):
+        for file in self.get_files(directory=self.directory, extensions=self.supported_types):
+            for key, value in psx_codes.items():
+                if key in os.path.basename(file):
+                    # filename = os.path.splitext(os.path.basename(file))[0]
+                    file_path = os.path.dirname(file)
+                    file_extension = os.path.splitext(file)[1]
+                    new_file = os.path.join(file_path, f"{value} - {key}{file_extension}")
+                    if file != new_file:
+                        os.rename(file, new_file)
+                        file = new_file
+                    print(f"The string contains the key: {key}")
             chd_file = f"{os.path.splitext(os.path.basename(file))[0]}.chd"
             chd_file_directory = os.path.dirname(file)
-            chd_file_path = f"{chd_file_directory}/{chd_file}"
-            self.chd_commands.append(['chdman', 'createcd', '-i', f'"{file}"', '-o', f'"{chd_file_path}"'])
+            chd_file_path = os.path.join(chd_file_directory, chd_file)
+            chd_command = ['chdman', 'createcd', '-i', f"{file}", '-o', f"{chd_file_path}"]
+            if force:
+                chd_command.append('-f')
+            self.chd_commands.append(chd_command)
 
     def parallel_run_commands(self, cpu_count=None):
         if not cpu_count:
             cpu_count = os.cpu_count()
         pool = Pool(processes=cpu_count)
         try:
             pool.map(self.run_command, self.chd_commands)
         finally:
             pool.close()
             pool.join()
+        print("Converting All Files Complete!")
 
     def run_command(self, command):
         try:
             if self.silent:
                 result = subprocess.run(command, stdout=open(os.devnull, 'wb'), stderr=open(os.devnull, 'wb'))
             else:
                 result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                         universal_newlines=True)
             print(result.returncode, result.stdout, result.stderr)
         except subprocess.CalledProcessError as e:
             print(e.output)
 
+    def process_archive(self, archive):
+        archive_directory = os.path.join(os.path.dirname(archive), os.path.splitext(os.path.basename(archive))[0])
+        print(f"Extracting {archive} to {archive_directory}...")
+        os.makedirs(archive_directory, exist_ok=True)
+        try:
+            patoolib.extract_archive(archive, outdir=archive_directory)
+        except patoolib.util.PatoolError as e:
+            print(f"Unable to extract: {archive}\nError: {e}")
 
-def get_files(directory, extensions):
-    matching_files = []
-    for root, dirs, files in os.walk(directory):
-        for file in files:
-            if any(file.endswith(ext) for ext in extensions):
-                matching_files.append(os.path.join(root, file))
-    return matching_files
+        print(f"Finished Extracting {archive} to {archive_directory}")
+        print("Generating any missing cue file(s)")
+        if (glob.glob(os.path.join(str(archive_directory), "*.bin"))
+                and not glob.glob(os.path.join(str(archive_directory), "*.cue"))):
+            self.cue_file_generator(archive_directory)
+
+    @staticmethod
+    def pad_leading_zero(number):
+        padded = "0" + str(number)
+        return padded[-2:]
+
+    def cue_file_generator(self, directory):
+        file_names = self.get_files(directory=directory, extensions=[".bin"])
+        first_file = file_names.pop(0)
+        first_file = os.path.basename(first_file)
+        sheet = (f'FILE "{first_file}" BINARY\n'
+                 f'  TRACK 01 MODE2/2352\n'
+                 f'    INDEX 01 00:00:00\n')
+        track_counter = 2
+        for file_name in file_names:
+            sheet += (f'FILE "{file_name}" BINARY\n'
+                      f'  TRACK {self.pad_leading_zero(track_counter)} AUDIO\n'
+                      f'    INDEX 00 00:00:00\n'
+                      f'    INDEX 01 00:02:00\n')
+            track_counter += 1
+        cue_file_path = os.path.join(directory, f"{os.path.splitext(os.path.basename(first_file))[0]}.cue")
+        with open(cue_file_path, "w") as cue_file:
+            cue_file.write(sheet)
+
+    @staticmethod
+    def get_files(directory, extensions):
+        matching_files = []
+        for root, dirs, files in os.walk(directory):
+            for file in files:
+                if any(file.endswith(ext) for ext in extensions):
+                    matching_files.append(os.path.join(root, file))
+        return matching_files
 
 
 def get_operating_system():
     operating_system = None
     system = platform.system()
     release = platform.release()
     version = platform.version()
@@ -110,58 +179,93 @@
 def usage():
     print(f'ROM Manager: Convert Game ROMs to Compressed Hunks of Data (CHD) file format\n'
           f'Version: {__version__}\n'
           f'Author: {__author__}\n'
           f'Credits: {__credits__}\n'
           f"\n"
           f"Usage: \n"
-          f"-h | --help      [ See usage for script ]\n"
-          f"-d | --directory [ Directory to process ROMs ]\n"
-          f"-s | --silent    [ Suppress output messages ]\n"
+          f"-h | --help       [ See usage for script ]\n"
+          f"-c | --cpu-count  [ Limit max number of CPUs to use for parallel processing ]\n"
+          f"-d | --directory  [ Directory to process ROMs ]\n"
+          f"-f | --force      [ Force overwrite of existing CHD files ]\n"
+          f"-s | --silent     [ Suppress output messages ]\n"
+          f"-x | --delete     [ Delete original files after processing ]\n"
           f"\n"
           f"Example: \n"
           f"rom-manager --directory 'C:/Users/default/Games/'\n")
     installation_instructions()
 
 
 def rom_manager(argv):
     cpu_count = None
     directory = ""
     silent = False
+    force = False
+    deep_clean = False
 
     try:
-        opts, args = getopt.getopt(argv, "hc:d:s", ["help", "cpu-count=", "directory=", "silent"])
+        opts, args = getopt.getopt(argv, "hc:d:fsx", ["help", "cpu-count=", "directory=", "force", "silent",
+                                                      "delete"])
     except getopt.GetoptError:
         usage()
         sys.exit(2)
     for opt, arg in opts:
         if opt in ("-h", "--help"):
             usage()
             sys.exit()
         elif opt in ("-c", "--cpu-count"):
-            cpu_count = arg
+            if 0 < int(arg) <= os.cpu_count():
+                cpu_count = int(arg)
         elif opt in ("-d", "--directory"):
             directory = arg
+        elif opt in ("-f", "--force"):
+            force = True
         elif opt in ("-s", "--silent"):
             silent = True
+        elif opt in ("-x", "--delete"):
+            deep_clean = True
 
     roms_manager = RomManager()
     roms_manager.silent = silent
     roms_manager.directory = directory
     roms_manager.parallel_process_archives(cpu_count=cpu_count)
-    roms_manager.build_commands()
+    roms_manager.build_commands(force=force)
     roms_manager.parallel_run_commands(cpu_count=cpu_count)
-    roms_manager.cleanup_extracted_archives()
+    roms_manager.cleanup(deep_clean=deep_clean)
 
 
 def main():
     if len(sys.argv) < 2:
         usage()
         sys.exit(2)
     rom_manager(sys.argv[1:])
 
 
 if __name__ == "__main__":
     if len(sys.argv) < 2:
         usage()
         sys.exit(2)
     rom_manager(sys.argv[1:])
+
+    # import csv
+    #
+    # csv_file = "ps1_codes.csv"
+    #
+    # # Initialize an empty dictionary
+    # data_dict = {}
+    #
+    # with open(csv_file, "r") as file:
+    #     reader = csv.reader(file)
+    #     for row in reader:
+    #         key, value = row
+    #         keys = key.split("\n")
+    #         value = value.replace("\xa0", "")
+    #         for k in keys:
+    #             data_dict[k] = value
+    #
+    #
+    #
+    # print(data_dict)
+    # import json
+    # with open('ps1_codes.json', 'w', encoding='utf-8') as f:
+    #     json.dump(data_dict, f, ensure_ascii=False, indent=2)
+    #
```

## rom_manager/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.0.6'
+__version__ = '0.0.9'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `rom_manager-0.0.6.dist-info/LICENSE` & `rom_manager-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rom_manager-0.0.6.dist-info/METADATA` & `rom_manager-0.0.9.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rom-manager
-Version: 0.0.6
+Version: 0.0.9
 Summary: Synchronize your subtitle files by shifting the subtitle time (+/-)
 Home-page: https://github.com/Knuckles-Team/rom-manager
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,18 +38,20 @@
 ![GitHub top language](https://img.shields.io/github/languages/top/Knuckles-Team/rom_manager)
 ![GitHub language count](https://img.shields.io/github/languages/count/Knuckles-Team/rom_manager)
 ![GitHub repo size](https://img.shields.io/github/repo-size/Knuckles-Team/rom_manager)
 ![GitHub repo file count (file type)](https://img.shields.io/github/directory-file-count/Knuckles-Team/rom_manager)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/rom_manager)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/rom_manager)
 
-*Version: 0.0.6*
+*Version: 0.0.9*
 
 Convert Game ROMs to Compressed Hunks of Data (CHD) file format
 
+Automatically generate missing .cue files for your .bin files!
+
 #### Why?
 
 CHD (“Compressed Hunks of Data”) files are compressed data files that can be used on most CD-based systems. 
 They are in a lossless compression format, meaning that they perfectly preserve all game data while reducing file sizes. 
 CHDs were originally developed for MAME to compress CD-based arcade games, 
 but now they are compatible with a variety emulators and CD-based consoles.
 
@@ -80,19 +82,22 @@
 - cue
 - iso
 - gdi
 
 <details>
   <summary><b>Usage:</b></summary>
 
-| Short Flag | Long Flag   | Description                |
-|------------|-------------|----------------------------|
-| -h         | --help      | See Usage                  |
-| -d         | --directory | Directory to scan for ROMs |
-| -s         | --silent    | Suppress output text       |
+| Short Flag | Long Flag   | Description                                             |
+|------------|-------------|---------------------------------------------------------|
+| -h         | --help      | See Usage                                               |
+| -c         | --cpu-count | Limit max number of CPUs to use for parallel processing |
+| -d         | --directory | Directory to scan for ROMs                              |
+| -x         | --delete    | Delete the original files                               |
+| -f         | --force     | Force overwrite of existing CHD files                   |
+| -s         | --silent    | Suppress output text                                    |
 
 </details>
 
 <details>
   <summary><b>Example:</b></summary>
 
 ```bash
```

