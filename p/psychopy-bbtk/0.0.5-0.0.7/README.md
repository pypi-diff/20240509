# Comparing `tmp/psychopy-bbtk-0.0.5.tar.gz` & `tmp/psychopy_bbtk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychopy-bbtk-0.0.5.tar", last modified: Mon Nov 20 17:21:01 2023, max compression
+gzip compressed data, was "psychopy_bbtk-0.0.7.tar", last modified: Thu May  9 18:44:18 2024, max compression
```

## Comparing `psychopy-bbtk-0.0.5.tar` & `psychopy_bbtk-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxr-xr-x   0 mdc        (501) staff       (20)        0 2023-11-20 17:21:01.573476 psychopy-bbtk-0.0.5/
--rw-r--r--   0 mdc        (501) staff       (20)    35149 2022-12-07 21:56:54.000000 psychopy-bbtk-0.0.5/LICENSE
--rw-r--r--   0 mdc        (501) staff       (20)     1784 2023-11-20 17:21:01.573394 psychopy-bbtk-0.0.5/PKG-INFO
--rw-r--r--   0 mdc        (501) staff       (20)      605 2022-12-07 22:06:44.000000 psychopy-bbtk-0.0.5/README.md
-drwxr-xr-x   0 mdc        (501) staff       (20)        0 2023-11-20 17:21:01.571632 psychopy-bbtk-0.0.5/docs/
--rw-r--r--   0 mdc        (501) staff       (20)     2256 2023-11-02 15:11:58.000000 psychopy-bbtk-0.0.5/docs/conf.py
--rw-r--r--   0 mdc        (501) staff       (20)     5173 2023-11-02 15:11:58.000000 psychopy-bbtk-0.0.5/docs/utils.py
-drwxr-xr-x   0 mdc        (501) staff       (20)        0 2023-11-20 17:21:01.572102 psychopy-bbtk-0.0.5/psychopy_bbtk/
--rw-r--r--   0 mdc        (501) staff       (20)    19121 2022-12-07 22:06:44.000000 psychopy-bbtk-0.0.5/psychopy_bbtk/__init__.py
-drwxr-xr-x   0 mdc        (501) staff       (20)        0 2023-11-20 17:21:01.573058 psychopy-bbtk-0.0.5/psychopy_bbtk/components/
--rw-r--r--   0 mdc        (501) staff       (20)     2267 2023-11-20 17:18:02.000000 psychopy-bbtk-0.0.5/psychopy_bbtk/components/tpad.py
--rw-r--r--   0 mdc        (501) staff       (20)     1772 2023-11-02 15:11:58.000000 psychopy-bbtk-0.0.5/psychopy_bbtk/forcePad.py
--rw-r--r--   0 mdc        (501) staff       (20)    12013 2023-11-20 15:45:34.000000 psychopy-bbtk-0.0.5/psychopy_bbtk/tpad.py
-drwxr-xr-x   0 mdc        (501) staff       (20)        0 2023-11-20 17:21:01.572910 psychopy-bbtk-0.0.5/psychopy_bbtk.egg-info/
--rw-r--r--   0 mdc        (501) staff       (20)     1784 2023-11-20 17:21:01.000000 psychopy-bbtk-0.0.5/psychopy_bbtk.egg-info/PKG-INFO
--rw-r--r--   0 mdc        (501) staff       (20)      364 2023-11-20 17:21:01.000000 psychopy-bbtk-0.0.5/psychopy_bbtk.egg-info/SOURCES.txt
--rw-r--r--   0 mdc        (501) staff       (20)        1 2023-11-20 17:21:01.000000 psychopy-bbtk-0.0.5/psychopy_bbtk.egg-info/dependency_links.txt
--rw-r--r--   0 mdc        (501) staff       (20)      107 2023-11-20 17:21:01.000000 psychopy-bbtk-0.0.5/psychopy_bbtk.egg-info/entry_points.txt
--rw-r--r--   0 mdc        (501) staff       (20)       24 2023-11-20 17:21:01.000000 psychopy-bbtk-0.0.5/psychopy_bbtk.egg-info/top_level.txt
--rw-r--r--   0 mdc        (501) staff       (20)     1416 2023-11-20 17:20:28.000000 psychopy-bbtk-0.0.5/pyproject.toml
--rw-r--r--   0 mdc        (501) staff       (20)      103 2023-11-20 17:21:01.573835 psychopy-bbtk-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/docs_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/docs_src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/docs_src/generatePages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/psychopy_bbtk/
+-rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/psychopy_bbtk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/psychopy_bbtk/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/psychopy_bbtk/components/tpad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/psychopy_bbtk/forcePad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/psychopy_bbtk/tpad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-09 18:44:18.000000 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-09 18:44:18.000000 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:44:18.000000 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-09 18:44:18.000000 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 18:44:18.000000 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 18:44:18.000000 psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/tests/test_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/tests/test_builder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:18.704760 psychopy_bbtk-0.0.7/tests/test_coder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/tests/test_coder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-09 18:44:07.000000 psychopy_bbtk-0.0.7/tests/test_coder/test_running_via_liaison.py
```

### Comparing `psychopy-bbtk-0.0.5/LICENSE` & `psychopy_bbtk-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `psychopy-bbtk-0.0.5/PKG-INFO` & `psychopy_bbtk-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychopy-bbtk
-Version: 0.0.5
+Version: 0.0.7
 Summary: Extension package for adding support for BlackBoxToolkit devices to PsychoPy.
 Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/psychopy/psychopy-bbtk
 Project-URL: changelog, https://github.com/psychopy/psychopy-bbtk/blob/main/CHANGELOG.txt
 Project-URL: documentation, https://pages.github.com/psychopy/psychopy-bbtk
 Project-URL: repository, https://github.com/psychopy/psychopy-bbtk
@@ -16,14 +16,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: docs
+Requires-Dist: psychopy; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: furo; extra == "docs"
+Provides-Extra: tests
+Requires-Dist: psychopy; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
 
 # psychopy-bbtk
 Extension package for adding support for devices by [Black Box ToolKit Ltd.](https://www.blackboxtoolkit.com/) to 
 PsychoPy.
 
 ## Supported Devices
```

