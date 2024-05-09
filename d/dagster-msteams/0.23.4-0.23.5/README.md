# Comparing `tmp/dagster-msteams-0.23.4.tar.gz` & `tmp/dagster-msteams-0.23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-msteams-0.23.4.tar", last modified: Thu May  2 20:39:34 2024, max compression
+gzip compressed data, was "dagster-msteams-0.23.5.tar", last modified: Thu May  9 17:57:13 2024, max compression
```

## Comparing `dagster-msteams-0.23.4.tar` & `dagster-msteams-0.23.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:39:34.293155 dagster-msteams-0.23.4/
--rw-r--r--   0 root         (0) root         (0)    11348 2024-05-02 20:31:41.000000 dagster-msteams-0.23.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-02 20:31:41.000000 dagster-msteams-0.23.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      727 2024-05-02 20:39:34.293155 dagster-msteams-0.23.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-05-02 20:31:41.000000 dagster-msteams-0.23.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:39:34.293155 dagster-msteams-0.23.4/dagster_msteams/
--rw-r--r--   0 root         (0) root         (0)      510 2024-05-02 20:31:41.000000 dagster-msteams-0.23.4/dagster_msteams/__init__.py
--rw-r--r--   0 root         (0) root         (0)      849 2024-05-02 20:31:41.000000 dagster-msteams-0.23.4/dagster_msteams/card.py
--rw-r--r--   0 root         (0) root         (0)     1389 2024-05-02 20:31:41.000000 dagster-msteams-0.23.4/dagster_msteams/client.py
--rw-r--r--   0 root         (0) root         (0)     5109 2024-05-02 20:31:41.000000 dagster-msteams-0.23.4/dagster_msteams/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-02 20:31:41.000000 dagster-msteams-0.23.4/dagster_msteams/py.typed
--rw-r--r--   0 root         (0) root         (0)     3778 2024-05-02 20:31:41.000000 dagster-msteams-0.23.4/dagster_msteams/resources.py
--rw-r--r--   0 root         (0) root         (0)     6264 2024-05-02 20:31:41.000000 dagster-msteams-0.23.4/dagster_msteams/sensors.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-02 20:31:41.000000 dagster-msteams-0.23.4/dagster_msteams/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:39:34.293155 dagster-msteams-0.23.4/dagster_msteams.egg-info/
--rw-r--r--   0 root         (0) root         (0)      727 2024-05-02 20:39:34.000000 dagster-msteams-0.23.4/dagster_msteams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2024-05-02 20:39:34.000000 dagster-msteams-0.23.4/dagster_msteams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:39:34.000000 dagster-msteams-0.23.4/dagster_msteams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:39:34.000000 dagster-msteams-0.23.4/dagster_msteams.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-02 20:39:34.000000 dagster-msteams-0.23.4/dagster_msteams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-02 20:39:34.000000 dagster-msteams-0.23.4/dagster_msteams.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-05-02 20:39:34.293155 dagster-msteams-0.23.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1335 2024-05-02 20:31:41.000000 dagster-msteams-0.23.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:57:13.560153 dagster-msteams-0.23.5/
+-rw-r--r--   0 root         (0) root         (0)    11348 2024-05-09 17:47:35.000000 dagster-msteams-0.23.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-09 17:47:35.000000 dagster-msteams-0.23.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-09 17:57:13.560153 dagster-msteams-0.23.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-05-09 17:47:35.000000 dagster-msteams-0.23.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:57:13.560153 dagster-msteams-0.23.5/dagster_msteams/
+-rw-r--r--   0 root         (0) root         (0)      510 2024-05-09 17:47:35.000000 dagster-msteams-0.23.5/dagster_msteams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      849 2024-05-09 17:47:35.000000 dagster-msteams-0.23.5/dagster_msteams/card.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2024-05-09 17:47:35.000000 dagster-msteams-0.23.5/dagster_msteams/client.py
+-rw-r--r--   0 root         (0) root         (0)     5109 2024-05-09 17:47:35.000000 dagster-msteams-0.23.5/dagster_msteams/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:47:35.000000 dagster-msteams-0.23.5/dagster_msteams/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3778 2024-05-09 17:47:35.000000 dagster-msteams-0.23.5/dagster_msteams/resources.py
+-rw-r--r--   0 root         (0) root         (0)     6264 2024-05-09 17:47:35.000000 dagster-msteams-0.23.5/dagster_msteams/sensors.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-09 17:47:35.000000 dagster-msteams-0.23.5/dagster_msteams/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:57:13.560153 dagster-msteams-0.23.5/dagster_msteams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-09 17:57:13.000000 dagster-msteams-0.23.5/dagster_msteams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2024-05-09 17:57:13.000000 dagster-msteams-0.23.5/dagster_msteams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:57:13.000000 dagster-msteams-0.23.5/dagster_msteams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:57:13.000000 dagster-msteams-0.23.5/dagster_msteams.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-09 17:57:13.000000 dagster-msteams-0.23.5/dagster_msteams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-09 17:57:13.000000 dagster-msteams-0.23.5/dagster_msteams.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-05-09 17:57:13.564153 dagster-msteams-0.23.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1335 2024-05-09 17:47:35.000000 dagster-msteams-0.23.5/setup.py
```

### Comparing `dagster-msteams-0.23.4/LICENSE` & `dagster-msteams-0.23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.23.4/PKG-INFO` & `dagster-msteams-0.23.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.23.4
+Version: 0.23.5
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-msteams-0.23.4/dagster_msteams/card.py` & `dagster-msteams-0.23.5/dagster_msteams/card.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.23.4/dagster_msteams/client.py` & `dagster-msteams-0.23.5/dagster_msteams/client.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.23.4/dagster_msteams/hooks.py` & `dagster-msteams-0.23.5/dagster_msteams/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.23.4/dagster_msteams/resources.py` & `dagster-msteams-0.23.5/dagster_msteams/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.23.4/dagster_msteams/sensors.py` & `dagster-msteams-0.23.5/dagster_msteams/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.23.4/dagster_msteams.egg-info/PKG-INFO` & `dagster-msteams-0.23.5/dagster_msteams.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.23.4
+Version: 0.23.5
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-msteams-0.23.4/setup.py` & `dagster-msteams-0.23.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,12 +32,12 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_msteams_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.4",
+        "dagster==1.7.5",
         "requests>=2,<3",
     ],
     zip_safe=False,
 )
```

