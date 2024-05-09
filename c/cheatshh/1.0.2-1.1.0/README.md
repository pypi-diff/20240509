# Comparing `tmp/cheatshh-1.0.2.tar.gz` & `tmp/cheatshh-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheatshh-1.0.2.tar", last modified: Thu May  9 10:24:34 2024, max compression
+gzip compressed data, was "cheatshh-1.1.0.tar", last modified: Thu May  9 08:14:30 2024, max compression
```

## Comparing `cheatshh-1.0.2.tar` & `cheatshh-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,12 @@
-drwxr-xr-x   0 anirudhgupta   (501) staff       (20)        0 2024-05-09 10:24:34.912898 cheatshh-1.0.2/
--rw-r--r--   0 anirudhgupta   (501) staff       (20)    11357 2024-05-09 07:38:12.000000 cheatshh-1.0.2/LICENSE
--rw-r--r--   0 anirudhgupta   (501) staff       (20)     1245 2024-05-09 10:24:34.912607 cheatshh-1.0.2/PKG-INFO
--rw-r--r--   0 anirudhgupta   (501) staff       (20)     2548 2024-05-09 07:55:28.000000 cheatshh-1.0.2/README.md
-drwxr-xr-x   0 anirudhgupta   (501) staff       (20)        0 2024-05-09 10:24:34.911891 cheatshh-1.0.2/cheatshh.egg-info/
--rw-r--r--   0 anirudhgupta   (501) staff       (20)     1245 2024-05-09 10:24:34.000000 cheatshh-1.0.2/cheatshh.egg-info/PKG-INFO
--rw-r--r--   0 anirudhgupta   (501) staff       (20)      256 2024-05-09 10:24:34.000000 cheatshh-1.0.2/cheatshh.egg-info/SOURCES.txt
--rw-r--r--   0 anirudhgupta   (501) staff       (20)        1 2024-05-09 10:24:34.000000 cheatshh-1.0.2/cheatshh.egg-info/dependency_links.txt
--rw-r--r--   0 anirudhgupta   (501) staff       (20)       51 2024-05-09 10:24:34.000000 cheatshh-1.0.2/cheatshh.egg-info/entry_points.txt
--rw-r--r--   0 anirudhgupta   (501) staff       (20)       21 2024-05-09 10:24:34.000000 cheatshh-1.0.2/cheatshh.egg-info/requires.txt
--rw-r--r--   0 anirudhgupta   (501) staff       (20)        4 2024-05-09 10:24:34.000000 cheatshh-1.0.2/cheatshh.egg-info/top_level.txt
--rw-r--r--   0 anirudhgupta   (501) staff       (20)       38 2024-05-09 10:24:34.912948 cheatshh-1.0.2/setup.cfg
--rw-r--r--   0 anirudhgupta   (501) staff       (20)     2772 2024-05-09 10:24:06.000000 cheatshh-1.0.2/setup.py
-drwxr-xr-x   0 anirudhgupta   (501) staff       (20)        0 2024-05-09 10:24:34.912133 cheatshh-1.0.2/src/
--rw-r--r--   0 anirudhgupta   (501) staff       (20)        0 2024-05-09 09:59:20.000000 cheatshh-1.0.2/src/__init__.py
--rw-r--r--   0 anirudhgupta   (501) staff       (20)      222 2024-05-09 10:05:58.000000 cheatshh-1.0.2/src/run_cheatshh.py
+drwxr-xr-x   0 anirudhgupta   (501) staff       (20)        0 2024-05-09 08:14:30.067656 cheatshh-1.1.0/
+-rw-r--r--   0 anirudhgupta   (501) staff       (20)    11357 2024-05-09 07:38:12.000000 cheatshh-1.1.0/LICENSE
+-rw-r--r--   0 anirudhgupta   (501) staff       (20)     1286 2024-05-09 08:14:30.067453 cheatshh-1.1.0/PKG-INFO
+-rw-r--r--   0 anirudhgupta   (501) staff       (20)     2548 2024-05-09 07:55:28.000000 cheatshh-1.1.0/README.md
+drwxr-xr-x   0 anirudhgupta   (501) staff       (20)        0 2024-05-09 08:14:30.067241 cheatshh-1.1.0/cheatshh.egg-info/
+-rw-r--r--   0 anirudhgupta   (501) staff       (20)     1286 2024-05-09 08:14:30.000000 cheatshh-1.1.0/cheatshh.egg-info/PKG-INFO
+-rw-r--r--   0 anirudhgupta   (501) staff       (20)      185 2024-05-09 08:14:30.000000 cheatshh-1.1.0/cheatshh.egg-info/SOURCES.txt
+-rw-r--r--   0 anirudhgupta   (501) staff       (20)        1 2024-05-09 08:14:30.000000 cheatshh-1.1.0/cheatshh.egg-info/dependency_links.txt
+-rw-r--r--   0 anirudhgupta   (501) staff       (20)       21 2024-05-09 08:14:30.000000 cheatshh-1.1.0/cheatshh.egg-info/requires.txt
+-rw-r--r--   0 anirudhgupta   (501) staff       (20)        8 2024-05-09 08:14:30.000000 cheatshh-1.1.0/cheatshh.egg-info/top_level.txt
+-rw-r--r--   0 anirudhgupta   (501) staff       (20)       38 2024-05-09 08:14:30.067690 cheatshh-1.1.0/setup.cfg
+-rw-r--r--   0 anirudhgupta   (501) staff       (20)     2553 2024-05-09 08:14:16.000000 cheatshh-1.1.0/setup.py
```

### Comparing `cheatshh-1.0.2/LICENSE` & `cheatshh-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cheatshh-1.0.2/PKG-INFO` & `cheatshh-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheatshh
-Version: 1.0.2
+Version: 1.1.0
 Author: Anirudh Gupta
 Keywords: cheatsheet, cheat, command-line, cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fuzzyfinder
 Requires-Dist: whiptail
 
