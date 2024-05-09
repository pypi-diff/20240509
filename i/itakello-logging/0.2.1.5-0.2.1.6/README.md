# Comparing `tmp/itakello_logging-0.2.1.5.tar.gz` & `tmp/itakello_logging-0.2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itakello_logging-0.2.1.5.tar", last modified: Mon Apr 29 16:54:27 2024, max compression
+gzip compressed data, was "itakello_logging-0.2.1.6.tar", last modified: Thu May  9 12:54:12 2024, max compression
```

## Comparing `itakello_logging-0.2.1.5.tar` & `itakello_logging-0.2.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:54:27.839011 itakello_logging-0.2.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-29 16:54:27.839011 itakello_logging-0.2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:54:27.839011 itakello_logging-0.2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:54:27.835011 itakello_logging-0.2.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:54:27.835011 itakello_logging-0.2.1.5/src/itakello_logging/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/src/itakello_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/src/itakello_logging/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:54:27.839011 itakello_logging-0.2.1.5/src/itakello_logging/filters/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/src/itakello_logging/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/src/itakello_logging/filters/custom_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/src/itakello_logging/filters/ignore_root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:54:27.839011 itakello_logging-0.2.1.5/src/itakello_logging/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/src/itakello_logging/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/src/itakello_logging/formatters/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:54:27.839011 itakello_logging-0.2.1.5/src/itakello_logging/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/src/itakello_logging/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/src/itakello_logging/loggers/custom_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:54:27.839011 itakello_logging-0.2.1.5/src/itakello_logging/test_logs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/src/itakello_logging/test_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-29 16:54:18.000000 itakello_logging-0.2.1.5/src/itakello_logging/test_logs/test_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:54:27.839011 itakello_logging-0.2.1.5/src/itakello_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-29 16:54:27.000000 itakello_logging-0.2.1.5/src/itakello_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-29 16:54:27.000000 itakello_logging-0.2.1.5/src/itakello_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:54:27.000000 itakello_logging-0.2.1.5/src/itakello_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 16:54:27.000000 itakello_logging-0.2.1.5/src/itakello_logging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:54:12.649917 itakello_logging-0.2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-09 12:54:12.649917 itakello_logging-0.2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:54:12.649917 itakello_logging-0.2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:54:12.645917 itakello_logging-0.2.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:54:12.645917 itakello_logging-0.2.1.6/src/itakello_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/src/itakello_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/src/itakello_logging/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:54:12.649917 itakello_logging-0.2.1.6/src/itakello_logging/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/src/itakello_logging/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/src/itakello_logging/filters/custom_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/src/itakello_logging/filters/ignore_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:54:12.649917 itakello_logging-0.2.1.6/src/itakello_logging/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/src/itakello_logging/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/src/itakello_logging/formatters/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:54:12.649917 itakello_logging-0.2.1.6/src/itakello_logging/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/src/itakello_logging/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/src/itakello_logging/loggers/custom_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:54:12.649917 itakello_logging-0.2.1.6/src/itakello_logging/test_logs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/src/itakello_logging/test_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-09 12:54:04.000000 itakello_logging-0.2.1.6/src/itakello_logging/test_logs/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:54:12.649917 itakello_logging-0.2.1.6/src/itakello_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-09 12:54:12.000000 itakello_logging-0.2.1.6/src/itakello_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-09 12:54:12.000000 itakello_logging-0.2.1.6/src/itakello_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:54:12.000000 itakello_logging-0.2.1.6/src/itakello_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 12:54:12.000000 itakello_logging-0.2.1.6/src/itakello_logging.egg-info/top_level.txt
```

### Comparing `itakello_logging-0.2.1.5/LICENSE` & `itakello_logging-0.2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `itakello_logging-0.2.1.5/PKG-INFO` & `itakello_logging-0.2.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itakello_logging
-Version: 0.2.1.5
+Version: 0.2.1.6
 Summary: A custom logging library by Itakello
 Home-page: https://github.com/Itakello/itakello_logging
 Author: Itakello
 Author-email: maxste000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itakello_logging-0.2.1.5/README.md` & `itakello_logging-0.2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `itakello_logging-0.2.1.5/setup.py` & `itakello_logging-0.2.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="itakello_logging",
-    version="0.2.1.5",
+    version="0.2.1.6",
     author="Itakello",
     author_email="maxste000@gmail.com",
     description="A custom logging library by Itakello",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Itakello/itakello_logging",
     package_dir={"": "src"},
```

### Comparing `itakello_logging-0.2.1.5/src/itakello_logging/core.py` & `itakello_logging-0.2.1.6/src/itakello_logging/core.py`

 * *Files identical despite different names*

### Comparing `itakello_logging-0.2.1.5/src/itakello_logging/formatters/console.py` & `itakello_logging-0.2.1.6/src/itakello_logging/formatters/console.py`

 * *Files identical despite different names*

### Comparing `itakello_logging-0.2.1.5/src/itakello_logging.egg-info/PKG-INFO` & `itakello_logging-0.2.1.6/src/itakello_logging.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itakello_logging
-Version: 0.2.1.5
+Version: 0.2.1.6
 Summary: A custom logging library by Itakello
 Home-page: https://github.com/Itakello/itakello_logging
 Author: Itakello
 Author-email: maxste000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itakello_logging-0.2.1.5/src/itakello_logging.egg-info/SOURCES.txt` & `itakello_logging-0.2.1.6/src/itakello_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

