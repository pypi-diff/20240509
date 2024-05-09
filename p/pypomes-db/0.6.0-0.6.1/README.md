# Comparing `tmp/pypomes_db-0.6.0.tar.gz` & `tmp/pypomes_db-0.6.1.tar.gz`

## Comparing `pypomes_db-0.6.0.tar` & `pypomes_db-0.6.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38244 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    24795 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    24090 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    22735 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38244 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    24638 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    23999 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    22578 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/PKG-INFO
```

### Comparing `pypomes_db-0.6.0/src/pypomes_db/__init__.py` & `pypomes_db-0.6.1/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.0/src/pypomes_db/db_common.py` & `pypomes_db-0.6.1/src/pypomes_db/db_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from __future__ import annotations
+import uuid
 from logging import DEBUG, Logger
+from tempfile import gettempdir
+from pathlib import Path
 from pypomes_core import (
     APP_PREFIX,
     env_get_int, env_get_str, str_sanitize, str_get_positional
 )
 
 # the preferred way to specify database connection parameters is dynamically with 'db_setup_params'
 # specifying database connection parameters with environment variables can be done in two ways:
@@ -75,25 +77,25 @@
     else:
         err_msg = f"Database engine '{engine}' unknown or not configured"
         errors.append(err_msg)
 
     return result
 
 
-def _assert_query_quota(errors: list[str],
-                        engine: str,
-                        query: str,
-                        where_vals: tuple,
-                        count: int,
-                        require_min: int,
-                        require_max: int) -> bool:
+def _db_assert_query_quota(errors: list[str],
+                           engine: str,
+                           query: str,
+                           where_vals: tuple,
+                           count: int,
+                           require_min: int,
+                           require_max: int) -> bool:
     """
     Verify whether the number of tuples returned is compliant with the constraints specified.
 
-    :param errors:  incidental error messages
+    :param errors: incidental error messages
     :param query: the query statement used
     :param where_vals: the bind values used in the query
     :param count: the number of tuples returned
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :return: whether or not the number of tuples returned is compliant
     """
@@ -123,14 +125,27 @@
             msg: str = _db_build_query_msg(query_stmt=query,
                                             engine=engine,
                                             bind_vals=where_vals)
             errors.append(f"{count} tuples returned, {require_min} expected, for '{msg}'")
 
     return result
 
