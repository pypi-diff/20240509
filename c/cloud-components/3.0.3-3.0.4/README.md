# Comparing `tmp/cloud_components-3.0.3.tar.gz` & `tmp/cloud_components-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_components-3.0.3.tar", max compression
+gzip compressed data, was "cloud_components-3.0.4.tar", max compression
```

## Comparing `cloud_components-3.0.3.tar` & `cloud_components-3.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1080 2024-05-08 19:22:49.747007 cloud_components-3.0.3/LICENSE
--rw-r--r--   0        0        0      870 2024-05-08 19:22:49.747007 cloud_components-3.0.3/README.md
--rw-r--r--   0        0        0      777 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/application/interface/infra/builder.py
--rwxr-xr-x   0        0        0      444 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/application/interface/infra/event.py
--rwxr-xr-x   0        0        0      246 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/application/interface/infra/function.py
--rwxr-xr-x   0        0        0      480 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/application/interface/infra/queue.py
--rw-r--r--   0        0        0      824 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/application/interface/infra/storage.py
--rw-r--r--   0        0        0      456 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/application/interface/services/env/enviroment.py
--rw-r--r--   0        0        0      456 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/application/interface/services/enviroment/enviroment.py
--rw-r--r--   0        0        0      235 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/application/interface/services/log/builder.py
--rw-r--r--   0        0        0      695 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/application/interface/services/log/logger.py
--rw-r--r--   0        0        0       94 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/application/types/aws.py
--rw-r--r--   0        0        0     2729 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/infra/aws/builder.py
--rw-r--r--   0        0        0      861 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/infra/aws/connection/connector_factory.py
--rw-r--r--   0        0        0     2457 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/infra/aws/connection/resource_connector.py
--rwxr-xr-x   0        0        0      740 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/infra/aws/resources/lambda_function.py
--rw-r--r--   0        0        0     3556 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/infra/aws/resources/s3.py
--rwxr-xr-x   0        0        0     1513 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/infra/aws/resources/sns.py
--rwxr-xr-x   0        0        0     1258 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/infra/aws/resources/sqs.py
--rw-r--r--   0        0        0     1471 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/infra/factory.py
--rw-r--r--   0        0        0      996 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/services/env/dotenv.py
--rw-r--r--   0        0        0      418 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/services/env/factory.py
--rw-r--r--   0        0        0      259 2024-05-08 19:22:49.751007 cloud_components-3.0.3/cloud_components/services/log/builder.py
--rw-r--r--   0        0        0      529 2024-05-08 19:22:49.751007 cloud_components-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     1393 1970-01-01 00:00:00.000000 cloud_components-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-08 22:18:53.439921 cloud_components-3.0.4/LICENSE
+-rw-r--r--   0        0        0      870 2024-05-08 22:18:53.439921 cloud_components-3.0.4/README.md
+-rw-r--r--   0        0        0      777 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/application/interface/infra/builder.py
+-rwxr-xr-x   0        0        0      444 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/application/interface/infra/event.py
+-rwxr-xr-x   0        0        0      246 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/application/interface/infra/function.py
+-rwxr-xr-x   0        0        0      480 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/application/interface/infra/queue.py
+-rw-r--r--   0        0        0      837 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/application/interface/infra/storage.py
+-rw-r--r--   0        0        0      475 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/application/interface/services/env/enviroment.py
+-rw-r--r--   0        0        0      475 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/application/interface/services/enviroment/enviroment.py
+-rw-r--r--   0        0        0      235 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/application/interface/services/log/builder.py
+-rw-r--r--   0        0        0      695 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/application/interface/services/log/logger.py
+-rw-r--r--   0        0        0       94 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/application/types/aws.py
+-rw-r--r--   0        0        0     2748 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/infra/aws/builder.py
+-rw-r--r--   0        0        0      861 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/infra/aws/connection/connector_factory.py
+-rw-r--r--   0        0        0     2476 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/infra/aws/connection/resource_connector.py
+-rwxr-xr-x   0        0        0      753 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/infra/aws/resources/lambda_function.py
+-rw-r--r--   0        0        0     3569 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/infra/aws/resources/s3.py
+-rwxr-xr-x   0        0        0     1532 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/infra/aws/resources/sns.py
+-rwxr-xr-x   0        0        0     1277 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/infra/aws/resources/sqs.py
+-rw-r--r--   0        0        0     1490 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/infra/factory.py
+-rw-r--r--   0        0        0     1015 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/services/env/dotenv.py
+-rw-r--r--   0        0        0      418 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/services/env/factory.py
+-rw-r--r--   0        0        0      259 2024-05-08 22:18:53.439921 cloud_components-3.0.4/cloud_components/services/log/builder.py
+-rw-r--r--   0        0        0      529 2024-05-08 22:18:53.439921 cloud_components-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1393 1970-01-01 00:00:00.000000 cloud_components-3.0.4/PKG-INFO
```

### Comparing `cloud_components-3.0.3/LICENSE` & `cloud_components-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.3/README.md` & `cloud_components-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.3/cloud_components/application/interface/infra/builder.py` & `cloud_components-3.0.4/cloud_components/application/interface/infra/builder.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.3/cloud_components/application/interface/infra/storage.py` & `cloud_components-3.0.4/cloud_components/application/interface/infra/storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from abc import ABC, abstractmethod
-from typing import Any
+from typing import Any, Union
 
 
 class IStorage(ABC):
     @abstractmethod
     def save_file(
         self,
         data: str,
         file_path: str,
         content_type: str,
         is_public: bool = False,
     ) -> bool:
         raise NotImplementedError
 
     @abstractmethod
