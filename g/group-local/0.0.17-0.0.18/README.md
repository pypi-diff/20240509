# Comparing `tmp/group_local-0.0.17.tar.gz` & `tmp/group_local-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "group_local-0.0.17.tar", last modified: Wed May  8 07:48:27 2024, max compression
+gzip compressed data, was "group_local-0.0.18.tar", last modified: Thu May  9 10:21:37 2024, max compression
```

## Comparing `group_local-0.0.17.tar` & `group_local-0.0.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:48:27.630983 group_local-0.0.17/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-08 07:48:27.630983 group_local-0.0.17/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:48:27.626983 group_local-0.0.17/group_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:48:27.630983 group_local-0.0.17/group_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:48:08.000000 group_local-0.0.17/group_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-05-08 07:48:08.000000 group_local-0.0.17/group_local/src/group_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-08 07:48:08.000000 group_local-0.0.17/group_local/src/group_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:48:27.630983 group_local-0.0.17/group_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-08 07:48:27.000000 group_local-0.0.17/group_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-08 07:48:27.000000 group_local-0.0.17/group_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:48:27.000000 group_local-0.0.17/group_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 07:48:27.000000 group_local-0.0.17/group_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 07:48:27.000000 group_local-0.0.17/group_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-08 07:48:08.000000 group_local-0.0.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:48:27.630983 group_local-0.0.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-08 07:48:08.000000 group_local-0.0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:21:37.195467 group_local-0.0.18/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 10:21:37.195467 group_local-0.0.18/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:21:37.191467 group_local-0.0.18/group_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:21:37.191467 group_local-0.0.18/group_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:21:18.000000 group_local-0.0.18/group_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-09 10:21:18.000000 group_local-0.0.18/group_local/src/group_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-09 10:21:18.000000 group_local-0.0.18/group_local/src/group_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:21:37.191467 group_local-0.0.18/group_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 10:21:37.000000 group_local-0.0.18/group_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-09 10:21:37.000000 group_local-0.0.18/group_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:21:37.000000 group_local-0.0.18/group_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 10:21:37.000000 group_local-0.0.18/group_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 10:21:37.000000 group_local-0.0.18/group_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-09 10:21:18.000000 group_local-0.0.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:21:37.195467 group_local-0.0.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-09 10:21:18.000000 group_local-0.0.18/setup.py
```

### Comparing `group_local-0.0.17/PKG-INFO` & `group_local-0.0.18/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.17
+Version: 0.0.18
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `group_local-0.0.17/group_local/src/group_local.py` & `group_local-0.0.18/group_local/src/group_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,17 +218,21 @@
             "updated_user_id": user_context.get_effective_user_id(),
             "updated_real_user_id": user_context.get_real_user_id(),
             "updated_effective_user_id": user_context.get_effective_user_id(),
             "updated_effective_profile_id": user_context.get_effective_profile_id(),
             "is_title_approved": group_dict.get('is_title_approved', None),
             "is_description_approved": group_dict.get('is_description_approved', None)
         }
-        GenericCRUDML.update_by_id(self, table_name="group_ml_table",
-                                   id_column_value=group_id, data_json=group_ml_data_json,
-                                   id_column_name="group_ml_id")
+        where_clause = "group_id = %s AND lang_code = %s"
+        GenericCRUDML.update_by_where(
+            self, table_name="group_ml_table",
+            where=where_clause,
+            params=(group_id, lang_code.value),
+            data_json=group_ml_data_json
+        )
         logger.end()
 
     def get_group_dict_by_group_id(self, group_id: int, group_ml_id: int = None,
                                    view_name: str = "group_view",
                                    ml_view_name: str = "group_ml_also_not_approved_view") -> Dict[str, any]:
         logger.start(object={'group_id': group_id})
         group_ml_dict = {}
```

### Comparing `group_local-0.0.17/group_local/src/group_local_constants.py` & `group_local-0.0.18/group_local/src/group_local_constants.py`

 * *Files identical despite different names*

### Comparing `group_local-0.0.17/group_local.egg-info/PKG-INFO` & `group_local-0.0.18/group_local.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.17
+Version: 0.0.18
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `group_local-0.0.17/setup.py` & `group_local-0.0.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "group-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/group-local
-    version='0.0.17',
+    version='0.0.18',
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles group-local Python",
     long_description="PyPI Package for Circles group-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/group-main-local-python-package",
     packages=[package_dir],
```

