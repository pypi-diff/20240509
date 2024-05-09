# Comparing `tmp/metabaserestclient-0.0.2.tar.gz` & `tmp/metabaserestclient-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabaserestclient-0.0.2.tar", last modified: Wed Apr 17 19:07:10 2024, max compression
+gzip compressed data, was "metabaserestclient-0.0.3.tar", last modified: Wed Apr 17 19:11:03 2024, max compression
```

## Comparing `metabaserestclient-0.0.2.tar` & `metabaserestclient-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-04-17 19:07:10.620736 metabaserestclient-0.0.2/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2023-05-15 01:16:08.000000 metabaserestclient-0.0.2/LICENSE
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-04-17 19:07:10.620359 metabaserestclient-0.0.2/MetabaseRestClient.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2021 2024-04-17 19:07:10.000000 metabaserestclient-0.0.2/MetabaseRestClient.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      400 2024-04-17 19:07:10.000000 metabaserestclient-0.0.2/MetabaseRestClient.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2024-04-17 19:07:10.000000 metabaserestclient-0.0.2/MetabaseRestClient.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2024-04-17 19:07:10.000000 metabaserestclient-0.0.2/MetabaseRestClient.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2024-04-17 19:07:10.000000 metabaserestclient-0.0.2/MetabaseRestClient.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2021 2024-04-17 19:07:10.620546 metabaserestclient-0.0.2/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1442 2024-04-17 19:04:03.000000 metabaserestclient-0.0.2/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-04-17 19:07:10.619764 metabaserestclient-0.0.2/metabase/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      151 2024-04-17 14:31:46.000000 metabaserestclient-0.0.2/metabase/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      323 2024-04-17 14:42:13.000000 metabaserestclient-0.0.2/metabase/exception.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-05-15 01:16:08.000000 metabaserestclient-0.0.2/metabase/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-04-17 19:07:10.620162 metabaserestclient-0.0.2/metabase/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       46 2024-04-17 14:31:46.000000 metabaserestclient-0.0.2/metabase/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1006 2024-04-17 17:59:44.000000 metabaserestclient-0.0.2/metabase/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1807 2024-04-17 18:34:41.000000 metabaserestclient-0.0.2/metabase/service/metabase_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2024-04-17 19:07:10.620775 metabaserestclient-0.0.2/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      884 2024-04-17 19:06:43.000000 metabaserestclient-0.0.2/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-04-17 19:11:03.444020 metabaserestclient-0.0.3/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2023-05-15 01:16:08.000000 metabaserestclient-0.0.3/LICENSE
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-04-17 19:11:03.443655 metabaserestclient-0.0.3/MetabaseRestClient.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2049 2024-04-17 19:11:03.000000 metabaserestclient-0.0.3/MetabaseRestClient.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      400 2024-04-17 19:11:03.000000 metabaserestclient-0.0.3/MetabaseRestClient.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2024-04-17 19:11:03.000000 metabaserestclient-0.0.3/MetabaseRestClient.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2024-04-17 19:11:03.000000 metabaserestclient-0.0.3/MetabaseRestClient.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2024-04-17 19:11:03.000000 metabaserestclient-0.0.3/MetabaseRestClient.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2049 2024-04-17 19:11:03.443833 metabaserestclient-0.0.3/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1442 2024-04-17 19:04:03.000000 metabaserestclient-0.0.3/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-04-17 19:11:03.443069 metabaserestclient-0.0.3/metabase/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      151 2024-04-17 14:31:46.000000 metabaserestclient-0.0.3/metabase/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      323 2024-04-17 14:42:13.000000 metabaserestclient-0.0.3/metabase/exception.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-05-15 01:16:08.000000 metabaserestclient-0.0.3/metabase/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2024-04-17 19:11:03.443472 metabaserestclient-0.0.3/metabase/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       46 2024-04-17 14:31:46.000000 metabaserestclient-0.0.3/metabase/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1006 2024-04-17 17:59:44.000000 metabaserestclient-0.0.3/metabase/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1807 2024-04-17 18:34:41.000000 metabaserestclient-0.0.3/metabase/service/metabase_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2024-04-17 19:11:03.444095 metabaserestclient-0.0.3/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      912 2024-04-17 19:10:55.000000 metabaserestclient-0.0.3/setup.py
```

### Comparing `metabaserestclient-0.0.2/LICENSE` & `metabaserestclient-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metabaserestclient-0.0.2/MetabaseRestClient.egg-info/PKG-INFO` & `metabaserestclient-0.0.3/MetabaseRestClient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: MetabaseRestClient
-Version: 0.0.2
+Version: 0.0.3
 Summary: Metabase Api Client Python package
-Home-page: https://github.com/blueromans/metabase.git
+Home-page: https://github.com/blueromans/Metabase-Python-Client.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
-Project-URL: Bug Tracker, https://github.com/blueromans/metabase.git/issues
+Project-URL: Bug Tracker, https://github.com/blueromans/Metabase-Python-Client.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
```

### Comparing `metabaserestclient-0.0.2/PKG-INFO` & `metabaserestclient-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: MetabaseRestClient
-Version: 0.0.2
+Version: 0.0.3
 Summary: Metabase Api Client Python package
-Home-page: https://github.com/blueromans/metabase.git
+Home-page: https://github.com/blueromans/Metabase-Python-Client.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
-Project-URL: Bug Tracker, https://github.com/blueromans/metabase.git/issues
+Project-URL: Bug Tracker, https://github.com/blueromans/Metabase-Python-Client.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
```

### Comparing `metabaserestclient-0.0.2/README.md` & `metabaserestclient-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `metabaserestclient-0.0.2/metabase/service/http_service.py` & `metabaserestclient-0.0.3/metabase/service/http_service.py`

 * *Files identical despite different names*

### Comparing `metabaserestclient-0.0.2/metabase/service/metabase_service.py` & `metabaserestclient-0.0.3/metabase/service/metabase_service.py`

 * *Files identical despite different names*

