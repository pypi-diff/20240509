# Comparing `tmp/pyflichub-tcpclient-0.1.8.tar.gz` & `tmp/pyflichub_tcpclient-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflichub-tcpclient-0.1.8.tar", last modified: Fri Oct 20 13:39:58 2023, max compression
+gzip compressed data, was "pyflichub_tcpclient-0.1.9.tar", last modified: Thu May  9 20:33:21 2024, max compression
```

## Comparing `pyflichub-tcpclient-0.1.8.tar` & `pyflichub_tcpclient-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 13:39:58.982036 pyflichub-tcpclient-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 13:39:58.978036 pyflichub-tcpclient-0.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 13:39:58.978036 pyflichub-tcpclient-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/.github/workflows/release-drafter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2023-10-20 13:39:58.982036 pyflichub-tcpclient-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 13:39:58.978036 pyflichub-tcpclient-0.1.8/pyflichub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/pyflichub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/pyflichub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/pyflichub/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/pyflichub/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/pyflichub/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/pyflichub/flichub.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/pyflichub/server_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/pyflichub/server_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-20 13:39:58.000000 pyflichub-tcpclient-0.1.8/pyflichub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 13:39:58.982036 pyflichub-tcpclient-0.1.8/pyflichub_tcpclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2023-10-20 13:39:58.000000 pyflichub-tcpclient-0.1.8/pyflichub_tcpclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-10-20 13:39:58.000000 pyflichub-tcpclient-0.1.8/pyflichub_tcpclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 13:39:58.000000 pyflichub-tcpclient-0.1.8/pyflichub_tcpclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-20 13:39:58.000000 pyflichub-tcpclient-0.1.8/pyflichub_tcpclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-20 13:39:58.000000 pyflichub-tcpclient-0.1.8/pyflichub_tcpclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-10-20 13:39:58.982036 pyflichub-tcpclient-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2023-10-20 13:39:42.000000 pyflichub-tcpclient-0.1.8/tcpserver.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:33:21.989113 pyflichub_tcpclient-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:33:21.985113 pyflichub_tcpclient-0.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:33:21.985113 pyflichub_tcpclient-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/.github/workflows/release-drafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-09 20:33:21.989113 pyflichub_tcpclient-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:33:21.989113 pyflichub_tcpclient-0.1.9/pyflichub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/pyflichub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/pyflichub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/pyflichub/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/pyflichub/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/pyflichub/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/pyflichub/flichub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/pyflichub/server_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/pyflichub/server_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 20:33:21.000000 pyflichub_tcpclient-0.1.9/pyflichub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:33:21.989113 pyflichub_tcpclient-0.1.9/pyflichub_tcpclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-09 20:33:21.000000 pyflichub_tcpclient-0.1.9/pyflichub_tcpclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-09 20:33:21.000000 pyflichub_tcpclient-0.1.9/pyflichub_tcpclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 20:33:21.000000 pyflichub_tcpclient-0.1.9/pyflichub_tcpclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 20:33:21.000000 pyflichub_tcpclient-0.1.9/pyflichub_tcpclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 20:33:21.000000 pyflichub_tcpclient-0.1.9/pyflichub_tcpclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-09 20:33:21.989113 pyflichub_tcpclient-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-09 20:33:11.000000 pyflichub_tcpclient-0.1.9/tcpserver.js
```

### Comparing `pyflichub-tcpclient-0.1.8/.github/release-drafter.yml` & `pyflichub_tcpclient-0.1.9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pyflichub-tcpclient-0.1.8/.github/workflows/codeql-analysis.yml` & `pyflichub_tcpclient-0.1.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pyflichub-tcpclient-0.1.8/.github/workflows/pythonpublish.yml` & `pyflichub_tcpclient-0.1.9/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `pyflichub-tcpclient-0.1.8/.github/workflows/test.yml` & `pyflichub_tcpclient-0.1.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyflichub-tcpclient-0.1.8/.gitignore` & `pyflichub_tcpclient-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyflichub-tcpclient-0.1.8/LICENSE` & `pyflichub_tcpclient-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflichub-tcpclient-0.1.8/PKG-INFO` & `pyflichub_tcpclient-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflichub-tcpclient
-Version: 0.1.8
+Version: 0.1.9
 Summary: Asynchronous Python TCP Client for FlicHub
 Home-page: https://github.com/JohNan/pyflichub-tcpclient
 Author: Johan Nenzén
 Author-email: johan.nanzen@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/JohNan/pyflichub-tcpclient/issues
 Classifier: Framework :: AsyncIO
```

### Comparing `pyflichub-tcpclient-0.1.8/README.md` & `pyflichub_tcpclient-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyflichub-tcpclient-0.1.8/main.py` & `pyflichub_tcpclient-0.1.9/main.py`

 * *Files identical despite different names*

### Comparing `pyflichub-tcpclient-0.1.8/pyflichub/button.py` & `pyflichub_tcpclient-0.1.9/pyflichub/button.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 from datetime import datetime
 
 
 @dataclass
 class FlicButton():
     def __init__(self, bdaddr: str, serial_number: str, color: str, name: str, active_disconnect: bool, connected: bool,
                  ready: bool, battery_status: int, uuid: str, flic_version: int, firmware_version: int, key: str,
-                 passive_mode: bool, battery_timestamp: datetime = None) -> None:
+                 passive_mode: bool, battery_timestamp: datetime = None, boot_id: str = "") -> None:
         self.bdaddr = bdaddr
         self.serial_number = serial_number
         self.color = color
         self.name = name
         self.active_disconnect = active_disconnect
         self.connected = connected
         self.ready = ready
         self.battery_status = battery_status
         self.uuid = uuid
         self.flic_version = flic_version
         self.firmware_version = firmware_version
         self.key = key
         self.passive_mode = passive_mode
         self.battery_timestamp = battery_timestamp
+        self.boot_id = boot_id
```

### Comparing `pyflichub-tcpclient-0.1.8/pyflichub/client.py` & `pyflichub_tcpclient-0.1.9/pyflichub/client.py`

 * *Files identical despite different names*

### Comparing `pyflichub-tcpclient-0.1.8/pyflichub/flichub.py` & `pyflichub_tcpclient-0.1.9/pyflichub/flichub.py`

 * *Files identical despite different names*

### Comparing `pyflichub-tcpclient-0.1.8/pyflichub_tcpclient.egg-info/PKG-INFO` & `pyflichub_tcpclient-0.1.9/pyflichub_tcpclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflichub-tcpclient
-Version: 0.1.8
+Version: 0.1.9
 Summary: Asynchronous Python TCP Client for FlicHub
 Home-page: https://github.com/JohNan/pyflichub-tcpclient
 Author: Johan Nenzén
 Author-email: johan.nanzen@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/JohNan/pyflichub-tcpclient/issues
 Classifier: Framework :: AsyncIO
```

### Comparing `pyflichub-tcpclient-0.1.8/pyflichub_tcpclient.egg-info/SOURCES.txt` & `pyflichub_tcpclient-0.1.9/pyflichub_tcpclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyflichub-tcpclient-0.1.8/setup.cfg` & `pyflichub_tcpclient-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyflichub-tcpclient-0.1.8/tcpserver.js` & `pyflichub_tcpclient-0.1.9/tcpserver.js`

 * *Files identical despite different names*

