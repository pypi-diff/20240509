# Comparing `tmp/PKNSETools-0.1.20240506.99.tar.gz` & `tmp/PKNSETools-0.1.20240508.100.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240506.99.tar", last modified: Mon May  6 19:22:39 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240508.100.tar", last modified: Wed May  8 22:40:49 2024, max compression
```

## Comparing `PKNSETools-0.1.20240506.99.tar` & `PKNSETools-0.1.20240508.100.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 19:22:39.053507 PKNSETools-0.1.20240506.99/
--rw-rw-rw-   0        0        0     2661 2024-05-06 19:22:39.053507 PKNSETools-0.1.20240506.99/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 19:22:39.037879 PKNSETools-0.1.20240506.99/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-05-06 19:22:39.053507 PKNSETools-0.1.20240506.99/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 19:22:39.053507 PKNSETools-0.1.20240506.99/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3386 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10032 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2223 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0     5168 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0    13763 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       30 2024-05-06 19:22:34.000000 PKNSETools-0.1.20240506.99/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 19:22:39.053507 PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61961 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29916 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 19:22:39.053507 PKNSETools-0.1.20240506.99/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2661 2024-05-06 19:22:39.000000 PKNSETools-0.1.20240506.99/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2024-05-06 19:22:39.000000 PKNSETools-0.1.20240506.99/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 19:22:39.000000 PKNSETools-0.1.20240506.99/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 19:22:32.000000 PKNSETools-0.1.20240506.99/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-05-06 19:22:39.000000 PKNSETools-0.1.20240506.99/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-06 19:22:39.000000 PKNSETools-0.1.20240506.99/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/README.md
--rw-rw-rw-   0        0        0       86 2024-05-06 19:22:39.053507 PKNSETools-0.1.20240506.99/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-05-06 19:20:25.000000 PKNSETools-0.1.20240506.99/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:40:49.471512 PKNSETools-0.1.20240508.100/
+-rw-rw-rw-   0        0        0     2663 2024-05-08 22:40:49.471512 PKNSETools-0.1.20240508.100/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-08 22:40:49.455889 PKNSETools-0.1.20240508.100/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-05-08 22:40:49.455889 PKNSETools-0.1.20240508.100/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:40:49.455889 PKNSETools-0.1.20240508.100/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3386 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10770 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2635 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0     8640 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0    13763 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       31 2024-05-08 22:40:44.000000 PKNSETools-0.1.20240508.100/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:40:49.471512 PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61961 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29916 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:40:49.455889 PKNSETools-0.1.20240508.100/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2663 2024-05-08 22:40:49.000000 PKNSETools-0.1.20240508.100/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2024-05-08 22:40:49.000000 PKNSETools-0.1.20240508.100/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 22:40:49.000000 PKNSETools-0.1.20240508.100/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-08 22:40:42.000000 PKNSETools-0.1.20240508.100/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-05-08 22:40:49.000000 PKNSETools-0.1.20240508.100/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 22:40:49.000000 PKNSETools-0.1.20240508.100/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-08 22:40:49.471512 PKNSETools-0.1.20240508.100/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-05-08 22:39:30.000000 PKNSETools-0.1.20240508.100/setup.py
```

### Comparing `PKNSETools-0.1.20240506.99/PKG-INFO` & `PKNSETools-0.1.20240508.100/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240506.99
+Version: 0.1.20240508.100
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240506.99.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240508.100.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240508.100/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240508.100/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240508.100/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240508.100/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240508.100/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240508.100/PKNSETools/PKCompanyGeneral.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     SOFTWARE.
 
 """
 import json
 from collections import namedtuple
 
 import requests
-
+# from PKDevTools.classes.CookieHelper import CookieHelper
+# from PKDevTools.classes import Archiver
 from PKNSETools.PKConstants import (_autoComplete_url_path, _base_domain,
                                     _head, _quote_url_path)
 
 session = requests.session()
 
 def _get_Tuple_From_JSON(companyDict):
     return namedtuple('X', companyDict.keys())(*companyDict.values())
@@ -115,19 +116,17 @@
     # "sitemap":[
         
     # ]
     # }  
     search_result = json.loads(str(search_results.json()).replace("'","\""), object_hook=_get_Tuple_From_JSON)
     return search_result
 
-def get_Company_Details_By_Name(name):
-    search_results = get_Search_Results_By_Name(name)
-    search_result = search_results.symbols[0].symbol
+def download(symbol):
     get_details = f'{_base_domain}{_quote_url_path}'
-    company_details = session.get(url=get_details.format(search_result), headers=_head)
+    company_details = session.get(url=get_details.format(symbol), headers=_head)
     text = str(company_details.json()).replace("'","\"").replace('True','true').replace('False','false').replace('None','null')
     # '{"info": {
     #       "symbol": "SBIN", 
     #       "companyName": "State Bank of India", 
     #       "industry": "BANKS", 
     #       "activeSeries": ["EQ"], 
     #       "debtSeries": [], 
@@ -196,8 +195,22 @@
     #                   "totalSellQuantity": 603729, 
     #                   "atoBuyQty": 10667, 
     #                   "atoSellQty": 1621}
     # }'
     companyDetails = json.loads(text, object_hook=_get_Tuple_From_JSON)
     return companyDetails
 
-# print(get_Id_By_Name('SBIN'))
+def get_Company_Details_By_Name(name):
+    search_results = get_Search_Results_By_Name(name)
+    symbol = search_results.symbols[0].symbol
+    return download(symbol)
+    
+# def refreshNSECookies():
+#     cookieHelper = CookieHelper(download_folder=Archiver.get_user_outputs_dir(),
+#                                                  baseCookieUrl="https://www.barodaetrade.com/Markettracker/Dividend_Declared",
+#                                                  cookieStoreName="bcaps",
+#                                                  baseHtmlUrl="https://www.barodaetrade.com/Markettracker/Dividend_Declared",
+#                                                  htmlStoreName="bcaps")
+#     session.cookies.update(cookieHelper.cookies)
+
+# refreshNSECookies()
+# print(download('SBIN'))
```

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240508.100/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240508.100/PKNSETools/PKConstants.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 
 """
 from PKDevTools.classes.Utils import random_user_agent
 
 _base_domain = 'https://www.nseindia.com'
 _autoComplete_url_path = '/api/search/autocomplete?q={}'
 _quote_url_path= '/api/quote-equity?symbol={}'
