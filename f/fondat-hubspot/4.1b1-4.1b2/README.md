# Comparing `tmp/fondat_hubspot-4.1b1.tar.gz` & `tmp/fondat_hubspot-4.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondat_hubspot-4.1b1.tar", max compression
+gzip compressed data, was "fondat_hubspot-4.1b2.tar", max compression
```

## Comparing `fondat_hubspot-4.1b1.tar` & `fondat_hubspot-4.1b2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1055 2023-03-23 00:18:59.445824 fondat_hubspot-4.1b1/LICENSE
--rw-r--r--   0        0        0      824 2023-03-23 00:16:09.583074 fondat_hubspot-4.1b1/README.md
--rw-r--r--   0        0        0       38 2023-03-23 00:20:20.218975 fondat_hubspot-4.1b1/fondat/hubspot/__init__.py
--rw-r--r--   0        0        0     7603 2023-09-09 14:14:54.683912 fondat_hubspot-4.1b1/fondat/hubspot/client.py
--rw-r--r--   0        0        0      201 2023-06-02 19:41:42.605756 fondat_hubspot-4.1b1/fondat/hubspot/contacts/__init__.py
--rw-r--r--   0        0        0     4420 2023-06-03 00:00:58.858321 fondat_hubspot-4.1b1/fondat/hubspot/contacts/lists.py
--rw-r--r--   0        0        0      555 2023-09-09 14:16:32.724556 fondat_hubspot-4.1b1/fondat/hubspot/crm/__init__.py
--rw-r--r--   0        0        0    13080 2023-06-02 19:47:24.577196 fondat_hubspot-4.1b1/fondat/hubspot/crm/exports.py
--rw-r--r--   0        0        0     2253 2023-06-02 16:09:55.071083 fondat_hubspot-4.1b1/fondat/hubspot/crm/model.py
--rw-r--r--   0        0        0     5493 2023-09-11 06:46:39.015663 fondat_hubspot-4.1b1/fondat/hubspot/crm/objects.py
--rw-r--r--   0        0        0     1493 2023-06-02 15:59:10.268143 fondat_hubspot-4.1b1/fondat/hubspot/crm/owners.py
--rw-r--r--   0        0        0     3225 2023-06-02 19:47:24.500529 fondat_hubspot-4.1b1/fondat/hubspot/crm/pipelines.py
--rw-r--r--   0        0        0     1610 2023-06-02 18:03:10.729064 fondat_hubspot-4.1b1/fondat/hubspot/crm/properties.py
--rw-r--r--   0        0        0     1264 2023-06-02 18:30:15.700352 fondat_hubspot-4.1b1/fondat/hubspot/crm/schemas.py
--rw-r--r--   0        0        0     4161 2023-09-16 02:31:23.603238 fondat_hubspot-4.1b1/fondat/hubspot/oauth.py
--rw-r--r--   0        0        0      201 2023-05-16 22:20:53.537415 fondat_hubspot-4.1b1/fondat/hubspot/settings/__init__.py
--rw-r--r--   0        0        0     2313 2023-06-02 23:46:00.486675 fondat_hubspot-4.1b1/fondat/hubspot/settings/users.py
--rw-r--r--   0        0        0     1132 2023-09-16 02:33:37.763941 fondat_hubspot-4.1b1/pyproject.toml
--rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 fondat_hubspot-4.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-03-23 00:18:59.445824 fondat_hubspot-4.1b2/LICENSE
+-rw-r--r--   0        0        0      824 2023-03-23 00:16:09.583074 fondat_hubspot-4.1b2/README.md
+-rw-r--r--   0        0        0       38 2023-03-23 00:20:20.218975 fondat_hubspot-4.1b2/fondat/hubspot/__init__.py
+-rw-r--r--   0        0        0     7603 2023-09-09 14:14:54.683912 fondat_hubspot-4.1b2/fondat/hubspot/client.py
+-rw-r--r--   0        0        0      201 2023-06-02 19:41:42.605756 fondat_hubspot-4.1b2/fondat/hubspot/contacts/__init__.py
+-rw-r--r--   0        0        0     4420 2023-06-03 00:00:58.858321 fondat_hubspot-4.1b2/fondat/hubspot/contacts/lists.py
+-rw-r--r--   0        0        0      555 2023-09-09 14:16:32.724556 fondat_hubspot-4.1b2/fondat/hubspot/crm/__init__.py
+-rw-r--r--   0        0        0    13080 2023-06-02 19:47:24.577196 fondat_hubspot-4.1b2/fondat/hubspot/crm/exports.py
+-rw-r--r--   0        0        0     2253 2023-06-02 16:09:55.071083 fondat_hubspot-4.1b2/fondat/hubspot/crm/model.py
+-rw-r--r--   0        0        0     5772 2023-09-18 23:49:25.498893 fondat_hubspot-4.1b2/fondat/hubspot/crm/objects.py
+-rw-r--r--   0        0        0     1493 2023-06-02 15:59:10.268143 fondat_hubspot-4.1b2/fondat/hubspot/crm/owners.py
+-rw-r--r--   0        0        0     3225 2023-06-02 19:47:24.500529 fondat_hubspot-4.1b2/fondat/hubspot/crm/pipelines.py
+-rw-r--r--   0        0        0     1610 2023-06-02 18:03:10.729064 fondat_hubspot-4.1b2/fondat/hubspot/crm/properties.py
+-rw-r--r--   0        0        0     1264 2023-06-02 18:30:15.700352 fondat_hubspot-4.1b2/fondat/hubspot/crm/schemas.py
+-rw-r--r--   0        0        0     4161 2023-09-16 02:31:23.603238 fondat_hubspot-4.1b2/fondat/hubspot/oauth.py
+-rw-r--r--   0        0        0      201 2023-05-16 22:20:53.537415 fondat_hubspot-4.1b2/fondat/hubspot/settings/__init__.py
+-rw-r--r--   0        0        0     2313 2023-06-02 23:46:00.486675 fondat_hubspot-4.1b2/fondat/hubspot/settings/users.py
+-rw-r--r--   0        0        0     1132 2023-09-18 23:49:50.849010 fondat_hubspot-4.1b2/pyproject.toml
+-rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 fondat_hubspot-4.1b2/PKG-INFO
```

### Comparing `fondat_hubspot-4.1b1/LICENSE` & `fondat_hubspot-4.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/README.md` & `fondat_hubspot-4.1b2/README.md`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/fondat/hubspot/client.py` & `fondat_hubspot-4.1b2/fondat/hubspot/client.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/fondat/hubspot/contacts/lists.py` & `fondat_hubspot-4.1b2/fondat/hubspot/contacts/lists.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/fondat/hubspot/crm/__init__.py` & `fondat_hubspot-4.1b2/fondat/hubspot/crm/__init__.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/fondat/hubspot/crm/exports.py` & `fondat_hubspot-4.1b2/fondat/hubspot/crm/exports.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/fondat/hubspot/crm/model.py` & `fondat_hubspot-4.1b2/fondat/hubspot/crm/model.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/fondat/hubspot/crm/objects.py` & `fondat_hubspot-4.1b2/fondat/hubspot/crm/objects.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """..."""
 
-from contextlib import suppress
 from datetime import date, datetime
-from fondat.codec import Codec, DecodeError, JSONCodec
+from fondat.codec import Codec, DecodeError, StringCodec
 from fondat.data import datacls
 from fondat.hubspot.client import get_client
 from fondat.hubspot.crm.model import Filter, Property
 from fondat.pagination import Cursor, Page
 from fondat.resource import operation, query, resource
 from fondat.validation import MaxValue, MinValue
 from typing import Annotated, Any
@@ -55,46 +54,56 @@
 
 
 def _codecs(properties: list[Property] | None) -> dict[str, Codec[Any, Any]]:
     result = {}
     for property in properties or {}:
         match property.type:
             case "bool":
-                codec = JSONCodec.get(bool | None)
+                codec = StringCodec.get(bool)
             case "date":
-                codec = JSONCodec.get(date | None)
+                codec = StringCodec.get(date)
             case "datetime":
-                codec = JSONCodec.get(datetime | None)
+                codec = StringCodec.get(datetime)
             case "string" | "phone_number":
-                codec = JSONCodec.get(str | None)
+                codec = StringCodec.get(str)
             case "number":
-                codec = JSONCodec.get(int | float | None)
+                codec = StringCodec.get(int | float)
             case "enumeration":
                 match property.fieldType:
                     case "checkbox":
                         codec = _multi_value_codec
+                    case "booleancheckbox":
+                        codec = StringCodec.get(bool)
                     case _:
-                        codec = JSONCodec.get(str | None)
+                        codec = StringCodec.get(str)
             case _:
                 raise ValueError(f"unexpected property.type: {property.type}")
         result[property.name] = codec
     return result
 
 
 def _decode_object(object: Object, codecs: dict[str, Codec[Any, Any]]) -> None:
-    """Decode properties and propertiesWithHistory values on best-effort basis."""
-    for key in object.properties or ():
-        if codec := codecs.get(key):
-            with suppress(DecodeError):
-                object.properties[key] = codec.decode(object.properties[key])
-    for key in object.propertiesWithHistory or ():
-        if codec := codecs.get(key):
-            for update in object.propertiesWithHistory[key]:
-                with suppress(DecodeError):
-                    update.value = codec.decode(update.value)
+    """Decode properties and propertiesWithHistory values in place."""
+
+    object.properties = {k: v for k, v in (object.properties or {}).items() if k in codecs}
+    for key, value in object.properties.items():
+        if value == "":
+            object.properties[key] = None
+        elif value is not None:
+            object.properties[key] = codecs[key].decode(value)
+
+    object.propertiesWithHistory = {
+        k: v for k, v in (object.propertiesWithHistory or {}).items() if k in codecs
+    }
+    for key, updates in object.propertiesWithHistory.items():
+        for update in updates:
+            if update.value == "":
+                update.value = None
+            elif update.value is not None:
+                update.value = codecs[key].decode(update.value)
 
 
 @resource
 class ObjectResource:
     """..."""
 
     def __init__(self, objectType: str, objectId: str):
```

