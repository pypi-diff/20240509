# Comparing `tmp/fluxional-0.1.4.tar.gz` & `tmp/fluxional-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxional-0.1.4.tar", max compression
+gzip compressed data, was "fluxional-0.1.5.tar", max compression
```

## Comparing `fluxional-0.1.4.tar` & `fluxional-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2024-04-28 17:10:39.085356 fluxional-0.1.4/LICENSE
--rw-r--r--   0        0        0     3908 2024-04-29 21:12:21.619975 fluxional-0.1.4/README.md
--rw-r--r--   0        0        0      421 2024-04-30 22:07:55.223192 fluxional-0.1.4/fluxional/__init__.py
--rw-r--r--   0        0        0       85 2024-04-28 18:14:21.913877 fluxional-0.1.4/fluxional/__main__.py
--rw-r--r--   0        0        0     1429 2024-04-28 18:14:21.923877 fluxional-0.1.4/fluxional/cli/__init__.py
--rw-r--r--   0        0        0      397 2024-04-28 18:14:21.923877 fluxional-0.1.4/fluxional/core/__init__.py
--rw-r--r--   0        0        0    21402 2024-04-28 18:14:21.933877 fluxional-0.1.4/fluxional/core/app.py
--rw-r--r--   0        0        0     6976 2024-04-28 18:14:21.933877 fluxional-0.1.4/fluxional/core/core.py
--rw-r--r--   0        0        0     2927 2024-04-28 18:14:21.933877 fluxional-0.1.4/fluxional/core/events.py
--rw-r--r--   0        0        0    11708 2024-04-28 18:14:21.943877 fluxional-0.1.4/fluxional/core/handlers.py
--rw-r--r--   0        0        0        1 2024-04-28 18:14:21.943877 fluxional-0.1.4/fluxional/core/infrastructure/__init__.py
--rw-r--r--   0        0        0    19676 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/infrastructure/base.py
--rw-r--r--   0        0        0     7699 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/infrastructure/cdk.py
--rw-r--r--   0        0        0     9554 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/infrastructure/resources.py
--rw-r--r--   0        0        0      816 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/infrastructure/types.py
--rw-r--r--   0        0        0     5818 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/logic.py
--rw-r--r--   0        0        0     8343 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/settings.py
--rw-r--r--   0        0        0     4045 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/tools.py
--rw-r--r--   0        0        0     5158 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/core/types.py
--rw-r--r--   0        0        0       74 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/deployment/__init__.py
--rw-r--r--   0        0        0     1164 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/deployment/constants.py
--rw-r--r--   0        0        0    15517 2024-04-30 22:02:31.375706 fluxional-0.1.4/fluxional/deployment/engine.py
--rw-r--r--   0        0        0      345 2024-04-28 18:14:21.953877 fluxional-0.1.4/fluxional/deployment/exceptions.py
--rw-r--r--   0        0        0        1 2024-04-30 22:01:04.012000 fluxional-0.1.4/fluxional/deployment/utils.py
--rw-r--r--   0        0        0     3652 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/dev/__init__.py
--rw-r--r--   0        0        0     3003 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/dev/client.py
--rw-r--r--   0        0        0     3350 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/dev/runner.py
--rw-r--r--   0        0        0      326 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/py.typed
--rw-r--r--   0        0        0      461 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/types.py
--rw-r--r--   0        0        0      935 2024-04-28 18:14:21.963877 fluxional-0.1.4/fluxional/utils.py
--rw-r--r--   0        0        0     1151 2024-04-30 22:08:15.593233 fluxional-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 fluxional-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-28 17:10:39.085356 fluxional-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3908 2024-04-29 21:12:21.619975 fluxional-0.1.5/README.md
+-rw-r--r--   0        0        0      421 2024-05-08 21:22:01.016099 fluxional-0.1.5/fluxional/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-28 18:14:21.913877 fluxional-0.1.5/fluxional/__main__.py
+-rw-r--r--   0        0        0     1429 2024-04-28 18:14:21.923877 fluxional-0.1.5/fluxional/cli/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-28 18:14:21.923877 fluxional-0.1.5/fluxional/core/__init__.py
+-rw-r--r--   0        0        0    21690 2024-05-09 01:12:44.131127 fluxional-0.1.5/fluxional/core/app.py
+-rw-r--r--   0        0        0     6976 2024-04-28 18:14:21.933877 fluxional-0.1.5/fluxional/core/core.py
+-rw-r--r--   0        0        0     2927 2024-04-28 18:14:21.933877 fluxional-0.1.5/fluxional/core/events.py
+-rw-r--r--   0        0        0    11708 2024-04-28 18:14:21.943877 fluxional-0.1.5/fluxional/core/handlers.py
+-rw-r--r--   0        0        0        1 2024-04-28 18:14:21.943877 fluxional-0.1.5/fluxional/core/infrastructure/__init__.py
+-rw-r--r--   0        0        0    19676 2024-04-28 18:14:21.953877 fluxional-0.1.5/fluxional/core/infrastructure/base.py
+-rw-r--r--   0        0        0     7699 2024-04-28 18:14:21.953877 fluxional-0.1.5/fluxional/core/infrastructure/cdk.py
+-rw-r--r--   0        0        0     9554 2024-04-28 18:14:21.953877 fluxional-0.1.5/fluxional/core/infrastructure/resources.py
+-rw-r--r--   0        0        0      816 2024-04-28 18:14:21.953877 fluxional-0.1.5/fluxional/core/infrastructure/types.py
+-rw-r--r--   0        0        0     5818 2024-04-28 18:14:21.953877 fluxional-0.1.5/fluxional/core/logic.py
+-rw-r--r--   0        0        0     8343 2024-04-28 18:14:21.953877 fluxional-0.1.5/fluxional/core/settings.py
+-rw-r--r--   0        0        0     4045 2024-04-28 18:14:21.953877 fluxional-0.1.5/fluxional/core/tools.py
+-rw-r--r--   0        0        0     5158 2024-04-28 18:14:21.953877 fluxional-0.1.5/fluxional/core/types.py
+-rw-r--r--   0        0        0       74 2024-04-28 18:14:21.953877 fluxional-0.1.5/fluxional/deployment/__init__.py
+-rw-r--r--   0        0        0     1164 2024-04-28 18:14:21.953877 fluxional-0.1.5/fluxional/deployment/constants.py
+-rw-r--r--   0        0        0    15517 2024-04-30 22:02:31.375706 fluxional-0.1.5/fluxional/deployment/engine.py
+-rw-r--r--   0        0        0      345 2024-04-28 18:14:21.953877 fluxional-0.1.5/fluxional/deployment/exceptions.py
+-rw-r--r--   0        0        0        1 2024-04-30 22:01:04.012000 fluxional-0.1.5/fluxional/deployment/utils.py
+-rw-r--r--   0        0        0     3652 2024-04-28 18:14:21.963877 fluxional-0.1.5/fluxional/dev/__init__.py
+-rw-r--r--   0        0        0     3003 2024-04-28 18:14:21.963877 fluxional-0.1.5/fluxional/dev/client.py
+-rw-r--r--   0        0        0     3350 2024-04-28 18:14:21.963877 fluxional-0.1.5/fluxional/dev/runner.py
+-rw-r--r--   0        0        0      326 2024-04-28 18:14:21.963877 fluxional-0.1.5/fluxional/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-28 18:14:21.963877 fluxional-0.1.5/fluxional/py.typed
+-rw-r--r--   0        0        0      461 2024-04-28 18:14:21.963877 fluxional-0.1.5/fluxional/types.py
+-rw-r--r--   0        0        0      935 2024-04-28 18:14:21.963877 fluxional-0.1.5/fluxional/utils.py
+-rw-r--r--   0        0        0     1151 2024-05-09 01:21:39.878429 fluxional-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 fluxional-0.1.5/PKG-INFO
```

### Comparing `fluxional-0.1.4/LICENSE` & `fluxional-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/README.md` & `fluxional-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/cli/__init__.py` & `fluxional-0.1.5/fluxional/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/core/app.py` & `fluxional-0.1.5/fluxional/core/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     S3Bucket,
     S3Permission,
     RateSchedule,
     CronSchedule,
     SqsQueue,
     SqsPermission,
     AllPermission,
