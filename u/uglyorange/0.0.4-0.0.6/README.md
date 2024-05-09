# Comparing `tmp/uglyorange-0.0.4.tar.gz` & `tmp/uglyorange-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uglyorange-0.0.4.tar", max compression
+gzip compressed data, was "uglyorange-0.0.6.tar", max compression
```

## Comparing `uglyorange-0.0.4.tar` & `uglyorange-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2024-03-29 06:27:57.026996 uglyorange-0.0.4/README.md
--rw-r--r--   0        0        0      511 2024-04-18 02:26:36.235538 uglyorange-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-29 06:27:57.026944 uglyorange-0.0.4/uglyorange/__init__.py
--rw-r--r--   0        0        0     3424 2024-04-18 02:26:24.287567 uglyorange-0.0.4/uglyorange/network.py
--rw-r--r--   0        0        0      313 2024-03-30 03:39:04.125950 uglyorange-0.0.4/uglyorange/utils.py
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 uglyorange-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-29 06:27:57.026996 uglyorange-0.0.6/README.md
+-rw-r--r--   0        0        0      612 2024-05-09 03:55:45.653426 uglyorange-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-29 06:27:57.026944 uglyorange-0.0.6/uglyorange/__init__.py
+-rw-r--r--   0        0        0     5006 2024-05-09 03:55:20.122474 uglyorange-0.0.6/uglyorange/network.py
+-rw-r--r--   0        0        0      597 2024-05-09 03:35:30.934307 uglyorange-0.0.6/uglyorange/sys.py
+-rw-r--r--   0        0        0      313 2024-03-30 03:39:04.125950 uglyorange-0.0.6/uglyorange/utils.py
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 uglyorange-0.0.6/PKG-INFO
```

### Comparing `uglyorange-0.0.4/PKG-INFO` & `uglyorange-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uglyorange
-Version: 0.0.4
+Version: 0.0.6
 Summary: 
 Author: ultrasev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

