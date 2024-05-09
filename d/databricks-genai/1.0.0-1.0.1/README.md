# Comparing `tmp/databricks_genai-1.0.0.tar.gz` & `tmp/databricks_genai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_genai-1.0.0.tar", last modified: Wed May  8 01:13:57 2024, max compression
+gzip compressed data, was "databricks_genai-1.0.1.tar", last modified: Thu May  9 21:48:23 2024, max compression
```

## Comparing `databricks_genai-1.0.0.tar` & `databricks_genai-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.580798 databricks_genai-1.0.0/
--rw-r--r--   0 nancy.hung   (502) staff       (20)     1757 2024-05-08 01:13:57.580483 databricks_genai-1.0.0/PKG-INFO
--rw-r--r--   0 nancy.hung   (502) staff       (20)      274 2024-04-17 00:17:05.000000 databricks_genai-1.0.0/README.md
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.570473 databricks_genai-1.0.0/databricks/
--rw-r--r--   0 nancy.hung   (502) staff       (20)      350 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/__init__.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.571106 databricks_genai-1.0.0/databricks/model_training/
--rw-r--r--   0 nancy.hung   (502) staff       (20)      185 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/__init__.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.572322 databricks_genai-1.0.0/databricks/model_training/api/
--rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/__init__.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     3170 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/config.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.573192 databricks_genai-1.0.0/databricks/model_training/api/engine/
--rw-r--r--   0 nancy.hung   (502) staff       (20)      355 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/engine/__init__.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)    32800 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/engine/engine.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     6573 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/exceptions.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.575243 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/
--rw-r--r--   0 nancy.hung   (502) staff       (20)      334 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/__init__.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     2639 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/cancel.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     8601 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/create.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     3611 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/delete.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     1049 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/get.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     3328 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/get_events.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     4748 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/list.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)    17845 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/utils.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.576764 databricks_genai-1.0.0/databricks/model_training/types/
--rw-r--r--   0 nancy.hung   (502) staff       (20)      131 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/types/__init__.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     5516 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/types/common.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     5255 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/types/run_status.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)     6109 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/types/train_config.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)    12046 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/types/training_run.py
--rw-r--r--   0 nancy.hung   (502) staff       (20)       47 2024-05-08 01:12:13.000000 databricks_genai-1.0.0/databricks/model_training/version.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.579220 databricks_genai-1.0.0/databricks_genai.egg-info/
--rw-r--r--   0 nancy.hung   (502) staff       (20)     1757 2024-05-08 01:13:57.000000 databricks_genai-1.0.0/databricks_genai.egg-info/PKG-INFO
--rw-r--r--   0 nancy.hung   (502) staff       (20)     1241 2024-05-08 01:13:57.000000 databricks_genai-1.0.0/databricks_genai.egg-info/SOURCES.txt
--rw-r--r--   0 nancy.hung   (502) staff       (20)        1 2024-05-08 01:13:57.000000 databricks_genai-1.0.0/databricks_genai.egg-info/dependency_links.txt
--rw-r--r--   0 nancy.hung   (502) staff       (20)      465 2024-05-08 01:13:57.000000 databricks_genai-1.0.0/databricks_genai.egg-info/requires.txt
--rw-r--r--   0 nancy.hung   (502) staff       (20)       11 2024-05-08 01:13:57.000000 databricks_genai-1.0.0/databricks_genai.egg-info/top_level.txt
--rw-r--r--   0 nancy.hung   (502) staff       (20)    31118 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/pyproject.toml
--rw-r--r--   0 nancy.hung   (502) staff       (20)       38 2024-05-08 01:13:57.580851 databricks_genai-1.0.0/setup.cfg
--rw-r--r--   0 nancy.hung   (502) staff       (20)     1778 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/setup.py
-drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.578606 databricks_genai-1.0.0/tests/
--rw-r--r--   0 nancy.hung   (502) staff       (20)      358 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/tests/test_package.py
+drwxr-xr-x   0 vansh.singh   (502) staff       (20)        0 2024-05-09 21:48:23.101861 databricks_genai-1.0.1/
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     1757 2024-05-09 21:48:23.101550 databricks_genai-1.0.1/PKG-INFO
+-rw-r--r--   0 vansh.singh   (502) staff       (20)      274 2024-03-07 23:24:14.000000 databricks_genai-1.0.1/README.md
+drwxr-xr-x   0 vansh.singh   (502) staff       (20)        0 2024-05-09 21:48:23.091010 databricks_genai-1.0.1/databricks/
+-rw-r--r--   0 vansh.singh   (502) staff       (20)      350 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/__init__.py
+drwxr-xr-x   0 vansh.singh   (502) staff       (20)        0 2024-05-09 21:48:23.091845 databricks_genai-1.0.1/databricks/model_training/
+-rw-r--r--   0 vansh.singh   (502) staff       (20)      185 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/__init__.py
+drwxr-xr-x   0 vansh.singh   (502) staff       (20)        0 2024-05-09 21:48:23.093021 databricks_genai-1.0.1/databricks/model_training/api/
+-rw-r--r--   0 vansh.singh   (502) staff       (20)        0 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/api/__init__.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     3170 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/api/config.py
+drwxr-xr-x   0 vansh.singh   (502) staff       (20)        0 2024-05-09 21:48:23.093584 databricks_genai-1.0.1/databricks/model_training/api/engine/
+-rw-r--r--   0 vansh.singh   (502) staff       (20)      355 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/api/engine/__init__.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)    32800 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/api/engine/engine.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     6573 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/api/exceptions.py
+drwxr-xr-x   0 vansh.singh   (502) staff       (20)        0 2024-05-09 21:48:23.096316 databricks_genai-1.0.1/databricks/model_training/api/foundation_model/
+-rw-r--r--   0 vansh.singh   (502) staff       (20)      334 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/api/foundation_model/__init__.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     2639 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/api/foundation_model/cancel.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     8601 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/api/foundation_model/create.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     3611 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/api/foundation_model/delete.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     1049 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/api/foundation_model/get.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     3328 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/api/foundation_model/get_events.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     4748 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/api/foundation_model/list.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)    17961 2024-05-09 21:47:33.000000 databricks_genai-1.0.1/databricks/model_training/api/utils.py
+drwxr-xr-x   0 vansh.singh   (502) staff       (20)        0 2024-05-09 21:48:23.098134 databricks_genai-1.0.1/databricks/model_training/types/
+-rw-r--r--   0 vansh.singh   (502) staff       (20)      131 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/types/__init__.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     5516 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/types/common.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     5255 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/types/run_status.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     6109 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/databricks/model_training/types/train_config.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)    12102 2024-05-09 21:47:33.000000 databricks_genai-1.0.1/databricks/model_training/types/training_run.py
+-rw-r--r--   0 vansh.singh   (502) staff       (20)       47 2024-05-09 21:47:33.000000 databricks_genai-1.0.1/databricks/model_training/version.py
+drwxr-xr-x   0 vansh.singh   (502) staff       (20)        0 2024-05-09 21:48:23.100126 databricks_genai-1.0.1/databricks_genai.egg-info/
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     1757 2024-05-09 21:48:23.000000 databricks_genai-1.0.1/databricks_genai.egg-info/PKG-INFO
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     1241 2024-05-09 21:48:23.000000 databricks_genai-1.0.1/databricks_genai.egg-info/SOURCES.txt
+-rw-r--r--   0 vansh.singh   (502) staff       (20)        1 2024-05-09 21:48:23.000000 databricks_genai-1.0.1/databricks_genai.egg-info/dependency_links.txt
+-rw-r--r--   0 vansh.singh   (502) staff       (20)      465 2024-05-09 21:48:23.000000 databricks_genai-1.0.1/databricks_genai.egg-info/requires.txt
+-rw-r--r--   0 vansh.singh   (502) staff       (20)       11 2024-05-09 21:48:23.000000 databricks_genai-1.0.1/databricks_genai.egg-info/top_level.txt
+-rw-r--r--   0 vansh.singh   (502) staff       (20)    31118 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/pyproject.toml
+-rw-r--r--   0 vansh.singh   (502) staff       (20)       38 2024-05-09 21:48:23.101918 databricks_genai-1.0.1/setup.cfg
+-rw-r--r--   0 vansh.singh   (502) staff       (20)     1778 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/setup.py
+drwxr-xr-x   0 vansh.singh   (502) staff       (20)        0 2024-05-09 21:48:23.099676 databricks_genai-1.0.1/tests/
+-rw-r--r--   0 vansh.singh   (502) staff       (20)      358 2024-05-09 21:04:20.000000 databricks_genai-1.0.1/tests/test_package.py
```

### Comparing `databricks_genai-1.0.0/PKG-INFO` & `databricks_genai-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-genai
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interact with the Databricks Generative AI APIs in python
 Home-page: https://docs.mosaicml.com/projects/mcli/en/latest/finetuning/finetuning.html
 Author: Databricks
 Author-email: genai-eng-team@databricks.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -28,15 +28,15 @@
 Requires-Dist: pylint>=3.0.0; extra == "dev"
 Requires-Dist: pyright==1.1.256; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: yapf>=0.40.0; extra == "dev"
 Provides-Extra: notebook
 Requires-Dist: ipywidgets<9,>=8; extra == "notebook"
 Provides-Extra: all
