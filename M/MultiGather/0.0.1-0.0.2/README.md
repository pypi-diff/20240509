# Comparing `tmp/multigather-0.0.1.tar.gz` & `tmp/multigather-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Admin\Desktop\gathernous\dist\.tmp-78bkeczb\multigather-0.0.1.tar", last modified: Thu May  9 06:45:56 2024, max compression
+gzip compressed data, was "C:\Users\Admin\Desktop\gathernous\dist\.tmp-r49d4g8_\multigather-0.0.2.tar", last modified: Thu May  9 07:39:23 2024, max compression
```

## Comparing `multigather-0.0.1.tar` & `multigather-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 06:45:56.843564 multigather-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-09 06:45:56.812938 multigather-0.0.1/MultiGather/
--rw-rw-rw-   0        0        0     1821 2024-05-09 03:24:55.000000 multigather-0.0.1/MultiGather/Client.py
--rw-rw-rw-   0        0        0      708 2024-05-09 03:24:30.000000 multigather-0.0.1/MultiGather/Types.py
--rw-rw-rw-   0        0        0       43 2024-05-09 06:42:28.000000 multigather-0.0.1/MultiGather/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 06:45:56.836523 multigather-0.0.1/MultiGather.egg-info/
--rw-rw-rw-   0        0        0     2232 2024-05-09 06:45:56.000000 multigather-0.0.1/MultiGather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-05-09 06:45:56.000000 multigather-0.0.1/MultiGather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 06:45:56.000000 multigather-0.0.1/MultiGather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-09 06:45:56.000000 multigather-0.0.1/MultiGather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2232 2024-05-09 06:45:56.841499 multigather-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1730 2024-05-09 06:33:45.000000 multigather-0.0.1/README.md
--rw-rw-rw-   0        0        0      505 2024-05-09 06:44:25.000000 multigather-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 06:45:56.843564 multigather-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 07:39:23.645489 multigather-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-09 07:39:23.614869 multigather-0.0.2/MultiGather/
+-rw-rw-rw-   0        0        0     1825 2024-05-09 07:37:15.000000 multigather-0.0.2/MultiGather/Client.py
+-rw-rw-rw-   0        0        0      708 2024-05-09 07:31:32.000000 multigather-0.0.2/MultiGather/Types.py
+-rw-rw-rw-   0        0        0       43 2024-05-09 07:32:32.000000 multigather-0.0.2/MultiGather/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:39:23.642961 multigather-0.0.2/MultiGather.egg-info/
+-rw-rw-rw-   0        0        0     2256 2024-05-09 07:39:23.000000 multigather-0.0.2/MultiGather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-05-09 07:39:23.000000 multigather-0.0.2/MultiGather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 07:39:23.000000 multigather-0.0.2/MultiGather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-09 07:39:23.000000 multigather-0.0.2/MultiGather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2256 2024-05-09 07:39:23.643466 multigather-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1755 2024-05-09 07:37:15.000000 multigather-0.0.2/README.md
+-rw-rw-rw-   0        0        0      504 2024-05-09 07:38:21.000000 multigather-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 07:39:23.645489 multigather-0.0.2/setup.cfg
```

### Comparing `multigather-0.0.1/MultiGather/Client.py` & `multigather-0.0.2/MultiGather/Client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import aiohttp
 import asyncio
 from Types import Response, Request, Config
 
-class Client:
+class Connection:
     def __init__(self, request: Config):
         self.connector = aiohttp.TCPConnector(limit=request.max_connection_limit)  # Set connection limit
     async def sendRequest(self, request: Request):
         async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=Config.timeout)) as session:
             tasks = [self._sendRequest(request=request, session=session) for _ in range(request.amount)]
             return await asyncio.gather(*tasks) ## send Requests, and return them as generator.
```

### Comparing `multigather-0.0.1/MultiGather/Types.py` & `multigather-0.0.2/MultiGather/Types.py`

 * *Files identical despite different names*

### Comparing `multigather-0.0.1/MultiGather.egg-info/PKG-INFO` & `multigather-0.0.2/MultiGather.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: MultiGather
-Version: 0.0.1
+Version: 0.0.2
 Summary: Send multiple requests using 3 lines of code!
-Author-email: "Mr. Mahdi." <any@hi2.in>
+Author-email: "Mr. Mahdi" <any@hi2.in>
 Project-URL: Homepage, https://github.com/tm-sah/MultiGather
 Project-URL: Issues, https://github.com/tm-sah/MultiGather/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -18,24 +18,25 @@
 ```bash
 pip install MultiGather
 ```
 
 **Simple example for POST:**
 ```python
 import asyncio
-from MultiGather import Client, Config, Request
+from MultiGather import Client
+from MultiGather.Types import Config, Request
 
 # Replace with the actual URL for your POST endpoint
 url = "https://your-api-endpoint/posts"
 
 # Replace with the data you want to send in the POST request
 data = {"title": "New Post", "body": "This is a sample post content", "userId": 1}
 
 async def main():
-    client = Client(Config(timeout=10))  # Set timeout to 10 seconds (optional)
+    client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
 
     # Prepare a POST request object
     post_request = Request(method="POST", url=url, json=data, amount=5) ## gonna send 5 requests
 
     # Send the requests asynchronously and collect responses
     responses = await client.sendRequest(post_request)
 
@@ -44,29 +45,27 @@
         print(f"POST response status: {response.status}")
 
 asyncio.run(main())
 ```
 **Simple example for GET:**
 ```python
 import asyncio
-from MultiGather import Client, Config, Request
-
+from MultiGather import Client
+from MultiGather.Types import Config, Request
 # Replace with the actual URL for your GET endpoint
 url = "https://your-api-endpoint/posts"
 
 async def main():
-    client = Client(Config(timeout=10))  # Set timeout to 10 seconds (optional)
+    client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
 
     # Prepare a GET request object
     get_request = Request(method="GET", url=url, amount=5) # send 5 requests.
 
     # Send the requests asynchronously and collect responses
     responses = await client.sendRequest(get_request)
 
     # Print the status code for each response
     for response in responses:
         print(f"GET response status: {response.status}")
 
 asyncio.run(main())
 ```
