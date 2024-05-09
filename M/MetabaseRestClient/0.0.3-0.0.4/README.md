# Comparing `tmp/metabaserestclient-0.0.3.tar.gz` & `tmp/metabaserestclient-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabaserestclient-0.0.3.tar", last modified: Wed Apr 17 19:11:03 2024, max compression
+gzip compressed data, was "metabaserestclient-0.0.4.tar", last modified: Thu May  9 08:10:12 2024, max compression
```

## Comparing `metabaserestclient-0.0.3.tar` & `metabaserestclient-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-04-17 19:11:03.444020 metabaserestclient-0.0.3/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2023-05-15 01:16:08.000000 metabaserestclient-0.0.3/LICENSE
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-04-17 19:11:03.443655 metabaserestclient-0.0.3/MetabaseRestClient.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2049 2024-04-17 19:11:03.000000 metabaserestclient-0.0.3/MetabaseRestClient.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      400 2024-04-17 19:11:03.000000 metabaserestclient-0.0.3/MetabaseRestClient.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2024-04-17 19:11:03.000000 metabaserestclient-0.0.3/MetabaseRestClient.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2024-04-17 19:11:03.000000 metabaserestclient-0.0.3/MetabaseRestClient.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2024-04-17 19:11:03.000000 metabaserestclient-0.0.3/MetabaseRestClient.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2049 2024-04-17 19:11:03.443833 metabaserestclient-0.0.3/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1442 2024-04-17 19:04:03.000000 metabaserestclient-0.0.3/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-04-17 19:11:03.443069 metabaserestclient-0.0.3/metabase/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      151 2024-04-17 14:31:46.000000 metabaserestclient-0.0.3/metabase/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      323 2024-04-17 14:42:13.000000 metabaserestclient-0.0.3/metabase/exception.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-05-15 01:16:08.000000 metabaserestclient-0.0.3/metabase/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-04-17 19:11:03.443472 metabaserestclient-0.0.3/metabase/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       46 2024-04-17 14:31:46.000000 metabaserestclient-0.0.3/metabase/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1006 2024-04-17 17:59:44.000000 metabaserestclient-0.0.3/metabase/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1807 2024-04-17 18:34:41.000000 metabaserestclient-0.0.3/metabase/service/metabase_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2024-04-17 19:11:03.444095 metabaserestclient-0.0.3/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      912 2024-04-17 19:10:55.000000 metabaserestclient-0.0.3/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-05-09 08:10:12.767581 metabaserestclient-0.0.4/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2023-05-15 01:16:08.000000 metabaserestclient-0.0.4/LICENSE
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-05-09 08:10:12.767157 metabaserestclient-0.0.4/MetabaseRestClient.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2049 2024-05-09 08:10:12.000000 metabaserestclient-0.0.4/MetabaseRestClient.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      400 2024-05-09 08:10:12.000000 metabaserestclient-0.0.4/MetabaseRestClient.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2024-05-09 08:10:12.000000 metabaserestclient-0.0.4/MetabaseRestClient.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2024-05-09 08:10:12.000000 metabaserestclient-0.0.4/MetabaseRestClient.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2024-05-09 08:10:12.000000 metabaserestclient-0.0.4/MetabaseRestClient.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2049 2024-05-09 08:10:12.767365 metabaserestclient-0.0.4/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1442 2024-04-17 19:04:03.000000 metabaserestclient-0.0.4/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-05-09 08:10:12.766539 metabaserestclient-0.0.4/metabase/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      151 2024-04-17 14:31:46.000000 metabaserestclient-0.0.4/metabase/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      323 2024-04-17 14:42:13.000000 metabaserestclient-0.0.4/metabase/exception.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-05-15 01:16:08.000000 metabaserestclient-0.0.4/metabase/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-05-09 08:10:12.766958 metabaserestclient-0.0.4/metabase/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       46 2024-04-17 14:31:46.000000 metabaserestclient-0.0.4/metabase/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1006 2024-04-17 17:59:44.000000 metabaserestclient-0.0.4/metabase/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2081 2024-05-09 08:10:00.000000 metabaserestclient-0.0.4/metabase/service/metabase_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2024-05-09 08:10:12.767625 metabaserestclient-0.0.4/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      912 2024-05-09 08:10:00.000000 metabaserestclient-0.0.4/setup.py
```

### Comparing `metabaserestclient-0.0.3/LICENSE` & `metabaserestclient-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metabaserestclient-0.0.3/MetabaseRestClient.egg-info/PKG-INFO` & `metabaserestclient-0.0.4/MetabaseRestClient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetabaseRestClient
-Version: 0.0.3
+Version: 0.0.4
 Summary: Metabase Api Client Python package
 Home-page: https://github.com/blueromans/Metabase-Python-Client.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/Metabase-Python-Client.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metabaserestclient-0.0.3/PKG-INFO` & `metabaserestclient-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetabaseRestClient
-Version: 0.0.3
+Version: 0.0.4
 Summary: Metabase Api Client Python package
 Home-page: https://github.com/blueromans/Metabase-Python-Client.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/Metabase-Python-Client.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metabaserestclient-0.0.3/README.md` & `metabaserestclient-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `metabaserestclient-0.0.3/metabase/service/http_service.py` & `metabaserestclient-0.0.4/metabase/service/http_service.py`

 * *Files identical despite different names*

### Comparing `metabaserestclient-0.0.3/metabase/service/metabase_service.py` & `metabaserestclient-0.0.4/metabase/service/metabase_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,9 +38,13 @@
         return self.connect('GET', f'/api/collection/{collection_id}', headers=self.headers)
 
     def get_collection_items(self, collection_id: int = 0):
         if collection_id is 0:
             raise MetabaseException(ErrorCodes.INVALID_ATTRIBUTE)
         return self.connect('GET', f'/api/collection/{collection_id}/items', headers=self.headers)
 
-    def get_cards(self):
+    def get_cards(self, dashboard_id: int):
         return self.connect('GET', f'/api/card/', headers=self.headers)
+
+    def get_dash_card(self, dashboard_id: int, dash_id: int, card_id: int, payload):
+        return self.connect('POST', f'/api/dashboard/{dashboard_id}/dashcard/{dash_id}/card/{card_id}/query', payload,
+                            headers=self.headers)
```

### Comparing `metabaserestclient-0.0.3/setup.py` & `metabaserestclient-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='MetabaseRestClient',
-    version="0.0.3",
+    version="0.0.4",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='Metabase Api Client Python package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/Metabase-Python-Client.git',
     project_urls={
```

