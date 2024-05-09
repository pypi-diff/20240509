# Comparing `tmp/langchain_astradb-0.2.0.tar.gz` & `tmp/langchain_astradb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_astradb-0.2.0.tar", max compression
+gzip compressed data, was "langchain_astradb-0.3.0.tar", max compression
```

## Comparing `langchain_astradb-0.2.0.tar` & `langchain_astradb-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-04-24 09:08:50.481561 langchain_astradb-0.2.0/LICENSE
--rw-r--r--   0        0        0     2058 2024-04-24 09:08:50.481561 langchain_astradb-0.2.0/README.md
--rw-r--r--   0        0        0      529 2024-04-24 09:08:50.481561 langchain_astradb-0.2.0/langchain_astradb/__init__.py
--rw-r--r--   0        0        0    20613 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/cache.py
--rw-r--r--   0        0        0     5344 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/chat_message_histories.py
--rw-r--r--   0        0        0     4311 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/document_loaders.py
--rw-r--r--   0        0        0        0 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/py.typed
--rw-r--r--   0        0        0     8737 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/storage.py
--rw-r--r--   0        0        0    13501 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/utils/astradb.py
--rw-r--r--   0        0        0     3165 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/utils/mmr.py
--rw-r--r--   0        0        0    50645 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/vectorstores.py
--rw-r--r--   0        0        0     2692 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 langchain_astradb-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-09 13:00:38.106036 langchain_astradb-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2058 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/README.md
+-rw-r--r--   0        0        0      624 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/__init__.py
+-rw-r--r--   0        0        0    20613 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/cache.py
+-rw-r--r--   0        0        0     5344 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/chat_message_histories.py
+-rw-r--r--   0        0        0     4549 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/document_loaders.py
+-rw-r--r--   0        0        0        0 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/py.typed
+-rw-r--r--   0        0        0     8833 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/storage.py
+-rw-r--r--   0        0        0    14319 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/utils/astradb.py
+-rw-r--r--   0        0        0     3165 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/utils/mmr.py
+-rw-r--r--   0        0        0    62160 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/vectorstores.py
+-rw-r--r--   0        0        0     2692 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 langchain_astradb-0.3.0/PKG-INFO
```

### Comparing `langchain_astradb-0.2.0/LICENSE` & `langchain_astradb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.2.0/README.md` & `langchain_astradb-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.2.0/langchain_astradb/__init__.py` & `langchain_astradb-0.3.0/langchain_astradb/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from astrapy.info import CollectionVectorServiceOptions
+
 from langchain_astradb.cache import AstraDBCache, AstraDBSemanticCache
 from langchain_astradb.chat_message_histories import AstraDBChatMessageHistory
 from langchain_astradb.document_loaders import AstraDBLoader
 from langchain_astradb.storage import AstraDBByteStore, AstraDBStore
 from langchain_astradb.vectorstores import AstraDBVectorStore
 
 __all__ = [
     "AstraDBByteStore",
     "AstraDBStore",
     "AstraDBCache",
     "AstraDBSemanticCache",
     "AstraDBChatMessageHistory",
     "AstraDBLoader",
     "AstraDBVectorStore",
+    "CollectionVectorServiceOptions",
 ]
```

### Comparing `langchain_astradb-0.2.0/langchain_astradb/cache.py` & `langchain_astradb-0.3.0/langchain_astradb/cache.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.2.0/langchain_astradb/chat_message_histories.py` & `langchain_astradb-0.3.0/langchain_astradb/chat_message_histories.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.2.0/langchain_astradb/document_loaders.py` & `langchain_astradb-0.3.0/langchain_astradb/document_loaders.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,27 +19,29 @@
 from langchain_astradb.utils.astradb import (
     SetupMode,
     _AstraDBCollectionEnvironment,
 )
 
 logger = logging.getLogger(__name__)
 
+_NOT_SET = object()
+
 
 class AstraDBLoader(BaseLoader):
     def __init__(
         self,
         collection_name: str,
         *,
         token: Optional[str] = None,
         api_endpoint: Optional[str] = None,
         astra_db_client: Optional[AstraDB] = None,
         async_astra_db_client: Optional[AsyncAstraDB] = None,
         namespace: Optional[str] = None,
         filter_criteria: Optional[Dict[str, Any]] = None,
-        projection: Optional[Dict[str, Any]] = None,
+        projection: Optional[Dict[str, Any]] = _NOT_SET,  # type: ignore[assignment]
         find_options: Optional[Dict[str, Any]] = None,
         nb_prefetched: int = 1000,
         page_content_mapper: Callable[[Dict], str] = json.dumps,
         metadata_mapper: Optional[Callable[[Dict], Dict[str, Any]]] = None,
     ) -> None:
         """Load DataStax Astra DB documents.
 
@@ -51,15 +53,16 @@
             astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AstraDB' instance.
             async_astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AsyncAstraDB' instance.
             namespace: namespace (aka keyspace) where the
                 collection is. Defaults to the database's "default namespace".
             filter_criteria: Criteria to filter documents.
-            projection: Specifies the fields to return.
+            projection: Specifies the fields to return. If not provided, reads
+                fall back to the Data API default projection.
             find_options: Additional options for the query.
             nb_prefetched: Max number of documents to pre-fetch. Defaults to 1000.
             page_content_mapper: Function applied to collection documents to create
                 the `page_content` of the LangChain Document. Defaults to `json.dumps`.
         """
         astra_db_env = _AstraDBCollectionEnvironment(
             collection_name=collection_name,
@@ -68,15 +71,17 @@
             astra_db_client=astra_db_client,
             async_astra_db_client=async_astra_db_client,
             namespace=namespace,
             setup_mode=SetupMode.OFF,
         )
         self.astra_db_env = astra_db_env
         self.filter = filter_criteria
