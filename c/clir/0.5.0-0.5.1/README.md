# Comparing `tmp/clir-0.5.0.tar.gz` & `tmp/clir-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clir-0.5.0.tar", max compression
+gzip compressed data, was "clir-0.5.1.tar", max compression
```

## Comparing `clir-0.5.0.tar` & `clir-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-12-18 19:17:14.571360 clir-0.5.0/LICENSE
--rw-r--r--   0        0        0      751 2023-12-18 19:17:14.571360 clir-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-12-18 19:17:14.571360 clir-0.5.0/clir/__init__.py
--rw-r--r--   0        0        0     3048 2023-12-18 19:17:14.571360 clir-0.5.0/clir/cli.py
--rw-r--r--   0        0        0        0 2023-12-18 19:17:14.571360 clir-0.5.0/clir/utils/__init__.py
--rw-r--r--   0        0        0     9260 2023-12-18 19:17:14.571360 clir-0.5.0/clir/utils/objects.py
--rw-r--r--   0        0        0      648 2023-12-18 19:17:14.571360 clir-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 clir-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-09 17:50:23.573456 clir-0.5.1/LICENSE
+-rw-r--r--   0        0        0      751 2024-05-09 17:50:23.573456 clir-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 17:50:23.573456 clir-0.5.1/clir/__init__.py
+-rw-r--r--   0        0        0     3145 2024-05-09 17:50:23.573456 clir-0.5.1/clir/cli.py
+-rw-r--r--   0        0        0     9324 2024-05-09 17:50:23.573456 clir-0.5.1/clir/command.py
+-rw-r--r--   0        0        0      668 2024-05-09 17:50:23.577456 clir-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 clir-0.5.1/PKG-INFO
```

### Comparing `clir-0.5.0/LICENSE` & `clir-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clir-0.5.0/README.md` & `clir-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `clir-0.5.0/clir/cli.py` & `clir-0.5.1/clir/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import rich_click as click
 import os
 import subprocess
 from rich.prompt import Prompt
-from clir.utils.objects import Command
-from clir.utils.objects import CommandTable
+from clir.command import Command
+from clir.command import CommandTable
 
 @click.group()
 def cli():
     pass
 
 def check_config():
     dir_path = os.path.join(os.path.expanduser('~'), '.clir')
     file_path = os.path.join(dir_path, 'commands.json')
 
     return os.path.exists(file_path)
+
 #--------------------------------------- CLI commands  -------------------------------------------------------
 
 @cli.command(help="Clir initial configuration 🛠️")
 def init():
     dir_path = os.path.join(os.path.expanduser('~'), '.clir')
     os.makedirs(dir_path, exist_ok=True)
     
     # Define the file path and name
-    file_path = os.path.join(dir_path, 'commands.json')
+    files = ['commands.json', 'credentials.json']
 
     # Check if the file already exists
-    if not os.path.exists(file_path):
-        # Create the file
-        with open(file_path, 'w') as file:
-            file.write('{}')
-
-        print(f'File "{file_path}" created successfully.')
-    else:
-        print(f'A clir environment already exists in "{dir_path}".')
+    for file in files:
+        file_path = os.path.join(dir_path, file)
+        if not os.path.exists(file_path):
+            # Create the file
+            with open(file_path, 'w') as file_object:
+                file_object.write('{}')
+
+            print(f'File "{file_path}" created successfully.')
+        else:
+            print(f'A clir environment already exists in "{dir_path}".')
 
 @cli.command(help="Save new command 💾")
 @click.option('-c', '--command', help="Command to be saved", prompt=True)
 @click.option('-d', '--description', help="Description of the command", prompt=True)
 @click.option('-t', '--tag', help="Tag to be associated with the command", prompt=True)
 def new(command, description, tag):
     if not check_config():
```

### Comparing `clir-0.5.0/clir/utils/objects.py` & `clir-0.5.1/clir/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         for c in current_commands:
             if current_commands[c]["uid"] == uid:
                 command = c
         
         command = _replace_arguments(command)
         if uid and command:
             print(f'[bold green]Running command:[/bold green] {command}')
-            os.system(command)
+            subprocess.Popen(['bash', '-ic', 'set -o history; history -s "$1"', '_', command])
     
     def copy_command(self):
         current_commands = self.commands
 
         uid = self.get_command_uid()
         
         command = ""
```

### Comparing `clir-0.5.0/pyproject.toml` & `clir-0.5.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "clir"
-version = "0.5.0"
+version = "0.5.1"
 description = "A clear and fast way to store and recover your commands"
 authors = ["Elkin Aguas <elkinaguas@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/elkinaguas/clir"
 repository = "https://github.com/elkinaguas/clir"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/elkinaguas/clir/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 rich = "^13.5.2"
 click = "^8.1.7"
 rich-click = "^1.7.0"
+textual = "^0.47.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 clir = "clir.cli:cli"
```

### Comparing `clir-0.5.0/PKG-INFO` & `clir-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: clir
-Version: 0.5.0
+Version: 0.5.1
 Summary: A clear and fast way to store and recover your commands
 Home-page: https://github.com/elkinaguas/clir
 License: MIT
 Author: Elkin Aguas
 Author-email: elkinaguas@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: rich (>=13.5.2,<14.0.0)
 Requires-Dist: rich-click (>=1.7.0,<2.0.0)
+Requires-Dist: textual (>=0.47.1,<0.48.0)
 Project-URL: Bug Tracker, https://github.com/elkinaguas/clir/issues
 Project-URL: Repository, https://github.com/elkinaguas/clir
 Description-Content-Type: text/markdown
 
 # clir
 [![PyPI](https://img.shields.io/pypi/v/clir)](https://github.com/elkinaguas/clir/releases) ![PyPI - Downloads](https://img.shields.io/pypi/dm/clir) ![Total Download](https://static.pepy.tech/badge/clir)
```

