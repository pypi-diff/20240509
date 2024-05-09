# Comparing `tmp/nanonisTCP-1.0.2.tar.gz` & `tmp/nanonistcp-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanonisTCP-1.0.2.tar", last modified: Tue Mar 19 07:15:52 2024, max compression
+gzip compressed data, was "nanonistcp-1.1.2.tar", last modified: Thu May  9 09:56:09 2024, max compression
```

## Comparing `nanonisTCP-1.0.2.tar` & `nanonistcp-1.1.2.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 07:15:52.983389 nanonisTCP-1.0.2/
--rw-rw-rw-   0        0        0     1094 2022-05-29 00:32:05.000000 nanonisTCP-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1841 2024-03-19 07:15:52.980389 nanonisTCP-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1391 2022-12-09 10:27:56.000000 nanonisTCP-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 07:15:52.959389 nanonisTCP-1.0.2/nanonisTCP/
--rw-rw-rw-   0        0        0     1759 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/AutoApproach.py
--rw-rw-rw-   0        0        0     1342 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/AutoApproachTest.py
--rw-rw-rw-   0        0        0     6169 2023-01-20 01:16:03.000000 nanonisTCP-1.0.2/nanonisTCP/Bias.py
--rw-rw-rw-   0        0        0    34979 2022-10-14 01:45:57.000000 nanonisTCP-1.0.2/nanonisTCP/BiasSpectr.py
--rw-rw-rw-   0        0        0     6387 2022-10-14 01:51:14.000000 nanonisTCP-1.0.2/nanonisTCP/BiasSpectrTest.py
--rw-rw-rw-   0        0        0     2227 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/BiasTest.py
--rw-rw-rw-   0        0        0     5040 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/Current.py
--rw-rw-rw-   0        0        0     2167 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/CurrentTest.py
--rw-rw-rw-   0        0        0     6727 2022-05-29 00:09:29.000000 nanonisTCP-1.0.2/nanonisTCP/FolMe.py
--rw-rw-rw-   0        0        0     2832 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/FolMeTest.py
--rw-rw-rw-   0        0        0    32175 2022-10-18 22:26:38.000000 nanonisTCP-1.0.2/nanonisTCP/LockIn.py
--rw-rw-rw-   0        0        0     8294 2022-10-18 22:26:38.000000 nanonisTCP-1.0.2/nanonisTCP/LockInTest.py
--rw-rw-rw-   0        0        0     3888 2022-10-21 07:54:06.000000 nanonisTCP-1.0.2/nanonisTCP/Marks.py
--rw-rw-rw-   0        0        0     1856 2022-10-21 07:54:14.000000 nanonisTCP-1.0.2/nanonisTCP/MarksTest.py
--rw-rw-rw-   0        0        0     8010 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/Motor.py
--rw-rw-rw-   0        0        0     3275 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/MotorTest.py
--rw-rw-rw-   0        0        0    12317 2023-01-20 04:10:36.000000 nanonisTCP-1.0.2/nanonisTCP/Osci2T.py
--rw-rw-rw-   0        0        0     3171 2023-01-20 04:52:32.000000 nanonisTCP-1.0.2/nanonisTCP/Osci2TTest.py
--rw-rw-rw-   0        0        0    21689 2023-08-14 03:50:09.000000 nanonisTCP-1.0.2/nanonisTCP/Pattern.py
--rw-rw-rw-   0        0        0     6014 2022-06-15 07:48:03.000000 nanonisTCP-1.0.2/nanonisTCP/Piezo.py
--rw-rw-rw-   0        0        0     2230 2022-06-15 07:27:12.000000 nanonisTCP-1.0.2/nanonisTCP/PiezoTest.py
--rw-rw-rw-   0        0        0     4603 2022-05-29 00:09:29.000000 nanonisTCP-1.0.2/nanonisTCP/SafeTip.py
--rw-rw-rw-   0        0        0     2093 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/SafeTipTest.py
--rw-rw-rw-   0        0        0    19720 2022-05-29 00:09:29.000000 nanonisTCP-1.0.2/nanonisTCP/Scan.py
--rw-rw-rw-   0        0        0     5179 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/ScanTest.py
--rw-rw-rw-   0        0        0     8380 2022-05-30 04:36:09.000000 nanonisTCP-1.0.2/nanonisTCP/Signals.py
--rw-rw-rw-   0        0        0     2677 2022-05-30 04:38:31.000000 nanonisTCP-1.0.2/nanonisTCP/SignalsTest.py
--rw-rw-rw-   0        0        0     9312 2023-03-02 21:35:28.000000 nanonisTCP-1.0.2/nanonisTCP/TipShaper.py
--rw-rw-rw-   0        0        0     2312 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/TipShaperTest.py
--rw-rw-rw-   0        0        0    12739 2024-02-27 21:50:55.000000 nanonisTCP-1.0.2/nanonisTCP/UserOut.py
--rw-rw-rw-   0        0        0     3170 2024-02-27 21:57:55.000000 nanonisTCP-1.0.2/nanonisTCP/UserOutTest.py
--rw-rw-rw-   0        0        0    17174 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/ZController.py
--rw-rw-rw-   0        0        0     5533 2022-05-30 02:33:38.000000 nanonisTCP-1.0.2/nanonisTCP/ZControllerTest.py
--rw-rw-rw-   0        0        0       27 2022-05-29 00:32:05.000000 nanonisTCP-1.0.2/nanonisTCP/__init__.py
--rw-rw-rw-   0        0        0     6769 2024-03-11 05:45:49.000000 nanonisTCP-1.0.2/nanonisTCP/nanonisTCP.py
-drwxrwxrwx   0        0        0        0 2024-03-19 07:15:52.978390 nanonisTCP-1.0.2/nanonisTCP.egg-info/
--rw-rw-rw-   0        0        0     1841 2024-03-19 07:15:52.000000 nanonisTCP-1.0.2/nanonisTCP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-03-19 07:15:52.000000 nanonisTCP-1.0.2/nanonisTCP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 07:15:52.000000 nanonisTCP-1.0.2/nanonisTCP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-03-19 07:15:52.000000 nanonisTCP-1.0.2/nanonisTCP.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 07:15:52.000000 nanonisTCP-1.0.2/nanonisTCP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 07:15:52.983389 nanonisTCP-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-03-19 07:15:02.000000 nanonisTCP-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:56:09.951360 nanonistcp-1.1.2/
+-rw-rw-rw-   0        0        0     1094 2022-05-29 00:32:05.000000 nanonistcp-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2397 2024-05-09 09:56:09.951360 nanonistcp-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1947 2024-05-09 02:27:59.000000 nanonistcp-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 09:56:09.821389 nanonistcp-1.1.2/nanonisTCP/
+-rw-rw-rw-   0        0        0     1759 2022-05-30 02:33:38.000000 nanonistcp-1.1.2/nanonisTCP/AutoApproach.py
+-rw-rw-rw-   0        0        0     6169 2023-01-20 01:16:03.000000 nanonistcp-1.1.2/nanonisTCP/Bias.py
+-rw-rw-rw-   0        0        0    41438 2024-05-08 08:46:10.000000 nanonistcp-1.1.2/nanonisTCP/BiasSpectr.py
+-rw-rw-rw-   0        0        0     6640 2024-05-08 22:27:34.000000 nanonistcp-1.1.2/nanonisTCP/Current.py
+-rw-rw-rw-   0        0        0     6727 2022-05-29 00:09:29.000000 nanonistcp-1.1.2/nanonisTCP/FolMe.py
+-rw-rw-rw-   0        0        0    32175 2022-10-18 22:26:38.000000 nanonistcp-1.1.2/nanonisTCP/LockIn.py
+-rw-rw-rw-   0        0        0     3888 2022-10-21 07:54:06.000000 nanonistcp-1.1.2/nanonisTCP/Marks.py
+-rw-rw-rw-   0        0        0     8010 2022-05-30 02:33:38.000000 nanonistcp-1.1.2/nanonisTCP/Motor.py
+-rw-rw-rw-   0        0        0    12317 2023-01-20 04:10:36.000000 nanonistcp-1.1.2/nanonisTCP/Osci2T.py
+-rw-rw-rw-   0        0        0    21689 2024-04-16 09:45:04.000000 nanonistcp-1.1.2/nanonisTCP/Pattern.py
+-rw-rw-rw-   0        0        0     9916 2024-05-09 01:42:10.000000 nanonistcp-1.1.2/nanonisTCP/Piezo.py
+-rw-rw-rw-   0        0        0     4603 2022-05-29 00:09:29.000000 nanonistcp-1.1.2/nanonisTCP/SafeTip.py
+-rw-rw-rw-   0        0        0    20892 2024-05-08 08:16:12.000000 nanonistcp-1.1.2/nanonisTCP/Scan.py
+-rw-rw-rw-   0        0        0     8380 2022-05-30 04:36:09.000000 nanonistcp-1.1.2/nanonisTCP/Signals.py
+-rw-rw-rw-   0        0        0     9312 2023-03-02 21:35:28.000000 nanonistcp-1.1.2/nanonisTCP/TipShaper.py
+-rw-rw-rw-   0        0        0    12739 2024-02-27 21:50:55.000000 nanonistcp-1.1.2/nanonisTCP/UserOut.py
+-rw-rw-rw-   0        0        0    17174 2022-05-30 02:33:38.000000 nanonistcp-1.1.2/nanonisTCP/ZController.py
+-rw-rw-rw-   0        0        0       27 2022-05-29 00:32:05.000000 nanonistcp-1.1.2/nanonisTCP/__init__.py
+-rw-rw-rw-   0        0        0     6989 2024-05-09 02:24:33.000000 nanonistcp-1.1.2/nanonisTCP/nanonisTCP.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:56:09.941365 nanonistcp-1.1.2/nanonisTCP/test/
+-rw-rw-rw-   0        0        0     1493 2024-05-09 09:52:41.000000 nanonistcp-1.1.2/nanonisTCP/test/AutoApproachTest.py
+-rw-rw-rw-   0        0        0     6916 2024-05-09 09:52:41.000000 nanonistcp-1.1.2/nanonisTCP/test/BiasSpectrTest.py
+-rw-rw-rw-   0        0        0     2422 2024-05-09 09:52:41.000000 nanonistcp-1.1.2/nanonisTCP/test/BiasTest.py
+-rw-rw-rw-   0        0        0     2377 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/CurrentTest.py
+-rw-rw-rw-   0        0        0     3014 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/FolMeTest.py
+-rw-rw-rw-   0        0        0     8850 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/LockInTest.py
+-rw-rw-rw-   0        0        0     1640 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/MarksTest.py
+-rw-rw-rw-   0        0        0     3044 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/MotorTest.py
+-rw-rw-rw-   0        0        0     3366 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/Osci2TTest.py
+-rw-rw-rw-   0        0        0     2616 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/PiezoTest.py
+-rw-rw-rw-   0        0        0     2308 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/SafeTipTest.py
+-rw-rw-rw-   0        0        0     5545 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/ScanTest.py
+-rw-rw-rw-   0        0        0     3060 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/SignalsTest.py
+-rw-rw-rw-   0        0        0     2493 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/TipShaperTest.py
+-rw-rw-rw-   0        0        0     3405 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/UserOutTest.py
+-rw-rw-rw-   0        0        0     6045 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/ZControllerTest.py
+-rw-rw-rw-   0        0        0       27 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/__init__.py
+-rw-rw-rw-   0        0        0     4544 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/nanonisTCP/test/test.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:56:09.941365 nanonistcp-1.1.2/nanonisTCP.egg-info/
+-rw-rw-rw-   0        0        0     2397 2024-05-09 09:56:09.000000 nanonistcp-1.1.2/nanonisTCP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1161 2024-05-09 09:56:09.000000 nanonistcp-1.1.2/nanonisTCP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 09:56:09.000000 nanonistcp-1.1.2/nanonisTCP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-09 09:56:09.000000 nanonistcp-1.1.2/nanonisTCP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 09:56:09.000000 nanonistcp-1.1.2/nanonisTCP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 09:56:09.951360 nanonistcp-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-05-09 09:52:42.000000 nanonistcp-1.1.2/setup.py
```

### Comparing `nanonisTCP-1.0.2/LICENSE` & `nanonistcp-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/PKG-INFO` & `nanonistcp-1.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanonisTCP
-Version: 1.0.2
+Version: 1.1.2
 Summary: python module for communicating via nanonis TCP protocal
 Home-page: https://github.com/New-Horizons-SPM/nanonisTCP
 Author: Julian Ceddia
 Author-email: jdceddia@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/New-Horizons-SPM/nanonisTCP/issues
 Description-Content-Type: text/markdown
