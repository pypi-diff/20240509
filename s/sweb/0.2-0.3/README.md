# Comparing `tmp/sweb-0.2.tar.gz` & `tmp/sweb-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweb-0.2.tar", last modified: Thu May  9 11:36:10 2024, max compression
+gzip compressed data, was "sweb-0.3.tar", last modified: Thu May  9 11:39:23 2024, max compression
```

## Comparing `sweb-0.2.tar` & `sweb-0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:36:10.414429 sweb-0.2/
--rw-r--r--   0 redpist    (501) staff       (20)     1072 2024-05-09 10:54:39.000000 sweb-0.2/LICENSE
--rw-r--r--   0 redpist    (501) staff       (20)     1018 2024-05-09 11:36:10.413710 sweb-0.2/PKG-INFO
--rw-r--r--   0 redpist    (501) staff       (20)      134 2024-05-09 11:29:26.000000 sweb-0.2/README.md
--rw-r--r--   0 redpist    (501) staff       (20)       38 2024-05-09 11:36:10.414563 sweb-0.2/setup.cfg
--rw-r--r--   0 redpist    (501) staff       (20)     1182 2024-05-09 11:35:26.000000 sweb-0.2/setup.py
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:36:10.410242 sweb-0.2/sweb/
--rw-r--r--   0 redpist    (501) staff       (20)        0 2024-05-09 10:58:50.000000 sweb-0.2/sweb/__init__.py
--rw-r--r--   0 redpist    (501) staff       (20)     1701 2024-05-09 11:02:04.000000 sweb-0.2/sweb/app.py
--rw-r--r--   0 redpist    (501) staff       (20)      449 2024-05-09 11:00:23.000000 sweb-0.2/sweb/asset_manager.py
--rw-r--r--   0 redpist    (501) staff       (20)      832 2024-05-09 11:00:48.000000 sweb-0.2/sweb/data_loader.py
--rw-r--r--   0 redpist    (501) staff       (20)     1466 2024-05-09 11:00:48.000000 sweb-0.2/sweb/style_processor.py
--rw-r--r--   0 redpist    (501) staff       (20)     1317 2024-05-09 11:00:48.000000 sweb-0.2/sweb/template_processor.py
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:36:10.413119 sweb-0.2/sweb.egg-info/
--rw-r--r--   0 redpist    (501) staff       (20)     1018 2024-05-09 11:36:10.000000 sweb-0.2/sweb.egg-info/PKG-INFO
--rw-r--r--   0 redpist    (501) staff       (20)      318 2024-05-09 11:36:10.000000 sweb-0.2/sweb.egg-info/SOURCES.txt
--rw-r--r--   0 redpist    (501) staff       (20)        1 2024-05-09 11:36:10.000000 sweb-0.2/sweb.egg-info/dependency_links.txt
--rw-r--r--   0 redpist    (501) staff       (20)       39 2024-05-09 11:36:10.000000 sweb-0.2/sweb.egg-info/entry_points.txt
--rw-r--r--   0 redpist    (501) staff       (20)       16 2024-05-09 11:36:10.000000 sweb-0.2/sweb.egg-info/requires.txt
--rw-r--r--   0 redpist    (501) staff       (20)        5 2024-05-09 11:36:10.000000 sweb-0.2/sweb.egg-info/top_level.txt
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:39:23.856543 sweb-0.3/
+-rw-r--r--   0 redpist    (501) staff       (20)     1072 2024-05-09 10:54:39.000000 sweb-0.3/LICENSE
+-rw-r--r--   0 redpist    (501) staff       (20)     1018 2024-05-09 11:39:23.856096 sweb-0.3/PKG-INFO
+-rw-r--r--   0 redpist    (501) staff       (20)      134 2024-05-09 11:29:26.000000 sweb-0.3/README.md
+-rw-r--r--   0 redpist    (501) staff       (20)       38 2024-05-09 11:39:23.856629 sweb-0.3/setup.cfg
+-rw-r--r--   0 redpist    (501) staff       (20)     1182 2024-05-09 11:38:56.000000 sweb-0.3/setup.py
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:39:23.852801 sweb-0.3/sweb/
+-rw-r--r--   0 redpist    (501) staff       (20)        0 2024-05-09 10:58:50.000000 sweb-0.3/sweb/__init__.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1705 2024-05-09 11:38:48.000000 sweb-0.3/sweb/app.py
+-rw-r--r--   0 redpist    (501) staff       (20)      449 2024-05-09 11:00:23.000000 sweb-0.3/sweb/asset_manager.py
+-rw-r--r--   0 redpist    (501) staff       (20)      832 2024-05-09 11:00:48.000000 sweb-0.3/sweb/data_loader.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1466 2024-05-09 11:00:48.000000 sweb-0.3/sweb/style_processor.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1317 2024-05-09 11:00:48.000000 sweb-0.3/sweb/template_processor.py
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:39:23.855633 sweb-0.3/sweb.egg-info/
+-rw-r--r--   0 redpist    (501) staff       (20)     1018 2024-05-09 11:39:23.000000 sweb-0.3/sweb.egg-info/PKG-INFO
+-rw-r--r--   0 redpist    (501) staff       (20)      318 2024-05-09 11:39:23.000000 sweb-0.3/sweb.egg-info/SOURCES.txt
+-rw-r--r--   0 redpist    (501) staff       (20)        1 2024-05-09 11:39:23.000000 sweb-0.3/sweb.egg-info/dependency_links.txt
+-rw-r--r--   0 redpist    (501) staff       (20)       39 2024-05-09 11:39:23.000000 sweb-0.3/sweb.egg-info/entry_points.txt
+-rw-r--r--   0 redpist    (501) staff       (20)       16 2024-05-09 11:39:23.000000 sweb-0.3/sweb.egg-info/requires.txt
+-rw-r--r--   0 redpist    (501) staff       (20)        5 2024-05-09 11:39:23.000000 sweb-0.3/sweb.egg-info/top_level.txt
```

### Comparing `sweb-0.2/LICENSE` & `sweb-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sweb-0.2/PKG-INFO` & `sweb-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweb
-Version: 0.2
+Version: 0.3
 Summary: SWEB is a static site generator that processes templates, styles, and assets to build
 Author: Jeremy LECERF
 Author-email: redpist.com@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sweb-0.2/setup.py` & `sweb-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sweb',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     entry_points={
       'console_scripts': [
         'sweb=sweb.app:main',  # Define the command and point it to the entry function
       ]
     },
     description='SWEB is a static site generator that processes templates, styles, and assets to build',
