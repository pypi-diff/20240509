# Comparing `tmp/xyscreens-0.1.1.tar.gz` & `tmp/xyscreens-0.1.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyscreens-0.1.1.tar", last modified: Wed May  8 14:25:36 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `xyscreens-0.1.1.tar` & `xyscreens-0.1.2.dev1.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:25:36.630071 xyscreens-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 14:25:30.000000 xyscreens-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-08 14:25:36.626071 xyscreens-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-08 14:25:30.000000 xyscreens-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-08 14:25:30.000000 xyscreens-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:25:36.630071 xyscreens-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:25:36.626071 xyscreens-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-05-08 14:25:30.000000 xyscreens-0.1.1/tests/test_xyscreens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:25:36.626071 xyscreens-0.1.1/xyscreens/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 14:25:30.000000 xyscreens-0.1.1/xyscreens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-08 14:25:30.000000 xyscreens-0.1.1/xyscreens/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:25:30.000000 xyscreens-0.1.1/xyscreens/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-05-08 14:25:30.000000 xyscreens-0.1.1/xyscreens/xyscreens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:25:36.626071 xyscreens-0.1.1/xyscreens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-08 14:25:36.000000 xyscreens-0.1.1/xyscreens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-08 14:25:36.000000 xyscreens-0.1.1/xyscreens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:25:36.000000 xyscreens-0.1.1/xyscreens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 14:25:36.000000 xyscreens-0.1.1/xyscreens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 14:25:36.000000 xyscreens-0.1.1/xyscreens.egg-info/top_level.txt
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/_version.py
+-rw-r--r--   0        0        0    48808 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/usb-rs485.png
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/tests/__init__.py
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/tests/test_xyscreens.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/xyscreens/__init__.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/xyscreens/__main__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/xyscreens/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/xyscreens/py.typed
+-rw-r--r--   0        0        0    14254 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/xyscreens/xyscreens.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/LICENSE
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/README.md
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 xyscreens-0.1.2.dev1/PKG-INFO
```

### Comparing `xyscreens-0.1.1/LICENSE` & `xyscreens-0.1.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `xyscreens-0.1.1/PKG-INFO` & `xyscreens-0.1.2.dev1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: xyscreens
-Version: 0.1.1
-Summary: Library to control XY Screens projector screens and projector lifts.
-Author: Rogier van Staveren
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/rrooggiieerr/xyscreens.py
-Project-URL: Bug Tracker, https://github.com/rrooggiieerr/xyscreens.py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyserial>=3.5
-Requires-Dist: pyserial_asyncio>=0.6
-
 # Python library to control XY Screens projector screens and lifts
 
 ![Python][python-shield]
 [![GitHub Release][releases-shield]][releases]
 [![Licence][license-shield]][license]
 [![Maintainer][maintainer-shield]][maintainer]  
 [![Github Sponsors][github-shield]][github]
@@ -84,26 +66,26 @@
 `pip3 install xyscreens`
 
 ## `xyscreens` CLI
 
 You can use the Python XY Screens library directly from the command line to move your screen up or
 down or to stop the screen using the following syntax:
 
-Move the screen down: `python3 -m xyscreens <serial port> <time> down`  
-Stop the screen: `python3 -m xyscreens <serial port> <time> stop`  
-Move the screen up: `python3 -m xyscreens <serial port> <time> up`
+Move the screen down: `python3 -m xyscreens <serial port> <duration> down`  
+Stop the screen: `python3 -m xyscreens <serial port> <duration> stop`  
+Move the screen up: `python3 -m xyscreens <serial port> <duration> up`
 
-Where `<time>` is the time in seconds to move the screen down, respectively up. The process will
-wait till the screen is down/up and show the progress.
+Where `<duration>` is the time in seconds to move the screen up or down. The process will wait till
+the screen is up or down and show the progress.
 
 ### Troubleshooting
 
 You can add the `--debug` flag to any CLI command to get a more details on what's going on. Like so:
 
-`python3 -m xyscreens <serial port> <time> down --debug`
+`python3 -m xyscreens <serial port> <duration> down --debug`
 
 ## Support my work
 
 Do you enjoy using this Python library? Then consider supporting my work using one of the following
 platforms, your donation is greatly appreciated and keeps me motivated:
 
 [![Github Sponsors][github-shield]][github]
```

### Comparing `xyscreens-0.1.1/README.md` & `xyscreens-0.1.2.dev1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.3
+Name: xyscreens
+Version: 0.1.2.dev1
+Summary: Library to control XY Screens projector screens and lifts.
+Project-URL: Homepage, https://github.com/rrooggiieerr/xyscreens.py
+Project-URL: Issues, https://github.com/rrooggiieerr/xyscreens.py/issues
+Author-email: Rogier van Staveren <rogier@batoid.com>
+License: Apache-2.0
+License-File: LICENSE
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.11
+Requires-Dist: pyserial-asyncio>=0.6
+Requires-Dist: pyserial>=3.5
+Description-Content-Type: text/markdown
+
 # Python library to control XY Screens projector screens and lifts
 
 ![Python][python-shield]
 [![GitHub Release][releases-shield]][releases]
 [![Licence][license-shield]][license]
 [![Maintainer][maintainer-shield]][maintainer]  
 [![Github Sponsors][github-shield]][github]