@@ -14,38 +14,45 @@
 
 [![DOI](https://zenodo.org/badge/475187257.svg)](https://zenodo.org/badge/latestdoi/475187257)
 # nanonisTCP
 Python module for communicating to nanonis via TCP. I am actively developing this so if you have any requests or find any bugs, feel free to raise an issue.
 
 ### Installing
 
-Clone this repository, navigate to said directory, and run:
-```
-pip install .
-```
+Install with pip:
+```pip install nanonisTCP```
+
+Installing from source:
+Clone the repository, navigate to the root directory and run ```pip install .```
 
 ### Using
 
 The following code demonstrates how to change tip bias.
 
 ```python
 from nanonisTCP import nanonisTCP
 from nanonisTCP.Bias import Bias
 
-TCP_IP  = '127.0.0.1'               # Local host
-TCP_PORT= 6501                      # Check available ports in NANONIS > File > Settings Options > TCP Programming Interface
+TCP_IP  = '127.0.0.1'                               # Local host
+TCP_PORT= 6501                                      # Check available ports in NANONIS > File > Settings Options > TCP Programming Interface
 
-NTCP = nanonisTCP(TCP_IP, TCP_PORT) # This is how you establish a TCP connection. NTCP is the connection handle.
+NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=13520)  # This is how you establish a TCP connection. NTCP is the connection handle.
+                                                    # Check your nanonis version in Nanonis > help > info and enter the RT Engine number
 
-bias = Bias(NTCP)                   # Nanonis Bias Module - Pass in the connection handle
+bias = Bias(NTCP)                                   # Nanonis Bias Module - Pass in the connection handle
 
-bias.Set(1.1)                       # Set bias to 1.1 V
-v = bias.Get()                      # Get the current bias
-print("Bias: " + str(v) + " V")     # Confirm bias has been set
+bias.Set(1.1)                                       # Set bias to 1.1 V
+v = bias.Get()                                      # Get the current bias
+print("Bias: " + str(v) + " V")                     # Confirm bias has been set
 
-NTCP.close_connection()             # Close the connection.
+NTCP.close_connection()                             # Close the connection.
 ```
 
-See any of the xxxTest.py scripts to see how each module can be implemented in more detail
+See any of the xxxTest.py scripts to see how each module can be implemented in more detail.
+
+### Testing
+After installing, you can test any of the modules using the sctipts in the test folder.
+To test all of the modules, run test.py
+<strong>Note that Nanonis must be open for the tests to pass.</strong>
 
 ### Citing
 If you use nanonisTCP, please consider citing it: [10.5281/zenodo.7402664](https://doi.org/10.5281/zenodo.7402664)
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/AutoApproach.py` & `nanonistcp-1.1.2/nanonisTCP/AutoApproach.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/AutoApproachTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/AutoApproachTest.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,36 +9,41 @@
 !!!WARNING: RUNNING run_test() WILL AUTO APPROACH YOUR TIP. RUN IT ON A SIM!!!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 
 
 from nanonisTCP import nanonisTCP
 from nanonisTCP.AutoApproach import AutoApproach
+import time
 
 """
 Set up the TCP connection and interface
 """
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6502, make_plot=False):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6502, make_plot=False, debug=False, version=13520):
     
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                         # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                        # Nanonis TCP interface
     
     autoApp = AutoApproach(NTCP)                                                # Nanonis Auto Approach Module
     
     try:
         """
         Open
         """
         autoApp.Open()
+        time.sleep(1)
         
         """
         On/Off Set/Get
         """
         autoApp.OnOffSet(on_off=True)
         on_off = autoApp.OnOffGet()
-        print("Auto Approach On/Off")
-        print("Status: " + ["Off","Running"][on_off])
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Auto Approach On/Off")
+            print("Status: " + ["Off","Running"][on_off])
+            print("----------------------------------------------------------------------")
     except Exception as e:
-        print(e)
+        NTCP.close_connection()
+        return e
     
-    NTCP.close_connection()
+    NTCP.close_connection()
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/Bias.py` & `nanonistcp-1.1.2/nanonisTCP/Bias.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/BiasSpectr.py` & `nanonistcp-1.1.2/nanonisTCP/BiasSpectr.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 class BiasSpectr:
     """
     Nanonis Bias Spectroscopy Module
     """
     def __init__(self,NanonisTCP):
         self.NanonisTCP = NanonisTCP
+        self.version = NanonisTCP.version
         
     def Open(self):
         """
         Opens the Bias Spectroscopy Module
 
         """
         ## Make Header
@@ -141,24 +142,33 @@
         
         status = self.NanonisTCP.hex_to_int32(response[0:4])
         
         return status
         
     def ChsSet(self,channel_indexes,mode="set"):
         """
-        Sets/adds/removes the list of recortded channels in Bias Spectroscopy
+        Sets/adds/removes the list of recorded channels in Bias Spectroscopy
 
         Parameters
         ----------
-        channel_indexes : channel indexes to set, add, or remove. The indexes 
+        channel_indexes : Nanonis v < R11798, use slot number:
+                          channel indexes to set, add, or remove. The indexes 
                           are comprised between 0 and 23 for the 24 signals 
                           assigned in the Signals Manager. To get the signal 
                           name and its corresponding index in the list of 128 
                           available signals in the Nanonis Controller, use 
                           the Signals.InSlotsGet function
+
+                          Nanonis v >= R11798, use RT Index:
+                          indexes of recorded channels. The index is comprised between 0
+                          and 127, and it corresponds to the full list of signals available in the system.
+                          To get the signal name and its corresponding index in the list of the 128 available signals in the Nanonis
+                          Controller, use the Signal.NamesGet function, or check the RT Idx value in the Signals Manager module.
+
+
         mode            : "set"    : channel_indexes will become the entire 
                                      list of selected channels
                           "add"    : channel_indexes will be added to the list 
                                      of selected channels
                           "remove" : remove channel_indexes from list of 
                                      selected channels
 
@@ -190,14 +200,18 @@
             hex_rep += self.NanonisTCP.to_hex(index,4)
         
         self.NanonisTCP.send_command(hex_rep)
         
         self.NanonisTCP.receive_response(0)
         
     def ChsGet(self):
+        if(self.version  < 11798): return self.ChsGet_v0()
+        if(self.version >= 11798): return self.ChsGet_v1()
+
+    def ChsGet_v0(self):
         """
         Returns the list of recorded channels in Bias Spectroscopy
 
         Returns
         -------
         channel_indexes : The indexes of recorded channels. The indexes are 
                           comprised between 0 and 23 for the 24 signals 
@@ -219,14 +233,61 @@
         channel_indexes = []
         for i in range(number_of_channels):
             channel_index = self.NanonisTCP.hex_to_int32(response[idx:idx+4])
             channel_indexes.append(channel_index)
             idx += 4
         
         return channel_indexes
+    
+    def ChsGet_v1(self):
+        """
+        Returns the list of recorded channels in Bias Spectroscopy
+
+        Returns
+        -------
+        channel_indexes :  The index is comprised between 0
+                           and 127, and it corresponds to the 
+                           full list of signals available in 
+                           the system. To get the signal name
+                           and its corresponding index in the
+                           list of the 128 available signals
+                           in the Nanonis Controller, use the 
+                           Signal.NamesGet function, or check 
+                           the RT Idx value in the Signals 
+                           Manager module.
+        channel_names   :  Returns the names of the acquired
+                           channels in the sweep
+
+        """
+        hex_rep = self.NanonisTCP.make_header('BiasSpectr.ChsGet', body_size=0)
+        
+        self.NanonisTCP.send_command(hex_rep)
+        
+        response = self.NanonisTCP.receive_response()
+        
+        number_of_channels = self.NanonisTCP.hex_to_int32(response[0:4])
+        
+        idx = 4
+        channel_indexes = []
+        for i in range(number_of_channels):
+            channel_index = self.NanonisTCP.hex_to_int32(response[idx:idx+4])
+            channel_indexes.append(channel_index)
+            idx += 4
+        
+        # channels_size = self.NanonisTCP.hex_to_int32(response[12:16])         # Useless
+        idx += 4
+        channels_names = []
+        num_channels = len(channel_indexes)
+        for channel in range(num_channels):
+            channel_size = self.NanonisTCP.hex_to_int32(response[idx:idx+4])
+            idx += 4
+            channels_names.append(response[idx:idx+channel_size].decode())
+            idx += channel_size
+
+        return channel_indexes, channels_names
         
     def PropsSet(self,save_all=0,num_sweeps=0,back_sweep=0,num_points=0,z_offset=0,autosave=0,save_dialog=0):
         """
         Configures the Bias Spectroscopy parameters
 
         Returns
         -------
@@ -270,16 +331,20 @@
         hex_rep += self.NanonisTCP.to_hex(autosave,2)
         hex_rep += self.NanonisTCP.to_hex(save_dialog,2)
         
         
         self.NanonisTCP.send_command(hex_rep)
         
         self.NanonisTCP.receive_response(0)
-        
+    
     def PropsGet(self):
+        if(self.version  < 11798): return self.PropsGet_v0()
+        if(self.version >= 11798): return self.PropsGet_v1()
+        
+    def PropsGet_v0(self):
         """
         Returns the Bias Spectroscopy parameters
 
         Returns
         -------
         save_all : 1 : data from individual sweeps is saved, along with 
                        averaged data.
@@ -346,14 +411,91 @@
                 "num_sweeps"  : num_sweeps,
                 "back_sweep"  : back_sweep,
                 "num_points"  : num_points,
                 "channels"    : channels,
                 "parameters"  : parameters,
                 "fixed_parameters" : fixed_parameters}
     
