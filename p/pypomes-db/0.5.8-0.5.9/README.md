# Comparing `tmp/pypomes_db-0.5.8.tar.gz` & `tmp/pypomes_db-0.5.9.tar.gz`

## Comparing `pypomes_db-0.5.8.tar` & `pypomes_db-0.5.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38244 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    24498 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    22424 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38244 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    24855 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    22789 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.9/PKG-INFO
```

### Comparing `pypomes_db-0.5.8/src/pypomes_db/__init__.py` & `pypomes_db-0.5.9/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.8/src/pypomes_db/db_common.py` & `pypomes_db-0.5.9/src/pypomes_db/db_common.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         err_msg = f"Database engine '{engine}' unknown or not configured"
         errors.append(err_msg)
 
     return result
 
 
 def _assert_query_quota(errors: list[str],
+                        engine: str,
                         query: str,
                         where_vals: tuple,
                         count: int,
                         require_min: int,
                         require_max: int) -> bool:
     """
     Verify whether the number of tuples returned is compliant with the constraints specified.
@@ -103,29 +104,30 @@
     if (isinstance(require_min, int) and
         isinstance(require_max, int) and
         require_min == require_max and
         require_min != count):
         # yes, report the error, if applicable
         result = False
         if isinstance(errors, list):
-            errors.append(
-                f"{count} tuples returned, {require_min} expected, "
-                f"for '{_db_build_query_msg(query, where_vals)}'"
-            )
+            msg: str = _db_build_query_msg(query_stmt=query,
+                                            engine=engine,
+                                            bind_vals=where_vals)
+            errors.append(f"{count} tuples returned, {require_min} expected, for '{msg}'")
+
     # has a minimum number of tuples been defined but not returned ?
     elif (isinstance(require_min, int) and
           require_min > 0 and
           count < require_min):
         # yes, report the error, if applicable
         result = False
         if isinstance(errors, list):
-            errors.append(
-                f"{count} tuples returned, at least {require_min} expected, "
-                f"for '{_db_build_query_msg(query, where_vals)}'"
-            )
+            msg: str = _db_build_query_msg(query_stmt=query,
+                                            engine=engine,
+                                            bind_vals=where_vals)
+            errors.append(f"{count} tuples returned, {require_min} expected, for '{msg}'")
 
     return result
 
 def _db_get_params(engine: str) -> tuple:
     """
     Return the current connection parameters being used for *engine*.
 
@@ -162,36 +164,16 @@
     :return: the formatted error message
     """
     name: str = _DB_CONN_DATA[engine]["name"]
     host: str = _DB_CONN_DATA[engine]["host"]
     return f"Error accessing '{name}' at '{host}': {str_sanitize(f'{exception}')}"
 
 
-def _db_build_query_msg(query_stmt: str,
-                        bind_vals: tuple) -> str:
-    """
-    Format and return the message indicative of a query problem.
-
-    :param query_stmt: the query command
-    :param bind_vals: values associated with the query command
-    :return: message indicative of empty search
-    """
-    result: str = str_sanitize(query_stmt)
-
-    for val in bind_vals or []:
-        if isinstance(val, str):
-            sval: str = f"'{val}'"
-        else:
-            sval: str = str(val)
-        result = result.replace("?", sval, 1)
-
-    return result
-
-
 def _db_log(logger: Logger,
+            engine: str,
             err_msg: str = None,
             level: int = DEBUG,
             errors: list[str] = None,
             query_stmt: str = None,
             bind_vals: tuple = None) -> None:
     """
     Log *err_msg* and add it to *errors*, or else log the executed query, whichever is applicable.