-Requires-Dist: isort>=5.9.3; extra == "all"
-Requires-Dist: packaging<23,>=21; extra == "all"
-Requires-Dist: pre-commit>=2.17.0; extra == "all"
 Requires-Dist: ipywidgets<9,>=8; extra == "all"
+Requires-Dist: pytest>=7.4.0; extra == "all"
+Requires-Dist: isort>=5.9.3; extra == "all"
 Requires-Dist: pylint>=3.0.0; extra == "all"
 Requires-Dist: pyright==1.1.256; extra == "all"
-Requires-Dist: pytest>=7.4.0; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
+Requires-Dist: packaging<23,>=21; extra == "all"
 Requires-Dist: yapf>=0.40.0; extra == "all"
```

### Comparing `databricks_genai-1.0.0/databricks/model_training/api/config.py` & `databricks_genai-1.0.1/databricks/model_training/api/config.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/databricks/model_training/api/engine/engine.py` & `databricks_genai-1.0.1/databricks/model_training/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/databricks/model_training/api/exceptions.py` & `databricks_genai-1.0.1/databricks/model_training/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/databricks/model_training/api/foundation_model/cancel.py` & `databricks_genai-1.0.1/databricks/model_training/api/foundation_model/cancel.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/databricks/model_training/api/foundation_model/create.py` & `databricks_genai-1.0.1/databricks/model_training/api/foundation_model/create.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/databricks/model_training/api/foundation_model/delete.py` & `databricks_genai-1.0.1/databricks/model_training/api/foundation_model/delete.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/databricks/model_training/api/foundation_model/get.py` & `databricks_genai-1.0.1/databricks/model_training/api/foundation_model/get.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/databricks/model_training/api/foundation_model/get_events.py` & `databricks_genai-1.0.1/databricks/model_training/api/foundation_model/get_events.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/databricks/model_training/api/foundation_model/list.py` & `databricks_genai-1.0.1/databricks/model_training/api/foundation_model/list.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/databricks/model_training/api/utils.py` & `databricks_genai-1.0.1/databricks/model_training/api/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -247,15 +247,23 @@
     print('Hugging Face dataset validation successful.')
 
 
 def validate_data_prep(data_prep_cluster: Optional[str] = None):
     if data_prep_cluster is None:
         raise ValidationError(
             'Providing a delta table for foundation_model data or eval data requires specifying a data_prep_cluster.')
