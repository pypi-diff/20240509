# Comparing `tmp/darklock-0.1.3.tar.gz` & `tmp/darklock-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darklock-0.1.3.tar", last modified: Wed May  8 18:16:28 2024, max compression
+gzip compressed data, was "darklock-0.1.4.tar", last modified: Thu May  9 14:05:46 2024, max compression
```

## Comparing `darklock-0.1.3.tar` & `darklock-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:28.422464 darklock-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 18:16:24.000000 darklock-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 18:16:28.422464 darklock-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-08 18:16:24.000000 darklock-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:16:28.422464 darklock-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-08 18:16:24.000000 darklock-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:28.418464 darklock-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:28.418464 darklock-0.1.3/src/darklock/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-08 18:16:24.000000 darklock-0.1.3/src/darklock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-08 18:16:24.000000 darklock-0.1.3/src/darklock/log_disc_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-08 18:16:24.000000 darklock-0.1.3/src/darklock/no_internet_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-08 18:16:24.000000 darklock-0.1.3/src/darklock/restrict_network_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-08 18:16:24.000000 darklock-0.1.3/src/darklock/restrict_os_access.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-08 18:16:24.000000 darklock-0.1.3/src/darklock/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:28.422464 darklock-0.1.3/src/darklock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 18:16:28.000000 darklock-0.1.3/src/darklock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-08 18:16:28.000000 darklock-0.1.3/src/darklock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:16:28.000000 darklock-0.1.3/src/darklock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 18:16:28.000000 darklock-0.1.3/src/darklock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:28.422464 darklock-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-08 18:16:24.000000 darklock-0.1.3/tests/test_no_internet_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 18:16:24.000000 darklock-0.1.3/tests/test_restrict_internet_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-08 18:16:24.000000 darklock-0.1.3/tests/test_restrict_os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:05:46.840265 darklock-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 14:05:42.000000 darklock-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-09 14:05:46.840265 darklock-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-09 14:05:42.000000 darklock-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:05:46.840265 darklock-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-09 14:05:42.000000 darklock-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:05:46.836265 darklock-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:05:46.840265 darklock-0.1.4/src/darklock/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-09 14:05:42.000000 darklock-0.1.4/src/darklock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-09 14:05:42.000000 darklock-0.1.4/src/darklock/log_disc_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-09 14:05:42.000000 darklock-0.1.4/src/darklock/no_internet_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-09 14:05:42.000000 darklock-0.1.4/src/darklock/restrict_network_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-05-09 14:05:42.000000 darklock-0.1.4/src/darklock/restrict_os_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-09 14:05:42.000000 darklock-0.1.4/src/darklock/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:05:46.840265 darklock-0.1.4/src/darklock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-09 14:05:46.000000 darklock-0.1.4/src/darklock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-09 14:05:46.000000 darklock-0.1.4/src/darklock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:05:46.000000 darklock-0.1.4/src/darklock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 14:05:46.000000 darklock-0.1.4/src/darklock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:05:46.840265 darklock-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-09 14:05:42.000000 darklock-0.1.4/tests/test_no_internet_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-09 14:05:42.000000 darklock-0.1.4/tests/test_restrict_internet_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-09 14:05:42.000000 darklock-0.1.4/tests/test_restrict_os.py
```

### Comparing `darklock-0.1.3/LICENSE` & `darklock-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `darklock-0.1.3/PKG-INFO` & `darklock-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darklock
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/Capsize-Games/darklock
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `darklock-0.1.3/README.md` & `darklock-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `darklock-0.1.3/setup.py` & `darklock-0.1.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="darklock",
-    version="0.1.3",
+    version="0.1.4",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
```

### Comparing `darklock-0.1.3/src/darklock/__init__.py` & `darklock-0.1.4/src/darklock/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 os = RestrictOSAccess()
 
 def activate(
     whitelisted_operations: list = None,
     whitelisted_filenames: list = None,
     whitelisted_imports: list = None,
     blacklisted_filenames: list = None,
+    whitelisted_directories: list = None,
 ):
     # network.activate(
     #     allowed_port=4222
     # )
     os.activate(
         whitelisted_operations,
         whitelisted_filenames,
         whitelisted_imports,
         blacklisted_filenames,
+        whitelisted_directories,
     )
 
 def deactivate():
     network.deactivate()
     os.deactivate()
```

### Comparing `darklock-0.1.3/src/darklock/no_internet_socket.py` & `darklock-0.1.4/src/darklock/no_internet_socket.py`

 * *Files identical despite different names*

### Comparing `darklock-0.1.3/src/darklock/restrict_network_access.py` & `darklock-0.1.4/src/darklock/restrict_network_access.py`

 * *Files identical despite different names*

### Comparing `darklock-0.1.3/src/darklock/restrict_os_access.py` & `darklock-0.1.4/src/darklock/restrict_os_access.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,99 @@
 from darklock.singleton import Singleton
 from darklock.log_disc_writer import LogDiscWriter
 import builtins
 import re
 import os
 import sys
 import traceback
+import logging
 
 
 class RestrictOSAccess(metaclass=Singleton):
     def __init__(self):
         self.original_open = None
         self.original_import = None
         self.logging_importer = None
         self.original_os_write = None
         self.original_makedirs = None
 
         self.whitelisted_operations = [] # [('open', '/dev/null')]
         self.whitelisted_filenames = []
         self.whitelisted_imports = []
         self.blacklisted_filenames = []
