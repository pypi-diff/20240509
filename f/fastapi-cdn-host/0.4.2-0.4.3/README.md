# Comparing `tmp/fastapi_cdn_host-0.4.2.tar.gz` & `tmp/fastapi_cdn_host-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cdn_host-0.4.2.tar", max compression
+gzip compressed data, was "fastapi_cdn_host-0.4.3.tar", max compression
```

## Comparing `fastapi_cdn_host-0.4.2.tar` & `fastapi_cdn_host-0.4.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1086 2023-12-03 10:13:01.678736 fastapi_cdn_host-0.4.2/LICENSE
--rw-r--r--   0        0        0     2349 2024-04-19 02:58:25.003391 fastapi_cdn_host-0.4.2/README.md
--rw-r--r--   0        0        0      387 2024-04-18 09:57:50.755481 fastapi_cdn_host-0.4.2/fastapi_cdn_host/__init__.py
--rw-r--r--   0        0        0    18466 2024-04-11 07:19:56.278335 fastapi_cdn_host-0.4.2/fastapi_cdn_host/client.py
--rw-r--r--   0        0        0        0 2023-12-06 13:45:09.634356 fastapi_cdn_host-0.4.2/fastapi_cdn_host/py.typed
--rw-r--r--   0        0        0     1079 2024-04-19 02:05:58.080259 fastapi_cdn_host-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2908 1970-01-01 00:00:00.000000 fastapi_cdn_host-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-12-03 10:13:01.678736 fastapi_cdn_host-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2349 2024-04-19 02:58:25.003391 fastapi_cdn_host-0.4.3/README.md
+-rw-r--r--   0        0        0      387 2024-04-18 09:57:50.755481 fastapi_cdn_host-0.4.3/fastapi_cdn_host/__init__.py
+-rw-r--r--   0        0        0    18513 2024-05-09 08:01:07.579656 fastapi_cdn_host-0.4.3/fastapi_cdn_host/client.py
+-rw-r--r--   0        0        0        0 2023-12-06 13:45:09.634356 fastapi_cdn_host-0.4.3/fastapi_cdn_host/py.typed
+-rw-r--r--   0        0        0     1141 2024-05-09 06:53:12.757143 fastapi_cdn_host-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2908 1970-01-01 00:00:00.000000 fastapi_cdn_host-0.4.3/PKG-INFO
```

### Comparing `fastapi_cdn_host-0.4.2/LICENSE` & `fastapi_cdn_host-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cdn_host-0.4.2/README.md` & `fastapi_cdn_host-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_cdn_host-0.4.2/fastapi_cdn_host/client.py` & `fastapi_cdn_host-0.4.3/fastapi_cdn_host/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import re
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
+from ssl import SSLError
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
 import anyio
 import httpx
 from fastapi import FastAPI, Request
 from fastapi.datastructures import URL
 from fastapi.openapi.docs import get_redoc_html, get_swagger_ui_html
@@ -124,14 +125,15 @@
         try:
             r = await client.get(url)
         except (
             httpx.ConnectError,
             httpx.ReadError,
             httpx.ConnectTimeout,
             httpx.ReadTimeout,
+            SSLError,
         ):
             ...
         else:
             if r.status_code < 300:
                 results[index] = r.content
 
     @classmethod
```

### Comparing `fastapi_cdn_host-0.4.2/pyproject.toml` & `fastapi_cdn_host-0.4.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 [tool.poetry]
 name = "fastapi-cdn-host"
-version = "0.4.2"
+version = "0.4.3"
 description = ""
 authors = ["Waket Zheng <waketzheng@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = {version = ">=0.100"}
 httpx = {version = ">=0.23"}
 
 
 [tool.poetry.group.dev.dependencies]
 fast-dev-cli = {extras = ["all"], version=">=0.7.0", python=">=3.11"}
-asyncur = {version=">=0.4.2", python=">=3.11"}
-uvicorn = {extras = ["standard"], version = "*"}
+pre-commit = {version=">=3.7.0", python=">=3.11"}
+asyncur = {version=">=0.5.0", python=">=3.11"}
 bandit = "^1.7.8"
-ruff = ">=0.3"
-mypy = "*"
-pytest = "*"
-coverage = "*"
-starlette = "*"
-pydantic = "*"
-click = "*"
+ruff = "^0.4.3"
+mypy = "^1.10.0"
+pytest = "^8.2.0"
+coverage = "^7.5.1"
+click = "^8.1.7"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 pretty = true
 ignore_missing_imports = true
 explicit_package_bases = true
 check_untyped_defs = true
 
+[tool.ruff.lint]
+extend-select = ["I"]
+
 [tool.ruff.lint.per-file-ignores]
 "test_*.py" = ["E501"]
+"examples/main.py" = ["I001"]
 
 [tool.coverage.run]
 branch = true
 parallel=true
 source = ["fastapi_cdn_host"]
 [tool.coverage.report]
 omit = ["*/tests/*", "test_*"]
```

### Comparing `fastapi_cdn_host-0.4.2/PKG-INFO` & `fastapi_cdn_host-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cdn-host
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

