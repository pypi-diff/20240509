# Comparing `tmp/deepkeep-0.3.0.tar.gz` & `tmp/deepkeep-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepkeep-0.3.0.tar", max compression
+gzip compressed data, was "deepkeep-0.3.1.tar", max compression
```

## Comparing `deepkeep-0.3.0.tar` & `deepkeep-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2024-03-11 17:37:46.124980 deepkeep-0.3.0/LICENSE
--rw-r--r--   0        0        0     2623 2024-03-21 10:15:04.891310 deepkeep-0.3.0/README.md
--rw-r--r--   0        0        0     1920 2024-05-08 17:34:18.083996 deepkeep-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      639 2024-03-21 10:24:43.713079 deepkeep-0.3.0/src/deepkeep/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 17:37:46.124980 deepkeep-0.3.0/src/deepkeep/__main__.py
--rw-r--r--   0        0        0     4614 2024-03-24 13:42:49.152184 deepkeep-0.3.0/src/deepkeep/_client.py
--rw-r--r--   0        0        0      114 2024-03-21 10:24:04.340031 deepkeep-0.3.0/src/deepkeep/_exceptions.py
--rw-r--r--   0        0        0       51 2024-03-21 18:20:47.416547 deepkeep-0.3.0/src/deepkeep/_utils/__init__.py
--rw-r--r--   0        0        0      659 2024-03-21 18:10:41.979521 deepkeep-0.3.0/src/deepkeep/_utils/decorators.py
--rw-r--r--   0        0        0      178 2024-05-08 17:34:18.067996 deepkeep-0.3.0/src/deepkeep/modules/__init__.py
--rw-r--r--   0        0        0       81 2024-05-08 17:34:18.083996 deepkeep-0.3.0/src/deepkeep/modules/assessment/__init__.py
--rw-r--r--   0        0        0     1114 2024-05-08 17:34:18.079996 deepkeep-0.3.0/src/deepkeep/modules/assessment/llm.py
--rw-r--r--   0        0        0     1487 2024-03-21 18:18:59.176458 deepkeep-0.3.0/src/deepkeep/modules/base_module.py
--rw-r--r--   0        0        0      162 2024-03-18 19:46:07.313880 deepkeep-0.3.0/src/deepkeep/modules/chat/__init__.py
--rw-r--r--   0        0        0     1504 2024-03-21 10:24:04.324031 deepkeep-0.3.0/src/deepkeep/modules/chat/chat.py
--rw-r--r--   0        0        0     1842 2024-03-21 12:01:14.928441 deepkeep-0.3.0/src/deepkeep/modules/chat/conversation.py
--rw-r--r--   0        0        0     2423 2024-04-02 15:26:12.972822 deepkeep-0.3.0/src/deepkeep/modules/chat/message.py
--rw-r--r--   0        0        0       55 2024-03-18 18:13:20.225113 deepkeep-0.3.0/src/deepkeep/modules/pipeline/__init__.py
--rw-r--r--   0        0        0      444 2024-03-21 11:48:43.740298 deepkeep-0.3.0/src/deepkeep/modules/pipeline/pipeline.py
--rw-r--r--   0        0        0       49 2024-03-14 20:15:57.508364 deepkeep-0.3.0/src/deepkeep/modules/report/__init__.py
--rw-r--r--   0        0        0      236 2024-03-20 20:47:57.240529 deepkeep-0.3.0/src/deepkeep/modules/report/report.py
--rw-r--r--   0        0        0     4117 1970-01-01 00:00:00.000000 deepkeep-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-11 17:37:46.124980 deepkeep-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2623 2024-03-21 10:15:04.891310 deepkeep-0.3.1/README.md
+-rw-r--r--   0        0        0     1920 2024-05-08 19:02:50.483032 deepkeep-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      639 2024-03-21 10:24:43.713079 deepkeep-0.3.1/src/deepkeep/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 17:37:46.124980 deepkeep-0.3.1/src/deepkeep/__main__.py
+-rw-r--r--   0        0        0     4614 2024-03-24 13:42:49.152184 deepkeep-0.3.1/src/deepkeep/_client.py
+-rw-r--r--   0        0        0      114 2024-03-21 10:24:04.340031 deepkeep-0.3.1/src/deepkeep/_exceptions.py
+-rw-r--r--   0        0        0       51 2024-03-21 18:20:47.416547 deepkeep-0.3.1/src/deepkeep/_utils/__init__.py
+-rw-r--r--   0        0        0      659 2024-03-21 18:10:41.979521 deepkeep-0.3.1/src/deepkeep/_utils/decorators.py
+-rw-r--r--   0        0        0      178 2024-05-08 17:34:18.067996 deepkeep-0.3.1/src/deepkeep/modules/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-08 18:58:42.498719 deepkeep-0.3.1/src/deepkeep/modules/assessment/__init__.py
+-rw-r--r--   0        0        0     1114 2024-05-08 17:34:18.079996 deepkeep-0.3.1/src/deepkeep/modules/assessment/llm.py
+-rw-r--r--   0        0        0     1487 2024-03-21 18:18:59.176458 deepkeep-0.3.1/src/deepkeep/modules/base_module.py
+-rw-r--r--   0        0        0      162 2024-03-18 19:46:07.313880 deepkeep-0.3.1/src/deepkeep/modules/chat/__init__.py
+-rw-r--r--   0        0        0     1504 2024-03-21 10:24:04.324031 deepkeep-0.3.1/src/deepkeep/modules/chat/chat.py
+-rw-r--r--   0        0        0     1842 2024-03-21 12:01:14.928441 deepkeep-0.3.1/src/deepkeep/modules/chat/conversation.py
+-rw-r--r--   0        0        0     2423 2024-04-02 15:26:12.972822 deepkeep-0.3.1/src/deepkeep/modules/chat/message.py
+-rw-r--r--   0        0        0       55 2024-03-18 18:13:20.225113 deepkeep-0.3.1/src/deepkeep/modules/pipeline/__init__.py
+-rw-r--r--   0        0        0      444 2024-03-21 11:48:43.740298 deepkeep-0.3.1/src/deepkeep/modules/pipeline/pipeline.py
+-rw-r--r--   0        0        0       49 2024-03-14 20:15:57.508364 deepkeep-0.3.1/src/deepkeep/modules/report/__init__.py
+-rw-r--r--   0        0        0      236 2024-03-20 20:47:57.240529 deepkeep-0.3.1/src/deepkeep/modules/report/report.py
+-rw-r--r--   0        0        0     4117 1970-01-01 00:00:00.000000 deepkeep-0.3.1/PKG-INFO
```

### Comparing `deepkeep-0.3.0/README.md` & `deepkeep-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `deepkeep-0.3.0/pyproject.toml` & `deepkeep-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepkeep"
-version = "0.3.0"
+version = "0.3.1"
 description = "The official Python library for the Deepkeep API"
 readme = "README.md"
 license = "Apache-2.0"
 authors = ["DeepKeep Devs <dev@deepkeep.ai>"]
 packages = [{include = "deepkeep", from = "src"}]
 
 classifiers = [
```

