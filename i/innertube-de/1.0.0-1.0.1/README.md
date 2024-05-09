# Comparing `tmp/innertube-de-1.0.0.tar.gz` & `tmp/innertube-de-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innertube-de-1.0.0.tar", last modified: Thu May  9 16:06:30 2024, max compression
+gzip compressed data, was "innertube-de-1.0.1.tar", last modified: Thu May  9 17:28:27 2024, max compression
```

## Comparing `innertube-de-1.0.0.tar` & `innertube-de-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-09 16:06:30.391842 innertube-de-1.0.0/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     4985 2024-05-09 16:06:30.391842 innertube-de-1.0.0/PKG-INFO
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     4620 2024-05-09 15:34:13.000000 innertube-de-1.0.0/README.md
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-09 16:06:30.391842 innertube-de-1.0.0/innertube_de/
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     1687 2024-05-06 08:10:17.000000 innertube-de-1.0.0/innertube_de/__init__.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2264 2024-05-09 15:26:23.000000 innertube-de-1.0.0/innertube_de/containers.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     3079 2024-05-06 08:10:17.000000 innertube-de-1.0.0/innertube_de/endpoints.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     1105 2024-05-07 10:58:33.000000 innertube-de-1.0.0/innertube_de/errors.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    63412 2024-05-09 15:26:19.000000 innertube-de-1.0.0/innertube_de/extractor.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    11414 2024-05-09 15:26:05.000000 innertube-de-1.0.0/innertube_de/items.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     5224 2024-05-08 16:53:23.000000 innertube-de-1.0.0/innertube_de/types.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     7359 2024-05-08 19:01:06.000000 innertube-de-1.0.0/innertube_de/utils.py
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-09 16:06:30.391842 innertube-de-1.0.0/innertube_de.egg-info/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     4985 2024-05-09 16:06:30.000000 innertube-de-1.0.0/innertube_de.egg-info/PKG-INFO
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)      371 2024-05-09 16:06:30.000000 innertube-de-1.0.0/innertube_de.egg-info/SOURCES.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)        1 2024-05-09 16:06:30.000000 innertube-de-1.0.0/innertube_de.egg-info/dependency_links.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       13 2024-05-09 16:06:30.000000 innertube-de-1.0.0/innertube_de.egg-info/top_level.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       38 2024-05-09 16:06:30.391842 innertube-de-1.0.0/setup.cfg
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)      783 2024-05-08 19:05:17.000000 innertube-de-1.0.0/setup.py
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-09 16:06:30.391842 innertube-de-1.0.0/tests/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)    13558 2024-05-09 15:31:15.000000 innertube-de-1.0.0/tests/tester.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-09 17:28:27.863369 innertube-de-1.0.1/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     4985 2024-05-09 17:28:27.863369 innertube-de-1.0.1/PKG-INFO
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     4621 2024-05-09 17:28:24.000000 innertube-de-1.0.1/README.md
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-09 17:28:27.860036 innertube-de-1.0.1/innertube_de/
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     1625 2024-05-09 17:28:24.000000 innertube-de-1.0.1/innertube_de/__init__.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2262 2024-05-09 17:28:24.000000 innertube-de-1.0.1/innertube_de/containers.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     3079 2024-05-06 08:10:17.000000 innertube-de-1.0.1/innertube_de/endpoints.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     1105 2024-05-07 10:58:33.000000 innertube-de-1.0.1/innertube_de/errors.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    63412 2024-05-09 15:26:19.000000 innertube-de-1.0.1/innertube_de/extractor.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    11414 2024-05-09 15:26:05.000000 innertube-de-1.0.1/innertube_de/items.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     5224 2024-05-08 16:53:23.000000 innertube-de-1.0.1/innertube_de/types.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     7359 2024-05-08 19:01:06.000000 innertube-de-1.0.1/innertube_de/utils.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-09 17:28:27.863369 innertube-de-1.0.1/innertube_de.egg-info/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     4985 2024-05-09 17:28:27.000000 innertube-de-1.0.1/innertube_de.egg-info/PKG-INFO
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)      371 2024-05-09 17:28:27.000000 innertube-de-1.0.1/innertube_de.egg-info/SOURCES.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)        1 2024-05-09 17:28:27.000000 innertube-de-1.0.1/innertube_de.egg-info/dependency_links.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       13 2024-05-09 17:28:27.000000 innertube-de-1.0.1/innertube_de.egg-info/top_level.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       38 2024-05-09 17:28:27.863369 innertube-de-1.0.1/setup.cfg
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)      783 2024-05-09 17:28:24.000000 innertube-de-1.0.1/setup.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-09 17:28:27.863369 innertube-de-1.0.1/tests/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)    13940 2024-05-09 17:28:24.000000 innertube-de-1.0.1/tests/tester.py
```

### Comparing `innertube-de-1.0.0/PKG-INFO` & `innertube-de-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: innertube-de
-Version: 1.0.0
+Version: 1.0.1
 Summary: InnerTube Data Extractor
 Home-page: https://github.com/g3nsy/innertube-de
 Author: g3nsy
 Author-email: g3nsydev@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 # innertube-de (InnerTube Data Extractor)
