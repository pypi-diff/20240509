# Comparing `tmp/robotcode_debugger-0.82.0.tar.gz` & `tmp/robotcode_debugger-0.82.1.tar.gz`

## Comparing `robotcode_debugger-0.82.0.tar` & `robotcode_debugger-0.82.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/__version__.py
--rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/cli.py
--rw-r--r--   0        0        0    25783 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    69967 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/hooks.py
--rw-r--r--   0        0        0    12904 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0    12729 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/py.typed
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/run.py
--rw-r--r--   0        0        0    15850 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/launcher/cli.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/launcher/client.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/launcher/run.py
--rw-r--r--   0        0        0    13913 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/src/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/LICENSE.txt
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/README.md
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/pyproject.toml
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/__version__.py
+-rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/cli.py
+-rw-r--r--   0        0        0    25783 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    69793 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/hooks.py
+-rw-r--r--   0        0        0    12904 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0    12692 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/py.typed
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/run.py
+-rw-r--r--   0        0        0    15850 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/launcher/cli.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/launcher/client.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/launcher/run.py
+-rw-r--r--   0        0        0    13913 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/src/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/LICENSE.txt
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/README.md
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/pyproject.toml
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 robotcode_debugger-0.82.1/PKG-INFO
```

### Comparing `robotcode_debugger-0.82.0/src/robotcode/debugger/cli.py` & `robotcode_debugger-0.82.1/src/robotcode/debugger/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.82.0/src/robotcode/debugger/dap_types.py` & `robotcode_debugger-0.82.1/src/robotcode/debugger/dap_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.82.0/src/robotcode/debugger/debugger.py` & `robotcode_debugger-0.82.1/src/robotcode/debugger/debugger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from __future__ import annotations
-
-import asyncio
 import itertools
 import os
 import pathlib
 import re
 import reprlib
 import threading
 import time
