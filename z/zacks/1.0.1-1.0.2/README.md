# Comparing `tmp/zacks-1.0.1.tar.gz` & `tmp/zacks-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zacks-1.0.1.tar", last modified: Wed May  8 21:04:12 2024, max compression
+gzip compressed data, was "zacks-1.0.2.tar", last modified: Wed May  8 21:06:47 2024, max compression
```

## Comparing `zacks-1.0.1.tar` & `zacks-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 alesh     (1000) alesh     (1000)        0 2024-05-08 21:04:12.727563 zacks-1.0.1/
--rw-r--r--   0 alesh     (1000) alesh     (1000)      580 2024-05-08 21:04:12.727563 zacks-1.0.1/PKG-INFO
--rw-rw-r--   0 alesh     (1000) alesh     (1000)      200 2024-05-08 19:49:50.000000 zacks-1.0.1/README.md
--rw-rw-r--   0 alesh     (1000) alesh     (1000)     2414 2024-05-08 19:42:45.000000 zacks-1.0.1/experts_view.py
--rw-rw-r--   0 alesh     (1000) alesh     (1000)      528 2024-05-08 21:03:04.000000 zacks-1.0.1/pyproject.toml
--rw-rw-r--   0 alesh     (1000) alesh     (1000)       38 2024-05-08 21:04:12.727563 zacks-1.0.1/setup.cfg
-drwxrwxr-x   0 alesh     (1000) alesh     (1000)        0 2024-05-08 21:04:12.727563 zacks-1.0.1/zacks.egg-info/
--rw-r--r--   0 alesh     (1000) alesh     (1000)      580 2024-05-08 21:04:12.000000 zacks-1.0.1/zacks.egg-info/PKG-INFO
--rw-rw-r--   0 alesh     (1000) alesh     (1000)      184 2024-05-08 21:04:12.000000 zacks-1.0.1/zacks.egg-info/SOURCES.txt
--rw-rw-r--   0 alesh     (1000) alesh     (1000)        1 2024-05-08 21:04:12.000000 zacks-1.0.1/zacks.egg-info/dependency_links.txt
--rw-rw-r--   0 alesh     (1000) alesh     (1000)       37 2024-05-08 21:04:12.000000 zacks-1.0.1/zacks.egg-info/requires.txt
--rw-rw-r--   0 alesh     (1000) alesh     (1000)       13 2024-05-08 21:04:12.000000 zacks-1.0.1/zacks.egg-info/top_level.txt
+drwxrwxr-x   0 alesh     (1000) alesh     (1000)        0 2024-05-08 21:06:47.182123 zacks-1.0.2/
+-rw-r--r--   0 alesh     (1000) alesh     (1000)      580 2024-05-08 21:06:47.182123 zacks-1.0.2/PKG-INFO
+-rw-rw-r--   0 alesh     (1000) alesh     (1000)      200 2024-05-08 21:05:32.000000 zacks-1.0.2/README.md
+-rw-rw-r--   0 alesh     (1000) alesh     (1000)     2414 2024-05-08 19:42:45.000000 zacks-1.0.2/experts_view.py
+-rw-rw-r--   0 alesh     (1000) alesh     (1000)      528 2024-05-08 21:06:04.000000 zacks-1.0.2/pyproject.toml
+-rw-rw-r--   0 alesh     (1000) alesh     (1000)       38 2024-05-08 21:06:47.182123 zacks-1.0.2/setup.cfg
+drwxrwxr-x   0 alesh     (1000) alesh     (1000)        0 2024-05-08 21:06:47.182123 zacks-1.0.2/zacks.egg-info/
+-rw-r--r--   0 alesh     (1000) alesh     (1000)      580 2024-05-08 21:06:47.000000 zacks-1.0.2/zacks.egg-info/PKG-INFO
+-rw-rw-r--   0 alesh     (1000) alesh     (1000)      184 2024-05-08 21:06:47.000000 zacks-1.0.2/zacks.egg-info/SOURCES.txt
+-rw-rw-r--   0 alesh     (1000) alesh     (1000)        1 2024-05-08 21:06:47.000000 zacks-1.0.2/zacks.egg-info/dependency_links.txt
+-rw-rw-r--   0 alesh     (1000) alesh     (1000)       37 2024-05-08 21:06:47.000000 zacks-1.0.2/zacks.egg-info/requires.txt
+-rw-rw-r--   0 alesh     (1000) alesh     (1000)       13 2024-05-08 21:06:47.000000 zacks-1.0.2/zacks.egg-info/top_level.txt
```

### Comparing `zacks-1.0.1/PKG-INFO` & `zacks-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: zacks
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple web scraper for extracting data from Zacks Investment Research
 Author-email: Alon Leshem <aleshem20@gmail.com>
 Keywords: zacks,scraper,data extraction
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: bs4
 Requires-Dist: requests
 Requires-Dist: alive-progress
 Requires-Dist: argparse
 
-# Zucks
+# Zacks
 An unofficial package that extracts portfolio information from Zacks. The only current implementation is `experts_view()`
 
 ## Usage
 ```python
-from zucks import experts_view
+from zacks import experts_view
 
 experts_view()
 ```
```

### Comparing `zacks-1.0.1/experts_view.py` & `zacks-1.0.2/experts_view.py`

 * *Files identical despite different names*

### Comparing `zacks-1.0.1/pyproject.toml` & `zacks-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zacks"
-version = "1.0.1"
+version = "1.0.2"
 description = "A simple web scraper for extracting data from Zacks Investment Research"
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [{name = "Alon Leshem", email = "aleshem20@gmail.com"}]
 keywords = ["zacks", "scraper", "data extraction"]
 dependencies = [
     "bs4",
     "requests",
```

### Comparing `zacks-1.0.1/zacks.egg-info/PKG-INFO` & `zacks-1.0.2/zacks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: zacks
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple web scraper for extracting data from Zacks Investment Research
 Author-email: Alon Leshem <aleshem20@gmail.com>
 Keywords: zacks,scraper,data extraction
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: bs4
 Requires-Dist: requests
 Requires-Dist: alive-progress
 Requires-Dist: argparse
 
-# Zucks
+# Zacks
 An unofficial package that extracts portfolio information from Zacks. The only current implementation is `experts_view()`
 
 ## Usage
 ```python
-from zucks import experts_view
+from zacks import experts_view
 
 experts_view()
 ```
```