+        self.whitelisted_directories = []
+
+        self.logger = logging.getLogger(__name__)
+        self.logger.setLevel(logging.DEBUG)
+        self.logger.addHandler(logging.StreamHandler())
+
+    def is_directory_whitelisted(self, directory: str) -> bool:
+        print("IS DIRECTORY WHITELISTED")
+        print(directory)
+        print(self.whitelisted_directories)
+        return directory in self.whitelisted_directories
 
     def restrict_os_write(self, *args, **kwargs):
         return self.original_os_write(*args, **kwargs)
 
     def restricted_open(self, *args, **kwargs):
-        if ('open', args[0]) in self.whitelisted_operations or self.check_stack_trace():
+        if (
+            self.is_directory_whitelisted(args[0]) or
+            'open' in self.whitelisted_operations or self.check_stack_trace()
+        ):
             return self.original_open(*args, **kwargs)
-        raise PermissionError("File system operations are not allowed")
+        self.logger.error("File system operations are not allowed")
 
     def restricted_os_makedirs(self, *args, **kwargs):
-        if ('makedirs', args[0]) in self.whitelisted_operations or self.check_stack_trace():
+        if (
+            self.is_directory_whitelisted(args[0]) or
+            'makedirs' in self.whitelisted_operations or self.check_stack_trace()
+        ):
             return self.original_makedirs(*args, **kwargs)
-        #raise PermissionError("File system operations are not allowed")
-
-    def restricted_open(self, *args, **kwargs):
-        if ('open', args[0]) in self.whitelisted_operations or self.check_stack_trace():
-            return self.original_open(*args, **kwargs)
-        raise PermissionError("File system operations are not allowed")
+        self.logger.error(f"File system operations are not allowed. Attempted to create directory: {args}")
 
     def restricted_exec(self, *args, **kwargs):
-        raise PermissionError("System calls are not allowed")
+        if (
+            self.is_directory_whitelisted(args[0]) or
+            'exec' in self.whitelisted_operations or self.check_stack_trace()
+        ):
+            return os.exec(*args, **kwargs)
+        self.logger.error("System calls are not allowed")
 
     def restricted_subprocess(self, *args, **kwargs):
-        raise PermissionError("Subprocess invocations are not allowed")
+        if (
+            self.is_directory_whitelisted(args[0]) or
+            'subprocess' in self.whitelisted_operations or self.check_stack_trace()
+        ):
+            return os.system(*args, **kwargs)
+        self.logger.error("Subprocess invocations are not allowed")
 
     def restricted_import(self, name, *args, **kwargs):
+        if 'import' in self.whitelisted_operations or self.check_stack_trace():
+            return self.original_import(name, *args, **kwargs)
         if any(re.search(pattern, name) for pattern in self.whitelisted_imports):
             return self.original_import(name, *args, **kwargs)
         print(f"Failed to import: {name}")
-        raise PermissionError("Importing modules is not allowed")
+        self.logger.error("Importing modules is not allowed")
 
     def log_imports(self, name, *args, **kwargs):
         #self.logging_importer = LoggingImporter()
         sys.meta_path.insert(0, self.logging_importer)
 
     def restricted_module(self, *args, **kwargs):
-        raise PermissionError("Module operations are not allowed")
+        self.logger.error("Module operations are not allowed")
 
     def restricted_os(self, *args, **kwargs):
-        raise PermissionError("OS operations are not allowed")
+        self.logger.error("OS operations are not allowed")
 
     def restricted_sys(self, *args, **kwargs):
-        raise PermissionError("System operations are not allowed")
+        self.logger.error("System operations are not allowed")
 
     def restricted_socket(self, *args, **kwargs):
-        raise PermissionError("Socket operations are not allowed")
+        self.logger.error("Socket operations are not allowed")
 
     def check_stack_trace(self) -> bool:
         stack_trace = traceback.extract_stack()
         # Add more logic here to check the stack trace
         # and allow certain operations
         # from specific chains.
         res = False
@@ -86,24 +111,32 @@
 
     def activate(
         self,
         whitelisted_operations: list = None,
         whitelisted_filenames: list = None,
         whitelisted_imports: list = None,
         blacklisted_filenames: list = None,
+        whitelisted_directories: list = None,
     ):
         """
         Install restrictions on OS access.
         :return:
         """
         self.whitelisted_operations = whitelisted_operations or []
         self.whitelisted_filenames = whitelisted_filenames or []
         self.whitelisted_imports = whitelisted_imports or []
         self.blacklisted_filenames = blacklisted_filenames or []
 
+        whitelisted_directories = whitelisted_directories or []
+        parsed_directories = []
+        for directory in whitelisted_directories:
+            parsed_directories.append(os.path.expanduser(directory))
+        self.whitelisted_directories = parsed_directories
+
+
         self.original_open = builtins.open
         self.original_import = builtins.__import__
         self.original_os_write = os.write
         self.original_makedirs = os.makedirs
 
         os.makedirs = self.restricted_os_makedirs
```

### Comparing `darklock-0.1.3/src/darklock.egg-info/PKG-INFO` & `darklock-0.1.4/src/darklock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darklock
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/Capsize-Games/darklock
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `darklock-0.1.3/tests/test_restrict_internet_access.py` & `darklock-0.1.4/tests/test_restrict_internet_access.py`

 * *Files identical despite different names*

### Comparing `darklock-0.1.3/tests/test_restrict_os.py` & `darklock-0.1.4/tests/test_restrict_os.py`

 * *Files identical despite different names*

