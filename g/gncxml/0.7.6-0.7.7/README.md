# Comparing `tmp/gncxml-0.7.6.tar.gz` & `tmp/gncxml-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gncxml-0.7.6.tar", max compression
+gzip compressed data, was "gncxml-0.7.7.tar", max compression
```

## Comparing `gncxml-0.7.6.tar` & `gncxml-0.7.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2017-12-17 01:02:32.000000 gncxml-0.7.6/LICENSE
--rw-r--r--   0        0        0     1124 2023-07-21 23:25:02.000000 gncxml-0.7.6/README.md
--rw-r--r--   0        0        0      121 2017-11-23 20:24:39.000000 gncxml-0.7.6/gncxml/__init__.py
--rw-r--r--   0        0        0       90 2021-12-27 13:53:45.000000 gncxml-0.7.6/gncxml/__main__.py
--rw-r--r--   0        0        0     2871 2022-08-24 00:28:47.000000 gncxml-0.7.6/gncxml/_cli.py
--rw-r--r--   0        0        0    10353 2024-01-18 23:48:52.083394 gncxml-0.7.6/gncxml/_iso4217.py
--rw-r--r--   0        0        0    11085 2021-12-27 13:53:45.000000 gncxml-0.7.6/gncxml/book.py
--rw-r--r--   0        0        0      614 2024-01-20 12:46:31.846860 gncxml-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 gncxml-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2017-12-17 01:02:32.000000 gncxml-0.7.7/LICENSE
+-rw-r--r--   0        0        0     1124 2023-07-21 23:25:02.000000 gncxml-0.7.7/README.md
+-rw-r--r--   0        0        0      121 2017-11-23 20:24:39.000000 gncxml-0.7.7/gncxml/__init__.py
+-rw-r--r--   0        0        0       90 2021-12-27 13:53:45.000000 gncxml-0.7.7/gncxml/__main__.py
+-rw-r--r--   0        0        0     2871 2022-08-24 00:28:47.000000 gncxml-0.7.7/gncxml/_cli.py
+-rw-r--r--   0        0        0    10353 2024-05-09 13:08:20.918759 gncxml-0.7.7/gncxml/_iso4217.py
+-rw-r--r--   0        0        0    11085 2021-12-27 13:53:45.000000 gncxml-0.7.7/gncxml/book.py
+-rw-r--r--   0        0        0      614 2024-05-09 13:12:59.431717 gncxml-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 gncxml-0.7.7/PKG-INFO
```

### Comparing `gncxml-0.7.6/LICENSE` & `gncxml-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gncxml-0.7.6/README.md` & `gncxml-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `gncxml-0.7.6/gncxml/_cli.py` & `gncxml-0.7.7/gncxml/_cli.py`

 * *Files identical despite different names*

### Comparing `gncxml-0.7.6/gncxml/_iso4217.py` & `gncxml-0.7.7/gncxml/_iso4217.py`

 * *Files identical despite different names*

### Comparing `gncxml-0.7.6/gncxml/book.py` & `gncxml-0.7.7/gncxml/book.py`

 * *Files identical despite different names*

### Comparing `gncxml-0.7.6/pyproject.toml` & `gncxml-0.7.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gncxml"
-version = "0.7.6"
+version = "0.7.7"
 description = "Extract entries from GnuCash data file to pandas.DataFrame."
 license = "Apache-2.0"
 authors = ["LiosK <contact@mail.liosk.net>"]
 readme = "README.md"
 homepage = "https://github.com/LiosK/gncxml"
 classifiers = [
   "Operating System :: OS Independent",
```

### Comparing `gncxml-0.7.6/PKG-INFO` & `gncxml-0.7.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gncxml
-Version: 0.7.6
+Version: 0.7.7
 Summary: Extract entries from GnuCash data file to pandas.DataFrame.
 Home-page: https://github.com/LiosK/gncxml
 License: Apache-2.0
 Author: LiosK
 Author-email: contact@mail.liosk.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

