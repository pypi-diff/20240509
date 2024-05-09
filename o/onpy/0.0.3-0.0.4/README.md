# Comparing `tmp/onpy-0.0.3.tar.gz` & `tmp/onpy-0.0.4.tar.gz`

## Comparing `onpy-0.0.3.tar` & `onpy-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 onpy-0.0.3/.github/CODEOWNERS
--rw-r--r--   0        0        0   481095 2020-02-02 00:00:00.000000 onpy-0.0.3/.github/media/readme_screenshot.png
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 onpy-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 onpy-0.0.3/.github/workflows/validate.yml
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 onpy-0.0.3/examples/cylinder.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 onpy-0.0.3/examples/preliminary.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/__init__.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/client.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/document.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/api/endpoints.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/api/model.py
--rw-r--r--   0        0        0     9612 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/api/rest_api.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/api/versioning.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/elements/assembly.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/elements/base.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/elements/partstudio.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/features/__init__.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/features/base.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/features/default_planes.py
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/features/extrude.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/features/plane.py
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/features/sketch.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/features/entities/base.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/features/entities/sketch_entities.py
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/util/credentials.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/util/exceptions.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/util/misc.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 onpy-0.0.3/src/onpy/util/model.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 onpy-0.0.3/tests/test_documents.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 onpy-0.0.3/tests/test_features.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 onpy-0.0.3/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 onpy-0.0.3/LICENSE
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 onpy-0.0.3/README.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 onpy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 onpy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 onpy-0.0.4/.github/CODEOWNERS
+-rw-r--r--   0        0        0   481095 2020-02-02 00:00:00.000000 onpy-0.0.4/.github/media/readme_screenshot.png
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 onpy-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 onpy-0.0.4/.github/workflows/validate.yml
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 onpy-0.0.4/examples/cylinder.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 onpy-0.0.4/examples/preliminary.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/__init__.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/client.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/document.py
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/api/endpoints.py
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/api/model.py
+-rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/api/rest_api.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/api/versioning.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/elements/assembly.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/elements/base.py
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/elements/partstudio.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/features/__init__.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/features/base.py
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/features/extrude.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/features/loft.py
+-rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/features/planes.py
+-rw-r--r--   0        0        0    13997 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/features/sketch.py
+-rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/features/entities/base.py
+-rw-r--r--   0        0        0    17181 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/features/entities/sketch_entities.py
+-rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/features/query/list.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/features/query/types.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/util/credentials.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/util/exceptions.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/util/misc.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 onpy-0.0.4/src/onpy/util/model.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 onpy-0.0.4/tests/test_documents.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 onpy-0.0.4/tests/test_features.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 onpy-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 onpy-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 onpy-0.0.4/README.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 onpy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 onpy-0.0.4/PKG-INFO
```

### Comparing `onpy-0.0.3/.github/media/readme_screenshot.png` & `onpy-0.0.4/.github/media/readme_screenshot.png`

 * *Files identical despite different names*

### Comparing `onpy-0.0.3/.github/workflows/python-publish.yml` & `onpy-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `onpy-0.0.3/.github/workflows/validate.yml` & `onpy-0.0.4/.github/workflows/validate.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Integration Tests
+name: ci tests
 
 on:
   pull_request:
   push:
     branches: ["main"]
 
 jobs:
```

### Comparing `onpy-0.0.3/examples/cylinder.py` & `onpy-0.0.4/examples/cylinder.py`

 * *Files identical despite different names*

### Comparing `onpy-0.0.3/examples/preliminary.py` & `onpy-0.0.4/examples/preliminary.py`

 * *Files identical despite different names*

### Comparing `onpy-0.0.3/src/onpy/client.py` & `onpy-0.0.4/src/onpy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Entry point to this library"""
 
 from onpy.util.credentials import CredentialManager
 from onpy.api.rest_api import RestApi
 from onpy.document import Document
