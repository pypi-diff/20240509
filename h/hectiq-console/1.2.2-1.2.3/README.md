# Comparing `tmp/hectiq_console-1.2.2.tar.gz` & `tmp/hectiq_console-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python-collector/dist/.tmp-2lq6l6d3/hectiq_console-1.2.2.tar", last modified: Fri Apr 19 13:06:35 2024, max compression
+gzip compressed data, was "/home/runner/work/console/console/python-collector/dist/.tmp-igiudyko/hectiq_console-1.2.3.tar", last modified: Thu May  9 17:45:14 2024, max compression
```

## Comparing `hectiq_console-1.2.2.tar` & `hectiq_console-1.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    37370 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console/starlette/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/starlette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/starlette/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/utils/batch_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/utils/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/hectiq_console/utils/log_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:06:28.000000 hectiq_console-1.2.2/hectiq_console.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/hectiq_console.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:06:35.000000 hectiq_console-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-19 13:06:23.000000 hectiq_console-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/hectiq_console/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/hectiq_console/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/hectiq_console/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/hectiq_console/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/hectiq_console/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/hectiq_console/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37366 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/hectiq_console/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/hectiq_console/starlette/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/hectiq_console/starlette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/hectiq_console/starlette/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/hectiq_console/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/hectiq_console/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/hectiq_console/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/hectiq_console/utils/batch_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/hectiq_console/utils/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/hectiq_console/utils/log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/hectiq_console.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/hectiq_console.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/hectiq_console.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/hectiq_console.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/hectiq_console.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:45:07.000000 hectiq_console-1.2.3/hectiq_console.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/hectiq_console.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/hectiq_console.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:45:14.000000 hectiq_console-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-09 17:45:05.000000 hectiq_console-1.2.3/setup.py
```

### Comparing `hectiq_console-1.2.2/LICENSE` & `hectiq_console-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.2/PKG-INFO` & `hectiq_console-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectiq_console
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python client to use the Hectiq Console
 Home-page: https://console.hectiq.ai
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `hectiq_console-1.2.2/README.md` & `hectiq_console-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.2/hectiq_console/cli/__init__.py` & `hectiq_console-1.2.3/hectiq_console/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.2/hectiq_console/cli/auth.py` & `hectiq_console-1.2.3/hectiq_console/cli/auth.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.2/hectiq_console/functional.py` & `hectiq_console-1.2.3/hectiq_console/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,16 +369,16 @@
             Defaults to None.
     """
     resource = get_resource(resource)
     headers = get_authentification_headers()
 
     params = {
         "fields": fields,
-        "created_from_date": from_date.toisoformat() if from_date is not None else None,
-        "created_to_date": to_date.toisoformat() if to_date is not None else None,
+        "created_from_date": from_date.isoformat() if from_date is not None else None,
+        "created_to_date": to_date.isoformat() if to_date is not None else None,
         "labels": labels,
         "label_set": label_set,
         "annotated_by": annotated_by,
         "annotated_by_set": annotated_by_set,
         "page": page,
         "limit": limit,
         "order_by": order_by,
```

### Comparing `hectiq_console-1.2.2/hectiq_console/starlette/middleware.py` & `hectiq_console-1.2.3/hectiq_console/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.2/hectiq_console/upload.py` & `hectiq_console-1.2.3/hectiq_console/upload.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.2/hectiq_console/utils/batch_fetch.py` & `hectiq_console-1.2.3/hectiq_console/utils/batch_fetch.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.2/hectiq_console/utils/log_handler.py` & `hectiq_console-1.2.3/hectiq_console/utils/log_handler.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.2/hectiq_console.egg-info/PKG-INFO` & `hectiq_console-1.2.3/hectiq_console.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectiq-console
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python client to use the Hectiq Console
 Home-page: https://console.hectiq.ai
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `hectiq_console-1.2.2/hectiq_console.egg-info/SOURCES.txt` & `hectiq_console-1.2.3/hectiq_console.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.2/setup.py` & `hectiq_console-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
-__version__ = '1.2.2'
+__version__ = '1.2.3'
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 requirements = [
     "requests",
     "toml",
```