-    def get_file(self, file_path: str) -> str | None:
+    def get_file(self, file_path: str) -> Union[str, None]:
         raise NotImplementedError
 
     @property
     @abstractmethod
     def bucket(self) -> Any:
         raise NotImplementedError
```

### Comparing `cloud_components-3.0.3/cloud_components/application/interface/services/log/logger.py` & `cloud_components-3.0.4/cloud_components/application/interface/services/log/logger.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.3/cloud_components/infra/aws/builder.py` & `cloud_components-3.0.4/cloud_components/infra/aws/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Union
 from cloud_components.application.interface.infra.event import IEvent
 from cloud_components.application.interface.infra.function import IFunction
 from cloud_components.application.interface.infra.queue import IQueue
 from cloud_components.application.types.aws import ResourceType
 from cloud_components.infra.aws.connection.resource_connector import ResourceConnector
 from cloud_components.application.interface.infra.builder import IBuilder
 from cloud_components.application.interface.infra.storage import IStorage
@@ -36,16 +36,16 @@
     """
 
     def __init__(
         self,
         logger: ILogger,
         access_key: str,
         secret_access_key: str,
-        env: Literal["local"] | None = None,
-        localstack_url: str | None = None,
+        env: Union[Literal["local"], None] = None,
+        localstack_url: Union[str, None] = None,
     ) -> None:
         self.logger = logger
         self.resource = ResourceConnector(
             self.logger, access_key, secret_access_key, env, localstack_url
         )
 
     def _set_connection(self, resource_name: ResourceType):
```

### Comparing `cloud_components-3.0.3/cloud_components/infra/aws/connection/connector_factory.py` & `cloud_components-3.0.4/cloud_components/infra/aws/connection/connector_factory.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.3/cloud_components/infra/aws/connection/resource_connector.py` & `cloud_components-3.0.4/cloud_components/infra/aws/connection/resource_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Union
 from cloud_components.infra.aws.connection.connector_factory import ConnectorFactory
 from cloud_components.application.interface.services.log.logger import ILogger
 from cloud_components.application.types.aws import ResourceType
 
 
 class ResourceConnector:
     """
