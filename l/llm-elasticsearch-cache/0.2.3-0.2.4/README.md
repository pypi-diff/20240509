# Comparing `tmp/llm_elasticsearch_cache-0.2.3.tar.gz` & `tmp/llm_elasticsearch_cache-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_elasticsearch_cache-0.2.3.tar", max compression
+gzip compressed data, was "llm_elasticsearch_cache-0.2.4.tar", max compression
```

## Comparing `llm_elasticsearch_cache-0.2.3.tar` & `llm_elasticsearch_cache-0.2.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2024-02-12 12:29:42.006502 llm_elasticsearch_cache-0.2.3/LICENSE
--rw-r--r--   0        0        0     4792 2024-05-09 09:47:51.709916 llm_elasticsearch_cache-0.2.3/README.md
--rw-r--r--   0        0        0     1254 2024-05-09 09:53:09.080846 llm_elasticsearch_cache-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-12 12:54:53.592163 llm_elasticsearch_cache-0.2.3/src/llmescache/__init__.py
--rw-r--r--   0        0        0      185 2024-02-28 08:37:18.743318 llm_elasticsearch_cache-0.2.3/src/llmescache/langchain/__init__.py
--rw-r--r--   0        0        0     1128 2024-03-26 08:12:00.625891 llm_elasticsearch_cache-0.2.3/src/llmescache/langchain/base.py
--rw-r--r--   0        0        0     5384 2024-03-26 08:12:00.626922 llm_elasticsearch_cache-0.2.3/src/llmescache/langchain/cache.py
--rw-r--r--   0        0        0     6094 2024-04-08 10:11:31.752144 llm_elasticsearch_cache-0.2.3/src/llmescache/langchain/storage.py
--rw-r--r--   0        0        0        0 2024-02-20 16:20:08.430038 llm_elasticsearch_cache-0.2.3/src/llmescache/py.typed
--rw-r--r--   0        0        0     5926 1970-01-01 00:00:00.000000 llm_elasticsearch_cache-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-02-12 12:29:42.006502 llm_elasticsearch_cache-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4792 2024-05-09 09:47:51.709916 llm_elasticsearch_cache-0.2.4/README.md
+-rw-r--r--   0        0        0     1295 2024-05-09 09:56:27.225327 llm_elasticsearch_cache-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-12 12:54:53.592163 llm_elasticsearch_cache-0.2.4/src/llmescache/__init__.py
+-rw-r--r--   0        0        0      185 2024-02-28 08:37:18.743318 llm_elasticsearch_cache-0.2.4/src/llmescache/langchain/__init__.py
+-rw-r--r--   0        0        0     1128 2024-03-26 08:12:00.625891 llm_elasticsearch_cache-0.2.4/src/llmescache/langchain/base.py
+-rw-r--r--   0        0        0     5384 2024-03-26 08:12:00.626922 llm_elasticsearch_cache-0.2.4/src/llmescache/langchain/cache.py
+-rw-r--r--   0        0        0     6094 2024-04-08 10:11:31.752144 llm_elasticsearch_cache-0.2.4/src/llmescache/langchain/storage.py
+-rw-r--r--   0        0        0        0 2024-02-20 16:20:08.430038 llm_elasticsearch_cache-0.2.4/src/llmescache/py.typed
+-rw-r--r--   0        0        0     5973 1970-01-01 00:00:00.000000 llm_elasticsearch_cache-0.2.4/PKG-INFO
```

### Comparing `llm_elasticsearch_cache-0.2.3/LICENSE` & `llm_elasticsearch_cache-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.3/README.md` & `llm_elasticsearch_cache-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.3/pyproject.toml` & `llm_elasticsearch_cache-0.2.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-elasticsearch-cache"
-version = "0.2.3"
+version = "0.2.4"
 description = "A caching layer for LLMs that exploits Elasticsearch, fully compatible with LangChain caching, both for chat and embeddings models."
 packages = [{include = "llmescache", from = "./src"}]
 authors = ["SpazioDati s.r.l."]
 maintainers = ["Giacomo Berardi <berardi@spaziodati.eu>", "Gabriele Ghisleni <gabriele.ghisleni@spaziodati.eu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/SpazioDati/llm-elasticsearch-cache"
@@ -15,14 +15,15 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Development Status :: 7 - Inactive"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 langchain = "^0.1"
 elasticsearch = ">6"
```

### Comparing `llm_elasticsearch_cache-0.2.3/src/llmescache/langchain/base.py` & `llm_elasticsearch_cache-0.2.4/src/llmescache/langchain/base.py`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.3/src/llmescache/langchain/cache.py` & `llm_elasticsearch_cache-0.2.4/src/llmescache/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.3/src/llmescache/langchain/storage.py` & `llm_elasticsearch_cache-0.2.4/src/llmescache/langchain/storage.py`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.3/PKG-INFO` & `llm_elasticsearch_cache-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: llm-elasticsearch-cache
-Version: 0.2.3
+Version: 0.2.4
 Summary: A caching layer for LLMs that exploits Elasticsearch, fully compatible with LangChain caching, both for chat and embeddings models.
 Home-page: https://github.com/SpazioDati/llm-elasticsearch-cache
 License: MIT
 Keywords: langchain,elasticsearch,openai,llm,chatgpt
 Author: SpazioDati s.r.l.
 Maintainer: Giacomo Berardi
 Maintainer-email: berardi@spaziodati.eu
 Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 7 - Inactive
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