@@ -66,26 +88,26 @@
 `pip3 install xyscreens`
 
 ## `xyscreens` CLI
 
 You can use the Python XY Screens library directly from the command line to move your screen up or
 down or to stop the screen using the following syntax:
 
-Move the screen down: `python3 -m xyscreens <serial port> <time> down`  
-Stop the screen: `python3 -m xyscreens <serial port> <time> stop`  
-Move the screen up: `python3 -m xyscreens <serial port> <time> up`
+Move the screen down: `python3 -m xyscreens <serial port> <duration> down`  
+Stop the screen: `python3 -m xyscreens <serial port> <duration> stop`  
+Move the screen up: `python3 -m xyscreens <serial port> <duration> up`
 
-Where `<time>` is the time in seconds to move the screen down, respectively up. The process will
-wait till the screen is down/up and show the progress.
+Where `<duration>` is the time in seconds to move the screen up or down. The process will wait till
+the screen is up or down and show the progress.
 
 ### Troubleshooting
 
 You can add the `--debug` flag to any CLI command to get a more details on what's going on. Like so:
 
-`python3 -m xyscreens <serial port> <time> down --debug`
+`python3 -m xyscreens <serial port> <duration> down --debug`
 
 ## Support my work
 
 Do you enjoy using this Python library? Then consider supporting my work using one of the following
 platforms, your donation is greatly appreciated and keeps me motivated:
 
 [![Github Sponsors][github-shield]][github]
```

### Comparing `xyscreens-0.1.1/tests/test_xyscreens.py` & `xyscreens-0.1.2.dev1/tests/test_xyscreens.py`

 * *Files identical despite different names*

### Comparing `xyscreens-0.1.1/xyscreens/__main__.py` & `xyscreens-0.1.2.dev1/xyscreens/__main__.py`

 * *Files identical despite different names*

### Comparing `xyscreens-0.1.1/xyscreens/xyscreens.py` & `xyscreens-0.1.2.dev1/xyscreens/xyscreens.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,18 +57,18 @@
 
 
 class XYScreens:
     "XYScreens class for controlling XY Screens projector screens and projector lifts."
 
     # The serial port where the RS-485 interface and screen is connected to.
     _serial_port: str | None = None
-    # Time in seconds for the screen to go up.
-    _time_up: float
-    # Time in seconds for the screen to go down.
-    _time_down: float
+    # The amount of time in seconds it takes the cover to close from the fully-open state.
+    _close_duration: float
+    # The amount of time in seconds it takes the screen to open up from the fully-closed state.
+    _open_duration: float
 
     # Current state of the screen. Defaults to Up when object is created.
     _state: XYScreensState = XYScreensState.UP
     # Position of the screen where 0.0 is totally up and 100.0 is fully down.
     _position: float = 0.0
     # Timestamp when the up or down command has been executed.
     _timestamp: float
@@ -77,36 +77,38 @@
     _callbacks: list[Any] | None = None
     # The task that handles the set position functionality in async mode.
     _set_position_task: asyncio.Task | None = None
 
     def __init__(
         self,
         serial_port: str,  # The serial port where the RS-485 interface and screen is connected to.
-        time_down: float,  # Time in seconds for the screen to go down.
-        time_up: float | None = None,  # Time in seconds for the screen to go up.
+        open_duration: float,  # Duration in seconds for the screen to go down.
+        close_duration: (
+            float | None
+        ) = None,  # Duration in seconds for the screen to go up.
         position: float = 0.0,  # Position of the screen where 0.0 is totally up and 100.0 is
         # fully down.
     ):
         "Initialises the XYScreens object."
         # Validate the different arguments.
         assert serial_port is not None
-        assert time_down > 0.0
-        assert time_up is None or time_up > 0.0
+        assert open_duration > 0.0
+        assert close_duration is None or close_duration > 0.0
 
         self._serial_port = serial_port
-        # Set the time for the screen to go down.
-        self._time_down = time_down
+        # Set the duration for the screen to go down.
+        self._open_duration = open_duration
 
-        # Set the time for the screen to go up.
-        if time_up is not None:
-            self._time_up = time_up
-        # If no time for the screen to go up is given use the same value as the time for the screen
-        # to go down.
+        # Set the duration for the screen to go up.
+        if close_duration is not None:
+            self._close_duration = close_duration
+        # If no duration for the screen to go up is given use the same value as the duration for
+        # the screen to go down.
         else:
