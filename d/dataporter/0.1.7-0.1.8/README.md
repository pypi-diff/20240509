# Comparing `tmp/dataporter-0.1.7.tar.gz` & `tmp/dataporter-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataporter-0.1.7.tar", max compression
+gzip compressed data, was "dataporter-0.1.8.tar", max compression
```

## Comparing `dataporter-0.1.7.tar` & `dataporter-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      354 2023-06-14 10:59:50.072481 dataporter-0.1.7/README.md
--rw-r--r--   0        0        0      228 2023-07-10 07:28:06.020794 dataporter-0.1.7/dataporter/__init__.py
--rw-r--r--   0        0        0     6890 2023-07-10 08:04:38.673802 dataporter-0.1.7/dataporter/csv2file.py
--rw-r--r--   0        0        0     7001 2023-07-07 12:14:47.084091 dataporter-0.1.7/dataporter/csv2sql.py
--rw-r--r--   0        0        0     3880 2023-10-08 11:57:10.306776 dataporter-0.1.7/dataporter/sql2csv.py
--rw-r--r--   0        0        0     1828 2023-06-14 11:17:06.906524 dataporter-0.1.7/dataporter/sql_schema2txt.py
--rw-r--r--   0        0        0      373 2023-07-07 14:17:22.768820 dataporter-0.1.7/dataporter/utils.py
--rw-r--r--   0        0        0      584 2023-10-08 11:57:40.143238 dataporter-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 dataporter-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      354 2024-01-05 11:36:35.102910 dataporter-0.1.8/README.md
+-rw-r--r--   0        0        0      228 2023-07-10 07:28:06.020794 dataporter-0.1.8/dataporter/__init__.py
+-rw-r--r--   0        0        0     6890 2023-07-10 08:04:38.673802 dataporter-0.1.8/dataporter/csv2file.py
+-rw-r--r--   0        0        0     7446 2024-05-09 14:25:18.357491 dataporter-0.1.8/dataporter/csv2sql.py
+-rw-r--r--   0        0        0     3880 2023-10-08 11:57:10.306776 dataporter-0.1.8/dataporter/sql2csv.py
+-rw-r--r--   0        0        0     1828 2023-06-14 11:17:06.906524 dataporter-0.1.8/dataporter/sql_schema2txt.py
+-rw-r--r--   0        0        0      373 2023-07-07 14:17:22.768820 dataporter-0.1.8/dataporter/utils.py
+-rw-r--r--   0        0        0      584 2024-05-09 14:25:57.648444 dataporter-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 dataporter-0.1.8/PKG-INFO
```

### Comparing `dataporter-0.1.7/dataporter/csv2file.py` & `dataporter-0.1.8/dataporter/csv2file.py`

 * *Files identical despite different names*

### Comparing `dataporter-0.1.7/dataporter/csv2sql.py` & `dataporter-0.1.8/dataporter/csv2sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,40 +3,51 @@
 from fire import Fire
 import pandas as pd
 from sqlalchemy import create_engine, text, exc
 from sqlalchemy.orm import sessionmaker
 from dataporter.utils import exec_multi_expr
 
 
-def insert(trunk_df: Iterable[pd.DataFrame], pandas_exprs: List[str] | None, debug: bool, sql_data_exists: Literal["append", "fail", "replace"], ignore_error: bool, table_name: str, conn, index: bool):
+def insert(
+    trunk_df: Iterable[pd.DataFrame],
+    pandas_exprs: List[str] | None,
+    debug: bool,
+    sql_data_exists: Literal["append", "fail", "replace"],
+    ignore_error: bool,
+    table_name: str,
+    conn,
+    index: bool,
+):
     for i, df in enumerate(trunk_df):
         if pandas_exprs:
             df = exec_multi_expr(df, exprs=pandas_exprs, debug=debug)
         df: pd.DataFrame
         logger.info(f"writing trunk {len(df)} line...")
 
-        if sql_data_exists == 'append':
+        if sql_data_exists == "append":
             # if exist strategy is append, all trunk always append
-            current_data_exist = 'append'
-        elif sql_data_exists == 'fail':
+            current_data_exist = "append"
+        elif sql_data_exists == "fail":
             # if exist strategy is fail, it should failed in first trunk
             # in later trunk, it should be append
             if i == 0:
-                current_data_exist = 'fail'
+                current_data_exist = "fail"
             else:
-                current_data_exist = 'append'
-        elif sql_data_exists == 'replace':
+                current_data_exist = "append"
+        elif sql_data_exists == "replace":
             if i == 0:
-                current_data_exist = 'replace'
+                current_data_exist = "replace"
             else:
-                current_data_exist = 'append'
+                current_data_exist = "append"
         else:
             raise ValueError(f"cannot parse current_data_exist value:{sql_data_exists}")
 
-        with logger.catch(message="write to db error, loss chunk.", reraise=not ignore_error):
+        with logger.catch(
+            message="write to db error, loss chunk.", reraise=not ignore_error
+        ):
             df.to_sql(
                 name=table_name,
                 con=conn,
                 index=index,
                 if_exists=current_data_exist,
             )
 