-        self.projection = projection
+        self._projection: Optional[Dict[str, Any]] = (
+            projection if projection is not _NOT_SET else {"*": True}
+        )
         self.find_options = find_options or {}
         self.nb_prefetched = nb_prefetched
         self.page_content_mapper = page_content_mapper
         self.metadata_mapper = metadata_mapper or (
             lambda _: {
                 "namespace": self.astra_db_env.astra_db.namespace,
                 "api_endpoint": self.astra_db_env.astra_db.base_url,
@@ -90,26 +95,26 @@
             metadata=self.metadata_mapper(doc),
         )
 
     def lazy_load(self) -> Iterator[Document]:
         for doc in self.astra_db_env.collection.paginated_find(
             filter=self.filter,
             options=self.find_options,
-            projection=self.projection,
+            projection=self._projection,
             sort=None,
             prefetched=self.nb_prefetched,
         ):
             yield self._to_langchain_doc(doc)
 
     async def aload(self) -> List[Document]:
         """Load data into Document objects."""
         return [doc async for doc in self.alazy_load()]
 
     async def alazy_load(self) -> AsyncIterator[Document]:
         async for doc in self.astra_db_env.async_collection.paginated_find(
             filter=self.filter,
             options=self.find_options,
-            projection=self.projection,
+            projection=self._projection,
             sort=None,
             prefetched=self.nb_prefetched,
         ):
             yield self._to_langchain_doc(doc)
```

### Comparing `langchain_astradb-0.2.0/langchain_astradb/storage.py` & `langchain_astradb-0.3.0/langchain_astradb/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,23 +53,27 @@
     @abstractmethod
     def encode_value(self, value: Optional[V]) -> Any:
         """Encodes value for Astra DB"""
 
     def mget(self, keys: Sequence[str]) -> List[Optional[V]]:
         self.astra_env.ensure_db_setup()
         docs_dict = {}
-        for doc in self.collection.paginated_find(filter={"_id": {"$in": list(keys)}}):
+        for doc in self.collection.paginated_find(
+            filter={"_id": {"$in": list(keys)}},
+            projection={"*": True},
+        ):
             docs_dict[doc["_id"]] = doc.get("value")
         return [self.decode_value(docs_dict.get(key)) for key in keys]
 
     async def amget(self, keys: Sequence[str]) -> List[Optional[V]]:
         await self.astra_env.aensure_db_setup()
         docs_dict = {}
         async for doc in self.async_collection.paginated_find(
-            filter={"_id": {"$in": list(keys)}}
+            filter={"_id": {"$in": list(keys)}},
+            projection={"*": True},
         ):
             docs_dict[doc["_id"]] = doc.get("value")
         return [self.decode_value(docs_dict.get(key)) for key in keys]
 
     def mset(self, key_value_pairs: Sequence[Tuple[str, V]]) -> None:
         self.astra_env.ensure_db_setup()
         for k, v in key_value_pairs:
```

### Comparing `langchain_astradb-0.2.0/langchain_astradb/utils/astradb.py` & `langchain_astradb-0.3.0/langchain_astradb/utils/astradb.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from asyncio import InvalidStateError, Task
 from enum import Enum
 from typing import Any, Awaitable, Dict, List, Optional, Union
 
 import langchain_core
 from astrapy.api import APIRequestError
 from astrapy.db import AstraDB, AstraDBCollection, AsyncAstraDB, AsyncAstraDBCollection
+from astrapy.info import CollectionVectorServiceOptions
 
 
 class SetupMode(Enum):
     SYNC = 1
     ASYNC = 2
     OFF = 3
 
@@ -90,14 +91,17 @@
         namespace: Optional[str] = None,
         setup_mode: SetupMode = SetupMode.SYNC,
         pre_delete_collection: bool = False,
         embedding_dimension: Union[int, Awaitable[int], None] = None,
         metric: Optional[str] = None,
         requested_indexing_policy: Optional[Dict[str, Any]] = None,
         default_indexing_policy: Optional[Dict[str, Any]] = None,
+        collection_vector_service_options: Optional[
+            CollectionVectorServiceOptions
+        ] = None,
     ) -> None:
         super().__init__(
             token, api_endpoint, astra_db_client, async_astra_db_client, namespace
         )
         self.collection_name = collection_name
         self.collection = AstraDBCollection(
             collection_name=collection_name,
@@ -122,20 +126,26 @@
                 if pre_delete_collection:
                     await async_astra_db.delete_collection(collection_name)
                 if inspect.isawaitable(embedding_dimension):
                     dimension = await embedding_dimension
                 else:
                     dimension = embedding_dimension
 
+                # Used for enabling $vectorize on the collection
+                service_dict: Optional[Dict[str, Any]] = None
+                if collection_vector_service_options is not None:
+                    service_dict = collection_vector_service_options.as_dict()
+
                 try:
                     await async_astra_db.create_collection(
                         collection_name,
                         dimension=dimension,
                         metric=metric,
                         options=_options,
+                        service_dict=service_dict,
                     )
                 except (APIRequestError, ValueError):
                     # possibly the collection is preexisting and may have legacy,
                     # or custom, indexing settings: verify
                     get_coll_response = await async_astra_db.get_collections(
                         options={"explain": True}
                     )
@@ -157,20 +167,26 @@
                 self.astra_db.delete_collection(collection_name)
             if inspect.isawaitable(embedding_dimension):
                 raise ValueError(
                     "Cannot use an awaitable embedding_dimension with async_setup "
                     "set to False"
                 )
             else:
+                # Used for enabling $vectorize on the collection
+                service_dict: Optional[Dict[str, Any]] = None
+                if collection_vector_service_options is not None:
+                    service_dict = collection_vector_service_options.as_dict()
+
                 try:
                     self.astra_db.create_collection(
                         collection_name,
                         dimension=embedding_dimension,  # type: ignore[arg-type]
                         metric=metric,
                         options=_options,
+                        service_dict=service_dict,
                     )
                 except (APIRequestError, ValueError):
                     # possibly the collection is preexisting and may have legacy,
                     # or custom, indexing settings: verify
                     get_coll_response = self.astra_db.get_collections(  # type: ignore[union-attr]
                         options={"explain": True}
                     )
```

### Comparing `langchain_astradb-0.2.0/langchain_astradb/utils/mmr.py` & `langchain_astradb-0.3.0/langchain_astradb/utils/mmr.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.2.0/langchain_astradb/vectorstores.py` & `langchain_astradb-0.3.0/langchain_astradb/vectorstores.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import numpy as np
 from astrapy.db import (
     AstraDB as AstraDBClient,
 )
 from astrapy.db import (
     AsyncAstraDB as AsyncAstraDBClient,
 )
+from astrapy.info import CollectionVectorServiceOptions
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.runnables.utils import gather_with_concurrency
 from langchain_core.utils.iter import batch_iterate
 from langchain_core.vectorstores import VectorStore
 
 from langchain_astradb.utils.astradb import (
@@ -131,16 +132,16 @@
                 " `metadata_indexing_exclude` and `collection_indexing_policy`"
                 " can be specified as non null."
             )
 
     def __init__(
         self,
         *,
-        embedding: Embeddings,
         collection_name: str,
+        embedding: Optional[Embeddings] = None,
         token: Optional[str] = None,
         api_endpoint: Optional[str] = None,
         astra_db_client: Optional[AstraDBClient] = None,
         async_astra_db_client: Optional[AsyncAstraDBClient] = None,
         namespace: Optional[str] = None,
         metric: Optional[str] = None,
         batch_size: Optional[int] = None,
@@ -148,14 +149,17 @@
         bulk_insert_overwrite_concurrency: Optional[int] = None,
         bulk_delete_concurrency: Optional[int] = None,
         setup_mode: SetupMode = SetupMode.SYNC,
         pre_delete_collection: bool = False,
         metadata_indexing_include: Optional[Iterable[str]] = None,
         metadata_indexing_exclude: Optional[Iterable[str]] = None,
         collection_indexing_policy: Optional[Dict[str, Any]] = None,
+        collection_vector_service_options: Optional[
+            CollectionVectorServiceOptions
+        ] = None,
     ) -> None:
         """Wrapper around DataStax Astra DB for vector-store workloads.
 
         For quickstart and details, visit
         https://docs.datastax.com/en/astra/astra-db-vector/
 
         Example:
@@ -171,15 +175,18 @@
                     api_endpoint="https://<DB-ID>-<REGION>.apps.astra.datastax.com"
                 )
 
                 vectorstore.add_texts(["Giraffes", "All good here"])
                 results = vectorstore.similarity_search("Everything's ok", k=1)
 
         Args:
-            embedding: embedding function to use.
+            embedding: the embeddings function or service to use.
+                This enables client-side embedding functions or calls to external
+                embedding providers. Only one of `embedding` or
+                `collection_vector_service_options` can be provided.
             collection_name: name of the Astra DB collection to create/use.
             token: API token for Astra DB usage.
             api_endpoint: full URL to the API endpoint, such as
                 `https://<DB-ID>-us-east1.apps.astra.datastax.com`.
             astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AstraDB' instance.
             async_astra_db_client: *alternative to token+api_endpoint*,
@@ -205,14 +212,19 @@
             metadata_indexing_exclude: a denylist of the specific metadata subfields
                 that should not be indexed for later filtering in searches.
             collection_indexing_policy: a full "indexing" specification for
                 what fields should be indexed for later filtering in searches.
                 This dict must conform to to the API specifications
                 (see docs.datastax.com/en/astra/astra-db-vector/api-reference/
                 data-api-commands.html#advanced-feature-indexing-clause-on-createcollection)
+            collection_vector_service_options: specifies the use of server-side
+                embeddings within Astra DB. Only one of `embedding` or
+                `collection_vector_service_options` can be provided.
+                NOTE: This feature is under current development.
+
 
         Note:
             For concurrency in synchronous :meth:`~add_texts`:, as a rule of thumb, on a
             typical client machine it is suggested to keep the quantity
             bulk_insert_batch_concurrency * bulk_insert_overwrite_concurrency
             much below 1000 to avoid exhausting the client multithreading/networking
             resources. The hardcoded defaults are somewhat conservative to meet
@@ -223,20 +235,35 @@
 
             A bit of experimentation is required to nail the best results here,
             depending on both the machine/network specs and the expected workload
             (specifically, how often a write is an update of an existing id).
             Remember you can pass concurrency settings to individual calls to
             :meth:`~add_texts` and :meth:`~add_documents` as well.
         """
+        # Embedding and collection_vector_service_options are mutually exclusive,
+        # as both specify how to produce embeddings
+        if embedding is None and collection_vector_service_options is None:
+            raise ValueError(
+                "Either an `embedding` or a `collection_vector_service_options`\
+                    must be provided."
+            )
+
+        if embedding is not None and collection_vector_service_options is not None:
+            raise ValueError(
+                "Only one of `embedding` or `collection_vector_service_options`\
+                    can be provided."
+            )
+
         self.embedding_dimension: Optional[int] = None
         self.embedding = embedding
         self.collection_name = collection_name
         self.token = token
         self.api_endpoint = api_endpoint
         self.namespace = namespace
+        self.collection_vector_service_options = collection_vector_service_options
         # Concurrency settings
         self.batch_size: int = batch_size or DEFAULT_BATCH_SIZE
         self.bulk_insert_batch_concurrency: int = (
             bulk_insert_batch_concurrency or DEFAULT_BULK_INSERT_BATCH_CONCURRENCY
         )
         self.bulk_insert_overwrite_concurrency: int = (
             bulk_insert_overwrite_concurrency
@@ -244,18 +271,19 @@
         )
         self.bulk_delete_concurrency: int = (
             bulk_delete_concurrency or DEFAULT_BULK_DELETE_CONCURRENCY
         )
         # "vector-related" settings
         self.metric = metric
         embedding_dimension: Union[int, Awaitable[int], None] = None
-        if setup_mode == SetupMode.ASYNC:
-            embedding_dimension = self._aget_embedding_dimension()
-        elif setup_mode == SetupMode.SYNC or setup_mode == SetupMode.OFF:
-            embedding_dimension = self._get_embedding_dimension()
+        if self.embedding is not None:
+            if setup_mode == SetupMode.ASYNC:
+                embedding_dimension = self._aget_embedding_dimension()
+            elif setup_mode == SetupMode.SYNC or setup_mode == SetupMode.OFF:
+                embedding_dimension = self._get_embedding_dimension()
 
         # indexing policy setting
         self.indexing_policy: Dict[str, Any] = self._normalize_metadata_indexing_policy(
             metadata_indexing_include=metadata_indexing_include,
             metadata_indexing_exclude=metadata_indexing_exclude,
             collection_indexing_policy=collection_indexing_policy,
         )
@@ -269,38 +297,51 @@
             namespace=namespace,
             setup_mode=setup_mode,
             pre_delete_collection=pre_delete_collection,
             embedding_dimension=embedding_dimension,
             metric=metric,
             requested_indexing_policy=self.indexing_policy,
             default_indexing_policy=DEFAULT_INDEXING_OPTIONS,
+            collection_vector_service_options=collection_vector_service_options,
         )
         self.astra_db = self.astra_env.astra_db
         self.async_astra_db = self.astra_env.async_astra_db
         self.collection = self.astra_env.collection
         self.async_collection = self.astra_env.async_collection
 
     def _get_embedding_dimension(self) -> int:
+        assert self.embedding is not None
+
         if self.embedding_dimension is None:
             self.embedding_dimension = len(
                 self.embedding.embed_query(text="This is a sample sentence.")
             )
         return self.embedding_dimension
 
     async def _aget_embedding_dimension(self) -> int:
+        assert self.embedding is not None
+
         if self.embedding_dimension is None:
             self.embedding_dimension = len(
                 await self.embedding.aembed_query(text="This is a sample sentence.")
             )
         return self.embedding_dimension
 
     @property
-    def embeddings(self) -> Embeddings:
+    def embeddings(self) -> Optional[Embeddings]:
+        """
+        Accesses the supplied embeddings object. If using server-side embeddings,
+        this will return None.
+        """
         return self.embedding
 
+    def _using_vectorize(self) -> bool:
+        """Indicates whether server-side embeddings are being used."""
+        return self.collection_vector_service_options is not None
+
     def _select_relevance_score_fn(self) -> Callable[[float], float]:
         """
         The underlying API calls already returns a "score proper",
         i.e. one in [0, 1] where higher means more *similar*,
         so here the final score transformation is not reversing the interval:
         """
         return lambda score: score
@@ -471,14 +512,44 @@
         uniqued_documents_to_insert = _unique_list(
             documents_to_insert[::-1],
             lambda document: document["_id"],
         )[::-1]
         return uniqued_documents_to_insert
 
     @staticmethod
