# Comparing `tmp/indralib-0.0.5.tar.gz` & `tmp/indralib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indralib-0.0.5.tar", last modified: Thu May  9 14:47:22 2024, max compression
+gzip compressed data, was "indralib-0.0.6.tar", last modified: Thu May  9 15:58:59 2024, max compression
```

## Comparing `indralib-0.0.5.tar` & `indralib-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:47:22.407600 indralib-0.0.5/
--rw-r--r--   0 dsc        (501) staff       (20)      595 2024-05-09 14:47:22.407354 indralib-0.0.5/PKG-INFO
--rw-r--r--   0 dsc        (501) staff       (20)       52 2024-05-09 14:18:10.000000 indralib-0.0.5/README.md
--rw-r--r--   0 dsc        (501) staff       (20)      632 2024-05-09 14:47:04.000000 indralib-0.0.5/pyproject.toml
--rw-r--r--   0 dsc        (501) staff       (20)       38 2024-05-09 14:47:22.407650 indralib-0.0.5/setup.cfg
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:47:22.390730 indralib-0.0.5/src/
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:47:22.403130 indralib-0.0.5/src/indralib/
--rw-r--r--   0 dsc        (501) staff       (20)        0 2024-05-09 14:14:09.000000 indralib-0.0.5/src/indralib/__init__.py
--rw-r--r--   0 dsc        (501) staff       (20)    23177 2024-05-09 14:46:29.000000 indralib-0.0.5/src/indralib/indra_client.py
--rw-r--r--   0 dsc        (501) staff       (20)    17753 2024-05-09 14:46:36.000000 indralib-0.0.5/src/indralib/indra_downloader.py
--rw-r--r--   0 dsc        (501) staff       (20)     3230 2024-05-09 14:46:17.000000 indralib-0.0.5/src/indralib/indra_event.py
--rw-r--r--   0 dsc        (501) staff       (20)     2720 2024-05-09 14:46:45.000000 indralib-0.0.5/src/indralib/indra_module.py
--rw-r--r--   0 dsc        (501) staff       (20)    13670 2024-05-09 14:46:52.000000 indralib-0.0.5/src/indralib/indra_time.py
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:47:22.406572 indralib-0.0.5/src/indralib.egg-info/
--rw-r--r--   0 dsc        (501) staff       (20)      595 2024-05-09 14:47:22.000000 indralib-0.0.5/src/indralib.egg-info/PKG-INFO
--rw-r--r--   0 dsc        (501) staff       (20)      339 2024-05-09 14:47:22.000000 indralib-0.0.5/src/indralib.egg-info/SOURCES.txt
--rw-r--r--   0 dsc        (501) staff       (20)        1 2024-05-09 14:47:22.000000 indralib-0.0.5/src/indralib.egg-info/dependency_links.txt
--rw-r--r--   0 dsc        (501) staff       (20)        9 2024-05-09 14:47:22.000000 indralib-0.0.5/src/indralib.egg-info/top_level.txt
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 15:58:59.339834 indralib-0.0.6/
+-rw-r--r--   0 dsc        (501) staff       (20)      627 2024-05-09 15:58:59.339657 indralib-0.0.6/PKG-INFO
+-rw-r--r--   0 dsc        (501) staff       (20)       52 2024-05-09 14:18:10.000000 indralib-0.0.6/README.md
+-rw-r--r--   0 dsc        (501) staff       (20)      676 2024-05-09 15:57:52.000000 indralib-0.0.6/pyproject.toml
+-rw-r--r--   0 dsc        (501) staff       (20)       38 2024-05-09 15:58:59.339874 indralib-0.0.6/setup.cfg
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 15:58:59.337731 indralib-0.0.6/src/
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 15:58:59.338678 indralib-0.0.6/src/indralib/
+-rw-r--r--   0 dsc        (501) staff       (20)        0 2024-05-09 14:14:09.000000 indralib-0.0.6/src/indralib/__init__.py
+-rw-r--r--   0 dsc        (501) staff       (20)    23177 2024-05-09 14:46:29.000000 indralib-0.0.6/src/indralib/indra_client.py
+-rw-r--r--   0 dsc        (501) staff       (20)    17753 2024-05-09 14:46:36.000000 indralib-0.0.6/src/indralib/indra_downloader.py
+-rw-r--r--   0 dsc        (501) staff       (20)     3214 2024-05-09 15:30:32.000000 indralib-0.0.6/src/indralib/indra_event.py
+-rw-r--r--   0 dsc        (501) staff       (20)     2720 2024-05-09 14:46:45.000000 indralib-0.0.6/src/indralib/indra_module.py
+-rw-r--r--   0 dsc        (501) staff       (20)    13670 2024-05-09 14:46:52.000000 indralib-0.0.6/src/indralib/indra_time.py
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 15:58:59.339465 indralib-0.0.6/src/indralib.egg-info/
+-rw-r--r--   0 dsc        (501) staff       (20)      627 2024-05-09 15:58:59.000000 indralib-0.0.6/src/indralib.egg-info/PKG-INFO
+-rw-r--r--   0 dsc        (501) staff       (20)      374 2024-05-09 15:58:59.000000 indralib-0.0.6/src/indralib.egg-info/SOURCES.txt
+-rw-r--r--   0 dsc        (501) staff       (20)        1 2024-05-09 15:58:59.000000 indralib-0.0.6/src/indralib.egg-info/dependency_links.txt
+-rw-r--r--   0 dsc        (501) staff       (20)       17 2024-05-09 15:58:59.000000 indralib-0.0.6/src/indralib.egg-info/requires.txt
+-rw-r--r--   0 dsc        (501) staff       (20)        9 2024-05-09 15:58:59.000000 indralib-0.0.6/src/indralib.egg-info/top_level.txt
```

### Comparing `indralib-0.0.5/PKG-INFO` & `indralib-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: indralib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Client for the Indrajala system
 Author-email: Dominik Schlösser <dominik.schloesser@gmail.com>
 Project-URL: Homepage, https://github.com/domschl/indrajala
 Project-URL: Bug Tracker, https://github.com/domschl/indrajala/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: websockets>=12.0
 
 ## Client libraries for the Indrajala server
 
 T.B.D.
