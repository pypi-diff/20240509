# Comparing `tmp/unicorn_fy-0.8.0-py3-none-any.whl.zip` & `tmp/unicorn_fy-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 11852 bytes, number of entries: 7
+Zip file size: 11915 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx       43 b- defN 21-Mar-14 16:20 unicorn_fy/__init__.py
--rw-rw-r--  2.0 unx    49942 b- defN 21-Mar-14 16:39 unicorn_fy/unicorn_fy.py
--rw-rw-r--  2.0 unx     1134 b- defN 21-Mar-14 16:39 unicorn_fy-0.8.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx    16049 b- defN 21-Mar-14 16:39 unicorn_fy-0.8.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 21-Mar-14 16:39 unicorn_fy-0.8.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 21-Mar-14 16:39 unicorn_fy-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      561 b- defN 21-Mar-14 16:39 unicorn_fy-0.8.0.dist-info/RECORD
-7 files, 67832 bytes uncompressed, 10858 bytes compressed:  84.0%
+-rw-rw-r--  2.0 unx    51134 b- defN 21-Mar-18 20:47 unicorn_fy/unicorn_fy.py
+-rw-rw-r--  2.0 unx     1134 b- defN 21-Mar-18 20:49 unicorn_fy-0.9.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    16049 b- defN 21-Mar-18 20:49 unicorn_fy-0.9.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Mar-18 20:49 unicorn_fy-0.9.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 21-Mar-18 20:49 unicorn_fy-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      561 b- defN 21-Mar-18 20:49 unicorn_fy-0.9.0.dist-info/RECORD
+7 files, 69024 bytes uncompressed, 10921 bytes compressed:  84.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: unicorn_fy/__init__.py
 Comment: 
 
 Filename: unicorn_fy/unicorn_fy.py
 Comment: 
 
-Filename: unicorn_fy-0.8.0.dist-info/LICENSE
+Filename: unicorn_fy-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: unicorn_fy-0.8.0.dist-info/METADATA
+Filename: unicorn_fy-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: unicorn_fy-0.8.0.dist-info/WHEEL
+Filename: unicorn_fy-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: unicorn_fy-0.8.0.dist-info/top_level.txt
+Filename: unicorn_fy-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: unicorn_fy-0.8.0.dist-info/RECORD
+Filename: unicorn_fy-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## unicorn_fy/unicorn_fy.py

