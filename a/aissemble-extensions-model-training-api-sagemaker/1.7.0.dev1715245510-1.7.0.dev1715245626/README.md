# Comparing `tmp/aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245510.tar.gz` & `tmp/aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245626.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245510.tar", max compression
+gzip compressed data, was "aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245626.tar", max compression
```

## Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245510.tar` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245626.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9580 2024-05-09 09:04:34.178526 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245510/LICENSE
--rw-r--r--   0        0        0        0 2024-05-09 08:12:10.614245 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245510/README.md
--rw-r--r--   0        0        0      781 2024-05-09 09:05:11.304476 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245510/pyproject.toml
--rw-r--r--   0        0        0     8837 2024-05-09 08:12:10.615245 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245510/src/model_training_api_sagemaker/model_training_api_sagemaker.py
--rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245510/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-09 09:06:27.731169 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245626/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-09 08:12:09.251760 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245626/README.md
+-rw-r--r--   0        0        0      781 2024-05-09 09:07:06.490096 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245626/pyproject.toml
+-rw-r--r--   0        0        0     8837 2024-05-09 08:12:09.251760 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245626/src/model_training_api_sagemaker/model_training_api_sagemaker.py
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245626/PKG-INFO
```

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245510/LICENSE` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245626/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245510/pyproject.toml` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245626/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-extensions-model-training-api-sagemaker"
-version = "1.7.0.dev1715245510"
+version = "1.7.0.dev1715245626"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "model_training_api_sagemaker", from = "src"},
 ]
```

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245510/src/model_training_api_sagemaker/model_training_api_sagemaker.py` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245626/src/model_training_api_sagemaker/model_training_api_sagemaker.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245510/PKG-INFO` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715245626/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-extensions-model-training-api-sagemaker
-Version: 1.7.0.dev1715245510
+Version: 1.7.0.dev1715245626
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: fastapi (>=0.95.0)
 Requires-Dist: krausening (>=19)
```

