# Comparing `tmp/ambient_event_bus_client-0.1.0.tar.gz` & `tmp/ambient_event_bus_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_event_bus_client-0.1.0.tar", last modified: Wed May  8 21:56:21 2024, max compression
+gzip compressed data, was "ambient_event_bus_client-0.1.1.tar", last modified: Wed May  8 22:23:17 2024, max compression
```

## Comparing `ambient_event_bus_client-0.1.0.tar` & `ambient_event_bus_client-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 21:56:21.683874 ambient_event_bus_client-0.1.0/
--rw-r--r--   0 jose       (501) staff       (20)     1115 2024-05-08 21:56:21.683695 ambient_event_bus_client-0.1.0/PKG-INFO
--rw-r--r--   0 jose       (501) staff       (20)      557 2024-05-08 21:47:20.000000 ambient_event_bus_client-0.1.0/README.md
--rw-r--r--   0 jose       (501) staff       (20)       38 2024-05-08 21:56:21.683932 ambient_event_bus_client-0.1.0/setup.cfg
--rw-r--r--   0 jose       (501) staff       (20)      797 2024-05-08 21:53:26.000000 ambient_event_bus_client-0.1.0/setup.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 21:56:21.679554 ambient_event_bus_client-0.1.0/src/
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 21:56:21.681603 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client/
--rw-r--r--   0 jose       (501) staff       (20)      194 2024-05-03 18:53:14.000000 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client/__init__.py
--rw-r--r--   0 jose       (501) staff       (20)     5969 2024-05-08 21:38:41.000000 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client/client.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 21:56:21.683252 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client/models/
--rw-r--r--   0 jose       (501) staff       (20)        0 2024-05-03 17:03:20.000000 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client/models/__init__.py
--rw-r--r--   0 jose       (501) staff       (20)     4435 2024-05-08 19:33:33.000000 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client/models/event_api_models.py
--rw-r--r--   0 jose       (501) staff       (20)      264 2024-05-03 01:38:16.000000 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client/models/messages.py
--rw-r--r--   0 jose       (501) staff       (20)      213 2024-05-08 18:35:03.000000 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client/models/options.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 21:56:21.683470 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client.egg-info/
--rw-r--r--   0 jose       (501) staff       (20)     1115 2024-05-08 21:56:21.000000 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client.egg-info/PKG-INFO
--rw-r--r--   0 jose       (501) staff       (20)      556 2024-05-08 21:56:21.000000 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client.egg-info/SOURCES.txt
--rw-r--r--   0 jose       (501) staff       (20)        1 2024-05-08 21:56:21.000000 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client.egg-info/dependency_links.txt
--rw-r--r--   0 jose       (501) staff       (20)       28 2024-05-08 21:56:21.000000 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client.egg-info/requires.txt
--rw-r--r--   0 jose       (501) staff       (20)       25 2024-05-08 21:56:21.000000 ambient_event_bus_client-0.1.0/src/ambient_event_bus_client.egg-info/top_level.txt
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 22:23:17.718714 ambient_event_bus_client-0.1.1/
+-rw-r--r--   0 jose       (501) staff       (20)     1127 2024-05-08 22:23:17.718456 ambient_event_bus_client-0.1.1/PKG-INFO
+-rw-r--r--   0 jose       (501) staff       (20)      569 2024-05-08 22:21:23.000000 ambient_event_bus_client-0.1.1/README.md
+-rw-r--r--   0 jose       (501) staff       (20)       38 2024-05-08 22:23:17.718767 ambient_event_bus_client-0.1.1/setup.cfg
+-rw-r--r--   0 jose       (501) staff       (20)      797 2024-05-08 22:22:48.000000 ambient_event_bus_client-0.1.1/setup.py
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 22:23:17.715631 ambient_event_bus_client-0.1.1/src/
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 22:23:17.716321 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/
+-rw-r--r--   0 jose       (501) staff       (20)      194 2024-05-08 22:18:25.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/__init__.py
+-rw-r--r--   0 jose       (501) staff       (20)     6088 2024-05-08 22:18:59.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/client.py
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 22:23:17.717737 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/models/
+-rw-r--r--   0 jose       (501) staff       (20)        0 2024-05-03 17:03:20.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/models/__init__.py
+-rw-r--r--   0 jose       (501) staff       (20)     4435 2024-05-08 22:18:31.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/models/event_api_models.py
+-rw-r--r--   0 jose       (501) staff       (20)      266 2024-05-08 22:18:31.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/models/messages.py
+-rw-r--r--   0 jose       (501) staff       (20)      213 2024-05-08 18:35:03.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/models/options.py
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-08 22:23:17.718135 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/
+-rw-r--r--   0 jose       (501) staff       (20)     1127 2024-05-08 22:23:17.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/PKG-INFO
+-rw-r--r--   0 jose       (501) staff       (20)      556 2024-05-08 22:23:17.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jose       (501) staff       (20)        1 2024-05-08 22:23:17.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jose       (501) staff       (20)       28 2024-05-08 22:23:17.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/requires.txt
+-rw-r--r--   0 jose       (501) staff       (20)       25 2024-05-08 22:23:17.000000 ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/top_level.txt
```

### Comparing `ambient_event_bus_client-0.1.0/PKG-INFO` & `ambient_event_bus_client-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ambient_event_bus_client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to interact with the Ambient Labs Event Bus.
 Home-page: https://github.com/ambientlabscomputing/ambient-event-bus-client
 Author: Jose Catarino
 Author-email: jose@ambientlabscomputing.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: websockets
 Requires-Dist: pydantic
 