### Comparing `psychopy-bbtk-0.0.5/README.md` & `psychopy_bbtk-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `psychopy-bbtk-0.0.5/psychopy_bbtk/__init__.py` & `psychopy_bbtk-0.0.7/psychopy_bbtk/__init__.py`

 * *Files identical despite different names*

### Comparing `psychopy-bbtk-0.0.5/psychopy_bbtk/forcePad.py` & `psychopy_bbtk-0.0.7/psychopy_bbtk/forcePad.py`

 * *Files identical despite different names*

### Comparing `psychopy-bbtk-0.0.5/psychopy_bbtk/tpad.py` & `psychopy_bbtk-0.0.7/psychopy_bbtk/tpad.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from psychopy.hardware import base, serialdevice as sd, photodiode, button
 from psychopy.hardware.manager import deviceManager, DeviceManager
 from psychopy import logging, layout
 from psychopy.tools import systemtools as st
 import serial
 import re
+import sys
 
 # possible values for self.channel
 channelCodes = {
     'A': "Buttons",
     'C': "Optos",
     'M': "Voice key",
     'T': "TTL in",
@@ -31,71 +32,107 @@
     '0': "Button 2",
     '[': "Opto 1",
     ']': "Opto 2",
 }
 
 # define format for messages
 messageFormat = (
-    r"([{channels}]) ([{states}]) ([{buttons}]) (\d*)"
+    r"([{channels}]) ([{states}]) ([{buttons}]) (\d\d*)"
 ).format(
     channels="".join(re.escape(key) for key in channelCodes),
     states="".join(re.escape(key) for key in stateCodes),
     buttons="".join(re.escape(key) for key in buttonCodes)
 )
 
 
 def splitTPadMessage(message):
     return re.match(messageFormat, message).groups()
 
 
 class TPadPhotodiodeGroup(photodiode.BasePhotodiodeGroup):
-    def __init__(self, pad, channels):
+    def __init__(self, pad, channels, threshold=None, pos=None, size=None, units=None):
         _requestedPad = pad
         # try to get associated tpad
         if isinstance(_requestedPad, str):
             # try getting by name
             pad = DeviceManager.getDevice(pad)
             # if failed, try getting by port
             if pad is None:
                 pad = DeviceManager.getDeviceBy("portString", _requestedPad, deviceClass="psychopy_bbtk.tpad.TPad")
         # if still failed, make one
         if pad is None:
-            pad = DeviceManager.addDevice(
-                deviceClass="psychopy_bbtk.tpad.TPad",
-                deviceName=_requestedPad,
-                port=_requestedPad
-            )
+            pad = TPad(port=_requestedPad)
 
         # reference self in pad
         pad.nodes.append(self)
         # initialise base class
-        photodiode.BasePhotodiodeGroup.__init__(self, channels=channels)
         self.parent = pad
+        photodiode.BasePhotodiodeGroup.__init__(
+            self, channels=channels, threshold=threshold, pos=pos, size=size, units=units
+        )
+
+    def isSameDevice(self, other):
+        """
+        Determine whether this object represents the same physical device as a given other object.
+
+        Parameters
+        ----------
+        other : TPadPhotodiodeGroup, dict
+            Other TPadPhotodiodeGroup to compare against, or a dict of params (which much include
+            `port` or `pad` as a key)
+
+        Returns
+        -------
+        bool
+            True if the two objects represent the same physical device
+        """
+        if isinstance(other, type(self)):
+            # if given another TPadButtonGroup, compare parent boxes
+            other = other.parent
+        elif isinstance(other, dict) and "pad" in other:
+            # create copy of dict so we don't affect the original
+            other = other.copy()
+            # if given a dict, make sure we have a `port` rather than a `pad`
+            other['port'] = other['pad']
+        # use parent's comparison method
+        return self.parent.isSameDevice(other)
 
     @staticmethod
     def getAvailableDevices():
         devices = []
         # iterate through profiles of all serial port devices
         for profile in TPad.getAvailableDevices():
             devices.append({
                 'deviceName': profile['deviceName'] + "_photodiodes",
                 'pad': profile['port'],
                 'channels': 2,
             })
 
         return devices
 
-    def setThreshold(self, threshold, channels=(1, 2)):
-        self._threshold = threshold
+    def _setThreshold(self, threshold, channel):
+        if threshold is None:
+            return
+        # enter command mode
         self.parent.setMode(0)
-        for n in channels:
-            self.parent.sendMessage(f"AAO{n} {threshold}")
-            self.parent.pause()
+        # send command to set threshold
+        self.parent.sendMessage(f"AAO{channel+1} {threshold}")
+        resp = self.parent.awaitResponse()
+        # with this threshold, is the photodiode returning True?
+        measurement = None
+        if resp is not None:
+            if resp.strip() == "1":
+                measurement = True
+            if resp.strip() == "0":
+                measurement = False
+        # return to sampling mode
         self.parent.setMode(3)
 
+        return measurement
+
     def resetTimer(self, clock=logging.defaultClock):
         self.parent.resetTimer(clock=clock)
 
     def dispatchMessages(self):
         """
         Dispatch messages from parent TPad to this photodiode group
 
@@ -123,58 +160,86 @@
         #     "TPadPhotometer {} received non-photometer message: {}"
         # ).format(self.number, message)
         # assert number == str(self.number), (
         #     "TPadPhotometer {} received message intended for photometer {}: {}"
         # ).format(self.number, number, message)
         # create PhotodiodeResponse object
         resp = photodiode.PhotodiodeResponse(
-            time, channel, state, threshold=self.getThreshold()
+            t=time, channel=channel, value=state, threshold=self.getThreshold(channel-1)
         )
 
         return resp
 
     def findPhotodiode(self, win, channel):
         # set mode to 3
         self.parent.setMode(3)
         self.parent.pause()
         # continue as normal
         return photodiode.BasePhotodiodeGroup.findPhotodiode(self, win, channel)
 
     def findThreshold(self, win, channel):
-        # set mode to 3
-        self.parent.setMode(3)
-        self.parent.pause()
+        # set mode to 0 and lock it so mode doesn't change during setThreshold calls
+        self.parent.setMode(0)
+        self.parent.lockMode()
         # continue as normal
-        return photodiode.BasePhotodiodeGroup.findThreshold(self, win, channel)
+        resp = photodiode.BasePhotodiodeGroup.findThreshold(self, win, channel)
+        self._setThreshold(0, channel=1)
+        # set back to mode 3
+        self.parent.unlockMode()
+        self.parent.setMode(3)
+
+        return resp
 
 
 class TPadButtonGroup(button.BaseButtonGroup):
     def __init__(self, pad, channels=9):
         _requestedPad = pad
         # try to get associated tpad
         if isinstance(_requestedPad, str):
             # try getting by name
             pad = DeviceManager.getDevice(pad)
             # if failed, try getting by port
             if pad is None:
                 pad = DeviceManager.getDeviceBy("portString", _requestedPad, deviceClass="psychopy_bbtk.tpad.TPad")
         # if still failed, make one
         if pad is None:
-            pad = DeviceManager.addDevice(
-                deviceClass="psychopy_bbtk.tpad.TPad",
-                deviceName=_requestedPad,
-                port=_requestedPad
-            )
+            pad = TPad(port=_requestedPad)
 
         # reference self in pad
         pad.nodes.append(self)
         # initialise base class
         button.BaseButtonGroup.__init__(self, channels=channels)
         self.parent = pad
 
+    def isSameDevice(self, other):
+        """
+        Determine whether this object represents the same physical device as a given other object.
+
+        Parameters
+        ----------
+        other : TPadButtonGroup, dict
+            Other TPadButtonGroup to compare against, or a dict of params (which must include
+            `port` or `pad` as a key)
+
+        Returns
+        -------
+        bool
+            True if the two objects represent the same physical device
+        """
+        if isinstance(other, type(self)):
+            # if given another TPadButtonGroup, compare parent boxes
+            other = other.parent
+        elif isinstance(other, dict) and "pad" in other:
+            # create copy of dict so we don't affect the original
+            other = other.copy()
+            # if given a dict, make sure we have a `port` rather than a `pad`
+            other['port'] = other['pad']
+        # use parent's comparison method
+        return self.parent.isSameDevice(other)
+
     def dispatchMessages(self):
         """
         Dispatch messages from parent TPad to this button group
 
         Returns
         -------
         bool
