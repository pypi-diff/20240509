# Comparing `tmp/washpy-0.2.1.tar.gz` & `tmp/washpy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "washpy-0.2.1.tar", max compression
+gzip compressed data, was "washpy-0.2.2.tar", max compression
```

## Comparing `washpy-0.2.1.tar` & `washpy-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    42028 2024-04-23 21:57:43.954435 washpy-0.2.1/LICENSE
--rw-r--r--   0        0        0     2045 2024-04-23 21:57:43.954435 washpy-0.2.1/README.md
--rw-r--r--   0        0        0      528 2024-04-30 21:23:51.840448 washpy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      315 2024-04-23 21:57:43.991103 washpy-0.2.1/washpy/__init__.py
--rw-r--r--   0        0        0     1086 2024-04-23 21:57:43.987770 washpy-0.2.1/washpy/authenticate.py
--rw-r--r--   0        0        0     3111 2024-04-24 19:26:06.083745 washpy-0.2.1/washpy/device_user.py
--rw-r--r--   0        0        0     1224 2024-04-30 21:21:21.958949 washpy-0.2.1/washpy/pExtended.py
--rw-r--r--   0        0        0      778 2024-04-23 21:57:43.987770 washpy-0.2.1/washpy/post_new_password.py
--rw-r--r--   0        0        0     6158 2024-04-30 21:12:46.347166 washpy-0.2.1/washpy/state.py
--rw-r--r--   0        0        0     3453 2024-04-23 21:57:43.987770 washpy-0.2.1/washpy/status.py
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 washpy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    42028 2024-04-23 21:57:43.954435 washpy-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2731 2024-05-01 15:14:30.938342 washpy-0.2.2/README.md
+-rw-r--r--   0        0        0      526 2024-05-09 16:21:35.367515 washpy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      315 2024-04-23 21:57:43.991103 washpy-0.2.2/washpy/__init__.py
+-rw-r--r--   0        0        0     2164 2024-04-30 21:55:27.785903 washpy-0.2.2/washpy/authenticate.py
+-rw-r--r--   0        0        0     3595 2024-04-30 22:11:51.271198 washpy-0.2.2/washpy/device_user.py
+-rw-r--r--   0        0        0     1224 2024-04-30 21:21:21.958949 washpy-0.2.2/washpy/pExtended.py
+-rw-r--r--   0        0        0      778 2024-04-30 22:06:54.530814 washpy-0.2.2/washpy/post_new_password.py
+-rw-r--r--   0        0        0     6158 2024-04-30 21:12:46.347166 washpy-0.2.2/washpy/state.py
+-rw-r--r--   0        0        0     3453 2024-04-23 21:57:43.987770 washpy-0.2.2/washpy/status.py
+-rw-r--r--   0        0        0     3520 1970-01-01 00:00:00.000000 washpy-0.2.2/PKG-INFO
```

### Comparing `washpy-0.2.1/LICENSE` & `washpy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `washpy-0.2.1/README.md` & `washpy-0.2.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 # washpy
 
+[![PyPI](https://img.shields.io/pypi/v/washpy.svg)](https://pypi.org/project/washpy/)
+
 washpy offers a partial implementation of the Miele Professional IP Profile API.
 
 The project focusses on implementing the parts of the API
 for washing machines from Miele Professional.
 
 ## Getting started
 
+## Installation
+
+[washpy is available on PyPI](https://pypi.org/project/washpy/),
+so washpy can be installed via `pip`, [poetry](https://python-poetry.org/), 
+or any other tool that interfaces with PyPI.
+
 ### Hardware setup
 
 I have tested this library on Miele Professional PWM 507 machines,
 with the Miele XKM 3200-WL-PLT KOM module.
 
 - slide the KOM module into the slot of your machine
 - connect the RJ45 jack of the module to your network
@@ -46,27 +54,44 @@
 postNewPassword("https://192.168.1.251/Devices/000116343328", "Admin", "", "verySecurePassword!")
 ```
 
 #### Add new Account
 
 TODO
 
