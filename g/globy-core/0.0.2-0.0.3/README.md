# Comparing `tmp/globy_core-0.0.2.tar.gz` & `tmp/globy_core-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globy_core-0.0.2.tar", last modified: Wed May  1 18:37:59 2024, max compression
+gzip compressed data, was "globy_core-0.0.3.tar", last modified: Thu May  9 08:31:30 2024, max compression
```

## Comparing `globy_core-0.0.2.tar` & `globy_core-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-01 18:37:59.977497 globy_core-0.0.2/
--rw-r--r--   0 berre     (1000) berre     (1000)      486 2024-05-01 18:37:59.977497 globy_core-0.0.2/PKG-INFO
--rw-r--r--   0 berre     (1000) berre     (1000)       13 2024-03-28 19:32:06.000000 globy_core-0.0.2/README.md
--rw-r--r--   0 berre     (1000) berre     (1000)      525 2024-05-01 18:37:19.000000 globy_core-0.0.2/pyproject.toml
--rw-r--r--   0 berre     (1000) berre     (1000)       38 2024-05-01 18:37:59.977497 globy_core-0.0.2/setup.cfg
-drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-01 18:37:59.975497 globy_core-0.0.2/src/
-drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-01 18:37:59.975497 globy_core-0.0.2/src/globy_core/
-drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-01 18:37:59.976497 globy_core-0.0.2/src/globy_core/api/
--rw-r--r--   0 berre     (1000) berre     (1000)        0 2024-04-20 08:25:59.000000 globy_core-0.0.2/src/globy_core/api/private.py
--rw-r--r--   0 berre     (1000) berre     (1000)        0 2024-04-20 08:25:53.000000 globy_core-0.0.2/src/globy_core/api/public.py
-drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-01 18:37:59.976497 globy_core-0.0.2/src/globy_core/cms/
--rw-r--r--   0 berre     (1000) berre     (1000)     1238 2024-04-20 08:39:48.000000 globy_core-0.0.2/src/globy_core/cms/sitebuilder.py
--rw-r--r--   0 berre     (1000) berre     (1000)       42 2024-03-24 13:15:11.000000 globy_core-0.0.2/src/globy_core/cms/sitebuilder_test.py
-drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-01 18:37:59.976497 globy_core-0.0.2/src/globy_core/common/
--rw-r--r--   0 berre     (1000) berre     (1000)        0 2024-04-20 07:33:53.000000 globy_core-0.0.2/src/globy_core/common/helpers.py
--rw-r--r--   0 berre     (1000) berre     (1000)     2018 2024-03-28 19:52:47.000000 globy_core-0.0.2/src/globy_core/common/queue.py
-drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-01 18:37:59.976497 globy_core-0.0.2/src/globy_core/interaction/
--rw-r--r--   0 berre     (1000) berre     (1000)     3383 2024-04-29 12:54:00.000000 globy_core-0.0.2/src/globy_core/interaction/globy-interaction.py
-drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-01 18:37:59.976497 globy_core-0.0.2/src/globy_core/logging/
--rw-r--r--   0 berre     (1000) berre     (1000)     1289 2024-05-01 17:31:50.000000 globy_core-0.0.2/src/globy_core/logging/logger.py
-drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-01 18:37:59.977497 globy_core-0.0.2/src/globy_core/ml/
--rw-r--r--   0 berre     (1000) berre     (1000)        0 2024-04-20 07:30:35.000000 globy_core-0.0.2/src/globy_core/ml/inference-preprocess.py
--rw-r--r--   0 berre     (1000) berre     (1000)     1895 2024-04-20 07:40:27.000000 globy_core-0.0.2/src/globy_core/ml/inference.py
-drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-01 18:37:59.977497 globy_core-0.0.2/src/globy_core.egg-info/
--rw-r--r--   0 berre     (1000) berre     (1000)      486 2024-05-01 18:37:59.000000 globy_core-0.0.2/src/globy_core.egg-info/PKG-INFO
--rw-r--r--   0 berre     (1000) berre     (1000)      563 2024-05-01 18:37:59.000000 globy_core-0.0.2/src/globy_core.egg-info/SOURCES.txt
--rw-r--r--   0 berre     (1000) berre     (1000)        1 2024-05-01 18:37:59.000000 globy_core-0.0.2/src/globy_core.egg-info/dependency_links.txt
--rw-r--r--   0 berre     (1000) berre     (1000)       39 2024-05-01 18:37:59.000000 globy_core-0.0.2/src/globy_core.egg-info/requires.txt
--rw-r--r--   0 berre     (1000) berre     (1000)       11 2024-05-01 18:37:59.000000 globy_core-0.0.2/src/globy_core.egg-info/top_level.txt
+drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-09 08:31:30.489452 globy_core-0.0.3/
+-rw-r--r--   0 berre     (1000) berre     (1000)      611 2024-05-09 08:31:30.489452 globy_core-0.0.3/PKG-INFO
+-rw-r--r--   0 berre     (1000) berre     (1000)      137 2024-05-09 08:30:21.000000 globy_core-0.0.3/README.md
+-rw-r--r--   0 berre     (1000) berre     (1000)      525 2024-05-09 08:31:09.000000 globy_core-0.0.3/pyproject.toml
+-rw-r--r--   0 berre     (1000) berre     (1000)       38 2024-05-09 08:31:30.489452 globy_core-0.0.3/setup.cfg
+drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-09 08:31:30.486452 globy_core-0.0.3/src/
+drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-09 08:31:30.486452 globy_core-0.0.3/src/globy_core/
+drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-09 08:31:30.487452 globy_core-0.0.3/src/globy_core/api/
+-rw-r--r--   0 berre     (1000) berre     (1000)        0 2024-04-20 08:25:59.000000 globy_core-0.0.3/src/globy_core/api/private.py
+-rw-r--r--   0 berre     (1000) berre     (1000)        0 2024-04-20 08:25:53.000000 globy_core-0.0.3/src/globy_core/api/public.py
+drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-09 08:31:30.488452 globy_core-0.0.3/src/globy_core/cms/
+-rw-r--r--   0 berre     (1000) berre     (1000)     1238 2024-04-20 08:39:48.000000 globy_core-0.0.3/src/globy_core/cms/sitebuilder.py
+-rw-r--r--   0 berre     (1000) berre     (1000)       42 2024-03-24 13:15:11.000000 globy_core-0.0.3/src/globy_core/cms/sitebuilder_test.py
+drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-09 08:31:30.488452 globy_core-0.0.3/src/globy_core/common/
+-rw-r--r--   0 berre     (1000) berre     (1000)        0 2024-04-20 07:33:53.000000 globy_core-0.0.3/src/globy_core/common/helpers.py
+-rw-r--r--   0 berre     (1000) berre     (1000)     2277 2024-05-09 08:27:14.000000 globy_core-0.0.3/src/globy_core/common/queue.py
+drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-09 08:31:30.488452 globy_core-0.0.3/src/globy_core/interaction/
+-rw-r--r--   0 berre     (1000) berre     (1000)     3383 2024-04-29 12:54:00.000000 globy_core-0.0.3/src/globy_core/interaction/globy-interaction.py
+drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-09 08:31:30.488452 globy_core-0.0.3/src/globy_core/logging/
+-rw-r--r--   0 berre     (1000) berre     (1000)     1289 2024-05-01 17:31:50.000000 globy_core-0.0.3/src/globy_core/logging/logger.py
+drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-09 08:31:30.488452 globy_core-0.0.3/src/globy_core/ml/
+-rw-r--r--   0 berre     (1000) berre     (1000)        0 2024-04-20 07:30:35.000000 globy_core-0.0.3/src/globy_core/ml/inference-preprocess.py
+-rw-r--r--   0 berre     (1000) berre     (1000)     1895 2024-04-20 07:40:27.000000 globy_core-0.0.3/src/globy_core/ml/inference.py
+drwxr-xr-x   0 berre     (1000) berre     (1000)        0 2024-05-09 08:31:30.489452 globy_core-0.0.3/src/globy_core.egg-info/
+-rw-r--r--   0 berre     (1000) berre     (1000)      611 2024-05-09 08:31:30.000000 globy_core-0.0.3/src/globy_core.egg-info/PKG-INFO
+-rw-r--r--   0 berre     (1000) berre     (1000)      563 2024-05-09 08:31:30.000000 globy_core-0.0.3/src/globy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 berre     (1000) berre     (1000)        1 2024-05-09 08:31:30.000000 globy_core-0.0.3/src/globy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 berre     (1000) berre     (1000)       39 2024-05-09 08:31:30.000000 globy_core-0.0.3/src/globy_core.egg-info/requires.txt
+-rw-r--r--   0 berre     (1000) berre     (1000)       11 2024-05-09 08:31:30.000000 globy_core-0.0.3/src/globy_core.egg-info/top_level.txt
```

### Comparing `globy_core-0.0.2/pyproject.toml` & `globy_core-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "globy_core"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Björn L", email="bjorn@globy.ai" },
 ]
 description = "Globy Core"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `globy_core-0.0.2/src/globy_core/cms/sitebuilder.py` & `globy_core-0.0.3/src/globy_core/cms/sitebuilder.py`

 * *Files identical despite different names*