+    def _get_vectorize_documents_to_insert(
+        texts: Iterable[str],
+        metadatas: Optional[List[dict]] = None,
+        ids: Optional[List[str]] = None,
+    ) -> List[DocDict]:
+        if ids is None:
+            ids = [uuid.uuid4().hex for _ in texts]
+        if metadatas is None:
+            metadatas = [{} for _ in texts]
+        #
+        documents_to_insert = [
+            {
+                "_id": b_id,
+                "$vectorize": b_txt,
+                "metadata": b_md,
+            }
+            for b_txt, b_id, b_md in zip(
+                texts,
+                ids,
+                metadatas,
+            )
+        ]
+        # make unique by id, keeping the last
+        uniqued_documents_to_insert = _unique_list(
+            documents_to_insert[::-1],
+            lambda document: document["_id"],
+        )[::-1]
+        return uniqued_documents_to_insert
+
+    @staticmethod
     def _get_missing_from_batch(
         document_batch: List[DocDict], insert_result: Dict[str, Any]
     ) -> Tuple[List[str], List[DocDict]]:
         if "status" not in insert_result:
             raise ValueError(
                 f"API Exception while running bulk insertion: {str(insert_result)}"
             )
@@ -551,18 +622,24 @@
             warnings.warn(
                 "Method 'add_texts' of AstraDBVectorStore vector store invoked with "
                 f"unsupported arguments ({', '.join(sorted(kwargs.keys()))}), "
                 "which will be ignored."
             )
         self.astra_env.ensure_db_setup()
 
