# Comparing `tmp/dagster-mlflow-0.23.4.tar.gz` & `tmp/dagster-mlflow-0.23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mlflow-0.23.4.tar", last modified: Thu May  2 20:40:30 2024, max compression
+gzip compressed data, was "dagster-mlflow-0.23.5.tar", last modified: Thu May  9 17:55:15 2024, max compression
```

## Comparing `dagster-mlflow-0.23.4.tar` & `dagster-mlflow-0.23.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:40:30.744641 dagster-mlflow-0.23.4/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-02 20:31:41.000000 dagster-mlflow-0.23.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-02 20:31:41.000000 dagster-mlflow-0.23.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      607 2024-05-02 20:40:30.744641 dagster-mlflow-0.23.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2024-05-02 20:31:41.000000 dagster-mlflow-0.23.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:40:30.744641 dagster-mlflow-0.23.4/dagster_mlflow/
--rw-r--r--   0 root         (0) root         (0)      303 2024-05-02 20:31:41.000000 dagster-mlflow-0.23.4/dagster_mlflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-05-02 20:31:41.000000 dagster-mlflow-0.23.4/dagster_mlflow/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-02 20:31:41.000000 dagster-mlflow-0.23.4/dagster_mlflow/py.typed
--rw-r--r--   0 root         (0) root         (0)    10924 2024-05-02 20:31:41.000000 dagster-mlflow-0.23.4/dagster_mlflow/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-02 20:31:41.000000 dagster-mlflow-0.23.4/dagster_mlflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:40:30.744641 dagster-mlflow-0.23.4/dagster_mlflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      607 2024-05-02 20:40:30.000000 dagster-mlflow-0.23.4/dagster_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      403 2024-05-02 20:40:30.000000 dagster-mlflow-0.23.4/dagster_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:40:30.000000 dagster-mlflow-0.23.4/dagster_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:40:30.000000 dagster-mlflow-0.23.4/dagster_mlflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-02 20:40:30.000000 dagster-mlflow-0.23.4/dagster_mlflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-02 20:40:30.000000 dagster-mlflow-0.23.4/dagster_mlflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-02 20:40:30.748641 dagster-mlflow-0.23.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1225 2024-05-02 20:31:41.000000 dagster-mlflow-0.23.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:15.880077 dagster-mlflow-0.23.5/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-09 17:47:35.000000 dagster-mlflow-0.23.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-09 17:47:35.000000 dagster-mlflow-0.23.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      607 2024-05-09 17:55:15.880077 dagster-mlflow-0.23.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2024-05-09 17:47:35.000000 dagster-mlflow-0.23.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:15.880077 dagster-mlflow-0.23.5/dagster_mlflow/
+-rw-r--r--   0 root         (0) root         (0)      303 2024-05-09 17:47:35.000000 dagster-mlflow-0.23.5/dagster_mlflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-05-09 17:47:35.000000 dagster-mlflow-0.23.5/dagster_mlflow/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:47:35.000000 dagster-mlflow-0.23.5/dagster_mlflow/py.typed
+-rw-r--r--   0 root         (0) root         (0)    10924 2024-05-09 17:47:35.000000 dagster-mlflow-0.23.5/dagster_mlflow/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-09 17:47:35.000000 dagster-mlflow-0.23.5/dagster_mlflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:15.880077 dagster-mlflow-0.23.5/dagster_mlflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      607 2024-05-09 17:55:15.000000 dagster-mlflow-0.23.5/dagster_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      403 2024-05-09 17:55:15.000000 dagster-mlflow-0.23.5/dagster_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:55:15.000000 dagster-mlflow-0.23.5/dagster_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:55:15.000000 dagster-mlflow-0.23.5/dagster_mlflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-09 17:55:15.000000 dagster-mlflow-0.23.5/dagster_mlflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-09 17:55:15.000000 dagster-mlflow-0.23.5/dagster_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-09 17:55:15.884076 dagster-mlflow-0.23.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-05-09 17:47:35.000000 dagster-mlflow-0.23.5/setup.py
```

### Comparing `dagster-mlflow-0.23.4/LICENSE` & `dagster-mlflow-0.23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.23.4/PKG-INFO` & `dagster-mlflow-0.23.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.23.4
+Version: 0.23.5
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mlflow-0.23.4/dagster_mlflow/hooks.py` & `dagster-mlflow-0.23.5/dagster_mlflow/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.23.4/dagster_mlflow/resources.py` & `dagster-mlflow-0.23.5/dagster_mlflow/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.23.4/dagster_mlflow.egg-info/PKG-INFO` & `dagster-mlflow-0.23.5/dagster_mlflow.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.23.4
+Version: 0.23.5
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mlflow-0.23.4/setup.py` & `dagster-mlflow-0.23.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,10 +28,10 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_mlflow_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.4", "mlflow", "pandas"],
+    install_requires=["dagster==1.7.5", "mlflow", "pandas"],
     zip_safe=False,
 )
```

