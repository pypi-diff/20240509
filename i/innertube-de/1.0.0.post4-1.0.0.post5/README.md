# Comparing `tmp/innertube-de-1.0.0.post4.tar.gz` & `tmp/innertube-de-1.0.0.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innertube-de-1.0.0.post4.tar", last modified: Sun May  5 10:17:18 2024, max compression
+gzip compressed data, was "innertube-de-1.0.0.post5.tar", last modified: Sun May  5 10:24:33 2024, max compression
```

## Comparing `innertube-de-1.0.0.post4.tar` & `innertube-de-1.0.0.post5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-05 10:17:18.002547 innertube-de-1.0.0.post4/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-05 10:17:18.002547 innertube-de-1.0.0.post4/PKG-INFO
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2708 2024-05-05 10:17:12.000000 innertube-de-1.0.0.post4/README.md
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-05 10:17:17.999213 innertube-de-1.0.0.post4/innertube_de/
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     1651 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/innertube_de/__init__.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2435 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/innertube_de/containers.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2970 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/innertube_de/endpoints.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     1098 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post4/innertube_de/errors.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    60408 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/innertube_de/extractor.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     4223 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post4/innertube_de/itags.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    10562 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/innertube_de/items.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3970 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post4/innertube_de/stream.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     4796 2024-05-02 13:02:55.000000 innertube-de-1.0.0.post4/innertube_de/types.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8634 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/innertube_de/utils.py
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-05 10:17:17.999213 innertube-de-1.0.0.post4/innertube_de.egg-info/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-05 10:17:17.000000 innertube-de-1.0.0.post4/innertube_de.egg-info/PKG-INFO
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)      416 2024-05-05 10:17:17.000000 innertube-de-1.0.0.post4/innertube_de.egg-info/SOURCES.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)        1 2024-05-05 10:17:17.000000 innertube-de-1.0.0.post4/innertube_de.egg-info/dependency_links.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       13 2024-05-05 10:17:17.000000 innertube-de-1.0.0.post4/innertube_de.egg-info/top_level.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       38 2024-05-05 10:17:18.002547 innertube-de-1.0.0.post4/setup.cfg
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)      785 2024-05-05 10:17:07.000000 innertube-de-1.0.0.post4/setup.py
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-05 10:17:17.999213 innertube-de-1.0.0.post4/tests/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)    13856 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/tests/tester.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-05 10:24:33.141213 innertube-de-1.0.0.post5/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-05 10:24:33.141213 innertube-de-1.0.0.post5/PKG-INFO
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2708 2024-05-05 10:24:29.000000 innertube-de-1.0.0.post5/README.md
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-05 10:24:33.137879 innertube-de-1.0.0.post5/innertube_de/
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     1651 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post5/innertube_de/__init__.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2435 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post5/innertube_de/containers.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     3096 2024-05-05 10:24:14.000000 innertube-de-1.0.0.post5/innertube_de/endpoints.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     1098 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post5/innertube_de/errors.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    60408 2024-05-05 10:17:59.000000 innertube-de-1.0.0.post5/innertube_de/extractor.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     4223 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post5/innertube_de/itags.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    10562 2024-05-05 10:17:59.000000 innertube-de-1.0.0.post5/innertube_de/items.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3970 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post5/innertube_de/stream.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     4796 2024-05-02 13:02:55.000000 innertube-de-1.0.0.post5/innertube_de/types.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8634 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post5/innertube_de/utils.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-05 10:24:33.141213 innertube-de-1.0.0.post5/innertube_de.egg-info/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-05 10:24:33.000000 innertube-de-1.0.0.post5/innertube_de.egg-info/PKG-INFO
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)      416 2024-05-05 10:24:33.000000 innertube-de-1.0.0.post5/innertube_de.egg-info/SOURCES.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)        1 2024-05-05 10:24:33.000000 innertube-de-1.0.0.post5/innertube_de.egg-info/dependency_links.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       13 2024-05-05 10:24:33.000000 innertube-de-1.0.0.post5/innertube_de.egg-info/top_level.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       38 2024-05-05 10:24:33.141213 innertube-de-1.0.0.post5/setup.cfg
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)      785 2024-05-05 10:24:23.000000 innertube-de-1.0.0.post5/setup.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-05 10:24:33.141213 innertube-de-1.0.0.post5/tests/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)    13856 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post5/tests/tester.py
```

### Comparing `innertube-de-1.0.0.post4/PKG-INFO` & `innertube-de-1.0.0.post5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: innertube-de
-Version: 1.0.0.post4
+Version: 1.0.0.post5
 Summary: InnerTube Data Extractor
 Home-page: https://github.com/g3nsy/innertube-de
 Author: g3nsy
 Author-email: g3nsydev@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 # InnerTube Data Extractor (ITDE)
