# Comparing `tmp/addemongo-0.0.0.tar.gz` & `tmp/addemongo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addemongo-0.0.0.tar", last modified: Thu May  9 17:55:31 2024, max compression
+gzip compressed data, was "addemongo-0.1.0.tar", last modified: Wed May  8 16:55:49 2024, max compression
```

## Comparing `addemongo-0.0.0.tar` & `addemongo-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,22 @@
--rw-r--r--   0        0        0      116 2024-05-09 17:55:24.264157 addemongo-0.0.0/LICENSE
--rw-r--r--   0        0        0      134 2024-05-06 23:42:11.106990 addemongo-0.0.0/README.md
--rw-r--r--   0        0        0     3026 2024-05-09 17:55:31.647219 addemongo-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-08 20:28:00.960738 addemongo-0.0.0/src/addemongo/__init__.py
--rw-r--r--   0        0        0       29 2024-05-09 17:45:14.201304 addemongo-0.0.0/src/addemongo/__version__.py
--rw-r--r--   0        0        0     1246 2024-05-09 00:58:06.555925 addemongo-0.0.0/src/addemongo/_base_client.py
--rw-r--r--   0        0        0        0 2024-05-06 23:42:11.112510 addemongo-0.0.0/src/addemongo/_motor/__init__.py
--rw-r--r--   0        0        0     4225 2024-05-09 03:19:34.080737 addemongo-0.0.0/src/addemongo/_motor/_client.py
--rw-r--r--   0        0        0        0 2024-05-06 23:42:11.114021 addemongo-0.0.0/src/addemongo/_pymongo/__init__.py
--rw-r--r--   0        0        0     4147 2024-05-09 00:59:47.256672 addemongo-0.0.0/src/addemongo/_pymongo/_client.py
--rw-r--r--   0        0        0      279 2024-05-06 23:42:11.117041 addemongo-0.0.0/src/addemongo/_types.py
--rw-r--r--   0        0        0      130 2024-05-06 23:42:11.118043 addemongo-0.0.0/src/addemongo/builders/__init__.py
--rw-r--r--   0        0        0     3188 2024-05-09 00:59:47.258677 addemongo-0.0.0/src/addemongo/builders/aggregation.py
--rw-r--r--   0        0        0     3668 2024-05-09 03:07:59.917107 addemongo-0.0.0/src/addemongo/builders/query.py
--rw-r--r--   0        0        0     1461 2024-05-09 00:59:47.259677 addemongo-0.0.0/src/addemongo/connection.py
--rw-r--r--   0        0        0        0 2024-05-06 23:42:11.121042 addemongo-0.0.0/src/addemongo/models/__init__.py
--rw-r--r--   0        0        0      203 2024-05-06 23:42:11.122045 addemongo-0.0.0/src/addemongo/models/pagination.py
--rw-r--r--   0        0        0        0 2024-05-06 17:31:40.845368 addemongo-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0     3899 2024-05-06 23:42:11.123047 addemongo-0.0.0/tests/addemongo/test_async_functions.py
--rw-r--r--   0        0        0      988 2024-05-06 23:42:11.124041 addemongo-0.0.0/tests/addemongo/test_client.py
--rw-r--r--   0        0        0     2554 2024-05-06 23:42:11.124554 addemongo-0.0.0/tests/addemongo/test_sync_functions.py
--rw-r--r--   0        0        0      225 2024-05-09 00:58:06.561119 addemongo-0.0.0/tests/motor/test_motor.py
--rw-r--r--   0        0        0      235 2024-05-06 23:42:11.126568 addemongo-0.0.0/tests/pymongo/test_pymongo.py
--rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 addemongo-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      134 2024-05-06 23:42:11.106990 addemongo-0.1.0/README.md
+-rw-r--r--   0        0        0      880 2024-05-08 16:55:49.773441 addemongo-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 22:46:01.419649 addemongo-0.1.0/src/addemongo/__init__.py
+-rw-r--r--   0        0        0     1246 2024-05-06 23:42:11.111499 addemongo-0.1.0/src/addemongo/_base_client.py
+-rw-r--r--   0        0        0        0 2024-05-06 23:42:11.112510 addemongo-0.1.0/src/addemongo/_motor/__init__.py
+-rw-r--r--   0        0        0     5137 2024-05-06 23:42:11.112510 addemongo-0.1.0/src/addemongo/_motor/_client.py
+-rw-r--r--   0        0        0        0 2024-05-06 23:42:11.114021 addemongo-0.1.0/src/addemongo/_pymongo/__init__.py
+-rw-r--r--   0        0        0     4998 2024-05-06 23:42:11.116055 addemongo-0.1.0/src/addemongo/_pymongo/_client.py
+-rw-r--r--   0        0        0      279 2024-05-06 23:42:11.117041 addemongo-0.1.0/src/addemongo/_types.py
+-rw-r--r--   0        0        0      130 2024-05-06 23:42:11.118043 addemongo-0.1.0/src/addemongo/builders/__init__.py
+-rw-r--r--   0        0        0     3180 2024-05-06 23:42:11.119042 addemongo-0.1.0/src/addemongo/builders/aggregation.py
+-rw-r--r--   0        0        0     4261 2024-05-06 23:42:11.120046 addemongo-0.1.0/src/addemongo/builders/query.py
+-rw-r--r--   0        0        0     1365 2024-05-06 23:42:11.120046 addemongo-0.1.0/src/addemongo/connection.py
+-rw-r--r--   0        0        0        0 2024-05-06 23:42:11.121042 addemongo-0.1.0/src/addemongo/models/__init__.py
+-rw-r--r--   0        0        0      203 2024-05-06 23:42:11.122045 addemongo-0.1.0/src/addemongo/models/pagination.py
+-rw-r--r--   0        0        0        0 2024-05-06 17:31:40.845368 addemongo-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3899 2024-05-06 23:42:11.123047 addemongo-0.1.0/tests/addemongo/test_async_functions.py
+-rw-r--r--   0        0        0      988 2024-05-06 23:42:11.124041 addemongo-0.1.0/tests/addemongo/test_client.py
+-rw-r--r--   0        0        0     2554 2024-05-06 23:42:11.124554 addemongo-0.1.0/tests/addemongo/test_sync_functions.py
+-rw-r--r--   0        0        0      225 2024-05-06 23:42:11.125566 addemongo-0.1.0/tests/motor/test_motor.py
+-rw-r--r--   0        0        0      235 2024-05-06 23:42:11.126568 addemongo-0.1.0/tests/pymongo/test_pymongo.py
+-rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 addemongo-0.1.0/PKG-INFO
```

### Comparing `addemongo-0.0.0/src/addemongo/_base_client.py` & `addemongo-0.1.0/src/addemongo/_base_client.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.0/src/addemongo/builders/aggregation.py` & `addemongo-0.1.0/src/addemongo/builders/aggregation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Callable
 
 
 class AggregationBuilder:
-    def __init__(self) -> None:
+    def __init__(self):
         self.__aggregation_list: list[dict[str, Any]] = []
 
     def set_group(
         self,
         query: dict[str, Any],
         body: dict[str, Any],
         condition: Callable[[], bool] = lambda: True,
```

### Comparing `addemongo-0.0.0/tests/addemongo/test_async_functions.py` & `addemongo-0.1.0/tests/addemongo/test_async_functions.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.0/tests/addemongo/test_client.py` & `addemongo-0.1.0/tests/addemongo/test_client.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.0/tests/addemongo/test_sync_functions.py` & `addemongo-0.1.0/tests/addemongo/test_sync_functions.py`

 * *Files identical despite different names*