+    def PropsGet_v1(self):
+        """
+        Returns the Bias Spectroscopy parameters
+
+        Returns
+        -------
+        save_all : 1 : data from individual sweeps is saved, along with 
+                       averaged data.
+                   0 : Individual sweeps are not saved, only the average of 
+                       all of them is saved. This parameter only makes sense 
+                       when multiple sweeps are configured.
+        num_sweeps : Number of sweeps to measure and average. 0 means no change
+        back_sweep : Selects whether a backward sweep is acquired in addition 
+                     to the forward sweep (which is always acquired)
+                     0 : Don't acquire a backward sweep.
+                     1 : Acquire a backward sweep (in addition to the forward)
+        num_points : Defines the number of points to acquire over the sweep
+                     range. 0 means no change
+        parameters : Returns the parameters of the sweep
+        fixed_parameters : Returns the fixed parameters of the sweep
+        autosave    : Selects whether to automatically save the data to ASCII
+                      file once the sweep is done.
+                      0 : Autosave off
+                      1 : Autosave on
+        save_dialog : Selects whether to show the save dialog box once the 
+                      sweep is done
+                      0 : Don't show
+                      1 : Show
+        
+        """
+        hex_rep = self.NanonisTCP.make_header('BiasSpectr.PropsGet', body_size=0)
+        
+        self.NanonisTCP.send_command(hex_rep)
+        
+        response = self.NanonisTCP.receive_response()
+        
+        save_all   = self.NanonisTCP.hex_to_int16(response[0:2])
+        num_sweeps = self.NanonisTCP.hex_to_int32(response[2:6])
+        back_sweep = self.NanonisTCP.hex_to_int16(response[6:8])
+        num_points = self.NanonisTCP.hex_to_int32(response[8:12])
+        idx = 12
+
+        # parameters_size = self.NanonisTCP.hex_to_int32(response[idx:idx+4])   # Useless
+
+        idx += 4
+        parameters = []
+        num_parameters  = self.NanonisTCP.hex_to_int32(response[idx:idx+4])
+        idx += 4
+        for parameter in range(num_parameters):
+            parameter_size = self.NanonisTCP.hex_to_int32(response[idx:idx+4])
+            idx += 4
+            parameters.append(response[idx:idx+parameter_size].decode())
+            idx += parameter_size
+            
+        # fixed_parameters_size = self.NanonisTCP.hex_to_int32(response[idx:idx+4]) # Useless
+        idx += 4
+        fixed_parameters = []
+        num_fixed_parameters  = self.NanonisTCP.hex_to_int32(response[idx:idx+4])
+        idx += 4
+        for fixed_parameter in range(num_fixed_parameters):
+            fixed_parameter_size = self.NanonisTCP.hex_to_int32(response[idx:idx+4])
+            idx += 4
+            fixed_parameters.append(response[idx:idx+fixed_parameter_size].decode())
+            idx += fixed_parameter_size
+        
+        autosave    = self.NanonisTCP.hex_to_int16(response[idx:idx+4]); idx += 4
+        save_dialog = self.NanonisTCP.hex_to_int16(response[idx:idx+4]); idx += 4
+
+        return {"save_all"    : save_all,
+                "num_sweeps"  : num_sweeps,
+                "back_sweep"  : back_sweep,
+                "num_points"  : num_points,
+                "parameters"  : parameters,
+                "fixed_parameters" : fixed_parameters,
+                "autosave"    : autosave,
+                "save_dialog" : save_dialog}
+    
     def AdvPropsSet(self,reset_bias=0,z_controller_hold=0,record_final_z=0,lockin_run=0):
         """
         Sets parameters from the advanced configuration section of the bias 
         spectroscopy module.
 
         Parameters
         ----------
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/BiasSpectrTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/BiasSpectrTest.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,147 +8,166 @@
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !WARNING: RUNNING run_test() WILL CHANGE SETTINGS IN NANONIS. RUN IT ON A SIM!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 
 from nanonisTCP import nanonisTCP
 from nanonisTCP.BiasSpectr import BiasSpectr
-import traceback
 import numpy as np
+import time
+import traceback
 
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, plot_data=0):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, plot_data=0, debug=False, version=13520):
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                         # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                        # Nanonis TCP interface
     try:
         bspec = BiasSpectr(NTCP)                                                # Nanonis TCP Bias Spectroscopy Module
         
         """
         Open
         """
         bspec.Open()
-        print("Bias Spectroscopy module open")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Bias Spectroscopy module open")
+            print("----------------------------------------------------------------------")
+        time.sleep(0.5)
         
         """
         Start
         """
         data = bspec.Start(get_data=1,save_base_name="NTCP-Test-")
         data_dict  = data['data_dict']
         parameters = data['parameters']
         if(plot_data):
             import matplotlib.pyplot as plt
             plt.plot(data_dict['Bias calc (V)'],data_dict['Current (A)'])
-        print("data channels: " + str(data_dict.keys()))
-        print("parameters:    " + str(parameters))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("data channels: " + str(data_dict.keys()))
+            print("parameters:    " + str(parameters))
+            print("----------------------------------------------------------------------")
         
         """
         Stop
         """
         # Cannot test the Stop function like below... the reason is nanonis 
         # server side sends a response back over the initiating port and cannot
         # receive another instruction (i.e. Stop) until the data acquisition is
         # complete (even if get_data=0). This means if you want to start an 
         # acquisition and then stop it before it finishes, you must send the 
         # Stop command on a separate port.
         
         # bspec.Start(get_data=0,save_base_name="NTCP-Test-Stop-")              # Can't do this to test. must be started and stopped on separate ports
         
         bspec.Stop()
-        print("Acquisition stopped")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Acquisition stopped")
+            print("----------------------------------------------------------------------")
         
         """
         Status Get
         """
         status = bspec.StatusGet()
-        print("Status: " + ["Not running","Running"][status])
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Status: " + ["Not running","Running"][status])
+            print("----------------------------------------------------------------------")
         
         """
         ChsSet/Get
         """
-        channel_indexes = [0,14,16]
+        channel_indexes = [0,30]
+        if(version < 11798): channel_indexes = [0,14]
         bspec.ChsSet(channel_indexes=channel_indexes,mode="set")
         channel_indexes = bspec.ChsGet()
-        print("channels : " + str(channel_indexes))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("channels : " + str(channel_indexes))
+            print("----------------------------------------------------------------------")
         
         """
         Props Set/Get
         """
         bspec.PropsSet(save_all=1,num_sweeps=20,back_sweep=0,num_points=200,z_offset=10e-12,autosave=0,save_dialog=2)
         propsDict = bspec.PropsGet()
-        print("Properties:\n" + str(propsDict))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Properties:\n" + str(propsDict))
+            print("----------------------------------------------------------------------")
         
         """
         AdvPropsSet/Get
         """
         bspec.AdvPropsSet(reset_bias=0,z_controller_hold=0,record_final_z=0,lockin_run=0)
         advancedProps = bspec.AdvPropsGet()
-        print("Advanced Properties:\n" + str(advancedProps))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Advanced Properties:\n" + str(advancedProps))
+            print("----------------------------------------------------------------------")
         
         """
         LimitsSet/Get
         """
         bspec.LimitsSet(start_value=-1.1,end_value=1.1)
         limits = bspec.LimitsGet()
-        print("Spec limits:\n" + str(limits))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Spec limits:\n" + str(limits))
+            print("----------------------------------------------------------------------")
         
         """
         TimingSet/Get
         """
         # Note: minimum times are 50us. anything lower than this will either 
         # round up to 50us or down to 0s
         bspec.TimingSet(z_averaging_time=51e-5,z_offset=1.2e-9,initial_settling_time=370e-6,maximum_slew_rate=np.inf,settling_time=12e-6,integration_time=57e-6,end_settling_time=91e-6,z_control_time=61e-6)
         timing = bspec.TimingGet()
-        print("Spec Timing:\n" + str(timing))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Spec Timing:\n" + str(timing))
+            print("----------------------------------------------------------------------")
         
         """
         AltZCtrlSet/Get
         """
         bspec.AltZCtrlSet(alternate_setpoint_onoff=1,setpoint=22e-12,settling_time=60e-3)
         altZParams = bspec.AltZCtrlGet()
-        print("Spec AltZParams:\n" + str(altZParams))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Spec AltZParams:\n" + str(altZParams))
+            print("----------------------------------------------------------------------")
         
         """
         MLSLockinPerSegSet/Get and MLSModeSet/Get
         """
         # This test will fail if sweep mode is not explicitly set to 
         # Multi Segment first.
         bspec.MLSModeSet(sweep_mode="MLS")
         sweep_mode = bspec.MLSModeGet()
-        print("Sweep mode: " + sweep_mode)
+        if(debug):
+            print("Sweep mode: " + sweep_mode)
+
         bspec.MLSLockinPerSegSet(lockin_per_segment=0)
         lockin_per_segment = bspec.MLSLockinPerSegGet()
-        print("Spec lockin per segment: " + ["off","on"][lockin_per_segment])
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Spec lockin per segment: " + ["off","on"][lockin_per_segment])
+            print("----------------------------------------------------------------------")
         
         """
         MLSValsSet/Get
         """
         bias_start = [-2,-1]
         bias_end   = [1,2]
         initial_settling_time = [10e-3,12e-3]
         settling_time = [14e-3,16e-3]
         integration_time = [18e-3,20e-3]
         steps = [10,20]
         lockin_run=[0,0]
         bspec.MLSValsSet(bias_start,bias_end,initial_settling_time,settling_time,integration_time,steps,lockin_run)
         mlsVals = bspec.MLSValsGet()
-        print("MLS Values:\n" + str(mlsVals))
-        print("Setting sweep mode back to Linear...")
+        if(debug):
+            print("MLS Values:\n" + str(mlsVals))
+            print("Setting sweep mode back to Linear...")
         bspec.MLSModeSet(sweep_mode="Linear")
         sweep_mode = bspec.MLSModeGet()
-        print("Sweep mode: " + sweep_mode)
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Sweep mode: " + sweep_mode)
+            print("----------------------------------------------------------------------")
     except:
-        print(traceback.format_exc())
-        
+        NTCP.close_connection()
+        return(traceback.format_exc())
+    
     NTCP.close_connection()
-    return print('end of test')
-        
+    return "success"
+
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/BiasTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/BiasTest.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,55 +10,61 @@
 !WARNING: RUNNING run_test() WILL CHANGE SETTINGS IN NANONIS. RUN IT ON A SIM!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 
 
 from nanonisTCP import nanonisTCP
 from nanonisTCP.Bias import Bias
+import traceback
 
 """
 Set up the TCP connection and interface
 """
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, debug=True, version=13520):
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                             # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                                # Nanonis TCP interface
     try:
 
         """
         Bias Set/Get
         """
         bias = Bias(NTCP)                                                               # Nanonis Bias Module
 
         bias.Set(5)                                                                     # Set bias to 5 V
         v = bias.Get()                                                                  # Get the current bias
-        print("Bias Get")
-        print("Bias: " + str(v) + " V")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Bias Get")
+            print("Bias: " + str(v) + " V")
+            print("----------------------------------------------------------------------")
 
         """
         Range Set/Get
         """
         bias.RangeSet(0)
         bias_ranges, bias_range_index = bias.RangeGet()
-        print("Bias Range")
-        print("Ranges:      " + str(bias_ranges))
-        print("Range index: " + str(bias_range_index))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Bias Range")
+            print("Ranges:      " + str(bias_ranges))
+            print("Range index: " + str(bias_range_index))
+            print("----------------------------------------------------------------------")
 
         """
         Calibration Set/Get
         """
         bias.CalibrSet(calibration=2, offset=-0.1)
         calibration,offset = bias.CalibrGet()
-        print("Calibration")
-        print("Calibration: " + str(calibration))
-        print("Offset:      " + str(offset))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Calibration")
+            print("Calibration: " + str(calibration))
+            print("Offset:      " + str(offset))
+            print("----------------------------------------------------------------------")
 
         """
         Pulse
         """
         bias.Pulse(0.25, -3,z_hold=1,rel_abs=1,wait_until_done=True)
     except:
-        print('error')
+        NTCP.close_connection()
+        return(traceback.format_exc())
+    
     NTCP.close_connection()
-    return print('end of test')
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/Current.py` & `nanonistcp-1.1.2/nanonisTCP/Current.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 class Current:
     """
     Nanonis Current Module
     """
     def __init__(self,NanonisTCP):
         self.NanonisTCP = NanonisTCP
+        self.version = NanonisTCP.version
     
     def Get(self):
         """
         Returns the tunnelling current value
 
         Returns
         -------