-# event-client
+# Ambient Event Bus Client
 
 ## Typical usage example
 
 ```python
 
 options = ClientOptions(event_api_url="http://localhost:8000", connection_service_url="http://localhost:8001", api_token = "my_token")
 client = Client(options)
```

### Comparing `ambient_event_bus_client-0.1.0/README.md` & `ambient_event_bus_client-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# event-client
+# Ambient Event Bus Client
 
 ## Typical usage example
 
 ```python
 
 options = ClientOptions(event_api_url="http://localhost:8000", connection_service_url="http://localhost:8001", api_token = "my_token")
 client = Client(options)
```

### Comparing `ambient_event_bus_client-0.1.0/setup.py` & `ambient_event_bus_client-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ambient_event_bus_client",
-    version="0.1.0",
+    version="0.1.1",
     description="A library to interact with the Ambient Labs Event Bus.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Jose Catarino",
     author_email="jose@ambientlabscomputing.com",
     url="https://github.com/ambientlabscomputing/ambient-event-bus-client",
     package_dir={"": "src"},
```

### Comparing `ambient_event_bus_client-0.1.0/src/ambient_event_bus_client/client.py` & `ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import asyncio
-import aiohttp
 import json
-from ambient_event_bus_client.models.event_api_models import Message, MessageCreate, Session, Subscription, SubscriptionCreate, Subscriber
-from ambient_event_bus_client.models.options import ClientOptions
-from contextlib import asynccontextmanager
-import websockets
 import logging
 import urllib.parse
 
+import aiohttp
+import websockets
+
+from ambient_event_bus_client.models.event_api_models import (
+    Message,
+    MessageCreate,
+    Session,
+    Subscriber,
+    Subscription,
+)
+from ambient_event_bus_client.models.options import ClientOptions
+
 
 class Client:
     """
     A client to interact with the Ambient Labs Event Bus.
 
     Parameters:
         - options: ClientOptions - The options for the client.
@@ -38,27 +45,32 @@
 
     # publish a message
     message = MessageCreate(topic="my_topic", message="my_message")
     await client.publish(message)
     ```
 
     """