-    user_has_access_to_cluster(data_prep_cluster)
+    if data_prep_cluster == 'serverless':
+        raise ValidationError('Serverless data preparation is not supported. Please provide a cluster ID.')
+    w = WorkspaceClient()
+    try:
+        w.clusters.get(cluster_id=data_prep_cluster)
+    except Exception as e:
+        raise ValidationError(
+            f'You do not have access to the cluster you provided: {data_prep_cluster}. Please try again with another '
+            'cluster.') from e
 
 
 def validate_custom_weights_path(custom_weights_path: str):
     mlflow_dbfs_path_prefix = 'dbfs:/databricks/mlflow-tracking/'
     # dbfs will be prepended before this if the user input `/databricks`
     mlflow_custom_weights_regex = (r'^dbfs:\/databricks\/mlflow-tracking'
                                    r'\/[0-9]+\/[0-9a-z]+\/artifacts($|\/[\/a-zA-Z0-9 ()_\\\-.]*$)')
@@ -269,26 +277,14 @@
     client = MlflowClient(tracking_uri='databricks')
     for artifact in client.list_artifacts(run_id, artifact_dir):
         if artifact.path == artifact_path:
             return
     raise ValidationError(f'Could not find file for custom_weights_path {custom_weights_path}')
 
 
-def user_has_access_to_cluster(cluster_id: str):
-    if cluster_id == 'serverless':
-        raise ValidationError('Serverless data preparation is not supported. Please provide a cluster ID.')
-    w = WorkspaceClient()
-    try:
-        w.clusters.get(cluster_id=cluster_id)
-    except Exception as e:
-        raise ValidationError(
-            f'You do not have access to the cluster you provided: {cluster_id}. Please try again with another cluster.'
-        ) from e
-
-
 def is_cluster_sql(cluster_id: str) -> bool:
     # Returns True if DBR version < 14.1 and requires SqlConnect
     # Returns False if DBR version >= 14.1 and can use DBConnect
     if cluster_id == 'serverless':
         return False
     w = WorkspaceClient()
     cluster: ClusterDetails = w.clusters.get(cluster_id=cluster_id)
