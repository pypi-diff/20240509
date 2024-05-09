# Comparing `tmp/langgraph_sdk-0.1.4.tar.gz` & `tmp/langgraph_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_sdk-0.1.4.tar", max compression
+gzip compressed data, was "langgraph_sdk-0.1.5.tar", max compression
```

## Comparing `langgraph_sdk-0.1.4.tar` & `langgraph_sdk-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       12 2024-05-08 04:47:04.090972 langgraph_sdk-0.1.4/README.md
--rw-r--r--   0        0        0       70 2024-05-08 04:47:04.091058 langgraph_sdk-0.1.4/langgraph_sdk/__init__.py
--rw-r--r--   0        0        0     9616 2024-05-08 04:47:04.091177 langgraph_sdk-0.1.4/langgraph_sdk/client.py
--rw-r--r--   0        0        0     3212 2024-05-08 04:47:04.091240 langgraph_sdk-0.1.4/langgraph_sdk/schema.py
--rw-r--r--   0        0        0     1004 2024-05-08 05:02:56.476079 langgraph_sdk-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 langgraph_sdk-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-02 00:35:49.778092 langgraph_sdk-0.1.5/README.md
+-rw-r--r--   0        0        0       70 2024-05-02 17:41:01.189167 langgraph_sdk-0.1.5/langgraph_sdk/__init__.py
+-rw-r--r--   0        0        0    10894 2024-05-08 19:15:33.076998 langgraph_sdk-0.1.5/langgraph_sdk/client.py
+-rw-r--r--   0        0        0     3212 2024-05-03 18:21:58.272136 langgraph_sdk-0.1.5/langgraph_sdk/schema.py
+-rw-r--r--   0        0        0     1004 2024-05-08 19:48:34.135456 langgraph_sdk-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 langgraph_sdk-0.1.5/PKG-INFO
```

### Comparing `langgraph_sdk-0.1.4/langgraph_sdk/client.py` & `langgraph_sdk-0.1.5/langgraph_sdk/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import asyncio
 import sys
 from typing import Any, AsyncIterator, List, NamedTuple, Optional, Union
 
 import httpx
 import httpx_sse
+import orjson
 from httpx._types import QueryParamTypes
 
 from langgraph_sdk.schema import (
     Assistant,
     Config,
     GraphSchema,
     Metadata,
@@ -48,37 +50,39 @@
         r = await self.client.get(path, params=params)
         try:
             r.raise_for_status()
         except httpx.HTTPStatusError as e:
             if sys.version_info >= (3, 11):
                 e.add_note((await r.aread()).decode())
             raise e
-        return r.json()
+        return await decode_json(r)
 
     async def post(self, path: str, *, json: dict) -> dict:
         """Make a POST request."""
-        r = await self.client.post(path, json=json)
+        headers, content = await encode_json(json)
+        r = await self.client.post(path, headers=headers, content=content)
         try:
             r.raise_for_status()
         except httpx.HTTPStatusError as e:
             if sys.version_info >= (3, 11):
                 e.add_note((await r.aread()).decode())
             raise e
-        return r.json()
+        return await decode_json(r)
 
     async def put(self, path: str, *, json: dict) -> dict:
         """Make a PUT request."""
-        r = await self.client.put(path, json=json)
+        headers, content = await encode_json(json)
+        r = await self.client.put(path, headers=headers, content=content)
         try:
             r.raise_for_status()
         except httpx.HTTPStatusError as e:
             if sys.version_info >= (3, 11):
                 e.add_note((await r.aread()).decode())
             raise e
-        return r.json()
+        return await decode_json(r)
 
     async def delete(self, path: str) -> None:
         """Make a DELETE request."""
         r = await self.client.delete(path)
         try:
             r.raise_for_status()
         except httpx.HTTPStatusError as e:
@@ -86,23 +90,57 @@
                 e.add_note((await r.aread()).decode())
             raise e
 
     async def stream(
         self, path: str, method: str, *, json: dict = None
     ) -> AsyncIterator[StreamPart]:
         """Stream the results of a request using SSE."""
-        async with httpx_sse.aconnect_sse(self.client, method, path, json=json) as sse:
+        headers, content = await encode_json(json)
+        async with httpx_sse.aconnect_sse(
+            self.client, method, path, headers=headers, content=content
+        ) as sse:
             try:
                 sse.response.raise_for_status()
             except httpx.HTTPStatusError as e:
                 if sys.version_info >= (3, 11):
                     e.add_note((await sse.response.aread()).decode())
                 raise e
             async for event in sse.aiter_sse():
-                yield StreamPart(event.event, event.json() if event.data else None)
+                yield StreamPart(
+                    event.event, orjson.loads(event.data) if event.data else None
+                )
+
+
+def _orjson_default(obj: Any) -> Any:
+    if hasattr(obj, "model_dump") and callable(obj.model_dump):
+        return obj.model_dump()
+    elif hasattr(obj, "dict") and callable(obj.dict):
+        return obj.dict()
+    else:
+        raise TypeError(f"Object of type {type(obj)} is not JSON serializable")
+
+
+async def encode_json(json: Any) -> tuple[dict[str, str], bytes]:
+    body = await asyncio.get_running_loop().run_in_executor(
+        None,
+        orjson.dumps,
+        json,
+        _orjson_default,
+        orjson.OPT_SERIALIZE_NUMPY | orjson.OPT_NON_STR_KEYS,
+    )
+    content_length = str(len(body))
+    content_type = "application/json"
+    headers = {"Content-Length": content_length, "Content-Type": content_type}
+    return headers, body
+
+
+async def decode_json(r: httpx.Response) -> dict:
+    return await asyncio.get_running_loop().run_in_executor(
+        None, orjson.loads, await r.aread()
+    )
 
 
 class AssistantsClient:
     def __init__(self, http: HttpClient) -> None:
         self.http = http
 
     async def get(self, assistant_id: str) -> Assistant:
```

### Comparing `langgraph_sdk-0.1.4/langgraph_sdk/schema.py` & `langgraph_sdk-0.1.5/langgraph_sdk/schema.py`

 * *Files identical despite different names*

### Comparing `langgraph_sdk-0.1.4/pyproject.toml` & `langgraph_sdk-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langgraph-sdk"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.9.0,<4.0"
```

### Comparing `langgraph_sdk-0.1.4/PKG-INFO` & `langgraph_sdk-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: langgraph-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Nuno Campos
 Author-email: nuno@langchain.dev
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (==0.25.2)
 Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
 Requires-Dist: orjson (>=3.10.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 # langserve
```

