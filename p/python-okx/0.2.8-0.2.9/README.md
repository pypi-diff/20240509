# Comparing `tmp/python-okx-0.2.8.tar.gz` & `tmp/python-okx-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-okx-0.2.8.tar", last modified: Thu Mar  7 10:15:09 2024, max compression
+gzip compressed data, was "python-okx-0.2.9.tar", last modified: Thu May  9 08:24:47 2024, max compression
```

## Comparing `python-okx-0.2.8.tar` & `python-okx-0.2.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-03-07 10:15:09.978410 python-okx-0.2.8/
--rw-r--r--   0 oker       (501) staff       (20)     3123 2024-03-07 10:15:09.978052 python-okx-0.2.8/PKG-INFO
--rw-r--r--   0 oker       (501) staff       (20)     2618 2023-12-07 06:04:16.000000 python-okx-0.2.8/README.md
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-03-07 10:15:09.972249 python-okx-0.2.8/okx/
--rw-r--r--   0 oker       (501) staff       (20)     9685 2024-03-07 10:10:47.000000 python-okx-0.2.8/okx/Account.py
--rw-r--r--   0 oker       (501) staff       (20)     4128 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/BlockTrading.py
--rw-r--r--   0 oker       (501) staff       (20)     1575 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/Convert.py
--rw-r--r--   0 oker       (501) staff       (20)     2750 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/CopyTrading.py
--rw-r--r--   0 oker       (501) staff       (20)     3853 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/Earning.py
--rw-r--r--   0 oker       (501) staff       (20)      788 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/FDBroker.py
--rw-r--r--   0 oker       (501) staff       (20)     6090 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/Funding.py
--rw-r--r--   0 oker       (501) staff       (20)     6691 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/Grid.py
--rw-r--r--   0 oker       (501) staff       (20)     4928 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/MarketData.py
--rw-r--r--   0 oker       (501) staff       (20)     5063 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/NDBroker.py
--rw-r--r--   0 oker       (501) staff       (20)     5136 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/PublicData.py
--rw-r--r--   0 oker       (501) staff       (20)     3227 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/SpreadTrading.py
--rw-r--r--   0 oker       (501) staff       (20)      495 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/Status.py
--rw-r--r--   0 oker       (501) staff       (20)     3528 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/SubAccount.py
--rw-r--r--   0 oker       (501) staff       (20)    10797 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/Trade.py
--rw-r--r--   0 oker       (501) staff       (20)     2331 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/TradingData.py
--rw-r--r--   0 oker       (501) staff       (20)       58 2024-02-28 03:14:05.000000 python-okx-0.2.8/okx/__init__.py
--rw-r--r--   0 oker       (501) staff       (20)    14331 2024-02-27 09:18:35.000000 python-okx-0.2.8/okx/consts.py
--rw-r--r--   0 oker       (501) staff       (20)     1182 2023-12-07 06:04:16.000000 python-okx-0.2.8/okx/exceptions.py
--rw-r--r--   0 oker       (501) staff       (20)     2144 2024-02-02 06:46:15.000000 python-okx-0.2.8/okx/okxclient.py
--rw-r--r--   0 oker       (501) staff       (20)     1826 2024-01-24 06:58:57.000000 python-okx-0.2.8/okx/utils.py
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-03-07 10:15:09.975036 python-okx-0.2.8/okx/websocket/
--rw-r--r--   0 oker       (501) staff       (20)      895 2023-12-26 08:54:41.000000 python-okx-0.2.8/okx/websocket/WebSocketFactory.py
--rw-r--r--   0 oker       (501) staff       (20)     2282 2024-01-24 08:39:57.000000 python-okx-0.2.8/okx/websocket/WsPrivateAsync.py
--rw-r--r--   0 oker       (501) staff       (20)     1561 2024-01-24 08:39:57.000000 python-okx-0.2.8/okx/websocket/WsPublicAsync.py
--rw-r--r--   0 oker       (501) staff       (20)     2199 2023-12-26 08:54:41.000000 python-okx-0.2.8/okx/websocket/WsUtils.py
--rw-r--r--   0 oker       (501) staff       (20)        0 2023-12-27 10:30:41.000000 python-okx-0.2.8/okx/websocket/__init__.py
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-03-07 10:15:09.977630 python-okx-0.2.8/python_okx.egg-info/
--rw-r--r--   0 oker       (501) staff       (20)     3123 2024-03-07 10:15:09.000000 python-okx-0.2.8/python_okx.egg-info/PKG-INFO
--rw-r--r--   0 oker       (501) staff       (20)      677 2024-03-07 10:15:09.000000 python-okx-0.2.8/python_okx.egg-info/SOURCES.txt
--rw-r--r--   0 oker       (501) staff       (20)        1 2024-03-07 10:15:09.000000 python-okx-0.2.8/python_okx.egg-info/dependency_links.txt
--rw-r--r--   0 oker       (501) staff       (20)       67 2024-03-07 10:15:09.000000 python-okx-0.2.8/python_okx.egg-info/requires.txt
--rw-r--r--   0 oker       (501) staff       (20)        4 2024-03-07 10:15:09.000000 python-okx-0.2.8/python_okx.egg-info/top_level.txt
--rw-r--r--   0 oker       (501) staff       (20)       38 2024-03-07 10:15:09.978514 python-okx-0.2.8/setup.cfg
--rw-r--r--   0 oker       (501) staff       (20)      775 2024-02-02 06:45:26.000000 python-okx-0.2.8/setup.py
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-05-09 08:24:47.660338 python-okx-0.2.9/
+-rw-r--r--   0 oker       (501) staff       (20)     3123 2024-05-09 08:24:47.647648 python-okx-0.2.9/PKG-INFO
+-rw-r--r--   0 oker       (501) staff       (20)     2618 2023-12-07 06:04:16.000000 python-okx-0.2.9/README.md
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-05-09 08:24:47.639303 python-okx-0.2.9/okx/
+-rw-r--r--   0 oker       (501) staff       (20)     9684 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/Account.py
+-rw-r--r--   0 oker       (501) staff       (20)     4127 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/BlockTrading.py
+-rw-r--r--   0 oker       (501) staff       (20)     1574 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/Convert.py
+-rw-r--r--   0 oker       (501) staff       (20)     2750 2024-02-02 06:46:15.000000 python-okx-0.2.9/okx/CopyTrading.py
+-rw-r--r--   0 oker       (501) staff       (20)     3852 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/Earning.py
+-rw-r--r--   0 oker       (501) staff       (20)      787 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/FDBroker.py
+-rw-r--r--   0 oker       (501) staff       (20)     6277 2024-05-09 08:21:39.000000 python-okx-0.2.9/okx/Funding.py
+-rw-r--r--   0 oker       (501) staff       (20)     6690 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/Grid.py
+-rw-r--r--   0 oker       (501) staff       (20)     4927 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/MarketData.py
+-rw-r--r--   0 oker       (501) staff       (20)     5062 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/NDBroker.py
+-rw-r--r--   0 oker       (501) staff       (20)     5135 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/PublicData.py
+-rw-r--r--   0 oker       (501) staff       (20)     3226 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/SpreadTrading.py
+-rw-r--r--   0 oker       (501) staff       (20)      494 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/Status.py
+-rw-r--r--   0 oker       (501) staff       (20)     3527 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/SubAccount.py
+-rw-r--r--   0 oker       (501) staff       (20)    10795 2024-05-09 08:21:39.000000 python-okx-0.2.9/okx/Trade.py
+-rw-r--r--   0 oker       (501) staff       (20)     2330 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/TradingData.py
+-rw-r--r--   0 oker       (501) staff       (20)       58 2024-05-07 07:09:18.000000 python-okx-0.2.9/okx/__init__.py
+-rw-r--r--   0 oker       (501) staff       (20)    14387 2024-05-09 08:21:39.000000 python-okx-0.2.9/okx/consts.py
+-rw-r--r--   0 oker       (501) staff       (20)     1182 2023-12-07 06:04:16.000000 python-okx-0.2.9/okx/exceptions.py
+-rw-r--r--   0 oker       (501) staff       (20)     2510 2024-05-09 08:22:18.000000 python-okx-0.2.9/okx/okxclient.py
+-rw-r--r--   0 oker       (501) staff       (20)     1826 2024-01-24 06:58:57.000000 python-okx-0.2.9/okx/utils.py
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-05-09 08:24:47.642860 python-okx-0.2.9/okx/websocket/
+-rw-r--r--   0 oker       (501) staff       (20)      895 2023-12-26 08:54:41.000000 python-okx-0.2.9/okx/websocket/WebSocketFactory.py
+-rw-r--r--   0 oker       (501) staff       (20)     2282 2024-01-24 08:39:57.000000 python-okx-0.2.9/okx/websocket/WsPrivateAsync.py
+-rw-r--r--   0 oker       (501) staff       (20)     1561 2024-01-24 08:39:57.000000 python-okx-0.2.9/okx/websocket/WsPublicAsync.py
+-rw-r--r--   0 oker       (501) staff       (20)     2199 2023-12-26 08:54:41.000000 python-okx-0.2.9/okx/websocket/WsUtils.py
+-rw-r--r--   0 oker       (501) staff       (20)        0 2023-12-27 10:30:41.000000 python-okx-0.2.9/okx/websocket/__init__.py
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-05-09 08:24:47.646967 python-okx-0.2.9/python_okx.egg-info/
+-rw-r--r--   0 oker       (501) staff       (20)     3123 2024-05-09 08:24:47.000000 python-okx-0.2.9/python_okx.egg-info/PKG-INFO
+-rw-r--r--   0 oker       (501) staff       (20)      677 2024-05-09 08:24:47.000000 python-okx-0.2.9/python_okx.egg-info/SOURCES.txt
+-rw-r--r--   0 oker       (501) staff       (20)        1 2024-05-09 08:24:47.000000 python-okx-0.2.9/python_okx.egg-info/dependency_links.txt
+-rw-r--r--   0 oker       (501) staff       (20)       67 2024-05-09 08:24:47.000000 python-okx-0.2.9/python_okx.egg-info/requires.txt
+-rw-r--r--   0 oker       (501) staff       (20)        4 2024-05-09 08:24:47.000000 python-okx-0.2.9/python_okx.egg-info/top_level.txt
+-rw-r--r--   0 oker       (501) staff       (20)       38 2024-05-09 08:24:47.660500 python-okx-0.2.9/setup.cfg
+-rw-r--r--   0 oker       (501) staff       (20)      775 2024-02-02 06:45:26.000000 python-okx-0.2.9/setup.py
```

### Comparing `python-okx-0.2.8/PKG-INFO` & `python-okx-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-okx
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python SDK for OKX
 Home-page: https://okx.com/docs-v5/
 Author: okxv5api
 Author-email: api@okg.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-okx-0.2.8/README.md` & `python-okx-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.8/okx/Account.py` & `python-okx-0.2.9/okx/Account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .okxclient import OkxClient
 from .consts import *
 
 
 class AccountAPI(OkxClient):
 
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True,proxy = None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True,proxy = None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
     # Get Positions
     def get_position_risk(self, instType=''):
         params = {}
         if instType:
             params['instType'] = instType