-
-**Thanks for reading! I hope you contribute here.**
```

### Comparing `multigather-0.0.1/PKG-INFO` & `multigather-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: MultiGather
-Version: 0.0.1
+Version: 0.0.2
 Summary: Send multiple requests using 3 lines of code!
-Author-email: "Mr. Mahdi." <any@hi2.in>
+Author-email: "Mr. Mahdi" <any@hi2.in>
 Project-URL: Homepage, https://github.com/tm-sah/MultiGather
 Project-URL: Issues, https://github.com/tm-sah/MultiGather/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -18,24 +18,25 @@
 ```bash
 pip install MultiGather
 ```
 
 **Simple example for POST:**
 ```python
 import asyncio
-from MultiGather import Client, Config, Request
+from MultiGather import Client
+from MultiGather.Types import Config, Request
 
 # Replace with the actual URL for your POST endpoint
 url = "https://your-api-endpoint/posts"
 
 # Replace with the data you want to send in the POST request
 data = {"title": "New Post", "body": "This is a sample post content", "userId": 1}
 
 async def main():
-    client = Client(Config(timeout=10))  # Set timeout to 10 seconds (optional)
+    client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
 
     # Prepare a POST request object
     post_request = Request(method="POST", url=url, json=data, amount=5) ## gonna send 5 requests
 
     # Send the requests asynchronously and collect responses
     responses = await client.sendRequest(post_request)
 
@@ -44,29 +45,27 @@
         print(f"POST response status: {response.status}")
 
 asyncio.run(main())
 ```
 **Simple example for GET:**
 ```python
 import asyncio
-from MultiGather import Client, Config, Request
-
+from MultiGather import Client
+from MultiGather.Types import Config, Request
 # Replace with the actual URL for your GET endpoint
 url = "https://your-api-endpoint/posts"
 
 async def main():
-    client = Client(Config(timeout=10))  # Set timeout to 10 seconds (optional)
+    client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
 
     # Prepare a GET request object
     get_request = Request(method="GET", url=url, amount=5) # send 5 requests.
 
     # Send the requests asynchronously and collect responses
     responses = await client.sendRequest(get_request)
 
     # Print the status code for each response
     for response in responses:
         print(f"GET response status: {response.status}")
 
 asyncio.run(main())
 ```
-
-**Thanks for reading! I hope you contribute here.**
```

### Comparing `multigather-0.0.1/README.md` & `multigather-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 ```bash
 pip install MultiGather
 ```
 
 **Simple example for POST:**
 ```python
 import asyncio
-from MultiGather import Client, Config, Request
+from MultiGather import Client
+from MultiGather.Types import Config, Request
 
 # Replace with the actual URL for your POST endpoint
 url = "https://your-api-endpoint/posts"
 
 # Replace with the data you want to send in the POST request
 data = {"title": "New Post", "body": "This is a sample post content", "userId": 1}
 
 async def main():
-    client = Client(Config(timeout=10))  # Set timeout to 10 seconds (optional)
+    client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
 
     # Prepare a POST request object
     post_request = Request(method="POST", url=url, json=data, amount=5) ## gonna send 5 requests
 
     # Send the requests asynchronously and collect responses
     responses = await client.sendRequest(post_request)
 
@@ -31,29 +32,27 @@
         print(f"POST response status: {response.status}")
 
 asyncio.run(main())
 ```
 **Simple example for GET:**
 ```python
 import asyncio
-from MultiGather import Client, Config, Request
-
+from MultiGather import Client
+from MultiGather.Types import Config, Request
 # Replace with the actual URL for your GET endpoint
 url = "https://your-api-endpoint/posts"
 
 async def main():
-    client = Client(Config(timeout=10))  # Set timeout to 10 seconds (optional)
+    client = Client.Connection(Config(timeout=10))  # Set timeout to 10 seconds (optional)
 
     # Prepare a GET request object
     get_request = Request(method="GET", url=url, amount=5) # send 5 requests.
 
     # Send the requests asynchronously and collect responses
     responses = await client.sendRequest(get_request)
 
     # Print the status code for each response
     for response in responses:
         print(f"GET response status: {response.status}")
 
 asyncio.run(main())
-```
-
-**Thanks for reading! I hope you contribute here.**
+```
```

