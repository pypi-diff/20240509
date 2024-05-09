# Comparing `tmp/ode_style-0.0.3.tar.gz` & `tmp/ode_style-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ode_style-0.0.3.tar", last modified: Wed May  8 10:55:27 2024, max compression
+gzip compressed data, was "ode_style-0.0.4.tar", last modified: Thu May  9 10:55:47 2024, max compression
```

## Comparing `ode_style-0.0.3.tar` & `ode_style-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:55:27.308650 ode_style-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 10:55:27.308650 ode_style-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:55:23.000000 ode_style-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:55:27.304650 ode_style-0.0.3/ode/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/authentication_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/base_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/callback_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/chained_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/composite_job_disposable.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/error_output.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/guard_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/http_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/internet_connection_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/sequence_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/use_case_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/use_case_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/use_case_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/value_out_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:55:27.304650 ode_style-0.0.3/ode_style.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 10:55:27.000000 ode_style-0.0.3/ode_style.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-08 10:55:27.000000 ode_style-0.0.3/ode_style.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:55:27.000000 ode_style-0.0.3/ode_style.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 10:55:27.000000 ode_style-0.0.3/ode_style.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:55:27.308650 ode_style-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-08 10:55:23.000000 ode_style-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:55:47.322652 ode_style-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 10:55:47.322652 ode_style-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:55:43.000000 ode_style-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:55:47.318652 ode_style-0.0.4/ode/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/authentication_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/base_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/callback_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/chained_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/composite_job_disposable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/dispatcher_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/error_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/guard_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/http_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/internet_connection_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/sequence_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/use_case_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/use_case_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/use_case_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/value_out_put.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:55:47.318652 ode_style-0.0.4/ode_style.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 10:55:47.000000 ode_style-0.0.4/ode_style.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-09 10:55:47.000000 ode_style-0.0.4/ode_style.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:55:47.000000 ode_style-0.0.4/ode_style.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 10:55:47.000000 ode_style-0.0.4/ode_style.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:55:47.322652 ode_style-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-09 10:55:43.000000 ode_style-0.0.4/setup.py
```

### Comparing `ode_style-0.0.3/ode/base_controller.py` & `ode_style-0.0.4/ode/base_controller.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.3/ode/callback_decorator.py` & `ode_style-0.0.4/ode/callback_decorator.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.3/ode/chained_use_case.py` & `ode_style-0.0.4/ode/chained_use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.3/ode/composite_job_disposable.py` & `ode_style-0.0.4/ode/composite_job_disposable.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.3/ode/sequence_use_case.py` & `ode_style-0.0.4/ode/sequence_use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.3/ode/use_case.py` & `ode_style-0.0.4/ode/use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.3/ode/use_case_decorator.py` & `ode_style-0.0.4/ode/dispatcher_decorator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,29 @@
 from abc import abstractmethod
 from typing import TypeVar, Optional
 from ode.use_case import UseCase
 from ode.output import Output
+from ode.use_case_decorator import UseCaseDecorator
 import asyncio
 
 P = TypeVar('P')
 R = TypeVar('R')
 
-
-class UseCaseDecorator(UseCase[P, R]):
-    def __init__(self, use_case: UseCase[P, R]):
-        self.use_case = use_case
-
-    def on_error(self, error: Exception):
-        self.use_case.on_error(error)
-
-    def execute(self, param: Optional[P] = None) -> Output[R]:
-        return self.use_case.execute(param)
-
-    def on_result(self, output: Output[R]):
-        self.use_case.on_result(output)
-
-    def guard(self, param: Optional[P] = None) -> bool:
-        return self.use_case.guard(param)
-
-class UseCaseDispatcher:
+class DispatcherDecorator(UseCaseDecorator[P, R]):
     def __init__(
         self,
         use_case: UseCase[P, R],
         execute_on: asyncio.AbstractEventLoop = None,
         result_on: asyncio.AbstractEventLoop = None
     ):
-        self.decorator = self.DispatcherDecorator(use_case, execute_on, result_on)
-
-    async def dispatch(self, param: Optional[P] = None):
-        return self.decorator.dispatch(param)
+        super().__init__(use_case)
+        self.execute_on = execute_on
+        self.result_on = result_on
 
-    class DispatcherDecorator(UseCaseDecorator[P, R]):
-        def __init__(
-            self,
-            use_case: UseCase[P, R],
-            execute_on: asyncio.AbstractEventLoop = None,
-            result_on: asyncio.AbstractEventLoop = None
-        ):
-            super().__init__(use_case)
-            self.execute_on = execute_on
-            self.result_on = result_on
+    def dispatch(self, param: Optional[P] = None):
+        return asyncio.create_task(self.process(param), loop=self.execute_on)
 
-        async def dispatch(self, param: Optional[P] = None):
-            return asyncio.create_task(self.process(param), loop=self.execute_on)
-
-        async def on_error(self, error: Exception):
-            asyncio.to_thread(self.use_case.on_error, error, loop=self.result_on)
+    def on_error(self, error: Exception):
+        asyncio.to_thread(self.use_case.on_error, error, loop=self.result_on)
 
-        async def on_result(self, output: Output[R]):
-            asyncio.to_thread(self.use_case.on_result, output, loop=self.result_on)
+    def on_result(self, output: Output[R]):
+        asyncio.to_thread(self.use_case.on_result, output, loop=self.result_on)
```

### Comparing `ode_style-0.0.3/ode/use_case_unit.py` & `ode_style-0.0.4/ode/use_case_unit.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.3/ode_style.egg-info/SOURCES.txt` & `ode_style-0.0.4/ode_style.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.py
 ode/__init__.py
 ode/authentication_exception.py
 ode/base_controller.py
 ode/callback_decorator.py
 ode/chained_use_case.py
 ode/composite_job_disposable.py
+ode/dispatcher_decorator.py
 ode/error_output.py
 ode/guard_exception.py
 ode/http_exception.py
 ode/internet_connection_exception.py
 ode/output.py
 ode/sequence_use_case.py
 ode/use_case.py
```