### Comparing `deepkeep-0.3.0/src/deepkeep/__init__.py` & `deepkeep-0.3.1/src/deepkeep/__init__.py`

 * *Files identical despite different names*

### Comparing `deepkeep-0.3.0/src/deepkeep/_client.py` & `deepkeep-0.3.1/src/deepkeep/_client.py`

 * *Files identical despite different names*

### Comparing `deepkeep-0.3.0/src/deepkeep/_utils/decorators.py` & `deepkeep-0.3.1/src/deepkeep/_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `deepkeep-0.3.0/src/deepkeep/modules/assessment/llm.py` & `deepkeep-0.3.1/src/deepkeep/modules/assessment/llm.py`

 * *Files identical despite different names*

### Comparing `deepkeep-0.3.0/src/deepkeep/modules/base_module.py` & `deepkeep-0.3.1/src/deepkeep/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `deepkeep-0.3.0/src/deepkeep/modules/chat/chat.py` & `deepkeep-0.3.1/src/deepkeep/modules/chat/chat.py`

 * *Files identical despite different names*

### Comparing `deepkeep-0.3.0/src/deepkeep/modules/chat/conversation.py` & `deepkeep-0.3.1/src/deepkeep/modules/chat/conversation.py`

 * *Files identical despite different names*

### Comparing `deepkeep-0.3.0/src/deepkeep/modules/chat/message.py` & `deepkeep-0.3.1/src/deepkeep/modules/chat/message.py`

 * *Files identical despite different names*

### Comparing `deepkeep-0.3.0/PKG-INFO` & `deepkeep-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepkeep
-Version: 0.3.0
+Version: 0.3.1
 Summary: The official Python library for the Deepkeep API
 License: Apache-2.0
 Author: DeepKeep Devs
 Author-email: dev@deepkeep.ai
 Requires-Python: >=3.8,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

