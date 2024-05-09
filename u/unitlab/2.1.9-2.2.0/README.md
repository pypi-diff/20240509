# Comparing `tmp/unitlab-2.1.9.tar.gz` & `tmp/unitlab-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-2.1.9.tar", last modified: Mon Apr 15 06:05:00 2024, max compression
+gzip compressed data, was "unitlab-2.2.0.tar", last modified: Thu May  9 07:18:41 2024, max compression
```

## Comparing `unitlab-2.1.9.tar` & `unitlab-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-15 06:05:00.721197 unitlab-2.1.9/
--rw-rw-r--   0 me        (1000) me        (1000)     1069 2024-02-13 07:39:37.000000 unitlab-2.1.9/LICENSE.md
--rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-15 06:05:00.721197 unitlab-2.1.9/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     1450 2024-04-09 12:41:44.000000 unitlab-2.1.9/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2024-04-15 06:05:00.721197 unitlab-2.1.9/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1092 2024-04-15 06:01:52.000000 unitlab-2.1.9/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-15 06:05:00.721197 unitlab-2.1.9/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-15 06:05:00.721197 unitlab-2.1.9/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)      214 2024-04-05 11:53:23.000000 unitlab-2.1.9/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)       29 2024-03-06 15:43:31.000000 unitlab-2.1.9/src/unitlab/__main__.py
--rw-rw-r--   0 me        (1000) me        (1000)    11952 2024-04-15 05:57:27.000000 unitlab-2.1.9/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)    12386 2024-04-05 09:59:30.000000 unitlab-2.1.9/src/unitlab/dataset.py
--rw-rw-r--   0 me        (1000) me        (1000)      950 2024-04-05 12:19:27.000000 unitlab-2.1.9/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     4547 2024-04-15 05:56:37.000000 unitlab-2.1.9/src/unitlab/main.py
--rw-rw-r--   0 me        (1000) me        (1000)     1888 2024-04-15 06:00:14.000000 unitlab-2.1.9/src/unitlab/utils.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-15 06:05:00.721197 unitlab-2.1.9/src/unitlab.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-15 06:05:00.000000 unitlab-2.1.9/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      411 2024-04-15 06:05:00.000000 unitlab-2.1.9/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2024-04-15 06:05:00.000000 unitlab-2.1.9/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       45 2024-04-15 06:05:00.000000 unitlab-2.1.9/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       48 2024-04-15 06:05:00.000000 unitlab-2.1.9/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2024-04-15 06:05:00.000000 unitlab-2.1.9/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-05-09 07:18:41.845503 unitlab-2.2.0/
+-rw-rw-r--   0 me        (1000) me        (1000)     1069 2024-02-13 07:39:37.000000 unitlab-2.2.0/LICENSE.md
+-rw-r--r--   0 me        (1000) me        (1000)      793 2024-05-09 07:18:41.845503 unitlab-2.2.0/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     1450 2024-04-09 12:41:44.000000 unitlab-2.2.0/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2024-05-09 07:18:41.845503 unitlab-2.2.0/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1092 2024-05-09 07:18:15.000000 unitlab-2.2.0/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-05-09 07:18:41.845503 unitlab-2.2.0/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-05-09 07:18:41.845503 unitlab-2.2.0/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)      214 2024-04-05 11:53:23.000000 unitlab-2.2.0/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)       29 2024-03-06 15:43:31.000000 unitlab-2.2.0/src/unitlab/__main__.py
+-rw-rw-r--   0 me        (1000) me        (1000)    11955 2024-05-09 06:53:40.000000 unitlab-2.2.0/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)    12386 2024-04-05 09:59:30.000000 unitlab-2.2.0/src/unitlab/dataset.py
+-rw-rw-r--   0 me        (1000) me        (1000)      950 2024-04-05 12:19:27.000000 unitlab-2.2.0/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     4547 2024-04-15 05:56:37.000000 unitlab-2.2.0/src/unitlab/main.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1888 2024-04-15 06:00:14.000000 unitlab-2.2.0/src/unitlab/utils.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-05-09 07:18:41.845503 unitlab-2.2.0/src/unitlab.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)      793 2024-05-09 07:18:41.000000 unitlab-2.2.0/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      411 2024-05-09 07:18:41.000000 unitlab-2.2.0/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2024-05-09 07:18:41.000000 unitlab-2.2.0/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       45 2024-05-09 07:18:41.000000 unitlab-2.2.0/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       48 2024-05-09 07:18:41.000000 unitlab-2.2.0/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2024-05-09 07:18:41.000000 unitlab-2.2.0/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-2.1.9/LICENSE.md` & `unitlab-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.9/PKG-INFO` & `unitlab-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 2.1.9
+Version: 2.2.0
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `unitlab-2.1.9/README.md` & `unitlab-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.9/setup.py` & `unitlab-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="2.1.9",
+    version="2.2.0",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
```

### Comparing `unitlab-2.1.9/src/unitlab/client.py` & `unitlab-2.2.0/src/unitlab/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import aiofiles
 import aiohttp
 import requests
 import tqdm
 
 from . import exceptions
 from .dataset import DatasetUploadHandler
-from .utils import handle_exceptions
+from .utils import get_api_url, handle_exceptions
 
 logger = logging.getLogger(__name__)
 
 
 class UnitlabClient:
     """A client with a connection to the Unitlab.ai platform.
 
@@ -45,17 +45,17 @@
 
     Args:
         api_key: Your Unitlab.ai API key. If no API key given, reads ``UNITLAB_API_KEY`` from the environment. Defaults to :obj:`None`.
     Raises:
         :exc:`~unitlab.exceptions.AuthenticationError`: If an invalid API key is used or (when not passing the API key directly) if ``UNITLAB_API_KEY`` is not found in your environment.
     """
 
-    def __init__(self, api_key, api_url: str = "https://api.unitlab.ai"):
+    def __init__(self, api_key, api_url=None):
         self.api_key = api_key
-        self.api_url = api_url
+        self.api_url = api_url or get_api_url()
         self.api_session = requests.Session()
         adapter = requests.adapters.HTTPAdapter(max_retries=3)
         self.api_session.mount("http://", adapter)
         self.api_session.mount("https://", adapter)
 
     def close(self) -> None:
         """Close :class:`UnitlabClient` connections.
```

### Comparing `unitlab-2.1.9/src/unitlab/dataset.py` & `unitlab-2.2.0/src/unitlab/dataset.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.9/src/unitlab/exceptions.py` & `unitlab-2.2.0/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.9/src/unitlab/main.py` & `unitlab-2.2.0/src/unitlab/main.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.9/src/unitlab/utils.py` & `unitlab-2.2.0/src/unitlab/utils.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.9/src/unitlab.egg-info/PKG-INFO` & `unitlab-2.2.0/src/unitlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 2.1.9
+Version: 2.2.0
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