```

### Comparing `sweb-0.2/sweb/app.py` & `sweb-0.3/sweb/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # File: generator.py
 
 import json
 import os
 import shutil
-from template_processor import TemplateProcessor
-from style_processor import StyleProcessor
-from asset_manager import AssetManager
-from data_loader import DataLoader
+from .template_processor import TemplateProcessor
+from .style_processor import StyleProcessor
+from .asset_manager import AssetManager
+from .data_loader import DataLoader
 
 class SiteGenerator:
   """Generates a static website by processing templates, styles, and assets."""
 
   def __init__(self, data_dir, template_dir, output_dir, assets_src, assets_dst, styles_src, styles_dst):
     self.data_dir = data_dir
     self.template_dir = template_dir
```

### Comparing `sweb-0.2/sweb/data_loader.py` & `sweb-0.3/sweb/data_loader.py`

 * *Files identical despite different names*

### Comparing `sweb-0.2/sweb/style_processor.py` & `sweb-0.3/sweb/style_processor.py`

 * *Files identical despite different names*

### Comparing `sweb-0.2/sweb/template_processor.py` & `sweb-0.3/sweb/template_processor.py`

 * *Files identical despite different names*

### Comparing `sweb-0.2/sweb.egg-info/PKG-INFO` & `sweb-0.3/sweb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweb
-Version: 0.2
+Version: 0.3
 Summary: SWEB is a static site generator that processes templates, styles, and assets to build
 Author: Jeremy LECERF
 Author-email: redpist.com@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