-from onpy.util.exceptions import PyshapeParameterError
+from onpy.util.exceptions import OnPyParameterError
 from onpy.util.misc import find_by_name_or_id, UnitSystem
 
 from loguru import logger
 
 
 class Client:
     """Handles project management, authentication, and other related items"""
@@ -40,15 +40,15 @@
         Returns:
             A list of Document objects
         """
 
         candidate = find_by_name_or_id(id, name, self.list_documents())
 
         if candidate is None:
-            raise PyshapeParameterError(
+            raise OnPyParameterError(
                 "Unable to find a document with "
                 + (f"name {name}" if name else f"id {id}")
             )
 
         return candidate
 
     def create_document(self, name: str, description: str | None = None) -> Document:
```

### Comparing `onpy-0.0.3/src/onpy/document.py` & `onpy-0.0.4/src/onpy/document.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Interface to managing OnShape documents"""
 
+import re
+
+from loguru import logger
 import onpy.api.model as model
 from onpy.elements.partstudio import PartStudio
 from onpy.elements.assembly import Assembly
 from onpy.util.misc import find_by_name_or_id
 from onpy.api.versioning import WorkspaceWVM
-from onpy.util.exceptions import PyshapeParameterError
+from onpy.util.exceptions import OnPyParameterError
 
 from typing import TYPE_CHECKING, Any
 from functools import cache
 
 if TYPE_CHECKING:
     from onpy.client import Client
 
@@ -73,20 +76,45 @@
 
         if name is None and id is None:
             return self.list_partstudios()[0]
 
         match = find_by_name_or_id(id, name, self.list_partstudios())
 
         if match is None:
-            raise PyshapeParameterError(
+            raise OnPyParameterError(
                 "Unable to find a partstudio with "
                 + (f"name {name}" if name else f"id {id}")
             )
 
         return match
 
+    def create_version(self, name: str | None = None) -> None:
+        """Creates a version from the current workspace
+
+        Args:
+            name: An optional name of the version. Defaults to v1, v2, etc.
+        """
+
+        if name is None:
+            versions = self._client._api.endpoints.list_versions(self.id)
+            for version in versions:
+                pattern = r"^V(\d+)$"
+                match = re.match(pattern, version.name)
+                if match:
+                    name = f"V{int(match.group(1))+1}"
+                    break
+
+            if name is None:
+                name = "V1"
+
+        self._client._api.endpoints.create_version(
+            document_id=self.id, workspace_id=self.default_workspace.id, name=name
+        )
+
+        logger.info(f"Created new version {name}")
+
     def __eq__(self, other: Any) -> bool:
 
         if type(other) is type(self) and self.id == getattr(other, "id", None):
             return True
         else:
             return False
```

### Comparing `onpy-0.0.3/src/onpy/api/model.py` & `onpy-0.0.4/src/onpy/api/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,14 +53,33 @@
     """Request model of POST /documents"""
 
     name: str
     description: str | None
     isPublic: Optional[bool] = True
 
 
+class DocumentVersion(ApiModel):
+    """Represents a document version"""
+
+    documentId: str
+    name: str
+    id: str
+    microversion: str
+    createdAt: datetime
+    description: Optional[str] = ""
+
+
+class DocumentVersionUpload(ApiModel):
+    """Represents a partial document version, used for upload"""
+
+    documentId: str
+    name: str
+    workspaceId: str
+
+
 class Element(ApiModel):
     """Represents an OnShape element"""
 
     angleUnits: str | None
     areaUnits: str | None
     lengthUnits: str | None
     massUnits: str | None
@@ -104,14 +123,15 @@
 
     btType: str = "BTMSketchCurveSegment-155"
     startPointId: str
     endPointId: str
     startParam: float
     endParam: float
     geometry: dict
+    centerId: str | None = None
 
 
 class Feature(ApiModel):
     """Represents an OnShape feature"""
 
     name: str
     namespace: Optional[str] = None
@@ -142,22 +162,29 @@
 class FeatureAddResponse(ApiModel):
     """API Response after adding a feature"""
 
     feature: Feature
     featureState: FeatureState
 
 
+class FeatureListResponse(ApiModel):
+    """API Response of GET /partstudios/DWE/features"""
+
+    features: list[Feature]
+    defaultFeatures: list[Feature]
+
+
 class FeaturescriptUpload(ApiModel):
-    """Request model of POST /partstudio/DWE/featurescript"""
+    """Request model of POST /partstudios/DWE/featurescript"""
 
     script: str
 
 
 class FeaturescriptResponse(ApiModel):
-    result: dict
+    result: dict | None
 
 
 class Sketch(Feature):
     """Represents a Sketch Feature"""
 
     btType: str = "BTMSketch-151"
     featureType: str = "newSketch"
@@ -166,7 +193,21 @@
 
 
 class Extrude(Feature):
     """Represents an Extrude Feature"""
 
     btType: str = "BTMFeature-134"
     featureType: str = "extrude"
+
+
+class Plane(Feature):
+    """Represents a Plane Feature"""
+
+    btType: str = "BTMFeature-134"
+    featureType: str = "cPlane"
+
+
+class Loft(Feature):
+    """Represents a Loft Feature"""
+
+    btType: str = "BTMFeature-134"
+    featureType: str = "loft"
```

### Comparing `onpy-0.0.3/src/onpy/api/rest_api.py` & `onpy-0.0.4/src/onpy/api/rest_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Rest Api interface to OnShape server"""
 
 import json
 import sys
 from onpy.api.endpoints import EndpointContainer
 from onpy.api.model import ApiModel
 from onpy.util.model import HttpMethod
-from onpy.util.exceptions import PyshapeApiError, PyshapeInternalError
+from onpy.util.exceptions import OnPyApiError, OnPyInternalError
 
 import requests
 from requests.auth import HTTPBasicAuth
 import inspect
 from loguru import logger
 from typing import TYPE_CHECKING, Callable
 
@@ -51,15 +51,15 @@
 
         Returns:
             The response deserialized into the response_type type
         """
 
         # check endpoint formatting
         if not endpoint.startswith("/"):
-            raise PyshapeInternalError(f"Endpoint '{endpoint}' missing '/' prefix")
+            raise OnPyInternalError(f"Endpoint '{endpoint}' missing '/' prefix")
 
         # match method enum to requests function
         requests_func: Callable[..., requests.Response] = {
             HttpMethod.Post: requests.post,
             HttpMethod.Get: requests.get,
             HttpMethod.Delete: requests.delete,
             HttpMethod.Put: requests.put,
@@ -82,39 +82,37 @@
 
         # TODO: wrap this in a try/except to catch timeouts
         r = requests_func(
             url=self.BASE_URL + endpoint, json=payload_json, auth=self.get_auth()
         )
 
         if not r.ok:
-            raise PyshapeApiError(f"Bad response {r.status_code}", r)
+            raise OnPyApiError(f"Bad response {r.status_code}", r)
 
         # deserialize response
         try:
             if r.text.strip() == "":
                 response_dict: dict = {}  # allow empty responses
             else:
                 response_dict = r.json()
             logger.trace(
                 f"{http_method.name} {endpoint} responded with:\n"
                 f"{json.dumps(response_dict, indent=4)}"
             )
         except requests.JSONDecodeError as e:
-            raise PyshapeApiError("Response is not json", r)
+            raise OnPyApiError("Response is not json", r)
 
         if issubclass(response_type, ApiModel):
             return response_type(**response_dict)
 
         elif issubclass(response_type, str):
             return response_type(r.text)
 
         else:
-            raise PyshapeInternalError(
-                f"Illegal response type: {response_type.__name__}"
-            )
+            raise OnPyInternalError(f"Illegal response type: {response_type.__name__}")
 
     def http_wrap_list[
         T: ApiModel | str
     ](
         self,
         http_method: HttpMethod,
         endpoint: str,
@@ -134,15 +132,15 @@
         """
 
         response_raw = self.http_wrap(http_method, endpoint, str, payload)
 
         response_list = json.loads(response_raw)
 
         if not isinstance(response_list, list):
-            raise PyshapeApiError(f"Endpoint {endpoint} expected list response")
+            raise OnPyApiError(f"Endpoint {endpoint} expected list response")
 
         return [response_type(**i) for i in response_list]
 
     def post[
         T: ApiModel | str
     ](self, endpoint: str, response_type: type[T], payload: ApiModel) -> T:
         """Runs a POST request to the specified endpoint. Deserializes into response_type type
```

### Comparing `onpy-0.0.3/src/onpy/api/versioning.py` & `onpy-0.0.4/src/onpy/api/versioning.py`

 * *Files identical despite different names*

### Comparing `onpy-0.0.3/src/onpy/elements/assembly.py` & `onpy-0.0.4/src/onpy/elements/assembly.py`

 * *Files identical despite different names*

### Comparing `onpy-0.0.3/src/onpy/elements/base.py` & `onpy-0.0.4/src/onpy/elements/base.py`

 * *Files identical despite different names*

### Comparing `onpy-0.0.3/src/onpy/features/extrude.py` & `onpy-0.0.4/src/onpy/features/extrude.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 """OnShape extrusion feature"""
 
 from typing import TYPE_CHECKING, override
 from onpy.api.model import Feature, FeatureAddResponse
 from onpy.features.base import Feature, Extrudable
 import onpy.api.model as model
+from onpy.util.misc import unwrap
+from onpy.features.query.list import QueryList
 
 if TYPE_CHECKING:
     from onpy.elements.partstudio import PartStudio
 
 
 class Extrude(Feature):
 
     def __init__(
         self,
         partstudio: "PartStudio",
-        targets: list[Extrudable],
+        targets: QueryList | list[Extrudable],
         distance: float,
         name: str = "Extrusion",
     ) -> None:
-        self.targets = targets
+        self.targets = targets if isinstance(targets, list) else targets._available
         self._id: str | None = None
         self._partstudio = partstudio
         self._name = name
         self.distance = distance
 
+        self._upload_feature()
+
     @property
     @override
     def id(self) -> str | None:
-        return self._id
+        return unwrap(self._id, message="Extrude feature id unbound")
 
     @property
     @override
     def partstudio(self) -> "PartStudio":
         return self._partstudio
 
     @property
     @override
     def name(self) -> str:
         return self._name
 
+    @property
+    @override
+    def entities(self) -> list:
+        return (
+            []
+        )  # TODO: entities are only really relevant on sketches and actual bodies, not features
+
     def _list_queries(self) -> list[dict[str, str]]:
         """Gets a list of queries. Used to build model"""
 
         queries = []
 
         for target in self.targets:
             query_dict = {
@@ -54,14 +65,15 @@
         return queries
 
     @override
     def _to_model(self) -> model.Extrude:
 
         return model.Extrude(
             name=self.name,
+            featureId=self._id,
             suppressed=False,
             parameters=[
                 {
                     "btType": "BTMParameterEnum-145",
                     "parameterId": "bodyType",
                     "value": "SOLID",
                     "enumName": "ExtendedToolBodyType",
@@ -87,9 +99,10 @@
                     "btType": "BTMParameterQuantity-147",
                     "expression": f"{self.distance} {self._client.units.extension}",
                     "parameterId": "depth",
                 },
             ],
         )
 
+    @override
     def _load_response(self, response: FeatureAddResponse) -> None:
         self._id = response.feature.featureId
```

### Comparing `onpy-0.0.3/src/onpy/util/credentials.py` & `onpy-0.0.4/src/onpy/util/credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Manages OnShape credentials"""
 
-from onpy.util.exceptions import PyshapeAuthError
+from onpy.util.exceptions import OnPyAuthError
 
 import re
 import os
 import json
 from loguru import logger
 
 
@@ -64,37 +64,37 @@
 
             with open(CredentialManager.credential_path, "r") as f:
                 data = json.load(f)
                 dev_secret = str(data["dev_secret"])
                 dev_access = str(data["dev_access"])
 
         if not CredentialManager.is_access_key(dev_access):
-            raise PyshapeAuthError("Dev access key does not follow expected pattern")
+            raise OnPyAuthError("Dev access key does not follow expected pattern")
         if not CredentialManager.is_secret_key(dev_secret):
-            raise PyshapeAuthError("Dev secret key does not follow expected pattern")
+            raise OnPyAuthError("Dev secret key does not follow expected pattern")
 
         return (dev_access, dev_secret)
 
     @staticmethod
     def configure_file(access_token: str, secret_token: str) -> None:
         """Creates a configuration file at ~/.onpy/config.json
 
         Args:
             access_token: The access token/key from OnShape dev portal
             secret_token: The secret token/key from OnShape dev portal
         """
 
         # verify before adding
         if not CredentialManager.is_access_key(access_token):
-            raise PyshapeAuthError(
+            raise OnPyAuthError(
                 f"Cannot add token {access_token} to credentials file. "
                 "Not a valid access key."
             )
         if not CredentialManager.is_secret_key(secret_token):
-            raise PyshapeAuthError(
+            raise OnPyAuthError(
                 f"Cannot add token {secret_token} to credentials file. "
                 "Not a valid secret key."
             )
 
         os.makedirs(os.path.dirname(CredentialManager.credential_path), exist_ok=True)
 
         with open(CredentialManager.credential_path, "w") as f:
```

### Comparing `onpy-0.0.3/src/onpy/util/exceptions.py` & `onpy-0.0.4/src/onpy/util/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 from typing import override
 from requests import Response
 from abc import ABC, abstractmethod
 import sys
 from loguru import logger
 
 
-class PyshapeException(Exception, ABC):
+class OnPyException(Exception, ABC):
 
     def __init__(self, message: str):
         self.message = message
         super().__init__(message)
 
     @abstractmethod
     def display(self) -> str:
         """Display the exception as a user-friendly string"""
         ...
 
 
-class PyshapeAuthError(PyshapeException):
+class OnPyAuthError(OnPyException):
 
     @override
     def display(self) -> str:
         """Display the exception as a user-friendly string"""
-        return f"\nPyshapeAuthError({self.message})"
+        return f"\nOnPyAuthError({self.message})"
 
 
-class PyshapeApiError(PyshapeException):
+class OnPyApiError(OnPyException):
 
     def __init__(self, message: str, response: Response | None = None) -> None:
         self.response = response
         super().__init__(message)
 
     @override
     def display(self) -> str:
@@ -47,48 +47,48 @@
                 response_pretty = json.dumps(self.response.json(), indent=4)
             except json.JSONDecodeError:
                 response_pretty = self.response.text
         else:
             response_pretty = "Undefined"
 
         return (
-            f"\nPyshapeApiError: (\n"
+            f"\nOnPyApiError: (\n"
             f"  message: {self.message}\n"
             f"  url: {url}\n"
             f"  response: {response_pretty}\n"
             f")"
         )
 
 
-class PyshapeInternalError(PyshapeException):
+class OnPyInternalError(OnPyException):
 
     @override
     def display(self) -> str:
         """Display the exception as a user-friendly string"""
-        return f"\nPyshapeInternalError({self.message})"
+        return f"\nOnPyInternalError({self.message})"
 
 
-class PyshapeParameterError(PyshapeException):
+class OnPyParameterError(OnPyException):
 
     @override
     def display(self) -> str:
         """Display the exception as a user-friendly string"""
-        return f"\nPyshapeParameterError({self.message})"
+        return f"\nOnPyParameterError({self.message})"
 
 
-class PyshapeFeatureError(PyshapeException):
+class OnPyFeatureError(OnPyException):
 
     @override
     def display(self) -> str:
         """Display the exception as a user-friendly string"""
-        return f"\nPyshapeFeatureError({self.message})"
+        return f"\nOnPyFeatureError({self.message})"
 
 
 def handle_exception(exc_type, exc_value, exc_traceback):
-    if issubclass(exc_type, PyshapeException):
+    if issubclass(exc_type, OnPyException):
         logger.trace(str(exc_traceback))
         logger.error(exc_value.display())
         sys.exit(1)
 
     sys.__excepthook__(exc_type, exc_value, exc_traceback)
```

### Comparing `onpy-0.0.3/src/onpy/util/misc.py` & `onpy-0.0.4/src/onpy/util/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Miscellaneous tools"""
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import Self
 from onpy.api.model import NameIdFetchable
-from onpy.util.exceptions import PyshapeParameterError
+from onpy.util.exceptions import OnPyParameterError
 
 
 def find_by_name_or_id[
     T: NameIdFetchable
 ](id: str | None, name: str | None, items: list[T]) -> T | None:
     """Given a list of values and a name & id, find the first match. Only the
     name or id needs to be provided.
@@ -18,29 +18,29 @@
         name: The name to search for
         items: A list of items to search through
 
     Returns:
         The matching item, if found. Returns None if no match is found.
 
     Raises:
-        PyshapeParameterError if neither the id nor name were provided.
+        OnPyParameterError if neither the id nor name were provided.
     """
 
     if name is None and id is None:
-        raise PyshapeParameterError("A name or id is required to fetch")
+        raise OnPyParameterError("A name or id is required to fetch")
 
     if len(items) == 0:
         return None
 
     candidate: T | None = None
 
     if name:
         filtered = [i for i in items if i.name == name]
         if len(filtered) > 1:
-            raise PyshapeParameterError(
+            raise OnPyParameterError(
                 f"Duplicate names '{name}'. Use id instead to fetch."
             )
         if len(filtered) == 0:
             return None
 
         candidate = filtered[0]
 
@@ -113,25 +113,43 @@
 
     @property
     def extension(self) -> str:
         """Gets the extension of the unit; e.g., 'in' for inches."""
 
         return {UnitSystem.INCH: "in", UnitSystem.METRIC: "m"}[self]
 
+    @property
+    def fs_name(self) -> str:
+        """The featurescript name of the unit system"""
+
+        return {UnitSystem.INCH: "inch", UnitSystem.METRIC: "meter"}[self]
+
 
 @dataclass
 class Point2D:
     """Represents a 2D point"""
 
     x: float
     y: float
 
     def __mul__(self, value: float) -> "Point2D":
         return Point2D(x=self.x * value, y=self.y * value)
 
+    def __truediv__(self, value: float) -> "Point2D":
+        return Point2D(x=self.x / value, y=self.y / value)
+
+    def __add__(self, other: "Point2D") -> "Point2D":
+        return Point2D(self.x + other.x, self.y + other.y)
+
+    def __sub__(self, other: "Point2D") -> "Point2D":
+        return Point2D(self.x - other.x, self.y - other.y)
+
+    def __eq__(self, other: "Point2D") -> bool:
+        return self.x == other.x and self.y == other.y
+
     @classmethod
     def from_pair(cls, tuple: tuple[float, float]) -> Self:
         return cls(*tuple)
 
     @property
     def as_tuple(self) -> tuple[float, float]:
         return (self.x, self.y)
```

### Comparing `onpy-0.0.3/LICENSE` & `onpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onpy-0.0.3/README.md` & `onpy-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # OnPy
+[![CI Tests](https://github.com/kyle-tennison/onpy/actions/workflows/validate.yml/badge.svg)](https://github.com/kyle-tennison/onpy/actions/workflows/validate.yml)
+[![MIT License](https://img.shields.io/github/license/kyle-tennison/onpy?color=yellow)](https://opensource.org/license/mit)
+[![PyPi Version](https://img.shields.io/pypi/v/onpy?color=blue)](https://pypi.org/project/onpy/)
+[![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black)
 
-An interface for creating [OnShape](https://onshape.com) models entirely
-through Python.
-
-[![Integration Tests](https://github.com/kyle-tennison/onpy/actions/workflows/validate.yml/badge.svg)](https://github.com/kyle-tennison/onpy/actions/workflows/validate.yml)
-[![MIT License](https://img.shields.io/github/license/kyle-tennison/onpy)](https://opensource.org/license/mit)
-[![PyPi Version](https://img.shields.io/pypi/v/onpy)](https://pypi.org/project/onpy/)
 
 ## Overview
 
-Pyshape is a python-based, high level interface to building 3D models in [Onshape](https://onshape.com)—a cloud based CAD system.
+**OnPy is a high level Python interface for building 3D models in [Onshape](https://onshape.com)**
 
-In Pyshape you can:
+In OnPy you can:
 
 - Build 2D sketches
 - Extrude to create 3D geometries
 - Interface with other OnShape features
 
 ## Installation & Authentication
```

### Comparing `onpy-0.0.3/pyproject.toml` & `onpy-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "onpy"
-version = "0.0.3"
+version = "0.0.4"
 requires-python = ">=3.12"
 authors = [
   {name = "Kyle Tennison", email = "kyletennison@gmail.com"},
 ]
 maintainers = [
     {name = "Kyle Tennison", email = "kyletennison@gmail.com"},
 ]
@@ -17,14 +17,15 @@
 license = {file = "LICENSE"}
 classifiers = [
   "Programming Language :: Python"
 ]
 dependencies = [
     "loguru",
     "requests",
-    "pydantic"
+    "pydantic",
+    "numpy"
 ]
 [project.optional-dependencies]
 dev = [
     "black",
     "pytest"
 ]
```

### Comparing `onpy-0.0.3/PKG-INFO` & `onpy-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.3
 Name: onpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python API for building models in OnShape
 Author-email: Kyle Tennison <kyletennison@gmail.com>
 Maintainer-email: Kyle Tennison <kyletennison@gmail.com>
 License: Copyright 2024 Kyle Tennison
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Requires-Dist: loguru
+Requires-Dist: numpy
 Requires-Dist: pydantic
 Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # OnPy
+[![CI Tests](https://github.com/kyle-tennison/onpy/actions/workflows/validate.yml/badge.svg)](https://github.com/kyle-tennison/onpy/actions/workflows/validate.yml)
+[![MIT License](https://img.shields.io/github/license/kyle-tennison/onpy?color=yellow)](https://opensource.org/license/mit)
+[![PyPi Version](https://img.shields.io/pypi/v/onpy?color=blue)](https://pypi.org/project/onpy/)
+[![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black)
 
-An interface for creating [OnShape](https://onshape.com) models entirely
-through Python.
-
-[![Integration Tests](https://github.com/kyle-tennison/onpy/actions/workflows/validate.yml/badge.svg)](https://github.com/kyle-tennison/onpy/actions/workflows/validate.yml)
-[![MIT License](https://img.shields.io/github/license/kyle-tennison/onpy)](https://opensource.org/license/mit)
-[![PyPi Version](https://img.shields.io/pypi/v/onpy)](https://pypi.org/project/onpy/)
 
 ## Overview
 
-Pyshape is a python-based, high level interface to building 3D models in [Onshape](https://onshape.com)—a cloud based CAD system.
+**OnPy is a high level Python interface for building 3D models in [Onshape](https://onshape.com)**
 
-In Pyshape you can:
+In OnPy you can:
 
 - Build 2D sketches
 - Extrude to create 3D geometries
 - Interface with other OnShape features
 
 ## Installation & Authentication
```

