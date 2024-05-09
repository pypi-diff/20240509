# Comparing `tmp/py5paisa-0.7.8.tar.gz` & `tmp/py5paisa-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py5paisa-0.7.8.tar", last modified: Wed Jan 17 07:51:35 2024, max compression
+gzip compressed data, was "py5paisa-0.7.9.tar", last modified: Fri Jan 19 09:34:12 2024, max compression
```

## Comparing `py5paisa-0.7.8.tar` & `py5paisa-0.7.9.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 07:51:35.066829 py5paisa-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-17 07:51:27.000000 py5paisa-0.7.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-01-17 07:51:27.000000 py5paisa-0.7.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-17 07:51:27.000000 py5paisa-0.7.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-17 07:51:27.000000 py5paisa-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15524 2024-01-17 07:51:35.066829 py5paisa-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-01-17 07:51:27.000000 py5paisa-0.7.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 07:51:35.062829 py5paisa-0.7.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 07:51:35.062829 py5paisa-0.7.8/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    48489 2024-01-17 07:51:27.000000 py5paisa-0.7.8/docs/images/5-paisa-img.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 07:51:35.062829 py5paisa-0.7.8/py5paisa/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-17 07:51:27.000000 py5paisa-0.7.8/py5paisa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-17 07:51:27.000000 py5paisa-0.7.8/py5paisa/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-01-17 07:51:27.000000 py5paisa-0.7.8/py5paisa/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-17 07:51:27.000000 py5paisa-0.7.8/py5paisa/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-01-17 07:51:27.000000 py5paisa-0.7.8/py5paisa/order.py
--rw-r--r--   0 runner    (1001) docker     (127)    36361 2024-01-17 07:51:27.000000 py5paisa-0.7.8/py5paisa/py5paisa.py
--rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-01-17 07:51:27.000000 py5paisa-0.7.8/py5paisa/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-01-17 07:51:27.000000 py5paisa-0.7.8/py5paisa/urlconst.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 07:51:35.062829 py5paisa-0.7.8/py5paisa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15524 2024-01-17 07:51:35.000000 py5paisa-0.7.8/py5paisa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-17 07:51:35.000000 py5paisa-0.7.8/py5paisa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 07:51:35.000000 py5paisa-0.7.8/py5paisa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 07:51:35.000000 py5paisa-0.7.8/py5paisa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-17 07:51:35.000000 py5paisa-0.7.8/py5paisa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-17 07:51:35.000000 py5paisa-0.7.8/py5paisa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-17 07:51:35.066829 py5paisa-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-01-17 07:51:27.000000 py5paisa-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 07:51:35.066829 py5paisa-0.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 07:51:27.000000 py5paisa-0.7.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-17 07:51:27.000000 py5paisa-0.7.8/tests/test_py5paisa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:34:12.854938 py5paisa-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-19 09:33:56.000000 py5paisa-0.7.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-01-19 09:33:56.000000 py5paisa-0.7.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-19 09:33:56.000000 py5paisa-0.7.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-19 09:33:56.000000 py5paisa-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15524 2024-01-19 09:34:12.854938 py5paisa-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-01-19 09:33:56.000000 py5paisa-0.7.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:34:12.850938 py5paisa-0.7.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:34:12.850938 py5paisa-0.7.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    48489 2024-01-19 09:33:56.000000 py5paisa-0.7.9/docs/images/5-paisa-img.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:34:12.854938 py5paisa-0.7.9/py5paisa/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-19 09:33:56.000000 py5paisa-0.7.9/py5paisa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-19 09:33:56.000000 py5paisa-0.7.9/py5paisa/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-01-19 09:33:56.000000 py5paisa-0.7.9/py5paisa/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-01-19 09:33:56.000000 py5paisa-0.7.9/py5paisa/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-19 09:33:56.000000 py5paisa-0.7.9/py5paisa/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-01-19 09:33:56.000000 py5paisa-0.7.9/py5paisa/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37408 2024-01-19 09:33:56.000000 py5paisa-0.7.9/py5paisa/py5paisa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-01-19 09:33:56.000000 py5paisa-0.7.9/py5paisa/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-01-19 09:33:56.000000 py5paisa-0.7.9/py5paisa/urlconst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:34:12.854938 py5paisa-0.7.9/py5paisa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15524 2024-01-19 09:34:12.000000 py5paisa-0.7.9/py5paisa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-19 09:34:12.000000 py5paisa-0.7.9/py5paisa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 09:34:12.000000 py5paisa-0.7.9/py5paisa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 09:34:12.000000 py5paisa-0.7.9/py5paisa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-19 09:34:12.000000 py5paisa-0.7.9/py5paisa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-19 09:34:12.000000 py5paisa-0.7.9/py5paisa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-19 09:34:12.854938 py5paisa-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-01-19 09:33:56.000000 py5paisa-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:34:12.854938 py5paisa-0.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 09:33:56.000000 py5paisa-0.7.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-19 09:33:56.000000 py5paisa-0.7.9/tests/test_py5paisa.py
```

### Comparing `py5paisa-0.7.8/CONTRIBUTING.rst` & `py5paisa-0.7.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.8/PKG-INFO` & `py5paisa-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py5paisa
-Version: 0.7.8
+Version: 0.7.9
 Summary:  Python SDK for 5paisa APIs natively written in VB.NET
 Home-page: https://github.com/5paisa/py5paisa
 Author: 5paisa
 Author-email: coreteam@5paisa.com
 Keywords: py5paisa
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `py5paisa-0.7.8/README.rst` & `py5paisa-0.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.8/docs/images/5-paisa-img.jpg` & `py5paisa-0.7.9/docs/images/5-paisa-img.jpg`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.8/py5paisa/auth.py` & `py5paisa-0.7.9/py5paisa/auth.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.8/py5paisa/const.py` & `py5paisa-0.7.9/py5paisa/const.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.8/py5paisa/order.py` & `py5paisa-0.7.9/py5paisa/order.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.8/py5paisa/py5paisa.py` & `py5paisa-0.7.9/py5paisa/py5paisa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 from .auth import EncryptionClient
 from .const import *
 from .order import Order, Bo_co_order, RequestType, Basket_order
 from .logging import log_response
 import json
