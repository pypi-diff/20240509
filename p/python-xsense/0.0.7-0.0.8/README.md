# Comparing `tmp/python-xsense-0.0.7.tar.gz` & `tmp/python-xsense-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-xsense-0.0.7.tar", last modified: Sun May  5 18:08:07 2024, max compression
+gzip compressed data, was "python-xsense-0.0.8.tar", last modified: Thu May  9 19:54:14 2024, max compression
```

## Comparing `python-xsense-0.0.7.tar` & `python-xsense-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-05 18:08:07.297141 python-xsense-0.0.7/
--rw-r--r--   0 theo       (501) staff       (20)     1859 2024-05-05 18:08:07.296582 python-xsense-0.0.7/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)     1226 2024-04-18 18:45:42.000000 python-xsense-0.0.7/README.rst
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-05 18:08:07.295924 python-xsense-0.0.7/python_xsense.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)     1859 2024-05-05 18:08:07.000000 python-xsense-0.0.7/python_xsense.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      421 2024-05-05 18:08:07.000000 python-xsense-0.0.7/python_xsense.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2024-05-05 18:08:07.000000 python-xsense-0.0.7/python_xsense.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)       51 2024-05-05 18:08:07.000000 python-xsense-0.0.7/python_xsense.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)        7 2024-05-05 18:08:07.000000 python-xsense-0.0.7/python_xsense.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)       38 2024-05-05 18:08:07.297275 python-xsense-0.0.7/setup.cfg
--rw-r--r--   0 theo       (501) staff       (20)      911 2024-05-05 18:07:38.000000 python-xsense-0.0.7/setup.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-05 18:08:07.290475 python-xsense-0.0.7/xsense/
--rw-r--r--   0 theo       (501) staff       (20)      147 2024-02-20 08:37:03.000000 python-xsense-0.0.7/xsense/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     7086 2024-05-05 18:07:31.000000 python-xsense-0.0.7/xsense/async_xsense.py
--rw-r--r--   0 theo       (501) staff       (20)     3745 2024-05-05 17:48:22.000000 python-xsense-0.0.7/xsense/aws_signer.py
--rw-r--r--   0 theo       (501) staff       (20)     7201 2024-05-05 17:49:04.000000 python-xsense-0.0.7/xsense/base.py
--rw-r--r--   0 theo       (501) staff       (20)      387 2024-05-05 17:46:03.000000 python-xsense-0.0.7/xsense/device.py
--rw-r--r--   0 theo       (501) staff       (20)      801 2024-05-05 17:49:04.000000 python-xsense-0.0.7/xsense/entity.py
--rw-r--r--   0 theo       (501) staff       (20)      214 2024-05-05 17:49:04.000000 python-xsense-0.0.7/xsense/exceptions.py
--rw-r--r--   0 theo       (501) staff       (20)     1163 2024-05-05 17:49:04.000000 python-xsense-0.0.7/xsense/house.py
--rw-r--r--   0 theo       (501) staff       (20)     1114 2024-05-05 17:49:04.000000 python-xsense-0.0.7/xsense/mapping.py
--rw-r--r--   0 theo       (501) staff       (20)     1204 2024-05-05 17:49:04.000000 python-xsense-0.0.7/xsense/station.py
--rw-r--r--   0 theo       (501) staff       (20)     1411 2024-05-05 17:46:39.000000 python-xsense-0.0.7/xsense/utils.py
--rw-r--r--   0 theo       (501) staff       (20)     5972 2024-05-05 17:49:04.000000 python-xsense-0.0.7/xsense/xsense.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-09 19:54:14.340784 python-xsense-0.0.8/
+-rw-r--r--   0 theo       (501) staff       (20)     1859 2024-05-09 19:54:14.339751 python-xsense-0.0.8/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)     1226 2024-04-18 18:45:42.000000 python-xsense-0.0.8/README.rst
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-09 19:54:14.338553 python-xsense-0.0.8/python_xsense.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)     1859 2024-05-09 19:54:14.000000 python-xsense-0.0.8/python_xsense.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      421 2024-05-09 19:54:14.000000 python-xsense-0.0.8/python_xsense.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2024-05-09 19:54:14.000000 python-xsense-0.0.8/python_xsense.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)       51 2024-05-09 19:54:14.000000 python-xsense-0.0.8/python_xsense.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)        7 2024-05-09 19:54:14.000000 python-xsense-0.0.8/python_xsense.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)       38 2024-05-09 19:54:14.340859 python-xsense-0.0.8/setup.cfg
+-rw-r--r--   0 theo       (501) staff       (20)      911 2024-05-09 19:53:59.000000 python-xsense-0.0.8/setup.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-05-09 19:54:14.335515 python-xsense-0.0.8/xsense/
+-rw-r--r--   0 theo       (501) staff       (20)      147 2024-02-20 08:37:03.000000 python-xsense-0.0.8/xsense/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     7274 2024-05-09 19:53:50.000000 python-xsense-0.0.8/xsense/async_xsense.py
+-rw-r--r--   0 theo       (501) staff       (20)     3745 2024-05-09 19:49:56.000000 python-xsense-0.0.8/xsense/aws_signer.py
+-rw-r--r--   0 theo       (501) staff       (20)     7305 2024-05-09 19:53:50.000000 python-xsense-0.0.8/xsense/base.py
+-rw-r--r--   0 theo       (501) staff       (20)      387 2024-05-05 17:46:03.000000 python-xsense-0.0.8/xsense/device.py
+-rw-r--r--   0 theo       (501) staff       (20)      801 2024-05-05 17:49:04.000000 python-xsense-0.0.8/xsense/entity.py
+-rw-r--r--   0 theo       (501) staff       (20)      214 2024-05-05 17:49:04.000000 python-xsense-0.0.8/xsense/exceptions.py
+-rw-r--r--   0 theo       (501) staff       (20)     1163 2024-05-05 17:49:04.000000 python-xsense-0.0.8/xsense/house.py
+-rw-r--r--   0 theo       (501) staff       (20)     1114 2024-05-05 17:49:04.000000 python-xsense-0.0.8/xsense/mapping.py
+-rw-r--r--   0 theo       (501) staff       (20)     1204 2024-05-05 17:49:04.000000 python-xsense-0.0.8/xsense/station.py
+-rw-r--r--   0 theo       (501) staff       (20)     1411 2024-05-05 17:46:39.000000 python-xsense-0.0.8/xsense/utils.py
+-rw-r--r--   0 theo       (501) staff       (20)     6173 2024-05-09 19:53:59.000000 python-xsense-0.0.8/xsense/xsense.py
```

### Comparing `python-xsense-0.0.7/PKG-INFO` & `python-xsense-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-xsense
-Version: 0.0.7
+Version: 0.0.8
 Summary: XSense Python Module
 Home-page: https://github.com/theosnel/python-xsense
 Author: Theo Snelleman
 Author-email: <python@theo.snelleman.net>
 License: MIT
 Keywords: python,xsense
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-xsense-0.0.7/README.rst` & `python-xsense-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.7/python_xsense.egg-info/PKG-INFO` & `python-xsense-0.0.8/python_xsense.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-xsense
-Version: 0.0.7
+Version: 0.0.8
 Summary: XSense Python Module
 Home-page: https://github.com/theosnel/python-xsense
 Author: Theo Snelleman
 Author-email: <python@theo.snelleman.net>
 License: MIT
 Keywords: python,xsense
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-xsense-0.0.7/setup.py` & `python-xsense-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'XSense Python Module'
 
 with open('README.rst', 'r') as fd:
     LONG_DESCRIPTION = fd.read()
 
 setup(
     name='python-xsense',
```

### Comparing `python-xsense-0.0.7/xsense/async_xsense.py` & `python-xsense-0.0.8/xsense/async_xsense.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,30 +164,38 @@
         params = {
             'houseId': houseId,
             'utctimestamp': "0"
         }
         return await self.api_call("103007", **params)
 
     async def get_house_state(self, house: House):
-        res = await self.get_house(house, 'mainpage')
-        if self._lastres.status == 404:
-            raise NotFoundError(await self._lastres.text())
+        for page in ('mainpage', '2nd_mainpage'):
+            res = await self.get_house(house, page)
 
-        if 'reported' in res.get('state', {}):
-            self._parse_get_house_state(house, res['state']['reported'])
-        else:
-            text = await self._lastres.text()
-            raise APIFailure(f'Unable to retrieve house data: {self._lastres.status}/{text}')
+            if self._lastres.status == 404:
+                continue
+
+            if 'reported' in res.get('state', {}):
+                self._parse_get_house_state(house, res['state']['reported'])
+            else:
+                text = await self._lastres.text()
+                raise APIFailure(f'Unable to retrieve house data: {self._lastres.status}/{text}')
 
     async def get_station_state(self, station: Station):
-        if station.type == 'SBS50':
-            res = await self.get_thing(station, f'2nd_info_{station.sn}')
-        else:
+        res = None
+
+        if station.type not in ('SBS50', 'SC07-WX', 'XC04-WX'):
             res = await self.get_thing(station, f'info_{station.sn}')
 
+        if res is None or self._lastres.status == 404:
+            res = await self.get_thing(station, f'2nd_info_{station.sn}')
+
+        if self._lastres.status == 404:
+            return
+
         if 'reported' in res.get('state', {}):
             station.set_data(res['state']['reported'])
         else:
             text = await self._lastres.text()
             raise APIFailure(f'Unable to retrieve station data: {self._lastres.status}/{text}')
 
     async def get_state(self, station: Station):
```

### Comparing `python-xsense-0.0.7/xsense/aws_signer.py` & `python-xsense-0.0.8/xsense/aws_signer.py`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.7/xsense/base.py` & `python-xsense-0.0.8/xsense/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,20 @@
     def _thing_request(self, station: Station, page: str):
         headers = {
             'Content-Type': 'application/x-amz-json-1.0',
             'User-Agent': 'aws-sdk-iOS/2.26.5 iOS/17.3 nl_NL',
             'X-Amz-Security-Token': self.aws_session_token
         }
 
+        typename = station.type
+        if typename in ('XC04-WX', 'SC07-WX'):
+            typename += '-'
+
         host = f'{station.house.mqtt_region}.x-sense-iot.com'
-        uri = f'/things/{station.type}{station.sn}/shadow?name={page}'
+        uri = f'/things/{typename}{station.sn}/shadow?name={page}'
 
         url = f'https://{host}{uri}'
 
         signed = self.signer.sign_headers('GET', url, station.house.mqtt_region, headers, None)
         headers |= signed
 
         return url, headers
```

### Comparing `python-xsense-0.0.7/xsense/entity.py` & `python-xsense-0.0.8/xsense/entity.py`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.7/xsense/house.py` & `python-xsense-0.0.8/xsense/house.py`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.7/xsense/mapping.py` & `python-xsense-0.0.8/xsense/mapping.py`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.7/xsense/station.py` & `python-xsense-0.0.8/xsense/station.py`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.7/xsense/utils.py` & `python-xsense-0.0.8/xsense/utils.py`

 * *Files identical despite different names*

### Comparing `python-xsense-0.0.7/xsense/xsense.py` & `python-xsense-0.0.8/xsense/xsense.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,29 +149,36 @@
         params = {
             'houseId': houseId,
             'utctimestamp': "0"
         }
         return self.api_call("103007", **params)
 
     def get_house_state(self, house: House):
-        res = self.get_house(house, 'mainpage')
-        if self._lastres.status_code == 404:
-            raise NotFoundError(self._lastres.text)
+        for page in ('mainpage', '2nd_mainpage'):
+            res = self.get_house(house, page)
 
-        if 'reported' in res.get('state', {}):
-            self._parse_get_house_state(house, res['state']['reported'])
-        else:
-            raise APIFailure(f'Unable to retrieve station data: {self._lastres.status_code}/{self._lastres.text}')
+            if self._lastres.status_code == 404:
+                continue
+
+            if 'reported' in res.get('state', {}):
+                self._parse_get_house_state(house, res['state']['reported'])
+            else:
+                raise APIFailure(f'Unable to retrieve station data: {self._lastres.status_code}/{self._lastres.text}')
 
     def get_station_state(self, station: Station):
-        if station.type == 'SBS50':
-            res = self.get_thing(station, f'2nd_info_{station.sn}')
-        else:
+        res = None
+        if station.type not in ('SBS50', 'SC07-WX', 'XC04-WX'):
             res = self.get_thing(station, f'info_{station.sn}')
 
+        if res is None or self._lastres.status_code == 404:
+            res = self.get_thing(station, f'2nd_info_{station.sn}')
+
+        if self._lastres.status_code == 404:
+            return
+
         if 'reported' in res.get('state', {}):
             station.set_data(res['state']['reported'])
         else:
             raise APIFailure(f'Unable to retrieve station data: {self._lastres.status_code}/{self._lastres.text}')
 
     def get_state(self, station: Station):
         if not station.devices:
```

