# Comparing `tmp/llama_index_llms_nvidia-0.1.1.tar.gz` & `tmp/llama_index_llms_nvidia-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_nvidia-0.1.1.tar", max compression
+gzip compressed data, was "llama_index_llms_nvidia-0.1.2.tar", max compression
```

## Comparing `llama_index_llms_nvidia-0.1.1.tar` & `llama_index_llms_nvidia-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1004 2024-05-08 15:34:13.578998 llama_index_llms_nvidia-0.1.1/README.md
--rw-r--r--   0        0        0       17 2024-05-08 15:34:13.578998 llama_index_llms_nvidia-0.1.1/llama_index/llms/nvidia/BUILD
--rw-r--r--   0        0        0       70 2024-05-08 15:34:13.578998 llama_index_llms_nvidia-0.1.1/llama_index/llms/nvidia/__init__.py
--rw-r--r--   0        0        0     3189 2024-05-08 15:34:13.578998 llama_index_llms_nvidia-0.1.1/llama_index/llms/nvidia/base.py
--rw-r--r--   0        0        0      617 2024-05-08 15:34:13.578998 llama_index_llms_nvidia-0.1.1/llama_index/llms/nvidia/utils.py
--rw-r--r--   0        0        0     1738 2024-05-08 15:34:13.578998 llama_index_llms_nvidia-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 llama_index_llms_nvidia-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1004 2024-05-09 20:01:33.838047 llama_index_llms_nvidia-0.1.2/README.md
+-rw-r--r--   0        0        0       17 2024-05-09 20:01:33.838047 llama_index_llms_nvidia-0.1.2/llama_index/llms/nvidia/BUILD
+-rw-r--r--   0        0        0       70 2024-05-09 20:01:33.838047 llama_index_llms_nvidia-0.1.2/llama_index/llms/nvidia/__init__.py
+-rw-r--r--   0        0        0     3440 2024-05-09 20:01:33.838047 llama_index_llms_nvidia-0.1.2/llama_index/llms/nvidia/base.py
+-rw-r--r--   0        0        0      617 2024-05-09 20:01:33.838047 llama_index_llms_nvidia-0.1.2/llama_index/llms/nvidia/utils.py
+-rw-r--r--   0        0        0     1738 2024-05-09 20:01:33.838047 llama_index_llms_nvidia-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 llama_index_llms_nvidia-0.1.2/PKG-INFO
```

### Comparing `llama_index_llms_nvidia-0.1.1/README.md` & `llama_index_llms_nvidia-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_llms_nvidia-0.1.1/llama_index/llms/nvidia/base.py` & `llama_index_llms_nvidia-0.1.2/llama_index/llms/nvidia/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 )
 
 from llama_index.core.bridge.pydantic import PrivateAttr, BaseModel
 from llama_index.core.base.llms.generic_utils import (
     get_from_param_or_env,
 )
 
-from llama_index.llms.nvidia.utils import API_CATALOG_MODELS
 
 from llama_index.llms.openai_like import OpenAILike
 
 DEFAULT_MODEL = "meta/llama3-8b-instruct"
 BASE_URL = "https://integrate.api.nvidia.com/v1/"
 
 
@@ -50,18 +49,27 @@
             is_chat_model=True,
             default_headers={"User-Agent": "llama-index-llms-nvidia"},
             **kwargs,
         )
 
     @property
     def available_models(self) -> List[Model]:
-        ids = API_CATALOG_MODELS.keys()
+        exclude = {
+            "mistralai/mixtral-8x22b-v0.1",  # not a /chat/completion endpoint
+        }
+        # do not exclude models in nim mode. the nim administrator has control
+        # over the model name and may deploy an excluded name on the nim's
+        # /chat/completion endpoint.
         if self._mode == "nim":
-            ids = [model.id for model in self._get_client().models.list()]
-        return [Model(id=name) for name in ids]
+            exclude = set()
+        return [
+            model
+            for model in self._get_client().models.list().data
+            if model.id not in exclude
+        ]
 
     @classmethod
     def class_name(cls) -> str:
         return "NVIDIA"
 
     def mode(
         self,
```

### Comparing `llama_index_llms_nvidia-0.1.1/llama_index/llms/nvidia/utils.py` & `llama_index_llms_nvidia-0.1.2/llama_index/llms/nvidia/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_nvidia-0.1.1/pyproject.toml` & `llama_index_llms_nvidia-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [tool.poetry]
 authors = ["Chris Alexiuk <calexiuk@nvidia.com>"]
 description = "llama-index llms nvidia api catalog integration"
 license = "MIT"
 name = "llama-index-llms-nvidia"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 llama-index-llms-openai = "^0.1.17"
 llama-index-llms-openai-like = "^0.1.3"
```

### Comparing `llama_index_llms_nvidia-0.1.1/PKG-INFO` & `llama_index_llms_nvidia-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-nvidia
-Version: 0.1.1
+Version: 0.1.2
 Summary: llama-index llms nvidia api catalog integration
 License: MIT
 Author: Chris Alexiuk
 Author-email: calexiuk@nvidia.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