@@ -69,15 +70,31 @@
         
         response = self.NanonisTCP.receive_response(4)
         
         currentBEEM = self.NanonisTCP.hex_to_float32(response[0:4])
         
         return currentBEEM
     
-    def GainSet(self,gain_index):
+    def GainSet(self,gain_index,filter_index=-1):
+        """
+        Sets the gain of the current amplifier
+
+        Parameters
+        ----------
+        gain_index : The index out of the list of gains which can be retrieved
+                     by the function Current.GainsGet
+        filter_index : Nanonis version > 11798 only
+                       The index out of the list of filters which can be retrieved by the function
+                       Current.GainsGet. This is the list of filters available for the Basel PI SP 983c preamplifier. If the
+                       preamplifier in use is not this one or we don’t want to change this parameter, -1 should be used.
+        """
+        if(self.version  < 11798): return self.GainSet_v0(gain_index)
+        if(self.version >= 11798): return self.GainSet_v1(gain_index,filter_index)
+        
+    def GainSet_v0(self,gain_index):
         """
         Sets the gain of the current amplifier
 
         Parameters
         ----------
         gain_index : The index out of the list of gains which can be retrieved
                      by the function Current.GainsGet
@@ -88,14 +105,35 @@
         
         ## Arguments
         hex_rep += self.NanonisTCP.to_hex(gain_index,2)
         
         self.NanonisTCP.send_command(hex_rep)
         
         self.NanonisTCP.receive_response(0)
+           
+    def GainSet_v1(self,gain_index, filter_index=-1):
+        """
+        Sets the gain of the current amplifier
+
+        Parameters
+        ----------
+        gain_index : The index out of the list of gains which can be retrieved
+                     by the function Current.GainsGet
+
+        """
+        ## Make Header
+        hex_rep = self.NanonisTCP.make_header('Current.GainSet', body_size=8)
+        
+        ## Arguments
+        hex_rep += self.NanonisTCP.to_hex(gain_index,4)
+        hex_rep += self.NanonisTCP.to_hex(filter_index,4)
+        
+        self.NanonisTCP.send_command(hex_rep)
+        
+        self.NanonisTCP.receive_response(0)
     
     def GainsGet(self):
         """
         Returns the selectable gains of the current amplifier and the index of 
         the selected one
 
         Returns
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/CurrentTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/CurrentTest.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,51 +8,58 @@
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !WARNING: RUNNING run_test() WILL CHANGE SETTINGS IN NANONIS. RUN IT ON A SIM!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 
 from nanonisTCP import nanonisTCP
 from nanonisTCP.Current import Current
+import traceback
 
 """
 Set up the TCP connection and interface
 """
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, debug=False, version=13520):
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                         # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                        # Nanonis TCP interface
     try:
         currentModule = Current(NTCP)                                           # Nanonis TCP Current Module
         
         """
         Current Get
         """
         current     = currentModule.Get()
         # current100  = currentModule.Get100()
         # currentBEEM = currentModule.BEEMGet()
-        print("Current Get")
-        print("Current:      " + str(current) + " A")
+        if(debug):
+            print("Current Get")
+            print("Current:      " + str(current) + " A")
         # print("100 Current:  " + str(current100))
         # print("BEEM Current: " + str(currentBEEM))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("----------------------------------------------------------------------")
         
         """
         Current Gains Get/Set
         """
         currentModule.GainSet(13)
         gains,gain_index = currentModule.GainsGet()
-        print("Current Gains")
-        print("Gain: " + gains[gain_index])
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Current Gains")
+            print("Gain: " + gains[gain_index])
+            print("----------------------------------------------------------------------")
         
         """
         Calibration Set/Get
         """
         currentModule.CalibrSet(calibration=1.1e-9, offset=-1.69e-12)
         calibration,offset = currentModule.CalibrGet()
-        print("Calibration")
-        print("Calibration Factor: " + str(calibration) + " (A/V)")
-        print("Offset:             " + str(offset) + " A")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Calibration")
+            print("Calibration Factor: " + str(calibration) + " (A/V)")
+            print("Offset:             " + str(offset) + " A")
+            print("----------------------------------------------------------------------")
     except:
-        print('error')
+        NTCP.close_connection()
+        return(traceback.format_exc())
+    
     NTCP.close_connection()
-    return print('end of test')
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/FolMe.py` & `nanonistcp-1.1.2/nanonisTCP/FolMe.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/FolMeTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/FolMeTest.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,56 +9,61 @@
 !WARNING: RUNNING run_test() WILL CHANGE SETTINGS IN NANONIS. RUN IT ON A SIM!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 
 
 from nanonisTCP import nanonisTCP
 from nanonisTCP.FolMe import FolMe
+import traceback
 
 """
 Set up the TCP connection and interface
 """
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, debug=False, version=13520):
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                             # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                                # Nanonis TCP interface
     try:
         followme = FolMe(NTCP)                                                          # Nanonis Follow Me Module
 
         """
         XYPos Set/Get
         """
         followme.XYPosSet(5e-9, -5e-9, Wait_end_of_move=True)                           # Set xy pos to 5 nm, -5 nm
         x,y = followme.XYPosGet(Wait_for_newest_data=True)                              # Get the current XY tip position
-        print("Tip Position: " + str(x) + " m, " + str(y) + " m")    
+        if(debug):
+            print("Tip Position: " + str(x) + " m, " + str(y) + " m")    
 
         """
         Speed Set/Get
         """
         followme.SpeedSet(speed=100e-9, custom_speed=True)                              # Set the custom move speed to 100 nm/s. Set move mode to custom speed
         speed, custom_speed = followme.SpeedGet()                                       # Get the custom move speed. get the mode
-        print("Speed: " + str(speed) + " m/s")
-        print("Mode: " + ["Scan Speed","Custom Speed"][custom_speed])
+        if(debug):
+            print("Speed: " + str(speed) + " m/s")
+            print("Mode: " + ["Scan Speed","Custom Speed"][custom_speed])
 
         """
         Oversampl Set/Get
         """
         followme.OversamplSet(3)                                                        # Set the oversampling for data acquisition in follow me mode
         oversample, sample_rate = followme.OversamplGet()                               # Get the oversampling and sample rate for data acquisition in follow me mode
-        print("Oversampling: " + str(oversample) + " @ " + str(sample_rate) + "S/s")
+        if(debug):
+            print("Oversampling: " + str(oversample) + " @ " + str(sample_rate) + "S/s")
 
         """
         Stop
         """
         followme.Stop()                                                                 # Stop the tip from moving. no effect if tip position was set with Wait_end_of_move = True
 
         """
         Point and Shoot Set/Get
         """
         followme.PSOnOffSet(False)                                                      # Disable point and shoot in follow me mode
         ps_status = followme.PSOnOffGet()                                               # Get point and shoot status
-        print("Point & Shoot: " + ["disabled","enabled"][ps_status])
+        if(debug):
+            print("Point & Shoot: " + ["disabled","enabled"][ps_status])
     except:
-        print('error')
+        NTCP.close_connection()
+        return(traceback.format_exc())
 
     NTCP.close_connection()
-    
-    return print('end of test')
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/LockIn.py` & `nanonistcp-1.1.2/nanonisTCP/LockIn.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/LockInTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/LockInTest.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,178 +10,192 @@
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 
 from nanonisTCP import nanonisTCP
 from nanonisTCP.LockIn import LockIn
 import traceback
 
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, debug=False, version=13520):
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                         # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                        # Nanonis TCP interface
     try:
         lockin = LockIn(NTCP)                                                   # Nanonis TCP Lock In Module
         
         """
         On/Off Set/Get
         """
         lockin.ModOnOffSet(modulator_number=1,lockin_onoff=1)
         lockin1 = lockin.ModOnOffGet(modulator_number=1)
         lockin2 = lockin.ModOnOffGet(modulator_number=2)
-        print("lockin1: " + ["off","on"][lockin1])
-        print("lockin2: " + ["off","on"][lockin2])
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("lockin1: " + ["off","on"][lockin1])
+            print("lockin2: " + ["off","on"][lockin2])
+            print("----------------------------------------------------------------------")
         
         """
         ModSignalSet/Get
         """
         lockin.ModSignalSet(modulator_number=1,modulator_signal_index=24)       # Make sure the signal index you give is available with Signals.NamesGet
         modulator_signal_index1  = lockin.ModSignalGet(modulator_number=1)
         modulator_signal_index2  = lockin.ModSignalGet(modulator_number=2)
-        print("Signal1: " + str(modulator_signal_index1))
-        print("Signal2: " + str(modulator_signal_index2))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Signal1: " + str(modulator_signal_index1))
+            print("Signal2: " + str(modulator_signal_index2))
+            print("----------------------------------------------------------------------")
         
         """
         ModPhasRegSet/Get
         """
         try:
             lockin.ModPhasRegSet(modulator_number=1,phase_register_index=2)     # Access denied error in demo mode
         except Exception as e:
-            print("Could not set phase register. " + str(e))
+            print("Warning: Could not set phase register. " + str(e))
         phase_reg1 = lockin.ModPhasRegGet(modulator_number=1)
         phase_reg2 = lockin.ModPhasRegGet(modulator_number=2)
-        print("Signal1: " + str(phase_reg1))
-        print("Signal2: " + str(phase_reg2))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Signal1: " + str(phase_reg1))
+            print("Signal2: " + str(phase_reg2))
+            print("----------------------------------------------------------------------")
         
         """
         ModHarmonicSet/Get
         """
         try:
             lockin.ModHarmonicSet(modulator_number=1,harmonic=2)                # Access denied error in demo mode
         except Exception as e:
-            print("Could not set phase register. " + str(e))
+            print("Warning: Could not set phase register. " + str(e))
         harmonic1 = lockin.ModHarmonicGet(modulator_number=1)
         harmonic2 = lockin.ModHarmonicGet(modulator_number=2)
-        print("Harmonic1: " + str(harmonic1))
-        print("Harmonic2: " + str(harmonic2))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Harmonic1: " + str(harmonic1))
+            print("Harmonic2: " + str(harmonic2))
+            print("----------------------------------------------------------------------")
         
         """
         ModPhasSet/Get
         """
         try:
             lockin.ModPhasSet(modulator_number=1,phase_deg=99)                  # Access denied error in demo mode
         except Exception as e:
-            print("Could not set phase. " + str(e))
+            print("Warning: Could not set phase. " + str(e))
         phase1 = lockin.ModPhasGet(modulator_number=1)
         phase2 = lockin.ModPhasGet(modulator_number=2)
-        print("Phase1: " + str(phase1))
-        print("Phase2: " + str(phase2))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Phase1: " + str(phase1))
+            print("Phase2: " + str(phase2))
+            print("----------------------------------------------------------------------")
         
         """
         ModAmpSet/Get
         """
         try:
             lockin.ModAmpSet(modulator_number=1,amplitude=2)                    # Access denied error in demo mode
         except Exception as e:
-            print("Could not set amplitude. " + str(e))
+            print("Warning: Could not set amplitude. " + str(e))
         amplitude1 = lockin.ModAmpGet(modulator_number=1)
         amplitude2 = lockin.ModAmpGet(modulator_number=2)
-        print("Amplitude1: " + str(amplitude1))
-        print("Amplitude2: " + str(amplitude2))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Amplitude1: " + str(amplitude1))
+            print("Amplitude2: " + str(amplitude2))
+            print("----------------------------------------------------------------------")
         
         """
         ModPhasFreqSet/Get
         """
         try:
             lockin.ModPhasFreqSet(modulator_number=1,frequency=2e3)             # Access denied error in demo mode
         except Exception as e:
-            print("Could not set frequency. " + str(e))
+            print("Warning: Could not set frequency. " + str(e))
         frequency1 = lockin.ModPhasFreqGet(modulator_number=1)
         frequency2 = lockin.ModPhasFreqGet(modulator_number=2)
-        print("Frequency1: " + str(frequency1))
-        print("frequency2: " + str(frequency2))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Frequency1: " + str(frequency1))
+            print("frequency2: " + str(frequency2))
+            print("----------------------------------------------------------------------")
         
         """
         DemodSignalSet/Get
         """
         lockin.DemodSignalSet(demod_number=1,demod_signal_index=1)
         demod_signal_index1 = lockin.DemodSignalGet(demod_number=1)
         demod_signal_index2 = lockin.DemodSignalGet(demod_number=2)
-        print("Signal1: " + str(demod_signal_index1))
-        print("Signal2: " + str(demod_signal_index2))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Signal1: " + str(demod_signal_index1))
+            print("Signal2: " + str(demod_signal_index2))
+            print("----------------------------------------------------------------------")
         
         """
         DemodLPFilterSet/Get
         """
         try:
             lockin.DemodLPFilterSet(demod_number=1,lp_filter_order=1,cutoff=2e3)# Access denied error in demo mode
         except Exception as e:
-            print("Could not set lpfilter. " + str(e))
+            print("Warning: Could not set lpfilter. " + str(e))
         lpfilter1 = lockin.DemodLPFilterGet(demod_number=1)
         lpfilter2 = lockin.DemodLPFilterGet(demod_number=2)
-        print("LP Filter1: " + str(lpfilter1))
-        print("LP Filter2: " + str(lpfilter2))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("LP Filter1: " + str(lpfilter1))
+            print("LP Filter2: " + str(lpfilter2))
+            print("----------------------------------------------------------------------")
         
         """
         DemodPhasRegSet/Get
         """
         try:
             lockin.DemodPhasRegSet(demod_number=1,phase_register_index=1)       # Access denied error in demo mode
         except Exception as e:
-            print("Could not set phase register. " + str(e))
+            print("Warning: Could not set phase register. " + str(e))
         phase_reg1 = lockin.DemodPhasRegGet(demod_number=1)
         phase_reg2 = lockin.DemodPhasRegGet(demod_number=2)
-        print("Phase Register1: " + str(phase_reg1))
-        print("Phase Register2: " + str(phase_reg2))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Phase Register1: " + str(phase_reg1))
+            print("Phase Register2: " + str(phase_reg2))
+            print("----------------------------------------------------------------------")
         
         """
         DemodPhasSet/Get
         """
         try:
             lockin.DemodPhasSet(demod_number=1,phase_deg=98)                    # Access denied error in demo mode
         except Exception as e:
-            print("Could not set phase. " + str(e))
+            print("Warning: Could not set phase. " + str(e))
         phase1 = lockin.DemodPhasGet(demod_number=1)
         phase2 = lockin.DemodPhasGet(demod_number=2)
-        print("Phase1: " + str(phase1))
-        print("Phase2: " + str(phase2))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Phase1: " + str(phase1))
+            print("Phase2: " + str(phase2))
+            print("----------------------------------------------------------------------")
         
         """
         DemodSyncFilterSet/Get
         """
         try:
             lockin.DemodSyncFilterSet(demod_number=1,sync_filter=0)             # Access denied error in demo mode
         except Exception as e:
-            print("Could not set sync filter. " + str(e))
+            print("Warning: Could not set sync filter. " + str(e))
         syncFilter1 = lockin.DemodSyncFilterGet(demod_number=1)
         syncFilter2 = lockin.DemodSyncFilterGet(demod_number=2)
-        print("syncFilter1: " + str(syncFilter1))
-        print("syncFilter2: " + str(syncFilter2))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("syncFilter1: " + str(syncFilter1))
+            print("syncFilter2: " + str(syncFilter2))
+            print("----------------------------------------------------------------------")
         
         """
         DemodRTSignalsSet/Get
         """
         try:
             lockin.DemodRTSignalsSet(demod_number=1,rt_signals=1)               # Access denied error in demo mode
         except Exception as e:
-            print("Could not set RT Signals. " + str(e))
+            print("Warning: Could not set RT Signals. " + str(e))
         rtSignals1 = lockin.DemodRTSignalsGet(demod_number=1)
         rtSignals2 = lockin.DemodRTSignalsGet(demod_number=2)
-        print("rtSignals1: " + str(rtSignals1))
-        print("rtSignals2: " + str(rtSignals2))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("rtSignals1: " + str(rtSignals1))
+            print("rtSignals2: " + str(rtSignals2))
+            print("----------------------------------------------------------------------")
     except:
-        print(traceback.format_exc())
+        NTCP.close_connection()
+        return traceback.format_exc()
         
     NTCP.close_connection()
-    return print('end of test')
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/Marks.py` & `nanonistcp-1.1.2/nanonisTCP/Marks.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/MarksTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/MarksTest.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,49 +7,47 @@
 """
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !WARNING: RUNNING run_test() WILL CHANGE SETTINGS IN NANONIS. RUN IT ON A SIM!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 
 from nanonisTCP import nanonisTCP
-# from nanonisTCP.Marks import Marks
-from Marks import Marks
+from nanonisTCP.Marks import Marks
 import traceback
 
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, debug=False, version=13520):
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                         # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                        # Nanonis TCP interface
     try:
         marks = Marks(NTCP)                                                     # Nanonis TCP Marks In Scan Module
         
         """
         PointDraw
         """
         marks.PointDraw(p=(0,0),text="(0,0)",c=0)
         marks.PointDraw(p=(300e-9,-300e-9),text="(300nm,-300nm)",c=0)
-        print('Placed blacl text: "Xx." at (0,0)')
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print('Placed blacl text: "Xx." at (0,0)')
+            print("----------------------------------------------------------------------")
         
         """
         LineDraw
         """
         start = (0,0)
         end   = (300e-9,-300e-9)
         marks.LineDraw(start=start, end=end)
-        print("----------------------------------------------------------------------")
         
         """
         PointsErase
         """
         marks.PointsErase()
-        print("----------------------------------------------------------------------")
         
         """
         LinesErase
         """
         marks.LinesErase()
-        print("----------------------------------------------------------------------")
     except:
-        print(traceback.format_exc())
+        NTCP.close_connection()
+        return traceback.format_exc()
         
     NTCP.close_connection()
-    return print('end of test')
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/Motor.py` & `nanonistcp-1.1.2/nanonisTCP/Motor.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/MotorTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/SignalsTest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,77 @@
 # -*- coding: utf-8 -*-
 """
-Created on Tue May  3 19:34:49 2022
+Created on Mon May 30 12:41:36 2022
 
 @author: Julian Ceddia
 """
 """
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !WARNING: RUNNING run_test() WILL CHANGE SETTINGS IN NANONIS. RUN IT ON A SIM!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 
 from nanonisTCP import nanonisTCP
-from nanonisTCP.Motor import Motor
+from nanonisTCP.Signals import Signals
+import traceback
 
-"""
-Set up the TCP connection and interface
-"""
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6502, make_plot=False):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, version=13520, debug=False):
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                         # Nanonis TCP interface
-    
-    motor = Motor(NTCP)                                                         # Nanonis Coarse Motion (Motor)Module
-    
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                        # Nanonis TCP interface
     try:
-        """
-        Start Move
-        """
-        motor.StartMove(direction="Z+",steps=100,group=2,wait_until_finished=False)
+        signalsModule = Signals(NTCP)                                           # Nanonis TCP Signals Module
         
         """
-        Stop Moter Move
+        Signals NamesGet
         """
-        motor.StopMove()
+        signal_names = signalsModule.NamesGet()
+        if(debug):
+            print("Signals NamesGet")
+            print("Signal names:\n" + "\n".join(signal_names))
+            print("----------------------------------------------------------------------")
         
-        print("----------------------------------------------------------------------")
         """
-        Start Closed Loop
+        Signals InSlots Set/Get
         """
-        try:
-            motor.StartClosedLoop(abs_rel=True, target_x=0, target_y=0, target_z=10, wait_until_finished=False)
-        except Exception as e:
-            print("Error in Motor.StartClosedLoop: ")
-            print(e)
-            print("----------------------------------------------------------------------")
+        if(version < 11798):                                                    # Deprecated in version 11798
+            signalsModule.InSlotSet(slot=5, RTSignalIndex=10)                   # Puts "Input 11 (V)" into slot index 5 of 24
+            signal_names,signal_indexes = signalsModule.InSlotsGet()
+            if(debug):
+                print("Signals InSlots")
+                for i,signal_name in enumerate(signal_names):
+                    print("signal " + str(i) + ": " + str(signal_indexes[i]) + "| " + signal_name)
+                print("----------------------------------------------------------------------")
+        
         """
-        Motor Pos Get
+        Signals CalibrGet
         """
-        try:
-            x_pos,y_pos,z_pos = motor.PosGet()
-            print("Motor Positions")
-            print("x pos: " + str(x_pos))
-            print("y pos: " + str(y_pos))
-            print("z pos: " + str(z_pos))
-            print("----------------------------------------------------------------------")
-        except Exception as e:
-            print("Error in Motor.PosGet: ")
-            print(e)
+        calibration,offset = signalsModule.CalibrGet(24)
+        if(debug):
+            print("Signals CalibrGet")
+            print("Calibration: " + str(calibration))
+            print("Offset:      " + str(offset))
             print("----------------------------------------------------------------------")
         
         """
-        Step Counter Get
+        Signals RangeGet
         """
-        try:
-            counter_x,counter_y,counter_z = motor.StepCounterGet()
-            print("Motor Step Counters")
-            print("x steps: " + str(counter_x))
-            print("y steps: " + str(counter_y))
-            print("z steps: " + str(counter_z))
-            print("----------------------------------------------------------------------")
-        except Exception as e:
-            print("Error in Motor.StepCounterGet: ")
-            print(e)
+        max_limit,min_limit = signalsModule.RangeGet(24)
+        if(debug):
+            print("Signals RageGet")
+            print("Max limit: " + str(max_limit))
+            print("Min limit: " + str(min_limit))
             print("----------------------------------------------------------------------")
         
         """
-        Freq/Amp Set/Get
+        Signals GetVal
         """
-        motor.FreqAmpSet(frequency=1111, amplitude=199)
-        [frequency,amplitude] = motor.FreqAmpGet()
-        print("Motor Frequency/Amplidtude")
-        print("Frequency: " + str(frequency))
-        print("Amplitude: " + str(amplitude))
-        print("----------------------------------------------------------------------")
-        
-        print("test complete")
-    except Exception as e:
-        print(e)
+        signal_val = signalsModule.ValGet(2)
+        if(debug):
+            print("Signals GetVal")
+            print("Signal value: " + str(signal_val))
+            print("----------------------------------------------------------------------")
+    except:
+        NTCP.close_connection()
+        return(traceback.format_exc())
     
-    NTCP.close_connection()
+    NTCP.close_connection()
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/Osci2T.py` & `nanonistcp-1.1.2/nanonisTCP/Osci2T.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/Osci2TTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/Osci2TTest.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,77 +10,83 @@
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 import time
 from nanonisTCP import nanonisTCP
 from nanonisTCP.Osci2T import Osci2T
 import traceback
 
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, plotData=1):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, plotData=1, debug=False, version=13520):
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                         # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                        # Nanonis TCP interface
     try:
         osci2T = Osci2T(NTCP)                                                   # Nanonis TCP Oscilloscope 2-Channels Module
         """
         Osci2T Run
         """
         osci2T.Run()
-        print("Osci2T Running")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Osci2T Running")
+            print("----------------------------------------------------------------------")
         
         """
         Osci2T ChsSet/Get
         """
         osci2T.ChsSet(chA=0,chB=24)
         chA,chB = osci2T.ChsGet()
