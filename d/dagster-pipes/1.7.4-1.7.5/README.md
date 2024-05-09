# Comparing `tmp/dagster-pipes-1.7.4.tar.gz` & `tmp/dagster-pipes-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-pipes-1.7.4.tar", last modified: Thu May  2 20:32:29 2024, max compression
+gzip compressed data, was "dagster-pipes-1.7.5.tar", last modified: Thu May  9 17:48:20 2024, max compression
```

## Comparing `dagster-pipes-1.7.4.tar` & `dagster-pipes-1.7.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:29.645032 dagster-pipes-1.7.4/
--rw-r--r--   0 root         (0) root         (0)    11348 2024-05-02 20:31:40.000000 dagster-pipes-1.7.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 20:31:40.000000 dagster-pipes-1.7.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      794 2024-05-02 20:32:29.645032 dagster-pipes-1.7.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      125 2024-05-02 20:31:40.000000 dagster-pipes-1.7.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:29.645032 dagster-pipes-1.7.4/dagster_pipes/
--rw-r--r--   0 root         (0) root         (0)    48159 2024-05-02 20:31:40.000000 dagster-pipes-1.7.4/dagster_pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-02 20:31:40.000000 dagster-pipes-1.7.4/dagster_pipes/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-02 20:31:40.000000 dagster-pipes-1.7.4/dagster_pipes/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:29.645032 dagster-pipes-1.7.4/dagster_pipes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      794 2024-05-02 20:32:29.000000 dagster-pipes-1.7.4/dagster_pipes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-02 20:32:29.000000 dagster-pipes-1.7.4/dagster_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:32:29.000000 dagster-pipes-1.7.4/dagster_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:32:29.000000 dagster-pipes-1.7.4/dagster_pipes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-02 20:32:29.000000 dagster-pipes-1.7.4/dagster_pipes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2024-05-02 20:32:29.645032 dagster-pipes-1.7.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1313 2024-05-02 20:31:40.000000 dagster-pipes-1.7.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:20.255758 dagster-pipes-1.7.5/
+-rw-r--r--   0 root         (0) root         (0)    11348 2024-05-09 17:47:35.000000 dagster-pipes-1.7.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-09 17:47:35.000000 dagster-pipes-1.7.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      794 2024-05-09 17:48:20.255758 dagster-pipes-1.7.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-09 17:47:35.000000 dagster-pipes-1.7.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:20.255758 dagster-pipes-1.7.5/dagster_pipes/
+-rw-r--r--   0 root         (0) root         (0)    48159 2024-05-09 17:47:35.000000 dagster-pipes-1.7.5/dagster_pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-09 17:47:35.000000 dagster-pipes-1.7.5/dagster_pipes/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 17:47:35.000000 dagster-pipes-1.7.5/dagster_pipes/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:20.255758 dagster-pipes-1.7.5/dagster_pipes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      794 2024-05-09 17:48:20.000000 dagster-pipes-1.7.5/dagster_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-09 17:48:20.000000 dagster-pipes-1.7.5/dagster_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:48:20.000000 dagster-pipes-1.7.5/dagster_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:48:20.000000 dagster-pipes-1.7.5/dagster_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-09 17:48:20.000000 dagster-pipes-1.7.5/dagster_pipes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2024-05-09 17:48:20.259758 dagster-pipes-1.7.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1313 2024-05-09 17:47:35.000000 dagster-pipes-1.7.5/setup.py
```

### Comparing `dagster-pipes-1.7.4/LICENSE` & `dagster-pipes-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pipes-1.7.4/PKG-INFO` & `dagster-pipes-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pipes
-Version: 1.7.4
+Version: 1.7.5
 Summary: Toolkit for Dagster integrations with transform logic outside of Dagster
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-pipes
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pipes-1.7.4/dagster_pipes/__init__.py` & `dagster-pipes-1.7.5/dagster_pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-pipes-1.7.4/dagster_pipes.egg-info/PKG-INFO` & `dagster-pipes-1.7.5/dagster_pipes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pipes
-Version: 1.7.4
+Version: 1.7.5
 Summary: Toolkit for Dagster integrations with transform logic outside of Dagster
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-pipes
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pipes-1.7.4/setup.py` & `dagster-pipes-1.7.5/setup.py`

 * *Files identical despite different names*

