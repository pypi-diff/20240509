# Comparing `tmp/dagster-airbyte-0.23.4.tar.gz` & `tmp/dagster-airbyte-0.23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airbyte-0.23.4.tar", last modified: Thu May  2 20:43:30 2024, max compression
+gzip compressed data, was "dagster-airbyte-0.23.5.tar", last modified: Thu May  9 17:56:26 2024, max compression
```

## Comparing `dagster-airbyte-0.23.4.tar` & `dagster-airbyte-0.23.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:30.167010 dagster-airbyte-0.23.4/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      753 2024-05-02 20:43:30.167010 dagster-airbyte-0.23.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:30.147010 dagster-airbyte-0.23.4/dagster_airbyte/
--rw-r--r--   0 root         (0) root         (0)     1215 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48304 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      425 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:30.159010 dagster-airbyte-0.23.4/dagster_airbyte/managed/
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/managed/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:30.163010 dagster-airbyte-0.23.4/dagster_airbyte/managed/generated/
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/managed/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119751 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/managed/generated/destinations.py
--rw-r--r--   0 root         (0) root         (0)   282772 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/managed/generated/sources.py
--rw-r--r--   0 root         (0) root         (0)    34862 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)    14588 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     4128 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/py.typed
--rw-r--r--   0 root         (0) root         (0)    27040 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/resources.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/types.py
--rw-r--r--   0 root         (0) root         (0)     2823 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/dagster_airbyte/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:30.151010 dagster-airbyte-0.23.4/dagster_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)      753 2024-05-02 20:43:29.000000 dagster-airbyte-0.23.4/dagster_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      809 2024-05-02 20:43:30.000000 dagster-airbyte-0.23.4/dagster_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:43:29.000000 dagster-airbyte-0.23.4/dagster_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-05-02 20:43:29.000000 dagster-airbyte-0.23.4/dagster_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:43:29.000000 dagster-airbyte-0.23.4/dagster_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-02 20:43:29.000000 dagster-airbyte-0.23.4/dagster_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-02 20:43:29.000000 dagster-airbyte-0.23.4/dagster_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-05-02 20:43:30.171010 dagster-airbyte-0.23.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1636 2024-05-02 20:31:40.000000 dagster-airbyte-0.23.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:56:26.528126 dagster-airbyte-0.23.5/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-09 17:56:26.528126 dagster-airbyte-0.23.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:56:26.520126 dagster-airbyte-0.23.5/dagster_airbyte/
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48304 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)      425 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:56:26.520126 dagster-airbyte-0.23.5/dagster_airbyte/managed/
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/managed/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:56:26.528126 dagster-airbyte-0.23.5/dagster_airbyte/managed/generated/
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/managed/generated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   119751 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/managed/generated/destinations.py
+-rw-r--r--   0 root         (0) root         (0)   282772 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/managed/generated/sources.py
+-rw-r--r--   0 root         (0) root         (0)    34862 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/managed/reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)    14588 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/managed/types.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/py.typed
+-rw-r--r--   0 root         (0) root         (0)    27040 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/types.py
+-rw-r--r--   0 root         (0) root         (0)     2823 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/dagster_airbyte/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:56:26.520126 dagster-airbyte-0.23.5/dagster_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-09 17:56:26.000000 dagster-airbyte-0.23.5/dagster_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      809 2024-05-09 17:56:26.000000 dagster-airbyte-0.23.5/dagster_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:56:26.000000 dagster-airbyte-0.23.5/dagster_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-05-09 17:56:26.000000 dagster-airbyte-0.23.5/dagster_airbyte.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:56:26.000000 dagster-airbyte-0.23.5/dagster_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-09 17:56:26.000000 dagster-airbyte-0.23.5/dagster_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-09 17:56:26.000000 dagster-airbyte-0.23.5/dagster_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-05-09 17:56:26.532126 dagster-airbyte-0.23.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1636 2024-05-09 17:47:35.000000 dagster-airbyte-0.23.5/setup.py
```

### Comparing `dagster-airbyte-0.23.4/LICENSE` & `dagster-airbyte-0.23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.4/PKG-INFO` & `dagster-airbyte-0.23.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.23.4
+Version: 0.23.5
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.23.4/dagster_airbyte/__init__.py` & `dagster-airbyte-0.23.5/dagster_airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.4/dagster_airbyte/asset_defs.py` & `dagster-airbyte-0.23.5/dagster_airbyte/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.4/dagster_airbyte/managed/generated/destinations.py` & `dagster-airbyte-0.23.5/dagster_airbyte/managed/generated/destinations.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.4/dagster_airbyte/managed/generated/sources.py` & `dagster-airbyte-0.23.5/dagster_airbyte/managed/generated/sources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.4/dagster_airbyte/managed/reconciliation.py` & `dagster-airbyte-0.23.5/dagster_airbyte/managed/reconciliation.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.4/dagster_airbyte/managed/types.py` & `dagster-airbyte-0.23.5/dagster_airbyte/managed/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.4/dagster_airbyte/ops.py` & `dagster-airbyte-0.23.5/dagster_airbyte/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.4/dagster_airbyte/resources.py` & `dagster-airbyte-0.23.5/dagster_airbyte/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.4/dagster_airbyte/types.py` & `dagster-airbyte-0.23.5/dagster_airbyte/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.4/dagster_airbyte/utils.py` & `dagster-airbyte-0.23.5/dagster_airbyte/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.4/dagster_airbyte.egg-info/PKG-INFO` & `dagster-airbyte-0.23.5/dagster_airbyte.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.23.4
+Version: 0.23.5
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.23.4/dagster_airbyte.egg-info/SOURCES.txt` & `dagster-airbyte-0.23.5/dagster_airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.4/setup.py` & `dagster-airbyte-0.23.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,25 +33,25 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airbyte_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.4",
+        "dagster==1.7.5",
         "requests",
     ],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-airbyte = dagster_airbyte.cli:main",
         ]
     },
     extras_require={
         "test": [
             "requests-mock",
         ],
         "managed": [
-            "dagster-managed-elements==0.23.4",
+            "dagster-managed-elements==0.23.5",
         ],
     },
 )
```
