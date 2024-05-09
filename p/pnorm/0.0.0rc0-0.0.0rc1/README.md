# Comparing `tmp/pnorm-0.0.0rc0.tar.gz` & `tmp/pnorm-0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pnorm-0.0.0rc0.tar", max compression
+gzip compressed data, was "pnorm-0.0.0rc1.tar", max compression
```

## Comparing `pnorm-0.0.0rc0.tar` & `pnorm-0.0.0rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-02-27 03:34:43.378065 pnorm-0.0.0rc0/LICENSE
--rw-r--r--   0        0        0       24 2024-02-27 03:34:43.378065 pnorm-0.0.0rc0/README.md
--rw-r--r--   0        0        0      419 2024-02-27 03:34:43.378065 pnorm-0.0.0rc0/pnorm/__init__.py
--rw-r--r--   0        0        0     1259 2024-02-27 03:34:43.378065 pnorm-0.0.0rc0/pnorm/__main__.py
--rw-r--r--   0        0        0    11657 2024-02-27 03:34:43.382065 pnorm-0.0.0rc0/pnorm/client.py
--rw-r--r--   0        0        0     2013 2024-02-27 03:34:43.382065 pnorm-0.0.0rc0/pnorm/contexts.py
--rw-r--r--   0        0        0      338 2024-02-27 03:34:43.382065 pnorm-0.0.0rc0/pnorm/credentials.py
--rw-r--r--   0        0        0     1794 2024-02-27 03:34:43.382065 pnorm-0.0.0rc0/pnorm/cursors.py
--rw-r--r--   0        0        0      891 2024-02-27 03:34:43.382065 pnorm-0.0.0rc0/pnorm/exceptions.py
--rw-r--r--   0        0        0     5707 2024-02-27 03:34:43.382065 pnorm-0.0.0rc0/pnorm/linter.py
--rw-r--r--   0        0        0     1108 2024-02-27 03:34:43.382065 pnorm-0.0.0rc0/pnorm/mapping_utilities.py
--rw-r--r--   0        0        0     7423 2024-02-27 03:34:43.382065 pnorm-0.0.0rc0/pnorm/migrations.py
--rw-r--r--   0        0        0      179 2024-02-27 03:34:43.382065 pnorm-0.0.0rc0/pnorm/model.py
--rw-r--r--   0        0        0        0 2024-02-27 03:34:43.382065 pnorm-0.0.0rc0/pnorm/py.typed
--rw-r--r--   0        0        0      213 2024-02-27 03:34:43.382065 pnorm-0.0.0rc0/pnorm/types.py
--rw-r--r--   0        0        0      635 2024-02-27 03:34:43.382065 pnorm-0.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 pnorm-0.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/LICENSE
+-rw-r--r--   0        0        0       24 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/README.md
+-rw-r--r--   0        0        0      757 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/__init__.py
+-rw-r--r--   0        0        0     1259 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/__main__.py
+-rw-r--r--   0        0        0    11125 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/client.py
+-rw-r--r--   0        0        0     1162 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/contexts.py
+-rw-r--r--   0        0        0      338 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/credentials.py
+-rw-r--r--   0        0        0     1794 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/cursors.py
+-rw-r--r--   0        0        0      891 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/exceptions.py
+-rw-r--r--   0        0        0     5707 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/linter.py
+-rw-r--r--   0        0        0     1121 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/mapping_utilities.py
+-rw-r--r--   0        0        0     7423 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/migrations.py
+-rw-r--r--   0        0        0      179 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/model.py
+-rw-r--r--   0        0        0        0 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/py.typed
+-rw-r--r--   0        0        0      213 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pnorm/types.py
+-rw-r--r--   0        0        0      636 2024-03-05 07:52:36.275136 pnorm-0.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 pnorm-0.0.0rc1/PKG-INFO
```

### Comparing `pnorm-0.0.0rc0/LICENSE` & `pnorm-0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pnorm-0.0.0rc0/pnorm/__main__.py` & `pnorm-0.0.0rc1/pnorm/__main__.py`

 * *Files identical despite different names*

### Comparing `pnorm-0.0.0rc0/pnorm/client.py` & `pnorm-0.0.0rc1/pnorm/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 from __future__ import annotations
 