-        embedding_vectors = self.embedding.embed_documents(list(texts))
-        documents_to_insert = self._get_documents_to_insert(
-            texts, embedding_vectors, metadatas, ids
-        )
+        if self._using_vectorize():
+            documents_to_insert = self._get_vectorize_documents_to_insert(
+                texts, metadatas, ids
+            )
+        else:
+            assert self.embedding is not None
+            embedding_vectors = self.embedding.embed_documents(list(texts))
+            documents_to_insert = self._get_documents_to_insert(
+                texts, embedding_vectors, metadatas, ids
+            )
 
         def _handle_batch(document_batch: List[DocDict]) -> List[str]:
             # self.collection is not None (by _ensure_astra_db_client)
             im_result = self.collection.insert_many(  # type: ignore[union-attr]
                 documents=document_batch,
                 options={"ordered": False},
                 partial_failures_allowed=True,
@@ -647,18 +724,25 @@
             warnings.warn(
                 "Method 'aadd_texts' of AstraDBVectorStore invoked with "
                 f"unsupported arguments ({', '.join(sorted(kwargs.keys()))}), "
                 "which will be ignored."
             )
         await self.astra_env.aensure_db_setup()
 
-        embedding_vectors = await self.embedding.aembed_documents(list(texts))
-        documents_to_insert = self._get_documents_to_insert(
-            texts, embedding_vectors, metadatas, ids
-        )
+        if self._using_vectorize():
+            # using server-side embeddings
+            documents_to_insert = self._get_vectorize_documents_to_insert(
+                texts, metadatas, ids
+            )
+        else:
+            assert self.embedding is not None
+            embedding_vectors = await self.embedding.aembed_documents(list(texts))
+            documents_to_insert = self._get_documents_to_insert(
+                texts, embedding_vectors, metadatas, ids
+            )
 
         async def _handle_batch(document_batch: List[DocDict]) -> List[str]:
             # self.async_collection is not None here for sure
             im_result = await self.async_collection.insert_many(
                 documents=document_batch,
                 options={"ordered": False},
                 partial_failures_allowed=True,
@@ -779,14 +863,89 @@
                     "_id": 1,
                     "content": 1,
                     "metadata": 1,
                 },
             )
         ]
 
+    def _similarity_search_with_score_id_with_vectorize(
+        self,
+        query: str,
+        k: int = 4,
+        filter: Optional[Dict[str, Any]] = None,
+    ) -> List[Tuple[Document, float, str]]:
+        """Return docs most similar to the query with score and id using $vectorize.
+
+        This is only available when using server-side embeddings.
+        """
+        self.astra_env.ensure_db_setup()
+        metadata_parameter = self._filter_to_metadata(filter)
+        #
+        hits = list(
+            # self.collection is not None (by _ensure_astra_db_client)
+            self.collection.paginated_find(  # type: ignore[union-attr]
+                filter=metadata_parameter,
+                sort={"$vectorize": query},
+                options={"limit": k, "includeSimilarity": True},
+                projection={
+                    "_id": 1,
+                    "$vectorize": 1,
+                    "metadata": 1,
+                },
+            )
+        )
+        #
+        return [
+            (
+                Document(
+                    # text content is stored in $vectorize instead of content
+                    page_content=hit["$vectorize"],
+                    metadata=hit["metadata"],
+                ),
+                hit["$similarity"],
+                hit["_id"],
+            )
+            for hit in hits
+        ]
+
+    async def _asimilarity_search_with_score_id_with_vectorize(
+        self,
+        query: str,
+        k: int = 4,
+        filter: Optional[Dict[str, Any]] = None,
+    ) -> List[Tuple[Document, float, str]]:
+        """Return docs most similar to the query with score and id using $vectorize.
+
+        This is only available when using server-side embeddings.
+        """
+        await self.astra_env.aensure_db_setup()
+        metadata_parameter = self._filter_to_metadata(filter)
+        #
+        return [
+            (
+                Document(
+                    # text content is stored in $vectorize instead of content
+                    page_content=hit["$vectorize"],
+                    metadata=hit["metadata"],
+                ),
+                hit["$similarity"],
+                hit["_id"],
+            )
+            async for hit in self.async_collection.paginated_find(
+                filter=metadata_parameter,
+                sort={"$vectorize": query},
+                options={"limit": k, "includeSimilarity": True},
+                projection={
+                    "_id": 1,
+                    "$vectorize": 1,
+                    "metadata": 1,
+                },
+            )
+        ]
+
     def similarity_search_with_score_id(
         self,
         query: str,
         k: int = 4,
         filter: Optional[Dict[str, Any]] = None,
     ) -> List[Tuple[Document, float, str]]:
         """Return docs most similar to the query with score and id.
@@ -795,20 +954,29 @@
             query: Query to look up documents similar to.
             k: Number of Documents to return. Defaults to 4.
             filter: Filter on the metadata to apply.
 
         Returns:
             The list of (Document, score, id), the most similar to the query.
         """
