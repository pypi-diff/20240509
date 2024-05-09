# Comparing `tmp/owl2else-0.9.2.tar.gz` & `tmp/owl2else-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owl2else-0.9.2.tar", last modified: Wed May  8 14:06:12 2024, max compression
+gzip compressed data, was "owl2else-0.9.3.tar", last modified: Thu May  9 04:44:31 2024, max compression
```

## Comparing `owl2else-0.9.2.tar` & `owl2else-0.9.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2024-05-08 14:06:12.001621 owl2else-0.9.2/
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)     3228 2022-05-13 09:13:03.000000 owl2else-0.9.2/.gitignore
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)    35149 2022-05-13 09:13:03.000000 owl2else-0.9.2/LICENSE
--rw-r--r--   0 bejar     (1000) bejar     (1000)      868 2024-05-08 14:06:12.001621 owl2else-0.9.2/PKG-INFO
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)      345 2022-05-13 09:13:03.000000 owl2else-0.9.2/README.md
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2024-05-08 14:06:11.964621 owl2else-0.9.2/bin/
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)     4803 2022-05-13 09:13:03.000000 owl2else-0.9.2/bin/owl2clips
--rw-r--r--   0 bejar     (1000) bejar     (1000)       35 2023-10-03 07:38:02.000000 owl2else-0.9.2/bin/owl2clips.bat
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)     4711 2022-05-13 09:13:03.000000 owl2else-0.9.2/bin/owl2plot
--rw-r--r--   0 bejar     (1000) bejar     (1000)       34 2023-10-03 07:54:33.000000 owl2else-0.9.2/bin/owl2plot.bat
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)     3691 2024-05-08 14:01:42.000000 owl2else-0.9.2/bin/owl2rdflib
--rw-r--r--   0 bejar     (1000) bejar     (1000)       36 2023-10-03 07:54:52.000000 owl2else-0.9.2/bin/owl2rdflib.bat
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2024-05-08 14:06:11.998621 owl2else-0.9.2/owl2conv/
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)      217 2022-05-13 09:13:03.000000 owl2else-0.9.2/owl2conv/__init__.py
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)    11874 2023-10-19 04:34:55.000000 owl2else-0.9.2/owl2conv/owlobjects.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2024-05-08 14:06:12.000621 owl2else-0.9.2/owl2else.egg-info/
--rw-r--r--   0 bejar     (1000) bejar     (1000)      868 2024-05-08 14:06:11.000000 owl2else-0.9.2/owl2else.egg-info/PKG-INFO
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      351 2024-05-08 14:06:11.000000 owl2else-0.9.2/owl2else.egg-info/SOURCES.txt
--rw-rw-r--   0 bejar     (1000) bejar     (1000)        1 2024-05-08 14:06:11.000000 owl2else-0.9.2/owl2else.egg-info/dependency_links.txt
--rw-rw-r--   0 bejar     (1000) bejar     (1000)       27 2024-05-08 14:06:11.000000 owl2else-0.9.2/owl2else.egg-info/requires.txt
--rw-rw-r--   0 bejar     (1000) bejar     (1000)        9 2024-05-08 14:06:11.000000 owl2else-0.9.2/owl2else.egg-info/top_level.txt
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)      203 2023-10-03 07:45:56.000000 owl2else-0.9.2/pack
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)       79 2024-05-08 14:06:12.002621 owl2else-0.9.2/setup.cfg
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)     1073 2024-05-08 14:05:46.000000 owl2else-0.9.2/setup.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2024-05-09 04:44:31.011349 owl2else-0.9.3/
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)     3228 2022-05-13 09:13:03.000000 owl2else-0.9.3/.gitignore
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)    35149 2022-05-13 09:13:03.000000 owl2else-0.9.3/LICENSE
+-rw-r--r--   0 bejar     (1000) bejar     (1000)      868 2024-05-09 04:44:31.011349 owl2else-0.9.3/PKG-INFO
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)      345 2022-05-13 09:13:03.000000 owl2else-0.9.3/README.md
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2024-05-09 04:44:30.989349 owl2else-0.9.3/bin/
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)     4803 2022-05-13 09:13:03.000000 owl2else-0.9.3/bin/owl2clips
+-rw-r--r--   0 bejar     (1000) bejar     (1000)       35 2023-10-03 07:38:02.000000 owl2else-0.9.3/bin/owl2clips.bat
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)     4711 2022-05-13 09:13:03.000000 owl2else-0.9.3/bin/owl2plot
+-rw-r--r--   0 bejar     (1000) bejar     (1000)       34 2023-10-03 07:54:33.000000 owl2else-0.9.3/bin/owl2plot.bat
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)     3702 2024-05-09 04:42:02.000000 owl2else-0.9.3/bin/owl2rdflib
+-rw-r--r--   0 bejar     (1000) bejar     (1000)       36 2023-10-03 07:54:52.000000 owl2else-0.9.3/bin/owl2rdflib.bat
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2024-05-09 04:44:30.989349 owl2else-0.9.3/owl2conv/
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)      217 2022-05-13 09:13:03.000000 owl2else-0.9.3/owl2conv/__init__.py
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)    11874 2023-10-19 04:34:55.000000 owl2else-0.9.3/owl2conv/owlobjects.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2024-05-09 04:44:31.010349 owl2else-0.9.3/owl2else.egg-info/
+-rw-r--r--   0 bejar     (1000) bejar     (1000)      868 2024-05-09 04:44:30.000000 owl2else-0.9.3/owl2else.egg-info/PKG-INFO
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      351 2024-05-09 04:44:30.000000 owl2else-0.9.3/owl2else.egg-info/SOURCES.txt
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)        1 2024-05-09 04:44:30.000000 owl2else-0.9.3/owl2else.egg-info/dependency_links.txt
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)       27 2024-05-09 04:44:30.000000 owl2else-0.9.3/owl2else.egg-info/requires.txt
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)        9 2024-05-09 04:44:30.000000 owl2else-0.9.3/owl2else.egg-info/top_level.txt
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)      203 2023-10-03 07:45:56.000000 owl2else-0.9.3/pack
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)       79 2024-05-09 04:44:31.011349 owl2else-0.9.3/setup.cfg
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)     1073 2024-05-09 04:44:10.000000 owl2else-0.9.3/setup.py
```

### Comparing `owl2else-0.9.2/.gitignore` & `owl2else-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `owl2else-0.9.2/LICENSE` & `owl2else-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `owl2else-0.9.2/PKG-INFO` & `owl2else-0.9.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owl2else
-Version: 0.9.2
+Version: 0.9.3
 Summary: Utilities to transform ontology OWL2 files to other formats
 Home-page: https://github.com/bejar/owl2else
 Author: Javier Bejar
 Author-email: bejar@cs.upc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `owl2else-0.9.2/bin/owl2clips` & `owl2else-0.9.3/bin/owl2clips`

 * *Files identical despite different names*

