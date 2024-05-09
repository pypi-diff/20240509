# Comparing `tmp/linknlink-0.2.3.tar.gz` & `tmp/linknlink-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linknlink-0.2.3.tar", last modified: Tue May  7 02:09:45 2024, max compression
+gzip compressed data, was "linknlink-0.2.4.tar", last modified: Thu May  9 03:44:24 2024, max compression
```

## Comparing `linknlink-0.2.3.tar` & `linknlink-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-07 02:09:45.248275 linknlink-0.2.3/
--rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-11-08 09:39:11.000000 linknlink-0.2.3/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      503 2024-05-07 02:09:45.244275 linknlink-0.2.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       77 2023-11-14 06:52:53.000000 linknlink-0.2.3/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-07 02:09:45.244275 linknlink-0.2.3/linknlink/
--rw-rw-r--   0 user      (1000) user      (1000)     4080 2024-04-10 10:04:04.000000 linknlink-0.2.3/linknlink/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      269 2024-04-02 02:50:19.000000 linknlink-0.2.3/linknlink/const.py
--rw-rw-r--   0 user      (1000) user      (1000)    12633 2024-04-30 13:41:20.000000 linknlink-0.2.3/linknlink/device.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-11-10 07:16:08.000000 linknlink-0.2.3/linknlink/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1847 2023-11-10 07:09:54.000000 linknlink-0.2.3/linknlink/protocol.py
--rw-rw-r--   0 user      (1000) user      (1000)     9042 2024-05-07 02:07:54.000000 linknlink-0.2.3/linknlink/remote.py
--rw-rw-r--   0 user      (1000) user      (1000)     1774 2024-03-25 06:45:21.000000 linknlink-0.2.3/linknlink/sensor.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-07 02:09:45.244275 linknlink-0.2.3/linknlink.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      503 2024-05-07 02:09:45.000000 linknlink-0.2.3/linknlink.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      369 2024-05-07 02:09:45.000000 linknlink-0.2.3/linknlink.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-07 02:09:45.000000 linknlink-0.2.3/linknlink.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-11-10 08:42:09.000000 linknlink-0.2.3/linknlink.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       18 2024-05-07 02:09:45.000000 linknlink-0.2.3/linknlink.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2024-05-07 02:09:45.000000 linknlink-0.2.3/linknlink.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-07 02:09:45.248275 linknlink-0.2.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      743 2024-05-07 02:09:16.000000 linknlink-0.2.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-09 03:44:24.236424 linknlink-0.2.4/
+-rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-11-08 09:39:11.000000 linknlink-0.2.4/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      503 2024-05-09 03:44:24.236424 linknlink-0.2.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)       77 2023-11-14 06:52:53.000000 linknlink-0.2.4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-09 03:44:24.236424 linknlink-0.2.4/linknlink/
+-rw-rw-r--   0 user      (1000) user      (1000)     4080 2024-04-10 10:04:04.000000 linknlink-0.2.4/linknlink/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      269 2024-04-02 02:50:19.000000 linknlink-0.2.4/linknlink/const.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12633 2024-04-30 13:41:20.000000 linknlink-0.2.4/linknlink/device.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-11-10 07:16:08.000000 linknlink-0.2.4/linknlink/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1847 2023-11-10 07:09:54.000000 linknlink-0.2.4/linknlink/protocol.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9202 2024-05-09 03:43:24.000000 linknlink-0.2.4/linknlink/remote.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1774 2024-03-25 06:45:21.000000 linknlink-0.2.4/linknlink/sensor.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-09 03:44:24.236424 linknlink-0.2.4/linknlink.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      503 2024-05-09 03:44:24.000000 linknlink-0.2.4/linknlink.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      369 2024-05-09 03:44:24.000000 linknlink-0.2.4/linknlink.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-09 03:44:24.000000 linknlink-0.2.4/linknlink.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-11-10 08:42:09.000000 linknlink-0.2.4/linknlink.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       18 2024-05-09 03:44:24.000000 linknlink-0.2.4/linknlink.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2024-05-09 03:44:24.000000 linknlink-0.2.4/linknlink.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-09 03:44:24.240424 linknlink-0.2.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      743 2024-05-09 03:43:59.000000 linknlink-0.2.4/setup.py
```

### Comparing `linknlink-0.2.3/LICENSE` & `linknlink-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.3/linknlink/__init__.py` & `linknlink-0.2.4/linknlink/__init__.py`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.3/linknlink/device.py` & `linknlink-0.2.4/linknlink/device.py`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.3/linknlink/exceptions.py` & `linknlink-0.2.4/linknlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.3/linknlink/protocol.py` & `linknlink-0.2.4/linknlink/protocol.py`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.3/linknlink/remote.py` & `linknlink-0.2.4/linknlink/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,18 @@
         if 20000 <= self.devtype <= 29999:
             packet = struct.pack("<HI", len(data) + 4, command) + data
         else:
             packet = struct.pack("<I", command) + data
         resp = self.send_packet(0x6A, packet)
         e.check_error(resp[0x22:0x24])
         payload = self.decrypt(resp[0x38:])
-        p_len = struct.unpack("<H", payload[:0x2])[0]
-        return payload[0x6 : p_len + 2]
+        if 20000 <= self.devtype <= 29999:
+            p_len = struct.unpack("<H", payload[:0x2])[0]
+            return payload[0x6 : p_len + 2]
+        return payload[0x4:]
     
     def check_sensors(self) -> dict:
         """Return the state of the sensors."""
         resp = self._send(0x24)
         return {
             "envtemp": resp[0x0] + resp[0x1] / 100.0,
             "envhumid": resp[0x2] + resp[0x3] / 100.0,
@@ -101,16 +103,18 @@
         if 20000 <= self.devtype <= 29999:
             packet = struct.pack("<HI", len(data) + 4, command) + data
         else:
             packet = struct.pack("<I", command) + data
         resp = self.send_packet(0x6A, packet)
         e.check_error(resp[0x22:0x24])
         payload = self.decrypt(resp[0x38:])
-        p_len = struct.unpack("<H", payload[:0x2])[0]
-        return payload[0x6 : p_len + 2]
+        if 20000 <= self.devtype <= 29999:
+            p_len = struct.unpack("<H", payload[:0x2])[0]
+            return payload[0x6 : p_len + 2]
+        return payload[0x4:]
     
     def _sendV2(self, command: int, data: bytes = b"") -> bytes:
         """Send a packet to the device."""
         cmdstu = self.build_cmdstuV2(command, data)
         resp = self.send_packet(0x6A, cmdstu)
         e.check_error(resp[0x22:0x24])
         payload = self.decrypt(resp[0x38:])
```

### Comparing `linknlink-0.2.3/linknlink/sensor.py` & `linknlink-0.2.4/linknlink/sensor.py`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.3/setup.py` & `linknlink-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 
 from setuptools import setup, find_packages
 
 
-version = '0.2.3'
+version = '0.2.4'
 
 setup(
     name="linknlink",
     version=version,
     author="Zhao Zehua",
     author_email="huahua.zzh@gmail.com",
     url="https://github.com/xuanxuan000/python-linknlink",
```