@@ -21,14 +21,14 @@
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
 - Press Enter on a command to copy it to clipboard and exit.
 
 Visit the Github Repository for more details: https://github.com/AnirudhG07/cheatshh
 
 # Version
-1.0.2
+1.1.0
 
 ## Note:
 - This package is best used in Unix based systems, like linux and MacOS. For Windows, see the github repository for more details.
-- The package is installed in ~/.config/cheatshh directory.
+- The package is installed in ~/.local/bin/cheatshh, so make sure to add this to your PATH variable.
```

### Comparing `cheatshh-1.0.2/README.md` & `cheatshh-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cheatshh-1.0.2/cheatshh.egg-info/PKG-INFO` & `cheatshh-1.1.0/cheatshh.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheatshh
-Version: 1.0.2
+Version: 1.1.0
 Author: Anirudh Gupta
 Keywords: cheatsheet, cheat, command-line, cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fuzzyfinder
 Requires-Dist: whiptail
 
@@ -21,14 +21,14 @@
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
 - Press Enter on a command to copy it to clipboard and exit.
 
 Visit the Github Repository for more details: https://github.com/AnirudhG07/cheatshh
 
 # Version
-1.0.2
+1.1.0
 
 ## Note:
 - This package is best used in Unix based systems, like linux and MacOS. For Windows, see the github repository for more details.
-- The package is installed in ~/.config/cheatshh directory.
+- The package is installed in ~/.local/bin/cheatshh, so make sure to add this to your PATH variable.
```

### Comparing `cheatshh-1.0.2/setup.py` & `cheatshh-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 import os
-import shutil, subprocess
-from setuptools import setup, find_packages
-from setuptools.command.install import install
-
-class CustomInstallCommand(install):
-    def run(self):
-        install.run(self)  # Run standard install logic
-        post_install()
+import shutil
+from setuptools import setup
 
 def install_man_page():
     source_path = os.path.join('docs', 'man', 'cheatshh.1')
-    dest_path = os.path.join('/usr/local/','share', 'man', 'man1', 'cheatshh.1')
-    os.makedirs(os.path.dirname(dest_path), exist_ok=True)
-    try:
-        shutil.copy(source_path, dest_path)
-    except PermissionError:
-        print("Permission denied. Please run this script as root for man pages.")
+    dest_path = os.path.join('share', 'man', 'man1', 'cheatshh.1')
+    shutil.copy(source_path, dest_path)
 
+def install_tldr_page():
+    source_path = os.path.join('docs', 'tldr', 'cheatshh.md')
+    dest_path = os.path.join('share', 'tldr', 'pages', 'cheatshh.md')
+    shutil.copy(source_path, dest_path)
 
 def post_install():
     install_man_page()
+    install_tldr_page()
     # Define the path to ~/.config/cheatshh
     config_dir = os.path.expanduser("~/.config/cheatshh")
 
     # Create ~/.config/cheatshh directory if it doesn't exist
     os.makedirs(config_dir, exist_ok=True)
 
     # Copy files to ~/.config/cheatshh
-    files_to_copy = ["cheats.sh", "commands.json", "groups.json", "README.md", "requirements.txt"]
+    files_to_copy = ["cheats.sh", "commands.json", "groups.json"]
     for file_name in files_to_copy:
         with open(file_name, "rb") as src:
             with open(os.path.join(config_dir, file_name), "wb") as dest:
                 dest.write(src.read())
 
-def run_cheatshh():
-    subprocess.run(['bash', '~/.config/cheatshh/cheats.sh'])
+    # Create a symbolic link to cheats.sh in ~/.local/bin
+    os.symlink(
+        os.path.join(config_dir, "cheats.sh"),
+        os.path.expanduser("~/.local/bin/cheatshh"),
+    )
 
 
-setup(name="cheatshh", version="1.0.2", cmdclass={"install": CustomInstallCommand}, 
-    long_description="""
+setup(name="cheatshh", version="1.1.0", cmdclass={"install": post_install}, 
+      long_description="""
 # cheatshh
 
 Cheatshh is an interactive CLI meant for managing command line cheatshheets. Now you don't have to remember CLI commands and just refer your cheatshhet. You can group commands and view their TLDR and MAN pages along with a custom description for the command.
 
 # Features
 
 - Comprehensive cheatsheets for various command-line utilities and tools.
@@ -51,27 +49,21 @@
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
 - Press Enter on a command to copy it to clipboard and exit.
 
 Visit the Github Repository for more details: https://github.com/AnirudhG07/cheatshh
 
 # Version
-1.0.2
+1.1.0
 
 ## Note:
 - This package is best used in Unix based systems, like linux and MacOS. For Windows, see the github repository for more details.
-- The package is installed in ~/.config/cheatshh directory.
+- The package is installed in ~/.local/bin/cheatshh, so make sure to add this to your PATH variable.
 
 
 """,
-    long_description_content_type="text/markdown",
-    keywords=["cheatsheet, cheat, command-line, cli"],
-    install_requires=["fuzzyfinder", "whiptail"],
-    author="Anirudh Gupta",
-    packages=find_packages(),
-    entry_points={
-        'console_scripts': [
-            'cheatshh=src.run_cheatshh:main',
-        ],
-    },
+      long_description_content_type="text/markdown",
+      keywords=["cheatsheet, cheat, command-line, cli"],
+      install_requires=["fuzzyfinder", "whiptail"],
+      author="Anirudh Gupta"
 )
```

