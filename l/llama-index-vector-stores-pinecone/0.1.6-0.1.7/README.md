# Comparing `tmp/llama_index_vector_stores_pinecone-0.1.6.tar.gz` & `tmp/llama_index_vector_stores_pinecone-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_pinecone-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_pinecone-0.1.7.tar", max compression
```

## Comparing `llama_index_vector_stores_pinecone-0.1.6.tar` & `llama_index_vector_stores_pinecone-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       49 2024-04-25 19:49:25.720608 llama_index_vector_stores_pinecone-0.1.6/README.md
--rw-r--r--   0        0        0      107 2024-04-25 19:49:25.720608 llama_index_vector_stores_pinecone-0.1.6/llama_index/vector_stores/pinecone/__init__.py
--rw-r--r--   0        0        0    16915 2024-04-25 19:49:25.720608 llama_index_vector_stores_pinecone-0.1.6/llama_index/vector_stores/pinecone/base.py
--rw-r--r--   0        0        0      814 2024-04-25 19:49:25.720608 llama_index_vector_stores_pinecone-0.1.6/llama_index/vector_stores/pinecone/utils.py
--rw-r--r--   0        0        0     1502 2024-04-25 19:49:25.720608 llama_index_vector_stores_pinecone-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 llama_index_vector_stores_pinecone-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       49 2024-05-09 16:04:34.493790 llama_index_vector_stores_pinecone-0.1.7/README.md
+-rw-r--r--   0        0        0      107 2024-05-09 16:04:34.493790 llama_index_vector_stores_pinecone-0.1.7/llama_index/vector_stores/pinecone/__init__.py
+-rw-r--r--   0        0        0    17008 2024-05-09 16:04:34.493790 llama_index_vector_stores_pinecone-0.1.7/llama_index/vector_stores/pinecone/base.py
+-rw-r--r--   0        0        0      814 2024-05-09 16:04:34.493790 llama_index_vector_stores_pinecone-0.1.7/llama_index/vector_stores/pinecone/utils.py
+-rw-r--r--   0        0        0     1502 2024-05-09 16:04:34.493790 llama_index_vector_stores_pinecone-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 llama_index_vector_stores_pinecone-0.1.7/PKG-INFO
```

### Comparing `llama_index_vector_stores_pinecone-0.1.6/llama_index/vector_stores/pinecone/base.py` & `llama_index_vector_stores_pinecone-0.1.7/llama_index/vector_stores/pinecone/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,16 @@
     elif operator == "nin":
         return "$nin"
     else:
         raise ValueError(f"Filter operator {operator} not supported")
 
 
 def build_dict(input_batch: List[List[int]]) -> List[Dict[str, Any]]:
-    """Build a list of sparse dictionaries from a batch of input_ids.
+    """
+    Build a list of sparse dictionaries from a batch of input_ids.
 
     NOTE: taken from https://www.pinecone.io/learn/hybrid-search-intro/.
 
     """
     # store a batch of sparse embeddings
     sparse_emb = []
     # iterate through input batch
@@ -93,27 +94,29 @@
     # return sparse_emb list
     return sparse_emb
 
 
 def generate_sparse_vectors(
     context_batch: List[str], tokenizer: Callable
 ) -> List[Dict[str, Any]]:
-    """Generate sparse vectors from a batch of contexts.
+    """
+    Generate sparse vectors from a batch of contexts.
 
     NOTE: taken from https://www.pinecone.io/learn/hybrid-search-intro/.
 
     """
     # create batch of input_ids
     inputs = tokenizer(context_batch)["input_ids"]
     # create sparse dictionaries
     return build_dict(inputs)
 
 
 def get_default_tokenizer() -> Callable:
-    """Get default tokenizer.
+    """
+    Get default tokenizer.
 
     NOTE: taken from https://www.pinecone.io/learn/hybrid-search-intro/.
 
     """
     from transformers import BertTokenizerFast
 
     orig_tokenizer = BertTokenizerFast.from_pretrained("bert-base-uncased")
@@ -161,15 +164,16 @@
 
 import_err_msg = (
     "`pinecone` package not found, please run `pip install pinecone-client`"
 )
 
 
 class PineconeVectorStore(BasePydanticVectorStore):
-    """Pinecone Vector Store.
+    """
+    Pinecone Vector Store.
 
     In this vector store, embeddings and docs are stored within a
     Pinecone index.
 
     During query time, the index uses Pinecone to query for the top
     k most similar nodes.
 
@@ -300,15 +304,17 @@
             not _is_pinecone_v3()
         ):  # If old version of Pinecone client (version bifurcation temporary):
             if not environment:
                 raise ValueError("environment is required for Pinecone client < 3.0.0")
             pinecone.init(api_key=api_key, environment=environment)
             return pinecone.Index(index_name)
         else:  # If new version of Pinecone client (serverless):
-            pinecone_instance = pinecone.Pinecone(api_key=api_key)
+            pinecone_instance = pinecone.Pinecone(
+                api_key=api_key, source_tag="llamaindex"
+            )
             return pinecone_instance.Index(index_name)
 
     @classmethod
     def from_params(
         cls,
         api_key: Optional[str] = None,
         index_name: Optional[str] = None,
@@ -348,15 +354,16 @@
         return "PinconeVectorStore"
 
     def add(
         self,
         nodes: List[BaseNode],
         **add_kwargs: Any,
     ) -> List[str]:
-        """Add nodes to index.
+        """
+        Add nodes to index.
 
         Args:
             nodes: List[BaseNode]: list of nodes with embeddings
 
         """
         ids = []
         entries = []
@@ -408,15 +415,16 @@
 
     @property
     def client(self) -> Any:
         """Return Pinecone client."""
         return self._pinecone_index
 
     def query(self, query: VectorStoreQuery, **kwargs: Any) -> VectorStoreQueryResult:
-        """Query index for top k most similar nodes.
+        """
+        Query index for top k most similar nodes.
 
         Args:
             query_embedding (List[float]): query embedding
             similarity_top_k (int): top k most similar nodes
 
         """
         sparse_vector = None
```

### Comparing `llama_index_vector_stores_pinecone-0.1.6/llama_index/vector_stores/pinecone/utils.py` & `llama_index_vector_stores_pinecone-0.1.7/llama_index/vector_stores/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_pinecone-0.1.6/pyproject.toml` & `llama_index_vector_stores_pinecone-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores pinecone integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-pinecone"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.13"
 llama-index-core = "^0.10.11.post1"
 pinecone-client = "^3.0.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_pinecone-0.1.6/PKG-INFO` & `llama_index_vector_stores_pinecone-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-pinecone
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index vector_stores pinecone integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

