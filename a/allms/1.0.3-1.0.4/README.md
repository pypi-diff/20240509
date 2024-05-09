# Comparing `tmp/allms-1.0.3.tar.gz` & `tmp/allms-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allms-1.0.3.tar", max compression
+gzip compressed data, was "allms-1.0.4.tar", max compression
```

## Comparing `allms-1.0.3.tar` & `allms-1.0.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2024-04-18 13:17:53.931928 allms-1.0.3/LICENSE
--rw-r--r--   0        0        0     8996 2024-04-18 13:17:53.931928 allms-1.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/chains/__init__.py
--rw-r--r--   0        0        0     4864 2024-04-18 13:17:53.931928 allms-1.0.3/allms/chains/long_text_processing_chain.py
--rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/constants/__init__.py
--rw-r--r--   0        0        0      575 2024-04-18 13:17:53.931928 allms-1.0.3/allms/constants/azure.py
--rw-r--r--   0        0        0      877 2024-04-18 13:17:53.931928 allms-1.0.3/allms/constants/input_data.py
--rw-r--r--   0        0        0      258 2024-04-18 13:17:53.931928 allms-1.0.3/allms/constants/prompt.py
--rw-r--r--   0        0        0      270 2024-04-18 13:17:53.931928 allms-1.0.3/allms/constants/vertex_ai.py
--rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/defaults/__init__.py
--rw-r--r--   0        0        0      666 2024-04-18 13:17:53.931928 allms-1.0.3/allms/defaults/azure_defaults.py
--rw-r--r--   0        0        0      117 2024-04-18 13:17:53.931928 allms-1.0.3/allms/defaults/general_defaults.py
--rw-r--r--   0        0        0      469 2024-04-18 13:17:53.931928 allms-1.0.3/allms/defaults/long_text_chain.py
--rw-r--r--   0        0        0      676 2024-04-18 13:17:53.931928 allms-1.0.3/allms/defaults/vertex_ai.py
--rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/domain/__init__.py
--rw-r--r--   0        0        0      471 2024-04-18 13:17:53.931928 allms-1.0.3/allms/domain/configuration.py
--rw-r--r--   0        0        0      777 2024-04-18 13:17:53.931928 allms-1.0.3/allms/domain/enumerables.py
--rw-r--r--   0        0        0      229 2024-04-18 13:17:53.931928 allms-1.0.3/allms/domain/input_data.py
--rw-r--r--   0        0        0      444 2024-04-18 13:17:53.931928 allms-1.0.3/allms/domain/prompt_dto.py
--rw-r--r--   0        0        0      726 2024-04-18 13:17:53.931928 allms-1.0.3/allms/domain/response.py
--rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/exceptions/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-18 13:17:53.931928 allms-1.0.3/allms/exceptions/validation_input_data_exceptions.py
--rw-r--r--   0        0        0     1134 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/__init__.py
--rw-r--r--   0        0        0    16564 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/abstract.py
--rw-r--r--   0        0        0      935 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/azure_base.py
--rw-r--r--   0        0        0     2247 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/azure_llama2.py
--rw-r--r--   0        0        0     2170 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/azure_mistral.py
--rw-r--r--   0        0        0     1840 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/azure_openai.py
--rw-r--r--   0        0        0     3894 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/vertexai_base.py
--rw-r--r--   0        0        0     1965 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/vertexai_gemini.py
--rw-r--r--   0        0        0     2128 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/vertexai_gemma.py
--rw-r--r--   0        0        0     1947 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/vertexai_palm.py
--rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/utils/__init__.py
--rw-r--r--   0        0        0     1256 2024-04-18 13:17:53.931928 allms-1.0.3/allms/utils/io_utils.py
--rw-r--r--   0        0        0      291 2024-04-18 13:17:53.931928 allms-1.0.3/allms/utils/logger_utils.py
--rw-r--r--   0        0        0     4839 2024-04-18 13:17:53.931928 allms-1.0.3/allms/utils/long_text_processing_utils.py
--rw-r--r--   0        0        0     2607 2024-04-18 13:17:53.931928 allms-1.0.3/allms/utils/response_parsing_utils.py
--rw-r--r--   0        0        0      663 2024-04-18 13:17:53.935928 allms-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     9825 1970-01-01 00:00:00.000000 allms-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-09 09:53:22.239090 allms-1.0.4/LICENSE
+-rw-r--r--   0        0        0     8996 2024-05-09 09:53:22.239090 allms-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:53:22.243090 allms-1.0.4/allms/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:53:22.243090 allms-1.0.4/allms/chains/__init__.py
+-rw-r--r--   0        0        0     4864 2024-05-09 09:53:22.243090 allms-1.0.4/allms/chains/long_text_processing_chain.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:53:22.243090 allms-1.0.4/allms/constants/__init__.py
+-rw-r--r--   0        0        0      575 2024-05-09 09:53:22.243090 allms-1.0.4/allms/constants/azure.py
+-rw-r--r--   0        0        0      877 2024-05-09 09:53:22.243090 allms-1.0.4/allms/constants/input_data.py
+-rw-r--r--   0        0        0      258 2024-05-09 09:53:22.243090 allms-1.0.4/allms/constants/prompt.py
+-rw-r--r--   0        0        0      270 2024-05-09 09:53:22.243090 allms-1.0.4/allms/constants/vertex_ai.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:53:22.243090 allms-1.0.4/allms/defaults/__init__.py
+-rw-r--r--   0        0        0      666 2024-05-09 09:53:22.243090 allms-1.0.4/allms/defaults/azure_defaults.py
+-rw-r--r--   0        0        0      117 2024-05-09 09:53:22.243090 allms-1.0.4/allms/defaults/general_defaults.py
+-rw-r--r--   0        0        0      469 2024-05-09 09:53:22.243090 allms-1.0.4/allms/defaults/long_text_chain.py
+-rw-r--r--   0        0        0      676 2024-05-09 09:53:22.243090 allms-1.0.4/allms/defaults/vertex_ai.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:53:22.243090 allms-1.0.4/allms/domain/__init__.py
+-rw-r--r--   0        0        0     1037 2024-05-09 09:53:22.243090 allms-1.0.4/allms/domain/configuration.py
+-rw-r--r--   0        0        0      777 2024-05-09 09:53:22.243090 allms-1.0.4/allms/domain/enumerables.py
+-rw-r--r--   0        0        0      229 2024-05-09 09:53:22.243090 allms-1.0.4/allms/domain/input_data.py
+-rw-r--r--   0        0        0      444 2024-05-09 09:53:22.243090 allms-1.0.4/allms/domain/prompt_dto.py
+-rw-r--r--   0        0        0      726 2024-05-09 09:53:22.243090 allms-1.0.4/allms/domain/response.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:53:22.243090 allms-1.0.4/allms/exceptions/__init__.py
+-rw-r--r--   0        0        0     1548 2024-05-09 09:53:22.243090 allms-1.0.4/allms/exceptions/validation_input_data_exceptions.py
+-rw-r--r--   0        0        0     1134 2024-05-09 09:53:22.243090 allms-1.0.4/allms/models/__init__.py
+-rw-r--r--   0        0        0    16564 2024-05-09 09:53:22.243090 allms-1.0.4/allms/models/abstract.py
+-rw-r--r--   0        0        0      935 2024-05-09 09:53:22.243090 allms-1.0.4/allms/models/azure_base.py
+-rw-r--r--   0        0        0     2247 2024-05-09 09:53:22.243090 allms-1.0.4/allms/models/azure_llama2.py
+-rw-r--r--   0        0        0     2170 2024-05-09 09:53:22.243090 allms-1.0.4/allms/models/azure_mistral.py
+-rw-r--r--   0        0        0     1840 2024-05-09 09:53:22.243090 allms-1.0.4/allms/models/azure_openai.py
+-rw-r--r--   0        0        0     3894 2024-05-09 09:53:22.243090 allms-1.0.4/allms/models/vertexai_base.py
+-rw-r--r--   0        0        0     1961 2024-05-09 09:53:22.243090 allms-1.0.4/allms/models/vertexai_gemini.py
+-rw-r--r--   0        0        0     2128 2024-05-09 09:53:22.243090 allms-1.0.4/allms/models/vertexai_gemma.py
+-rw-r--r--   0        0        0     1943 2024-05-09 09:53:22.243090 allms-1.0.4/allms/models/vertexai_palm.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:53:22.243090 allms-1.0.4/allms/utils/__init__.py
+-rw-r--r--   0        0        0     1256 2024-05-09 09:53:22.243090 allms-1.0.4/allms/utils/io_utils.py
+-rw-r--r--   0        0        0      291 2024-05-09 09:53:22.243090 allms-1.0.4/allms/utils/logger_utils.py
+-rw-r--r--   0        0        0     4839 2024-05-09 09:53:22.243090 allms-1.0.4/allms/utils/long_text_processing_utils.py
+-rw-r--r--   0        0        0     2607 2024-05-09 09:53:22.243090 allms-1.0.4/allms/utils/response_parsing_utils.py
+-rw-r--r--   0        0        0      663 2024-05-09 09:53:22.247090 allms-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9825 1970-01-01 00:00:00.000000 allms-1.0.4/PKG-INFO
```

### Comparing `allms-1.0.3/LICENSE` & `allms-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/README.md` & `allms-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/chains/long_text_processing_chain.py` & `allms-1.0.4/allms/chains/long_text_processing_chain.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/constants/azure.py` & `allms-1.0.4/allms/constants/azure.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/constants/input_data.py` & `allms-1.0.4/allms/constants/input_data.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/defaults/azure_defaults.py` & `allms-1.0.4/allms/defaults/azure_defaults.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/defaults/vertex_ai.py` & `allms-1.0.4/allms/defaults/vertex_ai.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/domain/enumerables.py` & `allms-1.0.4/allms/domain/enumerables.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/domain/response.py` & `allms-1.0.4/allms/domain/response.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/exceptions/validation_input_data_exceptions.py` & `allms-1.0.4/allms/exceptions/validation_input_data_exceptions.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/models/__init__.py` & `allms-1.0.4/allms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/models/abstract.py` & `allms-1.0.4/allms/models/abstract.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/models/azure_base.py` & `allms-1.0.4/allms/models/azure_base.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/models/azure_llama2.py` & `allms-1.0.4/allms/models/azure_llama2.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/models/azure_mistral.py` & `allms-1.0.4/allms/models/azure_mistral.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/models/azure_openai.py` & `allms-1.0.4/allms/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/models/vertexai_base.py` & `allms-1.0.4/allms/models/vertexai_base.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/models/vertexai_gemini.py` & `allms-1.0.4/allms/models/vertexai_gemini.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             max_concurrency=max_concurrency,
             max_retries=max_retries,
             event_loop=event_loop
         )
 
     def _create_llm(self) -> VertexAI:
         return CustomVertexAI(
-            model_name=GeminiModelDefaults.GCP_MODEL_NAME,
+            model_name=self._config.gemini_model_name,
             max_output_tokens=self._max_output_tokens,
             temperature=self._temperature,
             top_p=self._top_p,
             top_k=self._top_k,
             verbose=self._verbose,
             project=self._config.cloud_project,
             location=self._config.cloud_location
```

### Comparing `allms-1.0.3/allms/models/vertexai_gemma.py` & `allms-1.0.4/allms/models/vertexai_gemma.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/models/vertexai_palm.py` & `allms-1.0.4/allms/models/vertexai_palm.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             max_concurrency=max_concurrency,
             max_retries=max_retries,
             event_loop=event_loop
         )
 
     def _create_llm(self) -> VertexAI:
         return CustomVertexAI(
-            model_name=PalmModelDefaults.GCP_MODEL_NAME,
+            model_name=self._config.palm_model_name,
             max_output_tokens=self._max_output_tokens,
             temperature=self._temperature,
             top_p=self._top_p,
             top_k=self._top_k,
             verbose=self._verbose,
             project=self._config.cloud_project,
             location=self._config.cloud_location
```

### Comparing `allms-1.0.3/allms/utils/io_utils.py` & `allms-1.0.4/allms/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/utils/long_text_processing_utils.py` & `allms-1.0.4/allms/utils/long_text_processing_utils.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/allms/utils/response_parsing_utils.py` & `allms-1.0.4/allms/utils/response_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.3/pyproject.toml` & `allms-1.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "allms"
-version = "1.0.3"
+version = "1.0.4"
 description = ""
 authors = ["Allegro Opensource <opensource@allegro.com>"]
 readme = "README.md"
 packages = [{include = "allms"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `allms-1.0.3/PKG-INFO` & `allms-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allms
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Author: Allegro Opensource
 Author-email: opensource@allegro.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

