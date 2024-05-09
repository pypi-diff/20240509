# Comparing `tmp/sweb-0.4.tar.gz` & `tmp/sweb-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweb-0.4.tar", last modified: Thu May  9 11:44:49 2024, max compression
+gzip compressed data, was "sweb-0.5.tar", last modified: Thu May  9 17:08:06 2024, max compression
```

## Comparing `sweb-0.4.tar` & `sweb-0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:44:49.962354 sweb-0.4/
--rw-r--r--   0 redpist    (501) staff       (20)     1072 2024-05-09 10:54:39.000000 sweb-0.4/LICENSE
--rw-r--r--   0 redpist    (501) staff       (20)     1018 2024-05-09 11:44:49.961728 sweb-0.4/PKG-INFO
--rw-r--r--   0 redpist    (501) staff       (20)      134 2024-05-09 11:29:26.000000 sweb-0.4/README.md
--rw-r--r--   0 redpist    (501) staff       (20)       38 2024-05-09 11:44:49.962472 sweb-0.4/setup.cfg
--rw-r--r--   0 redpist    (501) staff       (20)     1182 2024-05-09 11:41:55.000000 sweb-0.4/setup.py
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:44:49.957284 sweb-0.4/sweb/
--rw-r--r--   0 redpist    (501) staff       (20)        0 2024-05-09 10:58:50.000000 sweb-0.4/sweb/__init__.py
--rw-r--r--   0 redpist    (501) staff       (20)     1726 2024-05-09 11:41:33.000000 sweb-0.4/sweb/app.py
--rw-r--r--   0 redpist    (501) staff       (20)      449 2024-05-09 11:00:23.000000 sweb-0.4/sweb/asset_manager.py
--rw-r--r--   0 redpist    (501) staff       (20)      832 2024-05-09 11:00:48.000000 sweb-0.4/sweb/data_loader.py
--rw-r--r--   0 redpist    (501) staff       (20)     1466 2024-05-09 11:00:48.000000 sweb-0.4/sweb/style_processor.py
--rw-r--r--   0 redpist    (501) staff       (20)     1317 2024-05-09 11:00:48.000000 sweb-0.4/sweb/template_processor.py
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:44:49.961151 sweb-0.4/sweb.egg-info/
--rw-r--r--   0 redpist    (501) staff       (20)     1018 2024-05-09 11:44:49.000000 sweb-0.4/sweb.egg-info/PKG-INFO
--rw-r--r--   0 redpist    (501) staff       (20)      318 2024-05-09 11:44:49.000000 sweb-0.4/sweb.egg-info/SOURCES.txt
--rw-r--r--   0 redpist    (501) staff       (20)        1 2024-05-09 11:44:49.000000 sweb-0.4/sweb.egg-info/dependency_links.txt
--rw-r--r--   0 redpist    (501) staff       (20)       39 2024-05-09 11:44:49.000000 sweb-0.4/sweb.egg-info/entry_points.txt
--rw-r--r--   0 redpist    (501) staff       (20)       16 2024-05-09 11:44:49.000000 sweb-0.4/sweb.egg-info/requires.txt
--rw-r--r--   0 redpist    (501) staff       (20)        5 2024-05-09 11:44:49.000000 sweb-0.4/sweb.egg-info/top_level.txt
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 17:08:06.324033 sweb-0.5/
+-rw-r--r--   0 redpist    (501) staff       (20)     1072 2024-05-09 10:54:39.000000 sweb-0.5/LICENSE
+-rw-r--r--   0 redpist    (501) staff       (20)     5857 2024-05-09 17:08:06.323322 sweb-0.5/PKG-INFO
+-rw-r--r--   0 redpist    (501) staff       (20)     4979 2024-05-09 17:03:21.000000 sweb-0.5/README.md
+-rw-r--r--   0 redpist    (501) staff       (20)       38 2024-05-09 17:08:06.324284 sweb-0.5/setup.cfg
+-rw-r--r--   0 redpist    (501) staff       (20)     1176 2024-05-09 17:05:11.000000 sweb-0.5/setup.py
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 17:08:06.317848 sweb-0.5/sweb/
+-rw-r--r--   0 redpist    (501) staff       (20)        0 2024-05-09 10:58:50.000000 sweb-0.5/sweb/__init__.py
+-rw-r--r--   0 redpist    (501) staff       (20)     3643 2024-05-09 17:07:57.000000 sweb-0.5/sweb/app.py
+-rw-r--r--   0 redpist    (501) staff       (20)      449 2024-05-09 11:00:23.000000 sweb-0.5/sweb/asset_manager.py
+-rw-r--r--   0 redpist    (501) staff       (20)      832 2024-05-09 11:00:48.000000 sweb-0.5/sweb/data_loader.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1466 2024-05-09 11:00:48.000000 sweb-0.5/sweb/style_processor.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1317 2024-05-09 11:00:48.000000 sweb-0.5/sweb/template_processor.py
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 17:08:06.322353 sweb-0.5/sweb.egg-info/
+-rw-r--r--   0 redpist    (501) staff       (20)     5857 2024-05-09 17:08:06.000000 sweb-0.5/sweb.egg-info/PKG-INFO
+-rw-r--r--   0 redpist    (501) staff       (20)      318 2024-05-09 17:08:06.000000 sweb-0.5/sweb.egg-info/SOURCES.txt
+-rw-r--r--   0 redpist    (501) staff       (20)        1 2024-05-09 17:08:06.000000 sweb-0.5/sweb.egg-info/dependency_links.txt
+-rw-r--r--   0 redpist    (501) staff       (20)       39 2024-05-09 17:08:06.000000 sweb-0.5/sweb.egg-info/entry_points.txt
+-rw-r--r--   0 redpist    (501) staff       (20)       16 2024-05-09 17:08:06.000000 sweb-0.5/sweb.egg-info/requires.txt
+-rw-r--r--   0 redpist    (501) staff       (20)        5 2024-05-09 17:08:06.000000 sweb-0.5/sweb.egg-info/top_level.txt
```

### Comparing `sweb-0.4/LICENSE` & `sweb-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sweb-0.4/setup.py` & `sweb-0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sweb',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     entry_points={
       'console_scripts': [
         'sweb=sweb.app:main',  # Define the command and point it to the entry function
       ]
     },
-    description='SWEB is a static site generator that processes templates, styles, and assets to build',
+    description='SWEB is a static website generator that processes templates, styles, and assets',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Jeremy LECERF',
     author_email='redpist.com@gmail.com',
     license='MIT',
     classifiers=[
       'Development Status :: 3 - Alpha',
```

### Comparing `sweb-0.4/sweb/data_loader.py` & `sweb-0.5/sweb/data_loader.py`

 * *Files identical despite different names*

### Comparing `sweb-0.4/sweb/style_processor.py` & `sweb-0.5/sweb/style_processor.py`

 * *Files identical despite different names*

### Comparing `sweb-0.4/sweb/template_processor.py` & `sweb-0.5/sweb/template_processor.py`

 * *Files identical despite different names*

