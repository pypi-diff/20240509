# Comparing `tmp/lambdaq-1.0.0-py3-none-any.whl.zip` & `tmp/lambdaq-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 7445 bytes, number of entries: 17
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-11 07:09 lambdaq/VERSION
--rw-r--r--  2.0 unx      298 b- defN 24-Apr-11 07:09 lambdaq/__init__.py
--rw-r--r--  2.0 unx     2839 b- defN 24-Apr-11 07:09 lambdaq/event_handler.py
--rw-r--r--  2.0 unx      961 b- defN 24-Apr-11 07:09 lambdaq/handle_event.py
--rw-r--r--  2.0 unx       89 b- defN 24-Apr-11 07:09 lambdaq/logging.py
--rw-r--r--  2.0 unx      291 b- defN 24-Apr-11 07:09 lambdaq/metadata.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-11 07:09 lambdaq/py.typed
--rw-r--r--  2.0 unx      215 b- defN 24-Apr-11 07:09 lambdaq/types/__init__.py
--rw-r--r--  2.0 unx       59 b- defN 24-Apr-11 07:09 lambdaq/types/message.py
--rw-r--r--  2.0 unx      215 b- defN 24-Apr-11 07:09 lambdaq/types/message_handler.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-11 07:09 lambdaq/types/py.typed
--rw-r--r--  2.0 unx       61 b- defN 24-Apr-11 07:09 lambdaq/types/response.py
--rw-r--r--  2.0 unx     1073 b- defN 24-Apr-11 07:09 lambdaq-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4159 b- defN 24-Apr-11 07:09 lambdaq-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 07:09 lambdaq-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-11 07:09 lambdaq-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1311 b- defN 24-Apr-11 07:09 lambdaq-1.0.0.dist-info/RECORD
-17 files, 11677 bytes uncompressed, 5289 bytes compressed:  54.7%
+Zip file size: 7741 bytes, number of entries: 17
+-rw-r--r--  2.0 unx        6 b- defN 24-May-09 06:45 lambdaq/VERSION
+-rw-r--r--  2.0 unx      298 b- defN 24-May-09 06:44 lambdaq/__init__.py
+-rw-r--r--  2.0 unx     3327 b- defN 24-May-09 06:44 lambdaq/event_handler.py
+-rw-r--r--  2.0 unx     1076 b- defN 24-May-09 06:44 lambdaq/handle_event.py
+-rw-r--r--  2.0 unx       89 b- defN 24-May-09 06:44 lambdaq/logging.py
+-rw-r--r--  2.0 unx      291 b- defN 24-May-09 06:44 lambdaq/metadata.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 06:44 lambdaq/py.typed
+-rw-r--r--  2.0 unx      215 b- defN 24-May-09 06:44 lambdaq/types/__init__.py
+-rw-r--r--  2.0 unx       59 b- defN 24-May-09 06:44 lambdaq/types/message.py
+-rw-r--r--  2.0 unx      215 b- defN 24-May-09 06:44 lambdaq/types/message_handler.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 06:44 lambdaq/types/py.typed
+-rw-r--r--  2.0 unx       61 b- defN 24-May-09 06:44 lambdaq/types/response.py
+-rw-r--r--  2.0 unx     1073 b- defN 24-May-09 06:45 lambdaq-2.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4415 b- defN 24-May-09 06:45 lambdaq-2.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-09 06:45 lambdaq-2.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-09 06:45 lambdaq-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1312 b- defN 24-May-09 06:45 lambdaq-2.0.0.dist-info/RECORD
+17 files, 12537 bytes uncompressed, 5585 bytes compressed:  55.5%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: lambdaq/types/py.typed
 Comment: 
 
 Filename: lambdaq/types/response.py
 Comment: 
 
-Filename: lambdaq-1.0.0.dist-info/LICENSE
+Filename: lambdaq-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: lambdaq-1.0.0.dist-info/METADATA
+Filename: lambdaq-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: lambdaq-1.0.0.dist-info/WHEEL
+Filename: lambdaq-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: lambdaq-1.0.0.dist-info/top_level.txt
+Filename: lambdaq-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: lambdaq-1.0.0.dist-info/RECORD
+Filename: lambdaq-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lambdaq/VERSION