-![Version](https://img.shields.io/badge/version-1.0.0-4-blue)
+![Version](https://img.shields.io/badge/version-1.0.0-5-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ITDE is a Python-based tool designed to extract valuable information, including multimedia content and associated metadata, from the data provided by InnerTube, Google's private API. 
 InnerTube serves as a comprehensive source of data, and ITDE empowers developers to seamlessly retrieve and organize essential details from this platform.
 
 ### Features
```

### Comparing `innertube-de-1.0.0.post4/README.md` & `innertube-de-1.0.0.post5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # InnerTube Data Extractor (ITDE)
-![Version](https://img.shields.io/badge/version-1.0.0-4-blue)
+![Version](https://img.shields.io/badge/version-1.0.0-5-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ITDE is a Python-based tool designed to extract valuable information, including multimedia content and associated metadata, from the data provided by InnerTube, Google's private API. 
 InnerTube serves as a comprehensive source of data, and ITDE empowers developers to seamlessly retrieve and organize essential details from this platform.
 
 ### Features
```

### Comparing `innertube-de-1.0.0.post4/innertube_de/__init__.py` & `innertube-de-1.0.0.post5/innertube_de/__init__.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post4/innertube_de/containers.py` & `innertube-de-1.0.0.post5/innertube_de/containers.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post4/innertube_de/endpoints.py` & `innertube-de-1.0.0.post5/innertube_de/endpoints.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from dataclasses import dataclass
 from typing import Optional, Dict
 from innertube_de.types import EndpointType
 
 
-@dataclass(kw_only=True)
+@dataclass(kw_only=True, unsafe_hash=True)
 class Endpoint:
     params: Optional[str] = None
 
     def dump(self) -> Dict:
         return {"params": self.params}
 
     def load(self, data: Dict) -> None:
         self.params = data["params"]
 
 
-@dataclass(kw_only=True)
+@dataclass(kw_only=True, unsafe_hash=True)
 class BrowseEndpoint(Endpoint):
     browse_id: Optional[str] = None
 
     def dump(self) -> Dict:
         d = super().dump()
         d.update({
             "type": EndpointType.BROWSE.value,
@@ -27,15 +27,15 @@
         return d
 
     def load(self, data: Dict) -> None:
         super().load(data)
         self.browse_id = data["browse_id"]
 
 
-@dataclass(kw_only=True)
+@dataclass(kw_only=True, unsafe_hash=True)
 class YouTubeBrowseEndpoint(BrowseEndpoint):
     canonical_base_url: Optional[str] = None
 
     def dump(self) -> Dict:
         d = super().dump()
         d.update({
             "type": EndpointType.YOUTUBE_BROWSE.value,
@@ -44,15 +44,15 @@
         return d
 
     def load(self, data: Dict) -> None:
         super().load(data)
         self.canonical_base_url = data["canonical_base_url"]
 
 
-@dataclass(kw_only=True)
+@dataclass(kw_only=True, unsafe_hash=True)
 class SearchEndpoint(Endpoint):
     query: Optional[str] = None
 
     def dump(self) -> Dict:
         d = super().dump()
         d.update({
             "type": EndpointType.SEARCH.value,
@@ -61,15 +61,15 @@
         return d
 
     def load(self, data: Dict) -> None:
         super().load(data)
         self.query = data["query"]
 
 
-@dataclass(kw_only=True)
+@dataclass(kw_only=True, unsafe_hash=True)
 class WatchEndpoint(Endpoint):
     video_id: Optional[str] = None
     playlist_id: Optional[str] = None
     index: Optional[int] = None
 
     def dump(self) -> Dict:
         d = super().dump()
@@ -84,15 +84,15 @@
     def load(self, data: Dict) -> None:
         super().load(data)
         self.video_id = data["video_id"]
         self.playlist_id = data["playlist_id"]
         self.index = data["index"]
 
 
-@dataclass(kw_only=True)
+@dataclass(kw_only=True, unsafe_hash=True)
 class ContinuationEndpoint(Endpoint):
     continuation: Optional[str] = None
 
     def dump(self) -> Dict:
         d = super().dump()
         d.update({
             "type": EndpointType.CONTINUATION.value,
@@ -101,15 +101,15 @@
         return d
 
     def load(self, data: Dict) -> None:
         super().load(data)
         self.continuation = data["continuation"]
 
 
-@dataclass(kw_only=True)
+@dataclass(kw_only=True, unsafe_hash=True)
 class UrlEndpoint(Endpoint):
     url: Optional[str] = None
 
     def dump(self) -> Dict:
         d = super().dump()
         d.update({
             "type": EndpointType.URL.value,
```

### Comparing `innertube-de-1.0.0.post4/innertube_de/errors.py` & `innertube-de-1.0.0.post5/innertube_de/errors.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post4/innertube_de/extractor.py` & `innertube-de-1.0.0.post5/innertube_de/extractor.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post4/innertube_de/itags.py` & `innertube-de-1.0.0.post5/innertube_de/itags.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post4/innertube_de/items.py` & `innertube-de-1.0.0.post5/innertube_de/items.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post4/innertube_de/stream.py` & `innertube-de-1.0.0.post5/innertube_de/stream.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post4/innertube_de/types.py` & `innertube-de-1.0.0.post5/innertube_de/types.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post4/innertube_de/utils.py` & `innertube-de-1.0.0.post5/innertube_de/utils.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post4/innertube_de.egg-info/PKG-INFO` & `innertube-de-1.0.0.post5/innertube_de.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: innertube-de
-Version: 1.0.0.post4
+Version: 1.0.0.post5
 Summary: InnerTube Data Extractor
 Home-page: https://github.com/g3nsy/innertube-de
 Author: g3nsy
 Author-email: g3nsydev@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 # InnerTube Data Extractor (ITDE)
-![Version](https://img.shields.io/badge/version-1.0.0-4-blue)
+![Version](https://img.shields.io/badge/version-1.0.0-5-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ITDE is a Python-based tool designed to extract valuable information, including multimedia content and associated metadata, from the data provided by InnerTube, Google's private API. 
 InnerTube serves as a comprehensive source of data, and ITDE empowers developers to seamlessly retrieve and organize essential details from this platform.
 
 ### Features
```

### Comparing `innertube-de-1.0.0.post4/setup.py` & `innertube-de-1.0.0.post5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 here = Path(__file__).parent
 long_description = (here / "README.md").read_text()
 
 
 setup(
     name="innertube-de",
-    version="1.0.0-4",
+    version="1.0.0-5",
     description="InnerTube Data Extractor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="g3nsy",
     author_email="g3nsydev@gmail.com",
     python_requires=">=3.6.0",
     url="https://github.com/g3nsy/innertube-de",
```

### Comparing `innertube-de-1.0.0.post4/tests/tester.py` & `innertube-de-1.0.0.post5/tests/tester.py`

 * *Files identical despite different names*