-        print("Channel A Index: ",chA)
-        print("Channel B Index: ",chB)
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Channel A Index: ",chA)
+            print("Channel B Index: ",chB)
+            print("----------------------------------------------------------------------")
         
         """
         Osci2T TimebaseSet/Get
         """
         osci2T.TimebaseSet(timebaseIndex=5)
         timebaseIndex,timebases = osci2T.TimebaseGet()
-        print("timebaseIndex: ",timebaseIndex)
-        print("timebases: ",timebases)
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("timebaseIndex: ",timebaseIndex)
+            print("timebases: ",timebases)
+            print("----------------------------------------------------------------------")
         
         """
         Oversample Set/Get
         """
         osci2T.OversamplSet(oversamplingIndex=4)
         oversamplingIndex = osci2T.OversamplGet()
-        print("Oversampling Index",oversamplingIndex)
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Oversampling Index",oversamplingIndex)
+            print("----------------------------------------------------------------------")
         
         """
         Trig Set/Get
         """
         time.sleep(1)                                                           # Updating trigger too soon sometimes causes Nanonis not to register for some reason?
         osci2T.TrigSet(mode=0, channel=0, slope=1, level=0, hysteresis=0, position=2)
         mode,channel,slope,level,hysteresis,position = osci2T.TrigGet()
-        print("Mode",mode)
-        print("Channel",channel)
-        print("slope",slope)
-        print("level",level)
-        print("hysteresis",hysteresis)
-        print("position",position)
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Mode",mode)
+            print("Channel",channel)
+            print("slope",slope)
+            print("level",level)
+            print("hysteresis",hysteresis)
+            print("position",position)
+            print("----------------------------------------------------------------------")
         
         """
         DataGet
         """
         time.sleep(2) # Wait for data
         t0,dt,chA,chB = osci2T.DataGet(dataToGet=0)
         if(plotData):
             import matplotlib.pyplot as plt
             import numpy as np
             xx = np.arange(len(chA))*dt + t0
             plt.plot(xx,chA)
             plt.plot(xx,chB)
             
         
-    except Exception as e:
-        print(traceback.format_exc())
-        print(e)
+    except:
+        NTCP.close_connection()
+        return traceback.format_exc()
+        
     NTCP.close_connection()
-    return print('end of test')
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/Pattern.py` & `nanonistcp-1.1.2/nanonisTCP/Pattern.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/SafeTip.py` & `nanonistcp-1.1.2/nanonisTCP/SafeTip.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/SafeTipTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/SafeTipTest.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,50 +8,56 @@
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !WARNING: RUNNING run_test() WILL CHANGE SETTINGS IN NANONIS. RUN IT ON A SIM!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 
 from nanonisTCP import nanonisTCP
 from nanonisTCP.SafeTip import SafeTip
+import traceback
 
 """
 Set up the TCP connection and interface
 """
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6502, make_plot=False):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6502, make_plot=False, debug=False, version=13520):
     
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                         # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                        # Nanonis TCP interface
     
     safeTip = SafeTip(NTCP)                                                     # Nanonis Safe Tip Module
     
     try:
         """
         On/Off Set/Get
         """
         safeTip.OnOffSet(safe_tip_status=2)
         safe_tip_status = safeTip.OnOffGet()
-        print("Safe Tip Status")
-        print("Safe Tip Mode:  " + ["off","on"][safe_tip_status])
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Safe Tip Status")
+            print("Safe Tip Mode:  " + ["off","on"][safe_tip_status])
+            print("----------------------------------------------------------------------")
         
         """
         Signal Get
         """
         signal_value = safeTip.SignalGet()
-        print("Safe Tip Signal")
-        print("Signal value:  " + str(signal_value) + " A")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Safe Tip Signal")
+            print("Signal value:  " + str(signal_value) + " A")
+            print("----------------------------------------------------------------------")
         
         """
         Properties Set/Get
         """
         safeTip.PropsSet(auto_recovery=True,auto_pause_scan=True,threshold=15e-10)
         auto_recovery,auto_pause_scan,threshold = safeTip.PropsGet()
-        print("Safe Tip Properties")
-        print("Auto recovery:  " + ["Off","On"][auto_recovery])
-        print("Auto pause:     " + ["Off","On"][auto_pause_scan])
-        print("Threshold:      " + str(threshold) + " A")
-        print("----------------------------------------------------------------------")
-    except Exception as e:
-        print(e)
-    
-    NTCP.close_connection()
+        if(debug):
+            print("Safe Tip Properties")
+            print("Auto recovery:  " + ["Off","On"][auto_recovery])
+            print("Auto pause:     " + ["Off","On"][auto_pause_scan])
+            print("Threshold:      " + str(threshold) + " A")
+            print("----------------------------------------------------------------------")
+    except:
+        NTCP.close_connection()
+        return traceback.format_exc()
+        
+    NTCP.close_connection()
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/Scan.py` & `nanonistcp-1.1.2/nanonisTCP/Scan.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,16 +130,23 @@
     
     def BufferSet(self,channel_indexes=None,pixels=None,lines=None):
         """
         Configures the scan buffer parameters
 
         Parameters
         num_channels    : number of recorded channels.
-        channel_indexes : indexes of recorded channels (see signals manager or
+        channel_indexes : Nanonis v < R11798, use slot number:
+                          Indexes of recorded channels (see signals manager or
                           use Signals.InSlotsGet function)
+
+                          Nanonis v >= R11798, use RT Index:
+                          Indexes of recorded channels. The index is comprised between 0
+                          and 127, and it corresponds to the full list of signals available in the system.
+                          To get the signal name and its corresponding index in the list of the 128 available signals in the Nanonis
+                          Controller, use the Signal.NamesGet function, or check the RT Idx value in the Signals Manager module.
         pixels          : number of pixels per line. forced to a multiple of 16
         lines           : number of scan lines
 
         """
         _, buf_channel_indexes, buf_pixels, buf_lines = self.BufferGet()        # Get the values currently in the buffer
         
         if(not channel_indexes): channel_indexes = buf_channel_indexes          # Keep the original value if we don't want to change it in this call
@@ -166,16 +173,23 @@
         
     def BufferGet(self):
         """
         Returns the scan buffer parameters
 
         Returns
         num_channels    : number of recorded channels.
-        channel_indexes : indexes of recorded channels (see signals manager or
+        channel_indexes : Nanonis v < R11798, slot number:
+                          Indexes of recorded channels (see signals manager or
                           use Signals.InSlotsGet function)
+
+                          Nanonis v >= R11798, RT Index:
+                          Indexes of recorded channels. The index is comprised between 0
+                          and 127, and it corresponds to the full list of signals available in the system.
+                          To get the signal name and its corresponding index in the list of the 128 available signals in the Nanonis
+                          Controller, use the Signal.NamesGet function, or check the RT Idx value in the Signals Manager module.
         pixels          : number of pixels per line. forced to a multiple of 16
         lines           : number of scan lines
 
         """
         ## Make Header
         hex_rep = self.nanonisTCP.make_header('Scan.BufferGet', body_size=0)
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/ScanTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/ScanTest.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,81 +8,86 @@
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !WARNING: RUNNING run_test() WILL CHANGE SETTINGS IN NANONIS. RUN IT ON A SIM!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 
 from nanonisTCP import nanonisTCP
 from nanonisTCP.Scan import Scan
+import traceback
 
 """
 Set up the TCP connection and interface
 """
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, make_plot=False):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, make_plot=False, debug=False, version=13520):
     
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                             # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                                # Nanonis TCP interface
     
     try:
         scan = Scan(NTCP)                                                               # Nanonis Scan Module
         
         """
         Frame Parameters Set/Get
         """
         scan.FrameSet(5e-9,-5e-9,30e-9,30e-9,15)
         x,y,w,h,angle = scan.FrameGet()
-        print("Frame Parameters")
-        print("Frame Position:  " + str(x) + " m," + str(y) + " m")
-        print("Frame dimension: " + str(w) + " m x " + str(h) + " m")
-        print("Frame angle:     " + str(angle) + " deg")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Frame Parameters")
+            print("Frame Position:  " + str(x) + " m," + str(y) + " m")
+            print("Frame dimension: " + str(w) + " m x " + str(h) + " m")
+            print("Frame angle:     " + str(angle) + " deg")
+            print("----------------------------------------------------------------------")
 
         """
         Buffer Parameters Set/Get
         """
-        scan.BufferSet(channel_indexes=[0,14],pixels=128,lines=128)
+        scan.BufferSet(channel_indexes=[0],pixels=128,lines=128)
         num_channels,channel_indexes,pixels,lines = scan.BufferGet()
-        print("Buffer Parameters")
-        print("Buffer num_channels:    " + str(num_channels))
-        print("Buffer channel_indexes: " + str(channel_indexes))
-        print("Buffer pixels:          " + str(pixels))
-        print("Buffer lines:           " + str(lines))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Buffer Parameters")
+            print("Buffer num_channels:    " + str(num_channels))
+            print("Buffer channel_indexes: " + str(channel_indexes))
+            print("Buffer pixels:          " + str(pixels))
+            print("Buffer lines:           " + str(lines))
+            print("----------------------------------------------------------------------")
 
         """
         Props Set/Get
         """
         scan.PropsSet(bouncy_scan=1,comment="testing123")
         continuous_scan,bouncy_scan,autosave,series_name,comment = scan.PropsGet()
-        print("Props Parameters")
-        print("Props continuous_scan: " + str(continuous_scan))
-        print("Props bouncy_scan:     " + str(bouncy_scan))
-        print("Props autosave:        " + str(autosave))
-        print("Props series_name:     " + str(series_name))
-        print("Props comment:         " + str(comment))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Props Parameters")
+            print("Props continuous_scan: " + str(continuous_scan))
+            print("Props bouncy_scan:     " + str(bouncy_scan))
+            print("Props autosave:        " + str(autosave))
+            print("Props series_name:     " + str(series_name))
+            print("Props comment:         " + str(comment))
+            print("----------------------------------------------------------------------")
 
         """
         Speed Set/Get
         """
         # Best practice here is to define at least (fwd_speed or fwd_line_time) + (corresponding bwd param or speed_ratio)
         # e.g. one of these...
         # scan.SpeedSet(fwd_speed=150e-9,bwd_speed=400e-9)                              # Expect speeds to be set accordingly and constant param = line speed
         # scan.SpeedSet(fwd_line_time=1,bwd_line_time=0.25)                             # Expect times to be set accordingly and constant param = line time
         # scan.SpeedSet(fwd_speed=150e-9,speed_ratio=2)                                 # Expect fwd_speed=150e-9 and bwd_speed=300e-9
-        scan.SpeedSet(fwd_line_time=1,speed_ratio=2)                                    # Expect fwd_line_time=1s and bwd_line_time=0.5s
+        scan.SpeedSet(fwd_line_time=0.05,speed_ratio=2)                                 # Expect fwd_line_time=1s and bwd_line_time=0.5s
 
         fwd_speed,bwd_speed,fwd_line_time,bwd_line_time,const_param,speed_ratio = scan.SpeedGet()
-        print("Scan Speed Parameters")
-        print("Forward speed:      " + str(fwd_speed))
-        print("Backward speed:     " + str(bwd_speed))
-        print("Forward line time:  " + str(fwd_line_time))
-        print("Backward line time: " + str(bwd_line_time))
-        print("Constant Param:     " + ["Constant speed", "Constant time"][const_param])
-        print("Speed ratio:        " + str(speed_ratio))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Scan Speed Parameters")
+            print("Forward speed:      " + str(fwd_speed))
+            print("Backward speed:     " + str(bwd_speed))
+            print("Forward line time:  " + str(fwd_line_time))
+            print("Backward line time: " + str(bwd_line_time))
+            print("Constant Param:     " + ["Constant speed", "Constant time"][const_param])
+            print("Speed ratio:        " + str(speed_ratio))
+            print("----------------------------------------------------------------------")
         
         
         """
         Action
         """
         scan.Action("start","down")
 