```diff
@@ -1 +1 @@
-1.0.0
+2.0.0
```

## lambdaq/event_handler.py

```diff
@@ -5,20 +5,35 @@
 
 from lambdaq.logging import logger
 from lambdaq.metadata import Metadata
 from lambdaq.types import MessageHandler, TMessage, TResponse
 
 
 class EventHandler(Generic[TMessage, TResponse]):
+    """
+    Event handler.
+
+    Arguments:
+        event: Function event.
+
+        handler: Reference to a message-handling function.
+
+        session: Optional Boto3 session. A new session will be created by
+        default.
+
+        task_token_key: Key of the Step Functions task token in each message.
+        Step Functions state will not be published if this is omitted.
+    """
+
     def __init__(
         self,
         event: Any,
         handler: MessageHandler[TMessage, TResponse],
-        task_token_key: str,
         session: Session | None = None,
+        task_token_key: str | None = None,
     ) -> None:
         self.event = event
         self.handler = handler
 
         self.metadata = Metadata(
             session or Session(),
         )
@@ -74,30 +89,32 @@
             logger.info(
                 "Processing enqueued message %s/%s",
                 index + 1,
                 len(records),
             )
 
             body = loads(record["body"])
+            token = body[self.task_token_key] if self.task_token_key else None
             message = cast(TMessage, body)
-            token = str(message[self.task_token_key])  # type: ignore
 
             try:
                 response = self.handler(
                     message,
                     self.metadata,
                 )
 
             except Exception as ex:
-                self._send_task_state(
-                    token,
-                    exception=ex,
-                )
+                if token:
+                    self._send_task_state(
+                        token,
+                        exception=ex,
+                    )
 
                 continue
 
-            self._send_task_state(
-                token,
-                response=response,
-            )
+            if token:
+                self._send_task_state(
+                    token,
+                    response=response,
+                )
 
         return None
```

## lambdaq/handle_event.py

```diff
@@ -5,36 +5,37 @@
 from lambdaq.event_handler import EventHandler
 from lambdaq.types import MessageHandler, TMessage, TResponse
 
 
 def handle_event(
     event: Any,
     handler: MessageHandler[TMessage, TResponse],
-    task_token_key: str,
     session: Session | None = None,
+    task_token_key: str | None = None,
 ) -> TResponse | None:
     """
     Handles a Lambda function event.
 
     Arguments:
         event: Function event.
 
         handler: Reference to a message-handling function.
 
-        task_token_key: Key of the task token in each message.
-
         session: Optional Boto3 session. A new session will be created by
         default.
 
+        task_token_key: Key of the Step Functions task token in each message.
+        Step Functions state will not be submitted if this is omitted.
+
     Returns:
         Message handling response if the function was invoked directly, or
         `None` if the function was invoked by an SQS queue.
     """
 
     event_handler = EventHandler(
         event,
         handler,
-        task_token_key,
         session=session,
+        task_token_key=task_token_key,
     )
 
     return event_handler.handle_messages()
```

## Comparing `lambdaq-1.0.0.dist-info/LICENSE` & `lambdaq-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lambdaq-1.0.0.dist-info/METADATA` & `lambdaq-2.0.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdaq
-Version: 1.0.0
+Version: 2.0.0
 Summary: Helps you write Amazon Web Services Lambda functions called by Step Functions via SQS
 Author: Cariad Eccleston
 Author-email: cariad@cariad.earth
 License: MIT
 Project-URL: Project, https://github.com/cariad/lambdaq
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -50,23 +50,25 @@
 class Sum(TypedDict):
     result: int
 
 def main(event: Any, context: Any) -> Sum | None:
     return handle_event(
         event,
         perform_sum,
-        "task_token",
+        task_token_key="task_token",
     )
 
 def perform_sum(inputs: Inputs, metadata: Metadata) -> Sum:
     return Sum(result=inputs["x"] + inputs["y"])
 ```
 
 The `lambdaq.handle_event` function reads the invocation event, a reference to a message handler, and the key of the task token injected by the state machine.
 
+If the task token key is omitted then the work will still be performed, but the state won't be reported back to Step Functions. This would be used, for example, for functions invoked by SQS queues that don't need to report back any status.
+
 The message handler--`perform_sum` in this example--reads a strongly-typed message and returns a strongly-typed response.
 
 ## How does it work?
 
 Behind the scenes, LambdaQ checks if the event describes a single direct invocation or a collection of (one or more) messages plucked from an SQS queue.
 
 If the event describes a single direct invocation, LambdaQ calls the message handler then returns the response directly.
```

