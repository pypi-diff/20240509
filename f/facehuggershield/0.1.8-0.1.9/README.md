# Comparing `tmp/facehuggershield-0.1.8.tar.gz` & `tmp/facehuggershield-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facehuggershield-0.1.8.tar", last modified: Wed May  8 18:20:19 2024, max compression
+gzip compressed data, was "facehuggershield-0.1.9.tar", last modified: Thu May  9 14:08:22 2024, max compression
```

## Comparing `facehuggershield-0.1.8.tar` & `facehuggershield-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:20:19.932838 facehuggershield-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 18:20:16.000000 facehuggershield-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-08 18:20:19.932838 facehuggershield-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 18:20:16.000000 facehuggershield-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:20:19.932838 facehuggershield-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-08 18:20:16.000000 facehuggershield-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:20:19.928838 facehuggershield-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:20:19.932838 facehuggershield-0.1.8/src/facehuggershield/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 18:20:16.000000 facehuggershield-0.1.8/src/facehuggershield/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:20:19.932838 facehuggershield-0.1.8/src/facehuggershield/huggingface/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-08 18:20:16.000000 facehuggershield-0.1.8/src/facehuggershield/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-08 18:20:16.000000 facehuggershield-0.1.8/src/facehuggershield/huggingface/set_environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-05-08 18:20:16.000000 facehuggershield-0.1.8/src/facehuggershield/huggingface/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:20:19.932838 facehuggershield-0.1.8/src/facehuggershield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-08 18:20:19.000000 facehuggershield-0.1.8/src/facehuggershield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-08 18:20:19.000000 facehuggershield-0.1.8/src/facehuggershield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:20:19.000000 facehuggershield-0.1.8/src/facehuggershield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 18:20:19.000000 facehuggershield-0.1.8/src/facehuggershield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 18:20:19.000000 facehuggershield-0.1.8/src/facehuggershield.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:08:22.035441 facehuggershield-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 14:08:13.000000 facehuggershield-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-09 14:08:22.031441 facehuggershield-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-09 14:08:13.000000 facehuggershield-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:08:22.035441 facehuggershield-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-09 14:08:13.000000 facehuggershield-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:08:22.031441 facehuggershield-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:08:22.031441 facehuggershield-0.1.9/src/facehuggershield/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 14:08:13.000000 facehuggershield-0.1.9/src/facehuggershield/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:08:22.031441 facehuggershield-0.1.9/src/facehuggershield/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-09 14:08:13.000000 facehuggershield-0.1.9/src/facehuggershield/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-09 14:08:13.000000 facehuggershield-0.1.9/src/facehuggershield/huggingface/set_environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-05-09 14:08:13.000000 facehuggershield-0.1.9/src/facehuggershield/huggingface/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:08:22.031441 facehuggershield-0.1.9/src/facehuggershield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-09 14:08:22.000000 facehuggershield-0.1.9/src/facehuggershield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-09 14:08:22.000000 facehuggershield-0.1.9/src/facehuggershield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:08:22.000000 facehuggershield-0.1.9/src/facehuggershield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 14:08:22.000000 facehuggershield-0.1.9/src/facehuggershield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 14:08:22.000000 facehuggershield-0.1.9/src/facehuggershield.egg-info/top_level.txt
```

### Comparing `facehuggershield-0.1.8/LICENSE` & `facehuggershield-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `facehuggershield-0.1.8/PKG-INFO` & `facehuggershield-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: facehuggershield
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/Capsize-Games/facehuggershield
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: defendatron==0.1.6
+Requires-Dist: defendatron==0.1.7
 
 # Facehugger Shield
 
 Facehugger Shield automatically locks down operations
 for specific modules. It was designed to non-destructively restrict access
 to the Huggingface library, but can be used with any library.
```

### Comparing `facehuggershield-0.1.8/README.md` & `facehuggershield-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `facehuggershield-0.1.8/setup.py` & `facehuggershield-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="facehuggershield",
-    version="0.1.8",
+    version="0.1.9",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
     url="https://github.com/Capsize-Games/facehuggershield",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
-        "defendatron==0.1.6",
+        "defendatron==0.1.7",
     ],
     dependency_links=[
     ],
 )
```

### Comparing `facehuggershield-0.1.8/src/facehuggershield/huggingface/set_environment_variables.py` & `facehuggershield-0.1.9/src/facehuggershield/huggingface/set_environment_variables.py`

 * *Files identical despite different names*

### Comparing `facehuggershield-0.1.8/src/facehuggershield/huggingface/settings.py` & `facehuggershield-0.1.9/src/facehuggershield/huggingface/settings.py`

 * *Files identical despite different names*

### Comparing `facehuggershield-0.1.8/src/facehuggershield.egg-info/PKG-INFO` & `facehuggershield-0.1.9/src/facehuggershield.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: facehuggershield
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/Capsize-Games/facehuggershield
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: defendatron==0.1.6
+Requires-Dist: defendatron==0.1.7
 
 # Facehugger Shield
 
 Facehugger Shield automatically locks down operations
 for specific modules. It was designed to non-destructively restrict access
 to the Huggingface library, but can be used with any library.
```

