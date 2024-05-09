# Comparing `tmp/external_resources_io-0.1.9.tar.gz` & `tmp/external_resources_io-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "external_resources_io-0.1.9.tar", max compression
+gzip compressed data, was "external_resources_io-0.2.0.tar", max compression
```

## Comparing `external_resources_io-0.1.9.tar` & `external_resources_io-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      127 2024-01-23 10:37:00.187282 external_resources_io-0.1.9/README.md
--rw-r--r--   0        0        0     2672 2024-03-14 10:58:17.873257 external_resources_io-0.1.9/external_resources_io/input.py
--rw-r--r--   0        0        0      403 2024-03-14 10:58:42.900555 external_resources_io-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 external_resources_io-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      127 2024-05-07 17:21:25.000000 external_resources_io-0.2.0/README.md
+-rw-r--r--   0        0        0     2395 2024-05-07 17:21:25.000000 external_resources_io-0.2.0/external_resources_io/input.py
+-rw-r--r--   0        0        0      637 2024-05-07 17:21:36.545696 external_resources_io-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 external_resources_io-0.2.0/PKG-INFO
```

### Comparing `external_resources_io-0.1.9/external_resources_io/input.py` & `external_resources_io-0.2.0/external_resources_io/input.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pydantic import BaseModel
 from typing import Optional
-import base64
 import json
+import base64
 from typing import TypeVar, Type, Any
 from collections.abc import Mapping
 import os
 
 # EXAMPLE INPUT
 # {
 #   "data": {
@@ -34,50 +34,44 @@
 #       "tf_state_region": "us-east-1",
 #       "tf_state_dynamodb_table": "test-external-resources-lock",
 #       "tf_state_key": "aws/ter-int-dev/aws-iam-role/test-external-resources-iam-role/terraform.state"
 #     }
 #   }
 # }
 
+
 class TerraformProvisionOptions(BaseModel):
     tf_state_bucket: str
     tf_state_region: str
     tf_state_dynamodb_table: str
     tf_state_key: str
 
-class Provision(BaseModel):
+
+class AppInterfaceProvision(BaseModel):
     provision_provider: str  # aws
     provisioner: str  # ter-int-dev
     provider: str  # aws-iam-role
     identifier: str
     target_cluster: str
     target_namespace: str
     target_secret_name: Optional[str]
-
-class Output(Provision):
-    data: dict[str, Any]
-
-class AppInterfaceProvision(Provision):
     module_provision_data: TerraformProvisionOptions
 
-def read_input_data(b64data: str) -> dict[str, Any]:
-    str_input = base64.b64decode(b64data.encode("utf-8")).decode("utf-8")
-    data = json.loads(str_input)
-    return data
 
-T = TypeVar('T', bound=BaseModel)
-def parse_model(model_class: Type[T], data: Mapping[str,Any]) -> T:
+T = TypeVar("T", bound=BaseModel)
+
+def parse_model(model_class: Type[T], data: Mapping[str, Any]) -> T:
     input = model_class.model_validate(data)
     return input
 
-def parse_base64_model(model_class: Type[T], b64data: str) -> T:
-    data = read_input_data(b64data)
-    return parse_model(model_class=model_class, data=data)
-
-def parse_app_interface_provision(b64data: str) -> AppInterfaceProvision:
-    data = read_input_data(b64data)
-    provision: AppInterfaceProvision = parse_model(AppInterfaceProvision, data["provision"])
-    return provision
+def read_input_from_file(file_path: str = "/inputs/input.json") -> dict[str, Any]:
+    with open(file_path, "r") as f:
+        return json.loads(f.read())
+
+def read_input_from_env_var(var: str = "INPUT") -> dict[str, Any]:
+    b64data = os.environ[var]
+    str_input = base64.b64decode(b64data.encode("utf-8")).decode("utf-8")
+    return json.loads(str_input)
 
 def check_container_env() -> None:
     if "INPUT" not in os.environ:
         raise Exception("INPUT env var not present")
```

### Comparing `external_resources_io-0.1.9/PKG-INFO` & `external_resources_io-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: external-resources-io
-Version: 0.1.9
+Version: 0.2.0
 Summary: Util classes for AppSRE External Resources system
 Author: Jordi Piriz
 Author-email: jpiriz@redhat.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

