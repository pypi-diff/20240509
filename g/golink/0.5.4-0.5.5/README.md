# Comparing `tmp/golink-0.5.4.tar.gz` & `tmp/golink-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golink-0.5.4.tar", max compression
+gzip compressed data, was "golink-0.5.5.tar", max compression
```

## Comparing `golink-0.5.4.tar` & `golink-0.5.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-29 04:04:28.448306 golink-0.5.4/LICENSE
--rw-r--r--   0        0        0     2858 2024-05-09 20:17:16.306197 golink-0.5.4/README.md
--rw-r--r--   0        0        0      100 2024-05-09 20:26:37.020179 golink-0.5.4/golink/__init__.py
--rw-r--r--   0        0        0     7928 2024-05-06 18:41:37.701305 golink-0.5.4/golink/cli.py
--rw-r--r--   0        0        0     1988 2024-04-29 04:04:28.448306 golink-0.5.4/golink/script.js
--rw-r--r--   0        0        0     3361 2024-04-29 04:04:28.448306 golink-0.5.4/golink/style.css
--rw-r--r--   0        0        0     7729 2024-04-29 04:04:28.448306 golink-0.5.4/golink/utils.py
--rw-r--r--   0        0        0      694 2024-05-09 20:35:23.674500 golink-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 golink-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-29 04:04:28.448306 golink-0.5.5/LICENSE
+-rw-r--r--   0        0        0     2858 2024-05-09 20:17:16.306197 golink-0.5.5/README.md
+-rw-r--r--   0        0        0      100 2024-05-09 20:26:37.020179 golink-0.5.5/golink/__init__.py
+-rw-r--r--   0        0        0     7928 2024-05-06 18:41:37.701305 golink-0.5.5/golink/cli.py
+-rw-r--r--   0        0        0     1988 2024-04-29 04:04:28.448306 golink-0.5.5/golink/script.js
+-rw-r--r--   0        0        0     3361 2024-04-29 04:04:28.448306 golink-0.5.5/golink/style.css
+-rw-r--r--   0        0        0     7729 2024-04-29 04:04:28.448306 golink-0.5.5/golink/utils.py
+-rw-r--r--   0        0        0      743 2024-05-09 20:40:54.340973 golink-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 golink-0.5.5/PKG-INFO
```

### Comparing `golink-0.5.4/LICENSE` & `golink-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `golink-0.5.4/README.md` & `golink-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `golink-0.5.4/golink/cli.py` & `golink-0.5.5/golink/cli.py`

 * *Files identical despite different names*

### Comparing `golink-0.5.4/golink/script.js` & `golink-0.5.5/golink/script.js`

 * *Files identical despite different names*

### Comparing `golink-0.5.4/golink/style.css` & `golink-0.5.5/golink/style.css`

 * *Files identical despite different names*

### Comparing `golink-0.5.4/golink/utils.py` & `golink-0.5.5/golink/utils.py`

 * *Files identical despite different names*

### Comparing `golink-0.5.4/pyproject.toml` & `golink-0.5.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 
 # [project.scripts]
 # golink = "golink.cli:main"
 
 
 [tool.poetry]
 name = "golink"
-version = "0.5.4"
+version = "0.5.5"
 license = "GPLv3"
 description = "A simple URL shortener"
 authors = ["Max Vogel", "Logan Engstrom"]
 readme = "README.md"
 repository = "https://github.com/Mehvix/golink"
 
+packages = [{ include = "golink", from = "." }]
+
 [tool.poetry.dependencies]
 python = "^3.9"
 tqdm = "^4.66.4"
 tabulate = "^0.9.0"
 requests = "^2.31.0"
 pandas = "^2.2.2"
```

### Comparing `golink-0.5.4/PKG-INFO` & `golink-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golink
-Version: 0.5.4
+Version: 0.5.5
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
-Metadata-Version: 2.1 Name: golink Version: 0.5.4 Summary: A simple URL
+Metadata-Version: 2.1 Name: golink Version: 0.5.5 Summary: A simple URL
 shortener Home-page: https://github.com/Mehvix/golink License: GPLv3 Author:
 Max Vogel Requires-Python: >=3.9,<4.0 Classifier: License :: Other/Proprietary
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: pandas
 (>=2.2.2,<3.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist:
 tabulate (>=0.9.0,<0.10.0) Requires-Dist: tqdm (>=4.66.4,<5.0.0) Project-URL:
```

