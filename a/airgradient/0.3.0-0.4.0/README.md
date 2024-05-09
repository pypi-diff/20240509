# Comparing `tmp/airgradient-0.3.0.tar.gz` & `tmp/airgradient-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airgradient-0.3.0.tar", max compression
+gzip compressed data, was "airgradient-0.4.0.tar", max compression
```

## Comparing `airgradient-0.3.0.tar` & `airgradient-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-04-13 11:01:43.923260 airgradient-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     4673 2024-04-13 11:01:43.923260 airgradient-0.3.0/README.md
--rw-r--r--   0        0        0     3856 2024-04-13 11:01:55.550829 airgradient-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      540 2024-04-13 11:01:43.927260 airgradient-0.3.0/src/airgradient/__init__.py
--rw-r--r--   0        0        0     3808 2024-04-13 11:01:43.927260 airgradient-0.3.0/src/airgradient/airgradient.py
--rw-r--r--   0        0        0      214 2024-04-13 11:01:43.927260 airgradient-0.3.0/src/airgradient/exceptions.py
--rw-r--r--   0        0        0     2733 2024-04-13 11:01:43.927260 airgradient-0.3.0/src/airgradient/models.py
--rw-r--r--   0        0        0        0 2024-04-13 11:01:43.927260 airgradient-0.3.0/src/airgradient/py.typed
--rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 airgradient-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-09 07:35:10.138172 airgradient-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     4673 2024-05-09 07:35:10.138172 airgradient-0.4.0/README.md
+-rw-r--r--   0        0        0     3857 2024-05-09 07:35:20.690251 airgradient-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      540 2024-05-09 07:35:10.138172 airgradient-0.4.0/src/airgradient/__init__.py
+-rw-r--r--   0        0        0     3893 2024-05-09 07:35:10.138172 airgradient-0.4.0/src/airgradient/airgradient.py
+-rw-r--r--   0        0        0      214 2024-05-09 07:35:10.138172 airgradient-0.4.0/src/airgradient/exceptions.py
+-rw-r--r--   0        0        0     2733 2024-05-09 07:35:10.138172 airgradient-0.4.0/src/airgradient/models.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:35:10.138172 airgradient-0.4.0/src/airgradient/py.typed
+-rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 airgradient-0.4.0/PKG-INFO
```

### Comparing `airgradient-0.3.0/LICENSE.md` & `airgradient-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `airgradient-0.3.0/README.md` & `airgradient-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `airgradient-0.3.0/pyproject.toml` & `airgradient-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airgradient"
-version = "0.3.0"
+version = "0.4.0"
 description = "Asynchronous Python client for AirGradient."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/airgradienthq/python-airgradient"
 repository = "https://github.com/airgradienthq/python-airgradient"
@@ -30,24 +30,24 @@
 yarl = ">=1.6.0"
 mashumaro = "^3.11"
 orjson = ">=3.9.0"
 
 [tool.poetry.group.dev.dependencies]
 codespell = "2.2.6"
 covdefaults = "2.3.0"
-coverage = {version = "7.4.4", extras = ["toml"]}
-mypy = "1.9.0"
+coverage = {version = "7.5.1", extras = ["toml"]}
+mypy = "1.10.0"
 pre-commit = "3.7.0"
 pre-commit-hooks = "4.6.0"
 pylint = "3.1.0"
-pytest = "8.1.1"
+pytest = "8.2.0"
 pytest-asyncio = "0.23.6"
 pytest-cov = "5.0.0"
-ruff = "0.3.7"
-safety = "3.1.0"
+ruff = "0.4.3"
+safety = "3.2.0"
 yamllint = "1.35.1"
 syrupy = "4.6.1"
 aioresponses = "0.7.6"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/airgradienthq/python-airgradient/issues"
 Changelog = "https://github.com/airgradienthq/python-airgradient/releases"
```

### Comparing `airgradient-0.3.0/src/airgradient/__init__.py` & `airgradient-0.4.0/src/airgradient/__init__.py`

 * *Files identical despite different names*

### Comparing `airgradient-0.3.0/src/airgradient/airgradient.py` & `airgradient-0.4.0/src/airgradient/airgradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Asynchronous Python client for AirGradient."""
 
 from __future__ import annotations
 
+from asyncio import timeout
 from dataclasses import dataclass
 from importlib import metadata
 from typing import TYPE_CHECKING, Any
 
 from aiohttp import ClientSession
 from aiohttp.hdrs import METH_GET, METH_PUT
 from yarl import URL
@@ -44,27 +45,28 @@
         data: dict[str, Any] | None = None,
     ) -> str:
         """Handle a request to AirGradient."""
         url = URL.build(scheme="http", host=self.host).joinpath(uri)
 
         headers = {
             "User-Agent": f"PythonAirGradient/{VERSION}",
-            "Accept": "application/json, text/plain, */*",
+            "Accept": "application/json",
         }
 
         if self.session is None:
             self.session = ClientSession()
             self._close_session = True
 
-        response = await self.session.request(
-            method,
-            url,
-            headers=headers,
-            data=data,
-        )
+        async with timeout(self.request_timeout):
+            response = await self.session.request(
+                method,
+                url,
+                headers=headers,
+                data=data,
+            )
 
         if response.status != 200:
             content_type = response.headers.get("Content-Type", "")
             text = await response.text()
             msg = "Unexpected response from AirGradient"
             raise AirGradientConnectionError(
                 msg,
```

### Comparing `airgradient-0.3.0/src/airgradient/models.py` & `airgradient-0.4.0/src/airgradient/models.py`

 * *Files identical despite different names*

### Comparing `airgradient-0.3.0/PKG-INFO` & `airgradient-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgradient
-Version: 0.3.0
+Version: 0.4.0
 Summary: Asynchronous Python client for AirGradient.
 Home-page: https://github.com/airgradienthq/python-airgradient
 License: MIT
 Keywords: Airgradient,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
```

