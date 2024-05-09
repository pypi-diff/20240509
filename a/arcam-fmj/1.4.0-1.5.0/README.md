# Comparing `tmp/arcam-fmj-1.4.0.tar.gz` & `tmp/arcam_fmj-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcam-fmj-1.4.0.tar", last modified: Tue Jun 20 08:53:29 2023, max compression
+gzip compressed data, was "arcam_fmj-1.5.0.tar", last modified: Thu May  9 00:26:26 2024, max compression
```

## Comparing `arcam-fmj-1.4.0.tar` & `arcam_fmj-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/src/arcam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/src/arcam/fmj/
--rw-r--r--   0 runner    (1001) docker     (123)    37106 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/console.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    15606 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-20 08:53:29.000000 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-20 08:53:29.000000 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:53:29.000000 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 08:53:29.000000 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 08:53:29.000000 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 08:53:29.000000 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:26.664952 arcam_fmj-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-09 00:26:26.664952 arcam_fmj-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-09 00:26:26.668952 arcam_fmj-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:26.660952 arcam_fmj-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:26.660952 arcam_fmj-1.5.0/src/arcam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:26.664952 arcam_fmj-1.5.0/src/arcam/fmj/
+-rw-r--r--   0 runner    (1001) docker     (127)    38187 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/src/arcam/fmj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/src/arcam/fmj/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/src/arcam/fmj/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/src/arcam/fmj/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/src/arcam/fmj/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/src/arcam/fmj/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/src/arcam/fmj/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:26.664952 arcam_fmj-1.5.0/src/arcam_fmj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-09 00:26:26.000000 arcam_fmj-1.5.0/src/arcam_fmj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-09 00:26:26.000000 arcam_fmj-1.5.0/src/arcam_fmj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:26:26.000000 arcam_fmj-1.5.0/src/arcam_fmj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 00:26:26.000000 arcam_fmj-1.5.0/src/arcam_fmj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 00:26:26.000000 arcam_fmj-1.5.0/src/arcam_fmj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 00:26:26.000000 arcam_fmj-1.5.0/src/arcam_fmj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:26.664952 arcam_fmj-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/tests/test_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-09 00:26:12.000000 arcam_fmj-1.5.0/tests/test_utils.py
```

### Comparing `arcam-fmj-1.4.0/LICENSE.txt` & `arcam_fmj-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arcam-fmj-1.4.0/PKG-INFO` & `arcam_fmj-1.5.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: arcam-fmj
-Version: 1.4.0
-Summary: A python library for speaking to Arcam receivers
-Home-page: https://github.com/elupus/arcam_fmj
-Author: Joakim Plate
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Environment :: Plugins
-Classifier: Framework :: AsyncIO
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: tests
-License-File: LICENSE.txt
-
 ********************************
 Arcam IP Control
 ********************************
 This module supports controlling an Arcam FMJ receiver (as well as JBL and AudioControl processors) over the network.
 It's built mainly for use with the Home Assistant project, but should work for other projects as well.
 
 Status
```

### Comparing `arcam-fmj-1.4.0/setup.py` & `arcam_fmj-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="arcam-fmj",
-    version="1.4.0",
+    version="1.5.0",
     description="A python library for speaking to Arcam receivers",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     license="MIT",
     packages=["arcam.fmj"],
     package_dir={"": "src"},
     package_data = {
         'arcam.fmj': ['py.typed'],
     },
     python_requires=">=3.8",
     author="Joakim Plate",
