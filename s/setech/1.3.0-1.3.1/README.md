# Comparing `tmp/setech-1.3.0.tar.gz` & `tmp/setech-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setech-1.3.0.tar", last modified: Wed Apr 24 12:15:38 2024, max compression
+gzip compressed data, was "setech-1.3.1.tar", last modified: Thu May  9 10:54:41 2024, max compression
```

## Comparing `setech-1.3.0.tar` & `setech-1.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1059 2024-04-03 10:57:10.000000 setech-1.3.0/LICENCE
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5375 2024-04-24 12:15:38.740177 setech-1.3.0/PKG-INFO
--rw-r--r--   0 eriks     (1000) eriks     (1000)     4473 2024-04-03 21:15:13.000000 setech-1.3.0/README.md
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1932 2024-04-24 12:15:32.000000 setech-1.3.0/pyproject.toml
--rw-r--r--   0 eriks     (1000) eriks     (1000)       38 2024-04-24 12:15:38.740177 setech-1.3.0/setup.cfg
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.736844 setech-1.3.0/src/
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/src/setech/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      117 2024-04-24 12:15:32.000000 setech-1.3.0/src/setech/__init__.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/src/setech/api_client/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      115 2024-04-03 13:03:49.000000 setech-1.3.0/src/setech/api_client/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     6368 2024-04-16 11:12:02.000000 setech-1.3.0/src/setech/api_client/_base.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2332 2024-04-16 11:12:02.000000 setech-1.3.0/src/setech/api_client/async_client.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2237 2024-04-16 11:12:02.000000 setech-1.3.0/src/setech/api_client/sync_client.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/src/setech/constants/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      125 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/constants/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      519 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/constants/date.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/src/setech/logging/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      138 2024-04-10 13:57:32.000000 setech-1.3.0/src/setech/logging/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1394 2024-04-03 20:53:03.000000 setech-1.3.0/src/setech/logging/formatters.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1718 2024-04-04 13:24:48.000000 setech-1.3.0/src/setech/logging/handlers.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)        0 2024-03-19 14:21:21.000000 setech-1.3.0/src/setech/py.typed
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/src/setech/utils/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1276 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      878 2024-04-16 11:12:02.000000 setech-1.3.0/src/setech/utils/numeric.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     4031 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/parse.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5634 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/ssn.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2140 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/text.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      264 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/time.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1082 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/validators.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      318 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/various.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1336 2024-04-24 12:12:00.000000 setech-1.3.0/src/setech/utils/warnings.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-24 12:15:38.740177 setech-1.3.0/src/setech.egg-info/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5375 2024-04-24 12:15:38.000000 setech-1.3.0/src/setech.egg-info/PKG-INFO
--rw-r--r--   0 eriks     (1000) eriks     (1000)      786 2024-04-24 12:15:38.000000 setech-1.3.0/src/setech.egg-info/SOURCES.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)        1 2024-04-24 12:15:38.000000 setech-1.3.0/src/setech.egg-info/dependency_links.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)       65 2024-04-24 12:15:38.000000 setech-1.3.0/src/setech.egg-info/requires.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)        7 2024-04-24 12:15:38.000000 setech-1.3.0/src/setech.egg-info/top_level.txt
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 10:54:41.165842 setech-1.3.1/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1059 2024-04-03 10:57:10.000000 setech-1.3.1/LICENCE
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5375 2024-05-09 10:54:41.165842 setech-1.3.1/PKG-INFO
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     4473 2024-04-03 21:15:13.000000 setech-1.3.1/README.md
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1932 2024-05-09 10:54:27.000000 setech-1.3.1/pyproject.toml
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       38 2024-05-09 10:54:41.165842 setech-1.3.1/setup.cfg
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 10:54:41.162509 setech-1.3.1/src/
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 10:54:41.165842 setech-1.3.1/src/setech/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      117 2024-05-09 10:54:27.000000 setech-1.3.1/src/setech/__init__.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 10:54:41.165842 setech-1.3.1/src/setech/api_client/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      115 2024-04-03 13:03:49.000000 setech-1.3.1/src/setech/api_client/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     6693 2024-05-09 10:53:08.000000 setech-1.3.1/src/setech/api_client/_base.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2332 2024-04-16 11:12:02.000000 setech-1.3.1/src/setech/api_client/async_client.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2237 2024-04-16 11:12:02.000000 setech-1.3.1/src/setech/api_client/sync_client.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 10:54:41.165842 setech-1.3.1/src/setech/constants/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      125 2024-04-24 12:12:00.000000 setech-1.3.1/src/setech/constants/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      519 2024-04-24 12:12:00.000000 setech-1.3.1/src/setech/constants/date.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 10:54:41.165842 setech-1.3.1/src/setech/logging/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      138 2024-04-10 13:57:32.000000 setech-1.3.1/src/setech/logging/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1394 2024-04-03 20:53:03.000000 setech-1.3.1/src/setech/logging/formatters.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1718 2024-05-09 10:54:20.000000 setech-1.3.1/src/setech/logging/handlers.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        0 2024-03-19 14:21:21.000000 setech-1.3.1/src/setech/py.typed
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 10:54:41.165842 setech-1.3.1/src/setech/utils/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1276 2024-04-24 12:12:00.000000 setech-1.3.1/src/setech/utils/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      878 2024-04-16 11:12:02.000000 setech-1.3.1/src/setech/utils/numeric.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     4031 2024-04-24 12:12:00.000000 setech-1.3.1/src/setech/utils/parse.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5634 2024-04-24 12:12:00.000000 setech-1.3.1/src/setech/utils/ssn.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2140 2024-04-24 12:12:00.000000 setech-1.3.1/src/setech/utils/text.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      264 2024-04-24 12:12:00.000000 setech-1.3.1/src/setech/utils/time.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1082 2024-04-24 12:12:00.000000 setech-1.3.1/src/setech/utils/validators.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      318 2024-04-24 12:12:00.000000 setech-1.3.1/src/setech/utils/various.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1336 2024-04-24 12:12:00.000000 setech-1.3.1/src/setech/utils/warnings.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 10:54:41.165842 setech-1.3.1/src/setech.egg-info/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5375 2024-05-09 10:54:41.000000 setech-1.3.1/src/setech.egg-info/PKG-INFO
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      786 2024-05-09 10:54:41.000000 setech-1.3.1/src/setech.egg-info/SOURCES.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        1 2024-05-09 10:54:41.000000 setech-1.3.1/src/setech.egg-info/dependency_links.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       65 2024-05-09 10:54:41.000000 setech-1.3.1/src/setech.egg-info/requires.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        7 2024-05-09 10:54:41.000000 setech-1.3.1/src/setech.egg-info/top_level.txt
```

### Comparing `setech-1.3.0/LICENCE` & `setech-1.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/PKG-INFO` & `setech-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setech
-Version: 1.3.0
+Version: 1.3.1
 Summary: Setech utilities
 Author-email: Eriks Karls <eriks.karls@sefinance.lv>
 Project-URL: Homepage, https://pypi.org/project/setech/
 Keywords: setech,logging,api-client,utility,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setech-1.3.0/README.md` & `setech-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/pyproject.toml` & `setech-1.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 [tool.setuptools.dynamic]
 version = { attr = "setech.__version__" }
 
 
 [tool.bumpversion]