@@ -26,16 +26,16 @@
     """
 
     def __init__(
         self,
         logger: ILogger,
         access_key: str,
         secret_access_key: str,
-        env: Literal["local"] | None = None,
-        localstack_url: str | None = None,
+        env: Union[Literal["local"], None] = None,
+        localstack_url: Union[str, None] = None,
     ) -> None:
         self.logger = logger
         self.access_key = access_key
         self.secret_access_key = secret_access_key
         self.localstack_url = localstack_url
         self.env = env
```

### Comparing `cloud_components-3.0.3/cloud_components/infra/aws/resources/lambda_function.py` & `cloud_components-3.0.4/cloud_components/infra/aws/resources/lambda_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Any
+from typing import Any, Union
 from cloud_components.application.interface.infra.function import IFunction
 from cloud_components.application.interface.services.log.logger import ILogger
 
 
 class Lambda(IFunction):
-    _name: str | None = None
+    _name: Union[str, None] = None
 
     def __init__(self, connection: Any, logger: ILogger) -> None:
         self.connection = connection
         self.logger = logger
 
     @property
     def function(self):
```

### Comparing `cloud_components-3.0.3/cloud_components/infra/aws/resources/s3.py` & `cloud_components-3.0.4/cloud_components/infra/aws/resources/s3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, Union
 from botocore.exceptions import ClientError
 
 from cloud_components.application.interface.services.log.logger import ILogger
 from cloud_components.application.interface.infra.storage import IStorage
 
 
 class S3(IStorage):
@@ -89,15 +89,15 @@
         except ClientError as err:
             self.logger.error(
                 f"An error occurred when try to save a file in S3. Error detail: {err}"
             )
             return False
         return True
 
-    def get_file(self, file_path: str) -> bytes | None:
+    def get_file(self, file_path: str) -> Union[bytes, None]:
         self.logger.info(f"Getting file from '{file_path}'")
         try:
             content = self.bucket.Object(file_path)
             content = content.get()["Body"].read()
         except ClientError as err:
             self.logger.error(
                 f"An error occurred when try to get a file in S3. Error detail: {err}"
```

### Comparing `cloud_components-3.0.3/cloud_components/infra/aws/resources/sns.py` & `cloud_components-3.0.4/cloud_components/infra/aws/resources/sns.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
-from typing import Any, Literal
+from typing import Any, Literal, Union
 from botocore.exceptions import ClientError
 from cloud_components.application.interface.infra.event import IEvent
 from cloud_components.application.interface.services.log.logger import ILogger
 
 
 class Sns(IEvent):
-    _source: str | None = None
+    _source: Union[str, None] = None
 
     def __init__(self, connection: Any, logger: ILogger):
         self.connection = connection
         self.logger = logger
 
     @property
     def source(self) -> Any:
@@ -19,15 +19,15 @@
         return self._source
 
     @source.setter
     def source(self, value: str):
         self._source = value
 
     def send(
-        self, message: dict, message_structere: Literal["json"] | None = None
+        self, message: dict, message_structere: Union[Literal["json"], None] = None
     ) -> bool:
         self.logger.info(f"Sending message to {self.source}")
         try:
             if message_structere:
                 self.connection.publish(
                     TargetArn=self.source,
                     Message=json.dumps({"default": json.dumps(message)}),
```

### Comparing `cloud_components-3.0.3/cloud_components/infra/aws/resources/sqs.py` & `cloud_components-3.0.4/cloud_components/infra/aws/resources/sqs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Any
+from typing import Any, Union
 from botocore.exceptions import ClientError
 from cloud_components.application.interface.infra.queue import IQueue
 from cloud_components.application.interface.services.log.logger import ILogger
 
 
 class Sqs(IQueue):
-    _queue: str | None = None
-    _queue_name: str | None = None
+    _queue: Union[str, None] = None
+    _queue_name: Union[str, None] = None
 
     def __init__(self, connection: Any, logger: ILogger) -> None:
         self.connection = connection
         self.logger = logger
 
     @property
     def queue(self) -> Any:
```

### Comparing `cloud_components-3.0.3/cloud_components/infra/factory.py` & `cloud_components-3.0.4/cloud_components/infra/factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Union
 from cloud_components.application.interface.infra.builder import IBuilder
 from cloud_components.application.interface.services.log.logger import ILogger
 
 
 class InfraFactory:
     """
     This class manufacture cloud implementations from infra package,
@@ -29,16 +29,16 @@
     def __init__(self, logger: ILogger) -> None:
         self.logger = logger
 
     def manufacture_aws(
         self,
         access_key: str,
         secret_access_key: str,
-        env: Literal["local"] | None = None,
-        localstack_url: str | None = None,
+        env: Union[Literal["local"], None] = None,
+        localstack_url: Union[str, None] = None,
     ) -> IBuilder:
         """
         Returns
         ----------
         IBuilder
             An IBuilder implemetation called AwsBuilder
         """
```

### Comparing `cloud_components-3.0.3/cloud_components/services/env/dotenv.py` & `cloud_components-3.0.4/cloud_components/services/env/dotenv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Any, Callable
+from typing import Any, Callable, Union
 
 from cloud_components.application.interface.services.enviroment.enviroment import (
     IEnviroment,
 )
 from cloud_components.application.interface.services.log.logger import ILogger
 
 
@@ -21,12 +21,12 @@
             self.log.error(
                 f"An error occurred when try to load dotenv lib. Error detail: {err}"
             )
 
     def get(  # pylint: disable=C0116
         self,
         env_name: str,
-        cast: Callable[[Any], Any] | None = None,
-        defalt: Any | None = None,
+        cast: Union[Callable[[Any], Any], None] = None,
+        defalt: Union[Any, None] = None,
     ) -> Any:
         value = os.getenv(env_name, defalt)
         return value if not cast else cast(value)
```

### Comparing `cloud_components-3.0.3/pyproject.toml` & `cloud_components-3.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud-components"
-version = "3.0.3"
+version = "3.0.4"
 description = ""
 authors = ["Giovani Liskoski Zanini <giovanilzanini@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cloud_components"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cloud_components-3.0.3/PKG-INFO` & `cloud_components-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-components
-Version: 3.0.3
+Version: 3.0.4
 Summary: 
 License: MIT
 Author: Giovani Liskoski Zanini
 Author-email: giovanilzanini@hotmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

