# Comparing `tmp/mke_sculib-2.4.5.tar.gz` & `tmp/mke_sculib-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.4.5.tar", last modified: Thu May  9 14:14:31 2024, max compression
+gzip compressed data, was "mke_sculib-2.4.6.tar", last modified: Thu May  9 20:03:39 2024, max compression
```

## Comparing `mke_sculib-2.4.5.tar` & `mke_sculib-2.4.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 14:14:31.376759 mke_sculib-2.4.5/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.5/LICENSE
--rw-rw-rw-   0        0        0     4120 2024-05-09 14:14:31.377758 mke_sculib-2.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.5/README.rst
--rw-rw-rw-   0        0        0      921 2024-05-09 14:14:31.385239 mke_sculib-2.4.5/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:14:31.322040 mke_sculib-2.4.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:14:31.364023 mke_sculib-2.4.5/src/mke_sculib/
--rw-rw-rw-   0        0        0      718 2024-05-09 13:58:07.000000 mke_sculib-2.4.5/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.5/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.5/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.5/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.5/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0    97177 2024-05-09 14:14:07.000000 mke_sculib-2.4.5/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.5/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.5/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:14:31.371431 mke_sculib-2.4.5/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-05-09 14:14:31.000000 mke_sculib-2.4.5/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2024-05-09 14:14:31.000000 mke_sculib-2.4.5/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 14:14:31.000000 mke_sculib-2.4.5/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 14:14:31.000000 mke_sculib-2.4.5/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 14:14:31.375759 mke_sculib-2.4.5/tests/
--rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.4.5/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.5/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:03:39.467004 mke_sculib-2.4.6/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.6/LICENSE
+-rw-rw-rw-   0        0        0     4120 2024-05-09 20:03:39.467004 mke_sculib-2.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.6/README.rst
+-rw-rw-rw-   0        0        0      921 2024-05-09 20:03:39.468008 mke_sculib-2.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:03:39.443365 mke_sculib-2.4.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 20:03:39.461689 mke_sculib-2.4.6/src/mke_sculib/
+-rw-rw-rw-   0        0        0      718 2024-05-09 20:03:26.000000 mke_sculib-2.4.6/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.6/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.6/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.6/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0     9874 2024-05-09 20:02:32.000000 mke_sculib-2.4.6/src/mke_sculib/js_helpers.py
+-rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.6/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0    97732 2024-05-09 20:02:39.000000 mke_sculib-2.4.6/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.6/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.6/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:03:39.464688 mke_sculib-2.4.6/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2024-05-09 20:03:39.000000 mke_sculib-2.4.6/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2024-05-09 20:03:39.000000 mke_sculib-2.4.6/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 20:03:39.000000 mke_sculib-2.4.6/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 20:03:39.000000 mke_sculib-2.4.6/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 20:03:39.465689 mke_sculib-2.4.6/tests/
+-rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.4.6/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.6/tests/test_scu.py
```

### Comparing `mke_sculib-2.4.5/LICENSE` & `mke_sculib-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.5/PKG-INFO` & `mke_sculib-2.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.4.5
+Version: 2.4.6
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.5/README.rst` & `mke_sculib-2.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.5/setup.cfg` & `mke_sculib-2.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.5/src/mke_sculib/__init__.py` & `mke_sculib-2.4.6/src/mke_sculib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.4.5'
+__version__ = '2.4.6'
 
 from mke_sculib.scu import scu as scu_api, plot_tt
 from mke_sculib.sim import scu_sim
 from mke_sculib.stellarium_api import stellarium_api as stellar_api
 from mke_sculib.sim import plot_motion_pyplot as plot_motion
```

### Comparing `mke_sculib-2.4.5/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.4.6/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.5/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.4.6/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.5/src/mke_sculib/helpers.py` & `mke_sculib-2.4.6/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.5/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.4.6/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.5/src/mke_sculib/scu.py` & `mke_sculib-2.4.6/src/mke_sculib/scu.py`

 * *Files 1% similar despite different names*

```diff
@@ -2211,14 +2211,27 @@
                 has_err = True
                 continue
             except ConnectionRefusedError:
                 _log.warn('Nobody seems to listen to this endpoint. Please check the URL.')
                 _log.warn('Retrying connection in {} sec (Ctrl-C to quit)'.format(sleep_time))
                 await asyncio.sleep(sleep_time)
                 continue
+    
+    def show_liveplot(self, channels:list=None):
+        try:
+            get_ipython().__class__.__name__
+            from IPython.display import display, HTML
+            from js_helpers import make_livepos_page, make_liveplot_page
+            if not channels:
+                return HTML(make_livepos_page(self.ip, port = self.port))
+            else:
+                return HTML(make_liveplot_page(self.ip, channels, port = self.port))
+        except NameError as err:
+            raise EnvironmentError('Not running in Ipython!') 
+
 
 
 def plot_tt(t, az, el, tint, do_show=True, is_simulation=False):
     if not 'plt' in locals():
         import matplotlib.pyplot as plt
 
     t_local = Time.now()
```

### Comparing `mke_sculib-2.4.5/src/mke_sculib/sim.py` & `mke_sculib-2.4.6/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.5/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.4.6/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.5/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.4.6/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.4.5
+Version: 2.4.6
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.5/tests/test_acu_sim.py` & `mke_sculib-2.4.6/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.5/tests/test_scu.py` & `mke_sculib-2.4.6/tests/test_scu.py`

 * *Files identical despite different names*