-    install_requires=["attrs>18.1"],
+    install_requires=["attrs>18.1", "async"],
     extras_require={
         "tests": [
             "pytest>3.6.4",
-            "pytest-asyncio",
+            "pytest-asyncio==0.21.2",
             "pytest-aiohttp>=1.0.0",
             "pytest-cov>=3.0.0",
             "coveralls",
             "pytest-mock",
             "aiohttp",
             "defusedxml"
         ]
```

### Comparing `arcam-fmj-1.4.0/src/arcam/fmj/__init__.py` & `arcam_fmj-1.5.0/src/arcam/fmj/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,101 +1,154 @@
 """Arcam AV Control"""
 import asyncio
 import enum
 import logging
 import re
 from asyncio.exceptions import IncompleteReadError
-from typing import Dict, Iterable, Optional, SupportsBytes, Tuple, Type, TypeVar, Union, Set, Literal, SupportsIndex
+from typing import (
+    Dict,
+    Iterable,
+    Optional,
+    SupportsBytes,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    Set,
+    Literal,
+    SupportsIndex,
+)
 
 import attr
 
-PROTOCOL_STR = b'\x21'
-PROTOCOL_ETR = b'\x0D'
-PROTOCOL_EOF = b''
+PROTOCOL_STR = b"\x21"
+PROTOCOL_ETR = b"\x0D"
+PROTOCOL_EOF = b""
 
 _LOGGER = logging.getLogger(__name__)
 _WRITE_TIMEOUT = 3
 _READ_TIMEOUT = 3
 
+
 class ArcamException(Exception):
     pass
 
+
 class ConnectionFailed(ArcamException):
     pass
 
+
 class NotConnectedException(ArcamException):
     pass
 
+class UnsupportedZone(ArcamException):
+    pass
+
 class ResponseException(ArcamException):
     def __init__(self, ac=None, zn=None, cc=None, data=None):
         self.ac = ac
         self.zn = zn
         self.cc = cc
         self.data = data
-        super().__init__("'ac':{}, 'zn':{}, 'cc':{}, 'data':{}".format(
-            ac, zn, cc, data
-        ))
+        super().__init__(
+            "'ac':{}, 'zn':{}, 'cc':{}, 'data':{}".format(ac, zn, cc, data)
+        )
 
     @staticmethod
-    def from_response(response: 'ResponsePacket'):
-        kwargs = {
-            'zn': response.zn,
-            'cc': response.cc,
-            'data': response.data
-        }
+    def from_response(response: "ResponsePacket"):
+        kwargs = {"zn": response.zn, "cc": response.cc, "data": response.data}
         if response.ac == AnswerCodes.ZONE_INVALID:
             return InvalidZoneException(**kwargs)
         elif response.ac == AnswerCodes.COMMAND_NOT_RECOGNISED:
             return CommandNotRecognised(**kwargs)
         elif response.ac == AnswerCodes.PARAMETER_NOT_RECOGNISED:
             return ParameterNotRecognised(**kwargs)
         elif response.ac == AnswerCodes.COMMAND_INVALID_AT_THIS_TIME:
             return CommandInvalidAtThisTime(**kwargs)
         elif response.ac == AnswerCodes.INVALID_DATA_LENGTH:
             return InvalidDataLength(**kwargs)
         else:
             return ResponseException(ac=response.ac, **kwargs)
 
+
 class InvalidZoneException(ResponseException):
     def __init__(self, zn=None, cc=None, data=None):
-        super().__init__(ac=AnswerCodes.ZONE_INVALID,
-                         zn=zn, cc=cc, data=data)
+        super().__init__(ac=AnswerCodes.ZONE_INVALID, zn=zn, cc=cc, data=data)
+
 
 class CommandNotRecognised(ResponseException):
     def __init__(self, zn=None, cc=None, data=None):
-        super().__init__(ac=AnswerCodes.COMMAND_NOT_RECOGNISED,
-                         zn=zn, cc=cc, data=data)
+        super().__init__(ac=AnswerCodes.COMMAND_NOT_RECOGNISED, zn=zn, cc=cc, data=data)
+
 
 class ParameterNotRecognised(ResponseException):
     def __init__(self, zn=None, cc=None, data=None):
-        super().__init__(ac=AnswerCodes.PARAMETER_NOT_RECOGNISED,
-                         zn=zn, cc=cc, data=data)
+        super().__init__(
+            ac=AnswerCodes.PARAMETER_NOT_RECOGNISED, zn=zn, cc=cc, data=data
+        )
+
 
 class CommandInvalidAtThisTime(ResponseException):
     def __init__(self, zn=None, cc=None, data=None):
-        super().__init__(ac=AnswerCodes.COMMAND_INVALID_AT_THIS_TIME,
-                         zn=zn, cc=cc, data=data)
+        super().__init__(
+            ac=AnswerCodes.COMMAND_INVALID_AT_THIS_TIME, zn=zn, cc=cc, data=data
+        )
+
 
 class InvalidDataLength(ResponseException):
     def __init__(self, zn=None, cc=None, data=None):
-        super().__init__(ac=AnswerCodes.INVALID_DATA_LENGTH,
-                         zn=zn, cc=cc, data=data)
+        super().__init__(ac=AnswerCodes.INVALID_DATA_LENGTH, zn=zn, cc=cc, data=data)
+
 
 class InvalidPacket(ArcamException):
     pass
 
+
 class NullPacket(ArcamException):
     pass
 
+
 APIVERSION_450_SERIES = {"AVR380", "AVR450", "AVR750"}
 APIVERSION_860_SERIES = {"AV860", "AVR850", "AVR550", "AVR390", "SR250"}
 APIVERSION_SA_SERIES = {"SA10", "SA20", "SA30"}
-APIVERSION_HDA_SERIES = {"AVR5", "AVR10", "AVR20", "AVR30", "AV40", "AVR11", "AVR21", "ARV31", "AV41", "SDP-55", "SDP-58"}
-APIVERSION_HDA_PREMIUM_SERIES = {"AVR10", "AVR20", "AVR30", "AV40", "AVR11", "AVR21", "ARV31", "AV41", "SDP-55", "SDP-58"}
-APIVERSION_HDA_MULTI_ZONE_SERIES = {"AVR20", "AVR30", "AV40", "AVR21", "ARV31", "AV41", "SDP-55", "SDP-58"}
+APIVERSION_HDA_SERIES = {
+    "AVR5",
+    "AVR10",
+    "AVR20",
+    "AVR30",
+    "AV40",
+    "AVR11",
+    "AVR21",
+    "ARV31",
+    "AV41",
+    "SDP-55",
+    "SDP-58",
+}
+APIVERSION_HDA_PREMIUM_SERIES = {
+    "AVR10",
+    "AVR20",
+    "AVR30",
+    "AV40",
+    "AVR11",
+    "AVR21",
+    "ARV31",
+    "AV41",
+    "SDP-55",
+    "SDP-58",
+}
+APIVERSION_HDA_MULTI_ZONE_SERIES = {
+    "AVR20",
+    "AVR30",
+    "AV40",
+    "AVR21",
+    "ARV31",
+    "AV41",
+    "SDP-55",
+    "SDP-58",
+}
 APIVERSION_PA_SERIES = {"PA720", "PA240", "PA410"}
 APIVERSION_ST_SERIES = {"ST60"}
 
 APIVERSION_DAB_SERIES = {"AVR450", "AVR750"}
 APIVERSION_DAB_SERIES.update("AV860", "AVR850", "AVR550", "AVR390")
 APIVERSION_DAB_SERIES.update(APIVERSION_HDA_SERIES)
 
@@ -132,25 +185,34 @@
 
 APIVERSION_PHONO_SERIES = {"SA30"}
 
 APIVERSION_SIMPLE_IP_SERIES = {"PA720", "PA240", "SA10", "SA20"}
 
 APIVERSION_APP_SAFETY_SERIES = {"SA30"}
 
+
 class ApiModel(enum.Enum):
     API450_SERIES = 1
     API860_SERIES = 2
     APISA_SERIES = 3
     APIHDA_SERIES = 4
     APIPA_SERIES = 5
     APIST_SERIES = 6
 
+
 _T = TypeVar("_T", bound="IntOrTypeEnum")
+
+class EnumFlags(enum.IntFlag):
+    ZONE_SUPPORT = enum.auto()
+    SEND_ONLY = enum.auto()
+
+
 class IntOrTypeEnum(enum.IntEnum):
     version: Optional[Set[str]]
+    flags: EnumFlags
 
     @classmethod
     def _missing_(cls, value):
         if isinstance(value, int):
             return cls._create_member(value)
         return None
 
@@ -158,104 +220,101 @@
     def _create_member(cls, value):
         pseudo_member = cls._value2member_map_.get(value, None)
         if pseudo_member is None:
             obj = int.__new__(cls, value)
             obj._name_ = f"CODE_{value}"
             obj._value_ = value
             obj.version = None
+            obj.flags = EnumFlags(0)
             pseudo_member = cls._value2member_map_.setdefault(value, obj)
         return pseudo_member
 
-    def __new__(cls, value: int, version: Optional[set] = None):
-             obj = int.__new__(cls, value)
-             obj._value_ = value
-             obj.version = version
-             return obj
+    def __new__(cls, value: int, version: Optional[Set[str]] = None, flags = EnumFlags(0)):
+        obj = int.__new__(cls, value)
+        obj._value_ = value
+        obj.version = version
+        obj.flags = flags
+        return obj
 
     @classmethod
     def from_int(cls: Type[_T], value: int) -> _T:
         return cls(value)
 
     @classmethod
-    def from_bytes(cls: Type[_T], bytes: Union[Iterable[SupportsIndex], SupportsBytes], byteorder: Literal['little', 'big'] = 'big', *, signed: bool = False) -> _T:  # type: ignore[override]
+    def from_bytes(cls: Type[_T], bytes: Union[Iterable[SupportsIndex], SupportsBytes], byteorder: Literal["little", "big"] = "big", *, signed: bool = False) -> _T:  # type: ignore[override]
         return cls.from_int(int.from_bytes(bytes, byteorder=byteorder, signed=signed))
 
 
 class AnswerCodes(IntOrTypeEnum):
     STATUS_UPDATE = 0x00
     ZONE_INVALID = 0x82
     COMMAND_NOT_RECOGNISED = 0x83
     PARAMETER_NOT_RECOGNISED = 0x84
     COMMAND_INVALID_AT_THIS_TIME = 0x85
     INVALID_DATA_LENGTH = 0x86
 
 
 class CommandCodes(IntOrTypeEnum):
     # System Commands
-    POWER = 0x00
+    POWER = 0x00, None, EnumFlags.ZONE_SUPPORT
     DISPLAY_BRIGHTNESS = 0x01
     HEADPHONES = 0x02
-    FMGENRE = 0x03
+    FMGENRE = 0x03, None, EnumFlags.ZONE_SUPPORT
     SOFTWARE_VERSION = 0x04
     RESTORE_FACTORY_DEFAULT = 0x05
     SAVE_RESTORE_COPY_OF_SETTINGS = 0x06
-    SIMULATE_RC5_IR_COMMAND = 0x08
-    DISPLAY_INFORMATION_TYPE = 0x09
-    CURRENT_SOURCE = 0x1D  # Request
-    HEADPHONES_OVERRIDE = 0x1F
-
+    SIMULATE_RC5_IR_COMMAND = 0x08, None, EnumFlags.ZONE_SUPPORT | EnumFlags.SEND_ONLY
+    DISPLAY_INFORMATION_TYPE = 0x09, None, EnumFlags.ZONE_SUPPORT
+    CURRENT_SOURCE = 0x1D, None, EnumFlags.ZONE_SUPPORT  # Request
+    HEADPHONES_OVERRIDE = 0x1F, None, EnumFlags.ZONE_SUPPORT
 
     # Input Commands
     VIDEO_SELECTION = 0x0A
     SELECT_ANALOG_DIGITAL = 0x0B
-    VIDEO_INPUT_TYPE = 0x0C # IMAX_ENHANCED on 860 and HDA Series (not AVR5)
-
+    VIDEO_INPUT_TYPE = 0x0C  # IMAX_ENHANCED on 860 and HDA Series (not AVR5)
 
     # Output Commands
-    VOLUME = 0x0D  # Set/Request
-    MUTE = 0x0E  # Request
+    VOLUME = 0x0D, None, EnumFlags.ZONE_SUPPORT  # Set/Request
+    MUTE = 0x0E, None, EnumFlags.ZONE_SUPPORT  # Request
     DIRECT_MODE_STATUS = 0x0F  # Request
     DECODE_MODE_STATUS_2CH = 0x10  # Request
     DECODE_MODE_STATUS_MCH = 0x11  # Request
-    RDS_INFORMATION = 0x12  # Request
-    VIDEO_OUTPUT_RESOLUTION = 0x13 # Set/Request
-
+    RDS_INFORMATION = 0x12, None, EnumFlags.ZONE_SUPPORT  # Request
+    VIDEO_OUTPUT_RESOLUTION = 0x13  # Set/Request
 
     # Menu Command
     MENU = 0x14  # Request
-    TUNER_PRESET = 0x15  # Set/Request
-    TUNE = 0x16  # Set/Request
-    DAB_STATION = 0x18  # Set/Request
-    DAB_PROGRAM_TYPE_CATEGORY = 0x19  # Set/Request
-    DLS_PDT_INFO = 0x1A  # Request
-    PRESET_DETAIL = 0x1B # Request
-    NETWORK_PLAYBACK_STATUS = 0x1C, APIVERSION_HDA_SERIES # Request
-    
+    TUNER_PRESET = 0x15, None, EnumFlags.ZONE_SUPPORT  # Set/Request
+    TUNE = 0x16, None, EnumFlags.ZONE_SUPPORT  # Set/Request
+    DAB_STATION = 0x18, None, EnumFlags.ZONE_SUPPORT  # Set/Request
+    DAB_PROGRAM_TYPE_CATEGORY = 0x19, None, EnumFlags.ZONE_SUPPORT  # Set/Request
+    DLS_PDT_INFO = 0x1A, None, EnumFlags.ZONE_SUPPORT  # Request
+    PRESET_DETAIL = 0x1B, None, EnumFlags.ZONE_SUPPORT  # Request
+    NETWORK_PLAYBACK_STATUS = 0x1C, APIVERSION_HDA_SERIES  # Request
 
     # Network Command
 
-
     # Setup
-    TREBLE_EQUALIZATION = 0x35
-    BASS_EQUALIZATION = 0x36
-    ROOM_EQUALIZATION = 0x37
-    DOLBY_VOLUME = 0x38 # DOLBY_AUDIO on HDA series
-    DOLBY_LEVELER = 0x39
-    DOLBY_VOLUME_CALIBRATION_OFFSET = 0x3A
-    BALANCE = 0x3B
+    TREBLE_EQUALIZATION = 0x35, None, EnumFlags.ZONE_SUPPORT
+    BASS_EQUALIZATION = 0x36, None, EnumFlags.ZONE_SUPPORT
+    ROOM_EQUALIZATION = 0x37, None, EnumFlags.ZONE_SUPPORT
+    DOLBY_VOLUME = 0x38, None, EnumFlags.ZONE_SUPPORT  # DOLBY_AUDIO on HDA series
+    DOLBY_LEVELER = 0x39, None, EnumFlags.ZONE_SUPPORT
+    DOLBY_VOLUME_CALIBRATION_OFFSET = 0x3A, None, EnumFlags.ZONE_SUPPORT
+    BALANCE = 0x3B, None, EnumFlags.ZONE_SUPPORT
 
     DOLBY_PLII_X_MUSIC_DIMENSION = 0x3C
     DOLBY_PLII_X_MUSIC_CENTRE_WIDTH = 0x3D
     DOLBY_PLII_X_MUSIC_PANORAMA = 0x3E
-    SUBWOOFER_TRIM = 0x3F
-    LIPSYNC_DELAY = 0x40
-    COMPRESSION = 0x41
+    SUBWOOFER_TRIM = 0x3F, None, EnumFlags.ZONE_SUPPORT
+    LIPSYNC_DELAY = 0x40, None, EnumFlags.ZONE_SUPPORT
+    COMPRESSION = 0x41, None, EnumFlags.ZONE_SUPPORT
 
-    INCOMING_VIDEO_FORMAT = 0x42
-    INCOMING_AUDIO_FORMAT = 0x43
+    INCOMING_VIDEO_FORMAT = 0x42, None, EnumFlags.ZONE_SUPPORT
+    INCOMING_AUDIO_FORMAT = 0x43, None, EnumFlags.ZONE_SUPPORT
     INCOMING_AUDIO_SAMPLERATE = 0x44
 
     SUB_STEREO_TRIM = 0x45  # Set/Request
     VIDEO_BRIGHTNESS = 0x46  # Set/Request
     VIDEO_CONTRAST = 0x47  # Set/Request
     VIDEO_COLOUR = 0x48  # Set/Request
     VIDEO_FILM_MODE = 0x49  # Set/Request
@@ -270,15 +329,15 @@
     INPUT_NAME = 0x20  # Set/Request
     FM_SCAN = 0x23
     DAB_SCAN = 0x24
     HEARTBEAT = 0x25
     REBOOT = 0x26
     SETUP = 0x27, APIVERSION_HDA_SERIES
     ROOM_EQ_NAMES = 0x34, APIVERSION_HDA_SERIES
-    NOW_PLAYING_INFO = 0x64, APIVERSION_HDA_SERIES
+    NOW_PLAYING_INFO = 0x64, APIVERSION_HDA_SERIES, EnumFlags.ZONE_SUPPORT
     INPUT_CONFIG = 0x28, APIVERSION_HDA_SERIES
     GENERAL_SETUP = 0x29, APIVERSION_HDA_SERIES
     SPEAKER_TYPES = 0x2A, APIVERSION_HDA_SERIES
     SPEAKER_DISTANCES = 0x2B, APIVERSION_HDA_SERIES
     SPEAKER_LEVELS = 0x2C, APIVERSION_HDA_SERIES
     VIDEO_INPUTS = 0x2D, APIVERSION_HDA_SERIES
     HDMI_SETTINGS = 0x2E, APIVERSION_HDA_SERIES
@@ -287,28 +346,34 @@
     BLUETOOTH_MENU_INFO = 0x32, APIVERSION_HDA_SERIES
     ENGINEERING_MENU_INFO = 0x33, APIVERSION_HDA_SERIES
 
     # Amp Diagnostics
     DC_OFFSET = 0x51, APIVERSION_AMP_DIAGNOSTICS_SERIES
     SHORT_CIRCUIT_STATUS = 0x52, APIVERSION_CLASS_G_SERIES
     TIMEOUT_COUNTER = 0x55, APIVERSION_AMP_DIAGNOSTICS_SERIES
-    LIFTER_TEMPERATURE = 0x56, APIVERSION_CLASS_G_SERIES # Bug in PA720 1.8 firmware - does not return sensor id
-    OUTPUT_TEMPERATURE = 0x57, APIVERSION_AMP_DIAGNOSTICS_SERIES # Bug in PA720 1.8 firmware - does not return sensor id
+    LIFTER_TEMPERATURE = (
+        0x56,
+        APIVERSION_CLASS_G_SERIES,
+    )  # Bug in PA720 1.8 firmware - does not return sensor id
+    OUTPUT_TEMPERATURE = (
+        0x57,
+        APIVERSION_AMP_DIAGNOSTICS_SERIES,
+    )  # Bug in PA720 1.8 firmware - does not return sensor id
     AUTO_SHUTDOWN_CONTROL = 0x58, APIVERSION_AMP_DIAGNOSTICS_SERIES
 
     # Status/Diagnostics
     FRIENDLY_NAME = 0x53, APIVERSION_SIMPLE_IP_SERIES
     IP_ADDRESS = 0x54, APIVERSION_SIMPLE_IP_SERIES
     PHONO_INPUT_TYPE = 0x59, APIVERSION_PHONO_SERIES
     INPUT_DETECT = 0x5A, APIVERSION_AMP_DIAGNOSTICS_SERIES
     PROCESSOR_MODE_INPUT = 0x5B, APIVERSION_SA_SERIES
     PROCESSOR_MODE_VOLUME = 0x5C, APIVERSION_SA_SERIES
     SYSTEM_STATUS = 0x5D, APIVERSION_AMP_DIAGNOSTICS_SERIES
     SYSTEM_MODEL = 0x5E, APIVERSION_AMP_DIAGNOSTICS_SERIES
-    DAC_FILTER = 0x61, APIVERSION_SA_SERIES # Clashes with AMPLIFIER_MODE on PA240
+    DAC_FILTER = 0x61, APIVERSION_SA_SERIES  # Clashes with AMPLIFIER_MODE on PA240
     MAXIMUM_TURN_ON_VOLUME = 0x65, APIVERSION_APP_SAFETY_SERIES
     MAXIMUM_VOLUME = 0x66, APIVERSION_APP_SAFETY_SERIES
     MAXIMUM_STREAMING_VOLUME = 0x67, APIVERSION_APP_SAFETY_SERIES
 
 
 class SourceCodes(enum.Enum):
     FOLLOW_ZONE_1 = enum.auto()
@@ -333,32 +398,45 @@
     DIG1 = enum.auto()
     DIG2 = enum.auto()
     DIG3 = enum.auto()
     DIG4 = enum.auto()
     NET_USB = enum.auto()
 
     @classmethod
-    def from_bytes(cls, data: bytes, model: ApiModel, zn: int) -> 'SourceCodes':
+    def from_bytes(cls, data: bytes, model: ApiModel, zn: int) -> "SourceCodes":
         try:
             table = SOURCE_CODES[(model, zn)]
         except KeyError:
-            raise ValueError("Unknown source map for model {} and zone {}".format(model, zn))
+            raise ValueError(
+                "Unknown source map for model {} and zone {}".format(model, zn)
+            )
         for key, value in table.items():
             if value == data:
                 return key
-        raise ValueError("Unknown source code for model {} and zone {} and value {!r}".format(model, zn, data))
+        raise ValueError(
+            "Unknown source code for model {} and zone {} and value {!r}".format(
+                model, zn, data
+            )
+        )
 
     def to_bytes(self, model: ApiModel, zn: int):
         try:
             table = SOURCE_CODES[(model, zn)]
         except KeyError:
-            raise ValueError("Unknown source map for model {} and zone {}".format(model, zn))
+            raise ValueError(
+                "Unknown source map for model {} and zone {}".format(model, zn)
+            )
         if data := table.get(self):
             return data
-        raise ValueError("Unknown byte code for model {} and zone {} and value {}".format(model, zn, self))
+        raise ValueError(
+            "Unknown byte code for model {} and zone {} and value {}".format(
+                model, zn, self
+            )
+        )
+
 
 class MenuCodes(IntOrTypeEnum):
     NONE = 0x00
     SETUP = 0x02
     TRIM = 0x03
     BASS = 0x04
     TREBLE = 0x05
@@ -384,14 +462,15 @@
     DTS_VIRTUAL_X = 0x0C, APIVERSION_DTS_X_SERIES
 
     DOLBY_VIRTUAL_HEIGHT = 0x0D, APIVERSION_DOLBY_VIRT_H_SERIES
     AURO_NATIVE = 0x0E, APIVERSION_AURO_SERIES
     AURO_MATIC_3D = 0x0F, APIVERSION_AURO_SERIES
     AURO_2D = 0x10, APIVERSION_AURO_SERIES
 
+
 class DecodeModeMCH(IntOrTypeEnum):
     STEREO_DOWNMIX = 0x01
     MULTI_CHANNEL = 0x02
 
     # This is used for DTS_NEURAL_X on 860 series and HDA series
     DOLBY_D_EX_OR_DTS_ES = 0x03
 
@@ -505,45 +584,39 @@
         DecodeModeMCH.DOLBY_PLII_IIx_MOVIE: bytes([16, 103]),
         DecodeModeMCH.DOLBY_PLII_IIx_MUSIC: bytes([16, 104]),
     },
     (ApiModel.API450_SERIES, 2): {},
     (ApiModel.API860_SERIES, 1): {
         DecodeModeMCH.STEREO_DOWNMIX: bytes([16, 107]),
         DecodeModeMCH.MULTI_CHANNEL: bytes([16, 106]),
-
         # We map to DTS_NEURAL_X
         DecodeModeMCH.DOLBY_D_EX_OR_DTS_ES: bytes([16, 113]),
-
         DecodeModeMCH.DOLBY_SURROUND: bytes([16, 110]),
         DecodeModeMCH.DTS_VIRTUAL_X: bytes([16, 115]),
     },
     (ApiModel.API860_SERIES, 2): {},
     (ApiModel.APIHDA_SERIES, 1): {
         DecodeModeMCH.STEREO_DOWNMIX: bytes([16, 107]),
         DecodeModeMCH.MULTI_CHANNEL: bytes([16, 106]),
-
         # We map to DTS_NEURAL_X
         DecodeModeMCH.DOLBY_D_EX_OR_DTS_ES: bytes([16, 113]),
-
         DecodeModeMCH.DOLBY_SURROUND: bytes([16, 110]),
-
         DecodeModeMCH.DOLBY_VIRTUAL_HEIGHT: bytes([16, 115]),
         DecodeModeMCH.AURO_NATIVE: bytes([16, 103]),
         DecodeModeMCH.AURO_MATIC_3D: bytes([16, 71]),
         DecodeModeMCH.AURO_2D: bytes([16, 104]),
-
     },
     (ApiModel.APIHDA_SERIES, 2): {},
     (ApiModel.APISA_SERIES, 1): {},
     (ApiModel.APISA_SERIES, 2): {},
     (ApiModel.APIPA_SERIES, 1): {},
     (ApiModel.APIPA_SERIES, 2): {},
 }
 
