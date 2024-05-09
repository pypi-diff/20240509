# Comparing `tmp/webio_api-0.1.8.tar.gz` & `tmp/webio_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webio_api-0.1.8.tar", last modified: Fri Sep 22 15:16:06 2023, max compression
+gzip compressed data, was "webio_api-0.1.9.tar", last modified: Thu Oct  5 14:46:13 2023, max compression
```

## Comparing `webio_api-0.1.8.tar` & `webio_api-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 lukasz    (1000) lukasz    (1000)        0 2023-09-22 15:16:06.792618 webio_api-0.1.8/
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)     1065 2023-07-20 14:40:23.000000 webio_api-0.1.8/LICENSE
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      479 2023-09-22 15:16:06.792618 webio_api-0.1.8/PKG-INFO
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      113 2023-07-20 14:41:45.000000 webio_api-0.1.8/README.md
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)       38 2023-09-22 15:16:06.792618 webio_api-0.1.8/setup.cfg
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      570 2023-09-22 15:15:03.000000 webio_api-0.1.8/setup.py
-drwxrwxr-x   0 lukasz    (1000) lukasz    (1000)        0 2023-09-22 15:16:06.792618 webio_api-0.1.8/webio_api/
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)    14180 2023-09-22 15:15:42.000000 webio_api-0.1.8/webio_api/__init__.py
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)     5691 2023-09-22 14:27:01.000000 webio_api-0.1.8/webio_api/api_client.py
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)     1571 2023-09-22 14:27:01.000000 webio_api-0.1.8/webio_api/const.py
-drwxrwxr-x   0 lukasz    (1000) lukasz    (1000)        0 2023-09-22 15:16:06.792618 webio_api-0.1.8/webio_api.egg-info/
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      479 2023-09-22 15:16:06.000000 webio_api-0.1.8/webio_api.egg-info/PKG-INFO
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      223 2023-09-22 15:16:06.000000 webio_api-0.1.8/webio_api.egg-info/SOURCES.txt
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)        1 2023-09-22 15:16:06.000000 webio_api-0.1.8/webio_api.egg-info/dependency_links.txt
--rw-rw-r--   0 lukasz    (1000) lukasz    (1000)       10 2023-09-22 15:16:06.000000 webio_api-0.1.8/webio_api.egg-info/top_level.txt
+drwxrwxr-x   0 lukasz    (1000) lukasz    (1000)        0 2023-10-05 14:46:13.640898 webio_api-0.1.9/
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)     1065 2023-07-20 14:40:23.000000 webio_api-0.1.9/LICENSE
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      479 2023-10-05 14:46:13.640898 webio_api-0.1.9/PKG-INFO
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      113 2023-07-20 14:41:45.000000 webio_api-0.1.9/README.md
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)       38 2023-10-05 14:46:13.640898 webio_api-0.1.9/setup.cfg
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      570 2023-10-05 14:45:58.000000 webio_api-0.1.9/setup.py
+drwxrwxr-x   0 lukasz    (1000) lukasz    (1000)        0 2023-10-05 14:46:13.640898 webio_api-0.1.9/webio_api/
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)    14178 2023-10-05 14:44:46.000000 webio_api-0.1.9/webio_api/__init__.py
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)     5689 2023-10-05 14:44:46.000000 webio_api-0.1.9/webio_api/api_client.py
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)     1571 2023-10-03 14:17:00.000000 webio_api-0.1.9/webio_api/const.py
+drwxrwxr-x   0 lukasz    (1000) lukasz    (1000)        0 2023-10-05 14:46:13.640898 webio_api-0.1.9/webio_api.egg-info/
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      479 2023-10-05 14:46:13.000000 webio_api-0.1.9/webio_api.egg-info/PKG-INFO
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)      223 2023-10-05 14:46:13.000000 webio_api-0.1.9/webio_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)        1 2023-10-05 14:46:13.000000 webio_api-0.1.9/webio_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 lukasz    (1000) lukasz    (1000)       10 2023-10-05 14:46:13.000000 webio_api-0.1.9/webio_api.egg-info/top_level.txt
```

### Comparing `webio_api-0.1.8/LICENSE` & `webio_api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `webio_api-0.1.8/setup.py` & `webio_api-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name="webio_api",
-    version="0.1.8",
+    version="0.1.9",
     author="nasWebio",
     author_email="devel_team@chomtech.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nasWebio/webio_api",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webio_api-0.1.8/webio_api/__init__.py` & `webio_api-0.1.9/webio_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,42 +165,42 @@
     async def refresh_device_info(self) -> bool:
         info = await self._api_client.get_info()
         try:
             serial: str = info[KEY_WEBIO_SERIAL]
             self._info[KEY_DEVICE_SERIAL] = serial.replace("-", "")
             self._info[KEY_DEVICE_NAME] = info[KEY_WEBIO_NAME]
         except (KeyError, AttributeError):
-            _LOGGER.warning("get_info: response has missing/invalid values")
+            _LOGGER.warning("Get_info: response has missing/invalid values")
             return False
         self.temp_sensor = TempSensor(self._info[KEY_DEVICE_SERIAL], None)
         self.thermostat = Thermostat(self._info[KEY_DEVICE_SERIAL], self._api_client)
         return True
 
     async def status_subscription(self, address: str, subscribe: bool) -> bool:
         return await self._api_client.status_subscription(address, subscribe)
 
     def update_device_status(self, new_status: dict[str, Any]) -> dict[str, list]:
         webio_outputs: Optional[list[dict[str, Any]]] = new_status.get(KEY_OUTPUTS)
         new_outputs: list[Output] = []
         if webio_outputs is None:
-            _LOGGER.error("No outputs data in status update")
+            _LOGGER.debug("No outputs data in status update")
         else:
             new_outputs = self._update_outputs(webio_outputs)
 
         webio_inputs: Optional[list[dict[str, Any]]] = new_status.get(KEY_INPUTS)
         new_inputs: list[Input] = []
         if webio_inputs is None:
-            _LOGGER.error("No inputs data in status update")
+            _LOGGER.debug("No inputs data in status update")
         else:
             new_inputs = self._update_inputs(webio_inputs)
 
         webio_zones: Optional[list[dict[str, Any]]] = new_status.get(KEY_ZONES)
         new_zones: list[Zone] = []
         if webio_zones is None:
-            _LOGGER.error("No zones data in status update")
+            _LOGGER.debug("No zones data in status update")
         else:
             new_zones = self._update_zones(webio_zones)
 
         self._update_temp_sensor(new_status.get(KEY_DEVICE_TEMP_ENV, "N/A"))
 
         webio_thermostat: dict[str, Any] = new_status.get(KEY_THERMOSTAT, {})
         self._update_thermostat(webio_thermostat)
@@ -236,15 +236,15 @@
         for out in self.outputs:
             out.state = None
             out.available = None
 
         for o in outputs:
             index: int = o.get(KEY_INDEX, -1)
             if index < 0:
-                _LOGGER.error("WebIO output has no index")
+                _LOGGER.debug("WebIO output has no index")
                 continue
             current_indexes.append(index)
             webio_output: Optional[Output] = self._get_output(index)
             if webio_output is None:
                 webio_output = Output(
                     self._info[KEY_DEVICE_SERIAL], self._api_client, index
                 )
@@ -268,15 +268,15 @@
         for webio_input in self.inputs:
             webio_input.state = None
             webio_input.available = False
 
         for i in inputs:
             index: int = i.get(KEY_INDEX, -1)
             if index < 0:
-                _LOGGER.error("WebIO input has no index")
+                _LOGGER.debug("WebIO input has no index")
                 continue
             current_indexes.append(index)
             webio_input: Optional[Input] = self._get_input(index)
             if webio_input is None:
                 webio_input = Input(
                     self._info[KEY_DEVICE_SERIAL], index
                 )
@@ -300,15 +300,15 @@
         for zone in self.zones:
             zone.state = None
             zone.available = False
 
         for z in zones:
             index: int = z.get(KEY_INDEX, -1)
             if index < 0:
-                _LOGGER.error("WebIO zone has no index")
+                _LOGGER.debug("WebIO zone has no index")
                 continue
             current_indexes.append(index)
             name: Optional[str] = z.get(KEY_NAME)
             state: Optional[str] = z.get(KEY_STATUS)
             webio_zone: Optional[Zone] = self._get_zone(index)
             if webio_zone is None:
                 webio_zone = Zone(
@@ -328,23 +328,23 @@
 
     def _update_temp_sensor(self, temp_value: str) -> None:
         try:
             new_value = None if temp_value == "N/A" else int(temp_value)
         except ValueError:
             new_value = None
         if self.temp_sensor is None:
-            _LOGGER.error("TempSensor is None, cannot update status")
+            _LOGGER.debug("TempSensor is None, cannot update status")
             return
         self.temp_sensor.last_update = time.time()
         self.temp_sensor.value = new_value
         self.temp_sensor.available = self.temp_sensor.value is not None
 
     def _update_thermostat(self, thermostat: dict[str, Any]) -> None:
         if self.thermostat is None:
-            _LOGGER.warning("Cannot update Thermostat status. Thermostat is None")
+            _LOGGER.debug("Cannot update Thermostat status. Thermostat is None")
             return
         if len(thermostat) <= 6:
             self.thermostat.available = False
             return
         self.thermostat.name = thermostat.get(KEY_NAME)
         self.thermostat.temp_target_min = WebioAPI.get_int_or_none(
             thermostat.get(KEY_RANGE_FROM)
```