+
     def __init__(self, options: ClientOptions) -> None:
         self._client_options = options
         self._session: Session | None = None
         logging.basicConfig()
         self.logger = logging.getLogger("event_bus_client")
         self.logger.setLevel(self._client_options.log_level)
 
     async def init_client(self) -> None:
         try:
             self.subscriber = await self._register_subscriber()
-            self.logger.debug("registered subscriber: %s", self.subscriber.model_dump_json(indent=4))
+            self.logger.debug(
+                "registered subscriber: %s", self.subscriber.model_dump_json(indent=4)
+            )
             self.session = await self._request_session()
-            self.logger.debug("registered session: %s", self.session.model_dump_json(indent=4))
+            self.logger.debug(
+                "registered session: %s", self.session.model_dump_json(indent=4)
+            )
         except aiohttp.ClientResponseError as e:
             self.logger.error("Failed to initialize client: %s", str(e))
             if e.status == 401:
                 raise Exception("Invalid API token, likely expired.")
             raise Exception(f"Failed to initialize client: {e}")
 
     async def _register_subscriber(self) -> Subscriber:
@@ -84,15 +96,17 @@
             try:
                 async with websockets.connect(self.uri) as websocket:
                     self.logger.debug("Connected")
                     async for message in websocket:
                         msg_data = json.loads(message)
                         yield Message.model_validate(msg_data)
             except websockets.exceptions.ConnectionClosedError as e:
-                self.logger.warning(f"Connection closed unexpectedly: {e}; retrying in 5 seconds.")
+                self.logger.warning(
+                    f"Connection closed unexpectedly: {e}; retrying in 5 seconds."
+                )
             except Exception as e:
                 self.logger.warning(f"An error occurred: {e}; retrying in 5 seconds.")
             await asyncio.sleep(5)
 
     async def publish(self, message: MessageCreate) -> None:
         self.logger.debug("publishing message:\n%s", message.model_dump_json(indent=4))
         try:
@@ -103,16 +117,20 @@
                 self.logger.debug("Connection closed: %s", str(e))
             else:
                 self.logger.error("Failed to publish message: %s", str(e))
                 raise e
 
     async def add_subscription(self, topic: str) -> Subscription:
         async with aiohttp.ClientSession() as session:
-            base_url = urllib.parse.urljoin(self._client_options.event_api_url, "/subscriptions/")
-            url_params = urllib.parse.urlencode({"topic": topic, "subscriber_id": self.subscriber.id})
+            base_url = urllib.parse.urljoin(
+                self._client_options.event_api_url, "/subscriptions/"
+            )
+            url_params = urllib.parse.urlencode(
+                {"topic": topic, "subscriber_id": self.subscriber.id}
+            )
             full_url = urllib.parse.urljoin(base_url, f"?{url_params}")
             self.logger.debug("full url: %s", full_url)
             async with session.post(
                 full_url,
                 headers={
                     "Authorization": f"Bearer {self._client_options.api_token}",
                     "Content-Type": "application/json",
@@ -130,15 +148,15 @@
     @session.setter
     def session(self, value: Session) -> None:
         self._session = value
 
     @property
     def subscriber(self) -> Subscriber:
         return self._subscriber
-    
+
     @subscriber.setter
     def subscriber(self, value: Subscriber) -> None:
         self._subscriber = value
 
     @property
     def uri(self) -> str:
         return f"{self._client_options.connection_service_url}/ws/{self.session.token}"
```

### Comparing `ambient_event_bus_client-0.1.0/src/ambient_event_bus_client/models/event_api_models.py` & `ambient_event_bus_client-0.1.1/src/ambient_event_bus_client/models/event_api_models.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,134 +8,134 @@
 from enum import Enum
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, Field
 
 
 class Connection(BaseModel):
-    id: Optional[int] = Field(None, title='Id')
+    id: Optional[int] = Field(None, title="Id")
     created_at: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.716266', title='Created At'
+        "2024-04-27T03:22:46.716266", title="Created At"
     )
-    session_id: Optional[int] = Field(None, title='Session Id')
-    is_active: Optional[bool] = Field(False, title='Is Active')
-    start_time: datetime = Field(..., title='Start Time')
-    end_time: Optional[datetime] = Field(None, title='End Time')
+    session_id: Optional[int] = Field(None, title="Session Id")
+    is_active: Optional[bool] = Field(False, title="Is Active")
+    start_time: datetime = Field(..., title="Start Time")
+    end_time: Optional[datetime] = Field(None, title="End Time")
 
 
 class CreateConnection(BaseModel):
-    session_id: int = Field(..., title='Session Id')
+    session_id: int = Field(..., title="Session Id")
     start_time: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.722048', title='Start Time'
+        "2024-04-27T03:22:46.722048", title="Start Time"
     )
 
 
 class ListResponseConnection(BaseModel):
     timestamp: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.717171', title='Timestamp'
