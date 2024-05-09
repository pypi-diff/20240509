# Comparing `tmp/pypomes_db-0.6.1.tar.gz` & `tmp/pypomes_db-0.6.2.tar.gz`

## Comparing `pypomes_db-0.6.1.tar` & `pypomes_db-0.6.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38244 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    24638 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    23999 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    22578 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     8993 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    24802 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    24238 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    22727 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.2/PKG-INFO
```

### Comparing `pypomes_db-0.6.1/src/pypomes_db/__init__.py` & `pypomes_db-0.6.2/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.1/src/pypomes_db/db_common.py` & `pypomes_db-0.6.2/src/pypomes_db/db_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,24 +121,24 @@
           count < require_min):
         # yes, report the error, if applicable
         result = False
         if isinstance(errors, list):
             msg: str = _db_build_query_msg(query_stmt=query,
                                             engine=engine,
                                             bind_vals=where_vals)
-            errors.append(f"{count} tuples returned, {require_min} expected, for '{msg}'")
+            errors.append(f"{count} tuples returned, at least {require_min} expected, for '{msg}'")
 
     return result
 
 
 def _db_assert_temp_file(temp_file: str | Path) -> Path:
 
     result: Path
     if temp_file is None:
-        result = Path(gettempdir(), str(uuid.uuid4()))
+        result = Path(gettempdir(), str(uuid.uuid4()), ".bin")
     elif isinstance(temp_file, str):
         result = Path(temp_file)
     else:
         result = temp_file
 
     return result
```

### Comparing `pypomes_db-0.6.1/src/pypomes_db/db_pomes.py` & `pypomes_db-0.6.2/src/pypomes_db/db_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -651,15 +651,14 @@
                                      lob_column=lob_column,
                                      pk_columns=pk_columns,
                                      pk_vals=pk_vals,
                                      lob_file=lob_file,
                                      chunk_size=chunk_size,
                                      conn=conn,
                                      logger=logger)