+import json
 from contextlib import contextmanager
 from typing import (
-    TYPE_CHECKING,
+    Annotated,
     Any,
     Generator,
     Optional,
     Sequence,
     Type,
+    TypeVar,
     cast,
     overload,
 )
 
 import psycopg2
 import psycopg2.extras as extras
 from psycopg2._psycopg import connection as Connection
 from psycopg2.extras import RealDictRow
-from psycopg2.sql import SQL, Composable, Composed, Identifier, Literal
-from pydantic import BaseModel
+from psycopg2.sql import Composable
+from pydantic import BaseModel, PlainSerializer
 from rcheck import r
 
 from pnorm import (
     ConnectionAlreadyEstablishedException,
     MultipleRecordsReturnedException,
     NoRecordsReturnedException,
     ParamType,
     PostgresCredentials,
     T,
     connection_not_created,
 )
 from pnorm.cursors import SingleCommitCursor, TransactionCursor
 from pnorm.mapping_utilities import combine_into_return, get_params
 
-if TYPE_CHECKING:
-    from pnorm.model import Model
+U = TypeVar("U", dict[Any, Any] | None, list[Any] | None)
+
+PostgresJSON = Annotated[
+    U,
+    PlainSerializer(json.dumps, when_used="json-unless-none"),
+]
 
 
 class PostgresClient:
     def __init__(
         self,
         credentials: PostgresCredentials,
         auto_create_connection: bool = True,  # todo: rather default to false
     ):
         self.credentials = credentials
         self.connection: Connection | None = None
         self.auto_create_connection = auto_create_connection
         self.cursor: SingleCommitCursor | TransactionCursor = SingleCommitCursor(self)
 
     def set_schema(self, schema: str):
