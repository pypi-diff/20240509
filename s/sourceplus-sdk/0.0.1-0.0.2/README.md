# Comparing `tmp/sourceplus_sdk-0.0.1.tar.gz` & `tmp/sourceplus_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourceplus_sdk-0.0.1.tar", last modified: Thu May  9 15:43:21 2024, max compression
+gzip compressed data, was "sourceplus_sdk-0.0.2.tar", last modified: Thu May  9 16:53:33 2024, max compression
```

## Comparing `sourceplus_sdk-0.0.1.tar` & `sourceplus_sdk-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 15:43:21.918840 sourceplus_sdk-0.0.1/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      597 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/.coveragerc
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      566 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/.gitignore
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      530 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/.readthedocs.yml
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       74 2024-05-09 14:50:35.000000 sourceplus_sdk-0.0.1/AUTHORS.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       77 2024-05-09 15:07:32.000000 sourceplus_sdk-0.0.1/CHANGELOG.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1079 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/LICENSE.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3139 2024-05-09 15:43:21.918781 sourceplus_sdk-0.0.1/PKG-INFO
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2071 2024-05-09 15:26:48.000000 sourceplus_sdk-0.0.1/README.rst
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 15:43:21.915138 sourceplus_sdk-0.0.1/docs/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1154 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/docs/Makefile
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 15:43:21.915367 sourceplus_sdk-0.0.1/docs/_static/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       18 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/docs/_static/.gitignore
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       41 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/docs/authors.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       43 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/docs/changelog.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     9769 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/docs/conf.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2302 2024-05-09 15:09:17.000000 sourceplus_sdk-0.0.1/docs/index.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       67 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/docs/license.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       39 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/docs/readme.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      233 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/docs/requirements.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      346 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/pyproject.toml
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1539 2024-05-09 15:43:21.919184 sourceplus_sdk-0.0.1/setup.cfg
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      709 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/setup.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 15:43:21.911496 sourceplus_sdk-0.0.1/src/
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 15:43:21.915970 sourceplus_sdk-0.0.1/src/sourceplus_sdk/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      625 2024-05-08 17:29:55.000000 sourceplus_sdk-0.0.1/src/sourceplus_sdk/__init__.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      393 2024-05-08 19:56:34.000000 sourceplus_sdk-0.0.1/src/sourceplus_sdk/libs.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)    12944 2024-05-09 14:40:10.000000 sourceplus_sdk-0.0.1/src/sourceplus_sdk/main.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 15:43:21.918304 sourceplus_sdk-0.0.1/src/sourceplus_sdk.egg-info/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3139 2024-05-09 15:43:21.000000 sourceplus_sdk-0.0.1/src/sourceplus_sdk.egg-info/PKG-INFO
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      792 2024-05-09 15:43:21.000000 sourceplus_sdk-0.0.1/src/sourceplus_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2024-05-09 15:43:21.000000 sourceplus_sdk-0.0.1/src/sourceplus_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       50 2024-05-09 15:43:21.000000 sourceplus_sdk-0.0.1/src/sourceplus_sdk.egg-info/entry_points.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2024-05-09 15:43:21.000000 sourceplus_sdk-0.0.1/src/sourceplus_sdk.egg-info/not-zip-safe
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      120 2024-05-09 15:43:21.000000 sourceplus_sdk-0.0.1/src/sourceplus_sdk.egg-info/requires.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       15 2024-05-09 15:43:21.000000 sourceplus_sdk-0.0.1/src/sourceplus_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 15:43:21.917493 sourceplus_sdk-0.0.1/tests/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      282 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.1/tests/conftest.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 15:43:21.917992 sourceplus_sdk-0.0.1/tests/files/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 12:40:19.000000 sourceplus_sdk-0.0.1/tests/files/bad.parquet
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 12:48:45.000000 sourceplus_sdk-0.0.1/tests/files/bad.tsv
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1027 2024-05-09 12:56:36.000000 sourceplus_sdk-0.0.1/tests/files/good.parquet
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1140 2024-05-09 12:58:10.000000 sourceplus_sdk-0.0.1/tests/test_libs.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     6491 2024-05-09 14:43:09.000000 sourceplus_sdk-0.0.1/tests/test_main.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2760 2024-05-09 12:25:50.000000 sourceplus_sdk-0.0.1/tox.ini
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.841229 sourceplus_sdk-0.0.2/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      597 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/.coveragerc
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      566 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/.gitignore
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      530 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/.readthedocs.yml
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       74 2024-05-09 14:50:35.000000 sourceplus_sdk-0.0.2/AUTHORS.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       77 2024-05-09 15:07:32.000000 sourceplus_sdk-0.0.2/CHANGELOG.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1079 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/LICENSE.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3139 2024-05-09 16:53:33.841163 sourceplus_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2071 2024-05-09 15:26:48.000000 sourceplus_sdk-0.0.2/README.rst
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.837990 sourceplus_sdk-0.0.2/docs/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1154 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/Makefile
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.838127 sourceplus_sdk-0.0.2/docs/_static/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       18 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/_static/.gitignore
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       41 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/authors.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       43 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/changelog.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     9769 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/conf.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1386 2024-05-09 15:49:09.000000 sourceplus_sdk-0.0.2/docs/index.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       67 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/license.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       39 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/readme.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      233 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/requirements.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      346 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1539 2024-05-09 16:53:33.841563 sourceplus_sdk-0.0.2/setup.cfg
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      709 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/setup.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.834688 sourceplus_sdk-0.0.2/src/
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.838729 sourceplus_sdk-0.0.2/src/sourceplus_sdk/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      625 2024-05-08 17:29:55.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk/__init__.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      393 2024-05-08 19:56:34.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk/libs.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)    12944 2024-05-09 14:40:10.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk/main.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.840719 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3139 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      792 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       50 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      120 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/requires.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       15 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.840088 sourceplus_sdk-0.0.2/tests/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      282 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/tests/conftest.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.840461 sourceplus_sdk-0.0.2/tests/files/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 12:40:19.000000 sourceplus_sdk-0.0.2/tests/files/bad.parquet
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 12:48:45.000000 sourceplus_sdk-0.0.2/tests/files/bad.tsv
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1027 2024-05-09 12:56:36.000000 sourceplus_sdk-0.0.2/tests/files/good.parquet
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1140 2024-05-09 12:58:10.000000 sourceplus_sdk-0.0.2/tests/test_libs.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     6491 2024-05-09 14:43:09.000000 sourceplus_sdk-0.0.2/tests/test_main.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2766 2024-05-09 16:49:30.000000 sourceplus_sdk-0.0.2/tox.ini
```

### Comparing `sourceplus_sdk-0.0.1/.coveragerc` & `sourceplus_sdk-0.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/.gitignore` & `sourceplus_sdk-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/.readthedocs.yml` & `sourceplus_sdk-0.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/LICENSE.txt` & `sourceplus_sdk-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/PKG-INFO` & `sourceplus_sdk-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourceplus-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Search, curate, and enrich collections for AI training.
 Home-page: https://github.com/Spawning-Inc/sourceplus-sdk/
 Author: Nick Padgett
 Author-email: nick@spawning.ai
 License: MIT
 Project-URL: Documentation, https://sourceplus-sdk.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spawning-Inc/sourceplus-sdk
