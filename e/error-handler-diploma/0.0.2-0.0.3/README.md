# Comparing `tmp/error_handler_diploma-0.0.2.tar.gz` & `tmp/error_handler_diploma-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error_handler_diploma-0.0.2.tar", last modified: Sun Mar 24 16:43:21 2024, max compression
+gzip compressed data, was "error_handler_diploma-0.0.3.tar", last modified: Thu May  9 17:24:33 2024, max compression
```

## Comparing `error_handler_diploma-0.0.2.tar` & `error_handler_diploma-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 16:43:21.314433 error_handler_diploma-0.0.2/
--rw-rw-rw-   0        0        0      534 2024-03-24 16:43:21.313646 error_handler_diploma-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-24 16:43:21.295594 error_handler_diploma-0.0.2/error_handler_diploma/
--rw-rw-rw-   0        0        0       29 2024-03-24 16:37:10.000000 error_handler_diploma-0.0.2/error_handler_diploma/__init__.py
--rw-rw-rw-   0        0        0       49 2024-03-24 16:36:38.000000 error_handler_diploma-0.0.2/error_handler_diploma/test.py
-drwxrwxrwx   0        0        0        0 2024-03-24 16:43:21.312647 error_handler_diploma-0.0.2/error_handler_diploma.egg-info/
--rw-rw-rw-   0        0        0      534 2024-03-24 16:43:21.000000 error_handler_diploma-0.0.2/error_handler_diploma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-03-24 16:43:21.000000 error_handler_diploma-0.0.2/error_handler_diploma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 16:43:21.000000 error_handler_diploma-0.0.2/error_handler_diploma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-03-24 16:43:21.000000 error_handler_diploma-0.0.2/error_handler_diploma.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-24 16:43:21.314433 error_handler_diploma-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      873 2024-03-24 16:43:11.000000 error_handler_diploma-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:24:33.641549 error_handler_diploma-0.0.3/
+-rw-rw-rw-   0        0        0      534 2024-05-09 17:24:33.640038 error_handler_diploma-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 17:24:33.618351 error_handler_diploma-0.0.3/error_handler_diploma/
+-rw-rw-rw-   0        0        0       99 2024-05-09 17:11:26.000000 error_handler_diploma-0.0.3/error_handler_diploma/__init__.py
+-rw-rw-rw-   0        0        0     4053 2024-05-09 17:10:59.000000 error_handler_diploma-0.0.3/error_handler_diploma/test.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:24:33.639047 error_handler_diploma-0.0.3/error_handler_diploma.egg-info/
+-rw-rw-rw-   0        0        0      534 2024-05-09 17:24:33.000000 error_handler_diploma-0.0.3/error_handler_diploma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-09 17:24:33.000000 error_handler_diploma-0.0.3/error_handler_diploma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 17:24:33.000000 error_handler_diploma-0.0.3/error_handler_diploma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-09 17:24:33.000000 error_handler_diploma-0.0.3/error_handler_diploma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 17:24:33.641549 error_handler_diploma-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      873 2024-05-09 17:19:55.000000 error_handler_diploma-0.0.3/setup.py
```

### Comparing `error_handler_diploma-0.0.2/PKG-INFO` & `error_handler_diploma-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error_handler_diploma
-Version: 0.0.2
+Version: 0.0.3
 Summary: Error handling library
 Author: Vladyslava Rozhkovan
 Keywords: python,error handling,library,diploma project
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `error_handler_diploma-0.0.2/error_handler_diploma.egg-info/PKG-INFO` & `error_handler_diploma-0.0.3/error_handler_diploma.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error_handler_diploma
-Version: 0.0.2
+Version: 0.0.3
 Summary: Error handling library
 Author: Vladyslava Rozhkovan
 Keywords: python,error handling,library,diploma project
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `error_handler_diploma-0.0.2/setup.py` & `error_handler_diploma-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'Error handling library'
 LONG_DESCRIPTION = 'Diploma project. Error handling library for Python.'
 
 setup(
         name="error_handler_diploma", 
         version=VERSION,
         author="Vladyslava Rozhkovan",
```