-RC5CODE_DECODE_MODE_2CH: Dict[Tuple[ApiModel, int], Dict[DecodeMode2CH, bytes]]  = {
+RC5CODE_DECODE_MODE_2CH: Dict[Tuple[ApiModel, int], Dict[DecodeMode2CH, bytes]] = {
     (ApiModel.API450_SERIES, 1): {
         DecodeMode2CH.STEREO: bytes([16, 107]),
         DecodeMode2CH.DOLBY_PLII_IIx_MOVIE: bytes([16, 103]),
         DecodeMode2CH.DOLBY_PLII_IIx_MUSIC: bytes([16, 104]),
         DecodeMode2CH.DOLBY_PLII_IIx_GAME: bytes([16, 102]),
         DecodeMode2CH.DOLBY_PL: bytes([16, 110]),
         DecodeMode2CH.DTS_NEO_6_CINEMA: bytes([16, 111]),
@@ -607,15 +680,15 @@
         SourceCodes.BD: bytes([23, 7]),
         SourceCodes.GAME: bytes([23, 11]),
         SourceCodes.CD: bytes([23, 6]),
         SourceCodes.AUX: bytes([23, 13]),
         SourceCodes.PVR: bytes([23, 15]),
         SourceCodes.USB: bytes([23, 18]),
         SourceCodes.NET: bytes([23, 19]),
-        SourceCodes.FOLLOW_ZONE_1: bytes([16, 20])
+        SourceCodes.FOLLOW_ZONE_1: bytes([16, 20]),
     },
     (ApiModel.API860_SERIES, 1): {
         SourceCodes.STB: bytes([16, 100]),
         SourceCodes.AV: bytes([16, 94]),
         SourceCodes.DAB: bytes([16, 72]),
         SourceCodes.FM: bytes([16, 28]),
         SourceCodes.BD: bytes([16, 98]),
@@ -639,15 +712,15 @@
         SourceCodes.CD: bytes([23, 6]),
         SourceCodes.AUX: bytes([23, 13]),
         SourceCodes.PVR: bytes([23, 15]),
         SourceCodes.USB: bytes([23, 18]),
         SourceCodes.NET: bytes([23, 19]),
         SourceCodes.SAT: bytes([23, 20]),
         SourceCodes.VCR: bytes([23, 21]),
-        SourceCodes.FOLLOW_ZONE_1: bytes([16, 20])
+        SourceCodes.FOLLOW_ZONE_1: bytes([16, 20]),
     },
     (ApiModel.APIHDA_SERIES, 1): {
         SourceCodes.STB: bytes([16, 100]),
         SourceCodes.AV: bytes([16, 94]),
         SourceCodes.DAB: bytes([16, 72]),
         SourceCodes.FM: bytes([16, 28]),
         SourceCodes.BD: bytes([16, 98]),
@@ -686,76 +759,52 @@
         SourceCodes.PVR: bytes([16, 96]),
         SourceCodes.AV: bytes([16, 94]),
         SourceCodes.AUX: bytes([16, 99]),
         SourceCodes.STB: bytes([16, 100]),
         SourceCodes.NET: bytes([16, 92]),
         SourceCodes.USB: bytes([16, 93]),
         SourceCodes.GAME: bytes([16, 97]),
-        SourceCodes.ARC_ERC: bytes([16, 125])
+        SourceCodes.ARC_ERC: bytes([16, 125]),
     },
     (ApiModel.APISA_SERIES, 2): {
         SourceCodes.PHONO: bytes([16, 117]),
         SourceCodes.CD: bytes([16, 118]),
         SourceCodes.BD: bytes([16, 98]),
         SourceCodes.SAT: bytes([16, 27]),
         SourceCodes.PVR: bytes([16, 96]),
         SourceCodes.AV: bytes([16, 94]),
         SourceCodes.AUX: bytes([16, 99]),
         SourceCodes.STB: bytes([16, 100]),
         SourceCodes.NET: bytes([16, 92]),
         SourceCodes.USB: bytes([16, 93]),
         SourceCodes.GAME: bytes([16, 97]),
-        SourceCodes.ARC_ERC: bytes([16, 125])
+        SourceCodes.ARC_ERC: bytes([16, 125]),
     },
     (ApiModel.APIST_SERIES, 1): {
         SourceCodes.DIG1: bytes([21, 94]),
         SourceCodes.DIG2: bytes([21, 98]),
         SourceCodes.DIG3: bytes([21, 27]),
         SourceCodes.DIG4: bytes([21, 97]),
         SourceCodes.USB: bytes([21, 93]),
-        SourceCodes.NET: bytes([21, 92])
+        SourceCodes.NET: bytes([21, 92]),
     },
     (ApiModel.APIST_SERIES, 2): {},
     (ApiModel.APIPA_SERIES, 1): {},
     (ApiModel.APIPA_SERIES, 2): {},
 }
 
 RC5CODE_POWER = {
-    (ApiModel.API450_SERIES, 1): {
-        True: bytes([16, 123]),
-        False: bytes([16, 124])
-    },
-    (ApiModel.API450_SERIES, 2): {
-        True: bytes([23, 123]),
-        False: bytes([23, 124])
-    },
-    (ApiModel.API860_SERIES, 1): {
-        True: bytes([16, 123]),
-        False: bytes([16, 124])
-    },
-    (ApiModel.API860_SERIES, 2): {
-        True: bytes([23, 123]),
-        False: bytes([23, 124])
-    },
-    (ApiModel.APIHDA_SERIES, 1): {
-        True: bytes([16, 123]),
-        False: bytes([16, 124])
-    },
-    (ApiModel.APIHDA_SERIES, 2): {
-        True: bytes([23, 123]),
-        False: bytes([23, 124])
-    },
-    (ApiModel.APISA_SERIES, 1): {
-        True: bytes([16, 123]),
-        False: bytes([16, 124])
-    },
-    (ApiModel.APISA_SERIES, 2): {
-        True: bytes([16, 123]),
-        False: bytes([16, 124])
-    }
+    (ApiModel.API450_SERIES, 1): {True: bytes([16, 123]), False: bytes([16, 124])},
+    (ApiModel.API450_SERIES, 2): {True: bytes([23, 123]), False: bytes([23, 124])},
+    (ApiModel.API860_SERIES, 1): {True: bytes([16, 123]), False: bytes([16, 124])},
+    (ApiModel.API860_SERIES, 2): {True: bytes([23, 123]), False: bytes([23, 124])},
+    (ApiModel.APIHDA_SERIES, 1): {True: bytes([16, 123]), False: bytes([16, 124])},
+    (ApiModel.APIHDA_SERIES, 2): {True: bytes([23, 123]), False: bytes([23, 124])},
+    (ApiModel.APISA_SERIES, 1): {True: bytes([16, 123]), False: bytes([16, 124])},
+    (ApiModel.APISA_SERIES, 2): {True: bytes([16, 123]), False: bytes([16, 124])},
 }
 
 RC5CODE_MUTE = {
     (ApiModel.API450_SERIES, 1): {
         True: bytes([16, 119]),
         False: bytes([16, 120]),
     },
@@ -782,15 +831,15 @@
     (ApiModel.APISA_SERIES, 1): {
         True: bytes([16, 26]),
         False: bytes([16, 120]),
     },
     (ApiModel.APISA_SERIES, 2): {
         True: bytes([16, 26]),
         False: bytes([16, 120]),
-    }
+    },
 }
 
 RC5CODE_VOLUME = {
     (ApiModel.API450_SERIES, 1): {
         True: bytes([16, 16]),
         False: bytes([16, 17]),
     },
@@ -821,17 +870,18 @@
     (ApiModel.APISA_SERIES, 2): {
         True: bytes([16, 16]),
         False: bytes([16, 17]),
     },
     (ApiModel.APIST_SERIES, 1): {
         True: bytes([21, 86]),
         False: bytes([21, 85]),
-    }
+    },
 }
 
