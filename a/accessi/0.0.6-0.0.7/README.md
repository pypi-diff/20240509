# Comparing `tmp/accessi-0.0.6.tar.gz` & `tmp/accessi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accessi-0.0.6.tar", last modified: Mon Apr 29 18:53:41 2024, max compression
+gzip compressed data, was "accessi-0.0.7.tar", last modified: Thu May  9 07:54:40 2024, max compression
```

## Comparing `accessi-0.0.6.tar` & `accessi-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:53:41.094946 accessi-0.0.6/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2024-04-29 18:53:29.000000 accessi-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1427 2024-04-29 18:53:41.090946 accessi-0.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      831 2024-04-29 18:53:29.000000 accessi-0.0.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      578 2024-04-29 18:53:29.000000 accessi-0.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 18:53:41.094946 accessi-0.0.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:53:41.090946 accessi-0.0.6/src/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 18:53:29.000000 accessi-0.0.6/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:53:41.090946 accessi-0.0.6/src/accessi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1427 2024-04-29 18:53:41.000000 accessi-0.0.6/src/accessi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      218 2024-04-29 18:53:41.000000 accessi-0.0.6/src/accessi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 18:53:41.000000 accessi-0.0.6/src/accessi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-29 18:53:41.000000 accessi-0.0.6/src/accessi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    35905 2024-04-29 18:53:29.000000 accessi-0.0.6/src/accessi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:53:41.090946 accessi-0.0.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)     6311 2024-04-29 18:53:29.000000 accessi-0.0.6/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 07:54:40.191392 accessi-0.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-05-09 07:54:28.000000 accessi-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-05-09 07:54:40.191392 accessi-0.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2024-05-09 07:54:28.000000 accessi-0.0.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-05-09 07:54:28.000000 accessi-0.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 07:54:40.191392 accessi-0.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 07:54:40.187392 accessi-0.0.7/src/
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2024-05-09 07:54:28.000000 accessi-0.0.7/src/DataConversion.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 07:54:28.000000 accessi-0.0.7/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 07:54:40.191392 accessi-0.0.7/src/accessi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-05-09 07:54:40.000000 accessi-0.0.7/src/accessi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-09 07:54:40.000000 accessi-0.0.7/src/accessi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 07:54:40.000000 accessi-0.0.7/src/accessi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-09 07:54:40.000000 accessi-0.0.7/src/accessi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    35905 2024-05-09 07:54:28.000000 accessi-0.0.7/src/accessi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 07:54:40.191392 accessi-0.0.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6190 2024-05-09 07:54:28.000000 accessi-0.0.7/tests/tests.py
```

### Comparing `accessi-0.0.6/LICENSE` & `accessi-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `accessi-0.0.6/pyproject.toml` & `accessi-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "accessi"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Martin Reinok", email="m.reinok@student.utwente.nl" },
 ]
 description = "Library for Siemens Access-i MR Scanner Interface to integrate and control the MR Scanner."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `accessi-0.0.6/src/accessi.py` & `accessi-0.0.7/src/accessi.py`

 * *Files identical despite different names*

### Comparing `accessi-0.0.6/tests/tests.py` & `accessi-0.0.7/tests/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Usage example and tests to make sure the library works.
 Siemens Access-i simulator should be running for this to work (or real MRI system with appropriate IP-address).
 """
 import json
-from asyncio import LifoQueue
-from types import SimpleNamespace
-from src import accessi as Access
-import threading
 import asyncio
-import time
+import numpy as np
+from src import accessi as Access
+from types import SimpleNamespace
+from src import DataConversion
 
 Access.config.ip_address = "127.0.0.1"
 Access.config.version = "v2"
 
 """
 Remote Service
 """
@@ -185,20 +184,19 @@
         output = Access.TemplateExecution.start(template_id).result.success
         print(f"start: {output}")
         assert output is True
 
         # Receive one image and quit
         while True:
             image_data = await websocket.recv()
-            if '"imageStream"' in image_data:
-                image_data = json.dumps(Access.handle_websocket_message(image_data))
-                image_data = json.loads(image_data, object_hook=lambda d: SimpleNamespace(**d))
-                print(f"Websocket callback image dimensions: "
-                      f"{image_data[2].value.image.dimensions.columns},"
-                      f"{image_data[2].value.image.dimensions.rows} ")
+            image, metadata = DataConversion.websocket_imagestream_to_image(image_data, 8)
+            if image is not None:
+                print(f"Websocket callback image dimensions: {image.shape}, "
+                      f"Image max value: {np.max(image)}, "
+                      f"Image min value: {np.min(image)}")
                 break
 
         """
         Done, cleanup
         """
         print("Tests done, cleaning up")
         Access.TemplateExecution.stop()
```

