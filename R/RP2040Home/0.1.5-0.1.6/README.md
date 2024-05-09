# Comparing `tmp/rp2040home-0.1.5.tar.gz` & `tmp/rp2040home-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rp2040home-0.1.5.tar", last modified: Thu May  9 12:22:17 2024, max compression
+gzip compressed data, was "rp2040home-0.1.6.tar", last modified: Thu May  9 13:01:16 2024, max compression
```

## Comparing `rp2040home-0.1.5.tar` & `rp2040home-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:22:17.419026 rp2040home-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-09 12:21:58.000000 rp2040home-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-09 12:22:17.419026 rp2040home-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-09 12:21:58.000000 rp2040home-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:22:17.419026 rp2040home-0.1.5/RP2040Home/
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/RP2040Home.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:22:17.419026 rp2040home-0.1.5/RP2040Home/configparsing/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/configparsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/configparsing/configparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/configparsing/homeassistantdiscoveryconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/configparsing/mqttconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/configparsing/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/configparsing/wificonfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:22:17.419026 rp2040home-0.1.5/RP2040Home/homeassistant/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/homeassistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/homeassistant/discoveryPayload.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/homeassistant/disoveryDevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/homeassistant/mqttClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-09 12:21:58.000000 rp2040home-0.1.5/RP2040Home/homeassistant/payloadGenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:22:17.419026 rp2040home-0.1.5/RP2040Home.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-09 12:22:17.000000 rp2040home-0.1.5/RP2040Home.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-09 12:22:17.000000 rp2040home-0.1.5/RP2040Home.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:22:17.000000 rp2040home-0.1.5/RP2040Home.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 12:22:17.000000 rp2040home-0.1.5/RP2040Home.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:22:17.419026 rp2040home-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-09 12:21:58.000000 rp2040home-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:22:17.419026 rp2040home-0.1.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:21:58.000000 rp2040home-0.1.5/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:22:17.419026 rp2040home-0.1.5/test/config_parsing/
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-09 12:21:58.000000 rp2040home-0.1.5/test/config_parsing/ConfigParserTest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:21:58.000000 rp2040home-0.1.5/test/config_parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:01:16.829179 rp2040home-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-09 13:00:57.000000 rp2040home-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-09 13:01:16.829179 rp2040home-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-09 13:00:57.000000 rp2040home-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:01:16.825179 rp2040home-0.1.6/RP2040Home/
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/RP2040Home.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:01:16.829179 rp2040home-0.1.6/RP2040Home/configparsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/configparsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/configparsing/configparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/configparsing/homeassistantdiscoveryconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/configparsing/mqttconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/configparsing/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/configparsing/wificonfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:01:16.829179 rp2040home-0.1.6/RP2040Home/homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/homeassistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/homeassistant/discoveryPayload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/homeassistant/disoveryDevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/homeassistant/mqttClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-09 13:00:57.000000 rp2040home-0.1.6/RP2040Home/homeassistant/payloadGenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:01:16.829179 rp2040home-0.1.6/RP2040Home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-09 13:01:16.000000 rp2040home-0.1.6/RP2040Home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-09 13:01:16.000000 rp2040home-0.1.6/RP2040Home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:01:16.000000 rp2040home-0.1.6/RP2040Home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 13:01:16.000000 rp2040home-0.1.6/RP2040Home.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:01:16.829179 rp2040home-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-09 13:00:57.000000 rp2040home-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:01:16.829179 rp2040home-0.1.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:00:57.000000 rp2040home-0.1.6/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:01:16.829179 rp2040home-0.1.6/test/config_parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-09 13:00:57.000000 rp2040home-0.1.6/test/config_parsing/ConfigParserTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:00:57.000000 rp2040home-0.1.6/test/config_parsing/__init__.py
```

### Comparing `rp2040home-0.1.5/LICENSE` & `rp2040home-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rp2040home-0.1.5/PKG-INFO` & `rp2040home-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RP2040Home
-Version: 0.1.5
+Version: 0.1.6
 Summary: MQTT Client for RP2040 based boards which integrates into Home Assistant
 Author: Ellington S
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `rp2040home-0.1.5/README.md` & `rp2040home-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `rp2040home-0.1.5/RP2040Home/RP2040Home.py` & `rp2040home-0.1.6/RP2040Home/RP2040Home.py`

 * *Files identical despite different names*

### Comparing `rp2040home-0.1.5/RP2040Home/configparsing/configparser.py` & `rp2040home-0.1.6/RP2040Home/configparsing/configparser.py`

 * *Files identical despite different names*

### Comparing `rp2040home-0.1.5/RP2040Home/configparsing/mqttconfig.py` & `rp2040home-0.1.6/RP2040Home/configparsing/mqttconfig.py`

 * *Files identical despite different names*

### Comparing `rp2040home-0.1.5/RP2040Home/homeassistant/discoveryPayload.py` & `rp2040home-0.1.6/RP2040Home/homeassistant/discoveryPayload.py`

 * *Files identical despite different names*

### Comparing `rp2040home-0.1.5/RP2040Home/homeassistant/disoveryDevice.py` & `rp2040home-0.1.6/RP2040Home/homeassistant/disoveryDevice.py`

 * *Files identical despite different names*

### Comparing `rp2040home-0.1.5/RP2040Home/homeassistant/mqttClient.py` & `rp2040home-0.1.6/RP2040Home/homeassistant/mqttClient.py`

 * *Files identical despite different names*

### Comparing `rp2040home-0.1.5/RP2040Home/homeassistant/payloadGenerator.py` & `rp2040home-0.1.6/RP2040Home/homeassistant/payloadGenerator.py`

 * *Files identical despite different names*

### Comparing `rp2040home-0.1.5/RP2040Home.egg-info/PKG-INFO` & `rp2040home-0.1.6/RP2040Home.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RP2040Home
-Version: 0.1.5
+Version: 0.1.6
 Summary: MQTT Client for RP2040 based boards which integrates into Home Assistant
 Author: Ellington S
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `rp2040home-0.1.5/RP2040Home.egg-info/SOURCES.txt` & `rp2040home-0.1.6/RP2040Home.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rp2040home-0.1.5/setup.py` & `rp2040home-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `rp2040home-0.1.5/test/config_parsing/ConfigParserTest.py` & `rp2040home-0.1.6/test/config_parsing/ConfigParserTest.py`

 * *Files identical despite different names*

