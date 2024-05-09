# Comparing `tmp/autoversioner-24.1.6-py2.py3-none-any.whl.zip` & `tmp/autoversioner-24.5.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5731 bytes, number of entries: 9
--rw-r--r--  2.0 unx      356 b- defN 24-Jan-04 06:31 autoversioner/__init__.py
--rw-r--r--  2.0 unx     6665 b- defN 24-Jan-05 21:47 autoversioner/autoversioner.py
--rw-r--r--  2.0 unx      117 b- defN 24-Jan-05 21:47 autoversioner/version.py
--rw-r--r--  2.0 unx     1059 b- defN 24-Jan-05 21:48 autoversioner-24.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     3995 b- defN 24-Jan-05 21:48 autoversioner-24.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Jan-05 21:48 autoversioner-24.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       68 b- defN 24-Jan-05 21:48 autoversioner-24.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 24-Jan-05 21:48 autoversioner-24.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      772 b- defN 24-Jan-05 21:48 autoversioner-24.1.6.dist-info/RECORD
-9 files, 13156 bytes uncompressed, 4385 bytes compressed:  66.7%
+Zip file size: 5770 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      394 b- defN 24-May-09 03:48 autoversioner/__init__.py
+-rw-r--r--  2.0 unx     6749 b- defN 24-May-09 03:48 autoversioner/autoversioner.py
+-rw-r--r--  2.0 unx      117 b- defN 24-May-09 03:49 autoversioner/version.py
+-rw-r--r--  2.0 unx     1060 b- defN 24-May-09 03:49 autoversioner-24.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3995 b- defN 24-May-09 03:49 autoversioner-24.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-09 03:49 autoversioner-24.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       68 b- defN 24-May-09 03:49 autoversioner-24.5.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 24-May-09 03:49 autoversioner-24.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      772 b- defN 24-May-09 03:49 autoversioner-24.5.0.dist-info/RECORD
+9 files, 13279 bytes uncompressed, 4424 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: autoversioner/autoversioner.py
 Comment: 
 
 Filename: autoversioner/version.py
 Comment: 
 
-Filename: autoversioner-24.1.6.dist-info/LICENSE
+Filename: autoversioner-24.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: autoversioner-24.1.6.dist-info/METADATA
+Filename: autoversioner-24.5.0.dist-info/METADATA
 Comment: 
 
-Filename: autoversioner-24.1.6.dist-info/WHEEL
+Filename: autoversioner-24.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: autoversioner-24.1.6.dist-info/entry_points.txt
+Filename: autoversioner-24.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: autoversioner-24.1.6.dist-info/top_level.txt
+Filename: autoversioner-24.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: autoversioner-24.1.6.dist-info/RECORD
+Filename: autoversioner-24.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## autoversioner/__init__.py

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python
 # coding: utf-8
 from autoversioner.version import __version__, __author__, __credits__
 from autoversioner.autoversioner import autoversioner, main
+
 """
 autoversioner
 
 This handy module with auto increment the version and save that to a JSON or .env file
 """
 
 __version__ = __version__
 __author__ = __author__
 __credits__ = __credits__
+
+__all__ = ["autoversioner", "main"]
```

## autoversioner/autoversioner.py

```diff
@@ -7,39 +7,41 @@
 import os
 import sys
 import getopt
 import json
 
 
 def usage():
-    print(f"Usage: \n"
-          f"-h | --help      [ See usage for script ]\n"
-          f"-e | --env       [ Export version metadata to environment file (/directory/.env) ]\n"
-          f"-j | --json      [ Export version metadata to JSON file (/directory/version.json) ]\n"
-          f"-d | --directory [ Directory to save .env and JSON files ]\n"
-          f"--major          [ Increment major version ]\n"
-          f"--minor          [ Increment minor version ]\n"
-          f"--patch          [ Patch version ]\n"
-          f"\n"
-          f"autoversioner -v 'v2024.1.4'\n"
-          f"autoversioner -v '2024.1.4'\n"
-          f"autoversioner -v '1.10.4' --json --directory '~/Downloads' --env\n")
+    print(
+        "Usage: \n"
+        "-h | --help      [ See usage for script ]\n"
+        "-e | --env       [ Export version metadata to environment file (/directory/.env) ]\n"
+        "-j | --json      [ Export version metadata to JSON file (/directory/version.json) ]\n"
+        "-d | --directory [ Directory to save .env and JSON files ]\n"
+        "--major          [ Increment major version ]\n"
+        "--minor          [ Increment minor version ]\n"
+        "--patch          [ Patch version ]\n"
+        "\n"
+        "autoversioner -v 'v2024.1.4'\n"
+        "autoversioner -v '2024.1.4'\n"
+        "autoversioner -v '1.10.4' --json --directory '~/Downloads' --env\n"
+    )
 
 
 def version(current_version="", major=False, minor=False, patch=False):