@@ -55,15 +66,15 @@
     sql_schema_file: str | None = None,
     sql_data_exists: Literal["fail", "replace", "append"] = "fail",
     read_chunk_size: Optional[int] = None,
     pandas_exprs: List[str] | None = None,
     debug: bool = False,
     ignore_error: bool = False,
     insert_in_transaction: bool = True,
-    **sql_kwargs: Any
+    **sql_kwargs: Any,
 ):
     """
     convert csv to sql table.
     :param sql_uri: database uri, according to sqlalchemy uri, according to sqlalchemy uri, e.g. "mysql+pymysql://username:pass@host:port/database.
     :param table_name: csv data insert table name.
     :param filename: source csv filename.
     :param header: default first line.
@@ -85,15 +96,17 @@
     engine = create_engine(url=sql_uri, **sql_kwargs)
 
     Session = sessionmaker(engine)
     # handle sql schema
     # if replace, drop table and create according to schema
     # if append or fail, try create table if not exist according to schema
     if sql_schema_file and sql_data_exists == "replace":
-        logger.warning("please ensure table_name matches the sql_schema_file content, or this will cause unexpected error.")
+        logger.warning(
+            "please ensure table_name matches the sql_schema_file content, or this will cause unexpected error."
+        )
 
         with open(sql_schema_file) as f:
             schema = f.read()
 
         with Session() as session:
             session.execute(text(f"DROP TABLE IF EXISTS {table_name}"))
             logger.info("dropping table...")
@@ -112,69 +125,77 @@
             except exc.OperationalError as e:
                 if e.orig.args[0] == 1050:
                     logger.info("table already exist.")
                 else:
                     raise e
 
     if read_chunk_size is None:
-        df = pd.read_csv(
-            filename,
-            sep=sep,
-            names=names,
-            header=header,
-            quotechar=quotechar,
-            escapechar=escapechar,
-            lineterminator=lineterminator,
-        )
+        if filename.lower().endswith(".csv"):
+            df = pd.read_csv(
+                filename,
+                sep=sep,
+                names=names,
+                header=header,
+                quotechar=quotechar,
+                escapechar=escapechar,
+                lineterminator=lineterminator,
+            )
+        else:
+            # json type
+            df = pd.read_json(
+                filename,
+                lines=True,
+            )
+
         if pandas_exprs:
             df = exec_multi_expr(df, exprs=pandas_exprs, debug=debug)
         with engine.begin() as conn:
-            df.to_sql(
-                name=table_name, con=conn, if_exists=sql_data_exists, index=index
-            )
+            df.to_sql(name=table_name, con=conn, if_exists=sql_data_exists, index=index)
             logger.info(f"inserted {len(df)} rows")
     else:
         logger.info("converting csv to sql...")
-        trunk_df = pd.read_csv(
-            filename,
-            sep=sep,
-            chunksize=read_chunk_size,
-            iterator=True,
-            names=names,
-            header=header,
-            quotechar=quotechar,
-            escapechar=escapechar,
-            lineterminator=lineterminator,
-        )
+        if filename.lower().endswith(".csv"):
+            trunk_df = pd.read_csv(
+                filename,
+                sep=sep,
+                chunksize=read_chunk_size,
+                iterator=True,
+                names=names,
+                header=header,
+                quotechar=quotechar,
+                escapechar=escapechar,
+                lineterminator=lineterminator,
+            )
+        else:
+            raise RuntimeError("not support json type in chunk mode")
         if insert_in_transaction:
             with engine.begin() as conn:
                 insert(
                     trunk_df=trunk_df,
                     pandas_exprs=pandas_exprs,
                     debug=debug,
                     sql_data_exists=sql_data_exists,
                     ignore_error=ignore_error,
                     table_name=table_name,
                     conn=conn,
-                    index=index
+                    index=index,
                 )
         else:
             with engine.connect() as conn:
                 insert(
                     trunk_df=trunk_df,
                     pandas_exprs=pandas_exprs,
                     debug=debug,
                     sql_data_exists=sql_data_exists,
                     ignore_error=ignore_error,
                     table_name=table_name,
                     conn=conn,
-                    index=index
+                    index=index,
                 )
 
-
         logger.info("done.")
 
 
 def main():
     Fire(csv2sql)
```

### Comparing `dataporter-0.1.7/dataporter/sql2csv.py` & `dataporter-0.1.8/dataporter/sql2csv.py`

 * *Files identical despite different names*

### Comparing `dataporter-0.1.7/dataporter/sql_schema2txt.py` & `dataporter-0.1.8/dataporter/sql_schema2txt.py`

 * *Files identical despite different names*

### Comparing `dataporter-0.1.7/pyproject.toml` & `dataporter-0.1.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataporter"
-version = "0.1.7"
+version = "0.1.8"
 description = "convert csv to csv/json/sql or convert sql to csv"
 authors = ["AuthorPlaceholder"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fire = "^0.5.0"
```

### Comparing `dataporter-0.1.7/PKG-INFO` & `dataporter-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataporter
-Version: 0.1.7
+Version: 0.1.8
 Summary: convert csv to csv/json/sql or convert sql to csv
 Author: AuthorPlaceholder
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=40.0.2,<41.0.0)
```

