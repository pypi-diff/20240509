# Comparing `tmp/kodexa-7.0.9017589911.tar.gz` & `tmp/kodexa-7.0.9017913951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.9017589911.tar", max compression
+gzip compressed data, was "kodexa-7.0.9017913951.tar", max compression
```

## Comparing `kodexa-7.0.9017589911.tar` & `kodexa-7.0.9017913951.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2024-05-09 12:55:09.265327 kodexa-7.0.9017589911/LICENSE
--rw-r--r--   0        0        0     2178 2024-05-09 12:55:09.265327 kodexa-7.0.9017589911/README.md
--rw-r--r--   0        0        0      957 2024-05-09 12:55:09.269327 kodexa-7.0.9017589911/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-05-09 12:55:09.269327 kodexa-7.0.9017589911/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-05-09 12:55:09.269327 kodexa-7.0.9017589911/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-05-09 12:55:09.269327 kodexa-7.0.9017589911/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/model/base.py
--rw-r--r--   0        0        0        0 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/model/entities/__init__.py
--rw-r--r--   0        0        0     3526 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/model/entities/product.py
--rw-r--r--   0        0        0     3810 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/model/entities/product_subscription.py
--rw-r--r--   0        0        0   115561 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/model/model.py
--rw-r--r--   0        0        0   174318 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/model/objects.py
--rw-r--r--   0        0        0    62032 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   217080 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    34024 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-05-09 12:55:09.273327 kodexa-7.0.9017589911/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 12:55:09.277327 kodexa-7.0.9017589911/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1389 2024-05-09 12:55:23.997312 kodexa-7.0.9017589911/pyproject.toml
--rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.9017589911/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-09 13:19:42.894475 kodexa-7.0.9017913951/LICENSE
+-rw-r--r--   0        0        0     2178 2024-05-09 13:19:42.894475 kodexa-7.0.9017913951/README.md
+-rw-r--r--   0        0        0      957 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/model/base.py
+-rw-r--r--   0        0        0        0 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/model/entities/__init__.py
+-rw-r--r--   0        0        0     3526 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/model/entities/product.py
+-rw-r--r--   0        0        0     3810 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/model/entities/product_subscription.py
+-rw-r--r--   0        0        0   115561 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/model/model.py
+-rw-r--r--   0        0        0   174318 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/model/objects.py
+-rw-r--r--   0        0        0    62032 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-05-09 13:19:42.898475 kodexa-7.0.9017913951/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   217215 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    34024 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 13:19:42.902475 kodexa-7.0.9017913951/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1389 2024-05-09 13:19:55.302609 kodexa-7.0.9017913951/pyproject.toml
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.9017913951/PKG-INFO
```

### Comparing `kodexa-7.0.9017589911/LICENSE` & `kodexa-7.0.9017913951/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/README.md` & `kodexa-7.0.9017913951/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/__init__.py` & `kodexa-7.0.9017913951/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/assistant/assistant.py` & `kodexa-7.0.9017913951/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/connectors/connectors.py` & `kodexa-7.0.9017913951/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/model/__init__.py` & `kodexa-7.0.9017913951/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/model/base.py` & `kodexa-7.0.9017913951/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/model/entities/product.py` & `kodexa-7.0.9017913951/kodexa/model/entities/product.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/model/entities/product_subscription.py` & `kodexa-7.0.9017913951/kodexa/model/entities/product_subscription.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/model/model.py` & `kodexa-7.0.9017913951/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/model/objects.py` & `kodexa-7.0.9017913951/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/model/persistence.py` & `kodexa-7.0.9017913951/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/pipeline/pipeline.py` & `kodexa-7.0.9017913951/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/platform/client.py` & `kodexa-7.0.9017913951/kodexa/platform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2783,29 +2783,30 @@
         Get the page class of the endpoint.
 
         Returns:
             PageProjectEndpoint: The page class of the endpoint.
         """
         return PageProjectEndpoint
 
-    def find_by_name(self, project_name: str) -> Optional[ProjectEndpoint]:
+    def find_by_name(self, project_name: str, organization: Optional[Organization] = None) -> Optional[ProjectEndpoint]:
         """
         Find a project by name.
 
         Args:
             project_name (str): The name of the project to find.
+            organization (Organization, optional): The organization to search in. Defaults to None.
 
         Returns:
             Optional[ProjectEndpoint]: The project endpoint if found, None otherwise.
         """
 
         url = f"/api/{self.get_type()}"
         filters = {"filter": [f"name: '{project_name}'"]}
-        if self.organization is not None:
-            filters["filter"].append(f"organization.id: '{self.organization.id}'")
+        if organization is not None:
+            filters["filter"].append(f"organization.id: '{organization.id}'")
         get_response = self.client.get(url, params=filters)
         if len(get_response.json()["content"]) > 0:
             return ProjectEndpoint.model_validate(
                 get_response.json()["content"][0]
             ).set_client(self.client)
         return None
```

### Comparing `kodexa-7.0.9017589911/kodexa/platform/interaction.py` & `kodexa-7.0.9017913951/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/platform/kodexa.py` & `kodexa-7.0.9017913951/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/selectors/ast.py` & `kodexa-7.0.9017913951/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/selectors/core.py` & `kodexa-7.0.9017913951/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/selectors/lexrules.py` & `kodexa-7.0.9017913951/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/selectors/lextab.py` & `kodexa-7.0.9017913951/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/selectors/parserules.py` & `kodexa-7.0.9017913951/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/selectors/parsetab.py` & `kodexa-7.0.9017913951/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/spatial/azure_models.py` & `kodexa-7.0.9017913951/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/spatial/bbox_common.py` & `kodexa-7.0.9017913951/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/spatial/table_form_common.py` & `kodexa-7.0.9017913951/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/steps/common.py` & `kodexa-7.0.9017913951/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/testing/test_components.py` & `kodexa-7.0.9017913951/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/kodexa/testing/test_utils.py` & `kodexa-7.0.9017913951/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9017589911/pyproject.toml` & `kodexa-7.0.9017913951/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.09017589911"
+version = "7.0.09017913951"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.9017589911/PKG-INFO` & `kodexa-7.0.9017913951/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.9017589911
+Version: 7.0.9017913951
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