-![Version](https://img.shields.io/badge/version-1.0.0-blue)
+![Version](https://img.shields.io/badge/version-1.0.1-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 innertube-de is a python tool for extracting, organizing and classifying data provided by InnerTube, Google's private API.
 The extraction process returns a Container object containing all relevant information.
 Regardless of the InnerTube client (WEB, WEB_REMIX, etc...) the extraction is performed using a single method.
 See also https://github.com/tombulled/innertube as an example of an InnerTube client.
 ### Installation
@@ -30,15 +30,15 @@
 # from https://github.com/tombulled/innertube
 from innertube.clients import InnerTube
 from innertube_de import InnerTubeDE, SongItem, AlbumItem
 
 client = InnerTube("WEB_REMIX")  # YouTube Music client
 extractor = InnerTubeDE(include_all_urls=False)  # InnerTube data extractor 
 
-unclear_data = client.search("Rioji Ikeda")
+unclear_data = client.search("Ryoji Ikeda")
 clear_data = extractor.extract(unclear_data)
 
 # the item at the top of the results
 print("header:", clear_data.header)
 
 # multimedia content is organized inside the shelves
 for shelf in clear_data:
@@ -72,15 +72,15 @@
 The following methods are currently supported and tested:
 
 |                              | YouTube | YouTubeMusic | YouTubeKids | YouTubeStudio |
 |------------------------------|---------|--------------|-------------|---------------|
 | search                       | &check; | &check;      |             |               |
 | browse                       | &check; | &check;      |             |               |
 | next                         | &check; | &check;      |             |               |
-| player                       | &check; | &check;      |             |               |
+| player                       |         |              |             |               |
 | guide                        |         |              |             |               |
 | config                       |         |              |             |               |
 | get_transcript               |         |              |             |               |
 | music/get_search_suggestions |         |              |             |               |
 | music/get_queue              |         |              |             |               |
```

### Comparing `innertube-de-1.0.0/README.md` & `innertube-de-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # innertube-de (InnerTube Data Extractor)
-![Version](https://img.shields.io/badge/version-1.0.0-blue)
+![Version](https://img.shields.io/badge/version-1.0.1-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 innertube-de is a python tool for extracting, organizing and classifying data provided by InnerTube, Google's private API.
 The extraction process returns a Container object containing all relevant information.
 Regardless of the InnerTube client (WEB, WEB_REMIX, etc...) the extraction is performed using a single method.
 See also https://github.com/tombulled/innertube as an example of an InnerTube client.
 ### Installation
@@ -17,15 +17,15 @@
 # from https://github.com/tombulled/innertube
 from innertube.clients import InnerTube
 from innertube_de import InnerTubeDE, SongItem, AlbumItem
 
 client = InnerTube("WEB_REMIX")  # YouTube Music client
 extractor = InnerTubeDE(include_all_urls=False)  # InnerTube data extractor 
 
-unclear_data = client.search("Rioji Ikeda")
+unclear_data = client.search("Ryoji Ikeda")
 clear_data = extractor.extract(unclear_data)
 
 # the item at the top of the results
 print("header:", clear_data.header)
 
 # multimedia content is organized inside the shelves
 for shelf in clear_data:
@@ -59,15 +59,15 @@
 The following methods are currently supported and tested:
 
 |                              | YouTube | YouTubeMusic | YouTubeKids | YouTubeStudio |
 |------------------------------|---------|--------------|-------------|---------------|
 | search                       | &check; | &check;      |             |               |
 | browse                       | &check; | &check;      |             |               |
 | next                         | &check; | &check;      |             |               |
-| player                       | &check; | &check;      |             |               |
+| player                       |         |              |             |               |
 | guide                        |         |              |             |               |
 | config                       |         |              |             |               |
 | get_transcript               |         |              |             |               |
 | music/get_search_suggestions |         |              |             |               |
 | music/get_queue              |         |              |             |               |
 
 
@@ -114,8 +114,8 @@
         }
     ]
 }
 ```
 
 ## Disclaimer
 innertube-de heavily relies on data provided by InnerTube. The reliability and functionality of this code may vary over time, as they are subject to any changes or updates made by InnerTube's data structure or API. 
-It's recommended to stay updated with any releases or announcements related to innertube-de.
+It's recommended to stay updated with any releases or announcements related to innertube-de.
```

### Comparing `innertube-de-1.0.0/innertube_de/__init__.py` & `innertube-de-1.0.1/innertube_de/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,16 +49,14 @@
     ItemType,
     EndpointType,
     ItemStructType,
     ShelfStructType,
     ContinuationStrucType
 )
 
