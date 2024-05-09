# Comparing `tmp/tooniez-timetree-sdk-0.0.3.tar.gz` & `tmp/tooniez-timetree-sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooniez-timetree-sdk-0.0.3.tar", last modified: Thu May  9 06:43:32 2024, max compression
+gzip compressed data, was "tooniez-timetree-sdk-0.0.4.tar", last modified: Thu May  9 06:49:45 2024, max compression
```

## Comparing `tooniez-timetree-sdk-0.0.3.tar` & `tooniez-timetree-sdk-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:43:32.586269 tooniez-timetree-sdk-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-09 06:43:32.586269 tooniez-timetree-sdk-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:43:32.586269 tooniez-timetree-sdk-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:43:32.586269 tooniez-timetree-sdk-0.0.3/timetree_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/timetree_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/timetree_sdk/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:43:32.586269 tooniez-timetree-sdk-0.0.3/timetree_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/timetree_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/timetree_sdk/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/timetree_sdk/models/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/timetree_sdk/models/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:43:32.586269 tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-09 06:43:32.000000 tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 06:43:32.000000 tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:43:32.000000 tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 06:43:32.000000 tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 06:43:32.000000 tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:49:45.802456 tooniez-timetree-sdk-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-09 06:49:45.802456 tooniez-timetree-sdk-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-09 06:49:42.000000 tooniez-timetree-sdk-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:49:45.802456 tooniez-timetree-sdk-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-09 06:49:42.000000 tooniez-timetree-sdk-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:49:45.798456 tooniez-timetree-sdk-0.0.4/timetree_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:49:42.000000 tooniez-timetree-sdk-0.0.4/timetree_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-09 06:49:42.000000 tooniez-timetree-sdk-0.0.4/timetree_sdk/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:49:45.802456 tooniez-timetree-sdk-0.0.4/timetree_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-09 06:49:42.000000 tooniez-timetree-sdk-0.0.4/timetree_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-09 06:49:42.000000 tooniez-timetree-sdk-0.0.4/timetree_sdk/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-09 06:49:42.000000 tooniez-timetree-sdk-0.0.4/timetree_sdk/models/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-05-09 06:49:42.000000 tooniez-timetree-sdk-0.0.4/timetree_sdk/models/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:49:45.802456 tooniez-timetree-sdk-0.0.4/tooniez_timetree_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-09 06:49:45.000000 tooniez-timetree-sdk-0.0.4/tooniez_timetree_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 06:49:45.000000 tooniez-timetree-sdk-0.0.4/tooniez_timetree_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:49:45.000000 tooniez-timetree-sdk-0.0.4/tooniez_timetree_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 06:49:45.000000 tooniez-timetree-sdk-0.0.4/tooniez_timetree_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 06:49:45.000000 tooniez-timetree-sdk-0.0.4/tooniez_timetree_sdk.egg-info/top_level.txt
```

### Comparing `tooniez-timetree-sdk-0.0.3/PKG-INFO` & `tooniez-timetree-sdk-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tooniez-timetree-sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: TimeTree SDK
-Home-page: https://github.com/tooniez/timetree-sdk
+Home-page: https://github.com/tooniez/tooniez-timetree-sdk
 Author: tooniez
 Author-email: tooni22@proton.me
 License: MIT
 Description: # TimeTree SDK for Python
         
         [TimeTree API](https://developers.timetreeapp.com/en/docs/api) SDK for Python.
```

### Comparing `tooniez-timetree-sdk-0.0.3/README.md` & `tooniez-timetree-sdk-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tooniez-timetree-sdk-0.0.3/setup.py` & `tooniez-timetree-sdk-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='tooniez-timetree-sdk',
     packages=['timetree_sdk', 'timetree_sdk/models/'],
-    version='0.0.3',
+    version='0.0.4',
     license='MIT',
     install_requires=['requests'],
     author='tooniez',
     author_email='tooni22@proton.me',
-    url='https://github.com/tooniez/timetree-sdk',
+    url='https://github.com/tooniez/tooniez-timetree-sdk',
     description='TimeTree SDK',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='timetree api sdk',
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
```

### Comparing `tooniez-timetree-sdk-0.0.3/timetree_sdk/api.py` & `tooniez-timetree-sdk-0.0.4/timetree_sdk/api.py`

 * *Files identical despite different names*

### Comparing `tooniez-timetree-sdk-0.0.3/timetree_sdk/models/base.py` & `tooniez-timetree-sdk-0.0.4/timetree_sdk/models/base.py`

 * *Files identical despite different names*

### Comparing `tooniez-timetree-sdk-0.0.3/timetree_sdk/models/events.py` & `tooniez-timetree-sdk-0.0.4/timetree_sdk/models/events.py`

 * *Files identical despite different names*

### Comparing `tooniez-timetree-sdk-0.0.3/timetree_sdk/models/responses.py` & `tooniez-timetree-sdk-0.0.4/timetree_sdk/models/responses.py`

 * *Files identical despite different names*

### Comparing `tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/PKG-INFO` & `tooniez-timetree-sdk-0.0.4/tooniez_timetree_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tooniez-timetree-sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: TimeTree SDK
-Home-page: https://github.com/tooniez/timetree-sdk
+Home-page: https://github.com/tooniez/tooniez-timetree-sdk
 Author: tooniez
 Author-email: tooni22@proton.me
 License: MIT
 Description: # TimeTree SDK for Python
         
         [TimeTree API](https://developers.timetreeapp.com/en/docs/api) SDK for Python.
```