+# Board meetings, corporate actions, financial results, latest announcements, shareholding patterns, 
+# https://www.nseindia.com/api/top-corp-info?symbol=SBIN&market=equities
+
+# Bulk block deals, market dept order book/bid/ask, security wise DP
+_quote_url_path_trade_info = f"{_quote_url_path}&section=trade_info&series=EQ"
+
+# Equity meta data
+# https://www.nseindia.com/api/equity-meta-info?symbol=SBIN
 _daily_report_url_path = '/api/merged-daily-reports?key=favCapital'
 _quote_url_path_html = '/get-quotes/equity?symbol={}'
 _historical_company_data_url_path_html = '/api/historical/cm/equity?symbol={}'
 _historical_company_data_url_path = '/api/historical/cm/equity?symbol={}&series=[%22EQ%22]&from={}&to={}&csv=true'
 _historical_index_data_url_path = '/api/historical/indicesHistory?indexType={}&from={}&to={}'
 _chart_data_preopen_url = '/api/chart-databyindex?index={}&preopen=true'
 _chart_data_open_url = '/api/chart-databyindex?index={}'
```

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240508.100/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240508.100/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240508.100/PKNSETools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240506.99
+Version: 0.1.20240508.100
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240506.99.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240508.100.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240506.99/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240508.100/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/README.md` & `PKNSETools-0.1.20240508.100/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.99/setup.py` & `PKNSETools-0.1.20240508.100/setup.py`

 * *Files identical despite different names*