```

### Comparing `indralib-0.0.5/pyproject.toml` & `indralib-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "indralib"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{ name = "Dominik Schlösser", email = "dominik.schloesser@gmail.com" }]
 description = "Client for the Indrajala system"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
 ]
+dependencies = [
+    "websockets >=12.0",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/domschl/indrajala"
 "Bug Tracker" = "https://github.com/domschl/indrajala/issues"
```

### Comparing `indralib-0.0.5/src/indralib/indra_client.py` & `indralib-0.0.6/src/indralib/indra_client.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.5/src/indralib/indra_downloader.py` & `indralib-0.0.6/src/indralib/indra_downloader.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.5/src/indralib/indra_event.py` & `indralib-0.0.6/src/indralib/indra_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import datetime
 import uuid
-from indralib.indra_time import IndraTime  # type: ignore
+from indralib.indra_time import IndraTime
 
 
 # XXX  https://en.wikipedia.org/wiki/Decimal_time
 class IndraEvent:
     def __init__(self):
         """Create an IndraEvent json object
```

### Comparing `indralib-0.0.5/src/indralib/indra_module.py` & `indralib-0.0.6/src/indralib/indra_module.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.5/src/indralib/indra_time.py` & `indralib-0.0.6/src/indralib/indra_time.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.5/src/indralib.egg-info/PKG-INFO` & `indralib-0.0.6/src/indralib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: indralib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Client for the Indrajala system
 Author-email: Dominik Schlösser <dominik.schloesser@gmail.com>
 Project-URL: Homepage, https://github.com/domschl/indrajala
 Project-URL: Bug Tracker, https://github.com/domschl/indrajala/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: websockets>=12.0
 
 ## Client libraries for the Indrajala server
 
 T.B.D.
```

