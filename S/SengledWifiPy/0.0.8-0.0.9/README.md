# Comparing `tmp/sengledwifipy-0.0.8.tar.gz` & `tmp/sengledwifipy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sengledwifipy-0.0.8.tar", max compression
+gzip compressed data, was "sengledwifipy-0.0.9.tar", max compression
```

## Comparing `sengledwifipy-0.0.8.tar` & `sengledwifipy-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-04-23 22:58:58.395581 sengledwifipy-0.0.8/LICENSE
--rw-r--r--   0        0        0     3333 2024-04-23 22:58:58.395581 sengledwifipy-0.0.8/README.md
--rw-r--r--   0        0        0     2847 2024-04-23 22:59:20.007888 sengledwifipy-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      228 2024-04-23 22:58:58.395581 sengledwifipy-0.0.8/sengledwifipy/__init__.py
--rw-r--r--   0        0        0      717 2024-04-23 22:58:58.395581 sengledwifipy-0.0.8/sengledwifipy/const.py
--rw-r--r--   0        0        0      662 2024-04-23 22:58:58.395581 sengledwifipy-0.0.8/sengledwifipy/errors.py
--rw-r--r--   0        0        0     6497 2024-04-23 22:58:58.395581 sengledwifipy-0.0.8/sengledwifipy/helpers.py
--rw-r--r--   0        0        0     7395 2024-04-23 22:58:58.395581 sengledwifipy-0.0.8/sengledwifipy/sengledwifiapi.py
--rw-r--r--   0        0        0    11716 2024-04-23 22:58:58.395581 sengledwifipy-0.0.8/sengledwifipy/sengledwifilogin.py
--rw-r--r--   0        0        0    12106 2024-04-23 22:58:58.395581 sengledwifipy-0.0.8/sengledwifipy/sengledwifimqtt.py
--rw-r--r--   0        0        0     4233 1970-01-01 00:00:00.000000 sengledwifipy-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-08 22:20:28.581283 sengledwifipy-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3333 2024-05-08 22:20:28.581283 sengledwifipy-0.0.9/README.md
+-rw-r--r--   0        0        0     2816 2024-05-08 22:20:45.273487 sengledwifipy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      228 2024-05-08 22:20:28.585283 sengledwifipy-0.0.9/sengledwifipy/__init__.py
+-rw-r--r--   0        0        0      717 2024-05-08 22:20:28.585283 sengledwifipy-0.0.9/sengledwifipy/const.py
+-rw-r--r--   0        0        0      662 2024-05-08 22:20:28.585283 sengledwifipy-0.0.9/sengledwifipy/errors.py
+-rw-r--r--   0        0        0     6665 2024-05-08 22:20:28.585283 sengledwifipy-0.0.9/sengledwifipy/helpers.py
+-rw-r--r--   0        0        0     6626 2024-05-08 22:20:28.585283 sengledwifipy-0.0.9/sengledwifipy/sengledwifiapi.py
+-rw-r--r--   0        0        0    11438 2024-05-08 22:20:28.585283 sengledwifipy-0.0.9/sengledwifipy/sengledwifilogin.py
+-rw-r--r--   0        0        0    11766 2024-05-08 22:20:28.585283 sengledwifipy-0.0.9/sengledwifipy/sengledwifimqtt.py
+-rw-r--r--   0        0        0     4147 1970-01-01 00:00:00.000000 sengledwifipy-0.0.9/PKG-INFO
```

### Comparing `sengledwifipy-0.0.8/LICENSE` & `sengledwifipy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.8/README.md` & `sengledwifipy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.8/pyproject.toml` & `sengledwifipy-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "SengledWifiPy"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python package to control Sengled Wifi Devices Programmatically."
 authors = [
   "Cesar <gv4plolxe@mozmail.com>"
 ]
 license = "Apache-2.0"
 readme = 'README.md'
 repository = "https://github.com/cpadil/sengledwifipy"
@@ -16,21 +16,18 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = ">=3.11, <4"
 aiofiles = "^23.2.1"
