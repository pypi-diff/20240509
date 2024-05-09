# Comparing `tmp/golink-0.5.2.tar.gz` & `tmp/golink-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golink-0.5.2.tar", max compression
+gzip compressed data, was "golink-0.5.3.tar", max compression
```

## Comparing `golink-0.5.2.tar` & `golink-0.5.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-29 04:04:28.448306 golink-0.5.2/LICENSE
--rw-r--r--   0        0        0     2858 2024-05-09 20:17:16.306197 golink-0.5.2/README.md
--rw-r--r--   0        0        0      100 2024-05-09 20:26:37.020179 golink-0.5.2/golink/__init__.py
--rw-r--r--   0        0        0     7928 2024-05-06 18:41:37.701305 golink-0.5.2/golink/cli.py
--rw-r--r--   0        0        0     1988 2024-04-29 04:04:28.448306 golink-0.5.2/golink/script.js
--rw-r--r--   0        0        0     3361 2024-04-29 04:04:28.448306 golink-0.5.2/golink/style.css
--rw-r--r--   0        0        0     7729 2024-04-29 04:04:28.448306 golink-0.5.2/golink/utils.py
--rw-r--r--   0        0        0      650 2024-05-09 20:26:12.929800 golink-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 golink-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-29 04:04:28.448306 golink-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2858 2024-05-09 20:17:16.306197 golink-0.5.3/README.md
+-rw-r--r--   0        0        0      100 2024-05-09 20:26:37.020179 golink-0.5.3/golink/__init__.py
+-rw-r--r--   0        0        0     7928 2024-05-06 18:41:37.701305 golink-0.5.3/golink/cli.py
+-rw-r--r--   0        0        0     1988 2024-04-29 04:04:28.448306 golink-0.5.3/golink/script.js
+-rw-r--r--   0        0        0     3361 2024-04-29 04:04:28.448306 golink-0.5.3/golink/style.css
+-rw-r--r--   0        0        0     7729 2024-04-29 04:04:28.448306 golink-0.5.3/golink/utils.py
+-rw-r--r--   0        0        0      645 2024-05-09 20:28:46.714921 golink-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 golink-0.5.3/PKG-INFO
```

### Comparing `golink-0.5.2/LICENSE` & `golink-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `golink-0.5.2/README.md` & `golink-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `golink-0.5.2/golink/cli.py` & `golink-0.5.3/golink/cli.py`

 * *Files identical despite different names*

### Comparing `golink-0.5.2/golink/script.js` & `golink-0.5.3/golink/script.js`

 * *Files identical despite different names*

### Comparing `golink-0.5.2/golink/style.css` & `golink-0.5.3/golink/style.css`

 * *Files identical despite different names*

### Comparing `golink-0.5.2/golink/utils.py` & `golink-0.5.3/golink/utils.py`

 * *Files identical despite different names*

### Comparing `golink-0.5.2/pyproject.toml` & `golink-0.5.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [project]
 name = "golink"
-
 package = "golink"
 
 # [build-system]
 # requires = ["setuptools>=42", "wheel"]
 # build-backend = "setuptools.build_meta"
 
-# [project.scripts]
-# golink = "golink.cli:main"
+[project.scripts]
+golink = "golink.cli:main"
 
 
 [tool.poetry]
 name = "golink"
-version = "0.5.2"
+version = "0.5.3"
 license = "GPLv3"
 description = "A simple URL shortener"
 authors = ["Max Vogel", "Logan Engstrom"]
 readme = "README.md"
 repository = "https://github.com/Mehvix/golink"
 
 [tool.poetry.dependencies]
```

### Comparing `golink-0.5.2/PKG-INFO` & `golink-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golink
-Version: 0.5.2
+Version: 0.5.3
 Summary: A simple URL shortener
 Home-page: https://github.com/Mehvix/golink
 License: GPLv3
 Author: Max Vogel
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: golink Version: 0.5.2 Summary: A simple URL
+Metadata-Version: 2.1 Name: golink Version: 0.5.3 Summary: A simple URL
 shortener Home-page: https://github.com/Mehvix/golink License: GPLv3 Author:
 Max Vogel Requires-Python: >=3.9,<4.0 Classifier: License :: Other/Proprietary
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: pandas
 (>=2.2.2,<3.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist:
 tabulate (>=0.9.0,<0.10.0) Requires-Dist: tqdm (>=4.66.4,<5.0.0) Project-URL:
```

