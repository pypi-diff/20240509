# Comparing `tmp/sweb-0.3.tar.gz` & `tmp/sweb-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweb-0.3.tar", last modified: Thu May  9 11:39:23 2024, max compression
+gzip compressed data, was "sweb-0.4.tar", last modified: Thu May  9 11:44:49 2024, max compression
```

## Comparing `sweb-0.3.tar` & `sweb-0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:39:23.856543 sweb-0.3/
--rw-r--r--   0 redpist    (501) staff       (20)     1072 2024-05-09 10:54:39.000000 sweb-0.3/LICENSE
--rw-r--r--   0 redpist    (501) staff       (20)     1018 2024-05-09 11:39:23.856096 sweb-0.3/PKG-INFO
--rw-r--r--   0 redpist    (501) staff       (20)      134 2024-05-09 11:29:26.000000 sweb-0.3/README.md
--rw-r--r--   0 redpist    (501) staff       (20)       38 2024-05-09 11:39:23.856629 sweb-0.3/setup.cfg
--rw-r--r--   0 redpist    (501) staff       (20)     1182 2024-05-09 11:38:56.000000 sweb-0.3/setup.py
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:39:23.852801 sweb-0.3/sweb/
--rw-r--r--   0 redpist    (501) staff       (20)        0 2024-05-09 10:58:50.000000 sweb-0.3/sweb/__init__.py
--rw-r--r--   0 redpist    (501) staff       (20)     1705 2024-05-09 11:38:48.000000 sweb-0.3/sweb/app.py
--rw-r--r--   0 redpist    (501) staff       (20)      449 2024-05-09 11:00:23.000000 sweb-0.3/sweb/asset_manager.py
--rw-r--r--   0 redpist    (501) staff       (20)      832 2024-05-09 11:00:48.000000 sweb-0.3/sweb/data_loader.py
--rw-r--r--   0 redpist    (501) staff       (20)     1466 2024-05-09 11:00:48.000000 sweb-0.3/sweb/style_processor.py
--rw-r--r--   0 redpist    (501) staff       (20)     1317 2024-05-09 11:00:48.000000 sweb-0.3/sweb/template_processor.py
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:39:23.855633 sweb-0.3/sweb.egg-info/
--rw-r--r--   0 redpist    (501) staff       (20)     1018 2024-05-09 11:39:23.000000 sweb-0.3/sweb.egg-info/PKG-INFO
--rw-r--r--   0 redpist    (501) staff       (20)      318 2024-05-09 11:39:23.000000 sweb-0.3/sweb.egg-info/SOURCES.txt
--rw-r--r--   0 redpist    (501) staff       (20)        1 2024-05-09 11:39:23.000000 sweb-0.3/sweb.egg-info/dependency_links.txt
--rw-r--r--   0 redpist    (501) staff       (20)       39 2024-05-09 11:39:23.000000 sweb-0.3/sweb.egg-info/entry_points.txt
--rw-r--r--   0 redpist    (501) staff       (20)       16 2024-05-09 11:39:23.000000 sweb-0.3/sweb.egg-info/requires.txt
--rw-r--r--   0 redpist    (501) staff       (20)        5 2024-05-09 11:39:23.000000 sweb-0.3/sweb.egg-info/top_level.txt
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:44:49.962354 sweb-0.4/
+-rw-r--r--   0 redpist    (501) staff       (20)     1072 2024-05-09 10:54:39.000000 sweb-0.4/LICENSE
+-rw-r--r--   0 redpist    (501) staff       (20)     1018 2024-05-09 11:44:49.961728 sweb-0.4/PKG-INFO
+-rw-r--r--   0 redpist    (501) staff       (20)      134 2024-05-09 11:29:26.000000 sweb-0.4/README.md
+-rw-r--r--   0 redpist    (501) staff       (20)       38 2024-05-09 11:44:49.962472 sweb-0.4/setup.cfg
+-rw-r--r--   0 redpist    (501) staff       (20)     1182 2024-05-09 11:41:55.000000 sweb-0.4/setup.py
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:44:49.957284 sweb-0.4/sweb/
+-rw-r--r--   0 redpist    (501) staff       (20)        0 2024-05-09 10:58:50.000000 sweb-0.4/sweb/__init__.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1726 2024-05-09 11:41:33.000000 sweb-0.4/sweb/app.py
+-rw-r--r--   0 redpist    (501) staff       (20)      449 2024-05-09 11:00:23.000000 sweb-0.4/sweb/asset_manager.py
+-rw-r--r--   0 redpist    (501) staff       (20)      832 2024-05-09 11:00:48.000000 sweb-0.4/sweb/data_loader.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1466 2024-05-09 11:00:48.000000 sweb-0.4/sweb/style_processor.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1317 2024-05-09 11:00:48.000000 sweb-0.4/sweb/template_processor.py
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:44:49.961151 sweb-0.4/sweb.egg-info/
+-rw-r--r--   0 redpist    (501) staff       (20)     1018 2024-05-09 11:44:49.000000 sweb-0.4/sweb.egg-info/PKG-INFO
+-rw-r--r--   0 redpist    (501) staff       (20)      318 2024-05-09 11:44:49.000000 sweb-0.4/sweb.egg-info/SOURCES.txt
+-rw-r--r--   0 redpist    (501) staff       (20)        1 2024-05-09 11:44:49.000000 sweb-0.4/sweb.egg-info/dependency_links.txt
+-rw-r--r--   0 redpist    (501) staff       (20)       39 2024-05-09 11:44:49.000000 sweb-0.4/sweb.egg-info/entry_points.txt
+-rw-r--r--   0 redpist    (501) staff       (20)       16 2024-05-09 11:44:49.000000 sweb-0.4/sweb.egg-info/requires.txt
+-rw-r--r--   0 redpist    (501) staff       (20)        5 2024-05-09 11:44:49.000000 sweb-0.4/sweb.egg-info/top_level.txt
```

### Comparing `sweb-0.3/LICENSE` & `sweb-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sweb-0.3/PKG-INFO` & `sweb-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweb
-Version: 0.3
+Version: 0.4
 Summary: SWEB is a static site generator that processes templates, styles, and assets to build
 Author: Jeremy LECERF
 Author-email: redpist.com@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sweb-0.3/setup.py` & `sweb-0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sweb',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     entry_points={
       'console_scripts': [
         'sweb=sweb.app:main',  # Define the command and point it to the entry function
       ]
     },
     description='SWEB is a static site generator that processes templates, styles, and assets to build',