-            self._time_up = time_down
+            self._close_duration = open_duration
 
         # Set the initial position of the screen.
         self.restore_position(position)
 
     def restore_position(self, position: float) -> None:
         """
         Restores the position of the screen, mainly introduced to restore the screen state in Home
@@ -212,21 +214,21 @@
 
     def update_status(self) -> Tuple[XYScreensState, float]:
         """
         Calculates and returns the status and position of the screen based on the direction the
         screen is moving.
         """
         if self._state == XYScreensState.DOWNWARD:
-            position = ((time.time() - self._timestamp) / self._time_down) * 100.0
+            position = ((time.time() - self._timestamp) / self._open_duration) * 100.0
             if position >= 100.0:
                 self._state = XYScreensState.DOWN
                 position = 100.0
             self._position = position
         elif self._state == XYScreensState.UPWARD:
-            position = ((time.time() - self._timestamp) / self._time_up) * 100.0
+            position = ((time.time() - self._timestamp) / self._close_duration) * 100.0
             position = 100 - position
             if position <= 0.0:
                 self._state = XYScreensState.UP
                 position = 0.0
             self._position = position
 
         return (self._state, self._position)
@@ -244,15 +246,15 @@
 
     def _post_up(self) -> bool:
         if self._state is XYScreensState.DOWNWARD:
             self.update_status()
 
         if self._state not in (XYScreensState.UPWARD, XYScreensState.UP):
             self._timestamp = time.time() - (
-                (100.0 - self._position) * (self._time_up / 100)
+                (100.0 - self._position) * (self._close_duration / 100)
             )
             logger.debug("up() time stamp: %s", self._timestamp)
             logger.debug("up() position: %s", self._position)
             self._state = XYScreensState.UPWARD
             return True
 
         return False
@@ -305,15 +307,17 @@
         return False
 
     def _post_down(self) -> bool:
         if self._state is XYScreensState.UPWARD:
             self.update_status()
 
         if self._state not in (XYScreensState.DOWNWARD, XYScreensState.DOWN):
-            self._timestamp = time.time() - (self._position * (self._time_down / 100))
+            self._timestamp = time.time() - (
+                self._position * (self._open_duration / 100)
+            )
             logger.debug("down() time stamp: %s", self._timestamp)
             logger.debug("down() position: %s", self._position)
             self._state = XYScreensState.DOWNWARD
             return True
 
         return False
 
@@ -331,47 +335,42 @@
         return await self.async_set_position(100.0)
 
     def _target_position_reached(self, target_position: float) -> bool:
         """Calculates if the target position has been reached."""
         self.update_status()
         self._update_callbacks()
 
-        if self._state == XYScreensState.DOWNWARD and self._position >= target_position:
-            return True
-        if self._state == XYScreensState.UPWARD and self._position <= target_position:
-            return True
-        if self._state not in (
-            XYScreensState.UPWARD,
-            XYScreensState.DOWNWARD,
-        ):
-            return True
+        if self._state == XYScreensState.DOWNWARD:
+            return self._position >= target_position
+        if self._state == XYScreensState.UPWARD:
+            return self._position <= target_position
 
-        # Target position is not yet reached
-        return False
+        # Target position has been reached
+        return True
 
     def set_position(self, target_position: float) -> bool:
         """Initiates the screen to move to a given position."""
         assert 0.0 <= target_position <= 100.0
 
         if round(self._position) == round(target_position):
             return self.stop()
 
         if self._position < target_position and not self.down():
             return False
         if self._position > target_position and not self.up():
             return False
 
-        sleep_time = min(self._time_up, self._time_down) / 1000.0
+        sleep_duration = min(self._close_duration, self._open_duration) / 1000.0
         while True:
             if self._target_position_reached(target_position):
                 if self._state in (XYScreensState.UPWARD, XYScreensState.DOWNWARD):
                     self.stop()
                 break
 
-            time.sleep(sleep_time)
+            time.sleep(sleep_duration)
 
         return True
 
     async def async_set_position(self, target_position: float) -> bool:
         """Initiates the screen to move to a given position."""
         assert 0.0 <= target_position <= 100.0
 
@@ -394,25 +393,25 @@
         self._set_position_task = asyncio.create_task(
             self._set_position_coroutine(target_position)
         )
 
         return True
 
     async def _set_position_coroutine(self, target_position: float):
-        sleep_time = min(self._time_up, self._time_down) / 1000.0
+        sleep_duration = min(self._close_duration, self._open_duration) / 1000.0
         while True:
             self._update_callbacks()
 
             if self._target_position_reached(target_position):
                 if self._state in (XYScreensState.UPWARD, XYScreensState.DOWNWARD):
                     await self._async_send_command(XYScreensCommand.STOP.to_bytes())
                     self._post_stop()
                 break
 
-            await asyncio.sleep(sleep_time)
+            await asyncio.sleep(sleep_duration)
 
     def state(self) -> XYScreensState:
         "Returns the current state of the screen."
         (state, _) = self.update_status()
 
         return state
```