@@ -153,15 +150,15 @@
     def __init__(self, thread_id: Any) -> None:
         super().__init__(f"Invalid thread id {thread_id}")
 
 
 class StackFrameEntry:
     def __init__(
         self,
-        parent: Optional[StackFrameEntry],
+        parent: Optional["StackFrameEntry"],
         context: Any,
         name: str,
         type: str,
         source: Optional[str],
         line: Optional[int],
         column: Optional[int] = None,
         handler: Optional[UserKeywordHandler] = None,
@@ -189,15 +186,15 @@
         self._local_marker = object()
         self._global_marker = object()
         self.stack_frames: Deque[StackFrameEntry] = deque()
 
     def __repr__(self) -> str:
         return f"StackFrameEntry({self.name!r}, {self.type!r}, {self.source!r}, {self.line!r}, {self.column!r})"
 
-    def get_first_or_self(self) -> StackFrameEntry:
+    def get_first_or_self(self) -> "StackFrameEntry":
         if self.stack_frames:
             return self.stack_frames[0]
         return self
 
     @property
     def id(self) -> int:
         return id(self)
@@ -256,22 +253,22 @@
             self.steps.append(data)
 
         def end_keyword(self, data: running.Keyword, result: result.Keyword) -> None:
             self.steps.pop()
 
 
 class Debugger:
-    __instance: ClassVar[Optional[Debugger]] = None
+    __instance: ClassVar[Optional["Debugger"]] = None
     __lock: ClassVar = threading.RLock()
     __inside_instance: ClassVar = False
 
     _logger = LoggingDescriptor()
 
     @classmethod
-    def instance(cls) -> Debugger:
+    def instance(cls) -> "Debugger":
         if cls.__instance is not None:
             return cls.__instance
         with cls.__lock:
             # re-check, perhaps it was created in the mean time...
             if cls.__instance is None:
                 cls.__inside_instance = True
                 try:
@@ -314,15 +311,14 @@
         self.hit_counts: Dict[HitCountEntry, int] = {}
         self.last_fail_message: Optional[str] = None
         self.stop_on_entry = False
         self._debug = True
         self.terminated = False
         self.attached = False
         self.path_mappings: List[PathMapping] = []
-        self.server_loop: Optional[asyncio.AbstractEventLoop] = None
 
         self._keyword_to_evaluate: Optional[Callable[..., Any]] = None
         self._evaluated_keyword_result: Any = None
         self._evaluate_keyword_event = threading.Event()
         self._evaluate_keyword_event.set()
         self._after_evaluate_keyword_event = threading.Event()
         self._after_evaluate_keyword_event.set()
@@ -913,22 +909,20 @@
                 self.wait_for_running()
 
     def end_suite(self, name: str, attributes: Dict[str, Any]) -> None:
         if self.debug:
             status = attributes.get("status", "")
 
             if status == "FAIL":
-                if self.server_loop:
-                    self.process_end_state(
-                        status,
-                        {"failed_suite"},
-                        "Suite failed.",
-                        f"Suite failed{f': {v}' if (v := attributes.get('message')) else ''}",
-                    )
-
+                self.process_end_state(
+                    status,
+                    {"failed_suite"},
+                    "Suite failed.",
+                    f"Suite failed{f': {v}' if (v := attributes.get('message')) else ''}",
+                )
                 self.wait_for_running()
 
         source = attributes.get("source")
         line_no = attributes.get("lineno", 1)
         type = "SUITE"
 
         self.remove_stackframe_entry(name, type, source, line_no)
```

### Comparing `robotcode_debugger-0.82.0/src/robotcode/debugger/listeners.py` & `robotcode_debugger-0.82.1/src/robotcode/debugger/listeners.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.82.0/src/robotcode/debugger/protocol.py` & `robotcode_debugger-0.82.1/src/robotcode/debugger/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     Any,
     Callable,
     Dict,
     Iterator,
     List,
     Mapping,
     Optional,
+    Set,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 from robotcode.core.concurrent import Task
@@ -77,14 +78,15 @@
     def __init__(self) -> None:
         super().__init__()
         self._sended_request_lock = threading.RLock()
         self._sended_request: OrderedDict[int, SendedRequestEntry] = OrderedDict()
         self._received_request_lock = threading.RLock()
         self._received_request: OrderedDict[int, asyncio.Future[Any]] = OrderedDict()
         self._initialized = False
+        self._running_handle_message_tasks: Set[asyncio.Future[Any]] = set()
 
     @_logger.call
     def send_message(self, message: ProtocolMessage) -> None:
         body = as_json(message, compact=True).encode(self.CHARSET)
 
         header = (f"Content-Length: {len(body)}\r\n\r\n").encode("ascii")
         if self.write_transport is not None:
@@ -136,22 +138,18 @@
             self._logger.exception(e)
             self.send_error(
                 f"Invalid Message: {type(e).__name__}: {e!s} -> {body!s}\n{traceback.format_exc()}",
                 error_message=Message(traceback.format_exc()),
             )
 
     def _handle_messages(self, iterator: Iterator[ProtocolMessage]) -> None:
-        def done(f: "asyncio.Future[Any]") -> None:
-            ex = f.exception()
-            if ex is not None and not isinstance(ex, asyncio.CancelledError):
-                self._logger.exception(ex, exc_info=ex)
-
         for m in iterator:
             task = asyncio.create_task(self.handle_message(m), name="handle_message")
-            task.add_done_callback(done)
+            self._running_handle_message_tasks.add(task)
+            task.add_done_callback(self._running_handle_message_tasks.discard)
 
     @_logger.call
     async def handle_message(self, message: ProtocolMessage) -> None:
         if isinstance(message, Request):
             self.handle_request(message)
         if isinstance(message, Event):
             self.handle_event(message)
```

### Comparing `robotcode_debugger-0.82.0/src/robotcode/debugger/run.py` & `robotcode_debugger-0.82.1/src/robotcode/debugger/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,14 @@
         Debugger.instance().output_messages = output_messages
         Debugger.instance().output_log = output_log
         Debugger.instance().group_output = group_output
         Debugger.instance().output_timestamps = output_timestamps
         Debugger.instance().colored_output = app.colored
         Debugger.instance().debug = debug
         Debugger.instance().set_main_thread(threading.current_thread())
-        Debugger.instance().server_loop = server.loop
 
         app.verbose("Start the debugger instance")
         Debugger.instance().start()
 
         exit_code = 0
         try:
             from robotcode.runner.cli.robot import robot
@@ -263,12 +262,12 @@
     except CancelledError:
         pass
     finally:
         if server.protocol.connected:
             server.protocol.terminate()
 
             if not server.protocol.wait_for_disconnected():
-                app.warning("Timeout to get disconnected from client")
+                app.verbose("Timeout to get disconnected from client")
 
         server.loop.stop()
 
     return exit_code
```

### Comparing `robotcode_debugger-0.82.0/src/robotcode/debugger/server.py` & `robotcode_debugger-0.82.1/src/robotcode/debugger/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.82.0/src/robotcode/debugger/launcher/cli.py` & `robotcode_debugger-0.82.1/src/robotcode/debugger/launcher/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.82.0/src/robotcode/debugger/launcher/client.py` & `robotcode_debugger-0.82.1/src/robotcode/debugger/launcher/client.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.82.0/src/robotcode/debugger/launcher/run.py` & `robotcode_debugger-0.82.1/src/robotcode/debugger/launcher/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.82.0/src/robotcode/debugger/launcher/server.py` & `robotcode_debugger-0.82.1/src/robotcode/debugger/launcher/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.82.0/.gitignore` & `robotcode_debugger-0.82.1/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.82.0/LICENSE.txt` & `robotcode_debugger-0.82.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.82.0/README.md` & `robotcode_debugger-0.82.1/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.82.0/pyproject.toml` & `robotcode_debugger-0.82.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.82.0",
-  "robotcode-runner==0.82.0",
+  "robotcode-jsonrpc2==0.82.1",
+  "robotcode-runner==0.82.1",
 ]
 
 [project.optional-dependencies]
 debugpy = ["debugpy"]
 
 [project.entry-points.robotcode]
 debugger = "robotcode.debugger.hooks"
```

### Comparing `robotcode_debugger-0.82.0/PKG-INFO` & `robotcode_debugger-0.82.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: robotcode-debugger
-Version: 0.82.0
+Version: 0.82.1
 Summary: RobotCode Debugger for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://opencollective.com/robotcode
 Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
 Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
 Project-URL: Source, https://github.com/robotcodedev/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.82.0
-Requires-Dist: robotcode-runner==0.82.0
+Requires-Dist: robotcode-jsonrpc2==0.82.1
+Requires-Dist: robotcode-runner==0.82.1
 Requires-Dist: robotframework>=4.1.0
 Provides-Extra: debugpy
 Requires-Dist: debugpy; extra == 'debugpy'
 Description-Content-Type: text/markdown
 
 # robotcode-debugger
```