```

### Comparing `sweb-0.3/sweb/app.py` & `sweb-0.4/sweb/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,21 @@
     style_processor = StyleProcessor(self.styles_src, self.styles_dst)
     asset_manager = AssetManager(self.assets_src, self.assets_dst)
 
     template_processor.process_templates()
     style_processor.process_styles()
     asset_manager.copy_assets()
 
-if __name__ == "__main__":
+def main():
   generator = SiteGenerator(
     data_dir='app/data',
     template_dir='app/templates',
     output_dir='dist',
     assets_src='app/assets',
     assets_dst='dist/assets',
     styles_src='app/styles',
     styles_dst='dist/styles'
   )
   generator.generate_site()
+
+if __name__ == "__main__":
+  main()
```

### Comparing `sweb-0.3/sweb/data_loader.py` & `sweb-0.4/sweb/data_loader.py`

 * *Files identical despite different names*

### Comparing `sweb-0.3/sweb/style_processor.py` & `sweb-0.4/sweb/style_processor.py`

 * *Files identical despite different names*

### Comparing `sweb-0.3/sweb/template_processor.py` & `sweb-0.4/sweb/template_processor.py`

 * *Files identical despite different names*

### Comparing `sweb-0.3/sweb.egg-info/PKG-INFO` & `sweb-0.4/sweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweb
-Version: 0.3
+Version: 0.4
 Summary: SWEB is a static site generator that processes templates, styles, and assets to build
 Author: Jeremy LECERF
 Author-email: redpist.com@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