+
 class IncomingAudioFormat(IntOrTypeEnum):
     PCM = 0x00
     ANALOGUE_DIRECT = 0x01
     DOLBY_DIGITAL = 0x02
     DOLBY_DIGITAL_EX = 0x03
     DOLBY_DIGITAL_SURROUND = 0x04
     DOLBY_DIGITAL_PLUS = 0x05
@@ -853,130 +903,133 @@
     DTS_X = 0x17, APIVERSION_DTS_X_SERIES
     IMAX_ENHANCED = 0x18, APIVERSION_IMAX_SERIES
     AURO_3D = 0x19, APIVERSION_AURO_SERIES
 
 
 class IncomingAudioConfig(IntOrTypeEnum):
     """List of possible audio configurations."""
+
     MONO = 0x01
     CENTER_ONLY = 0x01
     STEREO_ONLY = 0x02
     # Incomplete list...
 
 
 class PresetType(IntOrTypeEnum):
     """List of possible audio configurations."""
+
     AM_FREQUENCY = 0x00
     FM_FREQUENCY = 0x01
     FM_RDS_NAME = 0x02
     DAB = 0x03
 
+
 @attr.s
-class PresetDetail():
+class PresetDetail:
     index = attr.ib(type=int)
     type = attr.ib(type=Union[PresetType, int])
     name = attr.ib(type=str)
 
     @staticmethod
-    def from_bytes(data: bytes) -> 'PresetDetail':
+    def from_bytes(data: bytes) -> "PresetDetail":
         type = PresetType.from_int(data[1])
         if type == PresetType.FM_RDS_NAME or type == PresetType.DAB:
-            name = data[2:].decode('utf8').rstrip()
+            name = data[2:].decode("utf8").rstrip()
         elif type == PresetType.FM_FREQUENCY:
             name = f"{data[2]}.{data[3]:2} MHz"
         elif type == PresetType.AM_FREQUENCY:
             name = f"{data[2]}{data[3]:2} kHz"
         else:
             name = str(data[2:])
         return PresetDetail(data[0], type, name)
 
+
 @attr.s
-class ResponsePacket():
+class ResponsePacket:
     """Represent a response from device."""
+
     zn = attr.ib(type=int)
     cc = attr.ib(type=int)
     ac = attr.ib(type=int)
     data = attr.ib(type=bytes)
 
-    def respons_to(self, request: Union['AmxDuetRequest', 'CommandPacket']):
+    def respons_to(self, request: Union["AmxDuetRequest", "CommandPacket"]):
         if not isinstance(request, CommandPacket):
             return False
-        return (self.zn == request.zn and
-            self.cc == request.cc)
+        return self.zn == request.zn and self.cc == request.cc
 
     @staticmethod
-    def from_bytes(data: bytes) -> 'ResponsePacket':
+    def from_bytes(data: bytes) -> "ResponsePacket":
         if len(data) < 6:
             raise InvalidPacket("Packet to short {!r}".format(data))
 
-        if data[4] != len(data)-6:
+        if data[4] != len(data) - 6:
             raise InvalidPacket("Invalid length in data {!r}".format(data))
 
         return ResponsePacket(
             data[1],
             CommandCodes.from_int(data[2]),
             AnswerCodes.from_int(data[3]),
-            data[5:5+data[4]])
+            data[5 : 5 + data[4]],
+        )
 
     def to_bytes(self):
-        return bytes([
-            *PROTOCOL_STR,
-            self.zn,
-            self.cc,
-            self.ac,
-            len(self.data),
-            *self.data,
-            *PROTOCOL_ETR
-        ])
+        return bytes(
+            [
+                *PROTOCOL_STR,
+                self.zn,
+                self.cc,
+                self.ac,
+                len(self.data),
+                *self.data,
+                *PROTOCOL_ETR,
+            ]
+        )
+
 
 @attr.s
-class CommandPacket():
+class CommandPacket:
     """Represent a command sent to device."""
+
     zn = attr.ib(type=int)
     cc = attr.ib(type=int)
     data = attr.ib(type=bytes)
 
     def to_bytes(self):
-        return bytes([
-            *PROTOCOL_STR,
-            self.zn,
-            self.cc,
-            len(self.data),
-            *self.data,
-            *PROTOCOL_ETR
-        ])
+        return bytes(
+            [*PROTOCOL_STR, self.zn, self.cc, len(self.data), *self.data, *PROTOCOL_ETR]
+        )
 
     @staticmethod
-    def from_bytes(data: bytes) -> 'CommandPacket':
+    def from_bytes(data: bytes) -> "CommandPacket":
         if len(data) < 5:
             raise InvalidPacket("Packet to short {!r}".format(data))
 
-        if data[3] != len(data)-5:
+        if data[3] != len(data) - 5:
             raise InvalidPacket("Invalid length in data {!r}".format(data))
 
         return CommandPacket(
-            data[1],
-            CommandCodes.from_int(data[2]),
-            data[4:4+data[3]])
+            data[1], CommandCodes.from_int(data[2]), data[4 : 4 + data[3]]
+        )
+
 
 @attr.s
-class AmxDuetRequest():
-    
+class AmxDuetRequest:
     @staticmethod
-    def from_bytes(data: bytes) -> 'AmxDuetRequest':
+    def from_bytes(data: bytes) -> "AmxDuetRequest":
         if not data == b"AMX\r":
             raise InvalidPacket("Packet is not a amx request {!r}".format(data))
         return AmxDuetRequest()
 
     def to_bytes(self):
         return b"AMX\r"
 
-@attr.s
-class AmxDuetResponse():
 
+@attr.s
+class AmxDuetResponse:
     values = attr.ib(type=dict)
 
     @property
     def device_class(self) -> Optional[str]:
         return self.values.get("Device-SDKClass")
 
     @property
@@ -993,61 +1046,62 @@
 
     def respons_to(self, packet: Union[AmxDuetRequest, CommandPacket]):
         if not isinstance(packet, AmxDuetRequest):
             return False
         return True
 
     @staticmethod
-    def from_bytes(data: bytes) -> 'AmxDuetResponse':
+    def from_bytes(data: bytes) -> "AmxDuetResponse":
         if not data.startswith(b"AMXB"):
             raise InvalidPacket("Packet is not a amx response {!r}".format(data))
 
         tags = re.findall(r"<(.+?)=(.+?)>", data[4:].decode("ASCII"))
         return AmxDuetResponse(dict(tags))
 
     def to_bytes(self):
-        res = "AMXB" + "".join([
-            f"<{key}={value}>"
-            for key, value in self.values.items() 
-        ]) + "\r"
+        res = (
+            "AMXB"
+            + "".join([f"<{key}={value}>" for key, value in self.values.items()])
+            + "\r"
+        )
         return res.encode("ASCII")
 
 
 async def _read_delimited(reader: asyncio.StreamReader, header_len) -> Optional[bytes]:
     try:
         start = await reader.read(1)
         if start == PROTOCOL_EOF:
             _LOGGER.debug("eof")
             return None
 
         if start == PROTOCOL_STR:
-            header = await reader.read(header_len-1)
+            header = await reader.read(header_len - 1)
             data_len = await reader.read(1)
-            data = await reader.read(int.from_bytes(data_len, 'big'))
+            data = await reader.read(int.from_bytes(data_len, "big"))
             etr = await reader.read(1)
 
             if etr != PROTOCOL_ETR:
                 raise InvalidPacket("unexpected etr byte {!r}".format(etr))
 
             packet = bytes([*start, *header, *data_len, *data, *etr])
         elif start == b"\x01":
             """Sometime the AMX header seem to be sent as \x01^AMX"""
             header = await reader.read(4)
             if header != b"^AMX":
                 raise InvalidPacket("Unexpected AMX header: {!r}".format(header))
-        
+
             data = await reader.readuntil(PROTOCOL_ETR)
-            packet =  bytes([*b"AMX", *data])
+            packet = bytes([*b"AMX", *data])
         elif start == b"A":
             header = await reader.read(2)
             if header != b"MX":
                 raise InvalidPacket("Unexpected AMX header")
 
             data = await reader.readuntil(PROTOCOL_ETR)
-            packet =  bytes([*start, *header, *data])
+            packet = bytes([*start, *header, *data])
         elif start == b"\x00":
             raise NullPacket()
         else:
             raise InvalidPacket("unexpected str byte {!r}".format(start))
 
         return packet
 
@@ -1057,63 +1111,70 @@
         raise ConnectionFailed() from exception
     except OSError as exception:
         raise ConnectionFailed() from exception
     except IncompleteReadError as exception:
         raise ConnectionFailed() from exception
 
 
-async def _read_response(reader: asyncio.StreamReader) -> Optional[Union[ResponsePacket, AmxDuetResponse]]:
+async def _read_response(
+    reader: asyncio.StreamReader,
+) -> Optional[Union[ResponsePacket, AmxDuetResponse]]:
     data = await _read_delimited(reader, 4)
     if not data:
         return None
 
     if data.startswith(b"AMX"):
         return AmxDuetResponse.from_bytes(data)
     else:
         return ResponsePacket.from_bytes(data)
 
 
-async def read_response(reader: asyncio.StreamReader) -> Optional[Union[ResponsePacket, AmxDuetResponse]]:
+async def read_response(
+    reader: asyncio.StreamReader,
+) -> Optional[Union[ResponsePacket, AmxDuetResponse]]:
     while True:
         try:
             data = await _read_response(reader)
         except InvalidPacket as e:
             _LOGGER.warning(str(e))
             continue
         except NullPacket:
             _LOGGER.debug("Ignoring 0x00 start byte sent from some devices")
             continue
         return data
 
 
-async def _read_command(reader: asyncio.StreamReader) -> Optional[Union[CommandPacket, AmxDuetRequest]]:
+async def _read_command(
+    reader: asyncio.StreamReader,
+) -> Optional[Union[CommandPacket, AmxDuetRequest]]:
     data = await _read_delimited(reader, 3)
     if not data:
         return None
     if data.startswith(b"AMX"):
         return AmxDuetRequest.from_bytes(data)
     else:
         return CommandPacket.from_bytes(data)
 
 
