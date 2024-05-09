# Comparing `tmp/uiautodev-0.3.3.tar.gz` & `tmp/uiautodev-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiautodev-0.3.3.tar", max compression
+gzip compressed data, was "uiautodev-0.3.4.tar", max compression
```

## Comparing `uiautodev-0.3.3.tar` & `uiautodev-0.3.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1068 2024-02-18 02:48:04.400793 uiautodev-0.3.3/LICENSE
--rw-r--r--   0        0        0      586 2024-05-07 01:56:02.660382 uiautodev-0.3.3/README.md
--rw-r--r--   0        0        0     1136 2024-05-07 01:58:19.693419 uiautodev-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      267 2024-05-07 01:43:00.885006 uiautodev-0.3.3/uiautodev/__init__.py
--rw-r--r--   0        0        0      176 2024-05-07 01:35:26.228901 uiautodev-0.3.3/uiautodev/__main__.py
--rw-r--r--   0        0        0     2395 2024-05-07 01:44:03.045601 uiautodev-0.3.3/uiautodev/app.py
--rw-r--r--   0        0        0     1773 2024-04-11 04:49:41.915552 uiautodev-0.3.3/uiautodev/appium_proxy.py
--rw-r--r--   0        0        0     3919 2024-05-07 01:35:30.307901 uiautodev-0.3.3/uiautodev/case.py
--rw-r--r--   0        0        0     5405 2024-05-07 01:43:33.260959 uiautodev-0.3.3/uiautodev/cli.py
--rw-r--r--   0        0        0     4562 2024-05-07 01:35:30.307668 uiautodev-0.3.3/uiautodev/command_proxy.py
--rw-r--r--   0        0        0     1587 2024-05-07 01:35:30.294847 uiautodev-0.3.3/uiautodev/command_types.py
--rw-r--r--   0        0        0     7596 2024-05-07 01:41:44.330833 uiautodev-0.3.3/uiautodev/driver/android.py
--rw-r--r--   0        0        0     5308 2024-05-07 01:35:30.288946 uiautodev-0.3.3/uiautodev/driver/appium.py
--rw-r--r--   0        0        0     2048 2024-05-07 01:35:30.289562 uiautodev-0.3.3/uiautodev/driver/base_driver.py
--rw-r--r--   0        0        0     4353 2024-05-07 01:35:30.288349 uiautodev-0.3.3/uiautodev/driver/ios.py
--rw-r--r--   0        0        0     2422 2024-05-07 01:35:30.284010 uiautodev-0.3.3/uiautodev/driver/mock.py
--rw-r--r--   0        0        0  3675062 2024-04-23 14:24:03.590749 uiautodev-0.3.3/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk
--rw-r--r--   0        0        0     8351 2024-05-07 01:45:38.094224 uiautodev-0.3.3/uiautodev/driver/udt/udt.py
--rw-r--r--   0        0        0      465 2024-04-23 15:41:21.463678 uiautodev-0.3.3/uiautodev/exceptions.py
--rw-r--r--   0        0        0      717 2024-04-13 14:55:23.914034 uiautodev-0.3.3/uiautodev/model.py
--rw-r--r--   0        0        0     2370 2024-05-07 01:35:30.294786 uiautodev-0.3.3/uiautodev/provider.py
--rw-r--r--   0        0        0     3862 2024-05-07 01:35:30.283501 uiautodev-0.3.3/uiautodev/router/device.py
--rw-r--r--   0        0        0      891 2024-04-11 04:49:41.918406 uiautodev-0.3.3/uiautodev/router/xml.py
--rw-r--r--   0        0        0     1240 2024-04-11 04:49:41.918609 uiautodev-0.3.3/uiautodev/static/demo.html
--rw-r--r--   0        0        0     4785 2024-05-07 01:35:30.283086 uiautodev-0.3.3/uiautodev/utils/common.py
--rw-r--r--   0        0        0      637 2024-05-07 01:35:30.280280 uiautodev-0.3.3/uiautodev/utils/exceptions.py
--rw-r--r--   0        0        0    17386 2024-05-07 01:35:30.283490 uiautodev-0.3.3/uiautodev/utils/usbmux.py
--rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 uiautodev-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-09 03:46:25.038415 uiautodev-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1191 2024-05-09 03:46:25.038415 uiautodev-0.3.4/README.md
+-rw-r--r--   0        0        0     1091 2024-05-09 03:46:38.174371 uiautodev-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      267 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/__main__.py
+-rw-r--r--   0        0        0     2491 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/app.py
+-rw-r--r--   0        0        0     1773 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/appium_proxy.py
+-rw-r--r--   0        0        0     3919 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/case.py
+-rw-r--r--   0        0        0     6234 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/cli.py
+-rw-r--r--   0        0        0     4562 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/command_proxy.py
+-rw-r--r--   0        0        0     1587 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/command_types.py
+-rw-r--r--   0        0        0      534 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/common.py
+-rw-r--r--   0        0        0     7043 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/driver/android.py
+-rw-r--r--   0        0        0     5308 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/driver/appium.py
+-rw-r--r--   0        0        0     2048 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/driver/base_driver.py
+-rw-r--r--   0        0        0     4353 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/driver/ios.py
+-rw-r--r--   0        0        0     2422 2024-05-09 03:46:25.042415 uiautodev-0.3.4/uiautodev/driver/mock.py
+-rw-r--r--   0        0        0  3675062 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk
+-rw-r--r--   0        0        0     8351 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/driver/udt/udt.py
+-rw-r--r--   0        0        0      465 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/exceptions.py
+-rw-r--r--   0        0        0      717 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/model.py
+-rw-r--r--   0        0        0     2370 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/provider.py
+-rw-r--r--   0        0        0     3862 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/router/device.py
+-rw-r--r--   0        0        0      891 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/router/xml.py
+-rw-r--r--   0        0        0     1240 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/static/demo.html
+-rw-r--r--   0        0        0     4785 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/utils/common.py
+-rw-r--r--   0        0        0      637 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/utils/exceptions.py
+-rw-r--r--   0        0        0    17386 2024-05-09 03:46:25.054415 uiautodev-0.3.4/uiautodev/utils/usbmux.py
+-rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 uiautodev-0.3.4/PKG-INFO
```

### Comparing `uiautodev-0.3.3/LICENSE` & `uiautodev-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/pyproject.toml` & `uiautodev-0.3.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [tool.poetry]
 name = "uiautodev"