### Comparing `webio_api-0.1.8/webio_api/api_client.py` & `webio_api-0.1.9/webio_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,26 +57,26 @@
         response = await self._send_request(EP_DEVICE_INFO, data)
         if response is None:
             return {}
         try:
             info = json.loads(response)
             return info
         except json.JSONDecodeError as e:
-            _LOGGER.warning("get_info: received invalid json: %s", e.msg)
+            _LOGGER.warning("Get_info: received invalid json: %s", e.msg)
         return {}
 
     async def set_output(self, index: int, new_state: bool) -> bool:
         data = {
             KEY_LOGIN: self._login,
             KEY_PASSWORD: self._password,
             KEY_INDEX: index,
             KEY_STATUS: new_state,
         }
         result = await self._send_regular_request(EP_SET_OUTPUT, data)
-        _LOGGER.debug("set_output(%s, %s): %s", index, new_state, result)
+        _LOGGER.debug("Set_output(%s, %s): %s", index, new_state, result)
         return result
 
     async def arm_zone(self, index: int, arm: bool, passcode: Optional[str]) -> bool:
         passcode_sha = ""
         if passcode:
             hash_object = hashlib.sha1(passcode.encode("utf-8"))
             passcode_sha = hash_object.hexdigest().upper()
@@ -84,63 +84,63 @@
             KEY_LOGIN: self._login,
             KEY_PASSWORD: self._password,
             KEY_INDEX: f"{index}",
             KEY_STATUS: arm,
             KEY_PASSCODE: passcode_sha
         }
         result = await self._send_regular_request(EP_ARM_ZONE, data)