-current_version = "1.3.0"
+current_version = "1.3.1"
 commit = true
 tag = true
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
 allow_dirty = false
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
```

### Comparing `setech-1.3.0/src/setech/api_client/_base.py` & `setech-1.3.1/src/setech/api_client/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Coroutine
 
 import httpx
 from pydantic import HttpUrl
 
@@ -130,54 +131,57 @@
                 data=kwargs.get("data"),
                 json=kwargs.get("json"),
             ),
         )
         return request
 
     def _debug_log_request(self, method: str, full_url: str) -> None:
-        self._debug(f"Preparing {method} request for '{full_url}'")
+        self._debug(f"Preparing {method} request for '{full_url}'", stacklevel=4)
 
     def _debug_log_prepared_request(self, request: httpx.Request) -> None:
-        self._debug(f"Prepared {request.method} request to '{request.url}'", extra=request.__dict__)
+        self._debug(f"Prepared {request.method} request to '{request.url}'", extra=request.__dict__, stacklevel=4)
 
-    def _info_log_request_sending(self, request: httpx.Request, log_payload: Any) -> None:
+    def _info_log_request_sending(self, request: httpx.Request, log_payload: dict[str, Any]) -> None:
         self._info(
             f"Sending {request.method} request to '{request.url}'",
-            extra={"payload": shortify_log_extra_data(log_payload)},
+            extra={"payload": shortify_log_extra_data({k: v for k, v in log_payload.items() if v})},
+            stacklevel=4,
         )
 
     def _info_log_response(self, response: httpx.Response) -> None:
         try:
-            str_repr_content = response.content.decode("utf8")[:500]
+            if response.encoding == "application/json":
+                str_repr_content = json.dumps(shortify_log_extra_data(response.json()))[:500]
+                content = response.json()
+            else:
+                content = str_repr_content = response.content.decode("utf8")[:500]
             self._info(
                 f"Response {response.status_code=} {str_repr_content=}",
-                extra={"status_code": response.status_code, "content": str_repr_content},
+                extra={"status_code": response.status_code, "content": content, },
+                stacklevel=4,
             )
         except:  # noqa
-            self._info(
-                f"Response {response.status_code=}",
-                extra={"response": response.__dict__},
-            )
-
-    def _info(self, msg: str, *args: Any, **kwargs: Any) -> None:
-        self._log("INFO", f"[{self._nonce}] {msg}", *args, **kwargs)
+            self._info(f"Response {response.status_code=}", extra={"response": response.__dict__}, stacklevel=4)
 
     def _debug(self, msg: str, *args: Any, **kwargs: Any) -> None:
         self._log("DEBUG", f"[{self._nonce}] {msg}", *args, **kwargs)
 
+    def _info(self, msg: str, *args: Any, **kwargs: Any) -> None:
+        self._log("INFO", f"[{self._nonce}] {msg}", *args, **kwargs)
+
     def _warn(self, msg: str, *args: Any, **kwargs: Any) -> None:
         self._log("WARNING", f"[{self._nonce}] {msg}", *args, **kwargs)
 
     def _error(self, msg: str, *args: Any, **kwargs: Any) -> None:
         self._log("ERROR", f"[{self._nonce}] {msg}", *args, **kwargs)
 
     def _critical(self, msg: str, *args: Any, **kwargs: Any) -> None:
         self._log("CRITICAL", f"[{self._nonce}] {msg}", *args, **kwargs)
 
     def _log(
-        self, level: str, msg: object, *args: object, stacklevel: int = 5, extra: dict | None = None, **kwargs: Any
+        self, level: str, msg: object, *args: object, stacklevel: int = 2, extra: dict | None = None, **kwargs: Any
     ) -> None:
         extra = extra or {}
         extra.update(nonce=self._nonce)
         self._logger.log(
-            logging.getLevelNamesMapping()[level], msg, *args, stacklevel=stacklevel, extra=extra, **kwargs
+            logging.getLevelNamesMapping()[level], msg, *args, stacklevel=stacklevel+2, extra=extra, **kwargs
         )
```

### Comparing `setech-1.3.0/src/setech/api_client/async_client.py` & `setech-1.3.1/src/setech/api_client/async_client.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/src/setech/api_client/sync_client.py` & `setech-1.3.1/src/setech/api_client/sync_client.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/src/setech/constants/date.py` & `setech-1.3.1/src/setech/constants/date.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/src/setech/logging/formatters.py` & `setech-1.3.1/src/setech/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/src/setech/logging/handlers.py` & `setech-1.3.1/src/setech/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/src/setech/utils/__init__.py` & `setech-1.3.1/src/setech/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/src/setech/utils/numeric.py` & `setech-1.3.1/src/setech/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/src/setech/utils/parse.py` & `setech-1.3.1/src/setech/utils/parse.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/src/setech/utils/ssn.py` & `setech-1.3.1/src/setech/utils/ssn.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/src/setech/utils/text.py` & `setech-1.3.1/src/setech/utils/text.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/src/setech/utils/validators.py` & `setech-1.3.1/src/setech/utils/validators.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/src/setech/utils/warnings.py` & `setech-1.3.1/src/setech/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.0/src/setech.egg-info/PKG-INFO` & `setech-1.3.1/src/setech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setech
-Version: 1.3.0
+Version: 1.3.1
 Summary: Setech utilities
 Author-email: Eriks Karls <eriks.karls@sefinance.lv>
 Project-URL: Homepage, https://pypi.org/project/setech/
 Keywords: setech,logging,api-client,utility,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setech-1.3.0/src/setech.egg-info/SOURCES.txt` & `setech-1.3.1/src/setech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