+
+def _db_assert_temp_file(temp_file: str | Path) -> Path:
+
+    result: Path
+    if temp_file is None:
+        result = Path(gettempdir(), str(uuid.uuid4()))
+    elif isinstance(temp_file, str):
+        result = Path(temp_file)
+    else:
+        result = temp_file
+
+    return result
+
 def _db_get_params(engine: str) -> tuple:
     """
     Return the current connection parameters being used for *engine*.
 
     The connection parameters are returned as a *tuple*, with the elements
     *name*, *user*, *pwd*, *host*, *port*.
     The meaning of some parameters may vary between different database engines.
```

### Comparing `pypomes_db-0.6.0/src/pypomes_db/db_pomes.py` & `pypomes_db-0.6.1/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.0/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.6.1/src/pypomes_db/oracle_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # noinspection DuplicatedCode
 from logging import Logger
 from oracledb import Connection, connect, init_oracle_client
 from pathlib import Path
-from tempfile import NamedTemporaryFile
 from typing import Any
 
 from .db_common import (
     _DB_CONN_DATA,
-    _assert_query_quota, _db_get_params, _db_log, _db_except_msg
+    _db_assert_query_quota, _db_assert_temp_file,
+    _db_get_params, _db_log, _db_except_msg
 )
 from .db_pomes import db_bulk_insert as db_bulk_insert_to
 from .db_pomes import db_update_lob as db_update_lob_to
 
 
 def db_connect(errors: list[str],
                logger: Logger) -> Connection:
@@ -93,21 +93,21 @@
             # execute the query
             cursor.execute(statement=sel_stmt,
                            parameters=where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
-            if _assert_query_quota(errors=errors,
-                                   engine="oracle",
-                                   query=sel_stmt,
-                                   where_vals=where_vals,
-                                   count=count,
-                                   require_min=require_min,
-                                   require_max=require_max):
+            if _db_assert_query_quota(errors=errors,
+                                      engine="oracle",
+                                      query=sel_stmt,
+                                      where_vals=where_vals,
+                                      count=count,
+                                      require_min=require_min,
+                                      require_max=require_max):
                 # yes, retrieve the returned tuples
                 rows: list = cursor.fetchall()
                 result = [tuple(row) for row in rows]
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
@@ -321,21 +321,15 @@
                                                logger=logger)
 
     # make sure to have a target table
     if not target_table:
         target_table = lob_table
 
     # make sure to have a temporary file
-    lob_file: Any
-    if temp_file is None:
-        lob_file = NamedTemporaryFile("wb")
-    elif isinstance(temp_file, str | Path):
-        lob_file = Path(temp_file)
-    else:
-        lob_file = temp_file
+    lob_file: Any = _db_assert_temp_file(temp_file)
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
 
     # buid the query
     pks: str = ", ".join(pk_columns)
@@ -434,15 +428,15 @@
     :param logger: optional logger
     """
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     # make sure to have a data file
-    data_file: Path = Path(lob_file) if isinstance(lob_file, str | Path) else lob_file
+    data_file: Path = Path(lob_file) if isinstance(lob_file, str) else lob_file
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
 
     # build the UPDATE query
     where_clause: str = " AND ".join([f"{column} = :{inx}"
```

### Comparing `pypomes_db-0.6.0/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.6.1/src/pypomes_db/postgres_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # noinspection DuplicatedCode
 from logging import WARNING, Logger
 from pathlib import Path
 from psycopg2 import Binary, connect
 from psycopg2.extras import DictCursor, execute_values
 # noinspection PyProtectedMember
 from psycopg2._psycopg import connection
-from tempfile import NamedTemporaryFile
 from typing import Any
 
 from .db_common import (
-    _assert_query_quota, _db_get_params, _db_log, _db_except_msg
+    _db_assert_query_quota, _db_assert_temp_file,
+    _db_get_params, _db_log, _db_except_msg
 )
 from .db_pomes import db_bulk_insert as db_bulk_insert_to
 from .db_pomes import db_update_lob as db_update_lob_to
 
 
 def db_connect(errors: list[str],
                logger: Logger = None) -> connection:
@@ -93,21 +93,21 @@
         with curr_conn.cursor() as cursor:
             cursor.execute(query=f"{sel_stmt};",
                            vars=where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
-            if _assert_query_quota(errors=errors,
-                                   engine="postgres",
-                                   query=sel_stmt,
-                                   where_vals=where_vals,
-                                   count=count,
-                                   require_min=require_min,
-                                   require_max=require_max):
+            if _db_assert_query_quota(errors=errors,
+                                      engine="postgres",
+                                      query=sel_stmt,
+                                      where_vals=where_vals,
+                                      count=count,
+                                      require_min=require_min,
+                                      require_max=require_max):
                 # yes, retrieve the returned tuples
                 result = list(cursor)
 
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
@@ -164,17 +164,17 @@
                            sql=insert_stmt,
                            argslist=insert_vals)
             result = len(insert_vals)
         # commit the transaction
         curr_conn.commit()
     except ValueError as e:
         curr_conn.rollback()
-        # is the exception ValueError('A string literal cannot contain NUL (0x00) characters.') ?
+        # is the exception ValueError("A string literal cannot contain NUL (0x00) characters.") ?
         if "contain NUL" in e.args[0]:
-            # yes, log the occcurence and remove the NULLs
+            # yes, log the occurence, remove the NULLs, and try again
             _db_log(logger=logger,
                     engine="postgres",
                     level=WARNING,
                     stmt=f"Found NULLs in values for {insert_stmt}")
             # search for NULLs in input data
             clean_rows: list[tuple[int, list]] = []
             for inx, vals in enumerate(insert_vals):
@@ -192,18 +192,14 @@
                 insert_vals[clean_row[0]] = tuple(clean_row[1])
             # insert the clean data
             db_bulk_insert(errors=errors,
                            insert_stmt=insert_stmt,
                            insert_vals=insert_vals,
                            conn=conn,
                            logger=logger)
-
-
-
-
     except Exception as e:
         curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
@@ -357,21 +353,15 @@
                                                logger=logger)
 
     # make sure to have a target table
     if not target_table:
         target_table = lob_table
 
     # make sure to have a temporary file
-    lob_file: Any
-    if temp_file is None:
-        lob_file = NamedTemporaryFile("wb")
-    elif isinstance(temp_file, str | Path):
-        lob_file = Path(temp_file)
-    else:
-        lob_file = temp_file
+    lob_file: Path = _db_assert_temp_file(temp_file)
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
 
     # buid the query
     pks: str = ", ".join(pk_columns)
@@ -430,14 +420,16 @@
         curr_conn.rollback()
         if target_conn:
             target_conn.rollback()
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
+        if lob_file.exists():
+            lob_file.unlink()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
             stmt=(f"{result} LOBs migrated, "
@@ -470,15 +462,15 @@
     :param logger: optional logger
     """
     # make sure to have a connection
     curr_conn: connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     # make sure to have a data file
-    data_file: Path = Path(lob_file) if isinstance(lob_file, str | Path) else lob_file
+    data_file: Path = Path(lob_file) if isinstance(lob_file, str) else lob_file
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
 
     # build the UPDATE query
     where_clause: str = " AND ".join([f"{column} = %s" for column in pk_columns])
```

### Comparing `pypomes_db-0.6.0/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.6.1/src/pypomes_db/sqlserver_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # noinspection DuplicatedCode
 from logging import Logger
 from pyodbc import Binary, Connection, Row, connect
 from pathlib import Path
-from tempfile import NamedTemporaryFile
 from typing import Any
 
 from .db_common import (
-    _assert_query_quota, _db_get_params, _db_log, _db_except_msg
+    _db_assert_query_quota, _db_assert_temp_file,
+    _db_get_params, _db_log, _db_except_msg
 )
 from .db_pomes import db_bulk_insert as db_bulk_insert_to
 from .db_pomes import db_update_lob as db_update_lob_to
 
 
 def db_connect(errors: list[str],
                logger: Logger = None) -> Connection:
@@ -90,21 +90,21 @@
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(sel_stmt, where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
-            if _assert_query_quota(errors=errors,
-                                   engine="sqlserver",
-                                   query=sel_stmt,
-                                   where_vals=where_vals,
-                                   count=count,
-                                   require_min=require_min,
-                                   require_max=require_max):
+            if _db_assert_query_quota(errors=errors,
+                                      engine="sqlserver",
+                                      query=sel_stmt,
+                                      where_vals=where_vals,
+                                      count=count,
+                                      require_min=require_min,
+                                      require_max=require_max):
                 # yes, retrieve the returned tuples
                 rows: list[Row] = cursor.fetchall()
                 result = [tuple(row) for row in rows]
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
@@ -321,21 +321,15 @@
                                                logger=logger)
 
     # make sure to have a target table
     if not target_table:
         target_table = lob_table
 
     # make sure to have a temporary file
-    lob_file: Any
-    if temp_file is None:
-        lob_file = NamedTemporaryFile("wb")
-    elif isinstance(temp_file, str | Path):
-        lob_file = Path(temp_file)
-    else:
-        lob_file = temp_file
+    lob_file: Any = _db_assert_temp_file(temp_file)
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
 
     # buid the query
     pks: str = ", ".join(pk_columns)
@@ -434,15 +428,15 @@
     :param logger: optional logger
     """
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     # make sure to have a data file
-    data_file: Path = Path(lob_file) if isinstance(lob_file, str | Path) else lob_file
+    data_file: Path = Path(lob_file) if isinstance(lob_file, str) else lob_file
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
 
     # build the UPDATE query
     where_clause: str = " AND ".join([f"{column} = ?" for column in pk_columns])
```

### Comparing `pypomes_db-0.6.0/LICENSE` & `pypomes_db-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.0/pyproject.toml` & `pypomes_db-0.6.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.6.0/PKG-INFO` & `pypomes_db-0.6.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.6.0
+Version: 0.6.1
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