-        embedding_vector = self.embedding.embed_query(query)
-        return self.similarity_search_with_score_id_by_vector(
-            embedding=embedding_vector,
-            k=k,
-            filter=filter,
-        )
+
+        if self._using_vectorize():
+            return self._similarity_search_with_score_id_with_vectorize(
+                query=query,
+                k=k,
+                filter=filter,
+            )
+        else:
+            assert self.embedding is not None
+            embedding_vector = self.embedding.embed_query(query)
+            return self.similarity_search_with_score_id_by_vector(
+                embedding=embedding_vector,
+                k=k,
+                filter=filter,
+            )
 
     async def asimilarity_search_with_score_id(
         self,
         query: str,
         k: int = 4,
         filter: Optional[Dict[str, Any]] = None,
     ) -> List[Tuple[Document, float, str]]:
@@ -818,20 +986,28 @@
             query: Query to look up documents similar to.
             k: Number of Documents to return. Defaults to 4.
             filter: Filter on the metadata to apply.
 
         Returns:
             The list of (Document, score, id), the most similar to the query.
         """
-        embedding_vector = await self.embedding.aembed_query(query)
-        return await self.asimilarity_search_with_score_id_by_vector(
-            embedding=embedding_vector,
-            k=k,
-            filter=filter,
-        )
+        if self._using_vectorize():
+            return await self._asimilarity_search_with_score_id_with_vectorize(
+                query=query,
+                k=k,
+                filter=filter,
+            )
+        else:
+            assert self.embedding is not None
+            embedding_vector = await self.embedding.aembed_query(query)
+            return await self.asimilarity_search_with_score_id_by_vector(
+                embedding=embedding_vector,
+                k=k,
+                filter=filter,
+            )
 
     def similarity_search_with_score_by_vector(
         self,
         embedding: List[float],
         k: int = 4,
         filter: Optional[Dict[str, Any]] = None,
     ) -> List[Tuple[Document, float]]:
@@ -896,20 +1072,31 @@
             query: Query to look up documents similar to.
             k: Number of Documents to return. Defaults to 4.
             filter: Filter on the metadata to apply.
 
         Returns:
             The list of Documents most similar to the query.
         """
