# Comparing `tmp/mke_sculib-2.4.2.tar.gz` & `tmp/mke_sculib-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.4.2.tar", last modified: Thu May  9 12:49:56 2024, max compression
+gzip compressed data, was "mke_sculib-2.4.3.tar", last modified: Thu May  9 13:28:40 2024, max compression
```

## Comparing `mke_sculib-2.4.2.tar` & `mke_sculib-2.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 12:49:56.727763 mke_sculib-2.4.2/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.2/LICENSE
--rw-rw-rw-   0        0        0     4120 2024-05-09 12:49:56.727763 mke_sculib-2.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.2/README.rst
--rw-rw-rw-   0        0        0      921 2024-05-09 12:49:56.729764 mke_sculib-2.4.2/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:49:56.689946 mke_sculib-2.4.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 12:49:56.715906 mke_sculib-2.4.2/src/mke_sculib/
--rw-rw-rw-   0        0        0      718 2024-05-09 12:48:37.000000 mke_sculib-2.4.2/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.2/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.2/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.2/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.2/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0    96367 2024-05-09 12:48:51.000000 mke_sculib-2.4.2/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.2/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.2/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:49:56.722513 mke_sculib-2.4.2/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-05-09 12:49:56.000000 mke_sculib-2.4.2/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2024-05-09 12:49:56.000000 mke_sculib-2.4.2/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 12:49:56.000000 mke_sculib-2.4.2/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 12:49:56.000000 mke_sculib-2.4.2/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 12:49:56.726823 mke_sculib-2.4.2/tests/
--rw-rw-rw-   0        0        0     9759 2023-12-05 16:11:38.000000 mke_sculib-2.4.2/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.2/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:28:40.809783 mke_sculib-2.4.3/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.3/LICENSE
+-rw-rw-rw-   0        0        0     4120 2024-05-09 13:28:40.810783 mke_sculib-2.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.3/README.rst
+-rw-rw-rw-   0        0        0      921 2024-05-09 13:28:40.811784 mke_sculib-2.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:28:40.762006 mke_sculib-2.4.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 13:28:40.796299 mke_sculib-2.4.3/src/mke_sculib/
+-rw-rw-rw-   0        0        0      718 2024-05-09 13:27:55.000000 mke_sculib-2.4.3/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.3/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.3/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.3/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.3/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0    96729 2024-05-09 13:22:22.000000 mke_sculib-2.4.3/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.3/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.3/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:28:40.803781 mke_sculib-2.4.3/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2024-05-09 13:28:40.000000 mke_sculib-2.4.3/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-05-09 13:28:40.000000 mke_sculib-2.4.3/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 13:28:40.000000 mke_sculib-2.4.3/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 13:28:40.000000 mke_sculib-2.4.3/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 13:28:40.808783 mke_sculib-2.4.3/tests/
+-rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.4.3/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.3/tests/test_scu.py
```

### Comparing `mke_sculib-2.4.2/LICENSE` & `mke_sculib-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.2/PKG-INFO` & `mke_sculib-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.4.2
+Version: 2.4.3
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.2/README.rst` & `mke_sculib-2.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.2/setup.cfg` & `mke_sculib-2.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.2/src/mke_sculib/__init__.py` & `mke_sculib-2.4.3/src/mke_sculib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.4.2'
+__version__ = '2.4.3'
 
 from mke_sculib.scu import scu as scu_api, plot_tt
 from mke_sculib.sim import scu_sim
 from mke_sculib.stellarium_api import stellarium_api as stellar_api
 from mke_sculib.sim import plot_motion_pyplot as plot_motion
```

### Comparing `mke_sculib-2.4.2/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.4.3/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.2/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.4.3/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.2/src/mke_sculib/helpers.py` & `mke_sculib-2.4.3/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.2/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.4.3/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.2/src/mke_sculib/scu.py` & `mke_sculib-2.4.3/src/mke_sculib/scu.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,14 +370,17 @@
     def scu_get(self, device, params = {}):
         '''This is a generic GET command into http: scu port + folder 
         with params=payload'''
         URL = 'http://' + self.ip + ':' + self.port + device
         if device != '/devices/statusValue':
             self.call_log[datetime.datetime.utcnow()] = 'GET | ' + device
 
+        if self.debug == True:
+            log(f'request.get(**{dict(url = URL, params = params)}):')
+
         r = requests.get(url = URL, params = params)
         self._feedback(r)
         r.raise_for_status()
         if r.status_code != 200:
             log(f'Statuscode != 200. Returnded: {r.status_code}: {r.reason}', color=colors.WARNING)
 
         return r
@@ -402,14 +405,16 @@
             
         
     def scu_put(self, device, payload = {}, params = {}, data=''):
         '''This is a generic PUT command into http: scu port + folder 
         with json=payload'''
         URL = 'http://' + self.ip + ':' + self.port + device
         self.call_log[datetime.datetime.utcnow()] = 'PUT | ' + device
+        if self.debug == True:
+            log(f'request.put(**{dict(url = URL, json = payload, params = params, data = data)}):')
 
         r = requests.put(url = URL, json = payload, params = params, data = data)
         self._feedback(r)
         r.raise_for_status()
         if r.status_code != 200:
             log(f'Statuscode != 200. Returnded: {r.status_code}: {r.reason}', color=colors.WARNING)
 
@@ -419,14 +424,16 @@
         return r
 
     def scu_delete(self, device, payload = {}, params = {}):
         '''This is a generic DELETE command into http: scu port + folder 
         with params=payload'''
         URL = 'http://' + self.ip + ':' + self.port + device
         self.call_log[datetime.datetime.utcnow()] = 'DEL | ' + device
+        if self.debug == True:
+            log(f'request.delete(**{dict(url = URL, json = payload, params = params)}):')
 
         r = requests.delete(url = URL, json = payload, params = params)
         self._feedback(r)
         r.raise_for_status()
 
         if r.status_code != 200:
             log(f'Statuscode != 200. Returnded: {r.status_code}: {r.reason}', color=colors.WARNING)
```

### Comparing `mke_sculib-2.4.2/src/mke_sculib/sim.py` & `mke_sculib-2.4.3/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.2/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.4.3/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.2/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.4.3/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.4.2
+Version: 2.4.3
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.2/tests/test_acu_sim.py` & `mke_sculib-2.4.3/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.2/tests/test_scu.py` & `mke_sculib-2.4.3/tests/test_scu.py`

 * *Files identical despite different names*

