# Comparing `tmp/data_source_local-0.0.2.tar.gz` & `tmp/data_source_local-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_source_local-0.0.2.tar", last modified: Tue May  7 06:22:11 2024, max compression
+gzip compressed data, was "data_source_local-0.0.3.tar", last modified: Thu May  9 12:21:39 2024, max compression
```

## Comparing `data_source_local-0.0.2.tar` & `data_source_local-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:22:11.468521 data_source_local-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-07 06:22:11.468521 data_source_local-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-07 06:21:50.000000 data_source_local-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:22:11.464521 data_source_local-0.0.2/data_source_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:22:11.468521 data_source_local-0.0.2/data_source_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 06:21:50.000000 data_source_local-0.0.2/data_source_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-07 06:21:50.000000 data_source_local-0.0.2/data_source_local/src/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-07 06:21:50.000000 data_source_local-0.0.2/data_source_local/src/data_source_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 06:21:50.000000 data_source_local-0.0.2/data_source_local/src/data_source_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:22:11.468521 data_source_local-0.0.2/data_source_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-07 06:22:11.000000 data_source_local-0.0.2/data_source_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 06:22:11.000000 data_source_local-0.0.2/data_source_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 06:22:11.000000 data_source_local-0.0.2/data_source_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 06:22:11.000000 data_source_local-0.0.2/data_source_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 06:22:11.000000 data_source_local-0.0.2/data_source_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-07 06:21:50.000000 data_source_local-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 06:22:11.468521 data_source_local-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-07 06:21:50.000000 data_source_local-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:21:39.398729 data_source_local-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 12:21:39.394729 data_source_local-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-09 12:21:18.000000 data_source_local-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:21:39.394729 data_source_local-0.0.3/data_source_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:21:39.394729 data_source_local-0.0.3/data_source_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:21:18.000000 data_source_local-0.0.3/data_source_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-09 12:21:18.000000 data_source_local-0.0.3/data_source_local/src/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-09 12:21:18.000000 data_source_local-0.0.3/data_source_local/src/data_source_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-09 12:21:18.000000 data_source_local-0.0.3/data_source_local/src/data_source_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:21:39.394729 data_source_local-0.0.3/data_source_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 12:21:39.000000 data_source_local-0.0.3/data_source_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-09 12:21:39.000000 data_source_local-0.0.3/data_source_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:21:39.000000 data_source_local-0.0.3/data_source_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-09 12:21:39.000000 data_source_local-0.0.3/data_source_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 12:21:39.000000 data_source_local-0.0.3/data_source_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-09 12:21:18.000000 data_source_local-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:21:39.398729 data_source_local-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-09 12:21:18.000000 data_source_local-0.0.3/setup.py
```

### Comparing `data_source_local-0.0.2/README.md` & `data_source_local-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `data_source_local-0.0.2/data_source_local/src/data_source.py` & `data_source_local-0.0.3/data_source_local/src/data_source.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 from database_mysql_local.generic_crud import GenericCRUD
 from language_remote.lang_code import LangCode
 from logger_local.LoggerLocal import Logger
 
+# TODO constans -> constants, obj -> data_source_logger_code_obj
 from .data_source_constans import obj
 
 logger = Logger.create_logger(object=obj)
 
 
+# TODO Change to DataSources
+# TODO Add MetaLogger
 class DataSource(GenericCRUD):
 
     def __init__(self):
         super().__init__(default_schema_name='data_source',
                          default_table_name='data_source_table',
                          default_view_table_name='data_source_ml_en_view')
 
+    # TODO Why do we return two ints?
+    # TODO lang_code: LangCode
+    # TODO insert_fields() per our Python Class methods naming conventions https://docs.google.com/document/d/1QtCVak8f9rOtZo9raRhYHf1-7-Sfs8rru_iv3HjTH6E/edit?usp=sharing
     def insert_data_source(self, data_source_name: str, lang_code: str = LangCode.ENGLISH.value) -> (int, int):
+        # TODO Both are not needed if using the MetaLogger
         METHOD_NAME = 'insert_data_source'
         logger.start(METHOD_NAME, object={
             'data_source_name': data_source_name,
             'lang_code': lang_code})
         try:
             data_source_json = {
-                'created_user_id': logger.user_context.get_real_user_id(),
+                'created_user_id': logger.user_context.get_effective_user_id(),
                 'updated_user_id': logger.user_context.get_effective_user_id()
             }
             data_source_id = self.insert(data_json=data_source_json)
             data_source_ml_json = {
                 'data_source_id': data_source_id,
                 'lang_code': lang_code,
                 'data_source_name': data_source_name,
-                'created_user_id': logger.user_context.get_real_user_id(),
+                'created_user_id': logger.user_context.get_effective_user_id(),
                 'updated_user_id': logger.user_context.get_effective_user_id()
             }
             data_source_ml_id = self.insert(
                 table_name='data_source_ml_table',
                 data_json=data_source_ml_json)
+            # TODO Why do we need to return the data_source_ml_id?
             logger.end(METHOD_NAME, object={
                 'data_source_id': data_source_id,
                 'data_source_ml_id': data_source_ml_id})
             return data_source_id, data_source_ml_id
 
         except Exception as e:
             logger.exception(
```

### Comparing `data_source_local-0.0.2/setup.py` & `data_source_local-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "data-source-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/data-source-local
-    version='0.0.2',
+    version='0.0.3',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description=PACKAGE_NAME,
```