-from innertube_de.stream import StreamData
-
 
 __all__ = [
     "utils",
 
     "extract",
     "InnerTubeDE",
 
@@ -95,10 +93,8 @@
     "YouTubeMusicPlaylistItem",
 
     "ItemType",
     "EndpointType",
     "ItemStructType",
     "ShelfStructType",
     "ContinuationStrucType",
-
-    "StreamData"
 ]
```

### Comparing `innertube-de-1.0.0/innertube_de/containers.py` & `innertube-de-1.0.1/innertube_de/containers.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 
 
 @dataclass(kw_only=True)
 class Container(List[Shelf]):
     header: Optional[Item] = None 
 
     def dump(self) -> Dict:
-        return {
-            "header": None if self.header is None else self.header.dump(),
-            "contents": [shelf.dump() for shelf in self]
-        }
+        return dict(
+            header=None if self.header is None else self.header.dump(),
+            contents=[shelf.dump() for shelf in self]
+        )
 
     def load(self, data: Dict) -> None:
         self.header = None if data["header"] is None else get_item(data["header"])
         for shelf_data in data["contents"]:
             match shelf_data["type"]:
                 case ShelfType.SHELF.value:
                     shelf = Shelf()
```

### Comparing `innertube-de-1.0.0/innertube_de/endpoints.py` & `innertube-de-1.0.1/innertube_de/endpoints.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0/innertube_de/errors.py` & `innertube-de-1.0.1/innertube_de/errors.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0/innertube_de/extractor.py` & `innertube-de-1.0.1/innertube_de/extractor.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0/innertube_de/items.py` & `innertube-de-1.0.1/innertube_de/items.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0/innertube_de/types.py` & `innertube-de-1.0.1/innertube_de/types.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0/innertube_de/utils.py` & `innertube-de-1.0.1/innertube_de/utils.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0/innertube_de.egg-info/PKG-INFO` & `innertube-de-1.0.1/innertube_de.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: innertube-de
-Version: 1.0.0
+Version: 1.0.1
 Summary: InnerTube Data Extractor
 Home-page: https://github.com/g3nsy/innertube-de
 Author: g3nsy
 Author-email: g3nsydev@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 # innertube-de (InnerTube Data Extractor)