-async def read_command(reader: asyncio.StreamReader) -> Optional[Union[CommandPacket, AmxDuetRequest]]:
+async def read_command(
+    reader: asyncio.StreamReader,
+) -> Optional[Union[CommandPacket, AmxDuetRequest]]:
     while True:
         try:
             data = await _read_command(reader)
         except InvalidPacket as e:
             _LOGGER.warning(str(e))
             continue
         return data
 
 
-async def write_packet(writer: asyncio.StreamWriter,
-                       packet: Union[CommandPacket,
-                                     ResponsePacket,
-                                     AmxDuetRequest,
-                                     AmxDuetResponse]) -> None:
+async def write_packet(
+    writer: asyncio.StreamWriter,
+    packet: Union[CommandPacket, ResponsePacket, AmxDuetRequest, AmxDuetResponse],
+) -> None:
     try:
         data = packet.to_bytes()
         writer.write(data)
         await asyncio.wait_for(writer.drain(), _WRITE_TIMEOUT)
     except asyncio.TimeoutError as exception:
         raise ConnectionFailed() from exception
     except ConnectionError as exception:
```

### Comparing `arcam-fmj-1.4.0/src/arcam/fmj/client.py` & `arcam_fmj-1.5.0/src/arcam/fmj/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,77 +11,68 @@
     AmxDuetRequest,
     AmxDuetResponse,
     AnswerCodes,
     ArcamException,
     CommandCodes,
     CommandPacket,
     ConnectionFailed,
+    EnumFlags,
     NotConnectedException,
     ResponseException,
     ResponsePacket,
+    UnsupportedZone,
     read_response,
-    write_packet
+    write_packet,
 )
 from .utils import Throttle, async_retry
 
 _LOGGER = logging.getLogger(__name__)
 _REQUEST_TIMEOUT = timedelta(seconds=3)
 _REQUEST_THROTTLE = 0.2
 
 _HEARTBEAT_INTERVAL = timedelta(seconds=5)
-_HEARTBEAT_TIMEOUT  = _HEARTBEAT_INTERVAL + _HEARTBEAT_INTERVAL
+_HEARTBEAT_TIMEOUT = _HEARTBEAT_INTERVAL + _HEARTBEAT_INTERVAL
 
-class Client:
-    def __init__(self, host: str, port: int) -> None:
+
+class ClientBase:
+    def __init__(self) -> None:
         self._reader: Optional[StreamReader] = None
         self._writer: Optional[StreamWriter] = None
         self._task = None
         self._listen: Set[Callable] = set()
-        self._host = host
-        self._port = port
         self._throttle = Throttle(_REQUEST_THROTTLE)
         self._timestamp = datetime.now()
 
-    @property
-    def host(self) -> str:
-        return self._host
-
-    @property
-    def port(self) -> int:
-        return self._port
-
     @contextmanager
     def listen(self, listener: Callable):
         self._listen.add(listener)
         yield self
         self._listen.remove(listener)
 
     async def _process_heartbeat(self, writer: StreamWriter):
         while True:
             delay = self._timestamp + _HEARTBEAT_INTERVAL - datetime.now()
             if delay > timedelta():
                 await asyncio.sleep(delay.total_seconds())
             else:
                 _LOGGER.debug("Sending ping")
                 await write_packet(
-                    writer,
-                    CommandPacket(1, CommandCodes.POWER, bytes([0xF0]))
+                    writer, CommandPacket(1, CommandCodes.POWER, bytes([0xF0]))
                 )
                 self._timestamp = datetime.now()
 
     async def _process_data(self, reader: StreamReader):
         try:
             while True:
                 try:
                     packet = await asyncio.wait_for(
-                        read_response(reader),
-                        _HEARTBEAT_TIMEOUT.total_seconds()
+                        read_response(reader), _HEARTBEAT_TIMEOUT.total_seconds()
                     )
                 except asyncio.TimeoutError as exception:
-                    _LOGGER.warning("Missed all pings")
+                    _LOGGER.debug("Missed all pings")
                     raise ConnectionFailed() from exception
 
                 if packet is None:
                     _LOGGER.info("Server disconnected")
                     return
 
                 _LOGGER.debug("Packet received: %s", packet)
@@ -108,55 +99,32 @@
     def connected(self) -> bool:
         return self._reader is not None and not self._reader.at_eof()
 
     @property
     def started(self) -> bool:
         return self._writer is not None
 
-    async def start(self) -> None:
-        if self._writer:
-            raise ArcamException("Already started")
-
-        _LOGGER.debug("Connecting to %s:%d", self._host, self._port)
-        try:
-            self._reader, self._writer = await asyncio.open_connection(
-                self._host, self._port)
-        except ConnectionError as exception:
-            raise ConnectionFailed() from exception
-        except OSError as exception:
-            raise ConnectionFailed() from exception
-        _LOGGER.info("Connected to %s:%d", self._host, self._port)
-
-    async def stop(self) -> None:
-        if self._writer:
-            try:
-                _LOGGER.info("Disconnecting from %s:%d", self._host, self._port)
-                self._writer.close()
-                if sys.version_info >= (3, 7):
-                    await self._writer.wait_closed()
-            except (ConnectionError, OSError):
-                pass
-            finally:
-                self._writer = None
-                self._reader = None
-
     @overload
     async def request_raw(self, request: CommandPacket) -> ResponsePacket:
         ...
 
     @overload
     async def request_raw(self, request: AmxDuetRequest) -> AmxDuetResponse:
         ...
 
     @async_retry(2, asyncio.TimeoutError)
-    async def request_raw(self, request: Union[CommandPacket, AmxDuetRequest]) -> Union[ResponsePacket, AmxDuetResponse]:
+    async def request_raw(
+        self, request: Union[CommandPacket, AmxDuetRequest]
+    ) -> Union[ResponsePacket, AmxDuetResponse]:
         if not self._writer:
             raise NotConnectedException()
-        writer = self._writer # keep copy around if stopped by another task
-        future: 'asyncio.Future[Union[ResponsePacket, AmxDuetResponse]]' = asyncio.Future()
+        writer = self._writer  # keep copy around if stopped by another task
+        future: "asyncio.Future[Union[ResponsePacket, AmxDuetResponse]]" = (
+            asyncio.Future()
+        )
 
         def listen(response: Union[ResponsePacket, AmxDuetResponse]):
             if response.respons_to(request):
                 if not (future.cancelled() or future.done()):
                     future.set_result(response)
 
         await self._throttle.get()
@@ -164,45 +132,96 @@
         async def req() -> Union[ResponsePacket, AmxDuetResponse]:
             _LOGGER.debug("Requesting %s", request)
             with self.listen(listen):
                 await write_packet(writer, request)
                 self._timestamp = datetime.now()
                 return await future
 
-        return await asyncio.wait_for(
-            req(),
-            _REQUEST_TIMEOUT.total_seconds())
+        return await asyncio.wait_for(req(), _REQUEST_TIMEOUT.total_seconds())
 
-    async def send(self, zn: int, cc: int, data: bytes) -> None:
+    async def send(self, zn: int, cc: CommandCodes, data: bytes) -> None:
         if not self._writer:
             raise NotConnectedException()
+
+        if not (cc.flags & EnumFlags.ZONE_SUPPORT) and zn != 1:
+            raise UnsupportedZone()
+
         writer = self._writer
         request = CommandPacket(zn, cc, data)
         await self._throttle.get()
         await write_packet(writer, request)
 
-    async def request(self, zn: int, cc: int, data: bytes):
+    async def request(self, zn: int, cc: CommandCodes, data: bytes):
+        if not self._writer:
+            raise NotConnectedException()
+
+        if not (cc.flags & EnumFlags.ZONE_SUPPORT) and zn != 1:
+            raise UnsupportedZone()
+
+        if cc.flags & EnumFlags.SEND_ONLY:
+            await self.send(zn, cc, data)
+            return
+
         response = await self.request_raw(CommandPacket(zn, cc, data))
 
         if response.ac == AnswerCodes.STATUS_UPDATE:
             return response.data
 
         raise ResponseException.from_response(response)
 
+class Client(ClientBase):
+    def __init__(self, host: str, port: int) -> None:
+        super().__init__()
+        self._host = host
+        self._port = port
+
+    @property
+    def host(self) -> str:
+        return self._host
+
+    @property
+    def port(self) -> int:
+        return self._port
+
+    async def start(self) -> None:
+        if self._writer:
+            raise ArcamException("Already started")
+
+        _LOGGER.debug("Connecting to %s:%d", self._host, self._port)
+        try:
+            self._reader, self._writer = await asyncio.open_connection(
+                self._host, self._port
+            )
+        except ConnectionError as exception:
+            raise ConnectionFailed() from exception
+        except OSError as exception:
+            raise ConnectionFailed() from exception
+        _LOGGER.info("Connected to %s:%d", self._host, self._port)
+
+    async def stop(self) -> None:
+        if self._writer:
+            try:
+                _LOGGER.info("Disconnecting from %s:%d", self._host, self._port)
+                self._writer.close()
+                if sys.version_info >= (3, 7):
+                    await self._writer.wait_closed()
+            except (ConnectionError, OSError):
+                pass
+            finally:
+                self._writer = None
+                self._reader = None
 
 class ClientContext:
     def __init__(self, client: Client):
         self._client = client
         self._task: Optional[asyncio.Task] = None
 
     async def __aenter__(self) -> Client:
         await self._client.start()
-        self._task = asyncio.create_task(
-            self._client.process()
-        )
+        self._task = asyncio.create_task(self._client.process())
         return self._client
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         if self._task:
             self._task.cancel()
             try:
                 await self._task
```

### Comparing `arcam-fmj-1.4.0/src/arcam/fmj/console.py` & `arcam_fmj-1.5.0/src/arcam/fmj/console.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,99 @@
 import argparse
 import asyncio
 import logging
 import sys
 
-from . import APIVERSION_450_SERIES, APIVERSION_860_SERIES, APIVERSION_HDA_SERIES, ApiModel, CommandCodes, CommandInvalidAtThisTime, SourceCodes, IncomingAudioFormat, IncomingAudioConfig, DecodeMode2CH, DecodeModeMCH, CommandNotRecognised, _LOGGER, ResponsePacket, AnswerCodes, RC5CODE_SOURCE, RC5CODE_DECODE_MODE_2CH, RC5CODE_DECODE_MODE_MCH
+from . import (
+    APIVERSION_450_SERIES,
+    APIVERSION_860_SERIES,
+    APIVERSION_HDA_SERIES,
+    ApiModel,
+    CommandCodes,
+    CommandInvalidAtThisTime,
+    SourceCodes,
+    IncomingAudioFormat,
+    IncomingAudioConfig,
+    DecodeMode2CH,
+    DecodeModeMCH,
+    CommandNotRecognised,
+    _LOGGER,
+    ResponsePacket,
+    AnswerCodes,
+    RC5CODE_SOURCE,
+    RC5CODE_DECODE_MODE_2CH,
+    RC5CODE_DECODE_MODE_MCH,
+)
 from .client import Client, ClientContext
 from .server import Server, ServerContext
 from .state import State
 
 # pylint: disable=invalid-name
 
+
 def auto_int(x):
     return int(x, 0)
 
+
 def auto_bytes(x):
     print(x)
     return bytes.decode(x)
 
+
 def auto_source(x):
     return SourceCodes[x]
 
-parser = argparse.ArgumentParser(description='Communicate with arcam receivers.')
-parser.add_argument('--verbose', action='store_true')
+
+parser = argparse.ArgumentParser(description="Communicate with arcam receivers.")
+parser.add_argument("--verbose", action="store_true")
 
 subparsers = parser.add_subparsers(dest="subcommand")
 
