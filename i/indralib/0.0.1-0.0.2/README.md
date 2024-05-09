# Comparing `tmp/indralib-0.0.1.tar.gz` & `tmp/indralib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indralib-0.0.1.tar", last modified: Thu May  9 10:45:06 2024, max compression
+gzip compressed data, was "indralib-0.0.2.tar", last modified: Thu May  9 14:15:59 2024, max compression
```

## Comparing `indralib-0.0.1.tar` & `indralib-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 10:45:06.936213 indralib-0.0.1/
--rw-r--r--   0 dsc        (501) staff       (20)      541 2024-05-09 10:45:06.935967 indralib-0.0.1/PKG-INFO
--rw-r--r--   0 dsc        (501) staff       (20)      632 2024-05-09 10:35:17.000000 indralib-0.0.1/pyproject.toml
--rw-r--r--   0 dsc        (501) staff       (20)       38 2024-05-09 10:45:06.936282 indralib-0.0.1/setup.cfg
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 10:45:06.934878 indralib-0.0.1/src/
--rw-r--r--   0 dsc        (501) staff       (20)    23168 2024-02-14 14:23:50.000000 indralib-0.0.1/src/indra_client.py
--rw-r--r--   0 dsc        (501) staff       (20)    17744 2024-03-19 16:24:18.000000 indralib-0.0.1/src/indra_downloader.py
--rw-r--r--   0 dsc        (501) staff       (20)     3221 2024-03-15 13:14:27.000000 indralib-0.0.1/src/indra_event.py
--rw-r--r--   0 dsc        (501) staff       (20)     2711 2024-01-03 13:39:36.000000 indralib-0.0.1/src/indra_module.py
--rw-r--r--   0 dsc        (501) staff       (20)    13670 2024-03-16 09:35:30.000000 indralib-0.0.1/src/indra_time.py
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 10:45:06.935696 indralib-0.0.1/src/indralib.egg-info/
--rw-r--r--   0 dsc        (501) staff       (20)      541 2024-05-09 10:45:06.000000 indralib-0.0.1/src/indralib.egg-info/PKG-INFO
--rw-r--r--   0 dsc        (501) staff       (20)      259 2024-05-09 10:45:06.000000 indralib-0.0.1/src/indralib.egg-info/SOURCES.txt
--rw-r--r--   0 dsc        (501) staff       (20)        1 2024-05-09 10:45:06.000000 indralib-0.0.1/src/indralib.egg-info/dependency_links.txt
--rw-r--r--   0 dsc        (501) staff       (20)       66 2024-05-09 10:45:06.000000 indralib-0.0.1/src/indralib.egg-info/top_level.txt
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:15:59.623626 indralib-0.0.2/
+-rw-r--r--   0 dsc        (501) staff       (20)      541 2024-05-09 14:15:59.623392 indralib-0.0.2/PKG-INFO
+-rw-r--r--   0 dsc        (501) staff       (20)      632 2024-05-09 14:14:56.000000 indralib-0.0.2/pyproject.toml
+-rw-r--r--   0 dsc        (501) staff       (20)       38 2024-05-09 14:15:59.623676 indralib-0.0.2/setup.cfg
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:15:59.622530 indralib-0.0.2/src/
+-rw-r--r--   0 dsc        (501) staff       (20)        0 2024-05-09 14:14:09.000000 indralib-0.0.2/src/__init__.py
+-rw-r--r--   0 dsc        (501) staff       (20)    23168 2024-02-14 14:23:50.000000 indralib-0.0.2/src/indra_client.py
+-rw-r--r--   0 dsc        (501) staff       (20)    17744 2024-03-19 16:24:18.000000 indralib-0.0.2/src/indra_downloader.py
+-rw-r--r--   0 dsc        (501) staff       (20)     3221 2024-03-15 13:14:27.000000 indralib-0.0.2/src/indra_event.py
+-rw-r--r--   0 dsc        (501) staff       (20)     2711 2024-01-03 13:39:36.000000 indralib-0.0.2/src/indra_module.py
+-rw-r--r--   0 dsc        (501) staff       (20)    13670 2024-03-16 09:35:30.000000 indralib-0.0.2/src/indra_time.py
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:15:59.623187 indralib-0.0.2/src/indralib.egg-info/
+-rw-r--r--   0 dsc        (501) staff       (20)      541 2024-05-09 14:15:59.000000 indralib-0.0.2/src/indralib.egg-info/PKG-INFO
+-rw-r--r--   0 dsc        (501) staff       (20)      275 2024-05-09 14:15:59.000000 indralib-0.0.2/src/indralib.egg-info/SOURCES.txt
+-rw-r--r--   0 dsc        (501) staff       (20)        1 2024-05-09 14:15:59.000000 indralib-0.0.2/src/indralib.egg-info/dependency_links.txt
+-rw-r--r--   0 dsc        (501) staff       (20)       75 2024-05-09 14:15:59.000000 indralib-0.0.2/src/indralib.egg-info/top_level.txt
```

### Comparing `indralib-0.0.1/PKG-INFO` & `indralib-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indralib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Client for the Indrajala system
 Author-email: Dominik Schlösser <dominik.schloesser@gmail.com>
 Project-URL: Homepage, https://github.com/domschl/indrajala
 Project-URL: Bug Tracker, https://github.com/domschl/indrajala/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `indralib-0.0.1/pyproject.toml` & `indralib-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "indralib"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "Dominik Schlösser", email = "dominik.schloesser@gmail.com" }]
 description = "Client for the Indrajala system"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `indralib-0.0.1/src/indra_client.py` & `indralib-0.0.2/src/indra_client.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.1/src/indra_downloader.py` & `indralib-0.0.2/src/indra_downloader.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.1/src/indra_event.py` & `indralib-0.0.2/src/indra_event.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.1/src/indra_module.py` & `indralib-0.0.2/src/indra_module.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.1/src/indra_time.py` & `indralib-0.0.2/src/indra_time.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.1/src/indralib.egg-info/PKG-INFO` & `indralib-0.0.2/src/indralib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indralib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Client for the Indrajala system
 Author-email: Dominik Schlösser <dominik.schloesser@gmail.com>
 Project-URL: Homepage, https://github.com/domschl/indrajala
 Project-URL: Bug Tracker, https://github.com/domschl/indrajala/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