-version = "0.3.3"
+version = "0.3.4"
 description = "Mobile UI Automation, include UI hierarchy inspector, script recorder"
 homepage = "https://uiauto.dev"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-fastapi = {extras = ["all"], version = "^0.109.2"}
-uvicorn = {extras = ["standard"], version = "^0.27.1"}
 pillow = "*"
 adbutils = "^2.6.0"
 construct = "*"
 lxml = "*"
 click = "^8.1.7"
 pygments = ">=2"
 httpretty = {version = "^1.1.4", optional = true}
 appium-python-client = {version = "^4.0.0", optional = true}
-uiautomator2 = "^3.0.11"
+uiautomator2 = ">=2"
+httpx = "*"
+fastapi = "^0.111.0"
+uvicorn = "*"
+poetry = "^1.8.2"
 
 [tool.poetry.extras]
 appium = ["appium-python-client", "httppretty"]
 
 [tool.poetry.scripts]
 "uiauto.dev" = "uiautodev.__main__:main"
 "uiautodev" = "uiautodev.__main__:main"
```

### Comparing `uiautodev-0.3.3/uiautodev/app.py` & `uiautodev-0.3.4/uiautodev/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import FileResponse, RedirectResponse
 from pydantic import BaseModel
 
 from uiautodev import __version__
+from uiautodev.common import get_webpage_url
 from uiautodev.provider import AndroidProvider, IOSProvider, MockProvider
 from uiautodev.router.device import make_router
 from uiautodev.router.xml import router as xml_router
 
 logger = logging.getLogger(__name__)
 
 app = FastAPI()
@@ -85,8 +86,10 @@
     print(static_dir / "demo.html")
     return FileResponse(static_dir / "demo.html")
 
 
 @app.get("/")
 def index_redirect():
     """ redirect to official homepage """