@@ -90,34 +95,36 @@
         Status Get
         """
 
         """
         Wait end of scan
         """
         timeout_status, file_path_size, file_path = scan.WaitEndOfScan()
-        print("Wait end of scan")
-        print("timeout_status: " + ["EOS","Timed out"][timeout_status])
-        print("file_path: " + file_path)
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Wait end of scan")
+            print("timeout_status: " + ["EOS","Timed out"][timeout_status])
+            print("file_path: " + file_path)
+            print("----------------------------------------------------------------------")
        
         """
         FrameDataGrab
         """
-        channel_name,scan_data,scan_direction = scan.FrameDataGrab(14, 1)
-        print("Frame Data")
-        print("Channel name:   " + channel_name)
-        print("Scan direction: " + scan_direction)
-        print("Run commented code to show scan_data")
-        if make_plot == True:
-            import matplotlib.pyplot as plt
-            import matplotlib
-            fig = plt.figure()
-            ax = fig.add_subplot(111)
-            ax.imshow(scan_data)
-        print("----------------------------------------------------------------------")
+        channel_name,scan_data,scan_direction = scan.FrameDataGrab(0, 1)
+        if(debug):
+            print("Frame Data")
+            print("Channel name:   " + channel_name)
+            print("Scan direction: " + scan_direction)
+            print("Run commented code to show scan_data")
+            if make_plot == True:
+                import matplotlib.pyplot as plt
+                import matplotlib
+                fig = plt.figure()
+                ax = fig.add_subplot(111)
+                ax.imshow(scan_data)
+            print("----------------------------------------------------------------------")
 
     except:
-        print('error')
+        NTCP.close_connection()
+        return(traceback.format_exc())
     
     NTCP.close_connection()
-
-    return print('end of test')
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/Signals.py` & `nanonistcp-1.1.2/nanonisTCP/Signals.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/TipShaper.py` & `nanonistcp-1.1.2/nanonisTCP/TipShaper.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/TipShaperTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/TipShaperTest.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,51 +8,55 @@
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !WARNING: RUNNING run_test() WILL CHANGE SETTINGS IN NANONIS. RUN IT ON A SIM!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 
 from nanonisTCP import nanonisTCP
 from nanonisTCP.TipShaper import TipShaper
+import traceback
 
 """
 Set up the TCP connection and interface
 """
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, make_plot=False):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, make_plot=False, debug=False, version=13520):
     
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                         # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                        # Nanonis TCP interface
     
     tipShaper = TipShaper(NTCP)                                                 # Nanonis Tip Shaper Module
     
     try:
               
         """
         Properties Set/Get
         """
         tipShaper.PropsSet(Switch_off_delay=1,Change_bias=1,Bias=0.02,Tip_lift=-2e-9,Lift_time_1=0.2,Bias_lift=0.05,
                 Bias_settling_time=0.1,Lift_height=5e-9,Lift_time_2=0.2,End_wait_time=0.1,
                 Restore_feedback=1)
         
         Switch_off_delay,Change_bias,Bias,Tip_lift,Lift_time_1,Bias_lift,Bias_settling_time,Lift_height,Lift_time_2,End_wait_time,Restore_feedback = tipShaper.PropsGet()
-        print("Tip Shaper Properties")
-        print("Switch off delay:  " + "%f" % Switch_off_delay)
-        print("Change Bias status:" + ["no change","True","False"][Change_bias])
-        print("Bias: %f" % Bias)
-        print("Tip Lift: %f m" % Tip_lift)
-        print("Lift_time_1: %f s" % Lift_time_1)
-        print("Bias_lift: %f V" % Bias_lift)
-        print("Bias settling time: %f s" % Bias_settling_time)
-        print("Lift_height: %f m" % Lift_height)
-        print("Lift_time_2: %f s" % Lift_time_2)
-        print("End_wait_time: %f" % End_wait_time)
-        print("Restore Feedback?" + ["no change","yes","no"][Restore_feedback])
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Tip Shaper Properties")
+            print("Switch off delay:  " + "%f" % Switch_off_delay)
+            print("Change Bias status:" + ["no change","True","False"][Change_bias])
+            print("Bias: %f" % Bias)
+            print("Tip Lift: %f m" % Tip_lift)
+            print("Lift_time_1: %f s" % Lift_time_1)
+            print("Bias_lift: %f V" % Bias_lift)
+            print("Bias settling time: %f s" % Bias_settling_time)
+            print("Lift_height: %f m" % Lift_height)
+            print("Lift_time_2: %f s" % Lift_time_2)
+            print("End_wait_time: %f" % End_wait_time)
+            print("Restore Feedback? " + ["no change","yes","no"][Restore_feedback])
+            print("----------------------------------------------------------------------")
         
         """
         Start
         """
         tipShaper.Start(wait_until_finished=1,timeout=10)
         
-    except Exception as e:
-        print(e)
+    except:
+        NTCP.close_connection()
+        return(traceback.format_exc())
     
-    NTCP.close_connection()
+    NTCP.close_connection()
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/UserOut.py` & `nanonistcp-1.1.2/nanonisTCP/UserOut.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/UserOutTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/UserOutTest.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,41 +3,44 @@
 Created on Tue Feb 2 18:56:49 2024
 
 @author: jced0001
 """
 
 from nanonisTCP import nanonisTCP
 from nanonisTCP.UserOut import UserOut
+import traceback
 
 """
 Set up the TCP connection and interface
 """
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6501, debug=False, version=13520):
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                             # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                                # Nanonis TCP interface
     try:
         userOut = UserOut(NTCP)                                                         # Nanonis User Outs Module
 
         """
         Output Mode Set/Get
         """
         userOut.ModeSet(2,1)                                                            # Set Out2 to Monitor
         output_mode = userOut.ModeGet(2)                                                # Check to see if the mode for Output2 has changed
-        print("UserOut ModeGet")
-        print("Output Mode: ",["User Output","Monitor","Calc.Signal"][output_mode])
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("UserOut ModeGet")
+            print("Output Mode: ",["User Output","Monitor","Calc.Signal"][output_mode])
+            print("----------------------------------------------------------------------")
 
         """
         Output Monitor Set/Get
         """
         userOut.MonitorChSet(2,1)                                                       # Set the monitor channel to index 1 for output 2
         monitor_index = userOut.MonitorChGet(2)                                         # Check to see if it changed.
-        print("UserOut MonitorChGet")
-        print("Monitor index: ",monitor_index)
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("UserOut MonitorChGet")
+            print("Monitor index: ",monitor_index)
+            print("----------------------------------------------------------------------")
 
         """
         Output Val Set
         (There is no Get in the protocol)
         """
         userOut.ValSet(8,3.3)
         
@@ -48,37 +51,40 @@
         userOut.CalibrSet(8,0.2,0.1)
 
         """
         Output CalcSignalName Set/Get
         """
         userOut.CalcSignalNameSet(8,"Output 8 Test")
         calculated_signal_name = userOut.CalcSignalNameGet(8)
-        print("UserOut CalcSignalNameGet")
-        print("Signal name: ",calculated_signal_name)
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("UserOut CalcSignalNameGet")
+            print("Signal name: ",calculated_signal_name)
+            print("----------------------------------------------------------------------")
 
         """
         Output CalcSignalConfig Set/Get
         """
         userOut.CalcSignalConfigSet(8,1,2,1)
         signal_1,operation,signal_2 = userOut.CalcSignalConfigGet(8)
-        print("UserOut CalcSignalConfiGet")
-        print("Signal 1:  ",signal_1)
-        print("Operation: ",operation)
-        print("Signal 2:  ",signal_2)
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("UserOut CalcSignalConfiGet")
+            print("Signal 1:  ",signal_1)
+            print("Operation: ",operation)
+            print("Signal 2:  ",signal_2)
+            print("----------------------------------------------------------------------")
 
         """
         Output Limits Get/Set
         """
         userOut.LimitsSet(8,-3.3,4.3)
         lower_limit,upper_limit = userOut.LimitsGet(8)
-        print("UserOut Limits Get")
-        print("Lower Limit:",lower_limit)
-        print("Upper Limit:",upper_limit)
-        print("----------------------------------------------------------------------")
-    except Exception as e:
-        print('error',e)
+        if(debug):
+            print("UserOut Limits Get")
+            print("Lower Limit:",lower_limit)
+            print("Upper Limit:",upper_limit)
+            print("----------------------------------------------------------------------")
+    except:
+        NTCP.close_connection()
+        return(traceback.format_exc())
+    
     NTCP.close_connection()
