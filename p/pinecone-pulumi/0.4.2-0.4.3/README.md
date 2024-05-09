# Comparing `tmp/pinecone_pulumi-0.4.2.tar.gz` & `tmp/pinecone_pulumi-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_pulumi-0.4.2.tar", last modified: Wed Mar 27 23:28:57 2024, max compression
+gzip compressed data, was "pinecone_pulumi-0.4.3.tar", last modified: Thu May  9 21:27:06 2024, max compression
```

## Comparing `pinecone_pulumi-0.4.2.tar` & `pinecone_pulumi-0.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:28:57.650630 pinecone_pulumi-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-27 23:28:57.650630 pinecone_pulumi-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:28:57.650630 pinecone_pulumi-0.4.2/pinecone_pulumi/
--rw-------   0 runner    (1001) docker     (127)     1091 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/__init__.py
--rw-------   0 runner    (1001) docker     (127)      454 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/_enums.py
--rw-------   0 runner    (1001) docker     (127)     8997 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     9279 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:28:57.650630 pinecone_pulumi-0.4.2/pinecone_pulumi/config/
--rw-------   0 runner    (1001) docker     (127)      267 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      580 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/config/vars.py
--rw-------   0 runner    (1001) docker     (127)     4793 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/lookup_pinecone_collection.py
--rw-------   0 runner    (1001) docker     (127)     4482 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/lookup_pinecone_index.py
--rw-------   0 runner    (1001) docker     (127)     7622 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/outputs.py
--rw-------   0 runner    (1001) docker     (127)     7173 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/pinecone_collection.py
--rw-------   0 runner    (1001) docker     (127)     8590 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/pinecone_index.py
--rw-------   0 runner    (1001) docker     (127)     3924 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/provider.py
--rw-------   0 runner    (1001) docker     (127)      112 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:28:57.650630 pinecone_pulumi-0.4.2/pinecone_pulumi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/pinecone_pulumi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 23:28:57.650630 pinecone_pulumi-0.4.2/setup.cfg
--rw-------   0 runner    (1001) docker     (127)     1306 2024-03-27 23:28:57.000000 pinecone_pulumi-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:27:06.836509 pinecone_pulumi-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-09 21:27:06.836509 pinecone_pulumi-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:27:06.836509 pinecone_pulumi-0.4.3/pinecone_pulumi/
+-rw-------   0 runner    (1001) docker     (127)     1091 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      454 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     8997 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     9279 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:27:06.836509 pinecone_pulumi-0.4.3/pinecone_pulumi/config/
+-rw-------   0 runner    (1001) docker     (127)      267 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      580 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/config/vars.py
+-rw-------   0 runner    (1001) docker     (127)     4793 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/lookup_pinecone_collection.py
+-rw-------   0 runner    (1001) docker     (127)     4482 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/lookup_pinecone_index.py
+-rw-------   0 runner    (1001) docker     (127)     7622 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     7173 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/pinecone_collection.py
+-rw-------   0 runner    (1001) docker     (127)     8590 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/pinecone_index.py
+-rw-------   0 runner    (1001) docker     (127)     3924 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/provider.py
+-rw-------   0 runner    (1001) docker     (127)      112 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:27:06.836509 pinecone_pulumi-0.4.3/pinecone_pulumi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/pinecone_pulumi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 21:27:06.836509 pinecone_pulumi-0.4.3/setup.cfg
+-rw-------   0 runner    (1001) docker     (127)     1296 2024-05-09 21:27:06.000000 pinecone_pulumi-0.4.3/setup.py
```

### Comparing `pinecone_pulumi-0.4.2/PKG-INFO` & `pinecone_pulumi-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone_pulumi
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Pulumi native provider for Pinecone
 Home-page: https://www.pinecone.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pinecone-io/pulumi-pinecone
 Keywords: pulumi pinecone category/utility kind/native
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pinecone_pulumi-0.4.2/README.md` & `pinecone_pulumi-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pinecone_pulumi-0.4.2/pinecone_pulumi/__init__.py` & `pinecone_pulumi-0.4.3/pinecone_pulumi/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_pulumi-0.4.2/pinecone_pulumi/_inputs.py` & `pinecone_pulumi-0.4.3/pinecone_pulumi/_inputs.py`

 * *Files identical despite different names*

### Comparing `pinecone_pulumi-0.4.2/pinecone_pulumi/_utilities.py` & `pinecone_pulumi-0.4.3/pinecone_pulumi/_utilities.py`

 * *Files identical despite different names*

### Comparing `pinecone_pulumi-0.4.2/pinecone_pulumi/config/vars.py` & `pinecone_pulumi-0.4.3/pinecone_pulumi/config/vars.py`

 * *Files identical despite different names*

### Comparing `pinecone_pulumi-0.4.2/pinecone_pulumi/lookup_pinecone_collection.py` & `pinecone_pulumi-0.4.3/pinecone_pulumi/lookup_pinecone_collection.py`

 * *Files identical despite different names*

### Comparing `pinecone_pulumi-0.4.2/pinecone_pulumi/lookup_pinecone_index.py` & `pinecone_pulumi-0.4.3/pinecone_pulumi/lookup_pinecone_index.py`

 * *Files identical despite different names*

### Comparing `pinecone_pulumi-0.4.2/pinecone_pulumi/outputs.py` & `pinecone_pulumi-0.4.3/pinecone_pulumi/outputs.py`

 * *Files identical despite different names*

### Comparing `pinecone_pulumi-0.4.2/pinecone_pulumi/pinecone_collection.py` & `pinecone_pulumi-0.4.3/pinecone_pulumi/pinecone_collection.py`

 * *Files identical despite different names*

### Comparing `pinecone_pulumi-0.4.2/pinecone_pulumi/pinecone_index.py` & `pinecone_pulumi-0.4.3/pinecone_pulumi/pinecone_index.py`

 * *Files identical despite different names*

### Comparing `pinecone_pulumi-0.4.2/pinecone_pulumi/provider.py` & `pinecone_pulumi-0.4.3/pinecone_pulumi/provider.py`

 * *Files identical despite different names*

### Comparing `pinecone_pulumi-0.4.2/pinecone_pulumi.egg-info/PKG-INFO` & `pinecone_pulumi-0.4.3/pinecone_pulumi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-pulumi
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Pulumi native provider for Pinecone
 Home-page: https://www.pinecone.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pinecone-io/pulumi-pinecone
 Keywords: pulumi pinecone category/utility kind/native
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pinecone_pulumi-0.4.2/pinecone_pulumi.egg-info/SOURCES.txt` & `pinecone_pulumi-0.4.3/pinecone_pulumi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pinecone_pulumi-0.4.2/setup.py` & `pinecone_pulumi-0.4.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-language-python. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import errno
-import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.2"
+VERSION = "0.4.3"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "pinecone Pulumi Package - Development Version"
```

