# Comparing `tmp/suql-1.1.7a4.tar.gz` & `tmp/suql-1.1.7a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.1.7a4.tar", last modified: Wed May  8 07:12:58 2024, max compression
+gzip compressed data, was "suql-1.1.7a5.tar", last modified: Wed May  8 18:55:38 2024, max compression
```

## Comparing `suql-1.1.7a4.tar` & `suql-1.1.7a5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-05-08 07:12:58.295307 suql-1.1.7a4/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.7a4/LICENSE
--rw-------   0 oval      (1000) users      (100)     5021 2024-05-08 07:12:58.295307 suql-1.1.7a4/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4415 2024-04-30 04:28:53.000000 suql-1.1.7a4/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-05-08 07:12:58.295307 suql-1.1.7a4/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1541 2024-05-08 07:04:13.000000 suql-1.1.7a4/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-05-08 07:12:58.291307 suql-1.1.7a4/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-05-08 07:12:58.291307 suql-1.1.7a4/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17372 2024-05-08 07:07:27.000000 suql-1.1.7a4/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    20887 2024-05-07 05:23:38.000000 suql-1.1.7a4/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.7a4/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     3563 2024-05-06 21:19:43.000000 suql-1.1.7a4/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)     9612 2024-04-17 08:33:05.000000 suql-1.1.7a4/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-05-08 07:12:58.295307 suql-1.1.7a4/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.7a4/src/suql/prompts/__init__.py
--rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/answer_qa.prompt
--rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/field_classification.prompt
--rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/if_db_classification.prompt
--rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/opening_hours.prompt
--rw-------   0 oval      (1000) users      (100)     5671 2024-05-08 07:10:13.000000 suql-1.1.7a4/src/suql/prompts/parser_suql.prompt
--rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/verification.prompt
--rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/yelp_response_SQL.prompt
--rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/yelp_response_no_results.prompt
-drwx------   0 oval      (1000) users      (100)        0 2024-05-08 07:12:58.295307 suql-1.1.7a4/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.7a4/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    71135 2024-05-08 07:04:05.000000 suql-1.1.7a4/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-05-08 07:12:58.291307 suql-1.1.7a4/src/suql.egg-info/
--rw-r--r--   0 oval      (1000) users      (100)     5021 2024-05-08 07:12:58.000000 suql-1.1.7a4/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      824 2024-05-08 07:12:58.000000 suql-1.1.7a4/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-05-08 07:12:58.000000 suql-1.1.7a4/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      206 2024-05-08 07:12:58.000000 suql-1.1.7a4/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-05-08 07:12:58.000000 suql-1.1.7a4/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-05-08 18:55:38.863685 suql-1.1.7a5/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.7a5/LICENSE
+-rw-------   0 oval      (1000) users      (100)     5021 2024-05-08 18:55:38.863685 suql-1.1.7a5/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4415 2024-04-30 04:28:53.000000 suql-1.1.7a5/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-05-08 18:55:38.863685 suql-1.1.7a5/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1541 2024-05-08 18:54:38.000000 suql-1.1.7a5/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-05-08 18:55:38.859685 suql-1.1.7a5/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-05-08 18:55:38.863685 suql-1.1.7a5/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.7a5/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17521 2024-05-08 18:54:38.000000 suql-1.1.7a5/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    20887 2024-05-07 05:23:38.000000 suql-1.1.7a5/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.7a5/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     3563 2024-05-06 21:19:43.000000 suql-1.1.7a5/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)     9612 2024-04-17 08:33:05.000000 suql-1.1.7a5/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-05-08 18:55:38.863685 suql-1.1.7a5/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.7a5/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.7a5/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.7a5/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.7a5/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.7a5/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5671 2024-05-08 18:54:38.000000 suql-1.1.7a5/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.7a5/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.7a5/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.7a5/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-05-08 18:55:38.863685 suql-1.1.7a5/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.7a5/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    71135 2024-05-08 18:52:25.000000 suql-1.1.7a5/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.7a5/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-05-08 18:55:38.863685 suql-1.1.7a5/src/suql.egg-info/
+-rw-r--r--   0 oval      (1000) users      (100)     5021 2024-05-08 18:55:38.000000 suql-1.1.7a5/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-05-08 18:55:38.000000 suql-1.1.7a5/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-05-08 18:55:38.000000 suql-1.1.7a5/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      206 2024-05-08 18:55:38.000000 suql-1.1.7a5/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-05-08 18:55:38.000000 suql-1.1.7a5/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.1.7a4/LICENSE` & `suql-1.1.7a5/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/PKG-INFO` & `suql-1.1.7a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.7a4
+Version: 1.1.7a5
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.7a4 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.7a5 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.7a4/README.md` & `suql-1.1.7a5/README.md`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/setup.py` & `suql-1.1.7a5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.1.7a4"
+version = "1.1.7a5"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
```

### Comparing `suql-1.1.7a4/src/suql/agent.py` & `suql-1.1.7a5/src/suql/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,27 +366,29 @@
                 max_tokens=200,
                 temperature=0.0,
                 stop_tokens=["\n"],
                 postprocess=False,
             )
             return response
 
-        pattern = r"'([^']*)'\s*=\s*opening_hours"
+        pattern_1 = r"'([^']*)'\s*=\s*opening_hours"
+        pattern_2 = r"opening_hours\s*=\s*'([^']*)'"
 
-        def replacer(match):
-            opening_hours_query = match.group(0).split(" = ")[0]
+        def replacer(match, pattern):
+            opening_hours_query = match.group(0).split("=")[pattern]
             opening_hours_translated = convert_opening_hours_query(opening_hours_query)
             return (
                 'search_by_opening_hours("opening_hours", '
                 + "'"
                 + opening_hours_translated
                 + "')"
             )
 
-        return re.sub(pattern, replacer, suql_query_)
+        res = re.sub(pattern_1, lambda x: replacer(x, 0), suql_query_)
+        return re.sub(pattern_2, lambda x: replacer(x, 1), res)
 
     suql_query = process_query_location(suql_query)
     suql_query = process_query_opening_hours(suql_query)
     return suql_query
 
 
 def compute_next_turn(
```

### Comparing `suql-1.1.7a4/src/suql/faiss_embedding.py` & `suql-1.1.7a5/src/suql/faiss_embedding.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/src/suql/free_text_fcns_server.py` & `suql-1.1.7a5/src/suql/free_text_fcns_server.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/src/suql/postgresql_connection.py` & `suql-1.1.7a5/src/suql/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/src/suql/prompt_continuation.py` & `suql-1.1.7a5/src/suql/prompt_continuation.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/src/suql/prompts/if_db_classification.prompt` & `suql-1.1.7a5/src/suql/prompts/if_db_classification.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/src/suql/prompts/opening_hours.prompt` & `suql-1.1.7a5/src/suql/prompts/opening_hours.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/src/suql/prompts/parser_suql.prompt` & `suql-1.1.7a5/src/suql/prompts/parser_suql.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/src/suql/prompts/yelp_response_SQL.prompt` & `suql-1.1.7a5/src/suql/prompts/yelp_response_SQL.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/src/suql/prompts/yelp_response_no_results.prompt` & `suql-1.1.7a5/src/suql/prompts/yelp_response_no_results.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.1.7a5/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/src/suql/utils.py` & `suql-1.1.7a5/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a4/src/suql.egg-info/PKG-INFO` & `suql-1.1.7a5/src/suql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.7a4
+Version: 1.1.7a5
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.7a4 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.7a5 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.7a4/src/suql.egg-info/SOURCES.txt` & `suql-1.1.7a5/src/suql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