-    return print('end of test')
-
-run_test()
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/ZController.py` & `nanonistcp-1.1.2/nanonisTCP/ZController.py`

 * *Files identical despite different names*

### Comparing `nanonisTCP-1.0.2/nanonisTCP/ZControllerTest.py` & `nanonistcp-1.1.2/nanonisTCP/test/ZControllerTest.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,146 +9,161 @@
 !WARNING: RUNNING run_test() WILL CHANGE SETTINGS IN NANONIS. RUN IT ON A SIM!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 """
 
 import time
 from nanonisTCP import nanonisTCP
 from nanonisTCP.ZController import ZController
+import traceback
 
 """
 Set up the TCP connection and interface
 """
-def run_test(TCP_IP='127.0.0.1', TCP_PORT=6502, make_plot=False):
+def run_test(TCP_IP='127.0.0.1', TCP_PORT=6502, make_plot=False, debug=False, version=13520):
     
     # Listening Port: see Nanonis File>Settings>TCP Programming Interface
-    NTCP = nanonisTCP(TCP_IP, TCP_PORT)                                         # Nanonis TCP interface
+    NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=version)                        # Nanonis TCP interface
     
     zctrl = ZController(NTCP)                                                   # Nanonis Z-Controller Module
     
     try:
         """
         ZPos Set/Get
         """
         zctrl.ZPosSet(140e-9)
         zpos = zctrl.ZPosGet()
-        print("Z-Controller ZPos")
-        print("zpos: " + str(zpos) + " m")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Z-Controller ZPos")
+            print("zpos: " + str(zpos) + " m")
+            print("----------------------------------------------------------------------")
         
         """
         OnOff Set/Get
         """
         zctrl.OnOffSet(on=False)
         time.sleep(1)                                                           # Need to sleep otherwise it doesn't update in time
         z_status = zctrl.OnOffGet()
-        print("Z-Controller Status")
-        print("Controller: " + ["Off","On"][z_status])
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Z-Controller Status")
+            print("Controller: " + ["Off","On"][z_status])
+            print("----------------------------------------------------------------------")
         
         """
         Setpnt Set/Get
         """
         zctrl.SetpntSet(27e-12)
         setpoint = zctrl.SetpntGet()
-        print("Z-Controller Setpoint")
-        print("Setpoint: " + str(setpoint) + " A")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Z-Controller Setpoint")
+            print("Setpoint: " + str(setpoint) + " A")
+            print("----------------------------------------------------------------------")
         
         """
         Gain Set/Get
         """
         zctrl.GainSet(3e-12, 155e-6)
         p_gain,time_constant,i_gain = zctrl.GainGet()
-        print("Z-Controller Gain")
-        print("proportional gain: " + str(p_gain))
-        print("integral gain:     " + str(i_gain))
-        print("time constant:     " + str(time_constant))
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Z-Controller Gain")
+            print("proportional gain: " + str(p_gain))
+            print("integral gain:     " + str(i_gain))
+            print("time constant:     " + str(time_constant))
+            print("----------------------------------------------------------------------")
         
         """
         Switch off delay Set/Get
         """
         zctrl.SwitchOffDelaySet(0.07575)
         delay = zctrl.SwitchOffDelayGet()
-        print("Z-Controller Switch Off Delay")
-        print("Switch off delay: " + str(delay) + " s")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Z-Controller Switch Off Delay")
+            print("Switch off delay: " + str(delay) + " s")
+            print("----------------------------------------------------------------------")
         
         """
         Tip Lift Set/Get
         """
         zctrl.TipLiftSet(19e-9)
         tip_lift = zctrl.TipLiftGet()
-        print("Z-Controller Tip Lift")
-        print("Tip Lift: " + str(tip_lift) + " m")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Z-Controller Tip Lift")
+            print("Tip Lift: " + str(tip_lift) + " m")
+            print("----------------------------------------------------------------------")
         
         """
         Home Properties Set/Get
         """
         zctrl.HomePropsSet(1, 160e-9)
         abs_rel,home_pos = zctrl.HomePropsGet()
-        print("Z-Controller Home Properties")
-        print("Mode:     " + ["Absolute","Relative"][abs_rel])
-        print("Home Pos: " + str(home_pos) + " m")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Z-Controller Home Properties")
+            print("Mode:     " + ["Absolute","Relative"][abs_rel])
+            print("Home Pos: " + str(home_pos) + " m")
+            print("----------------------------------------------------------------------")
         
         """
         Home
         """
         zctrl.Home()
         
         """
         Control List Get
         """
         controllers,active_controller = zctrl.CtrlListGet()
-        print("Z-Controller Controller")
-        print("Available Controllers: " + str(controllers))
-        print("Active Controller:     " + controllers[active_controller])
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Z-Controller Controller")
+            print("Available Controllers: " + str(controllers))
+            print("Active Controller:     " + controllers[active_controller])
+            print("----------------------------------------------------------------------")
         
         """
         Withdraw Rate Set/Get
         """
         zctrl.WithdrawRateSet(20e-9)
         slew_rate = zctrl.WithdrawRateGet()
-        print("Z-Controller Slew Rate")
-        print("Slew Rate: " + str(slew_rate) + " m/s")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Z-Controller Slew Rate")
+            print("Slew Rate: " + str(slew_rate) + " m/s")
+            print("----------------------------------------------------------------------")
         
         """
         Withdraw
         """
         time.sleep(0.5)
         zctrl.Withdraw(wait_until_finished=True)
         
         """
         Limits Enabled Set
         """
         zctrl.LimitsEnabledSet(limit_z_status=True)
         limit_z_status = zctrl.LimitsEnabledGet()
-        print("Z-Controller Z Limits Enabled/Disabled")
-        print("Z limits " + ["disabled","enabled"][limit_z_status])
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Z-Controller Z Limits Enabled/Disabled")
+            print("Z limits " + ["disabled","enabled"][limit_z_status])
+            print("----------------------------------------------------------------------")
         
         """
         Limits Set/Get
         """
         zctrl.LimitsSet(200e-9, -210e-9)
         z_high_limit, z_low_limit = zctrl.LimitsGet()
-        print("Z-Controller Z Limits")
-        print("Z high limit: " + str(z_high_limit) + " m")
-        print("Z low limit:  " + str(z_low_limit) + " m")
-        print("----------------------------------------------------------------------")
+        if(debug):
+            print("Z-Controller Z Limits")
+            print("Z high limit: " + str(z_high_limit) + " m")
+            print("Z low limit:  " + str(z_low_limit) + " m")
+            print("----------------------------------------------------------------------")
         
         """
         Z Controller Status
         """
         _,status_string = zctrl.StatusGet()
-        print("Z-Controller Status")
-        print("Controller status: " + status_string)
-        print("----------------------------------------------------------------------")
-        
-    except Exception as e:
-        print(e)
+        if(debug):
+            print("Z-Controller Status")
+            print("Controller status: " + status_string)
+            print("----------------------------------------------------------------------")
+        
+    except:
+        NTCP.close_connection()
+        return(traceback.format_exc())
     
-    NTCP.close_connection()
+    NTCP.close_connection()
+    return "success"
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP/nanonisTCP.py` & `nanonistcp-1.1.2/nanonisTCP/nanonisTCP.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 """
 
 import struct
 import socket
 
 
 class nanonisTCP:
-    def __init__(self, IP='127.0.0.1', PORT=6501, max_buf_size=200):
+    def __init__(self, IP='127.0.0.1', PORT=6501, max_buf_size=200, version=99999999):
         """
         Parameters
         IP              : Listening IP address
         PORT            : Listening Port (check Nanonis File>Settings>TCP)
         max_buf_size    : maximum size of the response message. just make it big
+        version         : Nanonis version. See Nanonis > help > info and take the RT Engine number.
+                          Defaults to the latest version of Nanonis
         """
         self.IP   = IP
         self.PORT = PORT
         self.max_buf_size = max_buf_size
+        self.version = version
         
         self.s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)              # Set up the connection
         self.s.connect((IP, PORT))                                              # Open the TCP connection.
 
     def make_header(self, command_name, body_size, resp=True):
         """
         Parameters
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP.egg-info/PKG-INFO` & `nanonistcp-1.1.2/nanonisTCP.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanonisTCP
-Version: 1.0.2
+Version: 1.1.2
 Summary: python module for communicating via nanonis TCP protocal
 Home-page: https://github.com/New-Horizons-SPM/nanonisTCP
 Author: Julian Ceddia
 Author-email: jdceddia@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/New-Horizons-SPM/nanonisTCP/issues
 Description-Content-Type: text/markdown
@@ -14,38 +14,45 @@
 
 [![DOI](https://zenodo.org/badge/475187257.svg)](https://zenodo.org/badge/latestdoi/475187257)
 # nanonisTCP
 Python module for communicating to nanonis via TCP. I am actively developing this so if you have any requests or find any bugs, feel free to raise an issue.
 
 ### Installing
 
-Clone this repository, navigate to said directory, and run:
-```
-pip install .
-```
+Install with pip:
+```pip install nanonisTCP```
+
+Installing from source:
+Clone the repository, navigate to the root directory and run ```pip install .```
 
 ### Using
 
 The following code demonstrates how to change tip bias.
 
 ```python
 from nanonisTCP import nanonisTCP
 from nanonisTCP.Bias import Bias
 
-TCP_IP  = '127.0.0.1'               # Local host
-TCP_PORT= 6501                      # Check available ports in NANONIS > File > Settings Options > TCP Programming Interface
+TCP_IP  = '127.0.0.1'                               # Local host
+TCP_PORT= 6501                                      # Check available ports in NANONIS > File > Settings Options > TCP Programming Interface
 
-NTCP = nanonisTCP(TCP_IP, TCP_PORT) # This is how you establish a TCP connection. NTCP is the connection handle.
+NTCP = nanonisTCP(TCP_IP, TCP_PORT, version=13520)  # This is how you establish a TCP connection. NTCP is the connection handle.
+                                                    # Check your nanonis version in Nanonis > help > info and enter the RT Engine number
 
-bias = Bias(NTCP)                   # Nanonis Bias Module - Pass in the connection handle
+bias = Bias(NTCP)                                   # Nanonis Bias Module - Pass in the connection handle
 
-bias.Set(1.1)                       # Set bias to 1.1 V
-v = bias.Get()                      # Get the current bias
-print("Bias: " + str(v) + " V")     # Confirm bias has been set
+bias.Set(1.1)                                       # Set bias to 1.1 V
+v = bias.Get()                                      # Get the current bias
+print("Bias: " + str(v) + " V")                     # Confirm bias has been set
 
-NTCP.close_connection()             # Close the connection.
+NTCP.close_connection()                             # Close the connection.
 ```
 
-See any of the xxxTest.py scripts to see how each module can be implemented in more detail
+See any of the xxxTest.py scripts to see how each module can be implemented in more detail.
+
+### Testing
+After installing, you can test any of the modules using the sctipts in the test folder.
+To test all of the modules, run test.py
+<strong>Note that Nanonis must be open for the tests to pass.</strong>
 
 ### Citing
 If you use nanonisTCP, please consider citing it: [10.5281/zenodo.7402664](https://doi.org/10.5281/zenodo.7402664)
```

### Comparing `nanonisTCP-1.0.2/nanonisTCP.egg-info/SOURCES.txt` & `nanonistcp-1.1.2/nanonisTCP.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 LICENSE
 README.md
 setup.py
 nanonisTCP/AutoApproach.py
-nanonisTCP/AutoApproachTest.py
 nanonisTCP/Bias.py
 nanonisTCP/BiasSpectr.py
-nanonisTCP/BiasSpectrTest.py
-nanonisTCP/BiasTest.py
 nanonisTCP/Current.py
-nanonisTCP/CurrentTest.py
 nanonisTCP/FolMe.py
-nanonisTCP/FolMeTest.py
 nanonisTCP/LockIn.py
-nanonisTCP/LockInTest.py
 nanonisTCP/Marks.py
-nanonisTCP/MarksTest.py
 nanonisTCP/Motor.py
-nanonisTCP/MotorTest.py
 nanonisTCP/Osci2T.py
-nanonisTCP/Osci2TTest.py
 nanonisTCP/Pattern.py
 nanonisTCP/Piezo.py
-nanonisTCP/PiezoTest.py
 nanonisTCP/SafeTip.py
-nanonisTCP/SafeTipTest.py
 nanonisTCP/Scan.py
-nanonisTCP/ScanTest.py
 nanonisTCP/Signals.py
-nanonisTCP/SignalsTest.py
 nanonisTCP/TipShaper.py
-nanonisTCP/TipShaperTest.py
 nanonisTCP/UserOut.py
-nanonisTCP/UserOutTest.py
 nanonisTCP/ZController.py
-nanonisTCP/ZControllerTest.py
 nanonisTCP/__init__.py
 nanonisTCP/nanonisTCP.py
 nanonisTCP.egg-info/PKG-INFO
 nanonisTCP.egg-info/SOURCES.txt
 nanonisTCP.egg-info/dependency_links.txt
 nanonisTCP.egg-info/requires.txt
-nanonisTCP.egg-info/top_level.txt
+nanonisTCP.egg-info/top_level.txt
+nanonisTCP/test/AutoApproachTest.py
+nanonisTCP/test/BiasSpectrTest.py
+nanonisTCP/test/BiasTest.py
+nanonisTCP/test/CurrentTest.py
+nanonisTCP/test/FolMeTest.py
+nanonisTCP/test/LockInTest.py
+nanonisTCP/test/MarksTest.py
+nanonisTCP/test/MotorTest.py
+nanonisTCP/test/Osci2TTest.py
+nanonisTCP/test/PiezoTest.py
+nanonisTCP/test/SafeTipTest.py
+nanonisTCP/test/ScanTest.py
+nanonisTCP/test/SignalsTest.py
+nanonisTCP/test/TipShaperTest.py
+nanonisTCP/test/UserOutTest.py
+nanonisTCP/test/ZControllerTest.py
+nanonisTCP/test/__init__.py
+nanonisTCP/test/test.py
```

### Comparing `nanonisTCP-1.0.2/setup.py` & `nanonistcp-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-version = '1.0.2'
+version = '1.1.2'
 
 setup(
     name='nanonisTCP',
     version=version,
     author='Julian Ceddia',
     author_email='jdceddia@gmail.com',
     description='python module for communicating via nanonis TCP protocal',
```

