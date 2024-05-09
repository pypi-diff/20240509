# Comparing `tmp/duwi_smart_sdk-0.1.6.tar.gz` & `tmp/duwi_smart_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.1.6.tar", last modified: Tue May  7 09:10:32 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.1.7.tar", last modified: Thu May  9 02:49:56 2024, max compression
```

## Comparing `duwi_smart_sdk-0.1.6.tar` & `duwi_smart_sdk-0.1.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:10:32.824149 duwi_smart_sdk-0.1.6/
--rw-rw-rw-   0        0        0      649 2024-05-07 09:10:32.823173 duwi_smart_sdk-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      147 2024-05-07 06:42:21.000000 duwi_smart_sdk-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 09:10:32.774180 duwi_smart_sdk-0.1.6/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:10:32.790950 duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     2098 2024-05-07 08:49:07.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/account.py
--rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     4314 2024-05-07 09:09:43.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2686 2024-05-07 09:08:05.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     2156 2024-05-07 08:49:07.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     4788 2024-05-07 07:31:40.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:10:32.796808 duwi_smart_sdk-0.1.6/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:10:32.797783 duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:10:32.799736 duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:10:32.806573 duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/resp/house.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:10:32.811455 duwi_smart_sdk-0.1.6/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:10:32.781543 duwi_smart_sdk-0.1.6/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      649 2024-05-07 09:10:32.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1227 2024-05-07 09:10:32.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:10:32.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-07 09:10:32.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-07 09:10:32.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-07 09:10:32.000000 duwi_smart_sdk-0.1.6/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 09:10:32.824149 duwi_smart_sdk-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-05-07 09:10:26.000000 duwi_smart_sdk-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:10:32.812431 duwi_smart_sdk-0.1.6/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:10:32.820242 duwi_smart_sdk-0.1.6/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.1.6/test/api/__init__.py
--rw-rw-rw-   0        0        0      949 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.6/test/api/test_control.py
--rw-rw-rw-   0        0        0      812 2024-05-07 06:26:29.000000 duwi_smart_sdk-0.1.6/test/api/test_discover.py
--rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.1.6/test/api/test_house.py
--rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.1.6/test/api/test_login.py
--rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.1.6/test/api/test_ws.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:10:32.822196 duwi_smart_sdk-0.1.6/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.6/test/util/__init__.py
--rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.1.6/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:56.917475 duwi_smart_sdk-0.1.7/
+-rw-rw-rw-   0        0        0      649 2024-05-09 02:49:56.917475 duwi_smart_sdk-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2024-05-07 06:42:21.000000 duwi_smart_sdk-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:56.864101 duwi_smart_sdk-0.1.7/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:56.881436 duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2098 2024-05-07 08:49:07.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/account.py
+-rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4587 2024-05-09 02:49:53.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2686 2024-05-07 09:08:05.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2156 2024-05-07 08:49:07.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     4788 2024-05-07 07:31:40.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:56.887501 duwi_smart_sdk-0.1.7/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:56.888437 duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:56.890431 duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:56.896436 duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/resp/house.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:56.903437 duwi_smart_sdk-0.1.7/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:56.872436 duwi_smart_sdk-0.1.7/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      649 2024-05-09 02:49:56.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1227 2024-05-09 02:49:56.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 02:49:56.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-09 02:49:56.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-09 02:49:56.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-09 02:49:56.000000 duwi_smart_sdk-0.1.7/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 02:49:56.917475 duwi_smart_sdk-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      936 2024-05-09 02:49:53.000000 duwi_smart_sdk-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:56.904437 duwi_smart_sdk-0.1.7/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:56.913479 duwi_smart_sdk-0.1.7/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.1.7/test/api/__init__.py
+-rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.1.7/test/api/test_control.py
+-rw-rw-rw-   0        0        0      812 2024-05-07 06:26:29.000000 duwi_smart_sdk-0.1.7/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.1.7/test/api/test_house.py
+-rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.1.7/test/api/test_login.py
+-rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.1.7/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:56.915435 duwi_smart_sdk-0.1.7/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.7/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.1.7/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.1.6/PKG-INFO` & `duwi_smart_sdk-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/account.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/discover.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import logging
 
 from typing import Optional
 from typing import List
 
-
 from duwi_smart_sdk.model.resp.device import Device
 from duwi_smart_sdk.util.http import get
 from duwi_smart_sdk.const.status import Code
 from duwi_smart_sdk.const.const import URL
 from duwi_smart_sdk.util.sign import md5_encrypt
 from duwi_smart_sdk.util.timestamp import current_timestamp
 
