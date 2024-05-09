# Comparing `tmp/sql_test_cli-0.0.1.tar.gz` & `tmp/sql_test_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_test_cli-0.0.1.tar", max compression
+gzip compressed data, was "sql_test_cli-0.1.1.tar", max compression
```

## Comparing `sql_test_cli-0.0.1.tar` & `sql_test_cli-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-05-09 19:12:52.908789 sql_test_cli-0.0.1/LICENSE
--rw-r--r--   0        0        0      938 2024-05-09 19:12:52.908789 sql_test_cli-0.0.1/README.md
--rw-r--r--   0        0        0      847 2024-05-09 19:12:52.908789 sql_test_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       38 2024-05-09 19:12:52.912789 sql_test_cli-0.0.1/sql_test_cli/cli/__init__.py
--rw-r--r--   0        0        0      292 2024-05-09 19:12:52.916789 sql_test_cli-0.0.1/sql_test_cli/cli/commands.py
--rw-r--r--   0        0        0     3539 2024-05-09 19:12:52.916789 sql_test_cli-0.0.1/sql_test_cli/cli/outputs.py
--rw-r--r--   0        0        0      392 2024-05-09 19:12:52.916789 sql_test_cli-0.0.1/sql_test_cli/core/__init__.py
--rw-r--r--   0        0        0     2987 2024-05-09 19:12:52.916789 sql_test_cli-0.0.1/sql_test_cli/core/config.py
--rw-r--r--   0        0        0      832 2024-05-09 19:12:52.916789 sql_test_cli-0.0.1/sql_test_cli/core/config_manager.py
--rw-r--r--   0        0        0      443 2024-05-09 19:12:52.916789 sql_test_cli-0.0.1/sql_test_cli/core/connection.py
--rw-r--r--   0        0        0     1168 2024-05-09 19:12:52.916789 sql_test_cli-0.0.1/sql_test_cli/core/directory_check.py
--rw-r--r--   0        0        0     1199 2024-05-09 19:12:52.916789 sql_test_cli-0.0.1/sql_test_cli/core/initialize.py
--rw-r--r--   0        0        0      599 2024-05-09 19:12:52.916789 sql_test_cli-0.0.1/sql_test_cli/core/logger.py
--rw-r--r--   0        0        0     2120 2024-05-09 19:12:52.916789 sql_test_cli-0.0.1/sql_test_cli/core/run.py
--rw-r--r--   0        0        0     3042 2024-05-09 19:12:52.916789 sql_test_cli-0.0.1/sql_test_cli/core/run_test.py
--rw-r--r--   0        0        0      719 2024-05-09 19:12:52.916789 sql_test_cli-0.0.1/sql_test_cli/core/utils.py
--rw-r--r--   0        0        0     1664 1970-01-01 00:00:00.000000 sql_test_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-09 19:30:08.608499 sql_test_cli-0.1.1/LICENSE
+-rw-r--r--   0        0        0      938 2024-05-09 19:30:08.608499 sql_test_cli-0.1.1/README.md
+-rw-r--r--   0        0        0      848 2024-05-09 19:30:08.608499 sql_test_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       38 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/cli/__init__.py
+-rw-r--r--   0        0        0      292 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/cli/commands.py
+-rw-r--r--   0        0        0     3539 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/cli/outputs.py
+-rw-r--r--   0        0        0      392 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/core/__init__.py
+-rw-r--r--   0        0        0     2987 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/core/config.py
+-rw-r--r--   0        0        0      832 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/core/config_manager.py
+-rw-r--r--   0        0        0      443 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/core/connection.py
+-rw-r--r--   0        0        0     1168 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/core/directory_check.py
+-rw-r--r--   0        0        0     1199 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/core/initialize.py
+-rw-r--r--   0        0        0      599 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/core/logger.py
+-rw-r--r--   0        0        0     2120 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/core/run.py
+-rw-r--r--   0        0        0     3042 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/core/run_test.py
+-rw-r--r--   0        0        0      719 2024-05-09 19:30:08.616499 sql_test_cli-0.1.1/sql_test_cli/core/utils.py
+-rw-r--r--   0        0        0     1664 1970-01-01 00:00:00.000000 sql_test_cli-0.1.1/PKG-INFO
```

### Comparing `sql_test_cli-0.0.1/LICENSE` & `sql_test_cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_test_cli-0.0.1/README.md` & `sql_test_cli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sql_test_cli-0.0.1/pyproject.toml` & `sql_test_cli-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-test-cli"
-version = "0.0.1"
+version = "0.1.1"
 description = "A CLI tool for executing sql tests."
 authors = ["cohenj20 <cohenj20@sacredheart.edu>"]
 readme = "README.md"
 license = "MIT"
 include = [
     "LICENSE",
 ]
@@ -31,11 +31,11 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.1"
+version = "0.1.3"
 version_files = [
-    "pyproject.toml:version"
+    "pyproject.toml:^version"
 ]
```

### Comparing `sql_test_cli-0.0.1/sql_test_cli/cli/outputs.py` & `sql_test_cli-0.1.1/sql_test_cli/cli/outputs.py`

 * *Files identical despite different names*

### Comparing `sql_test_cli-0.0.1/sql_test_cli/core/config.py` & `sql_test_cli-0.1.1/sql_test_cli/core/config.py`

 * *Files identical despite different names*

### Comparing `sql_test_cli-0.0.1/sql_test_cli/core/config_manager.py` & `sql_test_cli-0.1.1/sql_test_cli/core/config_manager.py`

 * *Files identical despite different names*

### Comparing `sql_test_cli-0.0.1/sql_test_cli/core/directory_check.py` & `sql_test_cli-0.1.1/sql_test_cli/core/directory_check.py`

 * *Files identical despite different names*

### Comparing `sql_test_cli-0.0.1/sql_test_cli/core/initialize.py` & `sql_test_cli-0.1.1/sql_test_cli/core/initialize.py`

 * *Files identical despite different names*

### Comparing `sql_test_cli-0.0.1/sql_test_cli/core/logger.py` & `sql_test_cli-0.1.1/sql_test_cli/core/logger.py`

 * *Files identical despite different names*

### Comparing `sql_test_cli-0.0.1/sql_test_cli/core/run.py` & `sql_test_cli-0.1.1/sql_test_cli/core/run.py`

 * *Files identical despite different names*

### Comparing `sql_test_cli-0.0.1/sql_test_cli/core/run_test.py` & `sql_test_cli-0.1.1/sql_test_cli/core/run_test.py`

 * *Files identical despite different names*

### Comparing `sql_test_cli-0.0.1/sql_test_cli/core/utils.py` & `sql_test_cli-0.1.1/sql_test_cli/core/utils.py`

 * *Files identical despite different names*

### Comparing `sql_test_cli-0.0.1/PKG-INFO` & `sql_test_cli-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-test-cli
-Version: 0.0.1
+Version: 0.1.1
 Summary: A CLI tool for executing sql tests.
 License: MIT
 Author: cohenj20
 Author-email: cohenj20@sacredheart.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

