# Comparing `tmp/jupyter_jchannel-0.0.4.tar.gz` & `tmp/jupyter_jchannel-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_jchannel-0.0.4.tar", max compression
+gzip compressed data, was "jupyter_jchannel-0.0.5.tar", max compression
```

## Comparing `jupyter_jchannel-0.0.4.tar` & `jupyter_jchannel-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    14198 2024-02-24 11:59:10.599469 jupyter_jchannel-0.0.4/LICENSE
--rw-r--r--   0        0        0      538 2024-02-24 11:59:10.599469 jupyter_jchannel-0.0.4/README.md
--rw-r--r--   0        0        0      201 2024-02-24 11:59:10.599469 jupyter_jchannel-0.0.4/jchannel/__init__.py
--rw-r--r--   0        0        0       85 2024-02-24 11:59:10.599469 jupyter_jchannel-0.0.4/jchannel/frontend/__init__.py
--rw-r--r--   0        0        0     1370 2024-02-24 11:59:10.599469 jupyter_jchannel-0.0.4/jchannel/frontend/abstract.py
--rw-r--r--   0        0        0      509 2024-02-24 11:59:10.599469 jupyter_jchannel-0.0.4/jchannel/frontend/ipython.py
--rw-r--r--   0        0        0      266 2024-02-24 11:59:10.599469 jupyter_jchannel-0.0.4/jchannel/registry.py
--rw-r--r--   0        0        0     9695 2024-02-24 11:59:10.599469 jupyter_jchannel-0.0.4/jchannel/server.py
--rw-r--r--   0        0        0      731 2024-02-24 11:59:10.599469 jupyter_jchannel-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 jupyter_jchannel-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    14198 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/LICENSE
+-rw-r--r--   0        0        0      538 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/README.md
+-rw-r--r--   0        0        0      201 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/channel.py
+-rw-r--r--   0        0        0       85 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/frontend/__init__.py
+-rw-r--r--   0        0        0     1370 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/frontend/abstract.py
+-rw-r--r--   0        0        0      509 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/frontend/ipython.py
+-rw-r--r--   0        0        0      266 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/registry.py
+-rw-r--r--   0        0        0    13189 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/server.py
+-rw-r--r--   0        0        0      731 2024-05-09 19:04:09.203670 jupyter_jchannel-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 jupyter_jchannel-0.0.5/PKG-INFO
```

### Comparing `jupyter_jchannel-0.0.4/LICENSE` & `jupyter_jchannel-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_jchannel-0.0.4/README.md` & `jupyter_jchannel-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_jchannel-0.0.4/jchannel/frontend/abstract.py` & `jupyter_jchannel-0.0.5/jchannel/frontend/abstract.py`

 * *Files identical despite different names*

### Comparing `jupyter_jchannel-0.0.4/jchannel/server.py` & `jupyter_jchannel-0.0.5/jchannel/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import json
 import asyncio
 import logging
 
 from enum import Enum, auto
+from inspect import isawaitable
 from aiohttp import web, WSMsgType
+from jchannel.registry import registry
 from jchannel.frontend import frontend
+from jchannel.channel import Channel
 
 
 class StateError(Exception):
     pass
 
 
+class JavascriptError(Exception):
+    pass
+
+
 class DebugScenario(Enum):
     STOP_BEFORE_RESTART = auto()
     STOP_AFTER_BREAK = auto()
     CONNECT_BEFORE_BREAK = auto()
     CONNECT_BEFORE_CLEAN = auto()
     RECEIVE_BEFORE_CLEAN = auto()
     CATCH_BEFORE_CLEAN = auto()
@@ -94,24 +101,34 @@
             raise ValueError('Heartbeat must be positive')
 
         self.host = host
         self.port = port
         self.url = url
         self.heartbeat = heartbeat
         self.cleaned = None
-        self.sentinel = DebugSentinel()
 
         # None: user stoppage
         # web.WebSocketResponse: client connection
         self.connection = None
 
         # False: user stoppage
         # True: client disconnection
         self.disconnection = None
 