@@ -308,41 +304,37 @@
 def validate_create_training_run_inputs(train_data_path: str,
                                         register_to: Optional[str] = None,
                                         experiment_path: Optional[str] = None,
                                         eval_data_path: Optional[str] = None,
                                         data_prep_cluster: Optional[str] = None,
                                         custom_weights_path: Optional[str] = None,
                                         task_type: TrainTaskType = TrainTaskType.INSTRUCTION_FINETUNE) -> None:
-    delta_table_used = False
-    validate_path(train_data_path, task_type, 'train_data_path')
+    validate_path_and_data_prep_cluster(train_data_path, task_type, 'train_data_path', data_prep_cluster)
     if register_to:
         validate_register_to(register_to)
     if experiment_path:
         validate_experiment_path(experiment_path)
-    if eval_data_path is None:
-        pass
-    else:
-        validate_path(eval_data_path, task_type, 'eval_data_path')
-    if delta_table_used:
-        validate_data_prep(data_prep_cluster)
+    if eval_data_path is not None:
+        validate_path_and_data_prep_cluster(eval_data_path, task_type, 'eval_data_path', data_prep_cluster)
     if custom_weights_path:
         validate_custom_weights_path(custom_weights_path)
 
 
 def format_path(path: str) -> str:
     """
     Prepends `dbfs:` in front of paths that start with `/Volumes` or `/databricks`.
     """
     if isinstance(path, str) and (path.startswith('/Volumes') or path.startswith('/databricks')):
         return f'dbfs:{path}'
     else:
         return path
 
 