-    return RedirectResponse("https://uiauto.dev")
+    url = get_webpage_url()
+    logger.debug("redirect to %s", url)
+    return RedirectResponse(url)
```

### Comparing `uiautodev-0.3.3/uiautodev/appium_proxy.py` & `uiautodev-0.3.4/uiautodev/appium_proxy.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/case.py` & `uiautodev-0.3.4/uiautodev/case.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/cli.py` & `uiautodev-0.3.4/uiautodev/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,46 +4,59 @@
 """Created on Tue Mar 19 2024 10:53:03 by codeskyblue
 """
 
 from __future__ import annotations
 
 import logging
 import platform
+import subprocess
 import sys
 import threading
 import time
 from pprint import pprint
 
 import click
 import httpx
 import pydantic
 import uvicorn
 
 from uiautodev import __version__, command_proxy
 from uiautodev.command_types import Command
+from uiautodev.common import get_webpage_url
 from uiautodev.provider import AndroidProvider, BaseProvider, IOSProvider
 from uiautodev.utils.common import convert_params_to_model, print_json
 
 logger = logging.getLogger(__name__)
 
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
-@click.group()
+@click.group(context_settings=CONTEXT_SETTINGS)
 @click.option("--verbose", "-v", is_flag=True, default=False, help="verbose mode")
 def cli(verbose: bool):
     if verbose:
+        # try to enable logger is not very easy
+        # you have to setup logHandler(logFormatter) for the root logger
+        # and set all children logger to DEBUG
+        # that's why it is not easy to use it with logging
         root_logger = logging.getLogger(__name__.split(".")[0])
         root_logger.setLevel(logging.DEBUG)
 
         console_handler = logging.StreamHandler()
         console_handler.setLevel(logging.DEBUG)
         
         formatter = logging.Formatter('%(name)s - %(levelname)s - %(message)s')
         console_handler.setFormatter(formatter)
 
         root_logger.addHandler(console_handler)
+
+        # set all children logger to DEBUG
+        for k in root_logger.manager.loggerDict.keys():
+            if k.startswith(root_logger.name+"."):
+                logging.getLogger(k).setLevel(logging.DEBUG)
+        
         logger.debug("Verbose mode enabled")
 
 
 def run_driver_command(provider: BaseProvider, command: Command, params: list[str] = None):
     if command == Command.LIST:
         devices = provider.list_devices()
         print("==> Devices <==")
@@ -106,23 +119,30 @@
         run_driver_command(provider, command, params)
     except AppiumDriverException as e:
         print(f"Error: {e}")
 
 
 @cli.command('version')
 def print_version():
+    """ Print version """
     print(__version__)
 
 
-@cli.command(help="start uiauto.dev local server [default]")
+@cli.command('self-update')
+def self_update():
+    """ Update uiautodev to latest version """
+    subprocess.run([sys.executable, '-m', "pip", "install", "--upgrade", "uiautodev"])
+
+
+@cli.command(help="start uiauto.dev local server [Default]")
 @click.option("--port", default=20242, help="port number", show_default=True)
 @click.option("--host", default="127.0.0.1", help="host", show_default=True)
 @click.option("--reload", is_flag=True, default=False, help="auto reload, dev only")
 @click.option("-f", "--force", is_flag=True, default=False, help="shutdown alrealy runningserver")
-@click.option("--no-browser", is_flag=True, default=False, help="do not open browser")
+@click.option("-s", "--no-browser", is_flag=True, default=False, help="silent mode, do not open browser")
 def server(port: int, host: str, reload: bool, force: bool, no_browser: bool):
     logger.info("version: %s", __version__)
     if force:
         try:
             httpx.get(f"http://{host}:{port}/shutdown", timeout=3)
         except httpx.HTTPError:
             pass
@@ -143,15 +163,15 @@
     while time.time() < deadline:
         try:
             httpx.get(f"{server_url}/api/info", timeout=1)
             break
         except Exception as e:
             time.sleep(0.5)
     import webbrowser
-    web_url = "https://uiauto.dev"
+    web_url = get_webpage_url()
     logger.info("open browser: %s", web_url)
     webbrowser.open(web_url)
 
 def main():
     # set logger level to INFO
     # logging.basicConfig(level=logging.INFO)
     logger.setLevel(logging.INFO)
