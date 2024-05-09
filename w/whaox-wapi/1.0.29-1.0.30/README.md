# Comparing `tmp/whaox-wapi-1.0.29.tar.gz` & `tmp/whaox-wapi-1.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whaox-wapi-1.0.29.tar", last modified: Wed May  8 17:41:34 2024, max compression
+gzip compressed data, was "whaox-wapi-1.0.30.tar", last modified: Thu May  9 11:49:13 2024, max compression
```

## Comparing `whaox-wapi-1.0.29.tar` & `whaox-wapi-1.0.30.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 17:41:34.457036 whaox-wapi-1.0.29/
--rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.29/LICENSE
--rw-rw-rw-   0        0        0     3020 2024-05-08 17:41:34.455539 whaox-wapi-1.0.29/PKG-INFO
--rw-rw-rw-   0        0        0     2632 2024-04-15 10:27:15.000000 whaox-wapi-1.0.29/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 17:41:34.458047 whaox-wapi-1.0.29/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-05-08 17:41:06.000000 whaox-wapi-1.0.29/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:41:34.371553 whaox-wapi-1.0.29/wapi/
--rw-rw-rw-   0        0        0       27 2024-04-15 09:31:56.000000 whaox-wapi-1.0.29/wapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:41:34.381885 whaox-wapi-1.0.29/wapi/features/
--rw-rw-rw-   0        0        0     1001 2024-04-15 09:36:06.000000 whaox-wapi-1.0.29/wapi/features/GET.py
--rw-rw-rw-   0        0        0      797 2024-05-08 17:41:06.000000 whaox-wapi-1.0.29/wapi/features/POST.py
--rw-rw-rw-   0        0        0      941 2024-04-15 11:14:57.000000 whaox-wapi-1.0.29/wapi/features/Route.py
--rw-rw-rw-   0        0        0       72 2024-04-12 10:19:11.000000 whaox-wapi-1.0.29/wapi/features/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:41:34.384340 whaox-wapi-1.0.29/wapi/static/
--rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wapi-1.0.29/wapi/static/T.py
--rw-rw-rw-   0        0        0        0 2024-04-15 09:20:58.000000 whaox-wapi-1.0.29/wapi/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:41:34.413298 whaox-wapi-1.0.29/wapi/utils/
--rw-rw-rw-   0        0        0        0 2024-04-15 09:21:14.000000 whaox-wapi-1.0.29/wapi/utils/__init__.py
--rw-rw-rw-   0        0        0      307 2024-04-11 20:01:35.000000 whaox-wapi-1.0.29/wapi/utils/get_path.py
--rw-rw-rw-   0        0        0       56 2024-04-11 20:01:35.000000 whaox-wapi-1.0.29/wapi/utils/is_class.py
--rw-rw-rw-   0        0        0      124 2024-04-11 20:01:35.000000 whaox-wapi-1.0.29/wapi/utils/is_dataclass.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:41:34.454537 whaox-wapi-1.0.29/whaox_wapi.egg-info/
--rw-rw-rw-   0        0        0     3020 2024-05-08 17:41:34.000000 whaox-wapi-1.0.29/whaox_wapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2024-05-08 17:41:34.000000 whaox-wapi-1.0.29/whaox_wapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 17:41:34.000000 whaox-wapi-1.0.29/whaox_wapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-08 17:41:34.000000 whaox-wapi-1.0.29/whaox_wapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-08 17:41:34.000000 whaox-wapi-1.0.29/whaox_wapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 11:49:13.284633 whaox-wapi-1.0.30/
+-rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.30/LICENSE
+-rw-rw-rw-   0        0        0     3020 2024-05-09 11:49:13.281696 whaox-wapi-1.0.30/PKG-INFO
+-rw-rw-rw-   0        0        0     2632 2024-04-15 10:27:15.000000 whaox-wapi-1.0.30/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-09 11:49:13.285198 whaox-wapi-1.0.30/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-05-09 11:48:50.000000 whaox-wapi-1.0.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:49:13.223819 whaox-wapi-1.0.30/wapi/
+-rw-rw-rw-   0        0        0       27 2024-04-15 09:31:56.000000 whaox-wapi-1.0.30/wapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:49:13.228136 whaox-wapi-1.0.30/wapi/features/
+-rw-rw-rw-   0        0        0     1001 2024-05-09 11:47:29.000000 whaox-wapi-1.0.30/wapi/features/GET.py
+-rw-rw-rw-   0        0        0      797 2024-05-08 20:23:21.000000 whaox-wapi-1.0.30/wapi/features/POST.py
+-rw-rw-rw-   0        0        0      837 2024-05-09 11:47:35.000000 whaox-wapi-1.0.30/wapi/features/Route.py
+-rw-rw-rw-   0        0        0       72 2024-04-12 10:19:11.000000 whaox-wapi-1.0.30/wapi/features/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:49:13.229692 whaox-wapi-1.0.30/wapi/static/
+-rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wapi-1.0.30/wapi/static/T.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:20:58.000000 whaox-wapi-1.0.30/wapi/static/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:49:13.236053 whaox-wapi-1.0.30/wapi/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:21:14.000000 whaox-wapi-1.0.30/wapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      307 2024-05-08 19:32:55.000000 whaox-wapi-1.0.30/wapi/utils/get_path.py
+-rw-rw-rw-   0        0        0       54 2024-05-09 11:47:35.000000 whaox-wapi-1.0.30/wapi/utils/is_class.py
+-rw-rw-rw-   0        0        0      124 2024-04-11 20:01:35.000000 whaox-wapi-1.0.30/wapi/utils/is_dataclass.py
+-rw-rw-rw-   0        0        0       59 2024-05-09 09:32:44.000000 whaox-wapi-1.0.30/wapi/utils/is_object.py
+-rw-rw-rw-   0        0        0      390 2024-05-09 10:55:41.000000 whaox-wapi-1.0.30/wapi/utils/merge_paths.py
+-rw-rw-rw-   0        0        0      250 2024-05-09 10:56:52.000000 whaox-wapi-1.0.30/wapi/utils/set_path.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:49:13.279100 whaox-wapi-1.0.30/whaox_wapi.egg-info/
+-rw-rw-rw-   0        0        0     3020 2024-05-09 11:49:13.000000 whaox-wapi-1.0.30/whaox_wapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-05-09 11:49:13.000000 whaox-wapi-1.0.30/whaox_wapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 11:49:13.000000 whaox-wapi-1.0.30/whaox_wapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-09 11:49:13.000000 whaox-wapi-1.0.30/whaox_wapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-09 11:49:13.000000 whaox-wapi-1.0.30/whaox_wapi.egg-info/top_level.txt
```

### Comparing `whaox-wapi-1.0.29/LICENSE` & `whaox-wapi-1.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.29/PKG-INFO` & `whaox-wapi-1.0.30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.29
+Version: 1.0.30
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,web,api,requests,post,get
 Description-Content-Type: text/markdown
