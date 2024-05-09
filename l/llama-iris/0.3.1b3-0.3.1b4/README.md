# Comparing `tmp/llama_iris-0.3.1b3.tar.gz` & `tmp/llama_iris-0.3.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_iris-0.3.1b3.tar", max compression
+gzip compressed data, was "llama_iris-0.3.1b4.tar", max compression
```

## Comparing `llama_iris-0.3.1b3.tar` & `llama_iris-0.3.1b4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2024-04-16 10:57:03.085854 llama_iris-0.3.1b3/LICENSE
--rw-r--r--   0        0        0     1108 2024-04-16 10:57:03.085854 llama_iris-0.3.1b3/README.md
--rw-r--r--   0        0        0      224 2024-04-16 10:57:03.085854 llama_iris-0.3.1b3/llama_iris/__init__.py
--rw-r--r--   0        0        0    10160 2024-04-16 10:57:03.085854 llama_iris-0.3.1b3/llama_iris/vectorstore.py
--rw-r--r--   0        0        0     1060 2024-04-16 10:57:16.357998 llama_iris-0.3.1b3/pyproject.toml
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 llama_iris-0.3.1b3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-09 02:27:47.358149 llama_iris-0.3.1b4/LICENSE
+-rw-r--r--   0        0        0     1108 2024-05-09 02:27:47.358149 llama_iris-0.3.1b4/README.md
+-rw-r--r--   0        0        0      224 2024-05-09 02:27:47.358149 llama_iris-0.3.1b4/llama_iris/__init__.py
+-rw-r--r--   0        0        0    10429 2024-05-09 02:27:47.358149 llama_iris-0.3.1b4/llama_iris/vectorstore.py
+-rw-r--r--   0        0        0     1060 2024-05-09 02:28:02.278176 llama_iris-0.3.1b4/pyproject.toml
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 llama_iris-0.3.1b4/PKG-INFO
```

### Comparing `llama_iris-0.3.1b3/LICENSE` & `llama_iris-0.3.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_iris-0.3.1b3/README.md` & `llama_iris-0.3.1b4/README.md`

 * *Files identical despite different names*

### Comparing `llama_iris-0.3.1b3/llama_iris/vectorstore.py` & `llama_iris-0.3.1b4/llama_iris/vectorstore.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from llama_index.schema import BaseNode, MetadataMode
 from llama_index.vector_stores.types import (
     BasePydanticVectorStore,
     VectorStoreQuery,
     VectorStoreQueryResult,
 )
 from llama_index.vector_stores.utils import metadata_dict_to_node, node_to_metadata_dict
+from sqlalchemy.orm.session import close_all_sessions
 
 
 _logger = logging.getLogger(__name__)
 
 
 def get_data_model(
     base: Type,
@@ -56,14 +57,15 @@
 
     connection_string: str
     table_name: str
     schema_name: str
     embed_dim: int
     perform_setup: bool
     debug: bool
+    engine_args: Optional[dict]
 
     _base: Any = PrivateAttr()
     _table_class: Any = PrivateAttr()
     _engine: Any = PrivateAttr()
     _session: Any = PrivateAttr()
     _is_initialized: bool = PrivateAttr(default=False)
     _native_vector: bool = PrivateAttr(default=False)
@@ -72,32 +74,34 @@
         self,
         connection_string: str,
         table_name: str,
         schema_name: str,
         embed_dim: int = 1536,
         perform_setup: bool = True,
         debug: bool = False,
+        engine_args: Optional[dict] = None,
     ) -> None:
         table_name = table_name.lower()
         schema_name = schema_name.lower()
 
         super().__init__(
             connection_string=connection_string,
             table_name=table_name,
             schema_name=schema_name,
             embed_dim=embed_dim,
             perform_setup=perform_setup,
             debug=debug,
+            engine_args=engine_args or {},
         )
 
     async def close(self) -> None:
         if not self._is_initialized:
             return
 
-        self._session.close_all()
+        close_all_sessions()
         self._engine.dispose()
 
     @classmethod
     def class_name(cls) -> str:
         return "IRISVectorStore"
 
     @classmethod
@@ -110,40 +114,42 @@
         password: Optional[str] = None,
         table_name: str = "llamaindex",
         schema_name: str = "SQLUser",
         connection_string: Optional[str] = None,
         embed_dim: int = 1536,
         perform_setup: bool = True,
         debug: bool = False,
+        engine_args: Optional[dict] = None,
     ) -> "IRISVectorStore":
         """Return connection string from database parameters."""
         conn_str = (
             connection_string
             or f"iris://{username}:{password}@{hostname}:{port}/{namespace}"
         )
         return cls(
             connection_string=conn_str,
             table_name=table_name,
             schema_name=schema_name,
             embed_dim=embed_dim,
             perform_setup=perform_setup,
             debug=debug,
+            engine_args=engine_args,
         )
 
     @property
     def client(self) -> Any:
         if not self._is_initialized:
             return None
         return self._engine
 
     def _connect(self) -> Any:
         from sqlalchemy import create_engine
         from sqlalchemy.orm import sessionmaker
 
-        self._engine = create_engine(self.connection_string, echo=self.debug)
+        self._engine = create_engine(self.connection_string, echo=self.debug, **self.engine_args)
         self._session = sessionmaker(self._engine)
         with self._engine.connect() as conn:
             self._native_vector = conn.dialect.supports_vectors
 
             from sqlalchemy.orm import declarative_base
 
             # sqlalchemy model
```

### Comparing `llama_iris-0.3.1b3/pyproject.toml` & `llama_iris-0.3.1b4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry]
 name = "llama-iris"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-version = "0.3.1b3"
+version = "0.3.1b4"
 description = "Interface between LLMs and your data"
 authors = ["Dmitry Maslennikov <dmitry@caretdev.com>"]
 keywords = ["LLM", "NLP", "RAG", "data", "devtools", "index", "retrieval", "iris"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "llama_iris"}]
 repository = "https://github.com/caretdev/llama-iris"
```

### Comparing `llama_iris-0.3.1b3/PKG-INFO` & `llama_iris-0.3.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-iris
-Version: 0.3.1b3
+Version: 0.3.1b4
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/caretdev/llama-iris
 License: MIT
 Keywords: LLM,NLP,RAG,data,devtools,index,retrieval,iris
 Author: Dmitry Maslennikov
 Author-email: dmitry@caretdev.com
 Requires-Python: >=3.9,<4.0
```