-    long_date_pattern = re.compile(r'20[1-2][0-9]')
-    short_date_pattern = re.compile(r'^[1-2][0-9]')
+    long_date_pattern = re.compile(r"20[1-2][0-9]")
+    short_date_pattern = re.compile(r"^[1-2][0-9]")
     today = datetime.date.today()
     long_year = today.strftime("%Y")
     short_year = today.strftime("%y")
     month = int(today.strftime("%m"))
     long_date = f"{long_year}.{month}"
     short_date = f"{short_year}.{month}"
     if current_version == "":
-        new_version = f'{short_date}.0'
+        new_version = f"{short_date}.0"
         return new_version
     cleaned_current_version = current_version.split(".")
     cleaned_current_version = cleaned_current_version[:3]
     try:
         cleaned_current_version[0] = str(int(cleaned_current_version[0]))
     except Exception as e:
         print(f"Unable to convert major version to int. Error: {e}")
@@ -62,71 +64,87 @@
         return new_version
     if patch:
         current_version = semantic_version.Version(current_version)
         new_version = current_version.next_patch()
         return new_version
     if long_date_pattern.search(current_version):
         current_version = semantic_version.Version(current_version)
-        s = semantic_version.SimpleSpec(f'<{long_date}.0')
-        new_version = f'{long_date}.0'
+        s = semantic_version.SimpleSpec(f"<{long_date}.0")
+        new_version = f"{long_date}.0"
         if s.match(current_version):
-            new_version = f'{long_date}.0'
-        s = semantic_version.SimpleSpec(f'=={long_date}.{current_version.patch}')
+            new_version = f"{long_date}.0"
+        s = semantic_version.SimpleSpec(f"=={long_date}.{current_version.patch}")
         if s.match(current_version):
             new_version = current_version.next_patch()
-            new_version = f'{str(new_version)}'
+            new_version = f"{str(new_version)}"
         return new_version
     elif short_date_pattern.search(current_version):
         current_version = semantic_version.Version(current_version)
-        s = semantic_version.SimpleSpec(f'<{short_date}.0')
-        new_version = f'{short_date}.0'
+        s = semantic_version.SimpleSpec(f"<{short_date}.0")
+        new_version = f"{short_date}.0"
         if s.match(current_version):
-            new_version = f'{short_date}.0'
-        s = semantic_version.SimpleSpec(f'=={short_date}.{current_version.patch}')
+            new_version = f"{short_date}.0"
+        s = semantic_version.SimpleSpec(f"=={short_date}.{current_version.patch}")
         if s.match(current_version):
             new_version = current_version.next_patch()
-            new_version = f'{str(new_version)}'
+            new_version = f"{str(new_version)}"
         return new_version
     else:
         current_version = semantic_version.Version(current_version)
         new_version = current_version.next_patch()
         return new_version
 
 
-def output(metadata=None, json_output=False, env_output=False, print_output=False, directory=""):
+def output(
+    metadata=None, json_output=False, env_output=False, print_output=False, directory=""
+):
     if not metadata:
         print("No metadata supplied to output")
         return
     if json_output:
-        json_file_path = os.path.join(directory, 'version.json')
+        json_file_path = os.path.join(directory, "version.json")
         # Write the dictionary to the JSON file
-        with open(json_file_path, 'w') as json_file:
+        with open(json_file_path, "w") as json_file:
             json.dump(metadata, json_file, indent=2)
     if env_output:
         env_metadata = {k.upper(): v for k, v in metadata.items()}
-        env_content = "\n".join([f"{key}={value}" for key, value in env_metadata.items()])
-        env_file_path = os.path.join(directory, '.env')
+        env_content = "\n".join(
+            [f"{key}={value}" for key, value in env_metadata.items()]
+        )
+        env_file_path = os.path.join(directory, ".env")
         # Save the content to the .env file
-        with open(env_file_path, 'w') as env_file:
+        with open(env_file_path, "w") as env_file:
             env_file.write(env_content)
     if print_output:
         print(f"{metadata['new_version']}")
 
 
 def autoversioner(argv):
-    current_version = '1.0.0'
+    current_version = "1.0.0"
     directory = ""
     environment_output = False
     json_output = False
     major = False
     minor = False
     patch = False
     try:
-        opts, args = getopt.getopt(argv, "hejd:v:", ["help", "env", "json", "directory=", "version=",
-                                                     "major", "minor", "patch"])
+        opts, args = getopt.getopt(
+            argv,
+            "hejd:v:",
+            [
+                "help",
+                "env",
+                "json",
+                "directory=",
+                "version=",
+                "major",
+                "minor",
+                "patch",
+            ],
+        )
     except getopt.GetoptError:
         usage()
         sys.exit(2)
     for opt, arg in opts:
         if opt in ("-h", "--help"):
             usage()
             sys.exit()
@@ -145,33 +163,34 @@
         elif opt == "--patch":
             patch = True
 
     if "fatal" in current_version:
         current_version = ""
     current_version = re.sub("v", "", current_version)
 
