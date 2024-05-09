# Comparing `tmp/aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505.tar.gz` & `tmp/aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159556.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505.tar", max compression
+gzip compressed data, was "aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159556.tar", max compression
```

## Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505.tar` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159556.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9580 2024-05-08 09:11:05.300400 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/LICENSE
--rw-r--r--   0        0        0        0 2024-05-08 08:12:12.864270 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/README.md
--rw-r--r--   0        0        0      781 2024-05-08 09:11:46.146405 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/pyproject.toml
--rw-r--r--   0        0        0     8837 2024-05-08 08:12:12.864270 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/src/model_training_api_sagemaker/model_training_api_sagemaker.py
--rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-08 09:11:57.567732 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159556/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-08 08:12:08.853495 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159556/README.md
+-rw-r--r--   0        0        0      781 2024-05-08 09:12:36.676696 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159556/pyproject.toml
+-rw-r--r--   0        0        0     8837 2024-05-08 08:12:08.853495 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159556/src/model_training_api_sagemaker/model_training_api_sagemaker.py
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159556/PKG-INFO
```

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/LICENSE` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159556/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/pyproject.toml` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159556/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-extensions-model-training-api-sagemaker"
-version = "1.7.0.dev1715159505"
+version = "1.7.0.dev1715159556"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "model_training_api_sagemaker", from = "src"},
 ]
```

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/src/model_training_api_sagemaker/model_training_api_sagemaker.py` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159556/src/model_training_api_sagemaker/model_training_api_sagemaker.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/PKG-INFO` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159556/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-extensions-model-training-api-sagemaker
-Version: 1.7.0.dev1715159505
+Version: 1.7.0.dev1715159556
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: fastapi (>=0.95.0)
 Requires-Dist: krausening (>=19)
```