-parser_state = subparsers.add_parser('state')
-parser_state.add_argument('--host', required=True)
-parser_state.add_argument('--port', default=50000)
-parser_state.add_argument('--zone', default=1, type=int)
-parser_state.add_argument('--volume', type=int)
-parser_state.add_argument('--source', type=auto_source)
-parser_state.add_argument('--monitor', action='store_true')
-parser_state.add_argument('--power-on', action=argparse.BooleanOptionalAction)
-parser_state.add_argument('--power-off', action=argparse.BooleanOptionalAction)
-
-parser_client = subparsers.add_parser('client')
-parser_client.add_argument('--host', required=True)
-parser_client.add_argument('--port', default=50000)
-parser_client.add_argument('--zone', default=1, type=int)
-parser_client.add_argument('--command', type=auto_int)
-parser_client.add_argument('--data', nargs='+', default=[0xF0], type=auto_int)
-
-parser_server = subparsers.add_parser('server')
-parser_server.add_argument('--host', default='localhost')
-parser_server.add_argument('--port', default=50000)
-parser_server.add_argument('--model', default="AVR450")
+parser_state = subparsers.add_parser("state")
+parser_state.add_argument("--host", required=True)
+parser_state.add_argument("--port", default=50000)
+parser_state.add_argument("--zone", default=1, type=int)
+parser_state.add_argument("--volume", type=int)
+parser_state.add_argument("--source", type=auto_source)
+parser_state.add_argument("--monitor", action="store_true")
+parser_state.add_argument("--power-on", action=argparse.BooleanOptionalAction)
+parser_state.add_argument("--power-off", action=argparse.BooleanOptionalAction)
+
+parser_client = subparsers.add_parser("client")
+parser_client.add_argument("--host", required=True)
+parser_client.add_argument("--port", default=50000)
+parser_client.add_argument("--zone", default=1, type=int)
+parser_client.add_argument("--command", type=auto_int, required=True)
+parser_client.add_argument("--data", nargs="+", default=[0xF0], type=auto_int)
+
+parser_server = subparsers.add_parser("server")
+parser_server.add_argument("--host", default="localhost")
+parser_server.add_argument("--port", default=50000)
+parser_server.add_argument("--model", default="AVR450")
 
 
 async def run_client(args):
     client = Client(args.host, args.port)
     async with ClientContext(client):
-        result = await client.request(args.zone, args.command, bytes(args.data))
+        result = await client.request(args.zone, CommandCodes(args.command), bytes(args.data))
         print(result)
 
+
 async def run_state(args):
     client = Client(args.host, args.port)
     async with ClientContext(client):
         state = State(client, args.zone)
         await state.update()
 
         if args.volume is not None:
             await state.set_volume(args.volume)
 
         if args.source is not None:
             await state.set_source(args.source)
-        
+
         if args.power_on is not None:
             await state.set_power(True)
 
         if args.power_off is not None:
             await state.set_power(False)
 
         if args.monitor:
@@ -83,15 +107,14 @@
                     await asyncio.sleep(delay=1)
         else:
             print(state)
 
 
 async def run_server(args):
     class DummyServer(Server):
-
         def __init__(self, host, port, model):
             super().__init__(host, port, model)
 
             if model in APIVERSION_450_SERIES:
                 self._api_version = ApiModel.API450_SERIES
             elif model in APIVERSION_860_SERIES:
                 self._api_version = ApiModel.API860_SERIES
@@ -100,48 +123,80 @@
             else:
                 raise ValueError("Unexpected model")
 
             rc5_key = (self._api_version, 1)
 
             self._volume = bytes([10])
             self._source = bytes([SourceCodes.PVR])
-            self._audio_format = bytes([IncomingAudioFormat.PCM, IncomingAudioConfig.STEREO_ONLY])
-            self._decode_mode_2ch = bytes([next(iter(RC5CODE_DECODE_MODE_2CH[rc5_key]))])
-            self._decode_mode_mch = bytes([next(iter(RC5CODE_DECODE_MODE_MCH[rc5_key]))])
-            self._tuner_preset = b'\0xff'
+            self._audio_format = bytes(
+                [IncomingAudioFormat.PCM, IncomingAudioConfig.STEREO_ONLY]
+            )
+            self._decode_mode_2ch = bytes(
+                [next(iter(RC5CODE_DECODE_MODE_2CH[rc5_key]))]
+            )
+            self._decode_mode_mch = bytes(
+                [next(iter(RC5CODE_DECODE_MODE_MCH[rc5_key]))]
+            )
+            self._tuner_preset = b"\0xff"
             self._presets = {
-                b'\x01': b'\x03SR P1   ',
-                b'\x02': b'\x03SR Klass',
-                b'\x03' : b'\x03P3 Star ',
-                b'\x04': b'\x02SR P4   ',
-                b'\x05': b'\x02SR P4   ',
-                b'\x06': b'\x01jP',
+                b"\x01": b"\x03SR P1   ",
+                b"\x02": b"\x03SR Klass",
+                b"\x03": b"\x03P3 Star ",
+                b"\x04": b"\x02SR P4   ",
+                b"\x05": b"\x02SR P4   ",
+                b"\x06": b"\x01jP",
             }
 
             def invert_rc5(data):
-                return {
-                    value: key
-                    for key, value in data[rc5_key].items()
-                }
+                return {value: key for key, value in data[rc5_key].items()}
 
             self._source_rc5 = invert_rc5(RC5CODE_SOURCE)
             self._decode_mode_2ch_rc5 = invert_rc5(RC5CODE_DECODE_MODE_2CH)
             self._decode_mode_mch_rc5 = invert_rc5(RC5CODE_DECODE_MODE_MCH)
 
-            self.register_handler(0x01, CommandCodes.POWER, bytes([0xF0]), self.get_power)
-            self.register_handler(0x01, CommandCodes.VOLUME, bytes([0xF0]), self.get_volume)
+            self.register_handler(
+                0x01, CommandCodes.POWER, bytes([0xF0]), self.get_power
+            )
+            self.register_handler(
+                0x01, CommandCodes.VOLUME, bytes([0xF0]), self.get_volume
+            )
             self.register_handler(0x01, CommandCodes.VOLUME, None, self.set_volume)
-            self.register_handler(0x01, CommandCodes.CURRENT_SOURCE, bytes([0xF0]), self.get_source)
-            self.register_handler(0x01, CommandCodes.INCOMING_AUDIO_FORMAT, bytes([0xF0]), self.get_incoming_audio_format)
-            self.register_handler(0x01, CommandCodes.DECODE_MODE_STATUS_2CH, bytes([0xF0]), self.get_decode_mode_2ch)
-            self.register_handler(0x01, CommandCodes.DECODE_MODE_STATUS_MCH, bytes([0xF0]), self.get_decode_mode_mch)
-            self.register_handler(0x01, CommandCodes.SIMULATE_RC5_IR_COMMAND, None, self.ir_command)
-            self.register_handler(0x01, CommandCodes.PRESET_DETAIL, None, self.get_preset_detail)
-            self.register_handler(0x01, CommandCodes.TUNER_PRESET, bytes([0xF0]), self.get_tuner_preset)
-            self.register_handler(0x01, CommandCodes.TUNER_PRESET, None, self.set_tuner_preset)
+            self.register_handler(
+                0x01, CommandCodes.CURRENT_SOURCE, bytes([0xF0]), self.get_source
+            )
+            self.register_handler(
+                0x01,
+                CommandCodes.INCOMING_AUDIO_FORMAT,
+                bytes([0xF0]),
+                self.get_incoming_audio_format,
+            )
+            self.register_handler(
+                0x01,
+                CommandCodes.DECODE_MODE_STATUS_2CH,
+                bytes([0xF0]),
+                self.get_decode_mode_2ch,
+            )
+            self.register_handler(
+                0x01,
+                CommandCodes.DECODE_MODE_STATUS_MCH,
+                bytes([0xF0]),
+                self.get_decode_mode_mch,
+            )
+            self.register_handler(
+                0x01, CommandCodes.SIMULATE_RC5_IR_COMMAND, None, self.ir_command
+            )
+            self.register_handler(
+                0x01, CommandCodes.PRESET_DETAIL, None, self.get_preset_detail
+            )
+            self.register_handler(
+                0x01, CommandCodes.TUNER_PRESET, bytes([0xF0]), self.get_tuner_preset
+            )
+            self.register_handler(
+                0x01, CommandCodes.TUNER_PRESET, None, self.set_tuner_preset
+            )
 
         def get_power(self, **kwargs):
             return bytes([1])
 
         def set_volume(self, data, **kwargs):
             self._volume = data
             return self._volume
@@ -154,66 +209,66 @@
 
         def set_source(self, data, **kwargs):
             self._source = data
             return self._source
 
         def ir_command(self, data, **kwargs):
             status = None
-            
+
             source = self._source_rc5.get(data)
             if source:
                 self.set_source(bytes([source]))
                 return [
                     ResponsePacket(
                         zn=0x01,
                         cc=CommandCodes.SIMULATE_RC5_IR_COMMAND,
                         ac=AnswerCodes.STATUS_UPDATE,
-                        data=data
+                        data=data,
                     ),
                     ResponsePacket(
                         zn=0x01,
                         cc=CommandCodes.CURRENT_SOURCE,
                         ac=AnswerCodes.STATUS_UPDATE,
-                        data=bytes([source])
-                    )
+                        data=bytes([source]),
+                    ),
                 ]
             decode_mode_2ch = self._decode_mode_2ch_rc5.get(data)
             if decode_mode_2ch:
                 self._decode_mode_2ch = bytes([decode_mode_2ch])
                 return [
                     ResponsePacket(
                         zn=0x01,
                         cc=CommandCodes.SIMULATE_RC5_IR_COMMAND,
                         ac=AnswerCodes.STATUS_UPDATE,
-                        data=data
+                        data=data,
                     ),
                     ResponsePacket(
                         zn=0x01,
                         cc=CommandCodes.DECODE_MODE_STATUS_2CH,
                         ac=AnswerCodes.STATUS_UPDATE,
-                        data=self._decode_mode_2ch
-                    )
+                        data=self._decode_mode_2ch,
+                    ),
                 ]
 
             decode_mode_mch = self._decode_mode_mch_rc5.get(data)
             if decode_mode_mch:
                 self._decode_mode_mch = bytes([decode_mode_mch])
                 return [
                     ResponsePacket(
                         zn=0x01,
                         cc=CommandCodes.SIMULATE_RC5_IR_COMMAND,
                         ac=AnswerCodes.STATUS_UPDATE,
-                        data=data
+                        data=data,
                     ),
                     ResponsePacket(
                         zn=0x01,
                         cc=CommandCodes.DECODE_MODE_STATUS_MCH,
                         ac=AnswerCodes.STATUS_UPDATE,
-                        data=self._decode_mode_mch
-                    )
+                        data=self._decode_mode_mch,
+                    ),
                 ]
 
             raise CommandNotRecognised()
 
         def get_decode_mode_2ch(self, **kwargs):
             return self._decode_mode_2ch
 
@@ -238,30 +293,33 @@
                 raise CommandInvalidAtThisTime()
 
     server = DummyServer(args.host, args.port, args.model)
     async with ServerContext(server):
         while True:
             await asyncio.sleep(delay=1)
 
-def main():
 
+def main():
     args = parser.parse_args()
 
     if args.verbose:
         root = logging.getLogger()
         root.setLevel(logging.DEBUG)
 
         channel = logging.StreamHandler(sys.stdout)
         channel.setLevel(logging.DEBUG)