### Comparing `globy_core-0.0.2/src/globy_core/common/queue.py` & `globy_core-0.0.3/src/globy_core/common/queue.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from typing import Any, Optional
 import redis
 import boto3
 
-class QueueInterface:
+class GlobyQueue:
     """
     Common interface for a queue.
     """
     def enqueue(self, item: Any) -> None:
         """Add an item to the queue."""
         raise NotImplementedError
 
     def dequeue(self) -> Optional[Any]:
         """Remove and return an item from the queue. Return None if the queue is empty."""
         raise NotImplementedError
 
+    def put(self, item: Any) -> None:
+        """Add an item to the queue."""
+        return self.enqueue(item)
+
+    def pop(self) -> Optional[Any]:
+        """Remove and return an item from the queue. Return None if the queue is empty."""
+        return self.dequeue()
+
     def is_empty(self) -> bool:
         """Return True if the queue is empty, False otherwise."""
         raise NotImplementedError
 
-class RedisQueue(QueueInterface):
+class RedisQueue(GlobyQueue):
     """
     A queue implementation using Redis.
     """
     def __init__(self, name: str, host='localhost', port=6379, db=0):
         self._name = name
         self._client = redis.Redis(host=host, port=port, db=db)
 
@@ -32,15 +40,15 @@
     def dequeue(self) -> Optional[Any]:
         item = self._client.lpop(self._name)
         return item
 
     def is_empty(self) -> bool:
         return self._client.llen(self._name) == 0
 
-class SQSQueue(QueueInterface):
+class SQSQueue(GlobyQueue):
     def __init__(self, queue_name: str):
         self._sqs = boto3.resource('sqs')
         self._queue = self._sqs.get_queue_by_name(QueueName=queue_name)
 
     def enqueue(self, item: Any) -> None:
         self._queue.send_message(MessageBody=str(item))
```

### Comparing `globy_core-0.0.2/src/globy_core/interaction/globy-interaction.py` & `globy_core-0.0.3/src/globy_core/interaction/globy-interaction.py`

 * *Files identical despite different names*

### Comparing `globy_core-0.0.2/src/globy_core/logging/logger.py` & `globy_core-0.0.3/src/globy_core/logging/logger.py`

 * *Files identical despite different names*

### Comparing `globy_core-0.0.2/src/globy_core/ml/inference.py` & `globy_core-0.0.3/src/globy_core/ml/inference.py`

 * *Files identical despite different names*

### Comparing `globy_core-0.0.2/src/globy_core.egg-info/SOURCES.txt` & `globy_core-0.0.3/src/globy_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

