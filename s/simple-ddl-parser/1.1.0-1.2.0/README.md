# Comparing `tmp/simple_ddl_parser-1.1.0.tar.gz` & `tmp/simple_ddl_parser-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_ddl_parser-1.1.0.tar", max compression
+gzip compressed data, was "simple_ddl_parser-1.2.0.tar", max compression
```

## Comparing `simple_ddl_parser-1.1.0.tar` & `simple_ddl_parser-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1093 2024-04-21 13:06:45.341924 simple_ddl_parser-1.1.0/LICENSE
--rw-r--r--   0        0        0    34132 2024-04-21 18:02:39.551590 simple_ddl_parser-1.1.0/docs/README.rst
--rw-r--r--   0        0        0     1597 2024-04-21 15:09:57.914841 simple_ddl_parser-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      268 2024-04-21 13:06:45.342548 simple_ddl_parser-1.1.0/simple_ddl_parser/__init__.py
--rw-r--r--   0        0        0     2326 2024-04-21 13:06:45.342619 simple_ddl_parser-1.1.0/simple_ddl_parser/cli.py
--rwxr-xr-x   0        0        0     8775 2024-04-21 18:02:30.108248 simple_ddl_parser-1.1.0/simple_ddl_parser/ddl_parser.py
--rw-r--r--   0        0        0      755 2024-04-21 13:06:45.342889 simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/__init__.py
--rw-r--r--   0        0        0      702 2024-04-21 13:06:45.342962 simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/bigquery.py
--rw-r--r--   0        0        0     5326 2024-04-21 18:02:06.063289 simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/hql.py
--rw-r--r--   0        0        0      260 2024-04-21 13:06:45.343230 simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/ibm.py
--rw-r--r--   0        0        0     2608 2024-04-21 13:06:45.343300 simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/mssql.py
--rw-r--r--   0        0        0      510 2024-04-21 13:06:45.343371 simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/mysql.py
--rw-r--r--   0        0        0     1877 2024-04-21 13:06:45.343492 simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/oracle.py
--rw-r--r--   0        0        0      426 2024-04-21 13:06:45.343551 simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/psql.py
--rw-r--r--   0        0        0      928 2024-04-21 13:06:45.343627 simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/redshift.py
--rw-r--r--   0        0        0     7301 2024-04-21 15:29:08.970067 simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/snowflake.py
--rw-r--r--   0        0        0      305 2024-04-21 13:06:45.344047 simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/spark_sql.py
--rw-r--r--   0        0        0    57574 2024-04-21 16:13:24.628626 simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/sql.py
--rw-r--r--   0        0        0    13207 2024-04-21 13:06:45.344438 simple_ddl_parser-1.1.0/simple_ddl_parser/output/base_data.py
--rw-r--r--   0        0        0     5306 2024-04-21 13:06:45.344678 simple_ddl_parser-1.1.0/simple_ddl_parser/output/core.py
--rw-r--r--   0        0        0     9439 2024-04-21 13:06:45.344903 simple_ddl_parser-1.1.0/simple_ddl_parser/output/dialects.py
--rw-r--r--   0        0        0     2840 2024-04-21 13:06:45.345129 simple_ddl_parser-1.1.0/simple_ddl_parser/output/table_data.py
--rwxr-xr-x   0        0        0    13223 2024-04-21 13:06:45.345356 simple_ddl_parser-1.1.0/simple_ddl_parser/parser.py
--rw-r--r--   0        0        0   270915 2024-04-21 15:43:04.170510 simple_ddl_parser-1.1.0/simple_ddl_parser/parsetab.py
--rw-r--r--   0        0        0      279 2024-04-21 18:00:56.584045 simple_ddl_parser-1.1.0/simple_ddl_parser/test.py
--rw-r--r--   0        0        0     3113 2024-04-21 15:46:10.007759 simple_ddl_parser-1.1.0/simple_ddl_parser/tokens.py
--rw-r--r--   0        0        0     1391 2024-04-21 13:06:45.346777 simple_ddl_parser-1.1.0/simple_ddl_parser/utils.py
--rw-r--r--   0        0        0    35611 1970-01-01 00:00:00.000000 simple_ddl_parser-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-21 13:06:45.341924 simple_ddl_parser-1.2.0/LICENSE
+-rw-r--r--   0        0        0    34808 2024-05-09 12:29:57.878709 simple_ddl_parser-1.2.0/docs/README.rst
+-rw-r--r--   0        0        0     1597 2024-05-09 12:29:34.311940 simple_ddl_parser-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      268 2024-04-21 13:06:45.342548 simple_ddl_parser-1.2.0/simple_ddl_parser/__init__.py
+-rw-r--r--   0        0        0     2326 2024-04-21 13:06:45.342619 simple_ddl_parser-1.2.0/simple_ddl_parser/cli.py
+-rwxr-xr-x   0        0        0     8860 2024-05-09 12:29:34.312314 simple_ddl_parser-1.2.0/simple_ddl_parser/ddl_parser.py
+-rw-r--r--   0        0        0      755 2024-04-21 13:06:45.342889 simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/__init__.py
+-rw-r--r--   0        0        0      702 2024-04-21 13:06:45.342962 simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/bigquery.py
+-rw-r--r--   0        0        0     5326 2024-04-21 18:02:06.063289 simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/hql.py
+-rw-r--r--   0        0        0      260 2024-04-21 13:06:45.343230 simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/ibm.py
+-rw-r--r--   0        0        0     2608 2024-04-21 13:06:45.343300 simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/mssql.py
+-rw-r--r--   0        0        0      510 2024-05-09 11:52:40.501830 simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/mysql.py
+-rw-r--r--   0        0        0     2145 2024-05-09 12:29:34.312658 simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/oracle.py
+-rw-r--r--   0        0        0      426 2024-04-21 13:06:45.343551 simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/psql.py
+-rw-r--r--   0        0        0      928 2024-04-21 13:06:45.343627 simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/redshift.py
+-rw-r--r--   0        0        0     7278 2024-04-21 18:13:32.614147 simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/snowflake.py
+-rw-r--r--   0        0        0      305 2024-04-21 13:06:45.344047 simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/spark_sql.py
+-rw-r--r--   0        0        0    57779 2024-05-09 12:29:34.313079 simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/sql.py
+-rw-r--r--   0        0        0    13207 2024-04-21 13:06:45.344438 simple_ddl_parser-1.2.0/simple_ddl_parser/output/base_data.py
+-rw-r--r--   0        0        0     5306 2024-04-21 13:06:45.344678 simple_ddl_parser-1.2.0/simple_ddl_parser/output/core.py
+-rw-r--r--   0        0        0     9553 2024-05-09 12:29:34.313465 simple_ddl_parser-1.2.0/simple_ddl_parser/output/dialects.py
+-rw-r--r--   0        0        0     2840 2024-04-21 13:06:45.345129 simple_ddl_parser-1.2.0/simple_ddl_parser/output/table_data.py
+-rwxr-xr-x   0        0        0    13223 2024-05-09 11:53:06.889442 simple_ddl_parser-1.2.0/simple_ddl_parser/parser.py
+-rw-r--r--   0        0        0   953295 2024-05-09 12:29:34.314715 simple_ddl_parser-1.2.0/simple_ddl_parser/parsetab.py
+-rw-r--r--   0        0        0      247 2024-05-09 12:19:31.247646 simple_ddl_parser-1.2.0/simple_ddl_parser/test.py
+-rw-r--r--   0        0        0     3133 2024-05-09 12:29:34.315259 simple_ddl_parser-1.2.0/simple_ddl_parser/tokens.py
+-rw-r--r--   0        0        0     1391 2024-04-21 13:06:45.346777 simple_ddl_parser-1.2.0/simple_ddl_parser/utils.py
+-rw-r--r--   0        0        0    36287 1970-01-01 00:00:00.000000 simple_ddl_parser-1.2.0/PKG-INFO
```

### Comparing `simple_ddl_parser-1.1.0/LICENSE` & `simple_ddl_parser-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.1.0/docs/README.rst` & `simple_ddl_parser-1.2.0/docs/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -545,14 +545,44 @@
 
 * https://github.com/ankitdata ,
 * https://github.com/kalyan939
 
 Changelog
 ---------
 
