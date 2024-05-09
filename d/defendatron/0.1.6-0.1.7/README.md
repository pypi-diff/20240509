# Comparing `tmp/defendatron-0.1.6.tar.gz` & `tmp/defendatron-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defendatron-0.1.6.tar", last modified: Wed May  8 18:19:56 2024, max compression
+gzip compressed data, was "defendatron-0.1.7.tar", last modified: Thu May  9 14:06:48 2024, max compression
```

## Comparing `defendatron-0.1.6.tar` & `defendatron-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:19:56.177954 defendatron-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 18:19:51.000000 defendatron-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-08 18:19:56.177954 defendatron-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-08 18:19:51.000000 defendatron-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:19:56.177954 defendatron-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-08 18:19:51.000000 defendatron-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:19:56.173954 defendatron-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:19:56.177954 defendatron-0.1.6/src/defendatron/
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-08 18:19:51.000000 defendatron-0.1.6/src/defendatron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-08 18:19:51.000000 defendatron-0.1.6/src/defendatron/nullscream_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:19:56.177954 defendatron-0.1.6/src/defendatron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-08 18:19:56.000000 defendatron-0.1.6/src/defendatron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 18:19:56.000000 defendatron-0.1.6/src/defendatron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:19:56.000000 defendatron-0.1.6/src/defendatron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 18:19:56.000000 defendatron-0.1.6/src/defendatron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 18:19:56.000000 defendatron-0.1.6/src/defendatron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:06:48.809482 defendatron-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 14:06:42.000000 defendatron-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-09 14:06:48.809482 defendatron-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-09 14:06:42.000000 defendatron-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:06:48.809482 defendatron-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-09 14:06:42.000000 defendatron-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:06:48.805482 defendatron-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:06:48.805482 defendatron-0.1.7/src/defendatron/
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-09 14:06:42.000000 defendatron-0.1.7/src/defendatron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-09 14:06:42.000000 defendatron-0.1.7/src/defendatron/nullscream_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:06:48.809482 defendatron-0.1.7/src/defendatron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-09 14:06:48.000000 defendatron-0.1.7/src/defendatron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 14:06:48.000000 defendatron-0.1.7/src/defendatron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:06:48.000000 defendatron-0.1.7/src/defendatron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 14:06:48.000000 defendatron-0.1.7/src/defendatron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 14:06:48.000000 defendatron-0.1.7/src/defendatron.egg-info/top_level.txt
```

### Comparing `defendatron-0.1.6/LICENSE` & `defendatron-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `defendatron-0.1.6/PKG-INFO` & `defendatron-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: defendatron
-Version: 0.1.6
+Version: 0.1.7
 Home-page: https://github.com/Capsize-Games/defendatron
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nullscream==0.1.3
-Requires-Dist: darklock==0.1.3
+Requires-Dist: darklock==0.1.4
 Requires-Dist: shadowlogger==0.1.1
 
 # Defendatron
 
 Defendatron is a simple coordinator for `Protectabots`, Python modules that provide security features for your applications.
 
 ---
```

### Comparing `defendatron-0.1.6/README.md` & `defendatron-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `defendatron-0.1.6/setup.py` & `defendatron-0.1.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="defendatron",
-    version="0.1.6",
+    version="0.1.7",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
     url="https://github.com/Capsize-Games/defendatron",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
         "nullscream==0.1.3",
-        "darklock==0.1.3",
+        "darklock==0.1.4",
         "shadowlogger==0.1.1",
     ],
     dependency_links=[
     ],
 )
```

### Comparing `defendatron-0.1.6/src/defendatron/__init__.py` & `defendatron-0.1.7/src/defendatron/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     nullscream_function_blacklist: list = None,
 
     # darklock properites
     darklock_os_whitelisted_operations: list = None,
     darklock_os_whitelisted_filenames: list = None,
     darklock_os_whitelisted_imports: list = None,
     darklock_os_blacklisted_filenames: list = None,
+    darklock_os_whitelisted_directories: list = None,
 
     activate_shadowlogger: bool = False,
     activate_darklock: bool = False,
     activate_nullscream: bool = False,
 
     # Shadowlogger properties
     show_stdout: bool = True
@@ -41,14 +42,15 @@
     if activate_darklock:
         logger.info("Activating darklock")
         darklock.activate(
             whitelisted_operations=darklock_os_whitelisted_operations,
             whitelisted_filenames=darklock_os_whitelisted_filenames,
             whitelisted_imports=darklock_os_whitelisted_imports,
             blacklisted_filenames=darklock_os_blacklisted_filenames,
+            whitelisted_directories=darklock_os_whitelisted_directories,
         )
 
     if activate_nullscream:
         logger.info("Activating nullscream")
         nullscream.activate(
             blacklist=nullscream_blacklist,
             whitelist=nullscream_whitelist,
```

### Comparing `defendatron-0.1.6/src/defendatron/nullscream_tracker.py` & `defendatron-0.1.7/src/defendatron/nullscream_tracker.py`

 * *Files identical despite different names*

### Comparing `defendatron-0.1.6/src/defendatron.egg-info/PKG-INFO` & `defendatron-0.1.7/src/defendatron.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: defendatron
-Version: 0.1.6
+Version: 0.1.7
 Home-page: https://github.com/Capsize-Games/defendatron
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nullscream==0.1.3
-Requires-Dist: darklock==0.1.3
+Requires-Dist: darklock==0.1.4
 Requires-Dist: shadowlogger==0.1.1
 
 # Defendatron
 
 Defendatron is a simple coordinator for `Protectabots`, Python modules that provide security features for your applications.
 
 ---
```