```

### Comparing `uiautodev-0.3.3/uiautodev/command_proxy.py` & `uiautodev-0.3.4/uiautodev/command_proxy.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/command_types.py` & `uiautodev-0.3.4/uiautodev/command_types.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/driver/android.py` & `uiautodev-0.3.4/uiautodev/driver/android.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 """Created on Fri Mar 01 2024 14:19:29 by codeskyblue
 """
 
 import json
 import logging
 import re
-import socket
 import time
 from functools import cached_property, partial
 from typing import List, Tuple
 from xml.etree import ElementTree
 
 import adbutils
 import requests
+import uiautomator2 as u2
 from PIL import Image
 
 from uiautodev.command_types import CurrentAppResponse
 from uiautodev.driver.base_driver import BaseDriver
 from uiautodev.driver.udt.udt import UDT, UDTError
 from uiautodev.exceptions import AndroidDriverException, RequestError
 from uiautodev.model import Node, ShellResponse, WindowSize
@@ -30,32 +30,33 @@
     def __init__(self, serial: str):
         super().__init__(serial)
         self.device = adbutils.device(serial)
         self._try_dump_list = [
             self._get_u2_hierarchy,
             self._get_appium_hierarchy,
             self._get_udt_dump_hierarchy,
-            self.device.dump_hierarchy,
-            self._get_u2_lib_hierarchy,
         ]
     
     @cached_property
     def udt(self) -> UDT:    
         return UDT(self.device)
+
+    @cached_property
+    def ud(self) -> u2.Device:
+        return u2.connect_usb(self.serial)
     
     def screenshot(self, id: int) -> Image.Image:
-        # TODO: support multi-display
-        if id > 0:
-            raise ValueError("multi-display is not supported yet")
         try:
-            img = self.device.screenshot()
+            img = self.device.screenshot(display_id=id)
             return img.convert("RGB")
         except adbutils.AdbError as e:
             logger.warning("screenshot error: %s", str(e))
-            return self.udt.screenshot()
+            if id > 0:
+                raise AndroidDriverException("multi-display is not supported yet for uiautomator2")
+            return self.ud.screenshot()
 
     def shell(self, command: str) -> ShellResponse:
         try:
             ret = self.device.shell2(command, rstrip=True, timeout=20)
             if ret.returncode == 0:
                 return ShellResponse(output=ret.output, error=None)
             else:
@@ -89,28 +90,19 @@
             try:
                 logger.debug(f"try to dump with %s", dump_func.__name__)
                 result = dump_func()
                 logger.debug("dump success")
                 self._try_dump_list.remove(dump_func)
                 self._try_dump_list.insert(0, dump_func)
                 return result
-            except (
-                requests.RequestException,
-                AndroidDriverException,
-                UDTError,
-                adbutils.AdbError,
-                socket.timeout,
-            ) as e:
-                logger.warning("dump error: %s", e)
             except Exception as e:
                 logger.exception("unexpected dump error: %s", e)
         raise AndroidDriverException("Failed to dump hierarchy")
     
     def _get_u2_hierarchy(self) -> str:
-        import uiautomator2 as u2
         d = u2.connect_usb(self.serial)
         return d.dump_hierarchy()
         # c = self.device.create_connection(adbutils.Network.TCP, 9008)
         # try:
         #     compressed = False
         #     payload = {
         #         "jsonrpc": "2.0",
@@ -142,22 +134,14 @@
                 f"Failed to get hierarchy from appium server: {str(e)}"
             )
         finally:
             c.close()
 
     def _get_udt_dump_hierarchy(self) -> str:
         return self.udt.dump_hierarchy()
-
-    def _get_u2_lib_hierarchy(self) -> str:
-        try:
-            import uiautomator2 as u2
-            d = u2.connect_usb(self.serial)
-            return d.dump_hierarchy()
-        except ModuleNotFoundError:
-            raise AndroidDriverException("uiautomator2 lib not installed")
     
     def tap(self, x: int, y: int):
         self.device.click(x, y)
 
     def window_size(self) -> Tuple[int, int]:
         w, h = self.device.window_size()
         return (w, h)