## Comparing `lambdaq-1.0.0.dist-info/RECORD` & `lambdaq-2.0.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-lambdaq/VERSION,sha256=WYVJhIUxBN9cNT4vaBoV_HkkdC-aLkaMKa8kjc5FzgM,6
+lambdaq/VERSION,sha256=wo_MpTY3vIjhJK8XJd8Ty5jGne3v1i-zzb4c22t2BiQ,6
 lambdaq/__init__.py,sha256=3AgOT9KfM6RfE3hmX25M3kleXgG_maIyntkpKLuiZec,298
-lambdaq/event_handler.py,sha256=iUs20j55mIvLiBHY0LeUXpcO3QPzl59X5C32qZlhJKQ,2839
-lambdaq/handle_event.py,sha256=aQuDwIhlRai6TnybW1lBspPppXeEYLJE5qoVP0H7LmE,961
+lambdaq/event_handler.py,sha256=nCaBszVIFcHhsCUVipP9mXyo3qPqSKT6gQy2TIvQKAc,3327
+lambdaq/handle_event.py,sha256=MgrIB7Q8EE5wK8yDOvxIhV622zNwCQLWD1CdC902YQo,1076
 lambdaq/logging.py,sha256=CRfvNy4vKBdAt2viao5lTtDFRrsq6tti9AjvBkCgu3s,89
 lambdaq/metadata.py,sha256=Wb4wZTRMUBKXfDhqfDHCxJoBuHkewlryQFIe4LPvlBU,291
 lambdaq/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lambdaq/types/__init__.py,sha256=R4k_2OeLdvKbyffFw3jWbZYuaWfDW9NThoNpnrXCspw,215
 lambdaq/types/message.py,sha256=ryIJnCraE0BDK2d_suET0VkN_MjvCIcjJE2cKxksiqo,59
 lambdaq/types/message_handler.py,sha256=7oAgprGRs-DoPzjykpDb5RfkXLc92_Jar-gWRpFZrr0,215
 lambdaq/types/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lambdaq/types/response.py,sha256=IKagKXpdVEhAurqdXDrDvNUGXTj67bYGQQrHQoTAXRk,61
-lambdaq-1.0.0.dist-info/LICENSE,sha256=4g0rxlvaGRJXe119BmPUqMzp-9r5q7R4oRnrncQJWvU,1073
-lambdaq-1.0.0.dist-info/METADATA,sha256=dd70InQ4Ca8YmY2Ztoc4MemWXUdx7UMEotbioT8xybI,4159
-lambdaq-1.0.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-lambdaq-1.0.0.dist-info/top_level.txt,sha256=43SyedRqVg0zyo4GDd6Cvr-v3LPzw-Z7WaxrRhpv07A,8
-lambdaq-1.0.0.dist-info/RECORD,,
+lambdaq-2.0.0.dist-info/LICENSE,sha256=4g0rxlvaGRJXe119BmPUqMzp-9r5q7R4oRnrncQJWvU,1073
+lambdaq-2.0.0.dist-info/METADATA,sha256=hjOa62QhOWZZ9OXDZOtaKfnq1PF-cPzJLABpsR1Bpt8,4415
+lambdaq-2.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+lambdaq-2.0.0.dist-info/top_level.txt,sha256=43SyedRqVg0zyo4GDd6Cvr-v3LPzw-Z7WaxrRhpv07A,8
+lambdaq-2.0.0.dist-info/RECORD,,
```