```

### Comparing `sourceplus_sdk-0.0.1/README.rst` & `sourceplus_sdk-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/docs/Makefile` & `sourceplus_sdk-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/docs/conf.py` & `sourceplus_sdk-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/setup.cfg` & `sourceplus_sdk-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/setup.py` & `sourceplus_sdk-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/src/sourceplus_sdk/__init__.py` & `sourceplus_sdk-0.0.2/src/sourceplus_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/src/sourceplus_sdk/main.py` & `sourceplus_sdk-0.0.2/src/sourceplus_sdk/main.py`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/src/sourceplus_sdk.egg-info/PKG-INFO` & `sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourceplus-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Search, curate, and enrich collections for AI training.
 Home-page: https://github.com/Spawning-Inc/sourceplus-sdk/
 Author: Nick Padgett
 Author-email: nick@spawning.ai
 License: MIT
 Project-URL: Documentation, https://sourceplus-sdk.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spawning-Inc/sourceplus-sdk
```

### Comparing `sourceplus_sdk-0.0.1/src/sourceplus_sdk.egg-info/SOURCES.txt` & `sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/tests/files/good.parquet` & `sourceplus_sdk-0.0.2/tests/files/good.parquet`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/tests/test_libs.py` & `sourceplus_sdk-0.0.2/tests/test_libs.py`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/tests/test_main.py` & `sourceplus_sdk-0.0.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.1/tox.ini` & `sourceplus_sdk-0.0.2/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Tox configuration file
 # Read more under https://tox.wiki/
 
 [tox]
 minversion = 3.24
-envlist = py38,py39,py310,py311
+envlist = py38,py39,py310,py311,py312
 isolated_build = True
 
 
 [testenv]
 description = Invoke pytest to run automated tests
 setenv =
     TOXINIDIR = {toxinidir}
```

