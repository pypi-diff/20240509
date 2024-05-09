# Comparing `tmp/deltafi-2.0rc1713535554033.tar.gz` & `tmp/deltafi-2.0rc1714076410617.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-2.0rc1713535554033.tar", max compression
+gzip compressed data, was "deltafi-2.0rc1714076410617.tar", max compression
```

## Comparing `deltafi-2.0rc1713535554033.tar` & `deltafi-2.0rc1714076410617.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-2.0rc1713535554033/README.md
--rw-r--r--   0        0        0      709 2023-09-08 11:24:47.608536 deltafi-2.0rc1713535554033/deltafi/__init__.py
--rw-r--r--   0        0        0     5323 2024-04-19 12:26:49.516818 deltafi-2.0rc1713535554033/deltafi/action.py
--rw-r--r--   0        0        0     2847 2023-10-13 13:53:29.360657 deltafi-2.0rc1713535554033/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      865 2024-04-19 12:26:49.516818 deltafi-2.0rc1713535554033/deltafi/actiontype.py
--rw-r--r--   0        0        0    11301 2024-04-19 12:26:49.520818 deltafi-2.0rc1713535554033/deltafi/domain.py
--rw-r--r--   0        0        0      943 2024-04-19 12:26:49.522818 deltafi-2.0rc1713535554033/deltafi/exception.py
--rw-r--r--   0        0        0     1090 2023-11-16 03:01:54.189409 deltafi-2.0rc1713535554033/deltafi/genericmodel.py
--rw-r--r--   0        0        0     1656 2024-04-19 12:26:49.523818 deltafi-2.0rc1713535554033/deltafi/input.py
--rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-2.0rc1713535554033/deltafi/logger.py
--rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-2.0rc1713535554033/deltafi/metric.py
--rw-r--r--   0        0        0    12294 2024-04-19 12:26:49.531818 deltafi-2.0rc1713535554033/deltafi/plugin.py
--rw-r--r--   0        0        0     8177 2024-04-19 12:26:49.535818 deltafi-2.0rc1713535554033/deltafi/result.py
--rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-2.0rc1713535554033/deltafi/storage.py
--rw-r--r--   0        0        0      709 2023-09-08 11:24:47.609536 deltafi-2.0rc1713535554033/deltafi/test_kit/__init__.py
--rw-r--r--   0        0        0     1378 2023-09-08 11:24:47.609536 deltafi-2.0rc1713535554033/deltafi/test_kit/assertions.py
--rw-r--r--   0        0        0     1581 2023-09-08 11:24:47.609536 deltafi-2.0rc1713535554033/deltafi/test_kit/compare_helpers.py
--rw-r--r--   0        0        0      833 2023-08-07 14:10:09.593662 deltafi-2.0rc1713535554033/deltafi/test_kit/constants.py
--rw-r--r--   0        0        0     2090 2024-01-26 17:47:35.400662 deltafi-2.0rc1713535554033/deltafi/test_kit/domain.py
--rw-r--r--   0        0        0     1899 2024-01-26 17:47:35.400662 deltafi-2.0rc1713535554033/deltafi/test_kit/egress.py
--rw-r--r--   0        0        0     2587 2024-01-26 17:47:35.400662 deltafi-2.0rc1713535554033/deltafi/test_kit/enrich.py
--rw-r--r--   0        0        0    14602 2024-04-19 12:26:49.535818 deltafi-2.0rc1713535554033/deltafi/test_kit/framework.py
--rw-r--r--   0        0        0     4085 2024-04-19 12:26:49.536818 deltafi-2.0rc1713535554033/deltafi/test_kit/transform.py
--rw-r--r--   0        0        0     1933 2024-01-26 17:47:35.408662 deltafi-2.0rc1713535554033/deltafi/test_kit/validate.py
--rw-r--r--   0        0        0     1310 2024-04-19 14:06:20.290061 deltafi-2.0rc1713535554033/pyproject.toml
--rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 deltafi-2.0rc1713535554033/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-2.0rc1714076410617/README.md
+-rw-r--r--   0        0        0      709 2023-09-08 11:24:47.608536 deltafi-2.0rc1714076410617/deltafi/__init__.py
+-rw-r--r--   0        0        0     5323 2024-04-25 20:19:24.267191 deltafi-2.0rc1714076410617/deltafi/action.py
+-rw-r--r--   0        0        0     2847 2023-10-13 13:53:29.360657 deltafi-2.0rc1714076410617/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      865 2024-04-25 20:19:24.267191 deltafi-2.0rc1714076410617/deltafi/actiontype.py
+-rw-r--r--   0        0        0    11301 2024-04-25 20:19:24.267191 deltafi-2.0rc1714076410617/deltafi/domain.py
+-rw-r--r--   0        0        0      943 2024-04-25 20:19:24.267191 deltafi-2.0rc1714076410617/deltafi/exception.py
+-rw-r--r--   0        0        0     1090 2023-11-16 03:01:54.189409 deltafi-2.0rc1714076410617/deltafi/genericmodel.py
+-rw-r--r--   0        0        0     1656 2024-04-25 20:19:24.268191 deltafi-2.0rc1714076410617/deltafi/input.py
+-rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-2.0rc1714076410617/deltafi/logger.py
+-rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-2.0rc1714076410617/deltafi/metric.py
+-rw-r--r--   0        0        0    12294 2024-04-25 20:19:24.268191 deltafi-2.0rc1714076410617/deltafi/plugin.py
+-rw-r--r--   0        0        0     8177 2024-04-25 20:19:24.268191 deltafi-2.0rc1714076410617/deltafi/result.py
+-rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-2.0rc1714076410617/deltafi/storage.py
+-rw-r--r--   0        0        0      709 2023-09-08 11:24:47.609536 deltafi-2.0rc1714076410617/deltafi/test_kit/__init__.py
+-rw-r--r--   0        0        0     1378 2023-09-08 11:24:47.609536 deltafi-2.0rc1714076410617/deltafi/test_kit/assertions.py
+-rw-r--r--   0        0        0    12178 2024-04-25 20:19:24.268191 deltafi-2.0rc1714076410617/deltafi/test_kit/compare_helpers.py
+-rw-r--r--   0        0        0      833 2023-08-07 14:10:09.593662 deltafi-2.0rc1714076410617/deltafi/test_kit/constants.py
+-rw-r--r--   0        0        0     2090 2024-01-26 17:47:35.400662 deltafi-2.0rc1714076410617/deltafi/test_kit/domain.py
+-rw-r--r--   0        0        0     1899 2024-01-26 17:47:35.400662 deltafi-2.0rc1714076410617/deltafi/test_kit/egress.py
+-rw-r--r--   0        0        0     2587 2024-01-26 17:47:35.400662 deltafi-2.0rc1714076410617/deltafi/test_kit/enrich.py
+-rw-r--r--   0        0        0    14602 2024-04-25 20:19:24.269191 deltafi-2.0rc1714076410617/deltafi/test_kit/framework.py
+-rw-r--r--   0        0        0     4085 2024-04-25 20:19:24.269191 deltafi-2.0rc1714076410617/deltafi/test_kit/transform.py
+-rw-r--r--   0        0        0     1933 2024-01-26 17:47:35.408662 deltafi-2.0rc1714076410617/deltafi/test_kit/validate.py
+-rw-r--r--   0        0        0     1310 2024-04-25 20:20:40.177429 deltafi-2.0rc1714076410617/pyproject.toml
+-rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 deltafi-2.0rc1714076410617/PKG-INFO
```

### Comparing `deltafi-2.0rc1713535554033/deltafi/__init__.py` & `deltafi-2.0rc1714076410617/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/action.py` & `deltafi-2.0rc1714076410617/deltafi/action.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/actioneventqueue.py` & `deltafi-2.0rc1714076410617/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/actiontype.py` & `deltafi-2.0rc1714076410617/deltafi/actiontype.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/domain.py` & `deltafi-2.0rc1714076410617/deltafi/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/exception.py` & `deltafi-2.0rc1714076410617/deltafi/exception.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/genericmodel.py` & `deltafi-2.0rc1714076410617/deltafi/genericmodel.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/input.py` & `deltafi-2.0rc1714076410617/deltafi/input.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/logger.py` & `deltafi-2.0rc1714076410617/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/metric.py` & `deltafi-2.0rc1714076410617/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/plugin.py` & `deltafi-2.0rc1714076410617/deltafi/plugin.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/result.py` & `deltafi-2.0rc1714076410617/deltafi/result.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/storage.py` & `deltafi-2.0rc1714076410617/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/test_kit/__init__.py` & `deltafi-2.0rc1714076410617/deltafi/test_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/test_kit/assertions.py` & `deltafi-2.0rc1714076410617/deltafi/test_kit/assertions.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/test_kit/constants.py` & `deltafi-2.0rc1714076410617/deltafi/test_kit/constants.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/test_kit/domain.py` & `deltafi-2.0rc1714076410617/deltafi/test_kit/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/test_kit/egress.py` & `deltafi-2.0rc1714076410617/deltafi/test_kit/egress.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/test_kit/enrich.py` & `deltafi-2.0rc1714076410617/deltafi/test_kit/enrich.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/test_kit/framework.py` & `deltafi-2.0rc1714076410617/deltafi/test_kit/framework.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/test_kit/transform.py` & `deltafi-2.0rc1714076410617/deltafi/test_kit/transform.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/deltafi/test_kit/validate.py` & `deltafi-2.0rc1714076410617/deltafi/test_kit/validate.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1713535554033/pyproject.toml` & `deltafi-2.0rc1714076410617/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltafi"
-version = "2.0rc1713535554033"
+version = "2.0rc1714076410617"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `deltafi-2.0rc1713535554033/PKG-INFO` & `deltafi-2.0rc1714076410617/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 2.0rc1713535554033
+Version: 2.0rc1714076410617
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

