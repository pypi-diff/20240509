# Comparing `tmp/langchain_ibm-0.1.5.tar.gz` & `tmp/langchain_ibm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_ibm-0.1.5.tar", max compression
+gzip compressed data, was "langchain_ibm-0.1.6.tar", max compression
```

## Comparing `langchain_ibm-0.1.5.tar` & `langchain_ibm-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/LICENSE
--rw-r--r--   0        0        0     4395 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/README.md
--rw-r--r--   0        0        0      144 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/langchain_ibm/__init__.py
--rw-r--r--   0        0        0     6694 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/langchain_ibm/embeddings.py
--rw-r--r--   0        0        0    16163 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/langchain_ibm/llms.py
--rw-r--r--   0        0        0        0 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/langchain_ibm/py.typed
--rw-r--r--   0        0        0     2564 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 langchain_ibm-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4395 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/README.md
+-rw-r--r--   0        0        0      144 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/langchain_ibm/__init__.py
+-rw-r--r--   0        0        0     6702 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/langchain_ibm/embeddings.py
+-rw-r--r--   0        0        0    16171 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/langchain_ibm/llms.py
+-rw-r--r--   0        0        0        0 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/langchain_ibm/py.typed
+-rw-r--r--   0        0        0     2564 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 langchain_ibm-0.1.6/PKG-INFO
```

### Comparing `langchain_ibm-0.1.5/LICENSE` & `langchain_ibm-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_ibm-0.1.5/README.md` & `langchain_ibm-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `langchain_ibm-0.1.5/langchain_ibm/embeddings.py` & `langchain_ibm-0.1.6/langchain_ibm/embeddings.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     version: Optional[SecretStr] = None
     """Version of CPD instance"""
 
     params: Optional[dict] = None
     """Model parameters to use during generate requests."""
 
-    verify: Union[str, bool] = ""
+    verify: Union[str, bool, None] = None
     """User can pass as verify one of following:
         the path to a CA_BUNDLE file
         the path of directory with certificates of trusted CAs
         True - default path to truststore will be taken
         False - no verification will be made"""
 
     watsonx_embed: Embeddings = Field(default=None)  #: :meta private:
```

### Comparing `langchain_ibm-0.1.5/langchain_ibm/llms.py` & `langchain_ibm-0.1.6/langchain_ibm/llms.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     version: Optional[SecretStr] = None
     """Version of CPD instance"""
 
     params: Optional[dict] = None
     """Model parameters to use during generate requests."""
 
-    verify: Union[str, bool] = ""
+    verify: Union[str, bool, None] = None
     """User can pass as verify one of following:
         the path to a CA_BUNDLE file
         the path of directory with certificates of trusted CAs
         True - default path to truststore will be taken
         False - no verification will be made"""
 
     streaming: bool = False
```

### Comparing `langchain_ibm-0.1.5/pyproject.toml` & `langchain_ibm-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-ibm"
-version = "0.1.5"
+version = "0.1.6"
 description = "An integration package connecting IBM watsonx.ai and LangChain"
 authors = ["IBM"]
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_ibm-0.1.5/PKG-INFO` & `langchain_ibm-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-ibm
-Version: 0.1.5
+Version: 0.1.6
 Summary: An integration package connecting IBM watsonx.ai and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Author: IBM
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