@@ -190,17 +255,19 @@
         # assert isinstance(message, (tuple, list)) and len(message) == 4
         device, state, channel, time = message
         # convert state to bool
         if state == "P":
             state = True
         elif state == "R":
             state = False
+        # convert channel to int
+        channel = int(channel)
         
         resp = button.ButtonResponse(
-            time, channel, state
+            t=time, channel=channel, value=state
         )
 
         return resp
     
     @staticmethod
     def getAvailableDevices():
         devices = []
@@ -225,63 +292,82 @@
 
 class TPad(sd.SerialDevice):
     def __init__(
             self, port=None, baudrate=115200,
             byteSize=8, stopBits=1,
             parity="N",  # 'N'one, 'E'ven, 'O'dd, 'M'ask,
             eol=b"\n",
-            maxAttempts=1, pauseDuration=1/240,
+            maxAttempts=1, pauseDuration=1/1000,
             checkAwake=True
     ):
         # get port if not given
         if port is None:
             port = self._detectComPort()[0]
+        # initial value for last timer reset
+        self._lastTimerReset = logging.defaultClock._timeAtLastReset
+        # dict of responses by timestamp
+        self.messages = {}
+        # indicator that a message dispatch is currently in progress (prevents threaded 
+        # dispatch loops from tripping over one another)
+        self._dispatchInProgress = False
+        # nodes
+        self.nodes = []
+        # attribute to keep track of mode state
+        self._mode = None
+        self._modeLock = False
         # initialise serial
         sd.SerialDevice.__init__(
             self, port=port, baudrate=baudrate,
             byteSize=byteSize, stopBits=stopBits,
             parity=parity,  # 'N'one, 'E'ven, 'O'dd, 'M'ask,
             eol=eol,
             maxAttempts=maxAttempts, pauseDuration=pauseDuration,
             checkAwake=checkAwake
         )
-        # nodes
-        self.nodes = []
-
-        # dict of responses by timestamp
-        self.messages = {}
         # reset timer
-        self._lastTimerReset = None
         self.resetTimer()
 
+    def close(self):
+        # set mode to 0 on exit
+        self.setMode(0)
+        # close
+        sd.SerialDevice.close(self)
+
     @staticmethod
     def getAvailableDevices():
         devices = []
