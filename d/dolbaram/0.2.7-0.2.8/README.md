# Comparing `tmp/dolbaram-0.2.7.tar.gz` & `tmp/dolbaram-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolbaram-0.2.7.tar", max compression
+gzip compressed data, was "dolbaram-0.2.8.tar", max compression
```

## Comparing `dolbaram-0.2.7.tar` & `dolbaram-0.2.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254669 dolbaram-0.2.7/README.md
--rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254618 dolbaram-0.2.7/dolbaram/__init__.py
--rw-r--r--   0        0        0    19353 2024-05-03 03:53:07.281938 dolbaram-0.2.7/dolbaram/dolbaram.py
--rw-r--r--   0        0        0      576 2024-05-03 03:53:07.275807 dolbaram-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 dolbaram-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254669 dolbaram-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254618 dolbaram-0.2.8/dolbaram/__init__.py
+-rw-r--r--   0        0        0    19353 2024-05-03 03:53:07.281938 dolbaram-0.2.8/dolbaram/dolbaram.py
+-rw-r--r--   0        0        0      629 2024-05-09 09:30:54.681018 dolbaram-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 dolbaram-0.2.8/PKG-INFO
```

### Comparing `dolbaram-0.2.7/dolbaram/dolbaram.py` & `dolbaram-0.2.8/dolbaram/dolbaram.py`

 * *Files identical despite different names*

### Comparing `dolbaram-0.2.7/pyproject.toml` & `dolbaram-0.2.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dolbaram"
-version = "0.2.7"
+version = "0.2.8"
 description = ""
 authors = ["Kwangsik Lee <lks21c@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fire = "^0.4.0"
@@ -16,14 +16,15 @@
 ujson = "^5.5.0"
 requests = "^2.28.1"
 great-expectations = "0.18.12"
 pyathena = "3.0.6"
 sqlalchemy = "1.4.49"
 pyspark = "^3.5.1"
 baram = "^0.4.4"
+great-expectations-experimental = "^0.1.20240502061"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `dolbaram-0.2.7/PKG-INFO` & `dolbaram-0.2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dolbaram
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 Author: Kwangsik Lee
 Author-email: lks21c@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: baram (>=0.4.4,<0.5.0)
 Requires-Dist: boto3 (==1.28.62)
 Requires-Dist: fire (>=0.4.0,<0.5.0)
 Requires-Dist: great-expectations (==0.18.12)
+Requires-Dist: great-expectations-experimental (>=0.1.20240502061,<0.2.0)
 Requires-Dist: nest-asyncio (>=1.5.5,<2.0.0)
 Requires-Dist: pyathena (==3.0.6)
 Requires-Dist: pyspark (>=3.5.1,<4.0.0)
 Requires-Dist: pytest-cov (>=3.0.0,<4.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: sqlalchemy (==1.4.49)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