@@ -38,49 +37,56 @@
         self._app_key = app_key
         self._app_secret = app_secret
         self._access_token = access_token
         self._app_version = app_version
         self._client_version = client_version
         self._client_model = client_model
 
-
-    async def discover(self, house_no: str) -> tuple[str, Optional[List[Device]]]:
+    async def discover(self, house_nos: str) -> tuple[str, Optional[List[Device]]]:
         """
         Retrieves a list of devices associated with the specified house number.
 
         :param access_token: The access token for interacting with the cloud service.
         :param house_no: The house number for which to discover devices.
         :return: A tuple containing the status of the operation and a list of Device objects, or None if unsuccessful.
         """
-        body = {}
-        body_string = json.dumps(body, separators=(',', ':'))
-
-        # Generate a signature using the body string, app secret, and the current timestamp.
-        sign = md5_encrypt(f"houseNo={house_no}{self._app_secret}{current_timestamp()}")
+        status = None
+        message = None
+        res = None
+        devices_objects = []
+        # status, message, res
+        for house_no in house_nos:
+            body = {}
+            body_string = json.dumps(body, separators=(',', ':'))
+
+            # Generate a signature using the body string, app secret, and the current timestamp.
+            sign = md5_encrypt(f"houseNo={house_no}{self._app_secret}{current_timestamp()}")
+
+            headers = {
+                'Content-Type': 'application/json',
+                'accessToken': self._access_token,
+                'appkey': self._app_key,
+                'secret': self._app_secret,
+                'time': str(current_timestamp()),  # Ensure it's converted to string
+                'sign': sign,
+                'appVersion': self._app_version,
+                'clientVersion': self._client_version,
+                'clientModel': self._client_model
+            }
+
+            status, message, res = await get(f"{self._url}/device/infos?houseNo={house_no}", headers, body)
+
+            if status == Code.SUCCESS.value:
+                devices = res.get("devices", [])
+                ds = self._create_device_obj(device)
+                devices_objects = devices_objects.extend(ds)
+            # else:
+            #     return status, None
 
-        headers = {
-            'Content-Type': 'application/json',
-            'accessToken': self._access_token,
-            'appkey': self._app_key,
-            'secret': self._app_secret,
-            'time': str(current_timestamp()),  # Ensure it's converted to string
-            'sign': sign,
-            'appVersion': self._app_version,
-            'clientVersion': self._client_version,
-            'clientModel': self._client_model
-        }
-
-        status, message, res = await get(f"{self._url}/device/infos?houseNo={house_no}", headers, body)
-
-        if status == Code.SUCCESS.value:
-            devices = res.get("devices", [])
-            devices_objects = [self._create_device_obj(device) for device in devices]
-            return status, devices_objects
-        else:
-            return status, None
+        return status, devices_objects
 
     @staticmethod
     def _create_device_obj(device_dict: dict) -> Device:
         """
         Converts a dictionary representing a device into a Device object.
 
         :param device_dict: A dictionary containing device details.
```

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/const/status.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi-smart-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.1.6/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.1.7/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/setup.py` & `duwi_smart_sdk-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.1.6/test/api/test_control.py` & `duwi_smart_sdk-0.1.7/test/api/test_control.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                 app_secret="26af4883a943083a4c34083897fcea10",
                 access_token="715d1c63-85c0-4d74-9a89-5a0aa4806f74",
                 app_version="0.0.1",
                 client_version="0.0.1",
                 client_model="homeassistant",
             )
             cd = ControlDevice(
-                device_no="F17000000001-63",
+                device_no="F15000000001-4",
                 house_no="c7bf567d-225a-4533-ab72-5dc080b794f5",
             )
             cd.add_param_info("switch", "off")
             res =  await cc.control(cd)
             print(res)
 
         asyncio.run(run_test())
```

### Comparing `duwi_smart_sdk-0.1.6/test/api/test_discover.py` & `duwi_smart_sdk-0.1.7/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/test/api/test_house.py` & `duwi_smart_sdk-0.1.7/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/test/api/test_login.py` & `duwi_smart_sdk-0.1.7/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/test/api/test_ws.py` & `duwi_smart_sdk-0.1.7/test/api/test_ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.6/test/util/test_http.py` & `duwi_smart_sdk-0.1.7/test/util/test_http.py`

 * *Files identical despite different names*