-        # iterate through profiles of all serial port devices
-        for profile in st.systemProfilerWindowsOS(
-            classid="{4d36e978-e325-11ce-bfc1-08002be10318}",
-            connected=True
-        ):
-            # skip non-bbtk profiles
-            if "BBTKTPAD" not in profile['Instance ID']:
-                continue
-            # find "COM" in profile description
-            desc = profile['Device Description']
-            start = desc.find("COM") + 3
-            end = desc.find(")", start)
-            # if there's no reference to a COM port, skip
-            if -1 in (start, end):
-                continue
-            # get COM port number
-            num = desc[start:end]
-
-            devices.append({
-                'deviceName': profile['Instance ID'],
-                'port': f"COM{num}",
-            })
+        if sys.platform == "win32":  
+            # iterate through profiles of all serial port devices
+            for profile in st.systemProfilerWindowsOS(
+                classid="{4d36e978-e325-11ce-bfc1-08002be10318}",
+                connected=True
+            ):
+                # skip non-bbtk profiles
+                if "BBTKTPAD" not in profile['Instance ID']:
+                    continue
+                # find "COM" in profile description
+                desc = profile['Device Description']
+                start = desc.find("COM") + 3
+                end = desc.find(")", start)
+                # if there's no reference to a COM port, skip
+                if -1 in (start, end):
+                    continue
+                # get COM port number
+                num = desc[start:end]
+    
+                devices.append({
+                    'deviceName': profile['Instance ID'],
+                    'port': f"COM{num}",
+                })
+        else:
+            for profile in sd.SerialDevice.getAvailableDevices():
+                devices.append({
+                    'deviceName': profile['deviceName'],
+                    'port': profile['port'],
+                })
 
         return devices
 
     def addListener(self, listener):
         """
         Add a listener, which will receive all the messages dispatched by this TPad.
 
@@ -291,14 +377,19 @@
             Object to duplicate messages to when dispatched by this TPad.
         """
         # add listener to all nodes
         for node in self.nodes:
             node.addListener(listener)
 
     def dispatchMessages(self):
+        # do nothing if there's already a dispatch in progress
+        if self._dispatchInProgress:
+            return
+        # mark that a dispatch has begun
+        self._dispatchInProgress = True
         # get data from box
         self.pause()
         data = self.getResponse(length=2)
         self.pause()
         # parse lines
         for line in data:
             if re.match(messageFormat, line):
@@ -322,53 +413,124 @@
                         continue
                     # if device is M, dispatch only to voice keys
                     if device == "M" and not isinstance(node, TPadVoicekey):
                         continue
                     # dispatch to node
                     message = node.parseMessage(parts)
                     node.receiveMessage(message)
+                else:
+                    logging.debug(f"Received unparsable message from TPad: {line}")
+        # mark that a dispatch has finished
+        self._dispatchInProgress = False
 
     @staticmethod
     def _detectComPort():
         # find available devices
         available = TPad.getAvailableDevices()
         # error if there are none
         if not available:
             raise ConnectionError(
                 "Could not find any TPad."
             )
         # get all available ports
         return [profile['port'] for profile in available]
 
     def setMode(self, mode):
-        self.getResponse()
+        self.dispatchMessages()
+        # skip if mode is locked
+        if self._modeLock:
+            return
+        # store requested mode
+        self._mode = mode
         # exit out of whatever mode we're in (effectively set it to 0)
         self.sendMessage("X")
-        self.pause()
-        # set mode
-        self.sendMessage(f"MOD{mode}")
-        self.pause()
-        # clear messages
-        self.getResponse()
+        self.awaitResponse()
+        if mode > 0:
+            # set mode
+            self.sendMessage(f"MOD{mode}")
+            self.awaitResponse()
+
+    def getMode(self):
+        return self._mode
+
+    def lockMode(self):
+        """
+        Temporarily lock to the current mode, meaning that subsequent called to `setMode` will
+        return with no effect until `unlockMode` is called.
+
+        Returns
+        -------
+        int
+            Current mode
+        """
+        self._modeLock = True
+
+        return self.getMode()
+
+    def unlockMode(self):
+        """
+        Unlock the mode, allowing `setMode` to be called and to have an effect.
+
+        Returns
+        -------
+        int
+            Current mode
+        """
+        self._modeLock = False
+
+        return self.getMode()
 
     def isAwake(self):
         self.setMode(0)
-        self.pause()
         # call help and get response
         self.sendMessage("HELP")
-        self.pause()  # or response won't be ready
-        resp = self.getResponse()  # get all chars (a usage message)
+        resp = self.awaitResponse(multiline=True)
         # set to mode 3
         self.setMode(3)
         return bool(resp)
 