+        "2024-04-27T03:22:46.717171", title="Timestamp"
     )
-    results: List[Connection] = Field(..., title='Results')
-    count: Optional[int] = Field(None, title='Count')
+    results: List[Connection] = Field(..., title="Results")
+    count: Optional[int] = Field(None, title="Count")
 
 
 class Message(BaseModel):
-    id: Optional[int] = Field(None, title='Id')
+    id: Optional[int] = Field(None, title="Id")
     created_at: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.716266', title='Created At'
+        "2024-04-27T03:22:46.716266", title="Created At"
     )
-    topic: str = Field(..., title='Topic')
-    message: str = Field(..., title='Message')
-    connection_id: Optional[int] = Field(None, title='Connection Id')
-    session_id: Optional[int] = Field(None, title='Session Id')
+    topic: str = Field(..., title="Topic")
+    message: str = Field(..., title="Message")
+    connection_id: Optional[int] = Field(None, title="Connection Id")
+    session_id: Optional[int] = Field(None, title="Session Id")
     timestamp: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.726648', title='Timestamp'
+        "2024-04-27T03:22:46.726648", title="Timestamp"
     )
 
 
 class MessageCreate(BaseModel):
-    topic: str = Field(..., title='Topic')
-    message: str = Field(..., title='Message')
+    topic: str = Field(..., title="Topic")
+    message: str = Field(..., title="Message")
 
 
 class Status(Enum):
-    CREATED = 'CREATED'
-    CONNECTED = 'CONNECTED'
-    DISCONNECTED = 'DISCONNECTED'
-    DELETED = 'DELETED'
-    ERROR = 'ERROR'
+    CREATED = "CREATED"
+    CONNECTED = "CONNECTED"
+    DISCONNECTED = "DISCONNECTED"
+    DELETED = "DELETED"
+    ERROR = "ERROR"
 
 
 class Subscriber(BaseModel):
-    id: Optional[int] = Field(None, title='Id')
+    id: Optional[int] = Field(None, title="Id")
     created_at: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.716266', title='Created At'
+        "2024-04-27T03:22:46.716266", title="Created At"
     )
-    user_id: str = Field(..., title='User Id')
+    user_id: str = Field(..., title="User Id")
 
 
 class SubscriptionCreate(BaseModel):
-    topic: str = Field(..., title='Topic')
-    subscriber_id: int = Field(..., title='Subscriber Id')
+    topic: str = Field(..., title="Topic")
+    subscriber_id: int = Field(..., title="Subscriber Id")
 
 
 class Subscription(BaseModel):
-    id: Optional[int] = Field(None, title='Id')
+    id: Optional[int] = Field(None, title="Id")
     created_at: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.716266', title='Created At'
+        "2024-04-27T03:22:46.716266", title="Created At"
     )
-    subscriber_id: Optional[int] = Field(None, title='Subscriber Id')
-    topic: str = Field(..., title='Topic')
+    subscriber_id: Optional[int] = Field(None, title="Subscriber Id")
+    topic: str = Field(..., title="Topic")
 
 
 class ValidationError(BaseModel):
