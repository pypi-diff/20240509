# Comparing `tmp/mke_sculib-2.4.1.tar.gz` & `tmp/mke_sculib-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.4.1.tar", last modified: Thu May  2 12:36:43 2024, max compression
+gzip compressed data, was "mke_sculib-2.4.2.tar", last modified: Thu May  9 12:49:56 2024, max compression
```

## Comparing `mke_sculib-2.4.1.tar` & `mke_sculib-2.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 12:36:43.357651 mke_sculib-2.4.1/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.1/LICENSE
--rw-rw-rw-   0        0        0     4120 2024-05-02 12:36:43.357651 mke_sculib-2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.1/README.rst
--rw-rw-rw-   0        0        0      921 2024-05-02 12:36:43.363178 mke_sculib-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:36:43.286105 mke_sculib-2.4.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 12:36:43.331437 mke_sculib-2.4.1/src/mke_sculib/
--rw-rw-rw-   0        0        0      173 2024-05-02 12:34:26.000000 mke_sculib-2.4.1/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.1/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.1/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.1/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.1/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0    95276 2024-04-28 17:00:01.000000 mke_sculib-2.4.1/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.1/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.1/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:36:43.348614 mke_sculib-2.4.1/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-05-02 12:36:42.000000 mke_sculib-2.4.1/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2024-05-02 12:36:43.000000 mke_sculib-2.4.1/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 12:36:42.000000 mke_sculib-2.4.1/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 12:36:42.000000 mke_sculib-2.4.1/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 12:36:43.355652 mke_sculib-2.4.1/tests/
--rw-rw-rw-   0        0        0     9759 2023-12-05 16:11:38.000000 mke_sculib-2.4.1/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.1/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:49:56.727763 mke_sculib-2.4.2/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.2/LICENSE
+-rw-rw-rw-   0        0        0     4120 2024-05-09 12:49:56.727763 mke_sculib-2.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.2/README.rst
+-rw-rw-rw-   0        0        0      921 2024-05-09 12:49:56.729764 mke_sculib-2.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:49:56.689946 mke_sculib-2.4.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 12:49:56.715906 mke_sculib-2.4.2/src/mke_sculib/
+-rw-rw-rw-   0        0        0      718 2024-05-09 12:48:37.000000 mke_sculib-2.4.2/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.2/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.2/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.2/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.2/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0    96367 2024-05-09 12:48:51.000000 mke_sculib-2.4.2/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.2/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.2/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:49:56.722513 mke_sculib-2.4.2/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2024-05-09 12:49:56.000000 mke_sculib-2.4.2/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-05-09 12:49:56.000000 mke_sculib-2.4.2/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 12:49:56.000000 mke_sculib-2.4.2/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 12:49:56.000000 mke_sculib-2.4.2/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 12:49:56.726823 mke_sculib-2.4.2/tests/
+-rw-rw-rw-   0        0        0     9759 2023-12-05 16:11:38.000000 mke_sculib-2.4.2/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.2/tests/test_scu.py
```

### Comparing `mke_sculib-2.4.1/LICENSE` & `mke_sculib-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.1/PKG-INFO` & `mke_sculib-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.4.1
+Version: 2.4.2
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.1/README.rst` & `mke_sculib-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.1/setup.cfg` & `mke_sculib-2.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.1/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.4.2/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.1/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.4.2/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.1/src/mke_sculib/helpers.py` & `mke_sculib-2.4.2/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.1/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.4.2/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.1/src/mke_sculib/scu.py` & `mke_sculib-2.4.2/src/mke_sculib/scu.py`

 * *Files 0% similar despite different names*

```diff
@@ -2195,14 +2195,49 @@
                 continue
             except ConnectionRefusedError:
                 _log.warn('Nobody seems to listen to this endpoint. Please check the URL.')
                 _log.warn('Retrying connection in {} sec (Ctrl-C to quit)'.format(sleep_time))
                 await asyncio.sleep(sleep_time)
                 continue
 
+
+def plot_tt(t, az, el, tint, do_show=True, is_simulation=False):
+    if not 'plt' in locals():
+        import matplotlib.pyplot as plt
+
+    t_local = Time.now()
+    f, (ax1, ax2) = plt.subplots(2,1, figsize=(12,6), sharex=True)
+    ti = Time(t, format='mjd').datetime
+    # print(t)
+    # print(ti)
+    
+    ax1.plot(ti, az, 'b', label='AZ tracking curve')
+    ax2.plot(ti, el, 'g', label='EL tracking curve')
+
+    ax1.axvline(tint.datetime, label=f'Creation Time: {tint.datetime}', color='k')
+    ax2.axvline(tint.datetime, label=f'Creation Time: {tint.datetime}', color='k')
+    if not is_simulation:
+        ax1.axvline(t_local.datetime, label=f'Local Time: {t_local.datetime}', color='r')
+        ax2.axvline(t_local.datetime, label=f'Local Time: {t_local.datetime}', color='r')
+
+    ax1.set_ylabel('AZ [deg]')
+    ax2.set_ylabel('EL [deg]')
+    ax2.set_xlabel('time')
+    # ax1.set_title('Tracking Table')
+    ax1.legend()
+    ax2.legend()
+    ax1.grid()
+    ax2.grid()
+
+    if do_show:
+        plt.show()
+
+    return f, (ax1, ax2)
+        
+        
 if __name__ == '__main__':
     log("main")
 
     api = scu('http://10.96.64.10:8080/')
     channels = ['acu.azimuth.p_act', 'acu.elevation.p_act']
     
     while 1:
```

### Comparing `mke_sculib-2.4.1/src/mke_sculib/sim.py` & `mke_sculib-2.4.2/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.1/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.4.2/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.1/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.4.2/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.4.1
+Version: 2.4.2
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.1/tests/test_acu_sim.py` & `mke_sculib-2.4.2/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.1/tests/test_scu.py` & `mke_sculib-2.4.2/tests/test_scu.py`

 * *Files identical despite different names*