+**v1.2.0**
+
+Fixes
+^^^^^
+
+MySQL:
+
+
+#. Fixed issue relative to auto_increment that caused empty output if auto_increment defined in table properties -
+   https://github.com/xnuinside/simple-ddl-parser/issues/206
+
+Improvements
+^^^^^^^^^^^^
+
+MySQL:
+
+
+#. auto_increment added as property to mysql output
+
+Oracle:
+
+
+#. Added support for  constraint name in column definition - https://github.com/xnuinside/simple-ddl-parser/issues/203
+#. Added support for GENERATED (ALWAYS | (BY DEFAULT [ON NULL])) AS IDENTITY in column definition
+
+PostgreSQL:
+
+
+#. Added support for CAST statement in column GENERATE ALWAYS expression - https://github.com/xnuinside/simple-ddl-parser/issues/198
+
 **v1.1.0**
 
 Improvements
 ^^^^^^^^^^^^
 
 MySQL:
```

### Comparing `simple_ddl_parser-1.1.0/pyproject.toml` & `simple_ddl_parser-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simple-ddl-parser"
-version = "1.1.0"
+version = "1.2.0"
 description = "Simple DDL Parser to parse SQL & dialects like HQL, TSQL (MSSQL), Oracle, AWS Redshift, Snowflake, MySQL, PostgreSQL, etc ddl files to json/python dict with full information about columns: types, defaults, primary keys, etc.; sequences, alters, custom types & other entities from ddl."
 authors = ["Iuliia Volkova <xnuinside@gmail.com>"]
 license = "MIT"
 readme = "docs/README.rst"
 homepage = "https://github.com/xnuinside/simple-ddl-parser"
 repository = "https://github.com/xnuinside/simple-ddl-parser"
 classifiers = [
```

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/cli.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/cli.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/ddl_parser.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/ddl_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,17 @@
         if t.type != "ID":
             self.lexer.after_columns = True
         elif self.lexer.columns_def:
             t.type = tok.columns_definition.get(t.value.upper(), t.type)
         return t
 
     def process_body_tokens(self, t: LexToken) -> LexToken:
-        if (
-            self.lexer.last_par == "RP" and not self.lexer.lp_open
-        ) or (self.lexer.after_columns and not self.lexer.columns_def):
+        if (self.lexer.last_par == "RP" and not self.lexer.lp_open) or (
+            self.lexer.after_columns and not self.lexer.columns_def
+        ):
             t = self.after_columns_tokens(t)
         elif self.lexer.columns_def:
             t.type = tok.columns_definition.get(t.value.upper(), t.type)
         elif self.lexer.sequence:
             t.type = tok.sequence_reserved.get(t.value.upper(), "ID")
         return t
 
@@ -166,15 +166,18 @@
     def exceptional_cases(self, value: str) -> bool:
         if value == "TABLESPACE" and self.lexer.last_token == "INDEX":
             return True
         return False
 
     def t_AUTOINCREMENT(self, t: LexToken):
         r"(?i:AUTO_INCREMENT|AUTOINCREMENT)\b"
-        t.type = "AUTOINCREMENT"
+        if not self.lexer.after_columns:
+            t.type = "AUTOINCREMENT"
+        else:
+            t.type = "ID"
         return self.set_last_token(t)
 
     def t_ID(self, t: LexToken):
         r"([0-9]+[.][0-9]*([e][+-]?[0-9]+)?|[0-9]\.[0-9])\w|([a-zA-Z_,0-9:><\/\\\=\-\+\~\%$@#\|&?;*\()!{}\[\]\`\[\]]+)"
         t.type = tok.symbol_tokens.get(t.value, "ID")
 
         if t.type == "LP":
```

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/__init__.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/bigquery.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/bigquery.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/hql.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/hql.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/mssql.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/mssql.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/oracle.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/oracle.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,7 +58,14 @@
         p[0] = p[1]
         p[0]["storage"] = p_list[-1]
 
     def p_expr_index(self, p: List) -> None:
         """expr : expr ID INDEX"""
         p[0] = p[1]
         p[0][f"{p[2].lower()}_index"] = True
+
+    def p_generated_by(self, p: List) -> None:
+        """generated_by : GENERATED BY DEFAULT ON NULL AS ID
+        | GENERATED BY ID AS ID
+        | GENERATED BY DEFAULT AS ID"""
+        p_list = list(p)
+        p[0] = {"generated_by": " ".join(p_list[3:]).upper()}
```

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/redshift.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/redshift.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/snowflake.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
+import re
 from typing import List
 
 from simple_ddl_parser.utils import remove_par
-import re
 
 
 class Snowflake:
     def p_clone(self, p: List) -> None:
         """clone : CLONE id"""
         p_list = list(p)
         p[0] = {"clone": {"from": p_list[-1]}}
 
     def p_expression_cluster_by(self, p: List) -> None:
-        """expr : expr cluster_by
-        """
+        """expr : expr cluster_by"""
         p_list = list(p)
         p[0] = p[1]
         p[0].update(p_list[-1])
 
     def p_cluster_by(self, p: List) -> None:
         """cluster_by : CLUSTER BY LP pid RP
-               | CLUSTER BY pid
-               """
+        | CLUSTER BY pid
+        """
         p_list = remove_par(list(p))
         p[0] = {"cluster_by": p_list[-1]}
 
     def p_multi_id_or_string(self, p: List) -> None:
         """multi_id_or_string : id_or_string
         | multi_id_or_string id_or_string
         | f_call
```

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/dialects/sql.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/dialects/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,14 +413,16 @@
         | defcolumn on_update
         | defcolumn options
         | defcolumn autoincrement
         | defcolumn option_order_noorder
         | defcolumn option_with_tag
         | defcolumn option_with_masking_policy
         | defcolumn as_virtual
+        | defcolumn constraint
+        | defcolumn generated_by
         """
         p[0] = p[1]
         p_list = list(p)
 
         pk, default, unique, references, nullable = self.get_column_properties(p_list)
 
         self.set_property(p)
@@ -978,30 +980,32 @@
             schema = p_list[-3]
             table_name = p_list[-1]
         else:
             table_name = p_list[-1]
         p[0].update({"schema": schema, "table_name": table_name})
 
     def p_c_index(self, p: List) -> None:
-        """ c_index : INDEX LP index_pid RP
-                    | INDEX id LP index_pid RP
-                    | c_index INVISIBLE
-                    | c_index VISIBLE """
+        """c_index : INDEX LP index_pid RP
+        | INDEX id LP index_pid RP
+        | c_index INVISIBLE
+        | c_index VISIBLE"""
         p_list = remove_par(p_list=list(p))
         if isinstance(p_list[1], dict):
             p[0] = p_list[1]
-            p[0]["details"] = {p_list[-1].lower() : True}
+            p[0]["details"] = {p_list[-1].lower(): True}
         else:
             if len(p_list) == 3:
                 name = None
             else:
                 name = p_list[2]
-            p[0] = {'index_stmt': True,
-                    "name": name,
-                    "columns": p_list[-1]['detailed_columns']}
+            p[0] = {
+                "index_stmt": True,
+                "name": name,
+                "columns": p_list[-1]["detailed_columns"],
+            }
 
     def p_create_index(self, p: List) -> None:
         """create_index : CREATE INDEX id
         | CREATE UNIQUE INDEX id
         | create_index ON id
         | CREATE CLUSTERED INDEX id
         """
@@ -1057,43 +1061,41 @@
         | expr COMMA foreign ref
         | expr encode
         | expr DEFAULT id id id
         | expr RP
         """
         p[0] = p[1] or defaultdict(list)
         p_list = remove_par(list(p))
-        if len(p_list) > 2 and 'cluster_by' in p_list[2]:
+        if len(p_list) > 2 and "cluster_by" in p_list[2]:
             p[0].update(p_list[2])
         if p_list[-1] != "," and p_list[-1] is not None:
             if "type" in p_list[-1] and "name" in p_list[-1]:
                 if not p[0].get("columns"):
                     p[0]["columns"] = []
                 p[0]["columns"].append(p_list[-1])
             elif "index_stmt" in p_list[-1]:
                 del p_list[-1]["index_stmt"]
                 if not p[0].get("index"):
                     p[0]["index"] = []
                 index_data = p_list[-1]
                 _index = {
-                        "clustered": False,
-                        "columns": [index_data["columns"]],
-                        "detailed_columns": [
-                            {
-                                "name": index_data["columns"],
-                                "nulls": "LAST",
-                                "order": "ASC",
-                            }
-                        ],
-                        "index_name": index_data["name"],
-                        "unique": False,
-                    }
-                _index.update(index_data.get('details', {}))
-                p[0]["index"].append(
-                    _index
-                )
+                    "clustered": False,
+                    "columns": [index_data["columns"]],
+                    "detailed_columns": [
+                        {
+                            "name": index_data["columns"],
+                            "nulls": "LAST",
+                            "order": "ASC",
+                        }
+                    ],
+                    "index_name": index_data["name"],
+                    "unique": False,
+                }
+                _index.update(index_data.get("details", {}))
+                p[0]["index"].append(_index)
             elif "check" in p_list[-1]:
                 p[0] = self.extract_check_data(p, p_list)
             elif "enforced" in p_list[-1]:
                 p_list[-2].update(p_list[-1])
                 p[0].update({"primary_key_enforced": p_list[-1]["enforced"]})
             elif "DEFAULT" in p_list:
                 p[0].update({"default_charset": p_list[-1]})
