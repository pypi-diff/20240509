# Comparing `tmp/ambient_event_bus_client-0.1.1.tar.gz` & `tmp/ambient_event_bus_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_event_bus_client-0.1.1.tar", last modified: Wed May  8 22:23:17 2024, max compression
+gzip compressed data, was "ambient_event_bus_client-0.1.2.tar", last modified: Wed May  8 22:38:39 2024, max compression
```

## Comparing `ambient_event_bus_client-0.1.1.tar` & `ambient_event_bus_client-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 22:23:17.718714 ambient_event_bus_client-0.1.1/
--rw-r--r--   0 jose       (501) staff       (20)     1127 2024-05-08 22:23:17.718456 ambient_event_bus_client-0.1.1/PKG-INFO
--rw-r--r--   0 jose       (501) staff       (20)      569 2024-05-08 22:21:23.000000 ambient_event_bus_client-0.1.1/README.md
--rw-r--r--   0 jose       (501) staff       (20)       38 2024-05-08 22:23:17.718767 ambient_event_bus_client-0.1.1/setup.cfg
--rw-r--r--   0 jose       (501) staff       (20)      797 2024-05-08 22:22:48.000000 ambient_event_bus_client-0.1.1/setup.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 22:23:17.715631 ambient_event_bus_client-0.1.1/src/
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 22:23:17.716321 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/
--rw-r--r--   0 jose       (501) staff       (20)      194 2024-05-08 22:18:25.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/__init__.py
--rw-r--r--   0 jose       (501) staff       (20)     6088 2024-05-08 22:18:59.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/client.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 22:23:17.717737 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/models/
--rw-r--r--   0 jose       (501) staff       (20)        0 2024-05-03 17:03:20.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/models/__init__.py
--rw-r--r--   0 jose       (501) staff       (20)     4435 2024-05-08 22:18:31.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/models/event_api_models.py
--rw-r--r--   0 jose       (501) staff       (20)      266 2024-05-08 22:18:31.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/models/messages.py
--rw-r--r--   0 jose       (501) staff       (20)      213 2024-05-08 18:35:03.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/models/options.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 22:23:17.718135 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/
--rw-r--r--   0 jose       (501) staff       (20)     1127 2024-05-08 22:23:17.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/PKG-INFO
--rw-r--r--   0 jose       (501) staff       (20)      556 2024-05-08 22:23:17.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/SOURCES.txt
--rw-r--r--   0 jose       (501) staff       (20)        1 2024-05-08 22:23:17.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/dependency_links.txt
--rw-r--r--   0 jose       (501) staff       (20)       28 2024-05-08 22:23:17.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/requires.txt
--rw-r--r--   0 jose       (501) staff       (20)       25 2024-05-08 22:23:17.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:38:39.294057 ambient_event_bus_client-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-08 22:38:39.294057 ambient_event_bus_client-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-08 22:38:31.000000 ambient_event_bus_client-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:38:39.294057 ambient_event_bus_client-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-08 22:38:31.000000 ambient_event_bus_client-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:38:39.294057 ambient_event_bus_client-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:38:39.294057 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-08 22:38:31.000000 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-05-08 22:38:31.000000 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:38:39.294057 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:38:31.000000 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-08 22:38:31.000000 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client/models/event_api_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-08 22:38:31.000000 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client/models/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-08 22:38:31.000000 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client/models/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:38:39.294057 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-08 22:38:39.000000 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-08 22:38:39.000000 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:38:39.000000 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 22:38:39.000000 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 22:38:39.000000 ambient_event_bus_client-0.1.2/src/ambient_event_bus_client.egg-info/top_level.txt
```

### Comparing `ambient_event_bus_client-0.1.1/PKG-INFO` & `ambient_event_bus_client-0.1.2/src/ambient_event_bus_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
-Name: ambient_event_bus_client
-Version: 0.1.1
+Name: ambient-event-bus-client
+Version: 0.1.2
 Summary: A library to interact with the Ambient Labs Event Bus.
 Home-page: https://github.com/ambientlabscomputing/ambient-event-bus-client
 Author: Jose Catarino
 Author-email: jose@ambientlabscomputing.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: aiohttp
-Requires-Dist: websockets
-Requires-Dist: pydantic
 
 # Ambient Event Bus Client
 
 ## Typical usage example
 
 ```python
+from ambient_event_bus_client import Client, ClientOptions
 
-options = ClientOptions(event_api_url="http://localhost:8000", connection_service_url="http://localhost:8001", api_token = "my_token")
+options = ClientOptions(
+    event_api_url="http://localhost:8000",
+    connection_service_url="http://localhost:8001",
+    api_token = "my_token"
+)
 client = Client(options)
 await client.init_client() # ensure you are in an async context
 
 # add subscriptions
 await client.add_subscription(topic="test")
 
 # read messages from subscriptions
```

### Comparing `ambient_event_bus_client-0.1.1/README.md` & `ambient_event_bus_client-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Ambient Event Bus Client
 
 ## Typical usage example
 
 ```python
+from ambient_event_bus_client import Client, ClientOptions
 
-options = ClientOptions(event_api_url="http://localhost:8000", connection_service_url="http://localhost:8001", api_token = "my_token")
+options = ClientOptions(
+    event_api_url="http://localhost:8000",
+    connection_service_url="http://localhost:8001",
+    api_token = "my_token"
+)
 client = Client(options)
 await client.init_client() # ensure you are in an async context
 
 # add subscriptions
 await client.add_subscription(topic="test")
 
 # read messages from subscriptions
```

### Comparing `ambient_event_bus_client-0.1.1/setup.py` & `ambient_event_bus_client-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ambient_event_bus_client",
-    version="0.1.1",
+    version="0.1.2",
     description="A library to interact with the Ambient Labs Event Bus.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Jose Catarino",
     author_email="jose@ambientlabscomputing.com",
     url="https://github.com/ambientlabscomputing/ambient-event-bus-client",
     package_dir={"": "src"},
```

### Comparing `ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/client.py` & `ambient_event_bus_client-0.1.2/src/ambient_event_bus_client/client.py`

 * *Files identical despite different names*

### Comparing `ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/models/event_api_models.py` & `ambient_event_bus_client-0.1.2/src/ambient_event_bus_client/models/event_api_models.py`

 * *Files identical despite different names*

### Comparing `ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/PKG-INFO` & `ambient_event_bus_client-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: ambient_event_bus_client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to interact with the Ambient Labs Event Bus.
 Home-page: https://github.com/ambientlabscomputing/ambient-event-bus-client
 Author: Jose Catarino
 Author-email: jose@ambientlabscomputing.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: aiohttp
-Requires-Dist: websockets
-Requires-Dist: pydantic
 
 # Ambient Event Bus Client
 
 ## Typical usage example
 
 ```python
+from ambient_event_bus_client import Client, ClientOptions
 
-options = ClientOptions(event_api_url="http://localhost:8000", connection_service_url="http://localhost:8001", api_token = "my_token")
+options = ClientOptions(
+    event_api_url="http://localhost:8000",
+    connection_service_url="http://localhost:8001",
+    api_token = "my_token"
+)
 client = Client(options)
 await client.init_client() # ensure you are in an async context
 
 # add subscriptions
 await client.add_subscription(topic="test")
 
 # read messages from subscriptions
```

### Comparing `ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/SOURCES.txt` & `ambient_event_bus_client-0.1.2/src/ambient_event_bus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