@@ -205,9 +187,39 @@
     """
     if err_msg:
         if logger:
             logger.log(level, err_msg)
         if isinstance(errors, list):
             errors.append(err_msg)
     if logger and query_stmt:
-        log_msg: str = _db_build_query_msg(query_stmt, bind_vals)
+        log_msg: str = _db_build_query_msg(query_stmt=query_stmt,
+                                           engine=engine,
+                                           bind_vals=bind_vals)
         logger.log(level, log_msg)
+
+
+def _db_build_query_msg(query_stmt: str,
+                        engine: str,
+                        bind_vals: tuple) -> str:
+    """
+    Format and return the message indicative of a query problem.
+
+    :param query_stmt: the query command
+    :param bind_vals: values associated with the query command
+    :return: message indicative of empty search
+    """
+    result: str = str_sanitize(query_stmt)
+
+    for inx, val in enumerate(bind_vals or [], 1):
+        if isinstance(val, str):
+            sval: str = f"'{val}'"
+        else:
+            sval: str = str(val)
+        match engine:
+            case "oracle":
+                result = result.replace(f":{inx}", sval, 1)
+            case "postgres":
+                result = result.replace("%s", sval, 1)
+            case "sqlserver":
+                result = result.replace("?", sval, 1)
+
+    return result
```

### Comparing `pypomes_db-0.5.8/src/pypomes_db/db_pomes.py` & `pypomes_db-0.5.9/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.8/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.5.9/src/pypomes_db/oracle_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
 
     # log the results
     _db_log(logger=logger,
+            engine="oracle",
             err_msg=err_msg,
             errors=errors,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
@@ -93,14 +94,15 @@
             cursor.execute(statement=sel_stmt,
                            parameters=where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
+                                   engine="oracle",
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
                                    require_min=require_min,
                                    require_max=require_max):
                 # yes, retrieve the returned tuples
                 rows: list = cursor.fetchall()
@@ -114,14 +116,15 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="oracle",
             err_msg=err_msg,
             errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
@@ -167,14 +170,15 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="oracle",
             err_msg=err_msg,
             errors=errors,
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
@@ -255,19 +259,21 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="oracle",
             err_msg=err_msg,
             errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
     _db_log(logger=logger,
+            engine="oracle",
             query_stmt=(f"{result} tuples migrated, "
                         f"from oracle to {target_engine}"))
 
     return result
 
 
 def db_migrate_lobs(errors: list[str],
@@ -391,14 +397,15 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="oracle",
             err_msg=err_msg,
             errors=errors,
             query_stmt=(f"{result} LOBs migrated, "
                         f"from oracle at {lob_table}.{lob_column} "
                         f"to {target_engine} at {target_table}.{target_column}"))
 
     return result
@@ -469,14 +476,15 @@
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
             err_msg=err_msg,
+            engine="oracle",
             errors=errors,
             query_stmt=update_stmt,
             bind_vals=pk_vals)
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
@@ -524,14 +532,15 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="oracle",
             err_msg=err_msg,
             errors=errors,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
@@ -601,14 +610,15 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="oracle",
             err_msg=err_msg,
             errors=errors,
             query_stmt=proc_name,
             bind_vals=proc_vals)
 
     return result
 
@@ -635,12 +645,13 @@
             __is_initialized = True
         except Exception as e:
             result = False
             err_msg = _db_except_msg(exception=e,
                                      engine="oracle")
         # log the results
         _db_log(logger=logger,
+                engine="oracle",
                 err_msg=err_msg,
                 errors=errors,
                 query_stmt="Initializing the client")
 
     return result
```

### Comparing `pypomes_db-0.5.8/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.5.9/src/pypomes_db/postgres_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         # make sure the connection is not in autocommit mode
         result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(e, "postgres")
 
     # log the results
     _db_log(logger=logger,
+            engine="postgres",
             err_msg=err_msg,
             errors=errors,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
@@ -93,14 +94,15 @@
             cursor.execute(query=f"{sel_stmt};",
                            vars=where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
+                                   engine="postgres",
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
                                    require_min=require_min,
                                    require_max=require_max):
                 # yes, retrieve the returned tuples
                 result = list(cursor)
@@ -114,14 +116,15 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="postgres",
             err_msg=err_msg,
             errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
@@ -170,14 +173,15 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="postgres",
             err_msg=err_msg,
             errors=errors,
             query_stmt=insert_stmt)
 
     return result
 
 
@@ -257,21 +261,23 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="postgres",
             err_msg=err_msg,
             errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
     _db_log(logger=logger,
+            engine="postgres",
             query_stmt=(f"{result} tuples migrated, "
-                        f"from oracle to {target_engine}"))
+                        f"from postgres to {target_engine}"))
 
     return result
 
 
 def db_migrate_lobs(errors: list[str],
                     lob_table: str,
                     lob_column: str,
@@ -382,25 +388,26 @@
                     result += 1
 
         # commit the source and target transactions
         curr_conn.commit()
         target_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="postgres")
         curr_conn.rollback()
         if target_conn:
             target_conn.rollback()
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="postgres",
             err_msg=err_msg,
             errors=errors,
             query_stmt=(f"{result} LOBs migrated, "
                         f"from postgres at {lob_table}.{lob_column} "
                         f"to {target_engine} at {target_table}.{target_column}"))
 
     return result
@@ -460,22 +467,23 @@
                     lob_data = file.read(chunk_size)
 
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="postgres",
             err_msg=err_msg,
             errors=errors,
             query_stmt=update_stmt,
             bind_vals=pk_vals)
 
 
 def db_execute(errors: list[str],
@@ -524,14 +532,15 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="postgres",
             err_msg=err_msg,
             errors=errors,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
@@ -580,13 +589,14 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="postgres",
             err_msg=err_msg,
             errors=errors,
             query_stmt=proc_stmt,
             bind_vals=proc_vals)
 
     return result
```

### Comparing `pypomes_db-0.5.8/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.5.9/src/pypomes_db/sqlserver_pomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
 
     # log the results
     _db_log(logger=logger,
+            engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
@@ -90,14 +91,15 @@
         with curr_conn.cursor() as cursor:
             cursor.execute(sel_stmt, where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
+                                   engine="sqlserver",
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
                                    require_min=require_min,
                                    require_max=require_max):
                 # yes, retrieve the returned tuples
                 rows: list[Row] = cursor.fetchall()
@@ -111,14 +113,15 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
@@ -167,14 +170,15 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
@@ -255,21 +259,23 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
     _db_log(logger=logger,
+            engine="sqlserver",
             query_stmt=(f"{result} tuples migrated, "
-                        f"from oracle to {target_engine}"))
+                        f"from sqlserver to {target_engine}"))
 
     return result
 
 
 def db_migrate_lobs(errors: list[str],
                     lob_table: str,
                     lob_column: str,
@@ -380,29 +386,30 @@
                     result += 1
 
         # commit the source and target transactions
         curr_conn.commit()
         target_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
         curr_conn.rollback()
         if target_conn:
             target_conn.rollback()
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
             query_stmt=(f"{result} LOBs migrated, "
-                        f"from oracle at {lob_table}.{lob_column} "
+                        f"from sqlserver at {lob_table}.{lob_column} "
                         f"to {target_engine} at {target_table}.{target_column}"))
 
     return result
 
 
 def db_update_lob(errors: list[str],
                   lob_table: str,
@@ -457,22 +464,23 @@
                     lob_data = file.read(chunk_size)
 
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
             query_stmt=update_stmt,
             bind_vals=pk_vals)
 
 
 def db_execute(errors: list[str],
@@ -520,14 +528,15 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
@@ -576,13 +585,14 @@
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(logger=logger,
+            engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
             query_stmt=proc_stmt,
             bind_vals=proc_vals)
 
     return result
```

### Comparing `pypomes_db-0.5.8/LICENSE` & `pypomes_db-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.8/pyproject.toml` & `pypomes_db-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.5.8"
+version = "0.5.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.5.8/PKG-INFO` & `pypomes_db-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.5.8
+Version: 0.5.9
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

