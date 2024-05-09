# Comparing `tmp/pypomes_db-0.5.9.tar.gz` & `tmp/pypomes_db-0.6.0.tar.gz`

## Comparing `pypomes_db-0.5.9.tar` & `pypomes_db-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38244 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    24855 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    22789 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38244 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    24795 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    24090 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    22735 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.0/PKG-INFO
```

### Comparing `pypomes_db-0.5.9/src/pypomes_db/__init__.py` & `pypomes_db-0.6.0/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.9/src/pypomes_db/db_common.py` & `pypomes_db-0.6.0/src/pypomes_db/db_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,33 +169,33 @@
 
 
 def _db_log(logger: Logger,
             engine: str,
             err_msg: str = None,
             level: int = DEBUG,
             errors: list[str] = None,
-            query_stmt: str = None,
+            stmt: str = None,
             bind_vals: tuple = None) -> None:
     """
     Log *err_msg* and add it to *errors*, or else log the executed query, whichever is applicable.
 
     :param logger: the logger object
     :param err_msg: the error message to log
     :param level: log level (defaults to DEBUG)
     :param errors: optional incidental errors
-    :param query_stmt: optional the query statement
+    :param stmt: optional the query statement
     :param bind_vals: optional bind values for the query statement
     """
     if err_msg:
         if logger:
             logger.log(level, err_msg)
         if isinstance(errors, list):
             errors.append(err_msg)
-    if logger and query_stmt:
-        log_msg: str = _db_build_query_msg(query_stmt=query_stmt,
+    if logger and stmt:
+        log_msg: str = _db_build_query_msg(query_stmt=stmt,
                                            engine=engine,
                                            bind_vals=bind_vals)
         logger.log(level, log_msg)
 
 
 def _db_build_query_msg(query_stmt: str,
                         engine: str,
```

### Comparing `pypomes_db-0.5.9/src/pypomes_db/db_pomes.py` & `pypomes_db-0.6.0/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.9/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.6.0/src/pypomes_db/oracle_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                                  engine="oracle")
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=f"Connecting to '{name}' at '{host}'")
+            stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str],
                   sel_stmt: str,
                   where_vals: tuple,
@@ -119,15 +119,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=sel_stmt,
+            stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
@@ -173,15 +173,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=insert_stmt,
+            stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
 def db_bulk_migrate(errors: list[str],
                     sel_stmt: str,
@@ -262,19 +262,19 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=sel_stmt,
+            stmt=sel_stmt,
             bind_vals=where_vals)
     _db_log(logger=logger,
             engine="oracle",
-            query_stmt=(f"{result} tuples migrated, "
+            stmt=(f"{result} tuples migrated, "
                         f"from oracle to {target_engine}"))
 
     return result
 
 
 def db_migrate_lobs(errors: list[str],
                     lob_table: str,
@@ -400,15 +400,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=(f"{result} LOBs migrated, "
+            stmt=(f"{result} LOBs migrated, "
                         f"from oracle at {lob_table}.{lob_column} "
                         f"to {target_engine} at {target_table}.{target_column}"))
 
     return result
 
 
 def db_update_lob(errors: list[str],
@@ -478,15 +478,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             err_msg=err_msg,
             engine="oracle",
             errors=errors,
-            query_stmt=update_stmt,
+            stmt=update_stmt,
             bind_vals=pk_vals)
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
                conn: Connection,
@@ -535,15 +535,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=exc_stmt,
+            stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 # noinspection PyUnusedLocal
@@ -613,15 +613,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="oracle",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=proc_name,
+            stmt=proc_name,
             bind_vals=proc_vals)
 
     return result
 
 __is_initialized: str | None = None
 
 def initialize(errors: list[str],
@@ -648,10 +648,10 @@
             err_msg = _db_except_msg(exception=e,
                                      engine="oracle")
         # log the results
         _db_log(logger=logger,
                 engine="oracle",
                 err_msg=err_msg,
                 errors=errors,
-                query_stmt="Initializing the client")
+                stmt="Initializing the client")
 
     return result
```

### Comparing `pypomes_db-0.5.9/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.6.0/src/pypomes_db/postgres_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # noinspection DuplicatedCode
-from logging import Logger
+from logging import WARNING, Logger
 from pathlib import Path
 from psycopg2 import Binary, connect
 from psycopg2.extras import DictCursor, execute_values
 # noinspection PyProtectedMember
 from psycopg2._psycopg import connection
 from tempfile import NamedTemporaryFile
 from typing import Any
@@ -44,15 +44,15 @@
         err_msg = _db_except_msg(e, "postgres")
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=f"Connecting to '{name}' at '{host}'")
+            stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str],
                   sel_stmt: str,
                   where_vals: tuple,