### Comparing `owl2else-0.9.2/bin/owl2plot` & `owl2else-0.9.3/bin/owl2plot`

 * *Files identical despite different names*

### Comparing `owl2else-0.9.2/bin/owl2rdflib` & `owl2else-0.9.3/bin/owl2rdflib`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 __author__ = 'bejar'
 
 import argparse
 import time
 
 from rdflib import Graph, RDF, OWL, URIRef
-from owl2conv import chop, get_label
+from owl2conv.owl2object import chop, get_label
 
 
 # def chop(uriref):
 #     """
 #     returns the last part of the uriref
 #     :param uriref:
 #     :return:
```

### Comparing `owl2else-0.9.2/owl2conv/owlobjects.py` & `owl2else-0.9.3/owl2conv/owlobjects.py`

 * *Files identical despite different names*

### Comparing `owl2else-0.9.2/owl2else.egg-info/PKG-INFO` & `owl2else-0.9.3/owl2else.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owl2else
-Version: 0.9.2
+Version: 0.9.3
 Summary: Utilities to transform ontology OWL2 files to other formats
 Home-page: https://github.com/bejar/owl2else
 Author: Javier Bejar
 Author-email: bejar@cs.upc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `owl2else-0.9.2/setup.py` & `owl2else-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="owl2else", # Replace with your own username
-    version="0.9.2",
+    version="0.9.3",
     author="Javier Bejar",
     author_email="bejar@cs.upc.edu",
     description="Utilities to transform ontology OWL2 files to other formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bejar/owl2else",
     packages=['owl2conv'],
```