-        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+        formatter = logging.Formatter(
+            "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+        )
         channel.setFormatter(formatter)
         root.addHandler(channel)
 
-    if args.subcommand == 'client':
+    if args.subcommand == "client":
         asyncio.run(run_client(args))
-    elif args.subcommand == 'state':
+    elif args.subcommand == "state":
         asyncio.run(run_state(args))
-    elif args.subcommand == 'server':
+    elif args.subcommand == "server":
         asyncio.run(run_server(args))
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `arcam-fmj-1.4.0/src/arcam/fmj/server.py` & `arcam_fmj-1.5.0/src/arcam/fmj/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,45 +8,52 @@
     AmxDuetResponse,
     AnswerCodes,
     CommandNotRecognised,
     CommandPacket,
     ResponseException,
     ResponsePacket,
     read_command,
-    write_packet
+    write_packet,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
-class Server():
+
+class Server:
     def __init__(self, host: str, port: int, model: str) -> None:
         self._server: Optional[asyncio.AbstractServer] = None
         self._host = host
         self._port = port
-        self._handlers: Dict[Union[Tuple[int, int], Tuple[int, int, bytes]], Callable] = dict()
+        self._handlers: Dict[
+            Union[Tuple[int, int], Tuple[int, int, bytes]], Callable
+        ] = dict()
         self._tasks: List[asyncio.Task] = list()
-        self._amxduet = AmxDuetResponse({
-            "Device-SDKClass": "Receiver",
-            "Device-Make": "ARCAM",
-            "Device-Model": model,
-            "Device-Revision": "x.y.z"
-        })
+        self._amxduet = AmxDuetResponse(
+            {
+                "Device-SDKClass": "Receiver",
+                "Device-Make": "ARCAM",
+                "Device-Model": model,
+                "Device-Revision": "x.y.z",
+            }
+        )
 
     async def process(self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
         _LOGGER.debug("Client connected")
         task = asyncio.current_task()
         assert task
         self._tasks.append(task)
         try:
             await self.process_runner(reader, writer)
         finally:
             _LOGGER.debug("Client disconnected")
             self._tasks.remove(task)
 
-    async def process_runner(self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
+    async def process_runner(
+        self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter
+    ):
         while True:
             request = await read_command(reader)
             if request is None:
                 _LOGGER.debug("Client disconnected")
                 return
 
             responses = await self.process_request(request)
@@ -60,55 +67,40 @@
 
         handler = self._handlers.get((request.zn, request.cc, request.data))
         if handler is None:
             handler = self._handlers.get((request.zn, request.cc))
 
         try:
             if handler:
-                data = handler(
-                    zn=request.zn,
-                    cc=request.cc,
-                    data=request.data)
+                data = handler(zn=request.zn, cc=request.cc, data=request.data)
 
                 if isinstance(data, bytes):
                     response = [
                         ResponsePacket(
-                            request.zn,
-                            request.cc,
-                            AnswerCodes.STATUS_UPDATE,
-                            data)
+                            request.zn, request.cc, AnswerCodes.STATUS_UPDATE, data
+                        )
                     ]
                 else:
                     response = data
             else:
                 raise CommandNotRecognised()
         except ResponseException as e:
-            response = [
-                ResponsePacket(
-                    request.zn,
-                    request.cc,
-                    e.ac,
-                    e.data or bytes()
-                )
-            ]
+            response = [ResponsePacket(request.zn, request.cc, e.ac, e.data or bytes())]
 
         return response
 
     def register_handler(self, zn, cc, data, fun):
         if data:
             self._handlers[(zn, cc, data)] = fun
         else:
             self._handlers[(zn, cc)] = fun
 
     async def start(self):
         _LOGGER.debug("Starting server")
-        self._server = await asyncio.start_server(
-            self.process,
-            self._host,
-            self._port)
+        self._server = await asyncio.start_server(self.process, self._host, self._port)
         return self
 
     async def stop(self):
         if self._server:
             _LOGGER.debug("Stopping server")
             self._server.close()
             await self._server.wait_closed()
@@ -117,15 +109,15 @@
         if self._tasks:
             _LOGGER.debug("Cancelling clients %s", self._tasks)
             for task in self._tasks:
                 task.cancel()
             await asyncio.wait(self._tasks)
 
 
-class ServerContext():
+class ServerContext:
     def __init__(self, server: Server):
         self._server = server
 
     async def __aenter__(self):
         await self._server.start()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `arcam-fmj-1.4.0/src/arcam/fmj/state.py` & `arcam_fmj-1.5.0/src/arcam/fmj/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,25 +33,29 @@
     VOLUME_STEP_SUPPORTED,
     RC5CODE_SOURCE,
     RC5CODE_POWER,
     RC5CODE_MUTE,
     RC5CODE_VOLUME,
     RC5CODE_DECODE_MODE_2CH,
     RC5CODE_DECODE_MODE_MCH,
+    UnsupportedZone,
 )
 from .client import Client
 
 _LOGGER = logging.getLogger(__name__)
 _T = TypeVar("_T")
 
-class State():
+
+class State:
     _state: Dict[int, Optional[bytes]]
     _presets: Dict[int, PresetDetail]
 
-    def __init__(self, client: Client, zn: int, api_model: ApiModel = ApiModel.API450_SERIES) -> None:
+    def __init__(
+        self, client: Client, zn: int, api_model: ApiModel = ApiModel.API450_SERIES
+    ) -> None:
         self._zn = zn
         self._client = client
         self._state = dict()
         self._presets = dict()
         self._amxduet: Optional[AmxDuetResponse] = None
         self._api_model = api_model
 
@@ -68,31 +72,33 @@
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.stop()
 
     def to_dict(self) -> Dict[str, Any]:
         return {
-            'POWER': self.get_power(),
-            'VOLUME': self.get_volume(),
-            'SOURCE': self.get_source(),
-            'MUTE': self.get_mute(),
-            'MENU': self.get_menu(),
-            'INCOMING_AUDIO_FORMAT': self.get_incoming_audio_format(),
-            'DECODE_MODE_2CH': self.get_decode_mode_2ch(),
-            'DECODE_MODE_MCH': self.get_decode_mode_mch(),
-            'DAB_STATION': self.get_dab_station(),
-            'DLS_PDT': self.get_dls_pdt(),
-            'RDS_INFORMATION': self.get_rds_information(),
-            'TUNER_PRESET': self.get_tuner_preset(),
-            'PRESET_DETAIL': self.get_preset_details(),
+            "POWER": self.get_power(),
+            "VOLUME": self.get_volume(),
+            "SOURCE": self.get_source(),
+            "MUTE": self.get_mute(),
+            "MENU": self.get_menu(),
+            "INCOMING_AUDIO_FORMAT": self.get_incoming_audio_format(),
+            "DECODE_MODE_2CH": self.get_decode_mode_2ch(),
+            "DECODE_MODE_MCH": self.get_decode_mode_mch(),
+            "DAB_STATION": self.get_dab_station(),
+            "DLS_PDT": self.get_dls_pdt(),
+            "RDS_INFORMATION": self.get_rds_information(),
+            "TUNER_PRESET": self.get_tuner_preset(),
+            "PRESET_DETAIL": self.get_preset_details(),
         }
 
     def __repr__(self) -> str:
-        return "State ({}) Amx ({})".format(self.to_dict(), self._amxduet.values if self._amxduet else {})
+        return "State ({}) Amx ({})".format(
+            self.to_dict(), self._amxduet.values if self._amxduet else {}
+        )
 
     def _listen(self, packet: Union[ResponsePacket, AmxDuetResponse]) -> None:
         if isinstance(packet, AmxDuetResponse):
             self._amxduet = packet
             return
 
         if packet.zn != self._zn:
@@ -119,56 +125,71 @@
 
     @property
     def revision(self) -> Optional[str]:
         if self._amxduet:
             return self._amxduet.device_revision
         return None
 
-    def get_rc5code(self, table: Dict[Tuple[ApiModel, int], Dict[_T, bytes]], value: _T) -> bytes:
+    def get_rc5code(
+        self, table: Dict[Tuple[ApiModel, int], Dict[_T, bytes]], value: _T
+    ) -> bytes:
         lookup = table.get((self._api_model, self._zn))
         if not lookup:
-            raise ValueError("Unkown mapping for model {} and zone {}".format(self._api_model, self._zn))
+            raise ValueError(
+                "Unkown mapping for model {} and zone {}".format(
+                    self._api_model, self._zn
+                )
+            )
 
         command = lookup.get(value)
         if not command:
-            raise ValueError("Unkown command for model {} and zone {} and value {}".format(self._api_model, self._zn, value))
+            raise ValueError(
+                "Unkown command for model {} and zone {} and value {}".format(
+                    self._api_model, self._zn, value
+                )
+            )
         return command
 
     def get(self, cc):
         return self._state[cc]
 
-    def get_incoming_audio_format(self) -> Union[Tuple[IncomingAudioFormat, IncomingAudioConfig], Tuple[None, None]]:
+    def get_incoming_audio_format(
+        self,
+    ) -> Union[Tuple[IncomingAudioFormat, IncomingAudioConfig], Tuple[None, None]]:
         value = self._state.get(CommandCodes.INCOMING_AUDIO_FORMAT)
         if value is None:
             return None, None
-        return (IncomingAudioFormat.from_int(value[0]),
-                IncomingAudioConfig.from_int(value[1]))
-
+        return (
+            IncomingAudioFormat.from_int(value[0]),
+            IncomingAudioConfig.from_int(value[1]),
+        )
 
     def get_decode_mode_2ch(self) -> Optional[DecodeMode2CH]:
         value = self._state.get(CommandCodes.DECODE_MODE_STATUS_2CH)
         if value is None:
             return None
         return DecodeMode2CH.from_bytes(value)
 
     async def set_decode_mode_2ch(self, mode: DecodeMode2CH) -> None:
         command = self.get_rc5code(RC5CODE_DECODE_MODE_2CH, mode)
         await self._client.request(
-            self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command)
+            self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command
+        )
 
     def get_decode_mode_mch(self) -> Optional[DecodeModeMCH]:
         value = self._state.get(CommandCodes.DECODE_MODE_STATUS_MCH)
         if value is None:
             return None
         return DecodeModeMCH.from_bytes(value)
 
     async def set_decode_mode_mch(self, mode: DecodeModeMCH) -> None:
         command = self.get_rc5code(RC5CODE_DECODE_MODE_MCH, mode)
         await self._client.request(
-            self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command)
+            self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command
+        )
 
     def get_2ch(self) -> bool:
         """Return if source is 2 channel or not."""
         audio_format, _ = self.get_incoming_audio_format()
         return bool(
             audio_format
             in (
@@ -181,21 +202,25 @@
 
     def get_decode_mode(self) -> Optional[Union[DecodeModeMCH, DecodeMode2CH]]:
         if self.get_2ch():
             return self.get_decode_mode_2ch()
         else:
             return self.get_decode_mode_mch()
 
-    def get_decode_modes(self) -> Optional[Union[List[DecodeModeMCH], List[DecodeMode2CH]]]:
+    def get_decode_modes(
+        self,
+    ) -> Optional[Union[List[DecodeModeMCH], List[DecodeMode2CH]]]:
         if self.get_2ch():
             return list(RC5CODE_DECODE_MODE_2CH[(self._api_model, self._zn)])
         else:
             return list(RC5CODE_DECODE_MODE_MCH[(self._api_model, self._zn)])
- 
-    async def set_decode_mode(self, mode: Union[str, DecodeModeMCH, DecodeMode2CH]) -> None:
+
+    async def set_decode_mode(
+        self, mode: Union[str, DecodeModeMCH, DecodeMode2CH]
+    ) -> None:
         if self.get_2ch():
             if isinstance(mode, str):
                 mode = DecodeMode2CH[mode]
             elif not isinstance(mode, DecodeMode2CH):
                 raise ValueError("Decode mode not supported at this time")
             await self.set_decode_mode_2ch(mode)
         else:
@@ -205,58 +230,63 @@
                 raise ValueError("Decode mode not supported at this time")
             await self.set_decode_mode_mch(mode)
 
     def get_power(self) -> Optional[bool]:
         value = self._state.get(CommandCodes.POWER)
         if value is None:
             return None
-        return int.from_bytes(value, 'big') == 0x01
+        return int.from_bytes(value, "big") == 0x01
 
     async def set_power(self, power: bool) -> None:
         if self._api_model in POWER_WRITE_SUPPORTED:
             bool_to_hex = 0x01 if power else 0x00
             if not power:
                 self._state[CommandCodes.POWER] = bytes([0])
             await self._client.request(
-                self._zn, CommandCodes.POWER, bytes([bool_to_hex]))
+                self._zn, CommandCodes.POWER, bytes([bool_to_hex])
+            )
         else:
             command = self.get_rc5code(RC5CODE_POWER, power)
             if power:
                 await self._client.request(
-                    self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command)
+                    self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command
+                )
             else:
                 # seed with a response, since device might not
                 # respond in timely fashion, so let's just
                 # assume we succeded until response come
                 # back.
                 self._state[CommandCodes.POWER] = bytes([0])
                 await self._client.send(
-                    self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command)
+                    self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command
+                )
 
     def get_menu(self) -> Optional[MenuCodes]:
         value = self._state.get(CommandCodes.MENU)
         if value is None:
             return None
         return MenuCodes.from_bytes(value)
 
     def get_mute(self) -> Optional[bool]:
         value = self._state.get(CommandCodes.MUTE)
         if value is None:
             return None
