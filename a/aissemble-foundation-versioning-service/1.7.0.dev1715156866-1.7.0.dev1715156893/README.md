# Comparing `tmp/aissemble_foundation_versioning_service-1.7.0.dev1715156866.tar.gz` & `tmp/aissemble_foundation_versioning_service-1.7.0.dev1715156893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_versioning_service-1.7.0.dev1715156866.tar", max compression
+gzip compressed data, was "aissemble_foundation_versioning_service-1.7.0.dev1715156893.tar", max compression
```

## Comparing `aissemble_foundation_versioning_service-1.7.0.dev1715156866.tar` & `aissemble_foundation_versioning_service-1.7.0.dev1715156893.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9580 2024-05-08 08:27:18.389263 aissemble_foundation_versioning_service-1.7.0.dev1715156866/LICENSE
--rw-r--r--   0        0        0     2933 2024-05-08 08:12:08.903494 aissemble_foundation_versioning_service-1.7.0.dev1715156866/README.md
--rw-r--r--   0        0        0     1042 2024-05-08 08:27:47.328489 aissemble_foundation_versioning_service-1.7.0.dev1715156866/pyproject.toml
--rw-r--r--   0        0        0     2697 2024-05-08 08:12:08.903494 aissemble_foundation_versioning_service-1.7.0.dev1715156866/src/model_versioning/version.py
--rw-r--r--   0        0        0     2811 2024-05-08 08:12:08.903494 aissemble_foundation_versioning_service-1.7.0.dev1715156866/src/model_versioning/versioning_api.py
--rw-r--r--   0        0        0     1810 2024-05-08 08:12:08.903494 aissemble_foundation_versioning_service-1.7.0.dev1715156866/src/util/maven_util.py
--rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 aissemble_foundation_versioning_service-1.7.0.dev1715156866/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-08 08:27:38.354856 aissemble_foundation_versioning_service-1.7.0.dev1715156893/LICENSE
+-rw-r--r--   0        0        0     2933 2024-05-08 08:12:12.931270 aissemble_foundation_versioning_service-1.7.0.dev1715156893/README.md
+-rw-r--r--   0        0        0     1042 2024-05-08 08:28:13.695840 aissemble_foundation_versioning_service-1.7.0.dev1715156893/pyproject.toml
+-rw-r--r--   0        0        0     2697 2024-05-08 08:12:12.932270 aissemble_foundation_versioning_service-1.7.0.dev1715156893/src/model_versioning/version.py
+-rw-r--r--   0        0        0     2811 2024-05-08 08:12:12.932270 aissemble_foundation_versioning_service-1.7.0.dev1715156893/src/model_versioning/versioning_api.py
+-rw-r--r--   0        0        0     1810 2024-05-08 08:12:12.932270 aissemble_foundation_versioning_service-1.7.0.dev1715156893/src/util/maven_util.py
+-rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 aissemble_foundation_versioning_service-1.7.0.dev1715156893/PKG-INFO
```

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1715156866/LICENSE` & `aissemble_foundation_versioning_service-1.7.0.dev1715156893/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1715156866/README.md` & `aissemble_foundation_versioning_service-1.7.0.dev1715156893/README.md`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1715156866/pyproject.toml` & `aissemble_foundation_versioning_service-1.7.0.dev1715156893/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-versioning-service"
-version = "1.7.0.dev1715156866"
+version = "1.7.0.dev1715156893"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "model_versioning", from = "src"},
     {include = "util", from = "src"}
 ]
```

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1715156866/src/model_versioning/version.py` & `aissemble_foundation_versioning_service-1.7.0.dev1715156893/src/model_versioning/version.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1715156866/src/model_versioning/versioning_api.py` & `aissemble_foundation_versioning_service-1.7.0.dev1715156893/src/model_versioning/versioning_api.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1715156866/src/util/maven_util.py` & `aissemble_foundation_versioning_service-1.7.0.dev1715156893/src/util/maven_util.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1715156866/PKG-INFO` & `aissemble_foundation_versioning_service-1.7.0.dev1715156893/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-versioning-service
-Version: 1.7.0.dev1715156866
+Version: 1.7.0.dev1715156893
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: fastapi (>=0.95.0)
 Requires-Dist: mlflow (>=2.3.1,<3.0.0)
```

