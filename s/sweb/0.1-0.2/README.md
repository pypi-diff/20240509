# Comparing `tmp/sweb-0.1.tar.gz` & `tmp/sweb-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweb-0.1.tar", last modified: Thu May  9 11:28:54 2024, max compression
+gzip compressed data, was "sweb-0.2.tar", last modified: Thu May  9 11:36:10 2024, max compression
```

## Comparing `sweb-0.1.tar` & `sweb-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:28:54.618369 sweb-0.1/
--rw-r--r--   0 redpist    (501) staff       (20)     1072 2024-05-09 10:54:39.000000 sweb-0.1/LICENSE
--rw-r--r--   0 redpist    (501) staff       (20)      969 2024-05-09 11:28:54.617934 sweb-0.1/PKG-INFO
--rw-r--r--   0 redpist    (501) staff       (20)      128 2024-05-09 11:28:48.000000 sweb-0.1/README.md
--rw-r--r--   0 redpist    (501) staff       (20)       38 2024-05-09 11:28:54.618457 sweb-0.1/setup.cfg
--rw-r--r--   0 redpist    (501) staff       (20)     1139 2024-05-09 11:28:14.000000 sweb-0.1/setup.py
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:28:54.615163 sweb-0.1/sweb/
--rw-r--r--   0 redpist    (501) staff       (20)        0 2024-05-09 10:58:50.000000 sweb-0.1/sweb/__init__.py
--rw-r--r--   0 redpist    (501) staff       (20)     1701 2024-05-09 11:02:04.000000 sweb-0.1/sweb/app.py
--rw-r--r--   0 redpist    (501) staff       (20)      449 2024-05-09 11:00:23.000000 sweb-0.1/sweb/asset_manager.py
--rw-r--r--   0 redpist    (501) staff       (20)      832 2024-05-09 11:00:48.000000 sweb-0.1/sweb/data_loader.py
--rw-r--r--   0 redpist    (501) staff       (20)     1466 2024-05-09 11:00:48.000000 sweb-0.1/sweb/style_processor.py
--rw-r--r--   0 redpist    (501) staff       (20)     1317 2024-05-09 11:00:48.000000 sweb-0.1/sweb/template_processor.py
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:28:54.617500 sweb-0.1/sweb.egg-info/
--rw-r--r--   0 redpist    (501) staff       (20)      969 2024-05-09 11:28:54.000000 sweb-0.1/sweb.egg-info/PKG-INFO
--rw-r--r--   0 redpist    (501) staff       (20)      318 2024-05-09 11:28:54.000000 sweb-0.1/sweb.egg-info/SOURCES.txt
--rw-r--r--   0 redpist    (501) staff       (20)        1 2024-05-09 11:28:54.000000 sweb-0.1/sweb.egg-info/dependency_links.txt
--rw-r--r--   0 redpist    (501) staff       (20)       39 2024-05-09 11:28:54.000000 sweb-0.1/sweb.egg-info/entry_points.txt
--rw-r--r--   0 redpist    (501) staff       (20)       16 2024-05-09 11:28:54.000000 sweb-0.1/sweb.egg-info/requires.txt
--rw-r--r--   0 redpist    (501) staff       (20)        5 2024-05-09 11:28:54.000000 sweb-0.1/sweb.egg-info/top_level.txt
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:36:10.414429 sweb-0.2/
+-rw-r--r--   0 redpist    (501) staff       (20)     1072 2024-05-09 10:54:39.000000 sweb-0.2/LICENSE
+-rw-r--r--   0 redpist    (501) staff       (20)     1018 2024-05-09 11:36:10.413710 sweb-0.2/PKG-INFO
+-rw-r--r--   0 redpist    (501) staff       (20)      134 2024-05-09 11:29:26.000000 sweb-0.2/README.md
+-rw-r--r--   0 redpist    (501) staff       (20)       38 2024-05-09 11:36:10.414563 sweb-0.2/setup.cfg
+-rw-r--r--   0 redpist    (501) staff       (20)     1182 2024-05-09 11:35:26.000000 sweb-0.2/setup.py
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:36:10.410242 sweb-0.2/sweb/
+-rw-r--r--   0 redpist    (501) staff       (20)        0 2024-05-09 10:58:50.000000 sweb-0.2/sweb/__init__.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1701 2024-05-09 11:02:04.000000 sweb-0.2/sweb/app.py
+-rw-r--r--   0 redpist    (501) staff       (20)      449 2024-05-09 11:00:23.000000 sweb-0.2/sweb/asset_manager.py
+-rw-r--r--   0 redpist    (501) staff       (20)      832 2024-05-09 11:00:48.000000 sweb-0.2/sweb/data_loader.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1466 2024-05-09 11:00:48.000000 sweb-0.2/sweb/style_processor.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1317 2024-05-09 11:00:48.000000 sweb-0.2/sweb/template_processor.py
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 11:36:10.413119 sweb-0.2/sweb.egg-info/
+-rw-r--r--   0 redpist    (501) staff       (20)     1018 2024-05-09 11:36:10.000000 sweb-0.2/sweb.egg-info/PKG-INFO
+-rw-r--r--   0 redpist    (501) staff       (20)      318 2024-05-09 11:36:10.000000 sweb-0.2/sweb.egg-info/SOURCES.txt
+-rw-r--r--   0 redpist    (501) staff       (20)        1 2024-05-09 11:36:10.000000 sweb-0.2/sweb.egg-info/dependency_links.txt
+-rw-r--r--   0 redpist    (501) staff       (20)       39 2024-05-09 11:36:10.000000 sweb-0.2/sweb.egg-info/entry_points.txt
+-rw-r--r--   0 redpist    (501) staff       (20)       16 2024-05-09 11:36:10.000000 sweb-0.2/sweb.egg-info/requires.txt
+-rw-r--r--   0 redpist    (501) staff       (20)        5 2024-05-09 11:36:10.000000 sweb-0.2/sweb.egg-info/top_level.txt
```

### Comparing `sweb-0.1/LICENSE` & `sweb-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sweb-0.1/setup.py` & `sweb-0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sweb',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     entry_points={
       'console_scripts': [
         'sweb=sweb.app:main',  # Define the command and point it to the entry function
       ]
     },
-    description='A command line tool for processing',
+    description='SWEB is a static site generator that processes templates, styles, and assets to build',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Jeremy LECERF',
     author_email='redpist.com@gmail.com',
     license='MIT',
     classifiers=[
       'Development Status :: 3 - Alpha',
@@ -24,13 +24,13 @@
       'Programming Language :: Python :: 3.7',
       'Programming Language :: Python :: 3.8',
       'Programming Language :: Python :: 3.9',
       'Programming Language :: Python :: 3.10',
       'Programming Language :: Python :: 3.11',
       'Programming Language :: Python :: 3.12'
     ],
-    python_requires='>=3.6, <=3.12',
+    python_requires='>=3.6',
     install_requires=[
       'pybars3',
       'libsass'
     ]
 )
```

### Comparing `sweb-0.1/sweb/app.py` & `sweb-0.2/sweb/app.py`

 * *Files identical despite different names*

### Comparing `sweb-0.1/sweb/data_loader.py` & `sweb-0.2/sweb/data_loader.py`

 * *Files identical despite different names*

### Comparing `sweb-0.1/sweb/style_processor.py` & `sweb-0.2/sweb/style_processor.py`

 * *Files identical despite different names*

### Comparing `sweb-0.1/sweb/template_processor.py` & `sweb-0.2/sweb/template_processor.py`

 * *Files identical despite different names*