-        return int.from_bytes(value, 'big') == 0
+        return int.from_bytes(value, "big") == 0
 
     async def set_mute(self, mute: bool) -> None:
         if self._api_model in MUTE_WRITE_SUPPORTED:
             bool_to_hex = 0x00 if mute else 0x01
             await self._client.request(
-                self._zn, CommandCodes.MUTE, bytes([bool_to_hex]))
+                self._zn, CommandCodes.MUTE, bytes([bool_to_hex])
+            )
         else:
             command = self.get_rc5code(RC5CODE_MUTE, mute)
             await self._client.request(
-                self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command)
+                self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command
+            )
 
     def get_source(self) -> Optional[SourceCodes]:
         value = self._state.get(CommandCodes.CURRENT_SOURCE)
         if value is None:
             return None
         try:
             return SourceCodes.from_bytes(value, self._api_model, self._zn)
@@ -265,97 +295,102 @@
 
     def get_source_list(self) -> List[SourceCodes]:
         return list(RC5CODE_SOURCE[(self._api_model, self._zn)].keys())
 
     async def set_source(self, src: SourceCodes) -> None:
         if self._api_model in SOURCE_WRITE_SUPPORTED:
             value = src.to_bytes(self._api_model, self._zn)
-            await self._client.request(
-                self._zn, CommandCodes.CURRENT_SOURCE, value)
+            await self._client.request(self._zn, CommandCodes.CURRENT_SOURCE, value)
         else:
             command = self.get_rc5code(RC5CODE_SOURCE, src)
             await self._client.request(
-                self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command)
+                self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command
+            )
 
     def get_volume(self) -> Optional[int]:
         value = self._state.get(CommandCodes.VOLUME)
         if value is None:
             return None
-        return int.from_bytes(value, 'big')
+        return int.from_bytes(value, "big")
 
     async def set_volume(self, volume: int) -> None:
-        await self._client.request(
-            self._zn, CommandCodes.VOLUME, bytes([volume]))
+        await self._client.request(self._zn, CommandCodes.VOLUME, bytes([volume]))
 
     async def inc_volume(self) -> None:
         if self._api_model in VOLUME_STEP_SUPPORTED:
             await self._client.request(self._zn, CommandCodes.VOLUME, bytes([0xF1]))
         else:
             command = self.get_rc5code(RC5CODE_VOLUME, True)
             await self._client.request(
-                self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command)
+                self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command
+            )
 
     async def dec_volume(self) -> None:
         if self._api_model in VOLUME_STEP_SUPPORTED:
             await self._client.request(self._zn, CommandCodes.VOLUME, bytes([0xF2]))
         else:
             command = self.get_rc5code(RC5CODE_VOLUME, False)
             await self._client.request(
-                self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command)
+                self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command
+            )
 
     def get_dab_station(self) -> Optional[str]:
         value = self._state.get(CommandCodes.DAB_STATION)
         if value is None:
             return None
-        return value.decode('utf8').rstrip()
+        return value.decode("utf8").rstrip()
 
     def get_dls_pdt(self) -> Optional[str]:
         value = self._state.get(CommandCodes.DLS_PDT_INFO)
         if value is None:
             return None
-        return value.decode('utf8').rstrip()
+        return value.decode("utf8").rstrip()
 
     def get_rds_information(self) -> Optional[str]:
         value = self._state.get(CommandCodes.RDS_INFORMATION)
         if value is None:
             return None
-        return value.decode('utf8').rstrip()
+        return value.decode("utf8").rstrip()
 
     async def set_tuner_preset(self, preset: int) -> None:
         await self._client.request(self._zn, CommandCodes.TUNER_PRESET, bytes([preset]))
 
     def get_tuner_preset(self) -> Optional[int]:
         value = self._state.get(CommandCodes.TUNER_PRESET)
-        if value is None or value == b'\xff':
+        if value is None or value == b"\xff":
             return None
-        return int.from_bytes(value, 'big')
+        return int.from_bytes(value, "big")
 
     def get_preset_details(self) -> Dict[int, PresetDetail]:
         return self._presets
 
     async def update(self) -> None:
-        async def _update(cc):
+        async def _update(cc: CommandCodes):
             try:
                 data = await self._client.request(self._zn, cc, bytes([0xF0]))
                 self._state[cc] = data
+            except UnsupportedZone:
+                _LOGGER.debug("Unsupported zone %s for %s", self._zn, cc)
             except ResponseException as e:
                 _LOGGER.debug("Response error skipping %s - %s", cc, e.ac)
                 self._state[cc] = None
             except NotConnectedException as e:
                 _LOGGER.debug("Not connected skipping %s", cc)
                 self._state[cc] = None
             except asyncio.TimeoutError:
                 _LOGGER.error("Timeout requesting %s", cc)
 
         async def _update_presets() -> None:
             presets = {}
             for preset in range(1, 51):
                 try:
-                    data = await self._client.request(self._zn, CommandCodes.PRESET_DETAIL, bytes([preset]))
-                    if data != b'\x00':
+                    data = await self._client.request(
+                        self._zn, CommandCodes.PRESET_DETAIL, bytes([preset])
+                    )
+                    if data != b"\x00":
                         presets[preset] = PresetDetail.from_bytes(data)
                 except CommandInvalidAtThisTime:
                     break
                 except CommandNotRecognised:
                     _LOGGER.debug("Presets not supported skipping %s", preset)
                     break
                 except NotConnectedException as e:
@@ -381,41 +416,42 @@
                     self._api_model = ApiModel.APIHDA_SERIES
 
                 if data.device_model in APIVERSION_SA_SERIES:
                     self._api_model = ApiModel.APISA_SERIES
 
                 if data.device_model in APIVERSION_PA_SERIES:
                     self._api_model = ApiModel.APIPA_SERIES
-                
+
                 if data.device_model in APIVERSION_ST_SERIES:
                     self._api_model = ApiModel.APIST_SERIES
 
             except ResponseException as e:
                 _LOGGER.debug("Response error skipping %s", e.ac)
             except NotConnectedException as e:
                 _LOGGER.debug("Not connected skipping amx")
             except asyncio.TimeoutError:
                 _LOGGER.error("Timeout requesting amx")
 
         if self._client.connected:
             if self._amxduet is None:
                 await _update_amxduet()
 
-            await asyncio.gather(*[
-                _update(CommandCodes.POWER),
-                _update(CommandCodes.VOLUME),
-                _update(CommandCodes.MUTE),
-                _update(CommandCodes.CURRENT_SOURCE),
-                _update(CommandCodes.MENU),
-                _update(CommandCodes.DECODE_MODE_STATUS_2CH),
-                _update(CommandCodes.DECODE_MODE_STATUS_MCH),
-                _update(CommandCodes.INCOMING_AUDIO_FORMAT),
-                _update(CommandCodes.DAB_STATION),
-                _update(CommandCodes.DLS_PDT_INFO),
-                _update(CommandCodes.RDS_INFORMATION),
-                _update(CommandCodes.TUNER_PRESET),
-                _update_presets(),
-            ])
+            await asyncio.gather(
+                *[
+                    _update(CommandCodes.POWER),
+                    _update(CommandCodes.VOLUME),
+                    _update(CommandCodes.MUTE),
+                    _update(CommandCodes.CURRENT_SOURCE),
+                    _update(CommandCodes.MENU),
+                    _update(CommandCodes.DECODE_MODE_STATUS_2CH),
+                    _update(CommandCodes.DECODE_MODE_STATUS_MCH),
+                    _update(CommandCodes.INCOMING_AUDIO_FORMAT),
+                    _update(CommandCodes.DAB_STATION),
+                    _update(CommandCodes.DLS_PDT_INFO),
+                    _update(CommandCodes.RDS_INFORMATION),
+                    _update(CommandCodes.TUNER_PRESET),
+                    _update_presets(),
+                ]
+            )
         else:
             if self._state:
                 self._state = dict()
-
```

### Comparing `arcam-fmj-1.4.0/src/arcam/fmj/utils.py` & `arcam_fmj-1.5.0/src/arcam/fmj/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 from datetime import datetime, timedelta
 from defusedxml import ElementTree
 from typing import Optional, Any
 
 _LOGGER = logging.getLogger(__name__)
 
+
 def async_retry(attempts=2, allowed_exceptions=()):
     def decorator(f):
         @functools.wraps(f)
         async def wrapper(*args, **kwargs):
             attempt = attempts
             while True:
                 attempt -= 1
@@ -21,16 +22,18 @@
                     return await f(*args, **kwargs)
                 except allowed_exceptions:
                     if attempt == 0:
                         raise
                     _LOGGER.warning("Retrying: %s %s", f, args)
 
         return wrapper
+
     return decorator
 
+
 class Throttle:
     def __init__(self, delay: float) -> None:
         self._timestamp = datetime.now()
         self._lock = asyncio.Lock()
         self._delay = timedelta(seconds=delay)
 
     async def get(self) -> None:
@@ -57,21 +60,27 @@
 
 
 def get_possibly_invalid_xml(data) -> Any:
     try:
         return ElementTree.fromstring(data)
     except ElementTree.ParseError:
         _LOGGER.info("Device provide corrupt xml, trying with ampersand replacement")
-        data = re.sub(r'&(?![A-Za-z]+[0-9]*;|#[0-9]+;|#x[0-9a-fA-F]+;)', r'&amp;', data)
+        data = re.sub(r"&(?![A-Za-z]+[0-9]*;|#[0-9]+;|#x[0-9a-fA-F]+;)", r"&amp;", data)
         return ElementTree.fromstring(data)
 
+
 def get_udn_from_xml(xml: Any) -> Optional[str]:
-    return xml.findtext("d:device/d:UDN", None, {"d": "urn:schemas-upnp-org:device-1-0"})
+    return xml.findtext(
+        "d:device/d:UDN", None, {"d": "urn:schemas-upnp-org:device-1-0"}
+    )
+
 
-async def get_uniqueid_from_device_description(session: aiohttp.ClientSession, url: str):
+async def get_uniqueid_from_device_description(
+    session: aiohttp.ClientSession, url: str
+):
     """Retrieve and extract unique id from url."""
     try:
         async with session.get(url) as req:
             req.raise_for_status()
             data = await req.text()
             xml = get_possibly_invalid_xml(data)
             udn = get_udn_from_xml(xml)
```