### Comparing `fondat_hubspot-4.1b1/fondat/hubspot/crm/owners.py` & `fondat_hubspot-4.1b2/fondat/hubspot/crm/owners.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/fondat/hubspot/crm/pipelines.py` & `fondat_hubspot-4.1b2/fondat/hubspot/crm/pipelines.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/fondat/hubspot/crm/properties.py` & `fondat_hubspot-4.1b2/fondat/hubspot/crm/properties.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/fondat/hubspot/crm/schemas.py` & `fondat_hubspot-4.1b2/fondat/hubspot/crm/schemas.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/fondat/hubspot/oauth.py` & `fondat_hubspot-4.1b2/fondat/hubspot/oauth.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/fondat/hubspot/settings/users.py` & `fondat_hubspot-4.1b2/fondat/hubspot/settings/users.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1b1/pyproject.toml` & `fondat_hubspot-4.1b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 line-length = 96
 target-version = ['py310']
 
 [tool.poetry]
 name = "fondat-hubspot"
-version = "4.1b1"
+version = "4.1b2"
 description = "Fondat package for HubSpot."
 readme = "README.md"
 authors = ["fondat-hubspot authors"]
 homepage = "https://github.com/fondat/fondat-hubspot/"
 documentation = "https://github.com/fondat/fondat-hubspot/wiki"
 license = "MIT"
 keywords = ["asgi", "framework", "resource", "openapi"]
```

### Comparing `fondat_hubspot-4.1b1/PKG-INFO` & `fondat_hubspot-4.1b2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fondat-hubspot
-Version: 4.1b1
+Version: 4.1b2
 Summary: Fondat package for HubSpot.
 Home-page: https://github.com/fondat/fondat-hubspot/
 License: MIT
 Keywords: asgi,framework,resource,openapi
 Author: fondat-hubspot authors
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