```

### Comparing `uiautodev-0.3.3/uiautodev/driver/appium.py` & `uiautodev-0.3.4/uiautodev/driver/appium.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/driver/base_driver.py` & `uiautodev-0.3.4/uiautodev/driver/base_driver.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/driver/ios.py` & `uiautodev-0.3.4/uiautodev/driver/ios.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/driver/mock.py` & `uiautodev-0.3.4/uiautodev/driver/mock.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk` & `uiautodev-0.3.4/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/driver/udt/udt.py` & `uiautodev-0.3.4/uiautodev/driver/udt/udt.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 # -*- coding: utf-8 -*-
 
 """Created on Sun Apr 21 2024 21:15:15 by codeskyblue
 """
 
 
 import atexit
-from base64 import b64decode
 import enum
 import io
 import json
 import logging
-from pprint import pprint
 import threading
 import time
+from base64 import b64decode
 from pathlib import Path
+from pprint import pprint
 from typing import Any, Optional
 
-from PIL import Image
 import adbutils
 import requests
+from PIL import Image
 from pydantic import BaseModel
 
 """
 shell steps:
 adb push appium-uiautomator2-v5.12.4.apk /data/local/tmp/udt.jar
 adb shell CLASSPATH=/data/local/tmp/udt.jar app_process / "com.wetest.uia2.Main"
 adb forward tcp:6790 tcp:6790
```

### Comparing `uiautodev-0.3.3/uiautodev/model.py` & `uiautodev-0.3.4/uiautodev/model.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/provider.py` & `uiautodev-0.3.4/uiautodev/provider.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/router/device.py` & `uiautodev-0.3.4/uiautodev/router/device.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/router/xml.py` & `uiautodev-0.3.4/uiautodev/router/xml.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/static/demo.html` & `uiautodev-0.3.4/uiautodev/static/demo.html`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/utils/common.py` & `uiautodev-0.3.4/uiautodev/utils/common.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/utils/exceptions.py` & `uiautodev-0.3.4/uiautodev/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/uiautodev/utils/usbmux.py` & `uiautodev-0.3.4/uiautodev/utils/usbmux.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.3/PKG-INFO` & `uiautodev-0.3.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uiautodev
-Version: 0.3.3
+Version: 0.3.4
 Summary: Mobile UI Automation, include UI hierarchy inspector, script recorder
 Home-page: https://uiauto.dev
 License: MIT
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,31 +15,59 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: appium
 Requires-Dist: adbutils (>=2.6.0,<3.0.0)
 Requires-Dist: appium-python-client (>=4.0.0,<5.0.0) ; extra == "appium"
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: construct
-Requires-Dist: fastapi[all] (>=0.109.2,<0.110.0)
+Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: httpretty (>=1.1.4,<2.0.0)
+Requires-Dist: httpx
 Requires-Dist: lxml
 Requires-Dist: pillow
+Requires-Dist: poetry (>=1.8.2,<2.0.0)
 Requires-Dist: pygments (>=2)
-Requires-Dist: uiautomator2 (>=3.0.11,<4.0.0)
-Requires-Dist: uvicorn[standard] (>=0.27.1,<0.28.0)
+Requires-Dist: uiautomator2 (>=2)
+Requires-Dist: uvicorn
 Description-Content-Type: text/markdown
 
 # uiautodev
 [![codecov](https://codecov.io/gh/codeskyblue/appinspector/graph/badge.svg?token=aLTg4VOyQH)](https://codecov.io/gh/codeskyblue/appinspector)
 [![PyPI version](https://badge.fury.io/py/uiautodev.svg)](https://badge.fury.io/py/uiautodev)
 
 https://uiauto.dev
 
 UI Inspector for Android and iOS, help inspector element properties, and auto generate XPath, script.
 
+# Install
+```bash
+pip install uiautodev
+```
+
+# Usage
+```bash
+Usage: uiauto.dev [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  -v, --verbose  verbose mode
+  -h, --help     Show this message and exit.
+
+Commands:
+  android      COMMAND: tap, tapElement, installApp, currentApp,...
+  appium       COMMAND: tap, tapElement, installApp, currentApp,...
+  ios          COMMAND: tap, tapElement, installApp, currentApp,...
+  self-update  Update uiautodev to latest version
+  server       start uiauto.dev local server [Default]
+  version      Print version
+```
+
+```bash
+# run local server and open browser
+uiauto.dev
+```
 
 # DEVELOP
 ```bash
 # install poetry (python package manager)
 pip install poetry # pipx install poetry
 
 # install deps
```