-        schema = r.check_str("Schema", schema)
+        schema = r.check_str("schema", schema)
         self.execute("set search_path to %(search_path)s", {"search_path": schema})
 
     def get(
         self,
         return_model: Type[T],
         query: str | Composable,
         params: Optional[ParamType] = None,
@@ -94,15 +100,15 @@
 
         Examples
         --------
         >>>
         >>>
         >>>
         """
-        query = r.check_str("query", query)
+        # query = r.check_str("query", query) # OR Composable
         query_params = get_params("Query Params", params)
 
         with self._handle_auto_connection():
             with self.cursor(self.connection) as cursor:
                 cursor.execute(query, query_params)
                 query_result = cast(list[RealDictRow], cursor.fetchmany(2))
 
@@ -182,15 +188,14 @@
 
         Examples
         --------
         >>>
         >>>
         >>>
         """
-        query = r.check_str("query", query)
         query_params = get_params("Query Params", params)
         query_result: RealDictRow | BaseModel | None
 
         with self._handle_auto_connection():
             with self.cursor(self.connection) as cursor:
                 cursor.execute(query, query_params)
                 query_result = cast(RealDictRow | None, cursor.fetchone())
@@ -233,15 +238,15 @@
 
         Examples
         --------
         >>>
         >>>
         >>>
         """
-        query = r.check_str("query", query)
+        # query = r.check_str("query", query) # OR Composable
         query_params = get_params("Query Params", params)
 
         with self._handle_auto_connection():
             with self.cursor(self.connection) as cursor:
                 cursor.execute(query, query_params)
                 query_result = cast(list[RealDictRow], cursor.fetchall())
 
@@ -282,14 +287,15 @@
                 cursor.execute(query, query_params)
 
     def execute_values(
         self,
         query: str | Composable,
         values: Optional[Sequence[BaseModel]] = None,
         template: Optional[Sequence[str]] = None,
+        return_model: Optional[Type[T]] = None,
     ) -> None:
         """Execute a sql query with values
 
         [desc]
 
         Parameters
         ----------
@@ -315,14 +321,24 @@
             data = values
         else:
             data = [tuple(get_params("Query params", v).values()) for v in values]
 
         with self._handle_auto_connection():
             with self.cursor(self.connection) as cursor:
                 extras.execute_values(cursor, query, data, template)
+                
+                if return_model is None:
+                    return
+                
+                query_result = cast(list[RealDictRow], cursor.fetchall())
+
+        if len(query_result) == 0:
+            return tuple()
+
+        return tuple(combine_into_return(return_model, row) for row in query_result)
 
     def create_connection(self) -> None:
         if self.connection is not None:
             raise ConnectionAlreadyEstablishedException()
 
         self.connection = psycopg2.connect(**self.credentials.model_dump())
 
@@ -358,36 +374,7 @@
         elif self.connection is None:
             connection_not_created()
 
         yield
 
         if close_connection_after_use:
             self.close_connection()
-
-    def update_only(self, model: Model, *column_names: str):
-        for field in column_names:
-            field = r.check_str(f"column-{field}", field)
-
-            if not hasattr(model, field):
-                raise Exception()
-
-        set_fields = SQL(",").join(
-            [
-                SQL("{col_name} = {value}").format(
-                    col_name=Identifier(field_name),
-                    value=Literal(getattr(model, field_name)),
-                )
-                for field_name in column_names
-            ]
-        )
-
-        self.execute(
-            SQL(
-                "update {table_name} set {set_fields} where {id_col} = %(id_value)s"
-            ).format(
-                table_name=Identifier(model.pnorm_config.table_name),
-                # col_name=Identifier(field),
-                set_fields=set_fields,
-                id_col=Identifier(model.pnorm_config.id_column),
-            ),
-            {"id_value": getattr(model, model.pnorm_config.id_column)},
-        )
```

### Comparing `pnorm-0.0.0rc0/pnorm/contexts.py` & `pnorm-0.0.0rc1/pnorm/contexts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,16 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
-from types import TracebackType
-from typing import TYPE_CHECKING, Generator, Optional, Type
+from typing import TYPE_CHECKING, Generator, Optional
 
 if TYPE_CHECKING:
     from pnorm import PostgresClient
 
 
-# todo: rm
-class Session:
-    def __init__(self, client: PostgresClient):
-        self.client = client
-        self.original_auto_create_connection = self.client.auto_create_connection
-        self.client.auto_create_connection = False
-
-    def __enter__(self) -> PostgresClient:
-        if self.client.connection is None:
-            self.client.create_connection()
-
-        return self.client
-
-    def __exit__(
-        self,
-        exc_type: Optional[Type[Exception]],
-        exc_value: Optional[Exception],
-        exc_tb: Optional[TracebackType],
-    ):
-        if self.client.connection is not None:
-            if exc_type is not None:
-                self.client.rollback()
-
-            self.client.close_connection()
-
-        self.client.auto_create_connection = self.original_auto_create_connection
-
-
 @contextmanager
 def create_session(
     client: PostgresClient, *, schema: Optional[str] = None
 ) -> Generator[None, None, None]:
     original_auto_create_connection = client.auto_create_connection
     client.auto_create_connection = False
     close_connection_after_use = False
```

### Comparing `pnorm-0.0.0rc0/pnorm/cursors.py` & `pnorm-0.0.0rc1/pnorm/cursors.py`

 * *Files identical despite different names*

### Comparing `pnorm-0.0.0rc0/pnorm/exceptions.py` & `pnorm-0.0.0rc1/pnorm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pnorm-0.0.0rc0/pnorm/linter.py` & `pnorm-0.0.0rc1/pnorm/linter.py`

 * *Files identical despite different names*

### Comparing `pnorm-0.0.0rc0/pnorm/mapping_utilities.py` & `pnorm-0.0.0rc1/pnorm/mapping_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 def get_params(
     name: str, params: Optional[ParamType], by_alias: bool = False
 ) -> dict[str, Any]:
     if params is None:
         return {}
 
     if isinstance(params, BaseModel):
-        params = params.model_dump(by_alias=by_alias)
+        params = params.model_dump(by_alias=by_alias, mode="json")
 
     return cast(dict[str, Any], r.check_mapping(name, params, keys_of=str))
 
 
 def combine_into_return(
     return_model: Type[T],
     result: dict[str, Any] | BaseModel,
```

### Comparing `pnorm-0.0.0rc0/pnorm/migrations.py` & `pnorm-0.0.0rc1/pnorm/migrations.py`

 * *Files identical despite different names*

### Comparing `pnorm-0.0.0rc0/pyproject.toml` & `pnorm-0.0.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pnorm"
-version = "0.0.0c"
+version = "0.0.0c1"
 description = "(Postgres) Not an ORM"
 authors = ["Alex Rudolph <alex3rudolph@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/alrudolph/pnorm"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `pnorm-0.0.0rc0/PKG-INFO` & `pnorm-0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnorm
-Version: 0.0.0rc0
+Version: 0.0.0rc1
 Summary: (Postgres) Not an ORM
 Home-page: https://github.com/alrudolph/pnorm
 Author: Alex Rudolph
 Author-email: alex3rudolph@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

