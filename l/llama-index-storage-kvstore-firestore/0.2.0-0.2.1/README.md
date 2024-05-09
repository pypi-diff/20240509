# Comparing `tmp/llama_index_storage_kvstore_firestore-0.2.0.tar.gz` & `tmp/llama_index_storage_kvstore_firestore-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_storage_kvstore_firestore-0.2.0.tar", max compression
+gzip compressed data, was "llama_index_storage_kvstore_firestore-0.2.1.tar", max compression
```

## Comparing `llama_index_storage_kvstore_firestore-0.2.0.tar` & `llama_index_storage_kvstore_firestore-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       52 2024-04-23 21:20:01.676316 llama_index_storage_kvstore_firestore-0.2.0/README.md
--rw-r--r--   0        0        0      104 2024-04-23 21:20:01.676316 llama_index_storage_kvstore_firestore-0.2.0/llama_index/storage/kvstore/firestore/__init__.py
--rw-r--r--   0        0        0     7983 2024-04-23 21:20:01.676316 llama_index_storage_kvstore_firestore-0.2.0/llama_index/storage/kvstore/firestore/base.py
--rw-r--r--   0        0        0     1498 2024-04-23 21:20:01.676316 llama_index_storage_kvstore_firestore-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 llama_index_storage_kvstore_firestore-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       52 2024-05-09 20:02:15.325084 llama_index_storage_kvstore_firestore-0.2.1/README.md
+-rw-r--r--   0        0        0      104 2024-05-09 20:02:15.325084 llama_index_storage_kvstore_firestore-0.2.1/llama_index/storage/kvstore/firestore/__init__.py
+-rw-r--r--   0        0        0     7991 2024-05-09 20:02:15.325084 llama_index_storage_kvstore_firestore-0.2.1/llama_index/storage/kvstore/firestore/base.py
+-rw-r--r--   0        0        0     1498 2024-05-09 20:02:15.325084 llama_index_storage_kvstore_firestore-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 llama_index_storage_kvstore_firestore-0.2.1/PKG-INFO
```

### Comparing `llama_index_storage_kvstore_firestore-0.2.0/llama_index/storage/kvstore/firestore/base.py` & `llama_index_storage_kvstore_firestore-0.2.1/llama_index/storage/kvstore/firestore/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
             collection (str): collection name
         """
         collection_id = self.firestore_collection(collection)
         docs = self._adb.collection(collection_id).list_documents()
         output = {}
         async for doc in docs:
             key = doc.id
-            data = doc.get().to_dict()
+            data = (await doc.get()).to_dict()
             if data is None:
                 continue
             val = self.replace_field_name_get(data)
             output[key] = val
         return output
 
     def delete(self, key: str, collection: str = DEFAULT_COLLECTION) -> bool:
```

### Comparing `llama_index_storage_kvstore_firestore-0.2.0/pyproject.toml` & `llama_index_storage_kvstore_firestore-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index kvstore firestore integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-storage-kvstore-firestore"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 llama-index-core = "^0.10.1"
 google-cloud-firestore = "^2.14.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_storage_kvstore_firestore-0.2.0/PKG-INFO` & `llama_index_storage_kvstore_firestore-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-storage-kvstore-firestore
-Version: 0.2.0
+Version: 0.2.1
 Summary: llama-index kvstore firestore integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