```diff
@@ -7,15 +7,15 @@
 # Project website: https://github.com/oliver-zehentleitner/unicorn-fy
 # Documentation: https://oliver-zehentleitner.github.io/unicorn-fy
 # PyPI: https://pypi.org/project/unicorn-fy
 #
 # Author: Oliver Zehentleitner
 #         https://about.me/oliver-zehentleitner
 #
-# Copyright (c) 2019-2020, Oliver Zehentleitner
+# Copyright (c) 2019-2021, Oliver Zehentleitner
 # All rights reserved.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish, dis-
 # tribute, sublicense, and/or sell copies of the Software, and to permit
@@ -50,15 +50,15 @@
         - Binance-com-isolated_margin
         - Binance.je
         - Binance.us
         - trBinance.com
         - Binance.org
         - Jex.com
     """
-    VERSION = "0.8.0"
+    VERSION = "0.9.0"
 
     def __init__(self):
         self.last_update_check_github = {'timestamp': time.time(),
                                          'status': None}
 
     @staticmethod
     def binance_org_websocket(stream_data_json):
@@ -214,14 +214,16 @@
                 stream_data = {'data': stream_data}
             elif stream_data['e'] == 'executionReport':
                 stream_data = {'data': stream_data}
             elif stream_data['e'] == 'outboundAccountPosition':
                 stream_data = {'data': stream_data}
             elif stream_data['e'] == 'listStatus':
                 stream_data = {'data': stream_data}
+            elif stream_data['e'] == 'balanceUpdate':
+                stream_data = {'data': stream_data}
         except KeyError:
             pass
         try:
             if stream_data['stream'].find('@depth5') != -1:
                 stream_data['data']['e'] = "depth"
                 stream_data['data']['depth_level'] = 5
             elif stream_data['stream'].find('@depth10') != -1:
@@ -485,14 +487,21 @@
                                  'last_update_time': stream_data['data']['u'],
                                  'balances': []}
             for item in stream_data['data']['B']:
                 new_item = {'asset': item['a'],
                             'free': item['f'],
                             'locked': item['l']}
                 unicorn_fied_data['balances'] += [new_item]
+        elif stream_data['data']['e'] == 'balanceUpdate':
+            unicorn_fied_data = {'stream_type': '!userData@arr',
+                                 'event_type': stream_data['data']['e'],
+                                 'event_time': stream_data['data']['E'],
+                                 'asset': stream_data['data']['a'],
+                                 'balance_delta': stream_data['data']['d'],
+                                 'clear_time': stream_data['data']['T']}
         elif stream_data['data']['e'] == 'executionReport':
             unicorn_fied_data = {'stream_type': '!userData@arr',
                                  'event_type': stream_data['data']['e'],
                                  'event_time': stream_data['data']['E'],
                                  'symbol': stream_data['data']['s'],
                                  'client_order_id': stream_data['data']['c'],
                                  'side': stream_data['data']['S'],
@@ -556,14 +565,16 @@
         stream_data = json.loads(stream_data_json)
 
         try:
             if stream_data['e'] == 'outboundAccountInfo':
                 stream_data = {'data': stream_data}
             elif stream_data['e'] == 'executionReport':
                 stream_data = {'data': stream_data}
+            elif stream_data['e'] == 'balanceUpdate':
+                stream_data = {'data': stream_data}
         except KeyError:
             pass
         try:
             if stream_data['stream'].find('@depth5') != -1:
                 stream_data['data']['e'] = "depth"
                 stream_data['data']['depth_level'] = 5
             elif stream_data['stream'].find('@depth10') != -1:
@@ -794,14 +805,21 @@
                                      'can_deposit': stream_data['data']['D'],
                                      'balances': []}
                 for item in stream_data['data']['B']:
                     new_item = {'asset': item['a'],
                                 'free': item['f'],
                                 'locked': item['l']}
                     unicorn_fied_data['balances'] += [new_item]
+            elif stream_data['data']['e'] == 'balanceUpdate':
+                unicorn_fied_data = {'stream_type': '!userData@arr',
+                                 'event_type': stream_data['data']['e'],
+                                 'event_time': stream_data['data']['E'],
+                                 'asset': stream_data['data']['a'],
+                                 'balance_delta': stream_data['data']['d'],
+                                 'clear_time': stream_data['data']['T']}
             elif stream_data['data']['e'] == 'executionReport':
                 unicorn_fied_data = {'stream_type': '!userData@arr',
                                      'event_type': stream_data['data']['e'],
                                      'event_time': stream_data['data']['E'],
                                      'symbol': stream_data['data']['s'],
                                      'client_order_id': stream_data['data']['c'],
                                      'side': stream_data['data']['S'],
```

## Comparing `unicorn_fy-0.8.0.dist-info/LICENSE` & `unicorn_fy-0.9.0.dist-info/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MIT License
 ===========
 
-Copyright (c) 2019-2020 Oliver Zehentleitner (https://about.me/oliver-zehentleitner)
+Copyright (c) 2019-2021 Oliver Zehentleitner (https://about.me/oliver-zehentleitner)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `unicorn_fy-0.8.0.dist-info/METADATA` & `unicorn_fy-0.9.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicorn-fy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Convert received raw data from crypto exchange API endpoints into well-formed python dictionaries.
 Home-page: https://github.com/oliver-zehentleitner/unicorn-fy
 Author: Oliver Zehentleitner
 License: MIT License
 Project-URL: Documentation, https://oliver-zehentleitner.github.io/unicorn-fy/
 Project-URL: Wiki, https://github.com/oliver-zehentleitner/unicorn-fy/wiki
 Project-URL: Author, https://about.me/oliver-zehentleitner/
```

