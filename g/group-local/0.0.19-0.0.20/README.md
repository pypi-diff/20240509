# Comparing `tmp/group_local-0.0.19.tar.gz` & `tmp/group_local-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "group_local-0.0.19.tar", last modified: Thu May  9 11:37:26 2024, max compression
+gzip compressed data, was "group_local-0.0.20.tar", last modified: Thu May  9 11:43:10 2024, max compression
```

## Comparing `group_local-0.0.19.tar` & `group_local-0.0.20.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:37:26.251609 group_local-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 11:37:26.251609 group_local-0.0.19/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:37:26.247609 group_local-0.0.19/group_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:37:26.247609 group_local-0.0.19/group_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:37:05.000000 group_local-0.0.19/group_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-09 11:37:05.000000 group_local-0.0.19/group_local/src/group_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-09 11:37:05.000000 group_local-0.0.19/group_local/src/group_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:37:26.247609 group_local-0.0.19/group_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 11:37:26.000000 group_local-0.0.19/group_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-09 11:37:26.000000 group_local-0.0.19/group_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:37:26.000000 group_local-0.0.19/group_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 11:37:26.000000 group_local-0.0.19/group_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 11:37:26.000000 group_local-0.0.19/group_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-09 11:37:05.000000 group_local-0.0.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:37:26.251609 group_local-0.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-09 11:37:05.000000 group_local-0.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:43:10.888275 group_local-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 11:43:10.888275 group_local-0.0.20/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:43:10.888275 group_local-0.0.20/group_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:43:10.888275 group_local-0.0.20/group_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:42:50.000000 group_local-0.0.20/group_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-09 11:42:50.000000 group_local-0.0.20/group_local/src/group_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-09 11:42:50.000000 group_local-0.0.20/group_local/src/group_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:43:10.888275 group_local-0.0.20/group_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 11:43:10.000000 group_local-0.0.20/group_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-09 11:43:10.000000 group_local-0.0.20/group_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:43:10.000000 group_local-0.0.20/group_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 11:43:10.000000 group_local-0.0.20/group_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 11:43:10.000000 group_local-0.0.20/group_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-09 11:42:50.000000 group_local-0.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:43:10.888275 group_local-0.0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-09 11:42:50.000000 group_local-0.0.20/setup.py
```

### Comparing `group_local-0.0.19/PKG-INFO` & `group_local-0.0.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.19
+Version: 0.0.20
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `group_local-0.0.19/group_local/src/group_local.py` & `group_local-0.0.20/group_local/src/group_local.py`

 * *Files identical despite different names*

### Comparing `group_local-0.0.19/group_local/src/group_local_constants.py` & `group_local-0.0.20/group_local/src/group_local_constants.py`

 * *Files identical despite different names*

### Comparing `group_local-0.0.19/group_local.egg-info/PKG-INFO` & `group_local-0.0.20/group_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.19
+Version: 0.0.20
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `group_local-0.0.19/setup.py` & `group_local-0.0.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "group-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/group-local
-    version='0.0.19',
+    version='0.0.20',
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles group-local Python",
     long_description="PyPI Package for Circles group-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/group-main-local-python-package",
     packages=[package_dir],
```