-simplejson = "*"
 yarl = "*"
-certifi = "*"
 backoff = ">=2.2.1"
 aiohttp = "^3.9.4"
 paho-mqtt = "^2.0.0"
-ruff = "^0.3.7"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "*"
 pytest-aiohttp = "*"
 pytest-cov = "*"
 python-semantic-release = "^9.4.2"
 safety = ">=1.8.7"
@@ -38,14 +35,15 @@
 tomlkit = ">=0.7.0"
 sphinx-autoapi = ">=1.7.0"
 myst-parser = "^2.0.0"
 furo = "^2024.1.29"
 pre-commit = "^3.7.0"
 commitizen = "^3.24.0"
 pre-commit-hooks = "^4.6.0"
+ruff = "^0.4.1"
 
 [tool.ruff]
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
```

### Comparing `sengledwifipy-0.0.8/sengledwifipy/const.py` & `sengledwifipy-0.0.9/sengledwifipy/const.py`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.8/sengledwifipy/errors.py` & `sengledwifipy-0.0.9/sengledwifipy/errors.py`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.8/sengledwifipy/helpers.py` & `sengledwifipy-0.0.9/sengledwifipy/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from aiohttp import ClientConnectionError, ContentTypeError, ServerDisconnectedError
 
 from .const import EXCEPTION_TEMPLATE
 from .errors import (
     SengledWifipyConnectionError,
     SengledWifipyLoginCloseRequested,
     SengledWifipyLoginError,
+    SengledWifipyTooManyRequestsError,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def hide_email(email: str) -> str:
     """Obfuscate email."""
@@ -116,57 +117,47 @@
 def catch_all_exceptions(func):  # noqa: D103
     @functools.wraps(func)
     async def wrapper(*args, **kwargs):
         try:
             return await func(*args, **kwargs)
         except (ClientConnectionError, KeyError, ServerDisconnectedError) as ex:
             _LOGGER.warning(
-                "%s.%s(%s, %s): A connection error occurred: %s",
+                "SengledWifi %s.%s(%s, %s): A connection error occurred: %s",
                 func.__module__[func.__module__.find(".") + 1 :],
                 func.__name__,
                 obfuscate(args),
                 obfuscate(kwargs),
                 EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args),
             )
             raise SengledWifipyConnectionError from ex
-        except (JSONDecodeError, CookieError) as ex:
+        except (JSONDecodeError, CookieError, ContentTypeError) as ex:
             _LOGGER.warning(
-                "%s.%s(%s, %s): A login error occurred: %s",
-                func.__module__[func.__module__.find(".") + 1 :],
-                func.__name__,
-                obfuscate(args),
-                obfuscate(kwargs),
-                EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args),
-            )
-            raise SengledWifipyLoginError from ex
-        except ContentTypeError as ex:
-            _LOGGER.warning(
-                "%s.%s(%s, %s): A login error occurred: %s",
+                "SengledWifi %s.%s(%s, %s): A error occurred while calling an api: %s",
                 func.__module__[func.__module__.find(".") + 1 :],
                 func.__name__,
                 obfuscate(args),
                 obfuscate(kwargs),
                 EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args),
             )
             raise SengledWifipyLoginError from ex
         except CancelledError as ex:
             _LOGGER.warning(
-                "%s.%s(%s, %s): Timeout error occurred accessing SengledWifiAPI: %s",
+                "SengledWifi %s.%s(%s, %s): Timeout error occurred accessing SengledWifiAPI: %s",
                 func.__module__[func.__module__.find(".") + 1 :],
                 func.__name__,
                 obfuscate(args),
                 obfuscate(kwargs),
                 EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args),
             )
             return None
         except SengledWifipyLoginCloseRequested:
             raise
         except Exception as ex:
             _LOGGER.warning(
-                "%s.%s(%s, %s): An error occurred accessing SengledWifiAPI: %s",
+                "SengledWifi %s.%s(%s, %s): An error occurred accessing SengledWifiAPI: %s",
                 func.__module__[func.__module__.find(".") + 1 :],
                 func.__name__,
                 obfuscate(args),
                 obfuscate(kwargs),
                 EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args),
             )
             raise