-        embedding_vector = self.embedding.embed_query(query)
-        return self.similarity_search_by_vector(
-            embedding_vector,
-            k,
-            filter=filter,
-        )
+        if self._using_vectorize():
+            return [
+                doc
+                for (doc, _, _) in self._similarity_search_with_score_id_with_vectorize(
+                    query,
+                    k,
+                    filter=filter,
+                )
+            ]
+        else:
+            assert self.embedding is not None
+            embedding_vector = self.embedding.embed_query(query)
+            return self.similarity_search_by_vector(
+                embedding_vector,
+                k,
+                filter=filter,
+            )
 
     async def asimilarity_search(
         self,
         query: str,
         k: int = 4,
         filter: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
@@ -920,20 +1107,35 @@
             query: Query to look up documents similar to.
             k: Number of Documents to return. Defaults to 4.
             filter: Filter on the metadata to apply.
 
         Returns:
             The list of Documents most similar to the query.
         """
-        embedding_vector = await self.embedding.aembed_query(query)
-        return await self.asimilarity_search_by_vector(
-            embedding_vector,
-            k,
-            filter=filter,
-        )
+        if self._using_vectorize():
+            return [
+                doc
+                for (
+                    doc,
+                    _,
+                    _,
+                ) in await self._asimilarity_search_with_score_id_with_vectorize(
+                    query,
+                    k,
+                    filter=filter,
+                )
+            ]
+        else:
+            assert self.embedding is not None
+            embedding_vector = await self.embedding.aembed_query(query)
+            return await self.asimilarity_search_by_vector(
+                embedding_vector,
+                k,
+                filter=filter,
+            )
 
     def similarity_search_by_vector(
         self,
         embedding: List[float],
         k: int = 4,
         filter: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
@@ -995,20 +1197,35 @@
             query: Query to look up documents similar to.
             k: Number of Documents to return. Defaults to 4.
             filter: Filter on the metadata to apply.
 
         Returns:
             The list of (Document, score), the most similar to the query vector.
         """
-        embedding_vector = self.embedding.embed_query(query)
-        return self.similarity_search_with_score_by_vector(
-            embedding_vector,
-            k,
-            filter=filter,
-        )
+        if self._using_vectorize():
+            return [
+                (doc, score)
+                for (
+                    doc,
+                    score,
+                    doc_id,
+                ) in self._similarity_search_with_score_id_with_vectorize(
+                    query=query,
+                    k=k,
+                    filter=filter,
+                )
+            ]
+        else:
+            assert self.embedding is not None
+            embedding_vector = self.embedding.embed_query(query)
+            return self.similarity_search_with_score_by_vector(
+                embedding_vector,
+                k,
+                filter=filter,
+            )
 
     async def asimilarity_search_with_score(
         self,
         query: str,
         k: int = 4,
         filter: Optional[Dict[str, Any]] = None,
     ) -> List[Tuple[Document, float]]:
@@ -1018,20 +1235,35 @@
             query: Query to look up documents similar to.
             k: Number of Documents to return. Defaults to 4.
             filter: Filter on the metadata to apply.
 
         Returns:
             The list of (Document, score), the most similar to the query vector.
         """
-        embedding_vector = await self.embedding.aembed_query(query)
-        return await self.asimilarity_search_with_score_by_vector(
-            embedding_vector,
-            k,
-            filter=filter,
-        )
+        if self._using_vectorize():
+            return [
+                (doc, score)
+                for (
+                    doc,
+                    score,
+                    doc_id,
+                ) in await self._asimilarity_search_with_score_id_with_vectorize(
+                    query=query,
+                    k=k,
+                    filter=filter,
+                )
+            ]
+        else:
+            assert self.embedding is not None
+            embedding_vector = await self.embedding.aembed_query(query)
+            return await self.asimilarity_search_with_score_by_vector(
+                embedding_vector,
+                k,
+                filter=filter,
+            )
 
     @staticmethod
     def _get_mmr_hits(
         embedding: List[float], k: int, lambda_mult: float, prefetch_hits: List[DocDict]
     ) -> List[Document]:
         mmr_chosen_indices = maximal_marginal_relevance(
             np.array(embedding, dtype=np.float32),
@@ -1166,22 +1398,26 @@
                 of diversity among the results with 0 corresponding
                 to maximum diversity and 1 to minimum diversity.
             filter: Filter on the metadata to apply.
 
         Returns:
             The list of Documents selected by maximal marginal relevance.
         """
-        embedding_vector = self.embedding.embed_query(query)
-        return self.max_marginal_relevance_search_by_vector(
-            embedding_vector,
-            k,
-            fetch_k,
-            lambda_mult=lambda_mult,
-            filter=filter,
-        )
+        if self._using_vectorize():
+            raise ValueError("MMR search is unsupported for server-side embeddings.")
+        else:
+            assert self.embedding is not None
+            embedding_vector = self.embedding.embed_query(query)
+            return self.max_marginal_relevance_search_by_vector(
+                embedding_vector,
+                k,
+                fetch_k,
+                lambda_mult=lambda_mult,
+                filter=filter,
+            )
 
     async def amax_marginal_relevance_search(
         self,
         query: str,
         k: int = 4,
         fetch_k: int = 20,
         lambda_mult: float = 0.5,
@@ -1201,27 +1437,34 @@
                 of diversity among the results with 0 corresponding
                 to maximum diversity and 1 to minimum diversity.
             filter: Filter on the metadata to apply.
 
         Returns:
             The list of Documents selected by maximal marginal relevance.
         """
-        embedding_vector = await self.embedding.aembed_query(query)
-        return await self.amax_marginal_relevance_search_by_vector(
-            embedding_vector,
-            k,
-            fetch_k,
-            lambda_mult=lambda_mult,
-            filter=filter,
-        )
+        if self._using_vectorize():
+            raise ValueError("MMR search is unsupported for server-side embeddings.")
+        else:
+            assert self.embedding is not None
+            embedding_vector = await self.embedding.aembed_query(query)
+            return await self.amax_marginal_relevance_search_by_vector(
+                embedding_vector,
+                k,
+                fetch_k,
+                lambda_mult=lambda_mult,
+                filter=filter,
+            )
 
     @classmethod
     def _from_kwargs(
         cls: Type[AstraDBVectorStore],
-        embedding: Embeddings,
+        embedding: Optional[Embeddings] = None,
+        collection_vector_service_options: Optional[
+            CollectionVectorServiceOptions
+        ] = None,
         **kwargs: Any,
     ) -> AstraDBVectorStore:
         known_kwargs = {
             "collection_name",
             "token",
             "api_endpoint",
             "astra_db_client",
@@ -1264,97 +1507,162 @@
             metric=metric,
             batch_size=kwargs.get("batch_size"),
             bulk_insert_batch_concurrency=kwargs.get("bulk_insert_batch_concurrency"),
             bulk_insert_overwrite_concurrency=kwargs.get(
                 "bulk_insert_overwrite_concurrency"
             ),
             bulk_delete_concurrency=kwargs.get("bulk_delete_concurrency"),
+            collection_vector_service_options=collection_vector_service_options,
         )
 
     @classmethod
     def from_texts(
         cls: Type[AstraDBVectorStore],
         texts: List[str],
-        embedding: Embeddings,
+        embedding: Optional[Embeddings] = None,
         metadatas: Optional[List[dict]] = None,
         ids: Optional[List[str]] = None,
+        collection_vector_service_options: Optional[
+            CollectionVectorServiceOptions
+        ] = None,
         **kwargs: Any,
     ) -> AstraDBVectorStore:
         """Create an Astra DB vectorstore from raw texts.
 
         Args:
             texts: the texts to insert.
             embedding: the embedding function to use in the store.
+                This enables client-side embedding functions or calls to external
+                embedding providers. Only one of `embedding` or
+                `collection_vector_service_options` can be provided.
             metadatas: metadata dicts for the texts.
             ids: ids to associate to the texts.
+            collection_vector_service_options: specifies the use of server-side
+                embeddings within Astra DB. Only one of `embedding` or
+                `collection_vector_service_options` can be provided.
             **kwargs: you can pass any argument that you would
                 to :meth:`~add_texts` and/or to the 'AstraDBVectorStore' constructor
                 (see these methods for details). These arguments will be
                 routed to the respective methods as they are.
 
         Returns:
             an `AstraDBVectorStore` vectorstore.
         """
-        astra_db_store = AstraDBVectorStore._from_kwargs(embedding, **kwargs)
+        astra_db_store = AstraDBVectorStore._from_kwargs(
+            embedding=embedding,
+            collection_vector_service_options=collection_vector_service_options,
+            **kwargs,
+        )
         astra_db_store.add_texts(
             texts=texts,
             metadatas=metadatas,
             ids=ids,
             batch_size=kwargs.get("batch_size"),
             batch_concurrency=kwargs.get("batch_concurrency"),
             overwrite_concurrency=kwargs.get("overwrite_concurrency"),
         )
         return astra_db_store
 
     @classmethod
     async def afrom_texts(
         cls: Type[AstraDBVectorStore],
         texts: List[str],
-        embedding: Embeddings,
+        embedding: Optional[Embeddings] = None,
         metadatas: Optional[List[dict]] = None,
         ids: Optional[List[str]] = None,
+        collection_vector_service_options: Optional[
+            CollectionVectorServiceOptions
+        ] = None,
         **kwargs: Any,
     ) -> AstraDBVectorStore:
         """Create an Astra DB vectorstore from raw texts.
 
         Args:
             texts: the texts to insert.
             embedding: the embedding function to use in the store.
             metadatas: metadata dicts for the texts.
             ids: ids to associate to the texts.
+            collection_vector_service_options: specifies the use of server-side
+                embeddings within Astra DB. Only one of `embedding` or
+                `collection_vector_service_options` can be provided.
             **kwargs: you can pass any argument that you would
                 to :meth:`~add_texts` and/or to the 'AstraDBVectorStore' constructor
                 (see these methods for details). These arguments will be
                 routed to the respective methods as they are.
 
         Returns:
             an `AstraDBVectorStore` vectorstore.
         """
-        astra_db_store = AstraDBVectorStore._from_kwargs(embedding, **kwargs)
+        astra_db_store = AstraDBVectorStore._from_kwargs(
+            embedding,
+            collection_vector_service_options=collection_vector_service_options,
+            **kwargs,
+        )
         await astra_db_store.aadd_texts(
             texts=texts,
             metadatas=metadatas,
             ids=ids,
             batch_size=kwargs.get("batch_size"),
             batch_concurrency=kwargs.get("batch_concurrency"),
             overwrite_concurrency=kwargs.get("overwrite_concurrency"),
         )
         return astra_db_store
 
     @classmethod
     def from_documents(
         cls: Type[AstraDBVectorStore],
         documents: List[Document],
-        embedding: Embeddings,
+        embedding: Optional[Embeddings] = None,
+        collection_vector_service_options: Optional[
+            CollectionVectorServiceOptions
+        ] = None,
         **kwargs: Any,
     ) -> AstraDBVectorStore:
         """Create an Astra DB vectorstore from a document list.
 
         Utility method that defers to 'from_texts' (see that one).
 
         Args: see 'from_texts', except here you have to supply 'documents'
             in place of 'texts' and 'metadatas'.
 
         Returns:
             an `AstraDBVectorStore` vectorstore.
         """
-        return super().from_documents(documents, embedding, **kwargs)
+        texts = [d.page_content for d in documents]
+        metadatas = [d.metadata for d in documents]
+        return cls.from_texts(
+            texts,
+            embedding=embedding,
+            metadatas=metadatas,
+            collection_vector_service_options=collection_vector_service_options,
+            **kwargs,
+        )
+
+    @classmethod
+    async def afrom_documents(
+        cls: Type[AstraDBVectorStore],
+        documents: List[Document],
+        embedding: Optional[Embeddings] = None,
+        collection_vector_service_options: Optional[
+            CollectionVectorServiceOptions
+        ] = None,
+        **kwargs: Any,
+    ) -> AstraDBVectorStore:
+        """Create an Astra DB vectorstore from a document list.
+
+        Utility method that defers to 'afrom_texts' (see that one).
+
+        Args: see 'afrom_texts', except here you have to supply 'documents'
+            in place of 'texts' and 'metadatas'.
+
+        Returns:
+            an `AstraDBVectorStore` vectorstore.
+        """
+        texts = [d.page_content for d in documents]
+        metadatas = [d.metadata for d in documents]
+        return await cls.afrom_texts(
+            texts,
+            embedding=embedding,
+            metadatas=metadatas,
+            collection_vector_service_options=collection_vector_service_options,
+            **kwargs,
+        )
```

### Comparing `langchain_astradb-0.2.0/pyproject.toml` & `langchain_astradb-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-astradb"
-version = "0.2.0"
+version = "0.3.0"
 description = "An integration package connecting Astra DB and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-datastax"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_astradb-0.2.0/PKG-INFO` & `langchain_astradb-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-astradb
-Version: 0.2.0
+Version: 0.3.0
 Summary: An integration package connecting Astra DB and LangChain
 Home-page: https://github.com/langchain-ai/langchain-datastax
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