+import csv
 import websocket
 import pandas as pd
 import websocket
 from .urlconst import *
+
+from io import StringIO
 from enum import Enum
 
 
 class FivePaisaClient:
 
     def __init__(self, cred=None):
         """
@@ -25,14 +28,15 @@
             self.Aspx_auth = None
             self.web_url = None
             self.market_depth_url = None
             self.Res_Data = None
             self.ws = None
             self.access_token = ""
             self.request_token = None
+            self.scrip_data = None
             self.session = requests.Session()
             self.APP_SOURCE = cred["APP_SOURCE"]
             self.APP_NAME = cred["APP_NAME"]
             self.USER_ID = cred["USER_ID"]
             self.PASSWORD = cred["PASSWORD"]
             self.USER_KEY = cred["USER_KEY"]
             self.ENCRYPTION_KEY = cred["ENCRYPTION_KEY"]
@@ -40,14 +44,38 @@
             self.VTT_TYPE = VTT_TYPE
             self.create_payload()
             self.set_url()
 
         except Exception as e:
             log_response(e)
 
+    def get_scrips(self):
+        try:
+            if self.scrip_data is None:
+                response = self.session.get(
+                    self.SCRIP_MASTER_ROUTE, headers=HEADERS)
+
+                data = response.content.decode("utf-8").strip()
+
+                reader = csv.DictReader(StringIO(data))
+                records = pd.DataFrame(reader)
+
+                self.scrip_data = records
+            return self.scrip_data
+        except Exception as e:
+            log_response(e)
+
+    def query_scrips(self, exchange, exchangetype, symbol, strike, type, expiry):
+        try:
+            if self.scrip_data is None:
+                self.get_scrips()
+            return self.scrip_data.query('Exch=="'+exchange+'" & ExchType=="'+exchangetype+'" & SymbolRoot=="'+symbol+'" & StrikeRate=="'+strike+'" & ScripType=="'+type+'" & Expiry=="'+expiry+'"')
+        except Exception as e:
+            log_response(e)
+
     def holdings(self):
         try:
             return self._user_info_request("HOLDINGS")
         except Exception as e:
             log_response(e)
 
     def margin(self):
@@ -610,14 +638,15 @@
         try:
             return self.order_request("TB")
         except Exception as e:
             log_response(e)
 
     def set_url(self):
         try:
+            self.SCRIP_MASTER_ROUTE = SCRIP_MASTER_ROUTE
             self.LOGIN_ROUTE = LOGIN_ROUTE
             self.MARGIN_ROUTE = MARGIN_ROUTE
             self.ORDER_BOOK_ROUTE = ORDER_BOOK_ROUTE
             self.HOLDINGS_ROUTE = HOLDINGS_ROUTE
             self.POSITIONS_ROUTE = POSITIONS_ROUTE
             self.ORDER_PLACEMENT_ROUTE = ORDER_PLACEMENT_ROUTE
             self.ORDER_MODIFY_ROUTE = ORDER_MODIFY_ROUTE
```

### Comparing `py5paisa-0.7.8/py5paisa/strategy.py` & `py5paisa-0.7.9/py5paisa/strategy.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.8/py5paisa/urlconst.py` & `py5paisa-0.7.9/py5paisa/urlconst.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 BaseUrl = 'https://Openapi.5paisa.com/VendorsAPI/Service1.svc/'
 
 
 LOGIN_ROUTE = f'{BaseUrl}V4/LoginRequestMobileNewbyEmail'
 
+SCRIP_MASTER_ROUTE=f'{BaseUrl}ScripMaster/segment/All'
+
 MARGIN_ROUTE = f'{BaseUrl}V4/Margin'
 ORDER_BOOK_ROUTE = f'{BaseUrl}V3/OrderBook'
 HOLDINGS_ROUTE = f'{BaseUrl}V3/Holding'
 POSITIONS_ROUTE = f'{BaseUrl}V2/NetPositionNetWise'
 
 ORDER_PLACEMENT_ROUTE = f'{BaseUrl}V1/PlaceOrderRequest'
 ORDER_MODIFY_ROUTE = f'{BaseUrl}V1/ModifyOrderRequest'
```

### Comparing `py5paisa-0.7.8/py5paisa.egg-info/PKG-INFO` & `py5paisa-0.7.9/py5paisa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py5paisa
-Version: 0.7.8
+Version: 0.7.9
 Summary:  Python SDK for 5paisa APIs natively written in VB.NET
 Home-page: https://github.com/5paisa/py5paisa
 Author: 5paisa
 Author-email: coreteam@5paisa.com
 Keywords: py5paisa
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `py5paisa-0.7.8/setup.py` & `py5paisa-0.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     keywords='py5paisa',
     name='py5paisa',
     packages=find_packages(include=['py5paisa', 'py5paisa.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/5paisa/py5paisa',
-    version='0.7.8',
+    version='0.7.9',
     zip_safe=False,
 )
```