```

### Comparing `python-okx-0.2.8/okx/BlockTrading.py` & `python-okx-0.2.9/okx/BlockTrading.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .okxclient import OkxClient
 from .consts import *
 
 
 class BlockTradingAPI(OkxClient):
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
     def counterparties(self):
         params = {}
         return self._request_with_params(GET, COUNTERPARTIES, params)
 
     def create_rfq(self, counterparties=[], anonymous='false', clRfqId='', tag='', allowPartialExecution='false',
```

### Comparing `python-okx-0.2.8/okx/Convert.py` & `python-okx-0.2.9/okx/Convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .okxclient import OkxClient
 from .consts import *
 
 
 class ConvertAPI(OkxClient):
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True,proxy = None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True,proxy = None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
     def get_currencies(self):
         params = {}
         return self._request_with_params(GET, GET_CURRENCIES, params)
 
     def get_currency_pair(self, fromCcy='', toCcy=''):
```

### Comparing `python-okx-0.2.8/okx/CopyTrading.py` & `python-okx-0.2.9/okx/CopyTrading.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.8/okx/Earning.py` & `python-okx-0.2.9/okx/Earning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .okxclient import OkxClient
 from .consts import *
 
 
 class EarningAPI(OkxClient):
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
     def get_offers(self,productId = '',protocolType = '',ccy = ''):
         params = {
             'productId':productId,
             'protocolType':protocolType,
             'ccy':ccy
```

### Comparing `python-okx-0.2.8/okx/FDBroker.py` & `python-okx-0.2.9/okx/FDBroker.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .okxclient import OkxClient
 from .consts import *
 
 
 class FDBrokerAPI(OkxClient):
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
     def generate_rebate_details_download_link(self, begin ='', end = ''):
         params = {'begin': begin, 'end': end}
         return self._request_with_params(POST, FD_REBATE_PER_ORDERS, params)
 
     def get_rebate_details_download_link(self, type = '', begin = '', end = ''):
```

### Comparing `python-okx-0.2.8/okx/Funding.py` & `python-okx-0.2.9/okx/Funding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from .okxclient import OkxClient
 from .consts import *
 
 
 class FundingAPI(OkxClient):
 
 
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
+    # Get Non Tradable Assets
+    def get_non_tradable_assets(self, ccy: str = ''):
+        params = {'ccy': ccy}
+        return self._request_with_params(GET, NON_TRADABLE_ASSETS, params)
+
     # Get Deposit Address
     def get_deposit_address(self, ccy):
         params = {'ccy': ccy}
         return self._request_with_params(GET, DEPOSIT_ADDRESS, params)
 
     # Get Transfer State
     def transfer_state(self, transId,type=''):
@@ -35,20 +40,20 @@
                   'areaCode': areaCode, 'clientId': clientId}
         return self._request_with_params(POST, WITHDRAWAL_COIN, params)
 
     # Get Deposit History
     def get_deposit_history(self, ccy='', state='', after='', before='', limit='', txId='', depId='', fromWdId=''):
         params = {'ccy': ccy, 'state': state, 'after': after, 'before': before, 'limit': limit, 'txId': txId,
                   'depId': depId, 'fromWdId': fromWdId}
-        return self._request_with_params(GET, DEPOSIT_HISTORIY, params)
+        return self._request_with_params(GET, DEPOSIT_HISTORY, params)
 
     # Get Withdrawal History
     def get_withdrawal_history(self, ccy='', wdId='', state='', after='', before='', limit='',txId=''):
         params = {'ccy': ccy, 'wdId': wdId, 'state': state, 'after': after, 'before': before, 'limit': limit,'txId':txId}
-        return self._request_with_params(GET, WITHDRAWAL_HISTORIY, params)
+        return self._request_with_params(GET, WITHDRAWAL_HISTORY, params)
 
     # Get Currencies
     def get_currencies(self, ccy=''):
         params = {'ccy': ccy}
         return self._request_with_params(GET, CURRENCY_INFO, params)
 
     # PiggyBank Purchase/Redemption
```

### Comparing `python-okx-0.2.8/okx/Grid.py` & `python-okx-0.2.9/okx/Grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .okxclient import OkxClient
 from .consts import *
 
 
 class GridAPI(OkxClient):
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
     def grid_order_algo(self, instId='', algoOrdType='', maxPx='', minPx='', gridNum='', runType='', tpTriggerPx='',
                         slTriggerPx='', tag='', quoteSz='', baseSz='', sz='', direction='', lever='', basePos=''):
         params = {'instId': instId, 'algoOrdType': algoOrdType, 'maxPx': maxPx, 'minPx': minPx, 'gridNum': gridNum,
                   'runType': runType, 'tpTriggerPx': tpTriggerPx, 'slTriggerPx': slTriggerPx, 'tag': tag,
                   'quoteSz': quoteSz, 'baseSz': baseSz, 'sz': sz, 'direction': direction, 'lever': lever,
```

### Comparing `python-okx-0.2.8/okx/MarketData.py` & `python-okx-0.2.9/okx/MarketData.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .okxclient import OkxClient
 from .consts import *
 
 
 class MarketAPI(OkxClient):
 
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
 
     # Get Tickers
     def get_tickers(self, instType, uly='', instFamily =''):
         if uly:
             params = {'instType': instType, 'uly': uly, 'instFamily': instFamily}
```

### Comparing `python-okx-0.2.8/okx/NDBroker.py` & `python-okx-0.2.9/okx/NDBroker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .okxclient import OkxClient
 from .consts import *
 class NDBrokerAPI(OkxClient):
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
     #GET /api/v5/broker/nd/info
     def get_broker_info(self):
         return self._request_without_params(GET, BROKER_INFO)
 
     #POST /api/v5/broker/nd/create-subaccount
```

### Comparing `python-okx-0.2.8/okx/PublicData.py` & `python-okx-0.2.9/okx/PublicData.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .okxclient import OkxClient
 from .consts import *
 
 
 class PublicAPI(OkxClient):
 
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
     # Get Instruments
     def get_instruments(self, instType, uly='', instId='',instFamily = ''):
         params = {'instType': instType, 'uly': uly, 'instId': instId,'instFamily':instFamily}
         return self._request_with_params(GET, INSTRUMENT_INFO, params)
```

### Comparing `python-okx-0.2.8/okx/SpreadTrading.py` & `python-okx-0.2.9/okx/SpreadTrading.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .okxclient import OkxClient
 from .consts import *
 
 
 class SpreadTradingAPI(OkxClient):
 
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
     # Place Order
     def place_order(self, sprdId='', clOrdId='', tag='', side='', ordType='', sz='', px=''):
         params = {'sprdId': sprdId, 'clOrdId': clOrdId, 'tag': tag, 'side': side, 'ordType': ordType, 'sz': sz,
                   'px': px}
         return self._request_with_params(POST, SPREAD_PLACE_ORDER, params)
```

### Comparing `python-okx-0.2.8/okx/SubAccount.py` & `python-okx-0.2.9/okx/SubAccount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .okxclient import OkxClient
 from .consts import *
 
 
 class SubAccountAPI(OkxClient):
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
     def get_account_balance(self, subAcct):
         params = {"subAcct": subAcct}
         return self._request_with_params(GET, BALANCE, params)
 
     def bills(self, ccy='', type='', subAcct='', after='', before='', limit=''):
```

### Comparing `python-okx-0.2.8/okx/Trade.py` & `python-okx-0.2.9/okx/Trade.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from .okxclient import OkxClient
 from .consts import *
 
 
 class TradeAPI(OkxClient):
 
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1',
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1',
                  domain='https://www.okx.com', debug=True, proxy=None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
     # Place Order
     def place_order(self, instId, tdMode, side, ordType, sz, ccy='', clOrdId='', tag='', posSide='', px='',
                     reduceOnly='', tgtCcy='', tpTriggerPx='', tpOrdPx='', slTriggerPx='', slOrdPx='',
                     tpTriggerPxType='', slTriggerPxType='', quickMgnType='', stpId='', stpMode='',
@@ -36,15 +36,15 @@
     def cancel_multiple_orders(self, orders_data):
         return self._request_with_params(POST, CANCEL_BATCH_ORDERS, orders_data)
 
     # Amend Order
     def amend_order(self, instId, cxlOnFail='', ordId='', clOrdId='', reqId='', newSz='', newPx='', newTpTriggerPx='',
                     newTpOrdPx='', newSlTriggerPx='', newSlOrdPx='', newTpTriggerPxType='', newSlTriggerPxType='',
                     attachAlgoOrds=''):
-        params = {'instId': instId, 'cxlOnFailc': cxlOnFail, 'ordId': ordId, 'clOrdId': clOrdId, 'reqId': reqId,
+        params = {'instId': instId, 'cxlOnFail': cxlOnFail, 'ordId': ordId, 'clOrdId': clOrdId, 'reqId': reqId,
                   'newSz': newSz, 'newPx': newPx, 'newTpTriggerPx': newTpTriggerPx, 'newTpOrdPx': newTpOrdPx,
                   'newSlTriggerPx': newSlTriggerPx, 'newSlOrdPx': newSlOrdPx, 'newTpTriggerPxType': newTpTriggerPxType,
                   'newSlTriggerPxType': newSlTriggerPxType}
         params['attachAlgoOrds'] = attachAlgoOrds
         return self._request_with_params(POST, AMEND_ORDER, params)
 
     # Amend Multiple Orders
@@ -120,15 +120,15 @@
         return self._request_with_params(POST, Cancel_Advance_Algos, params)
 
     # Get Algo Order List
     def order_algos_list(self, ordType='', algoId='', instType='', instId='', after='', before='', limit='',
                          algoClOrdId=''):
         params = {'ordType': ordType, 'algoId': algoId, 'instType': instType, 'instId': instId, 'after': after,
                   'before': before, 'limit': limit, 'algoClOrdId': algoClOrdId}
-        return self._request_with_params(GET, ORDERS_ALGO_OENDING, params)
+        return self._request_with_params(GET, ORDERS_ALGO_PENDING, params)
 
     # Get Algo Order History
     def order_algos_history(self, ordType, state='', algoId='', instType='', instId='', after='', before='', limit=''):
         params = {'ordType': ordType, 'state': state, 'algoId': algoId, 'instType': instType, 'instId': instId,
                   'after': after, 'before': before, 'limit': limit}
         return self._request_with_params(GET, ORDERS_ALGO_HISTORY, params)
```

### Comparing `python-okx-0.2.8/okx/TradingData.py` & `python-okx-0.2.9/okx/TradingData.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .okxclient import OkxClient
 from .consts import *
 
 
 class TradingDataAPI(OkxClient):
 
-    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=False, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
+    def __init__(self, api_key='-1', api_secret_key='-1', passphrase='-1', use_server_time=None, flag='1', domain = 'https://www.okx.com',debug = True, proxy=None):
         OkxClient.__init__(self, api_key, api_secret_key, passphrase, use_server_time, flag, domain, debug, proxy)
 
 
     def get_support_coin(self):
         return self._request_without_params(GET, SUPPORT_COIN)
 
     def get_taker_volume(self, ccy, instType, begin='', end='', period=''):
```

### Comparing `python-okx-0.2.8/okx/consts.py` & `python-okx-0.2.9/okx/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,27 +52,28 @@
 GET_VIP_LOAN_ORDER_DETAIL= '/api/v5/account/vip-loan-order-detail'
 SET_RISK_OFFSET_TYPE = '/api/v5/account/set-riskOffset-type'
 SET_AUTO_LOAN = '/api/v5/account/set-auto-loan'
 ACTIVSTE_OPTION = '/api/v5/account/activate-option'
 POSITION_BUILDER = '/api/v5/account/position-builder'
 
 # funding-complete-testcomplete
+NON_TRADABLE_ASSETS = '/api/v5/asset/non-tradable-assets'
 DEPOSIT_ADDRESS = '/api/v5/asset/deposit-address'
 GET_BALANCES = '/api/v5/asset/balances'
 FUNDS_TRANSFER = '/api/v5/asset/transfer'
 TRANSFER_STATE = '/api/v5/asset/transfer-state'
 WITHDRAWAL_COIN = '/api/v5/asset/withdrawal'
-DEPOSIT_HISTORIY = '/api/v5/asset/deposit-history'
+DEPOSIT_HISTORY = '/api/v5/asset/deposit-history'
 CURRENCY_INFO = '/api/v5/asset/currencies'
 PURCHASE_REDEMPT = '/api/v5/asset/purchase_redempt'
 BILLS_INFO = '/api/v5/asset/bills'
 DEPOSIT_LIGHTNING = '/api/v5/asset/deposit-lightning'
 WITHDRAWAL_LIGHTNING = '/api/v5/asset/withdrawal-lightning'
 CANCEL_WITHDRAWAL = '/api/v5/asset/cancel-withdrawal' #need add
-WITHDRAWAL_HISTORIY = '/api/v5/asset/withdrawal-history'
+WITHDRAWAL_HISTORY = '/api/v5/asset/withdrawal-history'
 CONVERT_DUST_ASSETS = '/api/v5/asset/convert-dust-assets' #need add
 ASSET_VALUATION = '/api/v5/asset/asset-valuation' #need add
 SET_LENDING_RATE = '/api/v5/asset/set-lending-rate'
 LENDING_HISTORY = '/api/v5/asset/lending-history'
 LENDING_RATE_HISTORY = '/api/v5/asset/lending-rate-history'
 LENDING_RATE_SUMMARY = '/api/v5/asset/lending-rate-summary'
 GET_SAVING_BALANCE = '/api/v5/asset/saving-balance' #need to add
@@ -149,15 +150,15 @@
 ORDERS_HISTORY = '/api/v5/trade/orders-history'
 ORDERS_HISTORY_ARCHIVE = '/api/v5/trade/orders-history-archive'
 ORDER_FILLS = '/api/v5/trade/fills'
 ORDERS_FILLS_HISTORY = '/api/v5/trade/fills-history'
 PLACE_ALGO_ORDER = '/api/v5/trade/order-algo'
 CANCEL_ALGOS = '/api/v5/trade/cancel-algos'
 Cancel_Advance_Algos = '/api/v5/trade/cancel-advance-algos'
-ORDERS_ALGO_OENDING = '/api/v5/trade/orders-algo-pending'
+ORDERS_ALGO_PENDING = '/api/v5/trade/orders-algo-pending'
 ORDERS_ALGO_HISTORY = '/api/v5/trade/orders-algo-history'
 GET_ALGO_ORDER_DETAILS = '/api/v5/trade/order-algo'
 AMEND_ALGO_ORDER = '/api/v5/trade/amend-algos'
 
 EASY_CONVERT_CURRENCY_LIST = '/api/v5/trade/easy-convert-currency-list'
 EASY_CONVERT = '/api/v5/trade/easy-convert'
 CONVERT_EASY_HISTORY = '/api/v5/trade/easy-convert-history'
```

### Comparing `python-okx-0.2.8/okx/exceptions.py` & `python-okx-0.2.9/okx/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.8/okx/utils.py` & `python-okx-0.2.9/okx/utils.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.8/okx/websocket/WebSocketFactory.py` & `python-okx-0.2.9/okx/websocket/WebSocketFactory.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.8/okx/websocket/WsPrivateAsync.py` & `python-okx-0.2.9/okx/websocket/WsPrivateAsync.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.8/okx/websocket/WsPublicAsync.py` & `python-okx-0.2.9/okx/websocket/WsPublicAsync.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.8/okx/websocket/WsUtils.py` & `python-okx-0.2.9/okx/websocket/WsUtils.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.8/python_okx.egg-info/PKG-INFO` & `python-okx-0.2.9/python_okx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-okx
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python SDK for OKX
 Home-page: https://okx.com/docs-v5/
 Author: okxv5api
 Author-email: api@okg.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-okx-0.2.8/python_okx.egg-info/SOURCES.txt` & `python-okx-0.2.9/python_okx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.8/setup.py` & `python-okx-0.2.9/setup.py`

 * *Files identical despite different names*

