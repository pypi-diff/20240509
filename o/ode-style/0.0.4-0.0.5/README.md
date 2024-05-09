# Comparing `tmp/ode_style-0.0.4.tar.gz` & `tmp/ode_style-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ode_style-0.0.4.tar", last modified: Thu May  9 10:55:47 2024, max compression
+gzip compressed data, was "ode_style-0.0.5.tar", last modified: Thu May  9 11:17:28 2024, max compression
```

## Comparing `ode_style-0.0.4.tar` & `ode_style-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:55:47.322652 ode_style-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 10:55:47.322652 ode_style-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:55:43.000000 ode_style-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:55:47.318652 ode_style-0.0.4/ode/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/authentication_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/base_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/callback_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/chained_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/composite_job_disposable.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/dispatcher_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/error_output.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/guard_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/http_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/internet_connection_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/sequence_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/use_case_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/use_case_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/use_case_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-09 10:55:43.000000 ode_style-0.0.4/ode/value_out_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:55:47.318652 ode_style-0.0.4/ode_style.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 10:55:47.000000 ode_style-0.0.4/ode_style.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-09 10:55:47.000000 ode_style-0.0.4/ode_style.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:55:47.000000 ode_style-0.0.4/ode_style.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 10:55:47.000000 ode_style-0.0.4/ode_style.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:55:47.322652 ode_style-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-09 10:55:43.000000 ode_style-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:17:28.099196 ode_style-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 11:17:28.099196 ode_style-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:17:24.000000 ode_style-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:17:28.099196 ode_style-0.0.5/ode/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/authentication_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/base_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/callback_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/chained_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/composite_job_disposable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/dispatcher_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/error_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/guard_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/http_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/internet_connection_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/sequence_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/use_case_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/use_case_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/use_case_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-09 11:17:24.000000 ode_style-0.0.5/ode/value_out_put.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:17:28.099196 ode_style-0.0.5/ode_style.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 11:17:28.000000 ode_style-0.0.5/ode_style.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-09 11:17:28.000000 ode_style-0.0.5/ode_style.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:17:28.000000 ode_style-0.0.5/ode_style.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 11:17:28.000000 ode_style-0.0.5/ode_style.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:17:28.099196 ode_style-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-09 11:17:24.000000 ode_style-0.0.5/setup.py
```

### Comparing `ode_style-0.0.4/ode/base_controller.py` & `ode_style-0.0.5/ode/base_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Callable, Optional, TypeVar
 
 from ode.use_case import UseCase
 from ode.callback_decorator import CallbackDecorator
 
 from ode.composite_job_disposable import CompositeJobDisposable
 from ode.output import Output
-from ode.use_case_decorator import UseCaseDispatcher
+from ode.use_case_dispatcher import UseCaseDispatcher
 from ode.use_case_unit import UseCaseUnit
 
 P = TypeVar('P', bound=object)
 R = TypeVar('R', bound=object)
 
 class BaseController(object):
     composite_job_disposable: Optional[CompositeJobDisposable] = None
```

### Comparing `ode_style-0.0.4/ode/callback_decorator.py` & `ode_style-0.0.5/ode/callback_decorator.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.4/ode/chained_use_case.py` & `ode_style-0.0.5/ode/chained_use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.4/ode/composite_job_disposable.py` & `ode_style-0.0.5/ode/composite_job_disposable.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.4/ode/dispatcher_decorator.py` & `ode_style-0.0.5/ode/dispatcher_decorator.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.4/ode/sequence_use_case.py` & `ode_style-0.0.5/ode/sequence_use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.4/ode/use_case.py` & `ode_style-0.0.5/ode/use_case.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.4/ode/use_case_decorator.py` & `ode_style-0.0.5/ode/use_case_decorator.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.4/ode/use_case_dispatcher.py` & `ode_style-0.0.5/ode/use_case_dispatcher.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.4/ode/use_case_unit.py` & `ode_style-0.0.5/ode/use_case_unit.py`

 * *Files identical despite different names*

### Comparing `ode_style-0.0.4/ode_style.egg-info/SOURCES.txt` & `ode_style-0.0.5/ode_style.egg-info/SOURCES.txt`

 * *Files identical despite different names*

