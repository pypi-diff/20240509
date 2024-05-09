# Comparing `tmp/defendatron-0.1.5.tar.gz` & `tmp/defendatron-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defendatron-0.1.5.tar", last modified: Wed May  8 18:16:53 2024, max compression
+gzip compressed data, was "defendatron-0.1.6.tar", last modified: Wed May  8 18:19:56 2024, max compression
```

## Comparing `defendatron-0.1.5.tar` & `defendatron-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:53.598393 defendatron-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 18:16:49.000000 defendatron-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-08 18:16:53.598393 defendatron-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-08 18:16:49.000000 defendatron-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:16:53.598393 defendatron-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-08 18:16:49.000000 defendatron-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:53.598393 defendatron-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:53.598393 defendatron-0.1.5/src/defendatron/
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-08 18:16:49.000000 defendatron-0.1.5/src/defendatron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-08 18:16:49.000000 defendatron-0.1.5/src/defendatron/nullscream_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:53.598393 defendatron-0.1.5/src/defendatron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-08 18:16:53.000000 defendatron-0.1.5/src/defendatron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 18:16:53.000000 defendatron-0.1.5/src/defendatron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:16:53.000000 defendatron-0.1.5/src/defendatron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 18:16:53.000000 defendatron-0.1.5/src/defendatron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 18:16:53.000000 defendatron-0.1.5/src/defendatron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:19:56.177954 defendatron-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 18:19:51.000000 defendatron-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-08 18:19:56.177954 defendatron-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-08 18:19:51.000000 defendatron-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:19:56.177954 defendatron-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-08 18:19:51.000000 defendatron-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:19:56.173954 defendatron-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:19:56.177954 defendatron-0.1.6/src/defendatron/
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-08 18:19:51.000000 defendatron-0.1.6/src/defendatron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-08 18:19:51.000000 defendatron-0.1.6/src/defendatron/nullscream_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:19:56.177954 defendatron-0.1.6/src/defendatron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-08 18:19:56.000000 defendatron-0.1.6/src/defendatron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 18:19:56.000000 defendatron-0.1.6/src/defendatron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:19:56.000000 defendatron-0.1.6/src/defendatron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 18:19:56.000000 defendatron-0.1.6/src/defendatron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 18:19:56.000000 defendatron-0.1.6/src/defendatron.egg-info/top_level.txt
```

### Comparing `defendatron-0.1.5/LICENSE` & `defendatron-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `defendatron-0.1.5/PKG-INFO` & `defendatron-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: defendatron
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://github.com/Capsize-Games/defendatron
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nullscream==0.1.3
-Requires-Dist: darklock==0.1.2
+Requires-Dist: darklock==0.1.3
 Requires-Dist: shadowlogger==0.1.1
 
 # Defendatron
 
 Defendatron is a simple coordinator for `Protectabots`, Python modules that provide security features for your applications.
 
 ---
```

### Comparing `defendatron-0.1.5/README.md` & `defendatron-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `defendatron-0.1.5/setup.py` & `defendatron-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="defendatron",
-    version="0.1.5",
+    version="0.1.6",
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
-        "darklock==0.1.2",
+        "darklock==0.1.3",
         "shadowlogger==0.1.1",
     ],
     dependency_links=[
     ],
 )
```

### Comparing `defendatron-0.1.5/src/defendatron/__init__.py` & `defendatron-0.1.6/src/defendatron/__init__.py`

 * *Files identical despite different names*

### Comparing `defendatron-0.1.5/src/defendatron/nullscream_tracker.py` & `defendatron-0.1.6/src/defendatron/nullscream_tracker.py`

 * *Files identical despite different names*

### Comparing `defendatron-0.1.5/src/defendatron.egg-info/PKG-INFO` & `defendatron-0.1.6/src/defendatron.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: defendatron
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://github.com/Capsize-Games/defendatron
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nullscream==0.1.3
-Requires-Dist: darklock==0.1.2
+Requires-Dist: darklock==0.1.3
 Requires-Dist: shadowlogger==0.1.1
 
 # Defendatron
 
 Defendatron is a simple coordinator for `Protectabots`, Python modules that provide security features for your applications.
 
 ---
```