+        if __debug__:  # pragma: no cover
+            self.sentinel = DebugSentinel()
+
+        self.channels = {}
+
+    def open(self):
+        Channel(self)
+
+    def load(self):
+        frontend.run(f"jchannel.start('{self.url}')")
+
     def start(self):
         return asyncio.create_task(self._start())
 
     def stop(self):
         return asyncio.create_task(self._stop())
 
     async def __aenter__(self):
@@ -122,20 +139,21 @@
         await self._stop()
         return False
 
     async def _start(self, scenario=None):
         if self.cleaned is None:
             self.cleaned = asyncio.Event()
 
-            self.sentinel.enable(scenario)
-
             loop = asyncio.get_running_loop()
             self.connection = loop.create_future()
             self.disconnection = loop.create_future()
 
+            if __debug__:  # pragma: no cover
+                self.sentinel.enable(scenario)
+
             app = web.Application()
 
             app.socket = None
 
             app.on_shutdown.append(self._on_shutdown)
 
             app.add_routes([
@@ -146,20 +164,21 @@
 
             runner = web.AppRunner(app)
             await runner.setup()
 
             site = web.TCPSite(runner, self.host, self.port)
             await site.start()
 
-            frontend.run(f"jchannel.start('{self.url}')")
-
             asyncio.create_task(self._run(runner, site))
 
+            self.load()
+
     async def _stop(self):
-        await self.sentinel.wait_on_count(DebugScenario.STOP_AFTER_BREAK, 2)
+        if __debug__:  # pragma: no cover
+            await self.sentinel.wait_on_count(DebugScenario.STOP_AFTER_BREAK, 2)
 
         try:
             if self.cleaned is not None:
                 if self.connection is not None:
                     if not self.connection.done():
                         self.connection.set_result(None)
 
@@ -170,44 +189,48 @@
                         if restarting:
                             raise StateError('Cannot stop server while restarting')
                     else:
                         self.disconnection.set_result(False)
 
                 await self.cleaned.wait()
         finally:
-            await self.sentinel.set_and_yield(DebugScenario.STOP_BEFORE_RESTART)
+            if __debug__:  # pragma: no cover
+                await self.sentinel.set_and_yield(DebugScenario.STOP_BEFORE_RESTART)
 
     async def _run(self, runner, site):
         restarting = True
 
         while restarting:
             try:
                 await self.connection
             except asyncio.CancelledError:
                 pass
 
             restarting = await self.disconnection
 
             if restarting:
-                await self.sentinel.wait_on_count(DebugScenario.STOP_BEFORE_RESTART, 1)
+                if __debug__:  # pragma: no cover
+                    await self.sentinel.wait_on_count(DebugScenario.STOP_BEFORE_RESTART, 1)
 
                 loop = asyncio.get_running_loop()
                 self.connection = loop.create_future()
                 self.disconnection = loop.create_future()
             else:
-                await self.sentinel.set_and_yield(DebugScenario.DISCONNECT_AFTER_STOP)
-                await self.sentinel.wait_on_count(DebugScenario.CONNECT_BEFORE_BREAK, 1)
+                if __debug__:  # pragma: no cover
+                    await self.sentinel.set_and_yield(DebugScenario.DISCONNECT_AFTER_STOP)
+                    await self.sentinel.wait_on_count(DebugScenario.CONNECT_BEFORE_BREAK, 1)
 
                 self.connection = None
                 self.disconnection = None
 
-        await self.sentinel.set_and_yield(DebugScenario.STOP_AFTER_BREAK)
-        await self.sentinel.wait_on_count(DebugScenario.CONNECT_BEFORE_CLEAN, 1)
-        await self.sentinel.wait_on_count(DebugScenario.RECEIVE_BEFORE_CLEAN, 1)
-        await self.sentinel.wait_on_count(DebugScenario.CATCH_BEFORE_CLEAN, 1)
+        if __debug__:  # pragma: no cover
+            await self.sentinel.set_and_yield(DebugScenario.STOP_AFTER_BREAK)
+            await self.sentinel.wait_on_count(DebugScenario.CONNECT_BEFORE_CLEAN, 1)
+            await self.sentinel.wait_on_count(DebugScenario.RECEIVE_BEFORE_CLEAN, 1)
+            await self.sentinel.wait_on_count(DebugScenario.CATCH_BEFORE_CLEAN, 1)
 
         await site.stop()
         await runner.cleanup()
 
         self.cleaned.set()
         self.cleaned = None
 
@@ -216,36 +239,54 @@
 
         await socket.prepare(request)
 
         await socket.close()
 
         return socket
 
-    async def _send(self, body_type, body={}, timeout=3):
+    async def _accept(self, socket, body_type, body):
+        body['type'] = body_type
+
+        data = json.dumps(body)
+
+        await socket.send_str(data)
+
+    async def _send(self, body_type, input, channel_key, timeout):
         try:
             if self.connection is None:
                 socket = None
             else:
+                self.load()
+
                 try:
                     socket = await asyncio.wait_for(self.connection, timeout)
                 except asyncio.TimeoutError:
                     raise StateError('Client not connected: check the browser console for details')
 
             if socket is None:
                 raise StateError('Server not running')
 
             if not socket.prepared:
                 raise StateError('Server not prepared')
 
-            body['type'] = body_type
-            data = json.dumps(body)
+            payload = json.dumps(input)
+
+            loop = asyncio.get_running_loop()
+            future = loop.create_future()
 
-            await socket.send_str(data)
+            body = {
+                'future': registry.store(future),
+                'channel': channel_key,
+                'payload': payload,
+            }
+
+            await self._accept(socket, body_type, body)
         finally:
-            await self.sentinel.set_and_yield(DebugScenario.SEND_BEFORE_PREPARE)
+            if __debug__:  # pragma: no cover
+                await self.sentinel.set_and_yield(DebugScenario.SEND_BEFORE_PREPARE)
 
     async def _on_shutdown(self, app):
         if app.socket is not None:
             await app.socket.close()
 
     async def _handle_socket(self, request):
         if self.connection is None:
@@ -259,50 +300,97 @@
 
                 socket = await self._reject(request)
             else:
                 socket = web.WebSocketResponse(heartbeat=self.heartbeat)
 
                 self.connection.set_result(socket)
 
-                await self.sentinel.wait_on_count(DebugScenario.SEND_BEFORE_PREPARE, 1)
+                if __debug__:  # pragma: no cover
+                    await self.sentinel.wait_on_count(DebugScenario.SEND_BEFORE_PREPARE, 1)
 
                 await socket.prepare(request)
 
                 request.app.socket = socket
 
                 try:
                     async for message in socket:
-                        if message.type == WSMsgType.TEXT:
-                            body = json.loads(message.data)
-                            body_type = body.pop('type')
-
-                            match body_type:
-                                case _:
-                                    logging.error(f'Received unexpected body type {body_type}')
-                        else:
-                            logging.error(f'Received unexpected message type {message.type}')
+                        if message.type != WSMsgType.TEXT:
+                            raise TypeError(f'Received unexpected message type {message.type}')
+
+                        body = json.loads(message.data)
+
+                        future_key = body['future']
+                        channel_key = body['channel']
+                        payload = body.pop('payload')
+                        body_type = body.pop('type')
+
+                        match body_type:
+                            case 'closed':
+                                logging.warning('Unexpected channel closure')
+
+                                future = registry.retrieve(future_key)
+                                future.set_exception(StateError)
+                            case 'exception':
+                                future = registry.retrieve(future_key)
+                                future.set_exception(JavascriptError(payload))
+                            case 'result':
+                                output = json.loads(payload)
+
+                                future = registry.retrieve(future_key)
+                                future.set_result(output)
+                            case _:
+                                input = json.loads(payload)
+
+                                channel = self.channels[channel_key]
+
+                                try:
+                                    match body_type:
+                                        case 'echo':
+                                            body_type = 'result'
+                                        case 'call':
+                                            output = channel.handle_call(input['name'], input['args'])
+                                            if isawaitable(output):
+                                                output = await output
+                                            payload = json.dumps(output)
+                                            body_type = 'result'
+                                        case _:
+                                            payload = f'Received unexpected body type {body_type}'
+                                            body_type = 'exception'
+                                except Exception:
+                                    logging.exception('Caught handler exception')
+
+                                    payload = 'Check the notebook log for details'
+                                    body_type = 'exception'
+
+                                body['payload'] = payload
+
+                                await self._accept(socket, body_type, body)
 
-                        await self.sentinel.set_and_yield(DebugScenario.RECEIVE_BEFORE_CLEAN)
+                        if __debug__:  # pragma: no cover
+                            await self.sentinel.set_and_yield(DebugScenario.RECEIVE_BEFORE_CLEAN)
                 except Exception:
                     logging.exception('Caught unexpected exception')
 
-                    await self.sentinel.set_and_yield(DebugScenario.CATCH_BEFORE_CLEAN)
+                    if __debug__:  # pragma: no cover
+                        await self.sentinel.set_and_yield(DebugScenario.CATCH_BEFORE_CLEAN)
                 finally:
                     request.app.socket = None
 
-                await self.sentinel.wait_on_count(DebugScenario.DISCONNECT_AFTER_STOP, 1)
+                if __debug__:  # pragma: no cover
+                    await self.sentinel.wait_on_count(DebugScenario.DISCONNECT_AFTER_STOP, 1)
 
                 if self.disconnection is not None:
                     if not self.disconnection.done():
                         logging.warning('Unexpected client disconnection')
 
                         self.disconnection.set_result(True)
 
-        await self.sentinel.set_and_yield(DebugScenario.CONNECT_BEFORE_BREAK)
-        await self.sentinel.set_and_yield(DebugScenario.CONNECT_BEFORE_CLEAN)
+        if __debug__:  # pragma: no cover
+            await self.sentinel.set_and_yield(DebugScenario.CONNECT_BEFORE_BREAK)
+            await self.sentinel.set_and_yield(DebugScenario.CONNECT_BEFORE_CLEAN)
 
         return socket
 
     async def _handle_get(self, request):
         '''
         TODO
         '''
```

### Comparing `jupyter_jchannel-0.0.4/pyproject.toml` & `jupyter_jchannel-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "jupyter-jchannel"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = [
     "Marcelo Hashimoto <marcelo.hashimoto@gmail.com>"
 ]
 readme = "README.md"
 repository = "https://github.com/hashiprobr/jupyter-jchannel"
 packages = [
     { include = "jchannel" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-aiohttp = "^3.9.3"
+aiohttp = "^3.9.5"
 
 [tool.poetry.group.dev.dependencies]
-jupyterlab = "^4.1.2"
+jupyterlab = "^4.1.8"
 ipywidgets = "^8.1.2"
-autopep8 = "^2.0.4"
-pytest = "^7.4.4"
-pytest-asyncio = "~0.23.5"
-pytest-mock = "^3.12.0"
-pytest-cov = "^4.1.0"
-sphinx = "^7.2.6"
+autopep8 = "^2.1.0"
+pytest = "^8.2.0"
+pytest-asyncio = "~0.23.6"
+pytest-mock = "^3.14.0"
+pytest-cov = "^5.0.0"
+sphinx = "^7.3.7"
 
 [tool.poetry.scripts]
 notebooks = 'scripts:notebooks'
 tests = 'scripts:tests'
 docs = 'scripts:docs'
 
 [build-system]
```

### Comparing `jupyter_jchannel-0.0.4/PKG-INFO` & `jupyter_jchannel-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: jupyter-jchannel
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Home-page: https://github.com/hashiprobr/jupyter-jchannel
 Author: Marcelo Hashimoto
 Author-email: marcelo.hashimoto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
+Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Project-URL: Repository, https://github.com/hashiprobr/jupyter-jchannel
 Description-Content-Type: text/markdown
 
 jupyter-jchannel
 ----------------
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/jupyter-jchannel)](https://devguide.python.org/versions/)
```

