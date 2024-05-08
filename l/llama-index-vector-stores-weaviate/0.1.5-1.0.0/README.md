# Comparing `tmp/llama_index_vector_stores_weaviate-0.1.5.tar.gz` & `tmp/llama_index_vector_stores_weaviate-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_weaviate-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_weaviate-1.0.0.tar", max compression
```

## Comparing `llama_index_vector_stores_weaviate-0.1.5.tar` & `llama_index_vector_stores_weaviate-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       49 2024-04-22 02:36:02.224598 llama_index_vector_stores_weaviate-0.1.5/README.md
--rw-r--r--   0        0        0      107 2024-04-22 02:36:02.224598 llama_index_vector_stores_weaviate-0.1.5/llama_index/vector_stores/weaviate/__init__.py
--rw-r--r--   0        0        0    12383 2024-04-22 02:36:02.224598 llama_index_vector_stores_weaviate-0.1.5/llama_index/vector_stores/weaviate/base.py
--rw-r--r--   0        0        0     4890 2024-04-22 02:36:02.224598 llama_index_vector_stores_weaviate-0.1.5/llama_index/vector_stores/weaviate/utils.py
--rw-r--r--   0        0        0     1495 2024-04-22 02:36:02.224598 llama_index_vector_stores_weaviate-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 llama_index_vector_stores_weaviate-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       49 2024-05-08 23:35:30.424383 llama_index_vector_stores_weaviate-1.0.0/README.md
+-rw-r--r--   0        0        0      107 2024-05-08 23:35:30.424383 llama_index_vector_stores_weaviate-1.0.0/llama_index/vector_stores/weaviate/__init__.py
+-rw-r--r--   0        0        0    11585 2024-05-08 23:35:30.424383 llama_index_vector_stores_weaviate-1.0.0/llama_index/vector_stores/weaviate/base.py
+-rw-r--r--   0        0        0     4835 2024-05-08 23:35:30.424383 llama_index_vector_stores_weaviate-1.0.0/llama_index/vector_stores/weaviate/utils.py
+-rw-r--r--   0        0        0     1494 2024-05-08 23:35:30.424383 llama_index_vector_stores_weaviate-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 llama_index_vector_stores_weaviate-1.0.0/PKG-INFO
```

### Comparing `llama_index_vector_stores_weaviate-0.1.5/llama_index/vector_stores/weaviate/base.py` & `llama_index_vector_stores_weaviate-1.0.0/llama_index/vector_stores/weaviate/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Weaviate Vector store index.
 
 An index that is built on top of an existing vector store.
 
 """
 
 import logging
-from typing import Any, Dict, List, Optional, cast
+from typing import Any, Dict, List, Optional, Union, cast
 from uuid import uuid4
 
 from llama_index.core.bridge.pydantic import Field, PrivateAttr
 from llama_index.core.schema import BaseNode
 from llama_index.core.vector_stores.types import (
     BasePydanticVectorStore,
     MetadataFilters,
@@ -24,78 +24,72 @@
     create_default_schema,
     get_all_properties,
     get_node_similarity,
     parse_get_response,
     to_node,
 )
 
-import weaviate  # noqa
-from weaviate import AuthApiKey, Client
+import weaviate
+from weaviate import Client
+import weaviate.classes as wvc
 
 _logger = logging.getLogger(__name__)
 
 
 def _transform_weaviate_filter_condition(condition: str) -> str:
     """Translate standard metadata filter op to Chroma specific spec."""
     if condition == "and":
-        return "And"
+        return wvc.query.Filter.all_of
     elif condition == "or":
-        return "Or"
+        return wvc.query.Filter.any_of
     else:
         raise ValueError(f"Filter condition {condition} not supported")
 
 
 def _transform_weaviate_filter_operator(operator: str) -> str:
-    """Translate standard metadata filter operator to Chroma specific spec."""
+    """Translate standard metadata filter operator to Weaviate specific spec."""
     if operator == "!=":
-        return "NotEqual"
+        return "not_equal"
     elif operator == "==":
-        return "Equal"
+        return "equal"
     elif operator == ">":
-        return "GreaterThan"
+        return "greater_than"
     elif operator == "<":
-        return "LessThan"
+        return "less_than"
     elif operator == ">=":
-        return "GreaterThanEqual"
+        return "greater_or_equal"
     elif operator == "<=":
-        return "LessThanEqual"
+        return "less_or_equal"
     else:
         raise ValueError(f"Filter operator {operator} not supported")
 
 
-def _to_weaviate_filter(standard_filters: MetadataFilters) -> Dict[str, Any]:
+def _to_weaviate_filter(
+    standard_filters: MetadataFilters,
+) -> Union[wvc.query.Filter, List[wvc.query.Filter]]:
     filters_list = []
     condition = standard_filters.condition or "and"
     condition = _transform_weaviate_filter_condition(condition)
 
     if standard_filters.filters:
         for filter in standard_filters.filters:
-            value_type = "valueText"
-            if isinstance(filter.value, float):
-                value_type = "valueNumber"
-            elif isinstance(filter.value, int):
-                value_type = "valueInt"
-            elif isinstance(filter.value, str) and filter.value.isnumeric():
-                filter.value = float(filter.value)
-                value_type = "valueNumber"
             filters_list.append(
-                {
-                    "path": filter.key,
-                    "operator": _transform_weaviate_filter_operator(filter.operator),
-                    value_type: filter.value,
-                }
+                getattr(
+                    wvc.query.Filter.by_property(filter.key),
+                    _transform_weaviate_filter_operator(filter.operator),
+                )(filter.value)
             )
     else:
         return {}
 
     if len(filters_list) == 1:
         # If there is only one filter, return it directly
         return filters_list[0]
 
-    return {"operands": filters_list, "operator": condition}
+    return condition(filters_list)
 
 
 class WeaviateVectorStore(BasePydanticVectorStore):
     """Weaviate vector store.
 
     In this vector store, embeddings and docs are stored within a
     Weaviate collection.
