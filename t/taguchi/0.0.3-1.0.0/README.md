# Comparing `tmp/taguchi-0.0.3.tar.gz` & `tmp/taguchi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taguchi-0.0.3.tar", last modified: Sun May  5 05:55:17 2024, max compression
+gzip compressed data, was "taguchi-1.0.0.tar", last modified: Thu May  9 03:01:09 2024, max compression
```

## Comparing `taguchi-0.0.3.tar` & `taguchi-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 05:55:17.294633 taguchi-0.0.3/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1016 2024-05-05 05:55:17.294633 taguchi-0.0.3/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      587 2024-05-04 04:32:49.000000 taguchi-0.0.3/README.md
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-0.0.3/pyproject.toml
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-05 05:55:17.298633 taguchi-0.0.3/setup.cfg
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 05:55:17.289632 taguchi-0.0.3/taguchi/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-05 05:54:34.000000 taguchi-0.0.3/taguchi/__init__.py
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1834 2024-05-05 05:54:11.000000 taguchi-0.0.3/taguchi/__main__.py
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-05 05:55:17.292632 taguchi-0.0.3/taguchi.egg-info/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1016 2024-05-05 05:55:17.000000 taguchi-0.0.3/taguchi.egg-info/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      262 2024-05-05 05:55:17.000000 taguchi-0.0.3/taguchi.egg-info/SOURCES.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-05 05:55:17.000000 taguchi-0.0.3/taguchi.egg-info/dependency_links.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-05 05:55:17.000000 taguchi-0.0.3/taguchi.egg-info/entry_points.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-0.0.3/taguchi.egg-info/not-zip-safe
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-05 05:55:17.000000 taguchi-0.0.3/taguchi.egg-info/top_level.txt
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-09 03:01:09.253557 taguchi-1.0.0/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1016 2024-05-09 03:01:09.252557 taguchi-1.0.0/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      587 2024-05-04 04:32:49.000000 taguchi-1.0.0/README.md
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-1.0.0/pyproject.toml
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-09 03:01:09.255557 taguchi-1.0.0/setup.cfg
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-09 03:01:09.250557 taguchi-1.0.0/taguchi/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-09 02:43:51.000000 taguchi-1.0.0/taguchi/__init__.py
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     2648 2024-05-09 02:59:55.000000 taguchi-1.0.0/taguchi/__main__.py
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-09 03:01:09.252557 taguchi-1.0.0/taguchi.egg-info/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1016 2024-05-09 03:01:09.000000 taguchi-1.0.0/taguchi.egg-info/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      262 2024-05-09 03:01:09.000000 taguchi-1.0.0/taguchi.egg-info/SOURCES.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-09 03:01:09.000000 taguchi-1.0.0/taguchi.egg-info/dependency_links.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-09 03:01:09.000000 taguchi-1.0.0/taguchi.egg-info/entry_points.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-1.0.0/taguchi.egg-info/not-zip-safe
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-09 03:01:09.000000 taguchi-1.0.0/taguchi.egg-info/top_level.txt
```

### Comparing `taguchi-0.0.3/PKG-INFO` & `taguchi-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taguchi
-Version: 0.0.3
+Version: 1.0.0
 Summary: A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 Home-page: https://github.com/jcranney/taguchi
 Author: Jesse Cranney
 Author-email: jesse.cranney@anu.edu.au
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `taguchi-0.0.3/README.md` & `taguchi-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `taguchi-0.0.3/setup.cfg` & `taguchi-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `taguchi-0.0.3/taguchi.egg-info/PKG-INFO` & `taguchi-1.0.0/taguchi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taguchi
-Version: 0.0.3
+Version: 1.0.0
 Summary: A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 Home-page: https://github.com/jcranney/taguchi
 Author: Jesse Cranney
 Author-email: jesse.cranney@anu.edu.au
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