-    def resetTimer(self, clock=logging.defaultClock):
-        # enter settings mode
+    def checkSpeed(self, target=5/1000):
+        """
+        Parameters
+        ----------
+        target : float
+            Target time (s) which a single request should take to return.
+
+        Returns
+        -------
+        bool
+            True if average time to return was less than the target time
+        float
+            Average time taken to return
+        """
+        import time
+        # enter command mode
         self.setMode(0)
+        # repeat 25 times...
+        times = []
+        for n in range(25):
+            # start timing
+            start = time.time()
+            # send commands
+            self.sendMessage("FIRM")
+            # what did we get?
+            self.awaitResponse()
+            # how long did it take?
+            times.append(time.time() - start)
+        # average times
+        avg = sum(times) / len(times)
+        # return to data mode
+        self.setMode(3)
+        self.awaitResponse()
+        # are we below the target?
+        valid = avg <= target
+
+        return valid, avg
+
+    def resetTimer(self, clock=logging.defaultClock):
+        # make sure we're in mode 3
+        if self.getMode() != 3:
+            self.setMode(3)
         # send reset command
-        self.sendMessage(f"REST")
+        self.sendMessage("R")
         # store time
         self._lastTimerReset = clock.getTime(format=float)
-        # allow time to process
-        self.pause()
-        # reset mode
-        self.setMode(3)
```

### Comparing `psychopy-bbtk-0.0.5/psychopy_bbtk.egg-info/PKG-INFO` & `psychopy_bbtk-0.0.7/psychopy_bbtk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychopy-bbtk
-Version: 0.0.5
+Version: 0.0.7
 Summary: Extension package for adding support for BlackBoxToolkit devices to PsychoPy.
 Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/psychopy/psychopy-bbtk
 Project-URL: changelog, https://github.com/psychopy/psychopy-bbtk/blob/main/CHANGELOG.txt
 Project-URL: documentation, https://pages.github.com/psychopy/psychopy-bbtk
 Project-URL: repository, https://github.com/psychopy/psychopy-bbtk
@@ -16,14 +16,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: docs
+Requires-Dist: psychopy; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: furo; extra == "docs"
+Provides-Extra: tests
+Requires-Dist: psychopy; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
 
 # psychopy-bbtk
 Extension package for adding support for devices by [Black Box ToolKit Ltd.](https://www.blackboxtoolkit.com/) to 
 PsychoPy.
 
 ## Supported Devices
```

### Comparing `psychopy-bbtk-0.0.5/pyproject.toml` & `psychopy_bbtk-0.0.7/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psychopy-bbtk"
-version = "0.0.5"
+version = "0.0.7"
 description = "Extension package for adding support for BlackBoxToolkit devices to PsychoPy."
 readme = "README.md"
 requires-python = ">= 3.7"
 license = {text = "GNU General Public License v3 (GPLv3)"}
 authors = [
   { name = "Jon Peirce", email = "jon@opensceincetools.org" },
   { name = "Matthew Cutone", email = "mcutone@opensceincetools.org" },
@@ -28,9 +28,29 @@
 urls.changelog = "https://github.com/psychopy/psychopy-bbtk/blob/main/CHANGELOG.txt"
 urls.documentation = "https://pages.github.com/psychopy/psychopy-bbtk"
 urls.repository = "https://github.com/psychopy/psychopy-bbtk"
 
 [tool.setuptools.packages.find]
 where = ["",]
 
+[project.optional-dependencies]
+# dependencies for building the docs
+docs = [
+  "psychopy",
+  "sphinx",
+  "furo",
+]
+# dependencies for running the test suite
+tests = [
+  "psychopy",
+  "pytest",
+]
+
 [project.entry-points."psychopy.experiment.components"]
-TPadButtonBoxBackend = "psychopy_bbtk.components.tpad:TPadButtonBoxBackend"
+TPadButtonBoxBackend = "psychopy_bbtk.components.tpad:TPadButtonBoxBackend"
+
+[project.entry-points."psychopy.hardware.bbtk"]
+TPadPhotodiodeGroup = "psychopy_bbtk.tpad:TPadPhotodiodeGroup"
+TPadButtonGroup = "psychopy_bbtk.tpad:TPadButtonGroup"
+TPadVoiceKey = "psychopy_bbtk.tpad:TPadVoiceKey"
+TPad = "psychopy_bbtk.tpad:TPad"
+BBTKForcePad = "psychopy_bbtk.forcePad:BBTKForcePad"
```