-        pass
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
         sqlserver_pomes.db_update_lob(errors=errors,
                                       lob_table=lob_table,
                                       lob_column=lob_column,
                                       pk_columns=pk_columns,
                                       pk_vals=pk_vals,
```

### Comparing `pypomes_db-0.6.1/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.6.2/src/pypomes_db/oracle_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,33 +348,36 @@
             # fetch rows
             for row in cursor:
 
                 # retrieve the values of the primary key columns (leave blob column out)
                 pk_vals: tuple = tuple([row[inx] for inx in range(blob_index)])
 
                 # access the blob in chunks and write it to file
+                size: int = 0
                 blob: Any = row[blob_index]
                 with lob_file.open(mode="wb") as file:
                     blob_data: bytes = blob.read(chunk_size)
                     while blob_data:
+                        size += len(blob_data)
                         file.write(blob_data)
                         blob_data = blob.read(chunk_size)
 
-                # send blob to the destination database
+                # send blob to the destination database, if applicable
                 op_errors: list[str] = []
-                db_update_lob_to(errors=op_errors,
-                                 lob_table=target_table,
-                                 lob_column=target_column,
-                                 lob_file=lob_file,
-                                 chunk_size=chunk_size,
-                                 pk_columns=pk_columns,
-                                 pk_vals=pk_vals,
-                                 engine=target_engine,
-                                 conn=target_conn,
-                                 logger=logger)
+                if size > 0:
+                    db_update_lob_to(errors=op_errors,
+                                     lob_table=target_table,
+                                     lob_column=target_column,
+                                     lob_file=lob_file,
+                                     chunk_size=chunk_size,
+                                     pk_columns=pk_columns,
+                                     pk_vals=pk_vals,
+                                     engine=target_engine,
+                                     conn=target_conn,
+                                     logger=logger)
                 # errors ?
                 if op_errors:
                     # yes, register them
                     errors.extend(op_errors)
                 else:
                     # no, increment the LOB migration counter
                     result += 1
```

### Comparing `pypomes_db-0.6.1/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.6.2/src/pypomes_db/postgres_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,17 +178,19 @@
             # search for NULLs in input data
             clean_rows: list[tuple[int, list]] = []
             for inx, vals in enumerate(insert_vals):
                 replace: bool = False
                 clean_row: list = []
                 for val in vals:
                     if isinstance(val, str) and val.count(chr(0)) > 0:
-                        val = val.replace(chr(0), "")
+                        clean_val: str = val.replace(chr(0), "")
                         replace = True
-                    clean_row.append(val)
+                    else:
+                        clean_val: str = val
+                    clean_row.append(clean_val)
                 if replace:
                     clean_rows.append((inx, clean_row))
             # remove them
             for clean_row in clean_rows:
                 insert_vals[clean_row[0]] = tuple(clean_row[1])
             # insert the clean data
             db_bulk_insert(errors=errors,
@@ -380,33 +382,36 @@
             # fetch rows
             for row in cursor:
 
                 # retrieve the values of the primary key columns (leave blob column out)
                 pk_vals: tuple = tuple([row[inx] for inx in range(blob_index)])
 
                 # access the blob in chunks and write it to file
+                size: int = 0
                 blob: Any = row[blob_index]
                 with lob_file.open(mode="wb") as file:
                     blob_data: bytes = blob.read(chunk_size)
                     while blob_data:
+                        size += len(blob_data)
                         file.write(blob_data)
                         blob_data = blob.read(chunk_size)
 
                 # send blob to the destination database
                 op_errors: list[str] = []
-                db_update_lob_to(errors=op_errors,
-                                 lob_table=target_table,
-                                 lob_column=target_column,
-                                 lob_file=lob_file,
-                                 chunk_size=chunk_size,
-                                 pk_columns=pk_columns,
-                                 pk_vals=pk_vals,
-                                 engine=target_engine,
-                                 conn=target_conn,
-                                 logger=logger)
+                if size > 0:
+                    db_update_lob_to(errors=op_errors,
+                                     lob_table=target_table,
+                                     lob_column=target_column,
+                                     lob_file=lob_file,
+                                     chunk_size=chunk_size,
+                                     pk_columns=pk_columns,
+                                     pk_vals=pk_vals,
+                                     engine=target_engine,
+                                     conn=target_conn,
+                                     logger=logger)
                 # errors ?
                 if op_errors:
                     # yes, register them
                     errors.extend(op_errors)
                 else:
                     # no, increment the LOB migration counter
                     result += 1
```

### Comparing `pypomes_db-0.6.1/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.6.2/src/pypomes_db/sqlserver_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,33 +348,36 @@
             # fetch rows
             for row in cursor:
 
                 # retrieve the values of the primary key columns (leave blob column out)
                 pk_vals: tuple = tuple([row[inx] for inx in range(blob_index)])
 
                 # access the blob in chunks and write it to file
+                size: int = 0
                 blob: Any = row[blob_index]
                 with lob_file.open(mode="wb") as file:
                     blob_data: bytes = blob.read(chunk_size)
                     while blob_data:
+                        size += len(blob_data)
                         file.write(blob_data)
                         blob_data = blob.read(chunk_size)
 
                 # send blob to the destination database
                 op_errors: list[str] = []
-                db_update_lob_to(errors=op_errors,
-                                 lob_table=target_table,
-                                 lob_column=target_column,
-                                 lob_file=lob_file,
-                                 chunk_size=chunk_size,
-                                 pk_columns=pk_columns,
-                                 pk_vals=pk_vals,
-                                 engine=target_engine,
-                                 conn=target_conn,
-                                 logger=logger)
+                if size > 0:
+                    db_update_lob_to(errors=op_errors,
+                                     lob_table=target_table,
+                                     lob_column=target_column,
+                                     lob_file=lob_file,
+                                     chunk_size=chunk_size,
+                                     pk_columns=pk_columns,
+                                     pk_vals=pk_vals,
+                                     engine=target_engine,
+                                     conn=target_conn,
+                                     logger=logger)
                 # errors ?
                 if op_errors:
                     # yes, register them
                     errors.extend(op_errors)
                 else:
                     # no, increment the LOB migration counter
                     result += 1
```

### Comparing `pypomes_db-0.6.1/LICENSE` & `pypomes_db-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.1/pyproject.toml` & `pypomes_db-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.6.1/PKG-INFO` & `pypomes_db-0.6.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.6.1
+Version: 0.6.2
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

