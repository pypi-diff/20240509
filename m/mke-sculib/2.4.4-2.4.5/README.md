# Comparing `tmp/mke_sculib-2.4.4.tar.gz` & `tmp/mke_sculib-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.4.4.tar", last modified: Thu May  9 13:49:02 2024, max compression
+gzip compressed data, was "mke_sculib-2.4.5.tar", last modified: Thu May  9 14:14:31 2024, max compression
```

## Comparing `mke_sculib-2.4.4.tar` & `mke_sculib-2.4.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 13:49:02.286417 mke_sculib-2.4.4/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.4/LICENSE
--rw-rw-rw-   0        0        0     4120 2024-05-09 13:49:02.287418 mke_sculib-2.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.4/README.rst
--rw-rw-rw-   0        0        0      921 2024-05-09 13:49:02.288421 mke_sculib-2.4.4/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:49:02.190153 mke_sculib-2.4.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 13:49:02.271867 mke_sculib-2.4.4/src/mke_sculib/
--rw-rw-rw-   0        0        0      718 2024-05-09 13:48:44.000000 mke_sculib-2.4.4/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.4/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.4/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.4/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.4/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0    96875 2024-05-09 13:48:47.000000 mke_sculib-2.4.4/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.4/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.4/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:49:02.279030 mke_sculib-2.4.4/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-05-09 13:49:01.000000 mke_sculib-2.4.4/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2024-05-09 13:49:02.000000 mke_sculib-2.4.4/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 13:49:01.000000 mke_sculib-2.4.4/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 13:49:01.000000 mke_sculib-2.4.4/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 13:49:02.285417 mke_sculib-2.4.4/tests/
--rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.4.4/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.4/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:14:31.376759 mke_sculib-2.4.5/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.5/LICENSE
+-rw-rw-rw-   0        0        0     4120 2024-05-09 14:14:31.377758 mke_sculib-2.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.5/README.rst
+-rw-rw-rw-   0        0        0      921 2024-05-09 14:14:31.385239 mke_sculib-2.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:14:31.322040 mke_sculib-2.4.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 14:14:31.364023 mke_sculib-2.4.5/src/mke_sculib/
+-rw-rw-rw-   0        0        0      718 2024-05-09 13:58:07.000000 mke_sculib-2.4.5/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.5/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.5/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.5/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.5/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0    97177 2024-05-09 14:14:07.000000 mke_sculib-2.4.5/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.5/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.5/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:14:31.371431 mke_sculib-2.4.5/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2024-05-09 14:14:31.000000 mke_sculib-2.4.5/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-05-09 14:14:31.000000 mke_sculib-2.4.5/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 14:14:31.000000 mke_sculib-2.4.5/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 14:14:31.000000 mke_sculib-2.4.5/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 14:14:31.375759 mke_sculib-2.4.5/tests/
+-rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.4.5/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.5/tests/test_scu.py
```

### Comparing `mke_sculib-2.4.4/LICENSE` & `mke_sculib-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.4/PKG-INFO` & `mke_sculib-2.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.4.4
+Version: 2.4.5
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.4/README.rst` & `mke_sculib-2.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.4/setup.cfg` & `mke_sculib-2.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.4/src/mke_sculib/__init__.py` & `mke_sculib-2.4.5/src/mke_sculib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.4.4'
+__version__ = '2.4.5'
 
 from mke_sculib.scu import scu as scu_api, plot_tt
 from mke_sculib.sim import scu_sim
 from mke_sculib.stellarium_api import stellarium_api as stellar_api
 from mke_sculib.sim import plot_motion_pyplot as plot_motion
```

### Comparing `mke_sculib-2.4.4/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.4.5/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.4/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.4.5/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.4/src/mke_sculib/helpers.py` & `mke_sculib-2.4.5/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.4/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.4.5/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.4/src/mke_sculib/scu.py` & `mke_sculib-2.4.5/src/mke_sculib/scu.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     """A SCU interface object, which connects to a SCU controller by OHB Digital Connect GmbH
     for the SKA-MPI Demonstrator Radio Telescope in the Karroo Desert in South Africa as well
     as the MeerKAT Extension Radio telescopes. 
     
     This class can be used to communicate with and control of the Antennas control unit via 
     HTTP rest API.
     """
