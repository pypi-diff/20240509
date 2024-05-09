# Comparing `tmp/dagster-deltalake-polars-0.23.4.tar.gz` & `tmp/dagster-deltalake-polars-0.23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-deltalake-polars-0.23.4.tar", last modified: Thu May  2 20:43:42 2024, max compression
+gzip compressed data, was "dagster-deltalake-polars-0.23.5.tar", last modified: Thu May  9 17:55:35 2024, max compression
```

## Comparing `dagster-deltalake-polars-0.23.4.tar` & `dagster-deltalake-polars-0.23.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:42.026902 dagster-deltalake-polars-0.23.4/
--rw-r--r--   0 root         (0) root         (0)    11344 2024-05-02 20:31:41.000000 dagster-deltalake-polars-0.23.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-02 20:31:41.000000 dagster-deltalake-polars-0.23.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      778 2024-05-02 20:43:42.026902 dagster-deltalake-polars-0.23.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2024-05-02 20:31:41.000000 dagster-deltalake-polars-0.23.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:42.026902 dagster-deltalake-polars-0.23.4/dagster_deltalake_polars/
--rw-r--r--   0 root         (0) root         (0)      334 2024-05-02 20:31:41.000000 dagster-deltalake-polars-0.23.4/dagster_deltalake_polars/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2617 2024-05-02 20:31:41.000000 dagster-deltalake-polars-0.23.4/dagster_deltalake_polars/deltalake_polars_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:41.000000 dagster-deltalake-polars-0.23.4/dagster_deltalake_polars/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-02 20:31:41.000000 dagster-deltalake-polars-0.23.4/dagster_deltalake_polars/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:42.026902 dagster-deltalake-polars-0.23.4/dagster_deltalake_polars.egg-info/
--rw-r--r--   0 root         (0) root         (0)      778 2024-05-02 20:43:41.000000 dagster-deltalake-polars-0.23.4/dagster_deltalake_polars.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-05-02 20:43:41.000000 dagster-deltalake-polars-0.23.4/dagster_deltalake_polars.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:43:41.000000 dagster-deltalake-polars-0.23.4/dagster_deltalake_polars.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:43:41.000000 dagster-deltalake-polars-0.23.4/dagster_deltalake_polars.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       57 2024-05-02 20:43:41.000000 dagster-deltalake-polars-0.23.4/dagster_deltalake_polars.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-02 20:43:41.000000 dagster-deltalake-polars-0.23.4/dagster_deltalake_polars.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      135 2024-05-02 20:43:42.026902 dagster-deltalake-polars-0.23.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1493 2024-05-02 20:31:41.000000 dagster-deltalake-polars-0.23.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:35.888090 dagster-deltalake-polars-0.23.5/
+-rw-r--r--   0 root         (0) root         (0)    11344 2024-05-09 17:47:35.000000 dagster-deltalake-polars-0.23.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-09 17:47:35.000000 dagster-deltalake-polars-0.23.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      778 2024-05-09 17:55:35.888090 dagster-deltalake-polars-0.23.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      158 2024-05-09 17:47:35.000000 dagster-deltalake-polars-0.23.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:35.888090 dagster-deltalake-polars-0.23.5/dagster_deltalake_polars/
+-rw-r--r--   0 root         (0) root         (0)      334 2024-05-09 17:47:35.000000 dagster-deltalake-polars-0.23.5/dagster_deltalake_polars/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2024-05-09 17:47:35.000000 dagster-deltalake-polars-0.23.5/dagster_deltalake_polars/deltalake_polars_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-deltalake-polars-0.23.5/dagster_deltalake_polars/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-09 17:47:35.000000 dagster-deltalake-polars-0.23.5/dagster_deltalake_polars/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:35.888090 dagster-deltalake-polars-0.23.5/dagster_deltalake_polars.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      778 2024-05-09 17:55:35.000000 dagster-deltalake-polars-0.23.5/dagster_deltalake_polars.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-09 17:55:35.000000 dagster-deltalake-polars-0.23.5/dagster_deltalake_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:55:35.000000 dagster-deltalake-polars-0.23.5/dagster_deltalake_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:55:35.000000 dagster-deltalake-polars-0.23.5/dagster_deltalake_polars.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-09 17:55:35.000000 dagster-deltalake-polars-0.23.5/dagster_deltalake_polars.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-09 17:55:35.000000 dagster-deltalake-polars-0.23.5/dagster_deltalake_polars.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2024-05-09 17:55:35.888090 dagster-deltalake-polars-0.23.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-05-09 17:47:35.000000 dagster-deltalake-polars-0.23.5/setup.py
```

### Comparing `dagster-deltalake-polars-0.23.4/LICENSE` & `dagster-deltalake-polars-0.23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-polars-0.23.4/PKG-INFO` & `dagster-deltalake-polars-0.23.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake-polars
-Version: 0.23.4
+Version: 0.23.5
 Summary: Package for storing Polars DataFrames in Delta tables.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake-polars
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-polars-0.23.4/dagster_deltalake_polars/deltalake_polars_type_handler.py` & `dagster-deltalake-polars-0.23.5/dagster_deltalake_polars/deltalake_polars_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-polars-0.23.4/dagster_deltalake_polars.egg-info/PKG-INFO` & `dagster-deltalake-polars-0.23.5/dagster_deltalake_polars.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake-polars
-Version: 0.23.4
+Version: 0.23.5
 Summary: Package for storing Polars DataFrames in Delta tables.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake-polars
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-polars-0.23.4/setup.py` & `dagster-deltalake-polars-0.23.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,13 +33,13 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_deltalake_polars_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.4",
-        "dagster-deltalake==0.23.4",
+        "dagster==1.7.5",
+        "dagster-deltalake==0.23.5",
         "polars[pyarrow]",
     ],
     zip_safe=False,
 )
```

