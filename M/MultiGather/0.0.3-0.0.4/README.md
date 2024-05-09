# Comparing `tmp/multigather-0.0.3.tar.gz` & `tmp/multigather-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Admin\Desktop\gathernous\dist\.tmp-k2ih5vxr\multigather-0.0.3.tar", last modified: Thu May  9 07:44:08 2024, max compression
+gzip compressed data, was "C:\Users\Admin\Desktop\gathernous\dist\.tmp-hhgdr7ad\multigather-0.0.4.tar", last modified: Thu May  9 07:47:25 2024, max compression
```

## Comparing `multigather-0.0.3.tar` & `multigather-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 07:44:08.661065 multigather-0.0.3/
-drwxrwxrwx   0        0        0        0 2024-05-09 07:44:08.638834 multigather-0.0.3/MultiGather/
--rw-rw-rw-   0        0        0     1825 2024-05-09 07:37:15.000000 multigather-0.0.3/MultiGather/Client.py
--rw-rw-rw-   0        0        0      708 2024-05-09 07:31:32.000000 multigather-0.0.3/MultiGather/Types.py
--rw-rw-rw-   0        0        0       45 2024-05-09 07:42:54.000000 multigather-0.0.3/MultiGather/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 07:44:08.661065 multigather-0.0.3/MultiGather.egg-info/
--rw-rw-rw-   0        0        0     2256 2024-05-09 07:44:08.000000 multigather-0.0.3/MultiGather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-05-09 07:44:08.000000 multigather-0.0.3/MultiGather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 07:44:08.000000 multigather-0.0.3/MultiGather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-09 07:44:08.000000 multigather-0.0.3/MultiGather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2256 2024-05-09 07:44:08.661065 multigather-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1755 2024-05-09 07:37:15.000000 multigather-0.0.3/README.md
--rw-rw-rw-   0        0        0      504 2024-05-09 07:43:52.000000 multigather-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 07:44:08.666608 multigather-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 07:47:25.827041 multigather-0.0.4/
+drwxrwxrwx   0        0        0        0 2024-05-09 07:47:25.783414 multigather-0.0.4/MultiGather/
+-rw-rw-rw-   0        0        0     1836 2024-05-09 07:46:46.000000 multigather-0.0.4/MultiGather/Client.py
+-rw-rw-rw-   0        0        0      708 2024-05-09 07:31:32.000000 multigather-0.0.4/MultiGather/Types.py
+-rw-rw-rw-   0        0        0       45 2024-05-09 07:42:54.000000 multigather-0.0.4/MultiGather/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:47:25.827041 multigather-0.0.4/MultiGather.egg-info/
+-rw-rw-rw-   0        0        0     2256 2024-05-09 07:47:25.000000 multigather-0.0.4/MultiGather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-05-09 07:47:25.000000 multigather-0.0.4/MultiGather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 07:47:25.000000 multigather-0.0.4/MultiGather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-09 07:47:25.000000 multigather-0.0.4/MultiGather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2256 2024-05-09 07:47:25.827041 multigather-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1755 2024-05-09 07:37:15.000000 multigather-0.0.4/README.md
+-rw-rw-rw-   0        0        0      504 2024-05-09 07:47:07.000000 multigather-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 07:47:25.831066 multigather-0.0.4/setup.cfg
```

### Comparing `multigather-0.0.3/MultiGather/Client.py` & `multigather-0.0.4/MultiGather/Client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import aiohttp
 import asyncio
-from Types import Response, Request, Config
+from .Types import _Response, _Request, _Config
 
 class Connection:
-    def __init__(self, request: Config):
+    def __init__(self, request: _Config):
         self.connector = aiohttp.TCPConnector(limit=request.max_connection_limit)  # Set connection limit
-    async def sendRequest(self, request: Request):
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=Config.timeout)) as session:
+    async def sendRequest(self, request: _Request):
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=_Config.timeout)) as session:
             tasks = [self._sendRequest(request=request, session=session) for _ in range(request.amount)]
             return await asyncio.gather(*tasks) ## send Requests, and return them as generator.
 
-    async def _sendRequest(self, session: aiohttp.ClientSession, request: Request):
+    async def _sendRequest(self, session: aiohttp.ClientSession, request: _Request):
         try:
             async with session.request(
                     method=request.method, url=request.url,
                     headers=request.headers, json=request.json,
                     data=request.data, params=request.params
             ) as response:
                 response.raise_for_status()
                 content_type = response.headers.get('content-type')
                 json_content = None
                 if content_type and 'application/json' in content_type:
                     json_content = await response.json()
-                return Response(
+                return _Response(
                     status=response.status, url=str(response.url),
                     headers=response.headers, json=json_content,
                     text=await response.text(), content=await response.read()
                 )
         except (aiohttp.ClientError, aiohttp.ServerTimeoutError) as e:
-            return Response(status=609, url=request.url, headers={}, content=str(e), exception=True)
+            return _Response(status=609, url=request.url, headers={}, content=str(e), exception=True)
         except Exception as e:
-            return Response(status=609, url=request.url, headers={}, content=str(e), exception=True)
+            return _Response(status=609, url=request.url, headers={}, content=str(e), exception=True)
```

### Comparing `multigather-0.0.3/MultiGather/Types.py` & `multigather-0.0.4/MultiGather/Types.py`

 * *Files identical despite different names*

### Comparing `multigather-0.0.3/MultiGather.egg-info/PKG-INFO` & `multigather-0.0.4/MultiGather.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGather
-Version: 0.0.3
+Version: 0.0.4
 Summary: Send multiple requests using 3 lines of code!
 Author-email: "Mr. Mahdi" <any@hi2.in>
 Project-URL: Homepage, https://github.com/tm-sah/MultiGather
 Project-URL: Issues, https://github.com/tm-sah/MultiGather/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multigather-0.0.3/PKG-INFO` & `multigather-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGather
-Version: 0.0.3
+Version: 0.0.4
 Summary: Send multiple requests using 3 lines of code!
 Author-email: "Mr. Mahdi" <any@hi2.in>
 Project-URL: Homepage, https://github.com/tm-sah/MultiGather
 Project-URL: Issues, https://github.com/tm-sah/MultiGather/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multigather-0.0.3/README.md` & `multigather-0.0.4/README.md`

 * *Files identical despite different names*