@@ -119,15 +119,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=sel_stmt,
+            stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
@@ -162,29 +162,63 @@
         with curr_conn.cursor() as cursor:
             execute_values(cur=cursor,
                            sql=insert_stmt,
                            argslist=insert_vals)
             result = len(insert_vals)
         # commit the transaction
         curr_conn.commit()
+    except ValueError as e:
+        curr_conn.rollback()
+        # is the exception ValueError('A string literal cannot contain NUL (0x00) characters.') ?
+        if "contain NUL" in e.args[0]:
+            # yes, log the occcurence and remove the NULLs
+            _db_log(logger=logger,
+                    engine="postgres",
+                    level=WARNING,
+                    stmt=f"Found NULLs in values for {insert_stmt}")
+            # search for NULLs in input data
+            clean_rows: list[tuple[int, list]] = []
+            for inx, vals in enumerate(insert_vals):
+                replace: bool = False
+                clean_row: list = []
+                for val in vals:
+                    if isinstance(val, str) and val.count(chr(0)) > 0:
+                        val = val.replace(chr(0), "")
+                        replace = True
+                    clean_row.append(val)
+                if replace:
+                    clean_rows.append((inx, clean_row))
+            # remove them
+            for clean_row in clean_rows:
+                insert_vals[clean_row[0]] = tuple(clean_row[1])
+            # insert the clean data
+            db_bulk_insert(errors=errors,
+                           insert_stmt=insert_stmt,
+                           insert_vals=insert_vals,
+                           conn=conn,
+                           logger=logger)
+
+
+
+
     except Exception as e:
         curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=insert_stmt)
+            stmt=insert_stmt)
 
     return result
 
 
 def db_bulk_migrate(errors: list[str],
                     sel_stmt: str,
                     insert_stmt: str,
@@ -264,19 +298,19 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=sel_stmt,
+            stmt=sel_stmt,
             bind_vals=where_vals)
     _db_log(logger=logger,
             engine="postgres",
-            query_stmt=(f"{result} tuples migrated, "
+            stmt=(f"{result} tuples migrated, "
                         f"from postgres to {target_engine}"))
 
     return result
 
 
 def db_migrate_lobs(errors: list[str],
                     lob_table: str,
@@ -402,15 +436,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=(f"{result} LOBs migrated, "
+            stmt=(f"{result} LOBs migrated, "
                         f"from postgres at {lob_table}.{lob_column} "
                         f"to {target_engine} at {target_table}.{target_column}"))
 
     return result
 
 
 def db_update_lob(errors: list[str],
@@ -478,15 +512,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=update_stmt,
+            stmt=update_stmt,
             bind_vals=pk_vals)
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
                conn: connection,
@@ -535,15 +569,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=exc_stmt,
+            stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
 
 
 def db_call_procedure(errors: list[str],
@@ -592,11 +626,11 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="postgres",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=proc_stmt,
+            stmt=proc_stmt,
             bind_vals=proc_vals)
 
     return result
```

### Comparing `pypomes_db-0.5.9/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.6.0/src/pypomes_db/sqlserver_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                                  engine="sqlserver")
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=f"Connecting to '{name}' at '{host}'")
+            stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str],
                   sel_stmt: str,
                   where_vals: tuple,
@@ -116,15 +116,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=sel_stmt,
+            stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
@@ -173,15 +173,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=insert_stmt,
+            stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
 def db_bulk_migrate(errors: list[str],
                     sel_stmt: str,
@@ -262,19 +262,19 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=sel_stmt,
+            stmt=sel_stmt,
             bind_vals=where_vals)
     _db_log(logger=logger,
             engine="sqlserver",
-            query_stmt=(f"{result} tuples migrated, "
+            stmt=(f"{result} tuples migrated, "
                         f"from sqlserver to {target_engine}"))
 
     return result
 
 
 def db_migrate_lobs(errors: list[str],
                     lob_table: str,
@@ -400,15 +400,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=(f"{result} LOBs migrated, "
+            stmt=(f"{result} LOBs migrated, "
                         f"from sqlserver at {lob_table}.{lob_column} "
                         f"to {target_engine} at {target_table}.{target_column}"))
 
     return result
 
 
 def db_update_lob(errors: list[str],
@@ -475,15 +475,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=update_stmt,
+            stmt=update_stmt,
             bind_vals=pk_vals)
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
                conn: Connection,
@@ -531,15 +531,15 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=exc_stmt,
+            stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
 
 def db_call_procedure(errors: list[str],
                       proc_name: str,
@@ -588,11 +588,11 @@
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
-            query_stmt=proc_stmt,
+            stmt=proc_stmt,
             bind_vals=proc_vals)
 
     return result
```

### Comparing `pypomes_db-0.5.9/LICENSE` & `pypomes_db-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.9/pyproject.toml` & `pypomes_db-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.5.9"
+version = "0.6.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.5.9/PKG-INFO` & `pypomes_db-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.5.9
+Version: 0.6.0
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

