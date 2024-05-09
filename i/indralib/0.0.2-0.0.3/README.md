# Comparing `tmp/indralib-0.0.2.tar.gz` & `tmp/indralib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indralib-0.0.2.tar", last modified: Thu May  9 14:15:59 2024, max compression
+gzip compressed data, was "indralib-0.0.3.tar", last modified: Thu May  9 14:19:39 2024, max compression
```

## Comparing `indralib-0.0.2.tar` & `indralib-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:15:59.623626 indralib-0.0.2/
--rw-r--r--   0 dsc        (501) staff       (20)      541 2024-05-09 14:15:59.623392 indralib-0.0.2/PKG-INFO
--rw-r--r--   0 dsc        (501) staff       (20)      632 2024-05-09 14:14:56.000000 indralib-0.0.2/pyproject.toml
--rw-r--r--   0 dsc        (501) staff       (20)       38 2024-05-09 14:15:59.623676 indralib-0.0.2/setup.cfg
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:15:59.622530 indralib-0.0.2/src/
--rw-r--r--   0 dsc        (501) staff       (20)        0 2024-05-09 14:14:09.000000 indralib-0.0.2/src/__init__.py
--rw-r--r--   0 dsc        (501) staff       (20)    23168 2024-02-14 14:23:50.000000 indralib-0.0.2/src/indra_client.py
--rw-r--r--   0 dsc        (501) staff       (20)    17744 2024-03-19 16:24:18.000000 indralib-0.0.2/src/indra_downloader.py
--rw-r--r--   0 dsc        (501) staff       (20)     3221 2024-03-15 13:14:27.000000 indralib-0.0.2/src/indra_event.py
--rw-r--r--   0 dsc        (501) staff       (20)     2711 2024-01-03 13:39:36.000000 indralib-0.0.2/src/indra_module.py
--rw-r--r--   0 dsc        (501) staff       (20)    13670 2024-03-16 09:35:30.000000 indralib-0.0.2/src/indra_time.py
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:15:59.623187 indralib-0.0.2/src/indralib.egg-info/
--rw-r--r--   0 dsc        (501) staff       (20)      541 2024-05-09 14:15:59.000000 indralib-0.0.2/src/indralib.egg-info/PKG-INFO
--rw-r--r--   0 dsc        (501) staff       (20)      275 2024-05-09 14:15:59.000000 indralib-0.0.2/src/indralib.egg-info/SOURCES.txt
--rw-r--r--   0 dsc        (501) staff       (20)        1 2024-05-09 14:15:59.000000 indralib-0.0.2/src/indralib.egg-info/dependency_links.txt
--rw-r--r--   0 dsc        (501) staff       (20)       75 2024-05-09 14:15:59.000000 indralib-0.0.2/src/indralib.egg-info/top_level.txt
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:19:39.297176 indralib-0.0.3/
+-rw-r--r--   0 dsc        (501) staff       (20)      595 2024-05-09 14:19:39.296937 indralib-0.0.3/PKG-INFO
+-rw-r--r--   0 dsc        (501) staff       (20)       52 2024-05-09 14:18:10.000000 indralib-0.0.3/README.md
+-rw-r--r--   0 dsc        (501) staff       (20)      632 2024-05-09 14:18:21.000000 indralib-0.0.3/pyproject.toml
+-rw-r--r--   0 dsc        (501) staff       (20)       38 2024-05-09 14:19:39.297332 indralib-0.0.3/setup.cfg
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:19:39.291402 indralib-0.0.3/src/
+-rw-r--r--   0 dsc        (501) staff       (20)        0 2024-05-09 14:14:09.000000 indralib-0.0.3/src/__init__.py
+-rw-r--r--   0 dsc        (501) staff       (20)    23168 2024-02-14 14:23:50.000000 indralib-0.0.3/src/indra_client.py
+-rw-r--r--   0 dsc        (501) staff       (20)    17744 2024-03-19 16:24:18.000000 indralib-0.0.3/src/indra_downloader.py
+-rw-r--r--   0 dsc        (501) staff       (20)     3221 2024-03-15 13:14:27.000000 indralib-0.0.3/src/indra_event.py
+-rw-r--r--   0 dsc        (501) staff       (20)     2711 2024-01-03 13:39:36.000000 indralib-0.0.3/src/indra_module.py
+-rw-r--r--   0 dsc        (501) staff       (20)    13670 2024-03-16 09:35:30.000000 indralib-0.0.3/src/indra_time.py
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-09 14:19:39.296665 indralib-0.0.3/src/indralib.egg-info/
+-rw-r--r--   0 dsc        (501) staff       (20)      595 2024-05-09 14:19:39.000000 indralib-0.0.3/src/indralib.egg-info/PKG-INFO
+-rw-r--r--   0 dsc        (501) staff       (20)      285 2024-05-09 14:19:39.000000 indralib-0.0.3/src/indralib.egg-info/SOURCES.txt
+-rw-r--r--   0 dsc        (501) staff       (20)        1 2024-05-09 14:19:39.000000 indralib-0.0.3/src/indralib.egg-info/dependency_links.txt
+-rw-r--r--   0 dsc        (501) staff       (20)       75 2024-05-09 14:19:39.000000 indralib-0.0.3/src/indralib.egg-info/top_level.txt
```

### Comparing `indralib-0.0.2/pyproject.toml` & `indralib-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "indralib"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "Dominik Schlösser", email = "dominik.schloesser@gmail.com" }]
 description = "Client for the Indrajala system"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `indralib-0.0.2/src/indra_client.py` & `indralib-0.0.3/src/indra_client.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.2/src/indra_downloader.py` & `indralib-0.0.3/src/indra_downloader.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.2/src/indra_event.py` & `indralib-0.0.3/src/indra_event.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.2/src/indra_module.py` & `indralib-0.0.3/src/indra_module.py`

 * *Files identical despite different names*

### Comparing `indralib-0.0.2/src/indra_time.py` & `indralib-0.0.3/src/indra_time.py`

 * *Files identical despite different names*