-        _LOGGER.debug("arm_zone(%s, %s, [password]): %s", index, arm, result)
+        _LOGGER.debug("Arm_zone(%s, %s, [password]): %s", index, arm, result)
         return result
 
     async def set_hvac_mode(self, hvac_mode: str) -> bool:
         have_cooling = "cool" in hvac_mode
         have_heating = "heat" in hvac_mode
         data = {
             KEY_LOGIN: self._login,
             KEY_PASSWORD: self._password,
             KEY_ACTION: "set_hvac_mode",
             KEY_BELOW: have_heating,
             KEY_ABOVE: have_cooling,
         }
         result = await self._send_regular_request(EP_THERMOSTAT, data)
-        _LOGGER.debug("set_hvac_mode(%s): %s", hvac_mode, result)
+        _LOGGER.debug("Set_hvac_mode(%s): %s", hvac_mode, result)
         return result
 
     async def set_temperature(self, temp_min: int, temp_max: int) -> bool:
         data = {
             KEY_LOGIN: self._login,
             KEY_PASSWORD: self._password,
             KEY_ACTION: "set_temp_range",
             KEY_TEMP_MIN: temp_min,
             KEY_TEMP_MAX: temp_max,
         }
         result = await self._send_regular_request(EP_THERMOSTAT, data)
-        _LOGGER.debug("set_temperature(%s, %s): %s", temp_min, temp_max, result)
+        _LOGGER.debug("Set_temperature(%s, %s): %s", temp_min, temp_max, result)
         return result
 
     async def status_subscription(self, address: str, subscribe: bool) -> bool:
         data = {
             KEY_LOGIN: self._login,
             KEY_PASSWORD: self._password,
             KEY_ADDRESS: address,
             KEY_SUBSCRIBE: subscribe,
         }
         result = await self._send_regular_request(EP_STATUS_SUBSCRIPTION, data)
-        _LOGGER.debug("status_subscription(%s, %s): %s", address, subscribe, result)
+        _LOGGER.debug("Status_subscription(%s, %s): %s", address, subscribe, result)
         return result
 
     async def _send_regular_request(self, ep: str, data: dict) -> bool:
         response = await self._send_request(ep, data)
         if response is None:
             return False
         try:
             response_dict: dict = json.loads(response)
             return response_dict.get(KEY_ANSWER, "") == "OK"
         except json.JSONDecodeError as e:
-            _LOGGER.warning("regular_request: invalid json in response -> %s", e.msg)
+            _LOGGER.warning("Request error: invalid json in response -> %s", e.msg)
         return False
 
     async def _send_request(
         self, ep: str, data: Optional[dict] = None
     ) -> Optional[str]:
         async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=REQUEST_TIMEOUT)) as session:
             full_request = f"https://{self._host}/{ep}"
```

### Comparing `webio_api-0.1.8/webio_api/const.py` & `webio_api-0.1.9/webio_api/const.py`

 * *Files identical despite different names*

