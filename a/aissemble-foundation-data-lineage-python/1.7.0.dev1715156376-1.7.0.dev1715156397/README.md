# Comparing `tmp/aissemble_foundation_data_lineage_python-1.7.0.dev1715156376.tar.gz` & `tmp/aissemble_foundation_data_lineage_python-1.7.0.dev1715156397.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_data_lineage_python-1.7.0.dev1715156376.tar", max compression
+gzip compressed data, was "aissemble_foundation_data_lineage_python-1.7.0.dev1715156397.tar", max compression
```

## Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376.tar` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     9580 2024-05-08 08:19:13.052214 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/LICENSE
--rw-r--r--   0        0        0     3584 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/README.md
--rw-r--r--   0        0        0     1045 2024-05-08 08:19:36.381593 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/pyproject.toml
--rw-r--r--   0        0        0      557 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/__init__.py
--rw-r--r--   0        0        0     4277 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/data_lineage_config.py
--rw-r--r--   0        0        0     3888 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/dataset.py
--rw-r--r--   0        0        0      674 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/default_properties/microprofile-config.properties
--rw-r--r--   0        0        0     3129 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/emitter.py
--rw-r--r--   0        0        0     3244 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/facet.py
--rw-r--r--   0        0        0     1260 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/job.py
--rw-r--r--   0        0        0     1924 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/lineage_base.py
--rw-r--r--   0        0        0      988 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/run.py
--rw-r--r--   0        0        0     3267 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/run_event.py
--rw-r--r--   0        0        0      414 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/transport.py
--rw-r--r--   0        0        0     6788 2024-05-08 08:12:08.923493 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/util/lineage_util.py
--rw-r--r--   0        0        0     4162 1970-01-01 00:00:00.000000 aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-08 08:19:31.348085 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/LICENSE
+-rw-r--r--   0        0        0     3584 2024-05-08 08:12:12.958269 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/README.md
+-rw-r--r--   0        0        0     1045 2024-05-08 08:19:58.425072 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/pyproject.toml
+-rw-r--r--   0        0        0      557 2024-05-08 08:12:12.958269 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/__init__.py
+-rw-r--r--   0        0        0     4277 2024-05-08 08:12:12.959270 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/data_lineage_config.py
+-rw-r--r--   0        0        0     3888 2024-05-08 08:12:12.959270 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/dataset.py
+-rw-r--r--   0        0        0      674 2024-05-08 08:12:12.959270 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/default_properties/microprofile-config.properties
+-rw-r--r--   0        0        0     3129 2024-05-08 08:12:12.959270 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/emitter.py
+-rw-r--r--   0        0        0     3244 2024-05-08 08:12:12.959270 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/facet.py
+-rw-r--r--   0        0        0     1260 2024-05-08 08:12:12.959270 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/job.py
+-rw-r--r--   0        0        0     1924 2024-05-08 08:12:12.959270 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/lineage_base.py
+-rw-r--r--   0        0        0      988 2024-05-08 08:12:12.959270 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/run.py
+-rw-r--r--   0        0        0     3267 2024-05-08 08:12:12.959270 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/run_event.py
+-rw-r--r--   0        0        0      414 2024-05-08 08:12:12.959270 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/transport.py
+-rw-r--r--   0        0        0     6788 2024-05-08 08:12:12.959270 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/util/lineage_util.py
+-rw-r--r--   0        0        0     4162 1970-01-01 00:00:00.000000 aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/PKG-INFO
```

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/LICENSE` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/README.md` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/README.md`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/pyproject.toml` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-data-lineage-python"
-version = "1.7.0.dev1715156376"
+version = "1.7.0.dev1715156397"
 description = "Data lineage API for Python scripts"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "aissemble_data_lineage", from = "src"}
 ]
 include = [
```

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/__init__.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/data_lineage_config.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/data_lineage_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/dataset.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/dataset.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/default_properties/microprofile-config.properties` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/default_properties/microprofile-config.properties`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/emitter.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/emitter.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/facet.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/facet.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/job.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/job.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/lineage_base.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/lineage_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/run.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/run.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/run_event.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/run_event.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/src/aissemble_data_lineage/util/lineage_util.py` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/src/aissemble_data_lineage/util/lineage_util.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_data_lineage_python-1.7.0.dev1715156376/PKG-INFO` & `aissemble_foundation_data_lineage_python-1.7.0.dev1715156397/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-data-lineage-python
-Version: 1.7.0.dev1715156376
+Version: 1.7.0.dev1715156397
 Summary: Data lineage API for Python scripts
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aissemble-foundation-messaging-python (==1.7.0.*)
```

