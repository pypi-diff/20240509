# Comparing `tmp/labels-local-0.0.1.tar.gz` & `tmp/labels_local-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labels-local-0.0.1.tar", last modified: Mon Feb 12 04:58:19 2024, max compression
+gzip compressed data, was "labels_local-0.0.2.tar", last modified: Thu May  9 09:42:41 2024, max compression
```

## Comparing `labels-local-0.0.1.tar` & `labels_local-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 04:58:19.761873 labels-local-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-12 04:58:19.761873 labels-local-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-12 04:57:41.000000 labels-local-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 04:58:19.761873 labels-local-0.0.1/labels_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 04:58:19.761873 labels-local-0.0.1/labels_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-02-12 04:57:41.000000 labels-local-0.0.1/labels_local/src/labels_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-12 04:57:41.000000 labels-local-0.0.1/labels_local/src/labels_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 04:58:19.761873 labels-local-0.0.1/labels_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-12 04:58:19.000000 labels-local-0.0.1/labels_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-12 04:58:19.000000 labels-local-0.0.1/labels_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 04:58:19.000000 labels-local-0.0.1/labels_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-12 04:58:19.000000 labels-local-0.0.1/labels_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-12 04:58:19.000000 labels-local-0.0.1/labels_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-12 04:57:41.000000 labels-local-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 04:58:19.761873 labels-local-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-02-12 04:57:41.000000 labels-local-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:42:41.577107 labels_local-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-09 09:42:41.577107 labels_local-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 09:42:12.000000 labels_local-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:42:41.573107 labels_local-0.0.2/labels_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:42:41.577107 labels_local-0.0.2/labels_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-09 09:42:12.000000 labels_local-0.0.2/labels_local/src/labels_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-09 09:42:12.000000 labels_local-0.0.2/labels_local/src/labels_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:42:41.577107 labels_local-0.0.2/labels_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-09 09:42:41.000000 labels_local-0.0.2/labels_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-09 09:42:41.000000 labels_local-0.0.2/labels_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:42:41.000000 labels_local-0.0.2/labels_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-09 09:42:41.000000 labels_local-0.0.2/labels_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 09:42:41.000000 labels_local-0.0.2/labels_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-09 09:42:12.000000 labels_local-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:42:41.577107 labels_local-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-09 09:42:12.000000 labels_local-0.0.2/setup.py
```

### Comparing `labels-local-0.0.1/PKG-INFO` & `labels_local-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labels-local
-Version: 0.0.1
+Version: 0.0.2
 Summary: PyPI Package for Circles labels-local Python
 Home-page: https://github.com/circles-zone/label-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -13,9 +13,10 @@
 Requires-Dist: pytest>=7.4.0
 Requires-Dist: mysql-connector>=2.2.9
 Requires-Dist: logzio-python-handler>=4.1.0
 Requires-Dist: user-context-remote>=0.0.17
 Requires-Dist: python-sdk-remote>=0.0.27
 Requires-Dist: database-infrastructure-local>=0.0.23
 Requires-Dist: user-context-remote>=0.0.58
+Requires-Dist: group-local>=0.0.16
 
 PyPI Package for Circles labels-local Python
```

### Comparing `labels-local-0.0.1/labels_local/src/labels_local.py` & `labels_local-0.0.2/labels_local/src/labels_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from database_mysql_local.generic_crud_ml import GenericCRUDML
 from database_mysql_local.generic_mapping import GenericMapping
 from logger_local.LoggerLocal import Logger
 from language_remote.lang_code import LangCode
 from database_infrastructure_local.number_generator import NumberGenerator
 from user_context_remote.user_context import UserContext
+from group_local.group_local_constants import GroupLocalConstants
 
 from .labels_local_constants import LABELS_PYTHON_PACKAGE_CODE_LOGGER_OBJECT
 
 logger = Logger.create_logger(object=LABELS_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
 user_context = UserContext()
 
 DEFAULT_SCHEMA_NAME = "label"
 DEFAULT_TABLE_NAME = "label_table"
 DEFAULT_VIEW_TABLE_NAME = "label_view"
 DEFAULT_ID_COLUMN_NAME = "label_id"
 DEFAULT_ML_ID_COLUMN_NAME = "label_ml_id"
 DEFAULT_ENTITY1_NAME = "label"
+ENGLISH_GROUP_ID = GroupLocalConstants.ENGLISH_GROUP_ID
 
 
 class LabelsLocal(GenericMapping, GenericCRUDML):
 
     def __init__(self, default_schema_name: str = DEFAULT_SCHEMA_NAME, default_table_name: str = DEFAULT_TABLE_NAME,
                  default_view_table_name: str = DEFAULT_VIEW_TABLE_NAME,
                  default_id_column_name: str = DEFAULT_ID_COLUMN_NAME, default_entity_name1: str = DEFAULT_ENTITY1_NAME,
```

### Comparing `labels-local-0.0.1/labels_local/src/labels_local_constants.py` & `labels_local-0.0.2/labels_local/src/labels_local_constants.py`

 * *Files identical despite different names*

### Comparing `labels-local-0.0.1/labels_local.egg-info/PKG-INFO` & `labels_local-0.0.2/labels_local.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labels-local
-Version: 0.0.1
+Version: 0.0.2
 Summary: PyPI Package for Circles labels-local Python
 Home-page: https://github.com/circles-zone/label-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -13,9 +13,10 @@
 Requires-Dist: pytest>=7.4.0
 Requires-Dist: mysql-connector>=2.2.9
 Requires-Dist: logzio-python-handler>=4.1.0
 Requires-Dist: user-context-remote>=0.0.17
 Requires-Dist: python-sdk-remote>=0.0.27
 Requires-Dist: database-infrastructure-local>=0.0.23
 Requires-Dist: user-context-remote>=0.0.58
+Requires-Dist: group-local>=0.0.16
 
 PyPI Package for Circles labels-local Python
```

### Comparing `labels-local-0.0.1/setup.py` & `labels_local-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "labels-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.1',  # update only the minor version each time # https://pypi.org/project/labels-local/
+    version='0.0.2',  # update only the minor version each time # https://pypi.org/project/labels-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles labels-local Python",
     long_description="PyPI Package for Circles labels-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/label-local-python-package",
     packages=[package_dir],
@@ -25,10 +25,11 @@
         'PyMySQL>=1.0.2',
         'pytest>=7.4.0',
         'mysql-connector>=2.2.9',
         'logzio-python-handler>= 4.1.0',
         'user-context-remote>=0.0.17',
         'python-sdk-remote>=0.0.27',
         'database-infrastructure-local>=0.0.23',
-        'user-context-remote>=0.0.58'
+        'user-context-remote>=0.0.58',
+        'group-local>=0.0.16'
     ],
 )
```

