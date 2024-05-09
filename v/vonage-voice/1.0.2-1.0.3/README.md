# Comparing `tmp/vonage_voice-1.0.2.tar.gz` & `tmp/vonage_voice-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage_voice-1.0.2.tar", last modified: Mon Apr 29 01:52:07 2024, max compression
+gzip compressed data, was "vonage_voice-1.0.3.tar", last modified: Thu May  9 15:01:58 2024, max compression
```

## Comparing `vonage_voice-1.0.2.tar` & `vonage_voice-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.886000 vonage_voice-1.0.2/
--rw-r--r--   0 mkahan     (503) staff       (20)     4516 2024-04-29 01:52:07.885331 vonage_voice-1.0.2/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     3743 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      830 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-29 01:52:07.886131 vonage_voice-1.0.2/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.872566 vonage_voice-1.0.2/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.875743 vonage_voice-1.0.2/src/vonage_voice/
--rw-r--r--   0 mkahan     (503) staff       (20)       95 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      232 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/errors.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.884102 vonage_voice-1.0.2/src/vonage_voice/models/
--rw-r--r--   0 mkahan     (503) staff       (20)     1396 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      955 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/common.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1080 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/connect_endpoints.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1733 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/enums.py
--rw-r--r--   0 mkahan     (503) staff       (20)      666 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/input_types.py
--rw-r--r--   0 mkahan     (503) staff       (20)     5039 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/ncco.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2785 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/requests.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1422 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/responses.py
--rw-r--r--   0 mkahan     (503) staff       (20)     8327 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/voice.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.884535 vonage_voice-1.0.2/src/vonage_voice.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     4516 2024-04-29 01:52:07.000000 vonage_voice-1.0.2/src/vonage_voice.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      613 2024-04-29 01:52:07.000000 vonage_voice-1.0.2/src/vonage_voice.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-29 01:52:07.000000 vonage_voice-1.0.2/src/vonage_voice.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-29 01:52:07.000000 vonage_voice-1.0.2/src/vonage_voice.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       13 2024-04-29 01:52:07.000000 vonage_voice-1.0.2/src/vonage_voice.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:58.005287 vonage_voice-1.0.3/
+-rw-r--r--   0 mkahan     (503) staff       (20)     4516 2024-05-09 15:01:58.004363 vonage_voice-1.0.3/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     3743 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      830 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-05-09 15:01:58.005566 vonage_voice-1.0.3/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:57.990745 vonage_voice-1.0.3/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:57.994882 vonage_voice-1.0.3/src/vonage_voice/
+-rw-r--r--   0 mkahan     (503) staff       (20)       95 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      232 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice/errors.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:58.002721 vonage_voice-1.0.3/src/vonage_voice/models/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1402 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice/models/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      955 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice/models/common.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1080 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice/models/connect_endpoints.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1733 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice/models/enums.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      666 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice/models/input_types.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     5039 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice/models/ncco.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2785 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice/models/requests.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1262 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice/models/responses.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     8327 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice/voice.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:58.003422 vonage_voice-1.0.3/src/vonage_voice.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     4516 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      613 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       13 2024-05-09 15:01:57.000000 vonage_voice-1.0.3/src/vonage_voice.egg-info/top_level.txt
```

### Comparing `vonage_voice-1.0.2/PKG-INFO` & `vonage_voice-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vonage-voice
-Version: 1.0.2
+Version: 1.0.3
 Summary: Vonage voice package
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: vonage-http-client>=1.3.1
-Requires-Dist: vonage-utils>=1.1.1
+Requires-Dist: vonage-utils>=1.1.2
 Requires-Dist: pydantic>=2.7.1
 
 # Vonage Voice Package
 
 This package contains the code to use [Vonage's Voice API](https://developer.vonage.com/en/voice/voice-api/overview) in Python. This package includes methods for working with the Voice API. It also contains an NCCO (Call Control Object) builder to help you to control call flow.
 
 ## Structure
```

### Comparing `vonage_voice-1.0.2/README.md` & `vonage_voice-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.2/backend_shim.py` & `vonage_voice-1.0.3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.2/pyproject.toml` & `vonage_voice-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = 'vonage-voice'
-version = '1.0.2'
+version = '1.0.3'
 description = 'Vonage voice package'
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
   "vonage-http-client>=1.3.1",
-  "vonage-utils>=1.1.1",
+  "vonage-utils>=1.1.2",
   "pydantic>=2.7.1",
 ]
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
```

### Comparing `vonage_voice-1.0.2/src/vonage_voice/models/__init__.py` & `vonage_voice-1.0.3/src/vonage_voice/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 )
 from .responses import (
     CallInfo,
     CallList,
     CallMessage,
     CreateCallResponse,
     Embedded,
-    Links,
+    HalLinks,
 )
 
 __all__ = [
     'AdvancedMachineDetection',
     'AppEndpoint',
     'AudioStreamOptions',
     'CallInfo',
@@ -46,15 +46,15 @@
     'Conversation',
     'CreateCallRequest',
     'CreateCallResponse',
     'Dtmf',
     'Embedded',
     'Input',
     'ListCallsFilter',
-    'Links',
+    'HalLinks',
     'NccoAction',
     'NccoActionType',
     'Notify',
     'OnAnswer',
     'Phone',
     'PhoneEndpoint',
     'Record',
```

### Comparing `vonage_voice-1.0.2/src/vonage_voice/models/common.py` & `vonage_voice-1.0.3/src/vonage_voice/models/common.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.2/src/vonage_voice/models/connect_endpoints.py` & `vonage_voice-1.0.3/src/vonage_voice/models/connect_endpoints.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.2/src/vonage_voice/models/enums.py` & `vonage_voice-1.0.3/src/vonage_voice/models/enums.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.2/src/vonage_voice/models/input_types.py` & `vonage_voice-1.0.3/src/vonage_voice/models/input_types.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.2/src/vonage_voice/models/ncco.py` & `vonage_voice-1.0.3/src/vonage_voice/models/ncco.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.2/src/vonage_voice/models/requests.py` & `vonage_voice-1.0.3/src/vonage_voice/models/requests.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.2/src/vonage_voice/models/responses.py` & `vonage_voice-1.0.3/src/vonage_voice/models/responses.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, Field, model_validator
-from vonage_utils.models import Link
+from vonage_utils.models import HalLinks
 
 from .common import Phone, Sip, Vbc, Websocket
 
 
 class CreateCallResponse(BaseModel):
     uuid: str
     status: str
@@ -14,36 +14,28 @@
 
 
 class CallMessage(BaseModel):
     message: str
     uuid: str
 
 
-class Links(BaseModel):
-    self: Link
-    first: Optional[Link] = None
-    last: Optional[Link] = None
-    prev: Optional[Link] = None
-    next: Optional[Link] = None
-
-
 class CallInfo(BaseModel):
     uuid: str
     conversation_uuid: str
     to: Phone
     from_: Union[Phone, Sip, Websocket, Vbc] = Field(..., validation_alias='from')
     status: str
     direction: str
     rate: Optional[str] = None
     price: Optional[str] = None
     duration: Optional[str] = None
     start_time: Optional[str] = None
     end_time: Optional[str] = None
     network: Optional[str] = None
-    links: Links = Field(..., validation_alias='_links', exclude=True)
+    links: HalLinks = Field(..., validation_alias='_links', exclude=True)
     link: Optional[str] = None
 
     @model_validator(mode='after')
     def get_link(self):
         self.link = self.links.self.href
         return self
 
@@ -53,8 +45,8 @@
 
 
 class CallList(BaseModel):
     count: int
     page_size: int
     record_index: int
     embedded: Embedded = Field(..., validation_alias='_embedded')
-    links: Links = Field(..., validation_alias='_links')
+    links: HalLinks = Field(..., validation_alias='_links')
```

### Comparing `vonage_voice-1.0.2/src/vonage_voice/voice.py` & `vonage_voice-1.0.3/src/vonage_voice/voice.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.2/src/vonage_voice.egg-info/PKG-INFO` & `vonage_voice-1.0.3/src/vonage_voice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vonage-voice
-Version: 1.0.2
+Version: 1.0.3
 Summary: Vonage voice package
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: vonage-http-client>=1.3.1
-Requires-Dist: vonage-utils>=1.1.1
+Requires-Dist: vonage-utils>=1.1.2
 Requires-Dist: pydantic>=2.7.1
 
 # Vonage Voice Package
 
 This package contains the code to use [Vonage's Voice API](https://developer.vonage.com/en/voice/voice-api/overview) in Python. This package includes methods for working with the Voice API. It also contains an NCCO (Call Control Object) builder to help you to control call flow.
 
 ## Structure
```

### Comparing `vonage_voice-1.0.2/src/vonage_voice.egg-info/SOURCES.txt` & `vonage_voice-1.0.3/src/vonage_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

