# Comparing `tmp/streamlit_octostar_utils-0.0.2.tar.gz` & `tmp/streamlit_octostar_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_octostar_utils-0.0.2.tar", max compression
+gzip compressed data, was "streamlit_octostar_utils-0.0.3.tar", max compression
```

## Comparing `streamlit_octostar_utils-0.0.2.tar` & `streamlit_octostar_utils-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,23 @@
--rw-r--r--   0        0        0     1073 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/LICENSE
--rw-r--r--   0        0        0      324 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/README.md
--rw-r--r--   0        0        0      706 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        1 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/__init__.py
--rw-r--r--   0        0        0        1 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/core/__init__.py
--rw-r--r--   0        0        0        1 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/core/threading/__init__.py
--rw-r--r--   0        0        0     2224 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/core/threading/key_queue.py
--rw-r--r--   0        0        0       68 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/hello.py
--rw-r--r--   0        0        0        1 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/threading/__init__.py
--rw-r--r--   0        0        0     4627 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/threading/async_task_manager.py
--rw-r--r--   0        0        0     4078 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/threading/session_callback_manager.py
--rw-r--r--   0        0        0      809 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/threading/session_state_hot_swapper.py
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 streamlit_octostar_utils-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/LICENSE
+-rw-r--r--   0        0        0      324 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/README.md
+-rw-r--r--   0        0        0      741 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/api_crafter/__init__.py
+-rw-r--r--   0        0        0     4996 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/api_crafter/fastapi.py
+-rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/core/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/core/threading/__init__.py
+-rw-r--r--   0        0        0     2224 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/core/threading/key_queue.py
+-rw-r--r--   0        0        0       68 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/hello.py
+-rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/octostar/__init__.py
+-rw-r--r--   0        0        0     1690 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/octostar/client.py
+-rw-r--r--   0        0        0      210 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/octostar/context.py
+-rw-r--r--   0        0        0     1149 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/octostar/permissions.py
+-rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/ontology/__init__.py
+-rw-r--r--   0        0        0      137 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/ontology/inheritance.py
+-rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/style/__init__.py
+-rw-r--r--   0        0        0      605 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/style/common.py
+-rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/__init__.py
+-rw-r--r--   0        0        0     4591 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/async_task_manager.py
+-rw-r--r--   0        0        0     4001 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/session_callback_manager.py
+-rw-r--r--   0        0        0      809 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/session_state_hot_swapper.py
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 streamlit_octostar_utils-0.0.3/PKG-INFO
```

### Comparing `streamlit_octostar_utils-0.0.2/LICENSE` & `streamlit_octostar_utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_octostar_utils-0.0.2/pyproject.toml` & `streamlit_octostar_utils-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit-octostar-utils"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 license = "MIT"
 authors = ["Valerio Tonelli <tonellivalerio97@gmail.com>"]
 readme = "README.md"
 include = [
     "streamlit-octostar-utils/**/*"
 ]
@@ -20,12 +20,13 @@
 python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 pydantic = "^2.6.4"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 streamlit = "^1.33.0"
 streamlit-octostar-research = "^0.1.22"
+#octostar-python-client = "^1.0.0"
 mypy = "^1.9.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/core/threading/key_queue.py` & `streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/core/threading/key_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/threading/async_task_manager.py` & `streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/async_task_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import threading
 import time
 import traceback
 from enum import Enum
 import logging
 import streamlit as st
-from copy import deepcopy
 
 from ..core.threading.key_queue import KeyQueue
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 class AsyncTaskManager:
@@ -117,15 +116,15 @@
     def join_all(self):
         self.tasks_queue.join()
         self.kill_event.set()
         for worker in self.workers:
             worker.join()
     
     def get_result(self, task_id):
-        return deepcopy(self.results_queue.get_nowait(task_id))
+        return self.results_queue.get_nowait(task_id)
 
     def join(self, task_id):
         try:
             result = self.get_result(task_id)
             while result['status'].value < 10:
                 time.sleep(self._poll_freq)
                 result = self.get_result(task_id)
```

### Comparing `streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/threading/session_callback_manager.py` & `streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/session_callback_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,18 @@
         return SessionCallbackManager.instance
 
     def heartbeat(self):
         inactive_sessions = []
         for session_id, session_info in list(self.active_sessions.items()):
             if session_info['runtime'].is_active_session(session_id=session_info['context'].session_id):
                 heartbeat_fn = session_info.get('on_heartbeat')
-                if heartbeat_fn:
-                    heartbeat_fn(
-                        session_info['session_id'],
-                        session_info['context']
-                    )
+                heartbeat_fn(
+                    session_info['session_id'],
+                    session_info['context']
+                )
             else:
                 inactive_sessions.append(session_id)
         for session_id in inactive_sessions:
             self.on_session_end(session_id)
 
     def monitoring_thread(self):
         while self.monitoring_thread_active:
@@ -70,28 +69,27 @@
             self.active_sessions[session_id]['on_heartbeat'] = SessionCallbackManager.callback_wrapper(on_heartbeat)
             self.active_sessions[session_id]['on_session_end'] = SessionCallbackManager.callback_wrapper(on_session_end)
         self.on_session_start(session_id)
         return session_id
     
     def callback_wrapper(callback_fn):
         def _callback(session_id, st_context):
-            with SessionStateHotSwapper(st_context):
-                callback_fn(session_id)
+            if callback_fn:
+                with SessionStateHotSwapper(st_context):
+                    callback_fn(session_id)
         return _callback
     
     def on_session_start(self, session_id):
         start_fn = self.active_sessions[session_id].get('on_session_start')
-        if start_fn:
-            start_fn(self.active_sessions[session_id]['session_id'],
-                     self.active_sessions[session_id]['context'])
+        start_fn(self.active_sessions[session_id]['session_id'],
+                 self.active_sessions[session_id]['context'])
         self.start_monitoring()
 
     def on_session_end(self, session_id):
         with self.monitoring_thread_lock:
             if session_id in self.active_sessions:
                 end_fn = self.active_sessions[session_id].get('on_session_end')
-                if end_fn:
-                    end_fn(self.active_sessions[session_id]['session_id'],
-                           self.active_sessions[session_id]['context'])
+                end_fn(self.active_sessions[session_id]['session_id'],
+                       self.active_sessions[session_id]['context'])
                 self.active_sessions.pop(session_id, None)
                 if not self.active_sessions:
                     self.monitoring_thread_active = False
```

### Comparing `streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/threading/session_state_hot_swapper.py` & `streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/session_state_hot_swapper.py`

 * *Files identical despite different names*

### Comparing `streamlit_octostar_utils-0.0.2/PKG-INFO` & `streamlit_octostar_utils-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-octostar-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: MIT
 Author: Valerio Tonelli
 Author-email: tonellivalerio97@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

