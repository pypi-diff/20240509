# Comparing `tmp/dagster-datahub-0.23.4.tar.gz` & `tmp/dagster-datahub-0.23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-datahub-0.23.4.tar", last modified: Thu May  2 20:43:47 2024, max compression
+gzip compressed data, was "dagster-datahub-0.23.5.tar", last modified: Thu May  9 17:55:22 2024, max compression
```

## Comparing `dagster-datahub-0.23.4.tar` & `dagster-datahub-0.23.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:47.126856 dagster-datahub-0.23.4/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-02 20:31:41.000000 dagster-datahub-0.23.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      214 2024-05-02 20:31:41.000000 dagster-datahub-0.23.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      740 2024-05-02 20:43:47.130856 dagster-datahub-0.23.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-05-02 20:31:41.000000 dagster-datahub-0.23.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:47.126856 dagster-datahub-0.23.4/dagster_datahub/
--rw-r--r--   0 root         (0) root         (0)      492 2024-05-02 20:31:41.000000 dagster-datahub-0.23.4/dagster_datahub/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:41.000000 dagster-datahub-0.23.4/dagster_datahub/py.typed
--rw-r--r--   0 root         (0) root         (0)     4225 2024-05-02 20:31:41.000000 dagster-datahub-0.23.4/dagster_datahub/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-02 20:31:41.000000 dagster-datahub-0.23.4/dagster_datahub/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:47.126856 dagster-datahub-0.23.4/dagster_datahub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      740 2024-05-02 20:43:46.000000 dagster-datahub-0.23.4/dagster_datahub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2024-05-02 20:43:46.000000 dagster-datahub-0.23.4/dagster_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:43:46.000000 dagster-datahub-0.23.4/dagster_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:43:46.000000 dagster-datahub-0.23.4/dagster_datahub.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-02 20:43:46.000000 dagster-datahub-0.23.4/dagster_datahub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-02 20:43:46.000000 dagster-datahub-0.23.4/dagster_datahub.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-05-02 20:43:47.134856 dagster-datahub-0.23.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1543 2024-05-02 20:31:41.000000 dagster-datahub-0.23.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:22.272081 dagster-datahub-0.23.5/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-09 17:47:35.000000 dagster-datahub-0.23.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      214 2024-05-09 17:47:35.000000 dagster-datahub-0.23.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      740 2024-05-09 17:55:22.272081 dagster-datahub-0.23.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-05-09 17:47:35.000000 dagster-datahub-0.23.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:22.268081 dagster-datahub-0.23.5/dagster_datahub/
+-rw-r--r--   0 root         (0) root         (0)      492 2024-05-09 17:47:35.000000 dagster-datahub-0.23.5/dagster_datahub/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-datahub-0.23.5/dagster_datahub/py.typed
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-05-09 17:47:35.000000 dagster-datahub-0.23.5/dagster_datahub/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-09 17:47:35.000000 dagster-datahub-0.23.5/dagster_datahub/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:22.272081 dagster-datahub-0.23.5/dagster_datahub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      740 2024-05-09 17:55:22.000000 dagster-datahub-0.23.5/dagster_datahub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2024-05-09 17:55:22.000000 dagster-datahub-0.23.5/dagster_datahub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:55:22.000000 dagster-datahub-0.23.5/dagster_datahub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:55:22.000000 dagster-datahub-0.23.5/dagster_datahub.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-09 17:55:22.000000 dagster-datahub-0.23.5/dagster_datahub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-09 17:55:22.000000 dagster-datahub-0.23.5/dagster_datahub.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-05-09 17:55:22.272081 dagster-datahub-0.23.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1543 2024-05-09 17:47:35.000000 dagster-datahub-0.23.5/setup.py
```

### Comparing `dagster-datahub-0.23.4/LICENSE` & `dagster-datahub-0.23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-datahub-0.23.4/PKG-INFO` & `dagster-datahub-0.23.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.23.4
+Version: 0.23.5
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-datahub-0.23.4/dagster_datahub/resources.py` & `dagster-datahub-0.23.5/dagster_datahub/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-datahub-0.23.4/dagster_datahub.egg-info/PKG-INFO` & `dagster-datahub-0.23.5/dagster_datahub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.23.4
+Version: 0.23.5
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-datahub-0.23.4/setup.py` & `dagster-datahub-0.23.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_datahub_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
         "acryl-datahub[datahub-rest, datahub-kafka]",
-        "dagster==1.7.4",
+        "dagster==1.7.5",
         "packaging",
         "requests",
         "pydantic>=1.10.0,<2.0.0",
     ],
     extras_require={},
     zip_safe=False,
 )
```