+    WebsocketPermission,
 )
 from .infrastructure.types import (
     DynamoDBBillingModeT,
     DynamoDBKeyT,
     DynamoDBLsiT,
     DynamoDBStreamT,
     RateDurationUnitT,
@@ -164,14 +165,22 @@
             LambdaPermission(
                 resource_id=websocket_lambda.id,
                 resource_type=websocket_lambda.resource_type,
                 allow_invoke=True,
             )
         )
 
+        websocket_lambda.permissions.append(
+            WebsocketPermission(
+                resource_id=websocket_api_gateway.id,
+                resource_type=websocket_api_gateway.resource_type,
+                allow_publish=True,
+            )
+        )
+
         # Register
         resources[websocket_lambda.id] = websocket_lambda
         resources[websocket_api_gateway.id] = websocket_api_gateway
         self.websocket.websocket_gateway = websocket_api_gateway
         self.websocket.websocket_lambda = websocket_lambda
 
     def _build_storage(self, stack_name: str, resources: InfraResources):
@@ -344,15 +353,15 @@
         entity: LambdaFunction | None,
         permission: AllPermission,
         attributes: dict[str, bool],
     ):
         if entity and any(attributes.values()):
             for k, v in attributes.items():
                 setattr(permission, k, v)
-            entity.permissions.append(permission)
+            entity.permissions.insert(0, permission)
 
     def _build_db_permissions(self):
         ## DYNAMODB PERMISSIONS ##
         if self.database and isinstance(self.database, DynamoDB):
             permission = DynamoDbPermission(
                 resource_id=self.database.id,
                 resource_type=self.database.resource_type,
```

### Comparing `fluxional-0.1.4/fluxional/core/core.py` & `fluxional-0.1.5/fluxional/core/core.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/core/events.py` & `fluxional-0.1.5/fluxional/core/events.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/core/handlers.py` & `fluxional-0.1.5/fluxional/core/handlers.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/core/infrastructure/base.py` & `fluxional-0.1.5/fluxional/core/infrastructure/base.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/core/infrastructure/cdk.py` & `fluxional-0.1.5/fluxional/core/infrastructure/cdk.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/core/infrastructure/resources.py` & `fluxional-0.1.5/fluxional/core/infrastructure/resources.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/core/infrastructure/types.py` & `fluxional-0.1.5/fluxional/core/infrastructure/types.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/core/logic.py` & `fluxional-0.1.5/fluxional/core/logic.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/core/settings.py` & `fluxional-0.1.5/fluxional/core/settings.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/core/tools.py` & `fluxional-0.1.5/fluxional/core/tools.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/core/types.py` & `fluxional-0.1.5/fluxional/core/types.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/deployment/constants.py` & `fluxional-0.1.5/fluxional/deployment/constants.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/deployment/engine.py` & `fluxional-0.1.5/fluxional/deployment/engine.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/dev/__init__.py` & `fluxional-0.1.5/fluxional/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/dev/client.py` & `fluxional-0.1.5/fluxional/dev/client.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/dev/runner.py` & `fluxional-0.1.5/fluxional/dev/runner.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/fluxional/utils.py` & `fluxional-0.1.5/fluxional/utils.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.4/pyproject.toml` & `fluxional-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fluxional"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["fluxional"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">= 3.10 < 4.0"
```

### Comparing `fluxional-0.1.4/PKG-INFO` & `fluxional-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxional
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: MIT
 Author: fluxional
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

