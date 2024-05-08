# Comparing `tmp/pypomes_db-0.5.7.tar.gz` & `tmp/pypomes_db-0.5.8.tar.gz`

## Comparing `pypomes_db-0.5.7.tar` & `pypomes_db-0.5.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38128 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    24356 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    22234 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    22282 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38244 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    24498 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    22424 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/PKG-INFO
```

### Comparing `pypomes_db-0.5.7/src/pypomes_db/__init__.py` & `pypomes_db-0.5.8/src/pypomes_db/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .db_pomes import (
     db_setup, db_get_engines, db_get_params,
     db_assert_connection, db_connect, db_exists,
     db_select_one, db_select_all, db_update,
-    db_delete, db_insert, db_bulk_insert, db_bulk_copy,
+    db_delete, db_insert, db_bulk_insert, db_bulk_migrate,
     db_migrate_lobs, db_update_lob, db_execute,
     db_call_function, db_call_procedure,
 )
 
 __all__ = [
     # db_pomes
     "db_setup", "db_get_engines", "db_get_params",
     "db_assert_connection", "db_connect", "db_exists",
     "db_select_one", "db_select_all", "db_update",
-    "db_delete", "db_insert", "db_bulk_insert", "db_bulk_copy",
+    "db_delete", "db_insert", "db_bulk_insert", "db_bulk_migrate",
     "db_migrate_lobs", "db_update_lob", "db_execute",
     "db_call_function", "db_call_procedure",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_db")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_db-0.5.7/src/pypomes_db/db_common.py` & `pypomes_db-0.5.8/src/pypomes_db/db_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
             sval: str = str(val)
         result = result.replace("?", sval, 1)
 
     return result
 
 
 def _db_log(logger: Logger,
-            err_msg: str,
+            err_msg: str = None,
             level: int = DEBUG,
             errors: list[str] = None,
             query_stmt: str = None,
             bind_vals: tuple = None) -> None:
     """
     Log *err_msg* and add it to *errors*, or else log the executed query, whichever is applicable.
```

### Comparing `pypomes_db-0.5.7/src/pypomes_db/db_pomes.py` & `pypomes_db-0.5.8/src/pypomes_db/db_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,80 +436,80 @@
                                                 insert_vals=insert_vals,
                                                 conn=conn,
                                                 logger=logger)
 
     return result
 
 
-def db_bulk_copy(errors: list[str] | None,
-                 sel_stmt: str,
-                 insert_stmt: str,
-                 target_engine: str,
-                 batch_size: int = None,
-                 where_vals: tuple = None,
-                 target_conn: Any = None,
-                 engine: str = None,
-                 conn: Any = None,
-                 logger: Logger = None) -> int:
+def db_bulk_migrate(errors: list[str] | None,
+                    sel_stmt: str,
+                    insert_stmt: str,
+                    target_engine: str,
+                    batch_size: int = None,
+                    where_vals: tuple = None,
+                    target_conn: Any = None,
+                    engine: str = None,
+                    conn: Any = None,
+                    logger: Logger = None) -> int:
     """
-    Bulk copy data from one database to another database.
+    Bulk migrate data from one database to another database.
 
     The destination database brand must be in the list of databases configured and supported by this package.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param insert_stmt: the insert statement to use for bulk-inserting
     :param target_engine: the destination database engine type
     :param batch_size: number of tuples in the batch, or 0 or None for no limit
     :param where_vals: the values to be associated with the search criteria
     :param target_conn: the connection to the destination database
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
-    :return: number of tuples effectively copied
+    :return: number of tuples effectively migrated
     """
     # initialize the return variable
     result: int | None = None
 
     curr_engine: str = _assert_engine(errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_bulk_copy(errors=errors,
-                                           sel_stmt=sel_stmt,
-                                           insert_stmt=insert_stmt,
-                                           batch_size=batch_size,
-                                           target_engine=target_engine,
-                                           where_vals=where_vals,
-                                           target_conn=target_conn,
-                                           conn=conn,
-                                           logger=logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        result = postgres_pomes.db_bulk_copy(errors=errors,
-                                             sel_stmt=sel_stmt,
-                                             insert_stmt=insert_stmt,
-                                             batch_size=batch_size,
-                                             target_engine=target_engine,
-                                             where_vals=where_vals,
-                                             target_conn=target_conn,
-                                             conn=conn,
-                                             logger=logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        result = sqlserver_pomes.db_bulk_copy(errors=errors,
+        result = oracle_pomes.db_bulk_migrate(errors=errors,
                                               sel_stmt=sel_stmt,
                                               insert_stmt=insert_stmt,
                                               batch_size=batch_size,
                                               target_engine=target_engine,
                                               where_vals=where_vals,
                                               target_conn=target_conn,
                                               conn=conn,
                                               logger=logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes.db_bulk_migrate(errors=errors,
+                                                sel_stmt=sel_stmt,
+                                                insert_stmt=insert_stmt,
+                                                batch_size=batch_size,
+                                                target_engine=target_engine,
+                                                where_vals=where_vals,
+                                                target_conn=target_conn,
+                                                conn=conn,
+                                                logger=logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.db_bulk_migrate(errors=errors,
+                                                 sel_stmt=sel_stmt,
+                                                 insert_stmt=insert_stmt,
+                                                 batch_size=batch_size,
+                                                 target_engine=target_engine,
+                                                 where_vals=where_vals,
+                                                 target_conn=target_conn,
+                                                 conn=conn,
+                                                 logger=logger)
 
     return result
 
 
 def db_migrate_lobs(errors: list[str],
                     lob_table: str,
                     lob_column: str,
```

### Comparing `pypomes_db-0.5.7/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.5.8/src/pypomes_db/oracle_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,56 +175,55 @@
             errors=errors,
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
-def db_bulk_copy(errors: list[str],
-                 sel_stmt: str,
-                 insert_stmt: str,
-                 target_engine: str,
-                 batch_size: int,
-                 where_vals: tuple,
-                 target_conn: Any,
-                 conn: Connection,
-                 logger: Logger) -> int:
+def db_bulk_migrate(errors: list[str],
+                    sel_stmt: str,
+                    insert_stmt: str,
+                    target_engine: str,
+                    batch_size: int,
+                    where_vals: tuple,
+                    target_conn: Any,
+                    conn: Connection,
+                    logger: Logger) -> int:
     """
-    Bulk copy data from a Oracle database to another database.
+    Bulk migrate data from a Oracle database to another database.
 
     The destination database brand must be in the list of databases configured and supported by this package.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param insert_stmt: the insert statement to use for bulk-inserting
     :param target_engine: the destination database engine type
     :param batch_size: number of tuples in the batch, or 0 or None for no limit
     :param where_vals: the values to be associated with the search criteria
     :param target_conn: the connection to the destination database
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
-    :return: number of tuples effectively copied
+    :return: number of tuples effectively migrated
     """
     # initialize the return variable
-    result: int | None = None
+    result: int = 0
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
         with curr_conn.cursor() as cursor:
 
             # execute the query
             cursor.execute(statement=sel_stmt,
                            parameters=where_vals)
 
             # fetch rows in batches/all rows
-            result = 0
             op_errors: list[str] = []
             rows: list[tuple]
             if batch_size:
                 rows = cursor.fetchmany(size=batch_size)
             else:
                 rows = cursor.fetchall()
             while rows:
@@ -260,14 +259,17 @@
 
     # log the results
     _db_log(logger=logger,
             err_msg=err_msg,
             errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
+    _db_log(logger=logger,
+            query_stmt=(f"{result} tuples migrated, "
+                        f"from oracle to {target_engine}"))
 
     return result
 
 
 def db_migrate_lobs(errors: list[str],
                     lob_table: str,
                     lob_column: str,
```

### Comparing `pypomes_db-0.5.7/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.5.8/src/pypomes_db/postgres_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,56 +177,55 @@
             err_msg=err_msg,
             errors=errors,
             query_stmt=insert_stmt)
 
     return result
 
 
-def db_bulk_copy(errors: list[str],
-                 sel_stmt: str,
-                 insert_stmt: str,
-                 target_engine: str,
-                 batch_size: int,
-                 where_vals: tuple,
-                 target_conn: Any,
-                 conn: connection,
-                 logger: Logger) -> int:
+def db_bulk_migrate(errors: list[str],
+                    sel_stmt: str,
+                    insert_stmt: str,
+                    target_engine: str,
+                    batch_size: int,
+                    where_vals: tuple,
+                    target_conn: Any,
+                    conn: connection,
+                    logger: Logger) -> int:
     """
-    Bulk copy data from a Postgres database to another database.
+    Bulk migrate data from a Postgres database to another database.
 
     The destination database brand must be in the list of databases configured and supported by this package.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param insert_stmt: the insert statement to use for bulk-inserting
     :param target_engine: the destination database engine type
     :param batch_size: number of tuples in the batch, or 0 or None for no limit
     :param where_vals: the values to be associated with the search criteria
     :param target_conn: the connection to the destination database
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
-    :return: number of tuples effectively copied
+    :return: number of tuples effectively migrated
     """
     # initialize the return variable
-    result: int | None = None
+    result: int = 0
 
     # make sure to have a connection
     curr_conn: connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
         with curr_conn.cursor() as cursor:
 
             # execute the query
             cursor.execute(statement=sel_stmt,
                            parameters=where_vals)
 
             # fetch rows in batches/all rows
-            result = 0
             op_errors: list[str] = []
             rows: list[tuple]
             if batch_size:
                 rows = cursor.fetchmany(batch_size)
             else:
                 rows = cursor.fetchall()
             while rows:
@@ -262,14 +261,17 @@
 
     # log the results
     _db_log(logger=logger,
             err_msg=err_msg,
             errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
+    _db_log(logger=logger,
+            query_stmt=(f"{result} tuples migrated, "
+                        f"from oracle to {target_engine}"))
 
     return result
 
 
 def db_migrate_lobs(errors: list[str],
                     lob_table: str,
                     lob_column: str,
```

### Comparing `pypomes_db-0.5.7/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.5.8/src/pypomes_db/sqlserver_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,55 +175,54 @@
             errors=errors,
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
-def db_bulk_copy(errors: list[str],
-                 sel_stmt: str,
-                 insert_stmt: str,
-                 target_engine: str,
-                 batch_size: int,
-                 where_vals: tuple,
-                 target_conn: Any,
-                 conn: Connection,
-                 logger: Logger) -> int:
+def db_bulk_migrate(errors: list[str],
+                    sel_stmt: str,
+                    insert_stmt: str,
+                    target_engine: str,
+                    batch_size: int,
+                    where_vals: tuple,
+                    target_conn: Any,
+                    conn: Connection,
+                    logger: Logger) -> int:
     """
-    Bulk copy data from a SQLServer database to another database.
+    Bulk migrate data from a SQLServer database to another database.
 
     The destination database brand must be in the list of databases configured and supported by this package.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param insert_stmt: the insert statement to use for bulk-inserting
     :param target_engine: the destination database engine type
     :param batch_size: number of tuples in the batch, or 0 or None for no limit
     :param where_vals: the values to be associated with the search criteria
     :param target_conn: the connection to the destination database
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
-    :return: number of tuples effectively copied
+    :return: number of tuples effectively migrated
     """
     # initialize the return variable
-    result: int | None = None
+    result: int = 0
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
         with curr_conn.cursor() as cursor:
 
             # execute the query
             cursor.execute(sel_stmt, where_vals)
 
             # fetch rows in batches/all rows
-            result = 0
             op_errors: list[str] = []
             rows: list[Row]
             if batch_size:
                 rows = cursor.fetchmany(batch_size)
             else:
                 rows = cursor.fetchall()
             while rows:
@@ -260,14 +259,17 @@
 
     # log the results
     _db_log(logger=logger,
             err_msg=err_msg,
             errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
+    _db_log(logger=logger,
+            query_stmt=(f"{result} tuples migrated, "
+                        f"from oracle to {target_engine}"))
 
     return result
 
 
 def db_migrate_lobs(errors: list[str],
                     lob_table: str,
                     lob_column: str,
```

### Comparing `pypomes_db-0.5.7/LICENSE` & `pypomes_db-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.7/pyproject.toml` & `pypomes_db-0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.5.7"
+version = "0.5.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.5.7/PKG-INFO` & `pypomes_db-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.5.7
+Version: 0.5.8
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

