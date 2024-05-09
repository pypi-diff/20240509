# Comparing `tmp/pytrydan-0.4.0.tar.gz` & `tmp/pytrydan-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrydan-0.4.0.tar", max compression
+gzip compressed data, was "pytrydan-0.5.0.tar", max compression
```

## Comparing `pytrydan-0.4.0.tar` & `pytrydan-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-11-09 23:52:46.739224 pytrydan-0.4.0/LICENSE
--rw-r--r--   0        0        0     4822 2023-11-09 23:52:46.739224 pytrydan-0.4.0/README.md
--rw-r--r--   0        0        0     3480 2023-11-09 23:52:47.495232 pytrydan-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      754 2023-11-09 23:52:46.739224 pytrydan-0.4.0/src/pytrydan/__init__.py
--rw-r--r--   0        0        0      102 2023-11-09 23:52:46.739224 pytrydan-0.4.0/src/pytrydan/__main__.py
--rw-r--r--   0        0        0     1448 2023-11-09 23:52:46.739224 pytrydan-0.4.0/src/pytrydan/cli.py
--rw-r--r--   0        0        0      340 2023-11-09 23:52:46.739224 pytrydan-0.4.0/src/pytrydan/const.py
--rw-r--r--   0        0        0      562 2023-11-09 23:52:46.739224 pytrydan-0.4.0/src/pytrydan/exceptions.py
--rw-r--r--   0        0        0     1538 2023-11-09 23:52:46.739224 pytrydan-0.4.0/src/pytrydan/main.py
--rw-r--r--   0        0        0     3126 2023-11-09 23:52:46.739224 pytrydan-0.4.0/src/pytrydan/models/trydan.py
--rw-r--r--   0        0        0        0 2023-11-09 23:52:46.739224 pytrydan-0.4.0/src/pytrydan/py.typed
--rw-r--r--   0        0        0     8990 2023-11-09 23:52:46.743224 pytrydan-0.4.0/src/pytrydan/trydan.py
--rw-r--r--   0        0        0     6029 1970-01-01 00:00:00.000000 pytrydan-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-09 00:20:48.331840 pytrydan-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4822 2024-05-09 00:20:48.331840 pytrydan-0.5.0/README.md
+-rw-r--r--   0        0        0     3517 2024-05-09 00:20:49.615843 pytrydan-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      754 2024-05-09 00:20:48.335840 pytrydan-0.5.0/src/pytrydan/__init__.py
+-rw-r--r--   0        0        0      102 2024-05-09 00:20:48.335840 pytrydan-0.5.0/src/pytrydan/__main__.py
+-rw-r--r--   0        0        0     2003 2024-05-09 00:20:48.335840 pytrydan-0.5.0/src/pytrydan/cli.py
+-rw-r--r--   0        0        0      340 2024-05-09 00:20:48.335840 pytrydan-0.5.0/src/pytrydan/const.py
+-rw-r--r--   0        0        0      562 2024-05-09 00:20:48.335840 pytrydan-0.5.0/src/pytrydan/exceptions.py
+-rw-r--r--   0        0        0     2053 2024-05-09 00:20:48.335840 pytrydan-0.5.0/src/pytrydan/main.py
+-rw-r--r--   0        0        0     3308 2024-05-09 00:20:48.335840 pytrydan-0.5.0/src/pytrydan/models/trydan.py
+-rw-r--r--   0        0        0        0 2024-05-09 00:20:48.335840 pytrydan-0.5.0/src/pytrydan/py.typed
+-rw-r--r--   0        0        0     9118 2024-05-09 00:20:48.335840 pytrydan-0.5.0/src/pytrydan/trydan.py
+-rw-r--r--   0        0        0     6029 1970-01-01 00:00:00.000000 pytrydan-0.5.0/PKG-INFO
```

### Comparing `pytrydan-0.4.0/LICENSE` & `pytrydan-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrydan-0.4.0/README.md` & `pytrydan-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pytrydan-0.4.0/pyproject.toml` & `pytrydan-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytrydan"
-version = "0.4.0"
+version = "0.5.0"
 description = "Library to interface with V2C EVSE Trydan"
 authors = ["Diogo Gomes <diogogomes@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dgomes/pytrydan"
 documentation = "https://pytrydan.readthedocs.io"
 classifiers = [
@@ -36,14 +36,16 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
 python-semantic-release = "^8.3.0"
 pytest-asyncio = "^0.21.1"
 syrupy = "^4.6.0"
 respx = "^0.20.2"
+tenacity = "^8.2.3"
+typer = "^0.9.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
```

### Comparing `pytrydan-0.4.0/src/pytrydan/__init__.py` & `pytrydan-0.5.0/src/pytrydan/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrydan-0.4.0/src/pytrydan/cli.py` & `pytrydan-0.5.0/src/pytrydan/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import asyncio
 from ipaddress import ip_address
 
 import typer
 from rich import print
 
 from .main import (
+    trydan_charging,
+    trydan_connected,
     trydan_intensity,
     trydan_lock,
     trydan_pause,
+    trydan_ready,
     trydan_resume,
     trydan_set,
     trydan_status,
     trydan_unlock,
 )
 
 app = typer.Typer()
@@ -22,14 +25,38 @@
     """Retrieve Trydan Status."""
     print("Connecting to %s", ip_address(ip))
 
     asyncio.run(trydan_status(ip))
 
 
 @app.command()
+def connected(ip: str) -> None:
+    """Retrieve Trydan Status."""
+    print("Connecting to %s", ip_address(ip))
+
+    asyncio.run(trydan_connected(ip))
+
+
+@app.command()
+def charging(ip: str) -> None:
+    """Retrieve Trydan Status."""
+    print("Connecting to %s", ip_address(ip))
+
+    asyncio.run(trydan_charging(ip))
+
+
+@app.command()
+def ready(ip: str) -> None:
+    """Retrieve Trydan Status."""
+    print("Connecting to %s", ip_address(ip))
+
+    asyncio.run(trydan_ready(ip))
+
+
+@app.command()
 def pause(ip: str) -> None:
     """Pause Trydan EVSE."""
     print("Connecting to %s", ip_address(ip))
 
     asyncio.run(trydan_pause(ip))
```

### Comparing `pytrydan-0.4.0/src/pytrydan/exceptions.py` & `pytrydan-0.5.0/src/pytrydan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytrydan-0.4.0/src/pytrydan/main.py` & `pytrydan-0.5.0/src/pytrydan/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,44 @@
     data = await trydan.get_data()
 
     print(data)
 
     return 0
 
 
+async def trydan_connected(ip: str) -> int:
+    """Retrieve Trydan Status."""
+    trydan = Trydan(ip)
+    await trydan.get_data()
+
+    print(trydan.connected)
+
+    return 0
+
+
+async def trydan_charging(ip: str) -> int:
+    """Retrieve Trydan Status."""
+    trydan = Trydan(ip)
+    await trydan.get_data()
+
+    print(trydan.charging)
+
+    return 0
+
+
+async def trydan_ready(ip: str) -> int:
+    """Retrieve Trydan Status."""
+    trydan = Trydan(ip)
+    await trydan.get_data()
+
+    print(trydan.ready)
+
+    return 0
+
+
 async def trydan_set(ip: str, keyword: str, value: str) -> int:
     """Set KeyWord value in Trydan."""
     trydan = Trydan(ip)
     try:
         await trydan.set_keyword(keyword, value)
     except Exception as e:
         print(e)
```

### Comparing `pytrydan-0.4.0/src/pytrydan/models/trydan.py` & `pytrydan-0.5.0/src/pytrydan/models/trydan.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 
 class SlaveCommunicationState(IntEnum):
     """Enum for Slave Communication State."""
 
     NO_ERROR = 0
     ERROR_MESSAGE = 1
     COMMUNICATION_ERROR = 2
+    UNKNOWN_ERROR_1 = 3
+    UNKNOWN_ERROR_2 = 4
 
 
 class PauseState(IntEnum):
     """Enum for Pause State."""
 
     PAUSED = 1
     NOT_PAUSED = 0
@@ -74,22 +76,24 @@
     TIMED_POWER_DISABLED_AND_STOP_MODE_SETTED = 5
 
 
 @dataclass(slots=True)
 class TrydanData:
     """Model for Trydan data."""
 
+    ID: str | None
     charge_state: int
     ready_state: int | None
     charge_power: float
     charge_energy: float
     slave_error: SlaveCommunicationState
     charge_time: int
     house_power: int
     fv_power: float
+    battery_power: float | None
     paused: int
     locked: LockState
     timer: ChargePointTimerState
     intensity: int
     dynamic: DynamicState
     min_intensity: int
     max_intensity: int
@@ -98,22 +102,24 @@
     contracted_power: int
     firmware_version: str | None
 
     @classmethod
     def from_api(cls, data: dict[str, Any]) -> TrydanData:
         """Initialize from the API."""
         return cls(
+            ID=data.get("ID"),
             charge_state=ChargeState(data["ChargeState"]),
             ready_state=ReadyState(data.get("ReadyState", 0)),
             charge_power=data["ChargePower"],
             charge_energy=data["ChargeEnergy"],
             slave_error=SlaveCommunicationState(data["SlaveError"]),
             charge_time=data["ChargeTime"],
             house_power=data["HousePower"],
             fv_power=data["FVPower"],
+            battery_power=data.get("BatteryPower"),
             paused=PauseState(data["Paused"]),
             locked=LockState(data["Locked"]),
             timer=ChargePointTimerState(data["Timer"]),
             intensity=data["Intensity"],
             dynamic=DynamicState(data["Dynamic"]),
             min_intensity=data["MinIntensity"],
             max_intensity=data["MaxIntensity"],
```

### Comparing `pytrydan-0.4.0/src/pytrydan/trydan.py` & `pytrydan-0.5.0/src/pytrydan/trydan.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,16 @@
         )
 
         status_code = response.status_code
         if status_code in (HTTPStatus.UNAUTHORIZED, HTTPStatus.FORBIDDEN):
             raise TrydanCommunicationError(
                 f"Failed for {url} with status {status_code}"
             )
+        if status_code != HTTPStatus.OK:
+            raise TrydanInvalidResponse(f"Failed for {url} with status {status_code}")
 
         return response
 
     async def _json_request(self, end_point: str) -> Any:
         """Make a request to Trydan and return the JSON response."""
         response = await self._request(end_point)
         try:
```

### Comparing `pytrydan-0.4.0/PKG-INFO` & `pytrydan-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrydan
-Version: 0.4.0
+Version: 0.5.0
 Summary: Library to interface with V2C EVSE Trydan
 Home-page: https://github.com/dgomes/pytrydan
 License: MIT
 Author: Diogo Gomes
 Author-email: diogogomes@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytrydan Version: 0.4.0 Summary: Library to
+Metadata-Version: 2.1 Name: pytrydan Version: 0.5.0 Summary: Library to
 interface with V2C EVSE Trydan Home-page: https://github.com/dgomes/pytrydan
 License: MIT Author: Diogo Gomes Author-email: diogogomes@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