-    loc: List[Union[str, int]] = Field(..., title='Location')
-    msg: str = Field(..., title='Message')
-    type: str = Field(..., title='Error Type')
+    loc: List[Union[str, int]] = Field(..., title="Location")
+    msg: str = Field(..., title="Message")
+    type: str = Field(..., title="Error Type")
 
 
 class HTTPValidationError(BaseModel):
-    detail: Optional[List[ValidationError]] = Field(None, title='Detail')
+    detail: Optional[List[ValidationError]] = Field(None, title="Detail")
 
 
 class ListResponseMessage(BaseModel):
     timestamp: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.717171', title='Timestamp'
+        "2024-04-27T03:22:46.717171", title="Timestamp"
     )
-    results: List[Message] = Field(..., title='Results')
-    count: Optional[int] = Field(None, title='Count')
+    results: List[Message] = Field(..., title="Results")
+    count: Optional[int] = Field(None, title="Count")
 
 
 class ListResponseSubscriber(BaseModel):
     timestamp: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.717171', title='Timestamp'
+        "2024-04-27T03:22:46.717171", title="Timestamp"
     )
-    results: List[Subscriber] = Field(..., title='Results')
-    count: Optional[int] = Field(None, title='Count')
+    results: List[Subscriber] = Field(..., title="Results")
+    count: Optional[int] = Field(None, title="Count")
 
 
 class ListResponseSubscription(BaseModel):
     timestamp: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.717171', title='Timestamp'
+        "2024-04-27T03:22:46.717171", title="Timestamp"
     )
-    results: List[Subscription] = Field(..., title='Results')
-    count: Optional[int] = Field(None, title='Count')
+    results: List[Subscription] = Field(..., title="Results")
+    count: Optional[int] = Field(None, title="Count")
 
 
 class Session(BaseModel):
-    id: Optional[int] = Field(None, title='Id')
+    id: Optional[int] = Field(None, title="Id")
     created_at: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.716266', title='Created At'
+        "2024-04-27T03:22:46.716266", title="Created At"
     )
-    subscriber_id: Optional[int] = Field(None, title='Subscriber Id')
-    status: Optional[Status] = 'CREATED'
+    subscriber_id: Optional[int] = Field(None, title="Subscriber Id")
+    status: Optional[Status] = "CREATED"
     last_connected: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.720380', title='Last Connected'
+        "2024-04-27T03:22:46.720380", title="Last Connected"
     )
-    token: str = Field(..., title='Token')
+    token: str = Field(..., title="Token")
 
 
 class ListResponseSession(BaseModel):
     timestamp: Optional[datetime] = Field(
-        '2024-04-27T03:22:46.717171', title='Timestamp'
+        "2024-04-27T03:22:46.717171", title="Timestamp"
     )
-    results: List[Session] = Field(..., title='Results')
-    count: Optional[int] = Field(None, title='Count')
+    results: List[Session] = Field(..., title="Results")
+    count: Optional[int] = Field(None, title="Count")
```

### Comparing `ambient_event_bus_client-0.1.0/src/ambient_event_bus_client.egg-info/PKG-INFO` & `ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ambient_event_bus_client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to interact with the Ambient Labs Event Bus.
 Home-page: https://github.com/ambientlabscomputing/ambient-event-bus-client
 Author: Jose Catarino
 Author-email: jose@ambientlabscomputing.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: websockets
 Requires-Dist: pydantic
 
-# event-client
+# Ambient Event Bus Client
 
 ## Typical usage example
 
 ```python
 
 options = ClientOptions(event_api_url="http://localhost:8000", connection_service_url="http://localhost:8001", api_token = "my_token")
 client = Client(options)
```

### Comparing `ambient_event_bus_client-0.1.0/src/ambient_event_bus_client.egg-info/SOURCES.txt` & `ambient_event_bus_client-0.1.1/src/ambient_event_bus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