-![Version](https://img.shields.io/badge/version-1.0.0-blue)
+![Version](https://img.shields.io/badge/version-1.0.1-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 innertube-de is a python tool for extracting, organizing and classifying data provided by InnerTube, Google's private API.
 The extraction process returns a Container object containing all relevant information.
 Regardless of the InnerTube client (WEB, WEB_REMIX, etc...) the extraction is performed using a single method.
 See also https://github.com/tombulled/innertube as an example of an InnerTube client.
 ### Installation
@@ -30,15 +30,15 @@
 # from https://github.com/tombulled/innertube
 from innertube.clients import InnerTube
 from innertube_de import InnerTubeDE, SongItem, AlbumItem
 
 client = InnerTube("WEB_REMIX")  # YouTube Music client
 extractor = InnerTubeDE(include_all_urls=False)  # InnerTube data extractor 
 
-unclear_data = client.search("Rioji Ikeda")
+unclear_data = client.search("Ryoji Ikeda")
 clear_data = extractor.extract(unclear_data)
 
 # the item at the top of the results
 print("header:", clear_data.header)
 
 # multimedia content is organized inside the shelves
 for shelf in clear_data:
@@ -72,15 +72,15 @@
 The following methods are currently supported and tested:
 
 |                              | YouTube | YouTubeMusic | YouTubeKids | YouTubeStudio |
 |------------------------------|---------|--------------|-------------|---------------|
 | search                       | &check; | &check;      |             |               |
 | browse                       | &check; | &check;      |             |               |
 | next                         | &check; | &check;      |             |               |
-| player                       | &check; | &check;      |             |               |
+| player                       |         |              |             |               |
 | guide                        |         |              |             |               |
 | config                       |         |              |             |               |
 | get_transcript               |         |              |             |               |
 | music/get_search_suggestions |         |              |             |               |
 | music/get_queue              |         |              |             |               |
```

### Comparing `innertube-de-1.0.0/setup.py` & `innertube-de-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 here = Path(__file__).parent
 long_description = (here / "README.md").read_text()
 
 
 setup(
     name="innertube-de",
-    version="1.0.0",
+    version="1.0.1",
     description="InnerTube Data Extractor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="g3nsy",
     author_email="g3nsydev@gmail.com",
     python_requires=">=3.6.0",
     url="https://github.com/g3nsy/innertube-de",
```

### Comparing `innertube-de-1.0.0/tests/tester.py` & `innertube-de-1.0.1/tests/tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
             target: paths.Target,
             verbose: bool = False, 
             save_data: bool = True,
             log_errors: bool = True,
             stack_info: bool = True,
             exc_info: bool = True,
             enable_exceptions: bool = True,
-            include_all_urls: bool = True
+            include_all_urls: bool = True,
+            fit_screen: bool = False
     ) -> None:
 
         self.target = target
         self.innertube = innertube
         self.extractor = InnerTubeDE(
             log_errors=log_errors,
             stack_info=stack_info,
@@ -52,14 +53,15 @@
 
         self.ext_containers: Dict[str, Optional[Container]] = {}  # extracted containers
         self.ser_containers: Dict[str, Optional[Dict]] = {}       # serialized containers
         self.des_containers: Dict[str, Optional[Container]] = {}  # deserialized containers
 
         self.save_data = save_data
         self.verbose = verbose
+        self.fit_screen = fit_screen
 
         with open(paths.TEST_DATA, mode="r") as file:
             test_data = json.loads(file.read())
 
         target_tests = test_data[target.value]
         self.test_sear = target_tests["sear"]  # search tests
         self.test_brow = target_tests["brow"]  # browse tests
@@ -208,15 +210,15 @@
                 with open(os.path.join(self.errs_path, f"{name}.json"), mode="w") as file:
                     json.dump(innertube_data, file, indent=4)  # noqa # type: ignore
 
         else:
             self.ext_log.append(f"{name} [green][OK][/green]")
             self.ext_containers[name] = ext_container
             if self.verbose:
-                print_container(ext_container)
+                print_container(ext_container, fit_screen=self.fit_screen)
             if self.save_data:
                 with open(os.path.join(self.inne_path, f"{name}.json"), mode="w") as file:
                     json.dump(innertube_data, file, indent=4)
 
 
 def print_logs(
         testers: List[Tester], 
@@ -288,27 +290,32 @@
                 else:
                     if j > 0:
                         table_line += " " * distance
                     table_line += get_table_line(tester, i)
             cs.print(table_line)
 
 
-def print_container(container: Container) -> None:
+def print_container(container: Container, fit_screen: bool = False) -> None:
+    width = -1
+    if fit_screen is True:
+        td = get_terminal_dimensions()
+        if td is not None:
+            width = td.width
     for shelf in container:
         shelf_type = "CardShelf" if isinstance(shelf, CardShelf) else "Shelf"
         cs.print()
         cs.print(f"{shelf_type} title: {shelf.title}")
         cs.print(f"{shelf_type} endpoint: {shelf.endpoint}")
         if isinstance(shelf, CardShelf):
             cs.print(f"{shelf_type} Item: {shelf.item}")
         cs.print(f"{shelf_type} Items: ", end="")
         if len(shelf) != 0:
             cs.print("\n", end="")
             for item in shelf:
-                cs.print(f"{str(item)}")
+                cs.print(f"{str(item)[:width]}")
         else:
             cs.print("None")
 
 
 def get_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--verbose', '-v', action='store_false')
@@ -317,14 +324,15 @@
     parser.add_argument('--log-errors', '-le', action='store_false')
     parser.add_argument('--stack-info', '-si', action='store_false')
     parser.add_argument('--exc-info', '-ei', action='store_false')
     parser.add_argument('--include-all-urls', '-iau', action='store_false')
     parser.add_argument('--youtube-music', '-ym', action='store_false')
     parser.add_argument('--youtube', '-yt', action='store_false')
     parser.add_argument('--vertical-mode', '-vm', action='store_true')
+    parser.add_argument('--fit-screen', '-fs', action='store_true')
     return parser
 
 
 def main():
     parser = get_parser()
     args = parser.parse_args()
 
@@ -343,15 +351,16 @@
             save_data=args.save_data,
 
             # InnerTubeDE
             log_errors=args.log_errors,
             stack_info=args.stack_info,
             exc_info=args.exc_info,
             enable_exceptions=args.enable_exceptions,
-            include_all_urls=args.include_all_urls
+            include_all_urls=args.include_all_urls,
+            fit_screen=args.fit_screen
         )
 
         testers.append(_tester)
 
     for _tester in testers:
         _tester.test_search_extraction()
         _tester.test_browse_extraction()
```