+#### Interact with a device
+
+The core of washpy is the `DeviceUser` class. Once constructed,
+it provides many methods to control the Miele device.
+
+The script
+```python
+from washpy import DeviceUser
+
+my_device = DeviceUser("https://192.168.1.251/Devices/000116343328", "Admin", "", "verySecurePassword!")
+
+print(my_device.get_State().Status)
+```
+will yield
+```python
+<Status.RUNNING: 5>
+```
 
 ## Is there documentation of the IP Profile API?
 
 Yes, you have to request access to it from [Miele Professional](https://www.miele.com/en/com/index-pro.htm).
 
 ## known issues
 
-do not upgrade requests, as it will upgrade to urllib3 version 2.x
+Do not upgrade requests, as it will upgrade to urllib3 version `2.x`.
 
-problem: you will get handshake errors:
+Problem: you will get handshake errors:
 
 ```python
 SSLError(SSLError(1, '[SSL: SSLV3_ALERT_HANDSHAKE_FAILURE] ssl/tls alert handshake failure (_ssl.c:1006)'))
 ```
 
-also see this [Github Issue](https://github.com/urllib3/urllib3/pull/3060#issuecomment-1578815249).
+Also see this [GitHub Issue](https://github.com/urllib3/urllib3/pull/3060#issuecomment-1578815249).
 
 ## License
 
 [LGPL-3.0-only](LICENSE)
```

### Comparing `washpy-0.2.1/pyproject.toml` & `washpy-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "washpy"
-version = "0.2.1"
+version = "0.2.2"
 description = "A partial implementation of the Miele Professional IP Profile API"
 authors = ["Johann Carl Meyer <info@johannc.de>"]
 license = "LGPL-3.0-only"
 readme = "README.md"
-repository = "https://codeberg.org/johann.carl/washpy"
+repository = "https://codeberg.org/johann-cm/washpy"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "2.29.0"
 isodate = "^0.6.1"
 pydantic = "^2.7.1"
```

### Comparing `washpy-0.2.1/washpy/device_user.py` & `washpy-0.2.2/washpy/device_user.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 from typing import Any, Dict, Final, Optional, Union
 import requests
 
 import datetime
 import isodate
 
 from washpy.authenticate import authenticate
+from washpy.post_new_password import post_new_password
 from washpy.state import State
 from washpy.status import *
 
 
 class DeviceUser:
     """
     device_url: e.g. 'https://192.168.1.251/Devices/000116343328'
 
     token: a bearer-token, used for authenticating a user with a device at every other XKM API endpoint
     """
 
-    device_url: str
+    device_url: Final[str]
     user: Final[str]
-    password: Final[str]
+    password: str
     token: str
     timeout: datetime.timedelta
     last_used: datetime.datetime
 
     def __init__(self, device_url: str, user: str, password: str) -> None:
         """
         device_url: e.g. 'https://192.168.1.251/Devices/000116343328'
 
         user: a username
 
         password: the password of user
 
         Authenticates the user at the specified machine
+
+        raises: see `washpy.authenticate`
         """
         self.user = user
         self.password = password
         self.device_url = device_url
         self.last_used = datetime.datetime.now()
         (self.token, self.timeout) = authenticate(
             self.device_url, self.user, self.password
@@ -77,24 +80,36 @@
     def refresh_authentication(self) -> datetime.datetime:
         """
         if self.token is only valid for less then 10 seconds
         or if it is invalid,
         refresh it.
 
         returns: the point in time at which the check has happened
+
+        raises: see `washpy.authenticate`
         """
         now = datetime.datetime.now()
         token_valid_date = self.last_used + self.timeout
         if now > token_valid_date - datetime.timedelta(seconds=10):
             (self.token, self.timeout) = authenticate(
                 self.device_url, self.user, self.password
             )
             self.last_used = now
         return now
 
+    def post_new_password(self, new_password):
+        """
+        a wrapper around `washpy.post_new_password`.
+
+        Changes the password and refreshes authentication.
+        """
+        post_new_password(self.device_url, self.user, self.password, new_password)
+        self.password = new_password
+        self.refresh_authentication()
+
     def get_State(self) -> State:
         """
         queries the `/State` endpoint.
 
         returns: a complete state of the machine
 
         raises: ValueError, if the authentication was unsuccessfull
```

### Comparing `washpy-0.2.1/washpy/pExtended.py` & `washpy-0.2.2/washpy/pExtended.py`

 * *Files identical despite different names*

### Comparing `washpy-0.2.1/washpy/post_new_password.py` & `washpy-0.2.2/washpy/post_new_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,9 +20,9 @@
         {"LoginName": user, "Password": password_old, "PasswordNew": password_new}
     )
     headers = {"Content-Type": "application/json"}
 
     response = requests.request(
         "POST", device_url, headers=headers, data=payload, verify=False
     )
-    if response.status_code != 200:
+    if response.status_code != 204:
         raise ValueError(f"something went wrong: got HTTP response {response}")
```

### Comparing `washpy-0.2.1/washpy/state.py` & `washpy-0.2.2/washpy/state.py`

 * *Files identical despite different names*

### Comparing `washpy-0.2.1/washpy/status.py` & `washpy-0.2.2/washpy/status.py`

 * *Files identical despite different names*

### Comparing `washpy-0.2.1/PKG-INFO` & `washpy-0.2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 Metadata-Version: 2.1
 Name: washpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A partial implementation of the Miele Professional IP Profile API
-Home-page: https://codeberg.org/johann.carl/washpy
+Home-page: https://codeberg.org/johann-cm/washpy
 License: LGPL-3.0-only
 Author: Johann Carl Meyer
 Author-email: info@johannc.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: requests (==2.29.0)
-Project-URL: Repository, https://codeberg.org/johann.carl/washpy
+Project-URL: Repository, https://codeberg.org/johann-cm/washpy
 Description-Content-Type: text/markdown
 
 # washpy
 
+[![PyPI](https://img.shields.io/pypi/v/washpy.svg)](https://pypi.org/project/washpy/)
+
 washpy offers a partial implementation of the Miele Professional IP Profile API.
 
 The project focusses on implementing the parts of the API
 for washing machines from Miele Professional.
 
 ## Getting started
 
+## Installation
+
+[washpy is available on PyPI](https://pypi.org/project/washpy/),
+so washpy can be installed via `pip`, [poetry](https://python-poetry.org/), 
+or any other tool that interfaces with PyPI.
+
 ### Hardware setup
 
 I have tested this library on Miele Professional PWM 507 machines,
 with the Miele XKM 3200-WL-PLT KOM module.
 
 - slide the KOM module into the slot of your machine
 - connect the RJ45 jack of the module to your network
@@ -66,28 +74,45 @@
 postNewPassword("https://192.168.1.251/Devices/000116343328", "Admin", "", "verySecurePassword!")
 ```
 
 #### Add new Account
 
 TODO
 
+#### Interact with a device
+
+The core of washpy is the `DeviceUser` class. Once constructed,
+it provides many methods to control the Miele device.
+
+The script
+```python
+from washpy import DeviceUser
+
+my_device = DeviceUser("https://192.168.1.251/Devices/000116343328", "Admin", "", "verySecurePassword!")
+
+print(my_device.get_State().Status)
+```
+will yield
+```python
+<Status.RUNNING: 5>
+```
 
 ## Is there documentation of the IP Profile API?
 
 Yes, you have to request access to it from [Miele Professional](https://www.miele.com/en/com/index-pro.htm).
 
 ## known issues
 
-do not upgrade requests, as it will upgrade to urllib3 version 2.x
+Do not upgrade requests, as it will upgrade to urllib3 version `2.x`.
 
-problem: you will get handshake errors:
+Problem: you will get handshake errors:
 
 ```python
 SSLError(SSLError(1, '[SSL: SSLV3_ALERT_HANDSHAKE_FAILURE] ssl/tls alert handshake failure (_ssl.c:1006)'))
 ```
 
-also see this [Github Issue](https://github.com/urllib3/urllib3/pull/3060#issuecomment-1578815249).
+Also see this [GitHub Issue](https://github.com/urllib3/urllib3/pull/3060#issuecomment-1578815249).
 
 ## License
 
 [LGPL-3.0-only](LICENSE)
```