```

### Comparing `whaox-wapi-1.0.29/README.md` & `whaox-wapi-1.0.30/README.md`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.29/setup.py` & `whaox-wapi-1.0.30/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """
 :authors: WHAOX
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 WHAOX
 """
 
-version = '1.0.29'
+version = '1.0.30'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whaox-wapi',
     version=version,
```

### Comparing `whaox-wapi-1.0.29/wapi/features/GET.py` & `whaox-wapi-1.0.30/wapi/features/GET.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.29/wapi/features/POST.py` & `whaox-wapi-1.0.30/wapi/features/POST.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.29/wapi/features/Route.py` & `whaox-wapi-1.0.30/wapi/features/Route.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from functools import wraps
 from typing import Type
 
 from wapi.utils.is_class import is_class
+from wapi.utils.set_path import set_path
 
 
 def Route(path: str):
     def decorator(obj: Type[object]):
         def class_wrapper():
-            if hasattr(obj.__class__, 'path'):
+            if hasattr(obj, 'path'):
                 obj.path += path
             else:
                 obj.path = path
 
-            for name, cls in vars(obj).items():
-                if hasattr(cls.__class__, 'path'):
-                    cls.__class__.path = obj.path + cls.path
+            set_path(obj)
 
             return obj
 
         @wraps(obj)
         def func_wrapper(self, *args, **kwargs):
             if hasattr(obj.__wrapped__, 'path'):
                 obj.__wrapped__.path = path + obj.__wrapped__.path
```

### Comparing `whaox-wapi-1.0.29/whaox_wapi.egg-info/PKG-INFO` & `whaox-wapi-1.0.30/whaox_wapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.29
+Version: 1.0.30
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,web,api,requests,post,get
 Description-Content-Type: text/markdown
```