@@ -182,7 +173,23 @@
         )
 
         if not await login.valid_login():
             await login.login(SkipTest=True)
         return await func(*args, **kwargs)
 
     return wrapper
+
+
+async def valid_response(response) -> None:
+    """Response validation for aiohttp request.
+
+    Args:
+        response (ClientResponse): response from aiohttp request
+    Returns:
+        None
+    """
+    if response.status == 401:
+        raise SengledWifipyLoginError(response.reason)
+    if response.status == 429:
+        raise SengledWifipyTooManyRequestsError(response.reason)
+    if response.status >= 400:
+        raise SengledWifipyConnectionError(response.reason)
```

### Comparing `sengledwifipy-0.0.8/sengledwifipy/sengledwifiapi.py` & `sengledwifipy-0.0.9/sengledwifipy/sengledwifiapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,44 +9,44 @@
 
 import backoff
 from aiohttp import ClientConnectionError, ClientResponse
 from yarl import URL
 
 from .errors import (
     SengledWifipyConnectionError,
-    SengledWifipyLoginCloseRequested,
-    SengledWifipyLoginError,
     SengledWifipyTooManyRequestsError,
 )
 
 if TYPE_CHECKING:
     from .sengledwifilogin import SengledLogin
     from .sengledwifimqtt import SengledWifiMQTT
 
 
-from .helpers import catch_all_exceptions, hide_email, valid_login_required
+from .helpers import (
+    catch_all_exceptions,
+    hide_email,
+    valid_login_required,
+)
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class SengledWifiAPI:
     """Uses SengledWifiMqtt and SengledLogin to get information of the devices and set their state.
 
     Attributes:
         login (SengledLogin):  SengledLogin object
-        session (aiohttp ClientSession): Session attribute of login
     """
 
     devices: dict[str, Any] = {}
     """Class attribute. Saves the devices registered in the related Sengled account."""
 
-    def __init__(self, login: SengledLogin):
+    def __init__(self, login: SengledLogin) -> None:
         """Initialize Sengled Wifi device."""
         self._login = login
