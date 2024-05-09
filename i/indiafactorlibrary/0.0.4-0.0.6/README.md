# Comparing `tmp/indiafactorlibrary-0.0.4.tar.gz` & `tmp/indiafactorlibrary-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indiafactorlibrary-0.0.4.tar", last modified: Wed May  8 17:53:16 2024, max compression
+gzip compressed data, was "indiafactorlibrary-0.0.6.tar", last modified: Wed May  8 18:03:27 2024, max compression
```

## Comparing `indiafactorlibrary-0.0.4.tar` & `indiafactorlibrary-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:16.578992 indiafactorlibrary-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 17:53:13.000000 indiafactorlibrary-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-08 17:53:16.578992 indiafactorlibrary-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-08 17:53:13.000000 indiafactorlibrary-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:16.578992 indiafactorlibrary-0.0.4/indiafactorlibrary/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 17:53:13.000000 indiafactorlibrary-0.0.4/indiafactorlibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-08 17:53:13.000000 indiafactorlibrary-0.0.4/indiafactorlibrary/indiafactorlibrary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:16.578992 indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-08 17:53:16.000000 indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-08 17:53:16.000000 indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:53:16.000000 indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 17:53:16.000000 indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 17:53:16.000000 indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:53:16.578992 indiafactorlibrary-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-08 17:53:13.000000 indiafactorlibrary-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:03:27.614808 indiafactorlibrary-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 18:03:24.000000 indiafactorlibrary-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-08 18:03:27.614808 indiafactorlibrary-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-08 18:03:24.000000 indiafactorlibrary-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:03:27.610808 indiafactorlibrary-0.0.6/indiafactorlibrary/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 18:03:24.000000 indiafactorlibrary-0.0.6/indiafactorlibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-08 18:03:24.000000 indiafactorlibrary-0.0.6/indiafactorlibrary/indiafactorlibrary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:03:27.614808 indiafactorlibrary-0.0.6/indiafactorlibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-08 18:03:27.000000 indiafactorlibrary-0.0.6/indiafactorlibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-08 18:03:27.000000 indiafactorlibrary-0.0.6/indiafactorlibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:03:27.000000 indiafactorlibrary-0.0.6/indiafactorlibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 18:03:27.000000 indiafactorlibrary-0.0.6/indiafactorlibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 18:03:27.000000 indiafactorlibrary-0.0.6/indiafactorlibrary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:03:27.614808 indiafactorlibrary-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-08 18:03:24.000000 indiafactorlibrary-0.0.6/setup.py
```

### Comparing `indiafactorlibrary-0.0.4/LICENSE` & `indiafactorlibrary-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `indiafactorlibrary-0.0.4/PKG-INFO` & `indiafactorlibrary-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiafactorlibrary
-Version: 0.0.4
+Version: 0.0.6
 Summary: A Python library to fetch data from Invespar Factor library for Indian equities.
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `indiafactorlibrary-0.0.4/README.md` & `indiafactorlibrary-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `indiafactorlibrary-0.0.4/indiafactorlibrary/indiafactorlibrary.py` & `indiafactorlibrary-0.0.6/indiafactorlibrary/indiafactorlibrary.py`

 * *Files identical despite different names*

### Comparing `indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/PKG-INFO` & `indiafactorlibrary-0.0.6/indiafactorlibrary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiafactorlibrary
-Version: 0.0.4
+Version: 0.0.6
 Summary: A Python library to fetch data from Invespar Factor library for Indian equities.
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `indiafactorlibrary-0.0.4/setup.py` & `indiafactorlibrary-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="indiafactorlibrary",
-    version="0.0.4",
+    version="0.0.6",
     description="A Python library to fetch data from Invespar Factor library for Indian equities.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "pandas",
         "requests",
```

