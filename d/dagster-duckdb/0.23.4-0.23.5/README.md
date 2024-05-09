# Comparing `tmp/dagster-duckdb-0.23.4.tar.gz` & `tmp/dagster-duckdb-0.23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-0.23.4.tar", last modified: Thu May  2 20:43:21 2024, max compression
+gzip compressed data, was "dagster-duckdb-0.23.5.tar", last modified: Thu May  9 17:54:11 2024, max compression
```

## Comparing `dagster-duckdb-0.23.4.tar` & `dagster-duckdb-0.23.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:21.511088 dagster-duckdb-0.23.4/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-02 20:31:41.000000 dagster-duckdb-0.23.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-02 20:31:41.000000 dagster-duckdb-0.23.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-02 20:43:21.511088 dagster-duckdb-0.23.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2024-05-02 20:31:41.000000 dagster-duckdb-0.23.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:21.511088 dagster-duckdb-0.23.4/dagster_duckdb/
--rw-r--r--   0 root         (0) root         (0)      336 2024-05-02 20:31:41.000000 dagster-duckdb-0.23.4/dagster_duckdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12026 2024-05-02 20:31:41.000000 dagster-duckdb-0.23.4/dagster_duckdb/io_manager.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-02 20:31:41.000000 dagster-duckdb-0.23.4/dagster_duckdb/py.typed
--rw-r--r--   0 root         (0) root         (0)     1716 2024-05-02 20:31:41.000000 dagster-duckdb-0.23.4/dagster_duckdb/resource.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-02 20:31:41.000000 dagster-duckdb-0.23.4/dagster_duckdb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:21.511088 dagster-duckdb-0.23.4/dagster_duckdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-02 20:43:21.000000 dagster-duckdb-0.23.4/dagster_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-02 20:43:21.000000 dagster-duckdb-0.23.4/dagster_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:43:21.000000 dagster-duckdb-0.23.4/dagster_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:43:21.000000 dagster-duckdb-0.23.4/dagster_duckdb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 20:43:21.000000 dagster-duckdb-0.23.4/dagster_duckdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-02 20:43:21.000000 dagster-duckdb-0.23.4/dagster_duckdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      125 2024-05-02 20:43:21.515088 dagster-duckdb-0.23.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1545 2024-05-02 20:31:41.000000 dagster-duckdb-0.23.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:54:11.468031 dagster-duckdb-0.23.5/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-09 17:47:35.000000 dagster-duckdb-0.23.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-09 17:47:35.000000 dagster-duckdb-0.23.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-09 17:54:11.468031 dagster-duckdb-0.23.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2024-05-09 17:47:35.000000 dagster-duckdb-0.23.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:54:11.468031 dagster-duckdb-0.23.5/dagster_duckdb/
+-rw-r--r--   0 root         (0) root         (0)      336 2024-05-09 17:47:35.000000 dagster-duckdb-0.23.5/dagster_duckdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12026 2024-05-09 17:47:35.000000 dagster-duckdb-0.23.5/dagster_duckdb/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-09 17:47:35.000000 dagster-duckdb-0.23.5/dagster_duckdb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-05-09 17:47:35.000000 dagster-duckdb-0.23.5/dagster_duckdb/resource.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-09 17:47:35.000000 dagster-duckdb-0.23.5/dagster_duckdb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:54:11.468031 dagster-duckdb-0.23.5/dagster_duckdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-09 17:54:11.000000 dagster-duckdb-0.23.5/dagster_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-09 17:54:11.000000 dagster-duckdb-0.23.5/dagster_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:54:11.000000 dagster-duckdb-0.23.5/dagster_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:54:11.000000 dagster-duckdb-0.23.5/dagster_duckdb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-09 17:54:11.000000 dagster-duckdb-0.23.5/dagster_duckdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-09 17:54:11.000000 dagster-duckdb-0.23.5/dagster_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-09 17:54:11.472031 dagster-duckdb-0.23.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-05-09 17:47:35.000000 dagster-duckdb-0.23.5/setup.py
```

### Comparing `dagster-duckdb-0.23.4/LICENSE` & `dagster-duckdb-0.23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.23.4/PKG-INFO` & `dagster-duckdb-0.23.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.23.4
+Version: 0.23.5
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-0.23.4/dagster_duckdb/io_manager.py` & `dagster-duckdb-0.23.5/dagster_duckdb/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.23.4/dagster_duckdb/resource.py` & `dagster-duckdb-0.23.5/dagster_duckdb/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.23.4/dagster_duckdb.egg-info/PKG-INFO` & `dagster-duckdb-0.23.5/dagster_duckdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.23.4
+Version: 0.23.5
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-0.23.4/setup.py` & `dagster-duckdb-0.23.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
         "duckdb",
-        "dagster==1.7.4",
+        "dagster==1.7.5",
     ],
     extras_require={
         "pandas": [
             # Pinned pending duckdb removal of broken pandas import. Pin can be
             # removed as soon as it produces a working build.
             "pandas<2.1",
         ],
```