-        self._session = login.session
 
     @staticmethod
     @backoff.on_exception(
         backoff.expo,
         (SengledWifipyTooManyRequestsError, SengledWifipyConnectionError, ClientConnectionError),
         max_time=60,
         max_tries=5,
@@ -67,37 +67,22 @@
             uri (str): will use the appserver endpoint with this uri
             data (dict[str, str]): payload
             query (dict[str, str]): query parameters
 
         Returns:
             None or aiohttp ClientResponse
         """
-        session = login.session
-        url: URL = URL(login.urls["appserver"] + uri).update_query(query)
+        url = URL(login.urls["appserver"] + uri).update_query(query)
 
-        response = await getattr(session, method)(
-            url,
-            json=data,
-            headers=login._headers,
-            ssl=login._ssl,
-        )
+        response = await getattr(login.session, method)(url, json=data)
 
         _LOGGER.debug(f"SengledWifiApi: API {hide_email(login.email)}: \
                       \n--static {response.request_info.method}: {response.request_info.url} \
                       \n--returned {response.status}:{response.reason}:{response.content_type}")
 
-        login.stats["api_calls"] += 1
-        if response.status == 401:
-            login.status["login_successful"] = False
-            raise SengledWifipyLoginError(response.reason)
-        if response.status == 429:
-            raise SengledWifipyTooManyRequestsError(response.reason)
-        if response.status >= 400:
-            _LOGGER.debug(f"SengledWifiApi: API Returning None due to status: {response.status}")
-            return None
         return response
 
     @staticmethod
     @catch_all_exceptions
     async def get_devices(
         login: SengledLogin,
         entity_ids: list[str] = None,
@@ -112,16 +97,14 @@
         Returns:
             Json. Device information.
         """
         response = await SengledWifiAPI._static_request(
             "post",
             login,
             "device/list.json",
-            query=None,
-            data={},
         )
 
         SengledWifiAPI.devices[login.email] = (
             [
                 item
                 for item in (await response.json(content_type=None))["deviceList"]
                 if (item["category"] == "wifielement" and (entity_ids is None or item["deviceUuid"] in entity_ids))
```

### Comparing `sengledwifipy-0.0.8/sengledwifipy/sengledwifilogin.py` & `sengledwifipy-0.0.9/sengledwifipy/sengledwifilogin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """Python Package for controlling Sengled Wifi devices. SPDX-License-Identifier: Apache-2.0."""
 
 import logging
 import os as oos
-import ssl
 from datetime import datetime
-from json import JSONDecodeError, dumps
+from json import dumps
 from typing import Callable
 from uuid import uuid4
 
-import certifi
 from aiofiles import os
-from aiohttp import ClientSession, ContentTypeError, CookieJar
-from simplejson import JSONDecodeError as SimpleJSONDecodeError
+from aiohttp import ClientResponse, ClientSession, CookieJar
+from yarl import URL
 
 from .const import EXCEPTION_TEMPLATE, HA_DOMAIN, SENGLED_ENDPOINTS, USER_AGENT
-from .errors import SengledWifipyLoginError
+from .errors import (
+    SengledWifipyLoginError,
+)
 from .helpers import (
     catch_all_exceptions,
     hide_email,
     obfuscate,
+    valid_response,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class SengledLogin:
     """Handle login connection to Sengled.
 
     Attributes:
         _email (string): Sengled login account
         _password (string): Password for Sengled login account
         _outputpath (function): os.path.join function pointing to the folder to save a session cookie
-        _uuid: (string): Unique 32 char hex to serve as app serial number for registration
         _urls(dict[str, str]): points to the constant SENGLED_ENDPOINTS which is an initial list of Sengled endpoints
         _session (aiohttp.ClientSession): initializes an empty aiohttp.ClientSession to store the cookie information
         _ssl (ssl): used during the authentication
         _headers (dict[str, str]): based on USER_AGENT constant
         status (dict[str, str | bool]): track if the connection is still valid
         stats (dict[str, str | bool]): track number of api calls done
         _cookiefile (str): in combination with _outputpath, provides the path to save the cookie
@@ -62,34 +62,31 @@
             uuid: (string): Unique 32 char hex to serve as app serial number for registration
 
         """
         self._urls: dict[str, str] = SENGLED_ENDPOINTS
         self._email: str = email
         self._password: str = password
         self._session: ClientSession = None
-        self._ssl = ssl.create_default_context(purpose=ssl.Purpose.SERVER_AUTH, cafile=certifi.where())
         self._headers: dict[str, str] = {}
         self.status: dict[str, str | bool] = {}
         self.stats: dict[str, str | bool] = {
             "login_timestamp": datetime(1, 1, 1),
             "api_calls": 0,
         }
         self._outputpath = outputpath if outputpath is not None else (lambda b: oos.path.join("temp", b))
         self._cookiefile: str = self._outputpath(f".storage/{type(self).hass_domain}.{self.email}.pickle")
         self._customer_id: str = None
-        self._uuid = uuid if uuid else uuid4().hex.upper()
         self._data = {
             "user": self._email,
             "pwd": self._password,
-            "uuid": self._uuid,
+            "uuid": uuid if uuid else uuid4().hex.upper(),
             "osType": "android",
             "productCode": "life",
             "appCode": "life",
         }
-
         self._create_session()
 
     @property
     def urls(self) -> str:
         """SENGLED_ENDPOINTS plus the endpoints provided by _get_server_info."""
         return self._urls
 
@@ -109,23 +106,21 @@
         return self._session
 
     def _create_session(self) -> None:
         """Create an aiohttp session. Called during the initialization."""
         _LOGGER.debug("SengledWifiApi: LOGIN Creating session")
 
         if not self._session:
-            #  define session headers
             self._headers = {
                 "User-Agent": USER_AGENT,
                 "Accept": "*/*",
                 "Accept-Language": "*",
                 "Content-Type": "application/json",
             }
-            #  initiate session
-            self._session = ClientSession(headers=self._headers)
+            self._session = ClientSession(headers=self._headers, raise_for_status=valid_response)
 
     async def valid_login(self) -> bool:
         """Function that will test the connection is logged in.
 
         Args:
             None
         Returns:
@@ -134,37 +129,25 @@
         """
         _LOGGER.debug(f'SengledWifiApi: LOGIN validation of session \
                       \n--URL {self._urls["validSession"]}  \
                       \n--Headers {dumps(self._headers)} \
                       \n--last login: {self.stats["login_timestamp"]} \
                       \n--hours: {round((datetime.now() - self.stats["login_timestamp"]).total_seconds()/3600)}h ')
         if (datetime.now() - self.stats["login_timestamp"]).total_seconds() < 86400 and await os.path.exists(self._cookiefile):
-            resp = None
-
             if len(self._session.cookie_jar) == 0:
                 self._session.cookie_jar.load(self._cookiefile)
 
             _LOGGER.debug("SengledWifiApi: LOGIN calling validation api")
-            resp = await self._session.post(
-                self._urls["validSession"],
-                json={},
-                ssl=self._ssl,
-            )
-
-            try:
-                resp = await resp.json()
-            except (JSONDecodeError, SimpleJSONDecodeError, ContentTypeError) as ex:
-                _LOGGER.debug(f"SengledWifiApi: LOGIN Error during login validation: \
-                              \n--{EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args)}")
+            resp = await self._static_request("post", url=self._urls["validSession"], data={})
+            resp = await resp.json()
 
             if resp and int(resp.get("messageCode")) == 200:
                 _LOGGER.debug("SengledWifiApi: LOGIN login validation with cookie successful")
-                self.stats["api_calls"] += 1
                 return True
-            _LOGGER.debug(f"SengledWifiApi: LOGIN validation api problem: {resp}")
+            _LOGGER.debug(f"SengledWifiApi: LOGIN validation api response not successful: {resp}")
         _LOGGER.debug("SengledWifiApi: LOGIN login not valid, either the login is old >24h or cookie is not valid")
 
         await self.reset()
         return False
 
     @catch_all_exceptions
     async def login(self, SkipTest: bool = False) -> None:
@@ -178,33 +161,26 @@
         """
         if not SkipTest:
             if await self.valid_login():
                 return
 
         _LOGGER.debug("SengledWifiApi: LOGIN Using credentials to login")
 
-        post_resp = await self._session.post(
-            self._urls["login"],
-            json=self._data,
-            headers=self._headers,
-            ssl=self._ssl,
-        )
+        post_resp = await self._static_request("post", url=self._urls["login"], data=self._data)
         post_resp = await post_resp.json()
 
-        if post_resp:
-            if int(post_resp.get("ret")) == 0:
-                _LOGGER.debug(f"SengledWifiApi: LOGIN Login successful for {hide_email(self._email)}; saving cookie")
-                self._customer_id = post_resp.get("customerId")
-                self.status["login_successful"] = True
-                self.stats["login_timestamp"] = datetime.now()
-                self.stats["api_calls"] += 1
-                await self.save_cookiefile()
-                await self._get_server_info()
-                return
-            _LOGGER.debug(f"SengledWifiApi: LOGIN Login not possible for {hide_email(self._email)}")
+        if post_resp and int(post_resp.get("ret")) == 0:
+            _LOGGER.debug(f"SengledWifiApi: LOGIN Login successful for {hide_email(self._email)}; saving cookie")
+            self._customer_id = post_resp.get("customerId")
+            self.status["login_successful"] = True
+            self.stats["login_timestamp"] = datetime.now()
+            await self.save_cookiefile()
+            await self._get_server_info()
+            return
+        _LOGGER.debug(f"SengledWifiApi: LOGIN Login not possible for {hide_email(self._email)}")
 
     async def save_cookiefile(self) -> None:
         """Save login session cookie to file."""
         cookie_jar = self._session.cookie_jar
         assert isinstance(cookie_jar, CookieJar)
 
         _LOGGER.debug(f'SengledWifiApi: LOGIN Saving cookie to {self._cookiefile.split("/")[0]}')
@@ -213,41 +189,61 @@
             cookie_jar.save(self._cookiefile)
         except (OSError, EOFError, TypeError, AttributeError) as ex:
             _LOGGER.debug(f'SengledWifiApi: LOGIN Error saving pickled cookie to {self._cookiefile.split("/")[0]} .... \
                           \n--{EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args)}')
             raise SengledWifipyLoginError
 
         _LOGGER.debug(f"SengledWifiApi: LOGIN Saved session Cookies: \
-                      \n--{self._print_session_cookies()}")
+                      \n--{await self._print_session_cookies()}")
 
-    def _print_session_cookies(self) -> str:
+    async def _print_session_cookies(self) -> str:
         """Prints the value of the cookies in aiohttp session."""
         result: str = ""
         if not self._session.cookie_jar:
             result = "Session cookie jar is empty."
         for cookie in self._session.cookie_jar:
             result += f"{obfuscate(cookie)}"
         return result
 
+    async def _static_request(
+        self,
+        method: str,
+        url: str,
+        data: dict[str, str] = None,
+        query: dict[str, str] = None,
+    ) -> ClientResponse:
+        """Call an API.
+
+        Args:
+            login (SengledLogin): needs a valid login
+            uri (str): will use the appserver endpoint with this uri
+            data (dict[str, str]): payload
+            query (dict[str, str]): query parameters
+
+        Returns:
+            None or aiohttp ClientResponse
+        """
+        url = URL(url).update_query(query)
+
+        response = await getattr(self._session, method)(url, json=data)
+
+        _LOGGER.debug(f"SengledWifiApi: LOGIN API CALL {hide_email(self._email)}: \
+                      \n--static {response.request_info.method}: {response.request_info.url} \
+                      \n--returned {response.status}:{response.reason}:{response.content_type}")
+
+        self.stats["api_calls"] += 1
+
+        return response
+
     async def _get_server_info(self) -> None:
         """Call to serverDetails endpoint to get Mqtt related endpoints. Called from Login."""
         _LOGGER.debug("SengledWifiApi: LOGIN Getting server endpoints from: %s", self._urls["serverDetails"])
 
-        post_resp = await self._session.post(
-            self._urls["serverDetails"],
-            json={},
-            headers=self._headers,
-            ssl=self._ssl,
-        )
-
-        try:
-            post_resp = await post_resp.json()
-        except (JSONDecodeError, SimpleJSONDecodeError, ContentTypeError) as ex:
-            _LOGGER.debug(f"SengledWifiApi: LOGIN Error during getServerDetails: \
-                          \n--{EXCEPTION_TEMPLATE.format(type(ex).__name__, ex.args)}")
+        post_resp = await self._static_request("post", url=self._urls["serverDetails"])
+        post_resp = await post_resp.json()
 
         if int(post_resp.get("messageCode")) == 200:
             self._urls.update(
                 {
                     "appserver": post_resp.get("appServerAddr"),
                     "mqtt": post_resp.get("inceptionAddr"),
                     "mqttport": post_resp.get("mqttSslPort"),
```

### Comparing `sengledwifipy-0.0.8/sengledwifipy/sengledwifimqtt.py` & `sengledwifipy-0.0.9/sengledwifipy/sengledwifimqtt.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,20 +20,17 @@
 
 
 class SengledWifiMQTT:
     """Connect to Sengled MQTT broker, subscribe to topics and publish updates. Uses paho-mqtt package.
 
     Attributes:
         _login (SengledLogin): SengledLogin object
-        _session (SengledLogin session): SengledLogin session attribute
         _jsession_id (SengledLogin session JSESSIONID): value of cookie JSESSIONID saved in SengledLogin session
-        _headers (dict[str, str]): same headers used in Android app
-        _clientid (str): used during the creation of the mqtt client f"{_jsession_id}@lifeApp"
         mqtt_server (URL): url is obtained during the login and fetched from SengledLogin object
-        mqtt_client (paho.mqtt.client): initialization of paho.mqtt client
+        mqtt_client (paho.mqtt.client): initialization of paho.mqtt client with same headers used in Android app
         _status (bool): to indicate if mqtt connection is active
         devices (list[dict[str, str]]): list of Sengled devices, used to create the topic strings and subscribe, \
             during the initialization is set to None
         open_callback (Callable): an async function to call within the on_connect callback
         msg_callback (Callable): an async function to call within the on_message callback
         close_callback (Callable): an async function to call within the on_disconnect callback
         error_callback (Callable): an async function to call within the on_error callback
@@ -56,39 +53,35 @@
             msg_callback (Callable): callback function when new messages arrive.
             open_callback (Callable): callback function when connection is opened.
             close_callback (Callable): callback function when when the connection is closed.
             error_callback (Callable): callback function when there is an error.
             loop: (asyncio.AbstractEventLoop).
         """
         self._login = login
-        self._session = login.session
-        self._jsession_id = self._session.cookie_jar.filter_cookies("https://sengled.com")["JSESSIONID"].value
-        self._headers = {
-            "Cookie": f"JSESSIONID={self._jsession_id}",
-            "X-Requested-With": "com.sengled.life2",
-        }
-        self._clientid = f"{self._jsession_id}@lifeApp"
-        self.mqtt_server = URL(login.urls["mqtt"])
-        self.mqtt_client: mqtt.Client = None
+        self._jsession_id = self._login.session.cookie_jar.filter_cookies("https://sengled.com")["JSESSIONID"].value
         self._status: bool = False
         self.devices: dict = None
         self.open_callback: Callable[[], Coroutine[Any, Any, None]] = open_callback
         self.msg_callback: Callable[[], Coroutine[Any, Any, None]] = msg_callback
         self.close_callback: Callable[[], Coroutine[Any, Any, None]] = close_callback
         self.error_callback: Callable[[str], Coroutine[Any, Any, None]] = error_callback
         self._loop: asyncio.AbstractEventLoop = loop if loop else asyncio.get_event_loop()
+        self.mqtt_server = URL(login.urls["mqtt"])
         self.mqtt_client = mqtt.Client(
             callback_api_version=mqttenums.CallbackAPIVersion.VERSION2,
-            client_id=self._clientid,
+            client_id=f"{self._jsession_id}@lifeApp",
             transport="websockets",
         )
         self.mqtt_client.tls_set_context()
         self.mqtt_client.ws_set_options(
             path=self.mqtt_server.path,
-            headers=self._headers,
+            headers={
+                "Cookie": f"JSESSIONID={self._jsession_id}",
+                "X-Requested-With": "com.sengled.life2",
+            },
         )
         self.mqtt_client.on_message = self.on_message
         self.mqtt_client.on_connect = self.on_connect
         self.mqtt_client.on_disconnect = self.on_disconnect
         self.mqtt_client.on_subscribe = self.on_subscribe
         self.mqtt_client.on_log = self.on_log
```

### Comparing `sengledwifipy-0.0.8/PKG-INFO` & `sengledwifipy-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: SengledWifiPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package to control Sengled Wifi Devices Programmatically.
 Home-page: https://github.com/cpadil/sengledwifipy
 License: Apache-2.0
 Keywords: Sengled,Wifi,homeassistant
 Author: Cesar
 Author-email: gv4plolxe@mozmail.com
 Requires-Python: >=3.11,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: backoff (>=2.2.1)
-Requires-Dist: certifi
 Requires-Dist: paho-mqtt (>=2.0.0,<3.0.0)
-Requires-Dist: ruff (>=0.3.7,<0.4.0)
-Requires-Dist: simplejson
 Requires-Dist: yarl
 Project-URL: Repository, https://github.com/cpadil/sengledwifipy
 Description-Content-Type: text/markdown
 
 # SengledWifiPy
 
 [![License][license-badge]][license]
```