-    def __init__(self, address='', ip='', port='8080', debug=False, lims_az=(-270.0, 270, 3.0), lims_el=(15, 90, 1.35), dish_type='mke', post_put_delay=0.0):
+    def __init__(self, address='', ip='', port='8080', debug=False, lims_az=(-270.0, 270, 3.0), lims_el=(15, 90, 1.35), dish_type='mke', post_put_delay=0.2):
         """create an SCU object, which can be used to communicate with 
         and control of the Antennas control unit via HTTP rest API.
 
         Args:
             ip (str, optional): ip address of the antenna to connect to. Defaults to 'localhost'.
             port (str, optional): port of the antenna to connect to. Defaults to '8080'.
             debug (bool, optional): Set to True, to receive additional information in stdout, when using commands. Defaults to True.
@@ -295,15 +295,15 @@
         param_name_map = [re.match(r"^[Pp][0-9]+", k) for k in self.spem_keys]
         param_name_map = {m.group().upper():k for m, k in zip(param_name_map, self.spem_keys)}
         return param_name_map
     
     @property
     def stow_pos(self):
         az = 0.0 if self.dish_type == 'mke' else -90.0
-        el = 88.75
+        el = 89.75
         return az, el
 
     @property
     def band_in_focus(self):
         return self.status_finalValue('acu.general_management_and_controller.feed_indexer_pos')
 
     @property
@@ -909,18 +909,20 @@
 
     def stow(self, pre_move=True):
         """stow the antenna on pos 1 (both axes) and wait for stowing to be completed
         """
         log('Stowing...')
         if pre_move:
             self.abs_azel(*self.stow_pos)
+            self.wait_duration(0.5)
             self.wait_settle()
 
         if self.dish_type == 'mke':
             self.scu_put("/devices/command", {"path": "acu.azimuth.drive_to_stow", "params":{"action": "1"}})
+            self.wait_duration(1.0)
             self.scu_put("/devices/command", {"path": "acu.elevation.drive_to_stow", "params":{"action": "1"}})
         else:
             self.scu_put("/devices/command", {"path": "acu.dish_management_controller.stow", "params": {"action": "1"}})
 
         self.wait_duration(3, no_stout=True)
         self.wait_state("acu.stow_pin_controller.azimuth_status", "LOCKED", operator='<=')
         self.wait_state("acu.stow_pin_controller.elevation_status", "LOCKED", operator='<=')
@@ -1933,24 +1935,25 @@
 
         return df
 
 
 
         
 
-    def start(self, az_start=None, el_start=None, band_start=None, az_speed=None, el_speed=None, send_default_configs=False):
+    def start(self, az_start=None, el_start=None, band_start=None, az_speed=None, el_speed=None, send_default_configs=False, reset_after_start=True):
         """getting command authority, unstow, activate and start the antenna for usage
 
         Args:
             az_start (-270 <= az_start <= 270, optional): start position for AZ axis in degree. Defaults to None.
             el_start (15 <= el_start <= 90, optional): start position for EL axis in degree. Defaults to None.
             band_start (str or int, optional): start position ('Band 1'... 'Band 5c' or 1...7) for the Feed Indexer Axis to move to. Defaults to None.
             az_speed (0 < az_speed <= 3.0, optional): azimuth speed to use for movement to inital position. None means as fast as possible. Defaults to None.
             el_speed (0 < el_speed <= 1.0, optional): elevation speed to use for movement to inital position None means as fast as possible. Defaults to None.
             send_default_configs (bool, optional): Whether or not to generate the default logging configs on the SCU on startup. Defaults to True.
+            reset_after_start(bool, optional): Whether or not to generate send another "reset" after the whole startup routine. Defaults to True.
         """
         log('=== INITIATING STARTUP ROUTINE ===', color=colors.BOLD)
         self.t_start = Time.now()
         self.get_command_authority()
         self.wait_duration(0.1)
         if self.dish_type == 'mke':
             self.deactivate_lowpowermode()
@@ -1968,15 +1971,17 @@
                     log(f'Creating Default Config: {k} with n={len(v)} channels')
                     self.create_logger(k, v)
         
         self.wait_duration(5)
         self.activate_dmc()
         self.wait_duration(5)
         self.activate_axes()
-        self.wait_duration(5)
+        self.wait_duration(3)
+        self.reset_dmc()
+        self.wait_duration(2)
 
         if band_start is not None:
             self.move_to_band(band_start)
 
         if az_start is not None:
             self.abs_azimuth(az_start, az_speed)
         if el_start is not None:
```

### Comparing `mke_sculib-2.4.4/src/mke_sculib/sim.py` & `mke_sculib-2.4.5/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.4/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.4.5/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.4/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.4.5/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.4.4
+Version: 2.4.5
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.4/tests/test_acu_sim.py` & `mke_sculib-2.4.5/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.4/tests/test_scu.py` & `mke_sculib-2.4.5/tests/test_scu.py`

 * *Files identical despite different names*