@@ -149,22 +143,22 @@
         client_kwargs: Optional[Dict[str, Any]] = None,
         url: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
         if weaviate_client is None:
             if isinstance(auth_config, dict):
-                auth_config = AuthApiKey(**auth_config)
+                auth_config = weaviate.auth.AuthApiKey(auth_config)
 
             client_kwargs = client_kwargs or {}
-            self._client = Client(
-                url=url, auth_client_secret=auth_config, **client_kwargs
+            self._client = weaviate.WeaviateClient(
+                auth_client_secret=auth_config, **client_kwargs
             )
         else:
-            self._client = cast(Client, weaviate_client)
+            self._client = cast(weaviate.WeaviateClient, weaviate_client)
 
         # validate class prefix starts with a capital letter
         if class_prefix is not None:
             _logger.warning("class_prefix is deprecated, please use index_name")
             # legacy, kept for backward compatibility
             index_name = f"{class_prefix}_Node"
 
@@ -229,15 +223,15 @@
 
         Args:
             nodes: List[BaseNode]: list of nodes with embeddings
 
         """
         ids = [r.node_id for r in nodes]
 
-        with self._client.batch as batch:
+        with self._client.batch.dynamic() as batch:
             for node in nodes:
                 add_node(
                     self._client,
                     node,
                     self.index_name,
                     batch=batch,
                     text_key=self.text_key,
@@ -284,96 +278,83 @@
         """
         if not class_schema_exists(self._client, self.index_name):
             _logger.warning(
                 f"Index '{self.index_name}' does not exist. No action taken."
             )
             return
         try:
-            self._client.schema.delete_class(self.index_name)
+            self._client.collections.delete(self.index_name)
             _logger.info(f"Successfully deleted index '{self.index_name}'.")
         except Exception as e:
             _logger.error(f"Failed to delete index '{self.index_name}': {e}")
             raise Exception(f"Failed to delete index '{self.index_name}': {e}")
 
     def query(self, query: VectorStoreQuery, **kwargs: Any) -> VectorStoreQueryResult:
         """Query index for top k most similar nodes."""
         all_properties = get_all_properties(self._client, self.index_name)
-
-        # build query
-        query_builder = self._client.query.get(self.index_name, all_properties)
+        collection = self._client.collections.get(self.index_name)
+        filters = None
 
         # list of documents to constrain search
         if query.doc_ids:
-            filter_with_doc_ids = {
-                "operator": "Or",
-                "operands": [
-                    {"path": ["doc_id"], "operator": "Equal", "valueText": doc_id}
-                    for doc_id in query.doc_ids
-                ],
-            }
-            query_builder = query_builder.with_where(filter_with_doc_ids)
+            filters = wvc.query.Filter.by_property("doc_id").contains_any(query.doc_ids)
 
         if query.node_ids:
-            filter_with_node_ids = {
-                "operator": "Or",
-                "operands": [
-                    {"path": ["id"], "operator": "Equal", "valueText": node_id}
-                    for node_id in query.node_ids
-                ],
-            }
-            query_builder = query_builder.with_where(filter_with_node_ids)
+            filters = wvc.query.Filter.by_property("id").contains_any(query.node_ids)
 
-        query_builder = query_builder.with_additional(
-            ["id", "vector", "distance", "score"]
-        )
+        return_metatada = wvc.query.MetadataQuery(distance=True, score=True)
 
         vector = query.query_embedding
         similarity_key = "distance"
         if query.mode == VectorStoreQueryMode.DEFAULT:
             _logger.debug("Using vector search")
             if vector is not None:
-                query_builder = query_builder.with_near_vector(
-                    {
-                        "vector": vector,
-                    }
-                )
+                alpha = 1
         elif query.mode == VectorStoreQueryMode.HYBRID:
             _logger.debug(f"Using hybrid search with alpha {query.alpha}")
             similarity_key = "score"
             if vector is not None and query.query_str:
-                query_builder = query_builder.with_hybrid(
-                    query=query.query_str,
-                    alpha=query.alpha,
-                    vector=vector,
-                )
+                alpha = query.alpha
 
         if query.filters is not None:
-            filter = _to_weaviate_filter(query.filters)
-            query_builder = query_builder.with_where(filter)
+            filters = _to_weaviate_filter(query.filters)
         elif "filter" in kwargs and kwargs["filter"] is not None:
-            query_builder = query_builder.with_where(kwargs["filter"])
+            filters = kwargs["filter"]
 
-        query_builder = query_builder.with_limit(query.similarity_top_k)
+        limit = query.similarity_top_k
         _logger.debug(f"Using limit of {query.similarity_top_k}")
 
         # execute query
-        query_result = query_builder.do()
+        try:
+            query_result = collection.query.hybrid(
+                query=query.query_str,
+                vector=vector,
+                alpha=alpha,
+                limit=limit,
+                filters=filters,
+                return_metadata=return_metatada,
+                return_properties=all_properties,
+                include_vector=True,
+            )
+        except weaviate.exceptions.WeaviateQueryError as e:
+            raise ValueError(f"Invalid query, got errors: {e.message}")
 
         # parse results
-        parsed_result = parse_get_response(query_result)
-        entries = parsed_result[self.index_name]
+
+        entries = query_result.objects
 
         similarities = []
         nodes: List[BaseNode] = []
         node_ids = []
 
         for i, entry in enumerate(entries):
             if i < query.similarity_top_k:
-                similarities.append(get_node_similarity(entry, similarity_key))
-                nodes.append(to_node(entry, text_key=self.text_key))
+                entry_as_dict = entry.__dict__
+                similarities.append(get_node_similarity(entry_as_dict, similarity_key))
+                nodes.append(to_node(entry_as_dict, text_key=self.text_key))
                 node_ids.append(nodes[-1].node_id)
             else:
                 break
 
         return VectorStoreQueryResult(
             nodes=nodes, ids=node_ids, similarities=similarities
         )
```

### Comparing `llama_index_vector_stores_weaviate-0.1.5/llama_index/vector_stores/weaviate/utils.py` & `llama_index_vector_stores_weaviate-1.0.0/llama_index/vector_stores/weaviate/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 """
 
 import logging
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, cast
 
 if TYPE_CHECKING:
-    from weaviate import Client
+    from weaviate import WeaviateClient
+
 
 from llama_index.core.schema import BaseNode, MetadataMode, TextNode
 from llama_index.core.vector_stores.utils import (
     DEFAULT_TEXT_KEY,
     legacy_metadata_dict_to_node,
     metadata_dict_to_node,
     node_to_metadata_dict,
@@ -43,24 +44,23 @@
     },
 ]
 
 
 def validate_client(client: Any) -> None:
     """Validate client and import weaviate library."""
     try:
-        import weaviate  # noqa
-        from weaviate import Client
+        import weaviate
 
-        client = cast(Client, client)
+        client = cast(weaviate.WeaviateClient, client)
     except ImportError:
         raise ImportError(
             "Weaviate is not installed. "
             "Please install it with `pip install weaviate-client`."
         )
-    cast(Client, client)
+    cast(weaviate.WeaviateClient, client)
 
 
 def parse_get_response(response: Dict) -> Dict:
     """Parse get response from Weaviate."""
     if "errors" in response:
         raise ValueError("Invalid query, got errors: {}".format(response["errors"]))
     data_response = response["data"]
@@ -69,61 +69,58 @@
 
     return data_response["Get"]
 
 
 def class_schema_exists(client: Any, class_name: str) -> bool:
     """Check if class schema exists."""
     validate_client(client)
-    schema = client.schema.get()
-    classes = schema["classes"]
-    existing_class_names = {c["class"] for c in classes}
-    return class_name in existing_class_names
+    return client.collections.exists(class_name)
 
 
 def create_default_schema(client: Any, class_name: str) -> None:
     """Create default schema."""
     validate_client(client)
     class_schema = {
         "class": class_name,
         "description": f"Class for {class_name}",
         "properties": NODE_SCHEMA,
     }
-    client.schema.create_class(class_schema)
+    client.collections.create_from_dict(class_schema)
 
 
 def get_all_properties(client: Any, class_name: str) -> List[str]:
     """Get all properties of a class."""
     validate_client(client)
-    schema = client.schema.get()
-    classes = schema["classes"]
-    classes_by_name = {c["class"]: c for c in classes}
-    if class_name not in classes_by_name:
+    if not client.collections.exists(class_name):
         raise ValueError(f"{class_name} schema does not exist.")
-    schema = classes_by_name[class_name]
-    return [p["name"] for p in schema["properties"]]
+
+    properties = client.collections.get(class_name).config.get().properties
+    return [p.name for p in properties]
 
 
 def get_node_similarity(entry: Dict, similarity_key: str = "distance") -> float:
     """Get converted node similarity from distance."""
-    distance = entry["_additional"].get(similarity_key, 0.0)
+    distance = getattr(entry["metadata"], similarity_key)
 
     if distance is None:
         return 1.0
 
     # convert distance https://forum.weaviate.io/t/distance-vs-certainty-scores/258
     return 1.0 - float(distance)
 
 
 def to_node(entry: Dict, text_key: str = DEFAULT_TEXT_KEY) -> TextNode:
     """Convert to Node."""
-    additional = entry.pop("_additional")
-    text = entry.pop(text_key, "")
-    embedding = additional.pop("vector", None)
+    additional = entry["metadata"].__dict__
+    text = entry["properties"].pop(text_key, "")
+
+    embedding = entry["vector"].pop("default", None)
+
     try:
-        node = metadata_dict_to_node(entry)
+        node = metadata_dict_to_node(entry["properties"])
         node.text = text
         node.embedding = embedding
     except Exception as e:
         _logger.debug("Failed to parse Node metadata, fallback to legacy logic. %s", e)
         metadata, node_info, relationships = legacy_metadata_dict_to_node(entry)
 
         node = TextNode(
@@ -135,15 +132,15 @@
             relationships=relationships,
             embedding=embedding,
         )
     return node
 
 
 def add_node(
-    client: "Client",
+    client: "WeaviateClient",
     node: BaseNode,
     class_name: str,
     batch: Optional[Any] = None,
     text_key: str = DEFAULT_TEXT_KEY,
 ) -> None:
     """Add node."""
     metadata = {}
@@ -155,10 +152,14 @@
     metadata.update(additional_metadata)
 
     vector = node.get_embedding()
     id = node.node_id
 
     # if batch object is provided (via a context manager), use that instead
     if batch is not None:
-        batch.add_data_object(metadata, class_name, id, vector)
+        batch.add_object(
+            properties=metadata, collection=class_name, uuid=id, vector=vector
+        )
     else:
-        client.batch.add_data_object(metadata, class_name, id, vector)
+        client.collections.get(class_name).data.insert(
+            properties=metadata, uuid=id, vector=vector
+        )
```

### Comparing `llama_index_vector_stores_weaviate-0.1.5/pyproject.toml` & `llama_index_vector_stores_weaviate-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores weaviate integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-weaviate"
 readme = "README.md"
-version = "0.1.5"
+version = "1.0.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-weaviate-client = "^3.26.2"
+weaviate-client = "^4.5.7"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_vector_stores_weaviate-0.1.5/PKG-INFO` & `llama_index_vector_stores_weaviate-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-weaviate
-Version: 0.1.5
+Version: 1.0.0
 Summary: llama-index vector_stores weaviate integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
-Requires-Dist: weaviate-client (>=3.26.2,<4.0.0)
+Requires-Dist: weaviate-client (>=4.5.7,<5.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Vector_Stores Integration: Weaviate
```