-    new_version = version(current_version=current_version,
-                          major=major,
-                          minor=minor,
-                          patch=patch)
+    new_version = version(
+        current_version=current_version, major=major, minor=minor, patch=patch
+    )
 
     version_metadata = {
         "current_version": current_version,
         "new_version": new_version,
         "current_version_tag": f"v{current_version}",
         "new_version_tag": f"v{new_version}",
         "version": new_version,
         "tag": f"v{new_version}",
     }
 
-    output(metadata=version_metadata,
-           json_output=json_output,
-           env_output=environment_output,
-           print_output=True,
-           directory=directory)
+    output(
+        metadata=version_metadata,
+        json_output=json_output,
+        env_output=environment_output,
+        print_output=True,
+        directory=directory,
+    )
 
 
 def main():
     if len(sys.argv) < 2:
         usage()
         sys.exit(2)
     autoversioner(sys.argv[1:])
```

## autoversioner/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '24.1.6'
-__author__ = 'Audel Rouhi'
-__credits__ = 'Audel Rouhi'
+__version__ = '24.5.0'
+__author__ = "Audel Rouhi"
+__credits__ = "Audel Rouhi"
```

## Comparing `autoversioner-24.1.6.dist-info/LICENSE` & `autoversioner-24.5.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Comparing `autoversioner-24.1.6.dist-info/METADATA` & `autoversioner-24.5.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoversioner
-Version: 24.1.6
+Version: 24.5.0
 Summary: Synchronize your subtitle files by shifting the subtitle time (+/-)
 Home-page: https://github.com/Knuckles-Team/subsync
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -37,15 +37,15 @@
 ![GitHub top language](https://img.shields.io/github/languages/top/Knuckles-Team/autoversioner)
 ![GitHub language count](https://img.shields.io/github/languages/count/Knuckles-Team/autoversioner)
 ![GitHub repo size](https://img.shields.io/github/repo-size/Knuckles-Team/autoversioner)
 ![GitHub repo file count (file type)](https://img.shields.io/github/directory-file-count/Knuckles-Team/autoversioner)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/autoversioner)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/autoversioner)
 
-*Version: 24.1.6*
+*Version: 24.5.0*
 
 This handy module with auto increment the version and save that to a JSON or .env file
 
 Date versions get set to current Year.Month.Revision
 
 - 23.12.4 -> 24.1.0
```

## Comparing `autoversioner-24.1.6.dist-info/RECORD` & `autoversioner-24.5.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-autoversioner/__init__.py,sha256=gvjjtDTMGUgzWtRwMRXLDu1WxVnr3R4QMp_h5tYlp-g,356
-autoversioner/autoversioner.py,sha256=SiOfZErYbvjANrQ6ywCxqrb_9iGdhaJPM1AbRibRkqY,6665
-autoversioner/version.py,sha256=zqhhR4tFQcGn3tThZhqeO2IWdViDnA1bK1t_CmTTg8k,117
-autoversioner-24.1.6.dist-info/LICENSE,sha256=wtI1_YjppxJA2UTLHLbj_goBi-f3DebTfIFbe_XqJmY,1059
-autoversioner-24.1.6.dist-info/METADATA,sha256=Sd7q-bZJ9sH8qSWY9xZ21Ns_2A_x8gGWdDLPEc-OJrY,3995
-autoversioner-24.1.6.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-autoversioner-24.1.6.dist-info/entry_points.txt,sha256=A_Y2aTze0djD-_pVsUukEKQlUoumU5mh1WH811oXaMs,68
-autoversioner-24.1.6.dist-info/top_level.txt,sha256=80N_NsgMFgL3xyc5VSVvGy68AuRvf-HdQIGQbrb-EgY,14
-autoversioner-24.1.6.dist-info/RECORD,,
+autoversioner/__init__.py,sha256=jxiP4HQTqBgVZCrSoUYo9LPgnioSsUxDad303yxGCXQ,394
+autoversioner/autoversioner.py,sha256=ATlCEH9QL_saHGcj9FYXASkPpcEiApm1an18KWr_zDM,6749
+autoversioner/version.py,sha256=Co2nTtfQyvnHFgN2UaHH6eQA7ZwGuM6jfvglIZ-tWDE,117
+autoversioner-24.5.0.dist-info/LICENSE,sha256=Z1xmcrPHBnGCETO_LLQJUeaSNBSnuptcDVTt4kaPUOE,1060
+autoversioner-24.5.0.dist-info/METADATA,sha256=EWQdu5jFjudD9as5oz7RygErMJxnFnc6-yTjpf5e4qg,3995
+autoversioner-24.5.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+autoversioner-24.5.0.dist-info/entry_points.txt,sha256=A_Y2aTze0djD-_pVsUukEKQlUoumU5mh1WH811oXaMs,68
+autoversioner-24.5.0.dist-info/top_level.txt,sha256=80N_NsgMFgL3xyc5VSVvGy68AuRvf-HdQIGQbrb-EgY,14
+autoversioner-24.5.0.dist-info/RECORD,,
```