-def validate_path(data_path: str, task_type: TrainTaskType, data_path_type: str) -> None:
+def validate_path_and_data_prep_cluster(data_path: str, task_type: TrainTaskType, data_path_type: str,
+                                        data_prep_cluster: str) -> None:
     """
     Validates the given data path in UC volume format, HF dataset format, or Delta table format.
 
     Args:
         data_path: The data path to validate.
         task_type: The training run task type.
         data_path_type: The type of data path, either 'train_data_path' or 'eval_data_path' for error messages.
@@ -351,8 +343,10 @@
         validate_uc_path(data_path, task_type)
     else:  # 'INSTRUCTION_FINETUNE' or 'CHAT_COMPLETION' tasks
         if data_path.startswith('dbfs:/'):
             validate_uc_path(data_path, task_type)
         elif '/' in data_path:  # assume HF dataset TODO state this assumption in docs
             validate_hf_dataset(data_path)
         else:
+            # if we have delta table input, we must also ensure the cluster input is valid
             validate_delta_table(data_path, data_path_type)
+            validate_data_prep(data_prep_cluster)
```

### Comparing `databricks_genai-1.0.0/databricks/model_training/types/common.py` & `databricks_genai-1.0.1/databricks/model_training/types/common.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/databricks/model_training/types/run_status.py` & `databricks_genai-1.0.1/databricks/model_training/types/run_status.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/databricks/model_training/types/train_config.py` & `databricks_genai-1.0.1/databricks/model_training/types/train_config.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/databricks/model_training/types/training_run.py` & `databricks_genai-1.0.1/databricks/model_training/types/training_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,15 @@
                     'Missing MLflow experimentTracker, which is a required field to deserialize TrainingRun object',
                 )
             mlflow_config = experiment_tracker.get('mlflow')
             args['register_to'] = mlflow_config.get('modelRegistryPath')
             args['experiment_path'] = mlflow_config.get('experimentPath')
             args['experiment_id'] = mlflow_config.get('mlflowExperimentId')
             args['run_id'] = mlflow_config.get('mlflowRunId')
+            args['task_type'] = details.get('taskType')
 
             config_copy = deepcopy(details)
             # Remove events from details to keep only config properties
             if 'formattedFinetuningEvents' in config_copy:
                 del config_copy['formattedFinetuningEvents']
 
             if 'dataPrepConfig' in config_copy:
```

### Comparing `databricks_genai-1.0.0/databricks_genai.egg-info/PKG-INFO` & `databricks_genai-1.0.1/databricks_genai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-genai
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interact with the Databricks Generative AI APIs in python
 Home-page: https://docs.mosaicml.com/projects/mcli/en/latest/finetuning/finetuning.html
 Author: Databricks
 Author-email: genai-eng-team@databricks.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -28,15 +28,15 @@
 Requires-Dist: pylint>=3.0.0; extra == "dev"
 Requires-Dist: pyright==1.1.256; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: yapf>=0.40.0; extra == "dev"
 Provides-Extra: notebook
 Requires-Dist: ipywidgets<9,>=8; extra == "notebook"
 Provides-Extra: all
-Requires-Dist: isort>=5.9.3; extra == "all"
-Requires-Dist: packaging<23,>=21; extra == "all"
-Requires-Dist: pre-commit>=2.17.0; extra == "all"
 Requires-Dist: ipywidgets<9,>=8; extra == "all"
+Requires-Dist: pytest>=7.4.0; extra == "all"
+Requires-Dist: isort>=5.9.3; extra == "all"
 Requires-Dist: pylint>=3.0.0; extra == "all"
 Requires-Dist: pyright==1.1.256; extra == "all"
-Requires-Dist: pytest>=7.4.0; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
+Requires-Dist: packaging<23,>=21; extra == "all"
 Requires-Dist: yapf>=0.40.0; extra == "all"
```

### Comparing `databricks_genai-1.0.0/databricks_genai.egg-info/SOURCES.txt` & `databricks_genai-1.0.1/databricks_genai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/pyproject.toml` & `databricks_genai-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.0/setup.py` & `databricks_genai-1.0.1/setup.py`

 * *Files identical despite different names*