@@ -1383,19 +1385,23 @@
         p[0] = {"nullable": nullable}
 
     def p_f_call(self, p: List) -> None:
         """f_call : id LP RP
         | id LP f_call RP
         | id LP multi_id RP
         | id LP pid RP
+        | id LP id AS id RP
         """
         p_list = list(p)
         if isinstance(p[1], list):
             p[0] = p[1]
             p[0].append(p_list[-1])
+        elif p_list[1].upper() == "CAST":
+            p_list = remove_par(p_list)
+            p[0] = {"cast": {"value": p_list[2], "as": p_list[4]}}
         else:
             value = ""
             for elem in p_list[1:]:
                 if isinstance(elem, list):
                     elem = ",".join(elem)
                 value += elem
             p[0] = value
@@ -1406,14 +1412,16 @@
         | f_call
         | multi_id f_call
         """
         p_list = list(p)
         if isinstance(p[1], list):
             p[0] = p[1]
             p[0].append(p_list[-1])
+        elif isinstance(p_list[1], dict):
+            p[0] = p[1]
         else:
             value = " ".join(p_list[1:])
             p[0] = value
 
     def p_funct_args(self, p: List) -> None:
         """funct_args : LP multi_id RP"""
         p[0] = {"args": f"({p[2]})"}
```

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/output/base_data.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/output/base_data.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/output/core.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/output/core.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/output/dialects.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/output/dialects.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,17 @@
 class MySSQL(Dialect):
     engine: Optional[str] = field(
         default=None, metadata={"exclude_if_not_provided": True}
     )
     default_charset: Optional[str] = field(
         default=None, metadata={"exclude_if_not_provided": True}
     )
+    auto_increment: Optional[str] = field(
+        default=None, metadata={"exclude_if_not_provided": True}
+    )
 
 
 @dataclass
 @dialect(name="bigquery")
 class BigQuery(Dialect):
     dataset: Optional[str] = field(default=False)
     project: Optional[str] = field(
```

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/output/table_data.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/output/table_data.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/parser.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/tokens.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,18 @@
     "COMMENT",
     "POLICY",
     "MASKING",
     "WITH",
     "ORDER",
     "NOORDER",
     "VISIBLE",
-    "INVISIBLE"
+    "INVISIBLE",
+    "AUTOINCREMENT",
+    "GENERATED",
+    "BY",
 }
 columns_definition = {value: value for value in columns_definition}
 columns_definition[","] = "COMMA"
 
 
 first_liners = {
     "LIKE",
@@ -153,15 +156,14 @@
             "STRING_BASE",
             "DQ_STRING",
             "LP",
             "RP",
             "LT",
             "RT",
             "COMMAT",
-            "AUTOINCREMENT",
         ]
         + list(definition_statements.values())
         + list(common_statements.values())
         + list(columns_definition.values())
         + list(sequence_reserved.values())
         + list(after_columns_tokens.values())
         + list(alter_tokens.values())
```

### Comparing `simple_ddl_parser-1.1.0/simple_ddl_parser/utils.py` & `simple_ddl_parser-1.2.0/simple_ddl_parser/utils.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.1.0/PKG-INFO` & `simple_ddl_parser-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-ddl-parser
-Version: 1.1.0
+Version: 1.2.0
 Summary: Simple DDL Parser to parse SQL & dialects like HQL, TSQL (MSSQL), Oracle, AWS Redshift, Snowflake, MySQL, PostgreSQL, etc ddl files to json/python dict with full information about columns: types, defaults, primary keys, etc.; sequences, alters, custom types & other entities from ddl.
 Home-page: https://github.com/xnuinside/simple-ddl-parser
 License: MIT
 Author: Iuliia Volkova
 Author-email: xnuinside@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -574,14 +574,44 @@
 
 * https://github.com/ankitdata ,
 * https://github.com/kalyan939
 
 Changelog
 ---------
 
+**v1.2.0**
+
+Fixes
+^^^^^
+
+MySQL:
+
+
+#. Fixed issue relative to auto_increment that caused empty output if auto_increment defined in table properties -
+   https://github.com/xnuinside/simple-ddl-parser/issues/206
+
+Improvements
+^^^^^^^^^^^^
+
+MySQL:
+
+
+#. auto_increment added as property to mysql output
+
+Oracle:
+
+
+#. Added support for  constraint name in column definition - https://github.com/xnuinside/simple-ddl-parser/issues/203
+#. Added support for GENERATED (ALWAYS | (BY DEFAULT [ON NULL])) AS IDENTITY in column definition
+
+PostgreSQL:
+
+
+#. Added support for CAST statement in column GENERATE ALWAYS expression - https://github.com/xnuinside/simple-ddl-parser/issues/198
+
 **v1.1.0**
 
 Improvements
 ^^^^^^^^^^^^
 
 MySQL:
```

