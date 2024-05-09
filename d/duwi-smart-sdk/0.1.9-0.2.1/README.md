# Comparing `tmp/duwi_smart_sdk-0.1.9.tar.gz` & `tmp/duwi_smart_sdk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.1.9.tar", last modified: Thu May  9 03:20:56 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.2.1.tar", last modified: Thu May  9 05:15:48 2024, max compression
```

## Comparing `duwi_smart_sdk-0.1.9.tar` & `duwi_smart_sdk-0.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 03:20:56.880852 duwi_smart_sdk-0.1.9/
--rw-rw-rw-   0        0        0      885 2024-05-09 03:20:56.879849 duwi_smart_sdk-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-05-09 02:50:27.000000 duwi_smart_sdk-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 03:20:56.816571 duwi_smart_sdk-0.1.9/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:20:56.833221 duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     2098 2024-05-07 08:49:07.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/account.py
--rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     4346 2024-05-09 03:20:36.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2686 2024-05-07 09:08:05.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     2156 2024-05-07 08:49:07.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     4788 2024-05-07 07:31:40.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:20:56.838221 duwi_smart_sdk-0.1.9/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:20:56.839222 duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:20:56.841221 duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:20:56.858220 duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/resp/house.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:20:56.864221 duwi_smart_sdk-0.1.9/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:20:56.824570 duwi_smart_sdk-0.1.9/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      885 2024-05-09 03:20:56.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1227 2024-05-09 03:20:56.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 03:20:56.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-09 03:20:56.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-09 03:20:56.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-09 03:20:56.000000 duwi_smart_sdk-0.1.9/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 03:20:56.880852 duwi_smart_sdk-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-05-09 03:20:54.000000 duwi_smart_sdk-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:20:56.866222 duwi_smart_sdk-0.1.9/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:20:56.874847 duwi_smart_sdk-0.1.9/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.1.9/test/api/__init__.py
--rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.1.9/test/api/test_control.py
--rw-rw-rw-   0        0        0      812 2024-05-09 03:19:21.000000 duwi_smart_sdk-0.1.9/test/api/test_discover.py
--rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.1.9/test/api/test_house.py
--rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.1.9/test/api/test_login.py
--rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.1.9/test/api/test_ws.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:20:56.877848 duwi_smart_sdk-0.1.9/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.1.9/test/util/__init__.py
--rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.1.9/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.935298 duwi_smart_sdk-0.2.1/
+-rw-rw-rw-   0        0        0      885 2024-05-09 05:15:48.935298 duwi_smart_sdk-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-05-09 02:50:27.000000 duwi_smart_sdk-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.879988 duwi_smart_sdk-0.2.1/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.898480 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2098 2024-05-07 08:49:07.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/account.py
+-rw-rw-rw-   0        0        0     2784 2024-05-07 06:21:35.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4514 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2686 2024-05-07 09:08:05.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2156 2024-05-07 08:49:07.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     4788 2024-05-07 07:31:40.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.902895 duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.905404 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.907363 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.913222 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/house.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.918801 duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.888945 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      885 2024-05-09 05:15:48.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1227 2024-05-09 05:15:48.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 05:15:48.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-09 05:15:48.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-09 05:15:48.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-09 05:15:48.000000 duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 05:15:48.936400 duwi_smart_sdk-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      937 2024-05-09 05:15:42.000000 duwi_smart_sdk-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.920760 duwi_smart_sdk-0.2.1/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.927711 duwi_smart_sdk-0.2.1/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.2.1/test/api/__init__.py
+-rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.2.1/test/api/test_control.py
+-rw-rw-rw-   0        0        0      813 2024-05-09 03:37:26.000000 duwi_smart_sdk-0.2.1/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.2.1/test/api/test_house.py
+-rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.2.1/test/api/test_login.py
+-rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.2.1/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:15:48.930667 duwi_smart_sdk-0.2.1/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.1/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.2.1/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.1.9/PKG-INFO` & `duwi_smart_sdk-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.1.9
+Version: 0.2.1
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/account.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/discover.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,17 @@
             device_name=device_dict.get("deviceName", ""),
             terminal_sequence=device_dict.get("terminalSequence", ""),
             route_num=device_dict.get("routeNum", 0),
             device_type_no=device_dict.get("deviceTypeNo", ""),
             device_sub_type_no=device_dict.get("deviceSubTypeNo", ""),
             house_no=device_dict.get("houseNo", ""),
             room_no=device_dict.get("roomNo", ""),
+            room_name=device_dict.get("roomName", ""),
+            floor_no=device_dict.get("floorNo", ""),
+            floor_name=device_dict.get("floorName", ""),
             is_use=device_dict.get("isUse", False),
             is_online=device_dict.get("isOnline", False),
             create_time=device_dict.get("createTime", ""),
             seq=device_dict.get("seq", 0),
             is_favorite=device_dict.get("isFavorite", False),
             favorite_time=device_dict.get("favoriteTime", ""),
             key_binding_quantity=device_dict.get("keyBindingQuantity", 0),
```

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/const/status.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,17 @@
             device_name: str,
             terminal_sequence: str,
             route_num: int,
             device_type_no: str,
             device_sub_type_no: str,
             house_no: str,
             room_no: str,
+            room_name: str,
+            floor_no: str,
+            floor_name: str,
             is_use: bool,
             is_online: bool,
             create_time: str,
             seq: int,
             is_favorite: bool,
             favorite_time: str,
             key_binding_quantity: int,
@@ -27,14 +30,17 @@
         self.device_name: str = device_name
         self.terminal_sequence: str = terminal_sequence
         self.route_num: int = route_num
         self.device_type_no: str = device_type_no
         self.device_sub_type_no: str = device_sub_type_no
         self.house_no: str = house_no
         self.room_no: str = room_no
+        self.room_name: str = room_name
+        self.floor_no: str = floor_no
+        self.floor_name: str = floor_name
         self.is_use: bool = bool(is_use)
         self.is_online: bool = is_online
         self.create_time: datetime.datetime = self.safe_parse_datetime(create_time)
         self.seq: int = seq
         self.is_favorite: bool = bool(is_favorite)
         self.favorite_time: datetime.datetime = self.safe_parse_datetime(favorite_time)
         self.key_binding_quantity: int = key_binding_quantity
```

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi-smart-sdk
-Version: 0.1.9
+Version: 0.2.1
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.1.9/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.2.1/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/setup.py` & `duwi_smart_sdk-0.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.9'
+VERSION = '0.2.01'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.1.9/test/api/test_control.py` & `duwi_smart_sdk-0.2.1/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/test/api/test_discover.py` & `duwi_smart_sdk-0.2.1/test/api/test_discover.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,13 @@
                 app_secret="26af4883a943083a4c34083897fcea10",
                 access_token="715d1c63-85c0-4d74-9a89-5a0aa4806f74",
                 app_version="0.0.1",
                 client_version="0.0.1",
                 client_model="homeassistant",
             )
 
-            res = await cc.discover(
+            rexs = await cc.discover(
                 house_no="c7bf567d-225a-4533-ab72-5dc080b794f5",
             )
             print(res)
 
         asyncio.run(run_test())
```

### Comparing `duwi_smart_sdk-0.1.9/test/api/test_house.py` & `duwi_smart_sdk-0.2.1/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/test/api/test_login.py` & `duwi_smart_sdk-0.2.1/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/test/api/test_ws.py` & `duwi_smart_sdk-0.2.1/test/api/test_ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.1.9/test/util/test_http.py` & `duwi_smart_sdk-0.2.1/test/util/test_http.py`

 * *Files identical despite different names*

