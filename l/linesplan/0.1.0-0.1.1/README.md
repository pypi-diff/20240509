# Comparing `tmp/linesplan-0.1.0.tar.gz` & `tmp/linesplan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linesplan-0.1.0.tar", max compression
+gzip compressed data, was "linesplan-0.1.1.tar", max compression
```

## Comparing `linesplan-0.1.0.tar` & `linesplan-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       20 2024-05-09 09:27:59.593622 linesplan-0.1.0/README.md
--rw-r--r--   0        0        0      606 2024-05-09 10:46:12.162443 linesplan-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      145 2024-05-09 10:45:36.579171 linesplan-0.1.0/src/linesplan/__init__.py
--rw-r--r--   0        0        0     4476 2024-05-09 09:27:23.430451 linesplan-0.1.0/src/linesplan/dxfreader.py
--rw-r--r--   0        0        0    13333 2024-05-04 21:28:49.835341 linesplan-0.1.0/src/linesplan/lines.py
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 linesplan-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       20 2024-05-09 18:22:30.176393 linesplan-0.1.1/README.md
+-rw-r--r--   0        0        0      606 2024-05-09 18:22:30.176393 linesplan-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      145 2024-05-09 18:22:30.176393 linesplan-0.1.1/src/linesplan/__init__.py
+-rw-r--r--   0        0        0     4476 2024-05-09 18:22:30.176393 linesplan-0.1.1/src/linesplan/dxfreader.py
+-rw-r--r--   0        0        0    13333 2024-05-09 18:22:30.180393 linesplan-0.1.1/src/linesplan/lines.py
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 linesplan-0.1.1/PKG-INFO
```

### Comparing `linesplan-0.1.0/pyproject.toml` & `linesplan-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linesplan"
-version = "0.1.0"
+version = "0.1.1"
 description = "Ship Linesplan and Hydrostatics"
 authors = ["Jaap Versteegh <j.r.versteegh@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.*"
```

### Comparing `linesplan-0.1.0/src/linesplan/dxfreader.py` & `linesplan-0.1.1/src/linesplan/dxfreader.py`

 * *Files identical despite different names*

### Comparing `linesplan-0.1.0/src/linesplan/lines.py` & `linesplan-0.1.1/src/linesplan/lines.py`

 * *Files identical despite different names*

### Comparing `linesplan-0.1.0/PKG-INFO` & `linesplan-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linesplan
-Version: 0.1.0
+Version: 0.1.1
 Summary: Ship Linesplan and Hydrostatics
 License: GPLv3
 Author: Jaap Versteegh
 Author-email: j.r.versteegh@gmail.com
 Requires-Python: ==3.11.*
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

