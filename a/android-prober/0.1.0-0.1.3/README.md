# Comparing `tmp/android_prober-0.1.0.tar.gz` & `tmp/android_prober-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android_prober-0.1.0.tar", last modified: Fri May  3 11:37:40 2024, max compression
+gzip compressed data, was "android_prober-0.1.3.tar", last modified: Thu May  9 13:58:20 2024, max compression
```

## Comparing `android_prober-0.1.0.tar` & `android_prober-0.1.3.tar`

### file list

```diff
@@ -1,49 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:37:40.722380 android_prober-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-03 11:37:35.000000 android_prober-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-03 11:37:40.722380 android_prober-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-03 11:37:35.000000 android_prober-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:37:40.714380 android_prober-0.1.0/android_prober/
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:37:40.714380 android_prober-0.1.0/android_prober/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/agents/Android_Agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/agents/Bluetooth_Agent.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:37:40.718381 android_prober-0.1.0/android_prober/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/AndroidServiceInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/AudioRecorderInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/BatteryInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/BluetoothInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/BrightnessInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/CallInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/CameraInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/EmailInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/FileChooserInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/FlashInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/GpsInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/NotificationInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/RuntimePermissionInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/SensorInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/TextToSpeechInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/VibratorInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:37:40.718381 android_prober-0.1.0/android_prober/services/
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/services/android_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:37:40.718381 android_prober-0.1.0/android_prober/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/utils/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:37:40.718381 android_prober-0.1.0/android_prober/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-03 11:37:35.000000 android_prober-0.1.0/android_prober/wrappers/register_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:37:40.722380 android_prober-0.1.0/android_prober.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-03 11:37:40.000000 android_prober-0.1.0/android_prober.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-03 11:37:40.000000 android_prober-0.1.0/android_prober.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:37:40.000000 android_prober-0.1.0/android_prober.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-03 11:37:40.000000 android_prober-0.1.0/android_prober.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 11:37:40.000000 android_prober-0.1.0/android_prober.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:37:40.722380 android_prober-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-03 11:37:35.000000 android_prober-0.1.0/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-03 11:37:35.000000 android_prober-0.1.0/examples/start_and_stop_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-03 11:37:35.000000 android_prober-0.1.0/examples/with_rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:37:40.722380 android_prober-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-03 11:37:35.000000 android_prober-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.599536 android_prober-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-09 13:58:11.000000 android_prober-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-09 13:58:20.599536 android_prober-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-09 13:58:11.000000 android_prober-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.587536 android_prober-0.1.3/android_prober/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.591536 android_prober-0.1.3/android_prober/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/filechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/runtime_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/apis/vibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.595536 android_prober-0.1.3/android_prober/facades/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/filechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/runtime_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/facades/vibrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.587536 android_prober-0.1.3/android_prober/platforms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.595536 android_prober-0.1.3/android_prober/platforms/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/android/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/android/realtime_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/android/runtime_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/android/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.599536 android_prober-0.1.3/android_prober/platforms/generics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/filechooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/platforms/generics/vibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/proxy_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.599536 android_prober-0.1.3/android_prober/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.599536 android_prober-0.1.3/android_prober/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-09 13:58:11.000000 android_prober-0.1.3/android_prober/wrappers/register_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.599536 android_prober-0.1.3/android_prober.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-09 13:58:20.000000 android_prober-0.1.3/android_prober.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-09 13:58:20.000000 android_prober-0.1.3/android_prober.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:58:20.000000 android_prober-0.1.3/android_prober.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 13:58:20.000000 android_prober-0.1.3/android_prober.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 13:58:20.000000 android_prober-0.1.3/android_prober.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.587536 android_prober-0.1.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:20.599536 android_prober-0.1.3/examples/webview-app/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-09 13:58:11.000000 android_prober-0.1.3/examples/webview-app/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:58:20.599536 android_prober-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 13:58:11.000000 android_prober-0.1.3/setup.py
```

### Comparing `android_prober-0.1.0/LICENSE` & `android_prober-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.0/PKG-INFO` & `android_prober-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: android-prober
-Version: 0.1.0
+Version: 0.1.3
 Summary: Library for test android api's via service
 Home-page: https://github.com/gunaNeelamegam
 Author: GunaNeelamegam
 Author-email: gunag77730@gmail.com
 License: Apacher License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask
 Requires-Dist: kivy
 Requires-Dist: oscpy
 Requires-Dist: plyer
 Requires-Dist: swagger-gen
+Requires-Dist: pyjnius==1.6.1
 
-# Library mainly Concentrated on Android and iOS Hardware Testing Library
+# Android API Testing 
+[![Upload Python Package](https://github.com/gunaNeelamegam/android-prober/actions/workflows/python-publish.yml/badge.svg)](https://github.com/gunaNeelamegam/android-prober/actions/workflows/python-publish.yml)
+[![build](https://github.com/gunaNeelamegam/android-prober/actions/workflows/build_apk.yml/badge.svg)](https://github.com/gunaNeelamegam/android-prober/actions/workflows/build_apk.yml)
 
-# Supported platform's android, linux, iOS, windows, mac
+## Library to test the AOSP Hardware APIs
 
-
-## Trying to achive
-
-* `Library to test the android internal Hardware Service's`
-
-> Developed and Tested
+> **Currently Available APIs**
 
 * [X]  Bluetooth   ᛒ
     > ABLE TO DO
     * Connect , Disconnect
     * Pair , UnPair
     * Enable, Disable Service Provider
     * look for more..
@@ -55,50 +53,29 @@
 > NOTE  💡
 * Using the Android Background Service API you can able to receive the Android Internal Event Message's
     * Aeroplane mode change's 🛩️
     * Headset adaptor state change's 🎧
     * Incoming Phone Call 📲
     * more...
 
-> NOTE 💡 
-> 
-> `Python Module's`
-  * pyjnius
-  * plyer
-  * flask
-  * kivy
-  * oscpy
-
-##  Build and Run Example's
-
-**Requirements Installation**
+## Installation
 
 ```sh
-pip3 install -r requirements.txt
+pip install android-prober
 ```
 
-**Build Debug APK**
-```sh
-    buildozer android debug
-```
+## Usage
 
-**Build And Run into Target Machine**
-```sh
-    buildozer android debug deploy run
-```
-
-> NOTE Example main file💡  
-## Example `main.py`
+* Create `main.py` like the contents below.
 
 ```python
 from kivy.app import App
 from kivy.lang import Builder
-from hardware_agent.utils.permissions import RuntimePermission
-from hardware_agent import App as TesterApp
-
+from android_prober import AndroidProber
+from requests import get
 
 KV = '''
 BoxLayout:
     orientation: 'vertical'
     BoxLayout:
         size_hint_y: None
         height: '30sp'
@@ -116,59 +93,123 @@
         Label:
             id: label
             size_hint_y: None
             height: self.texture_size[1]
             text_size: self.size[0], None
 '''
 
-class Tester(App):
+class BluetoothTestViaWebService(App):
+    
+    BASE_URL = "http://localhost:5000"
 
     def init(self):
-        self.permission = RuntimePermission()
+        """ while using webservice to invoke the API's """
         TesterApp.use_flaskapp()
 
     def on_pause(self):
         return True
 
     def telephony_permission(self):
-        self.permission.telephony_permission()
+        response = get(f"{BASE_URL}/telephony_permission")
+        print(response.json)
 
     def location_permission(self):
-        self.permission.location_permission()
+        response = get(f"{BASE_URL}/location_permission")
+        print(response.json)
 
     def bluetooth_permission(self):
-        self.permission.blutooth_permission()
+        response = get(f"{BASE_URL}/bluetooth_permission")
+        print(response.json)
 
     def build(self):
         self.init()
         self.root = Builder.load_string(KV)
         return self.root
 
 if __name__ == '__main__':
-    Tester().run()
+    BluetoothTestViaWebService().run()
+
 ```
 
-> `Way to Use Doc's`
 
-* If you are enabled developer mode. adb daemon will start's or started automatically.
+* Create `main.py` without webservice.
 
-* Run the following command.
+```python
+from kivy.app import App
+from kivy.lang import Builder
+from android_prober import AndroidProber
+from android_prober import bluetooth
 
-```bash
-adb forward tcp:5000 tcp:5000
+KV = '''
+BoxLayout:
+    orientation: 'vertical'
+    BoxLayout:
+        size_hint_y: None
+        height: '30sp'
+        Button:
+            text: 'telephony_permission'
+            on_press: app.telephony_permission()
+        Button:
+            text: 'bluetoothPermission'
+            on_press: app.bluetooth_permission()
+        Button:
+            text: 'locationPermission'
+            on_press: app.location_permission()
+
+    ScrollView:
+        Label:
+            id: label
+            size_hint_y: None
+            height: self.texture_size[1]
+            text_size: self.size[0], None
+'''
+
+class BluetoothTest(App):
+
+    def on_pause(self):
+        return True
+
+    def bluetooth_permission(self):
+       response = bluetooth.bluetooth_permission()
+        print(response)
+
+    def build(self):
+        self.root = Builder.load_string(KV)
+        return self.root
+
+if __name__ == '__main__':
+    BluetoothTest().run()
+
+```
+
+##  Build & Run
+
+```sh
+pip install -r requirements.txt
+
+buildozer android debug
 ```
-* `why tcp:5000` ?
-  
-  * Inside the Flask Application service will run on tcp:5000 port. So, we trying to expose the port inside the phone 📱 to desktop or development enviroment.
-
-* Open the any web browser 🌐
-* [API Documentation](http://localhost:5000/docs) 
-* If the previous Link not works try below.
+Install the generated apk into the target device.
+
+
+## Documentation
+
+* python for android webview recipe internally start and serve's web service running on port 5000. 
+
+* You can also test api on Single Click.
+
+![image](./android_prober/docs/images/swagger_ui.png)
+
+* Connect the device using ADB.
+
+* If your using adb via cable, Run this to expose the port `tcp/5000`
 ```bash
-    http://ipaddress:5000/docs (please replace the ip-address with the mobile connected network ip)
+adb forward tcp:5000 tcp:5000
 ```
 
-### `Looking for` 🚀
+## Upcomming updates
+
+-> https://github.com/gunaNeelamegam/android-prober/issues
 
 * Stablity
 * API for All Other Interface's
 * FastAPI Intergration
```

### Comparing `android_prober-0.1.0/README.md` & `android_prober-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-# Library mainly Concentrated on Android and iOS Hardware Testing Library
+# Android API Testing 
+[![Upload Python Package](https://github.com/gunaNeelamegam/android-prober/actions/workflows/python-publish.yml/badge.svg)](https://github.com/gunaNeelamegam/android-prober/actions/workflows/python-publish.yml)
+[![build](https://github.com/gunaNeelamegam/android-prober/actions/workflows/build_apk.yml/badge.svg)](https://github.com/gunaNeelamegam/android-prober/actions/workflows/build_apk.yml)
 
-# Supported platform's android, linux, iOS, windows, mac
+## Library to test the AOSP Hardware APIs
 
-
-## Trying to achive
-
-* `Library to test the android internal Hardware Service's`
-
-> Developed and Tested
+> **Currently Available APIs**
 
 * [X]  Bluetooth   ᛒ
     > ABLE TO DO
     * Connect , Disconnect
     * Pair , UnPair
     * Enable, Disable Service Provider
     * look for more..
@@ -39,50 +36,29 @@
 > NOTE  💡
 * Using the Android Background Service API you can able to receive the Android Internal Event Message's
     * Aeroplane mode change's 🛩️
     * Headset adaptor state change's 🎧
     * Incoming Phone Call 📲
     * more...
 
-> NOTE 💡 
-> 
-> `Python Module's`
-  * pyjnius
-  * plyer
-  * flask
-  * kivy
-  * oscpy
-
-##  Build and Run Example's
-
-**Requirements Installation**
+## Installation
 
 ```sh
-pip3 install -r requirements.txt
+pip install android-prober
 ```
 
-**Build Debug APK**
-```sh
-    buildozer android debug
-```
+## Usage
 
-**Build And Run into Target Machine**
-```sh
-    buildozer android debug deploy run
-```
-
-> NOTE Example main file💡  
-## Example `main.py`
+* Create `main.py` like the contents below.
 
 ```python
 from kivy.app import App
 from kivy.lang import Builder
-from hardware_agent.utils.permissions import RuntimePermission
-from hardware_agent import App as TesterApp
-
+from android_prober import AndroidProber
+from requests import get
 
 KV = '''
 BoxLayout:
     orientation: 'vertical'
     BoxLayout:
         size_hint_y: None
         height: '30sp'
@@ -100,59 +76,123 @@
         Label:
             id: label
             size_hint_y: None
             height: self.texture_size[1]
             text_size: self.size[0], None
 '''
 
-class Tester(App):
+class BluetoothTestViaWebService(App):
+    
+    BASE_URL = "http://localhost:5000"
 
     def init(self):
-        self.permission = RuntimePermission()
+        """ while using webservice to invoke the API's """
         TesterApp.use_flaskapp()
 
     def on_pause(self):
         return True
 
     def telephony_permission(self):
-        self.permission.telephony_permission()
+        response = get(f"{BASE_URL}/telephony_permission")
+        print(response.json)
 
     def location_permission(self):
-        self.permission.location_permission()
+        response = get(f"{BASE_URL}/location_permission")
+        print(response.json)
 
     def bluetooth_permission(self):
-        self.permission.blutooth_permission()
+        response = get(f"{BASE_URL}/bluetooth_permission")
+        print(response.json)
 
     def build(self):
         self.init()
         self.root = Builder.load_string(KV)
         return self.root
 
 if __name__ == '__main__':
-    Tester().run()
+    BluetoothTestViaWebService().run()
+
 ```
 
-> `Way to Use Doc's`
 
-* If you are enabled developer mode. adb daemon will start's or started automatically.
+* Create `main.py` without webservice.
 
-* Run the following command.
+```python
+from kivy.app import App
+from kivy.lang import Builder
+from android_prober import AndroidProber
+from android_prober import bluetooth
 
-```bash
-adb forward tcp:5000 tcp:5000
+KV = '''
+BoxLayout:
+    orientation: 'vertical'
+    BoxLayout:
+        size_hint_y: None
+        height: '30sp'
+        Button:
+            text: 'telephony_permission'
+            on_press: app.telephony_permission()
+        Button:
+            text: 'bluetoothPermission'
+            on_press: app.bluetooth_permission()
+        Button:
+            text: 'locationPermission'
+            on_press: app.location_permission()
+
+    ScrollView:
+        Label:
+            id: label
+            size_hint_y: None
+            height: self.texture_size[1]
+            text_size: self.size[0], None
+'''
+
+class BluetoothTest(App):
+
+    def on_pause(self):
+        return True
+
+    def bluetooth_permission(self):
+       response = bluetooth.bluetooth_permission()
+        print(response)
+
+    def build(self):
+        self.root = Builder.load_string(KV)
+        return self.root
+
+if __name__ == '__main__':
+    BluetoothTest().run()
+
+```
+
+##  Build & Run
+
+```sh
+pip install -r requirements.txt
+
+buildozer android debug
 ```
-* `why tcp:5000` ?
-  
-  * Inside the Flask Application service will run on tcp:5000 port. So, we trying to expose the port inside the phone 📱 to desktop or development enviroment.
-
-* Open the any web browser 🌐
-* [API Documentation](http://localhost:5000/docs) 
-* If the previous Link not works try below.
+Install the generated apk into the target device.
+
+
+## Documentation
+
+* python for android webview recipe internally start and serve's web service running on port 5000. 
+
+* You can also test api on Single Click.
+
+![image](./android_prober/docs/images/swagger_ui.png)
+
+* Connect the device using ADB.
+
+* If your using adb via cable, Run this to expose the port `tcp/5000`
 ```bash
-    http://ipaddress:5000/docs (please replace the ip-address with the mobile connected network ip)
+adb forward tcp:5000 tcp:5000
 ```
 
-### `Looking for` 🚀
+## Upcomming updates
+
+-> https://github.com/gunaNeelamegam/android-prober/issues
 
 * Stablity
 * API for All Other Interface's
 * FastAPI Intergration
```

### Comparing `android_prober-0.1.0/android_prober/__init__.py` & `android_prober-0.1.3/android_prober/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 from flask import Flask as _Flask
-from _datetime import datetime as _datetime
+from datetime import datetime as _datetime
 from swagger_gen.swagger import Swagger as _Swagger
 from threading import Thread as _Thread
 from os import path as _path, curdir as _curdir
 
-#FIMXE: Use to create with proxy design pattern
-# reference https://github.com/kivy/plyer/blob/master/plyer/__init__.py
-
-
 # Need's to done with better design but it required
-class App:
-
+class AndroidProber:
     app : _Flask = None
     swagger: _Swagger = None
     flask_thread = None
-    APPNAME = "GUNA_TESTER"
+    APPNAME = "Prober"
     DOC_ENDPOINT: str = "/docs"
-    DOC_TITLE: str = "TESTER"
+    DOC_TITLE: str = "Android-Prober"
 
     @classmethod
     def use_flaskapp(cls, app_name: str = APPNAME , host = "0.0.0.0", port = 5000):
         cls.app = _Flask(app_name,
                         static_folder = cls.get_ui_path("static"),
                         template_folder = cls.get_ui_path("templates"))
         cls.swagger = _Swagger(
                 app   = cls.app,
                 title = cls.DOC_TITLE,
                 url   = cls.DOC_ENDPOINT
         )
+        # skipped auto documentation
         cls.start_flask_server(host, port)
-        register_interface(cls.app)
+        register_interface()
         cls.swagger.configure()
         return cls.app
 
     @classmethod
     def start_flask_server(cls, host, port):
         cls.flask_thread = _Thread(target = cls.start_server, kwargs= {
              "host": host,
@@ -51,53 +47,50 @@
     def start_server(cls, host, port):
         cls.app.run(host = host, port = port, threaded = False, debug = False)
 
     @staticmethod
     def home_route():
         return {
         "author": "gunaNeelamegam.N",
-        "api": 1,
+        "api": "0.1.0",
         "next_release": str(_datetime.now().date()),
         "status": False
     }
 
-def register_interface(app: _Flask):
+
+def register_interface():
     """Using this function library try's to use the previously implemented functionality
 
     Args:
         app (_Flask): _Flask app instance
     """
-    if App.app is None:
-        App.app  = app
     # ALL THE INTERFACE WILL RETURN THE INSTANCE OF THE CLASS
+    # AUTO MATE 
+    from android_prober.apis.bluetooth import register_bluetooth
+    from android_prober.apis.call import register_call
+    from android_prober.apis.tts import register_tts
+    from android_prober.apis.notification import register_notify
+    from android_prober.apis.audio import register_audio
+    from android_prober.apis.gps import register_gps
+    from android_prober.apis.battery import register_battery
+    from android_prober.apis.email import register_email
+    from android_prober.apis.brightness import register_brightness
+    from android_prober.apis.camera import register_camera
+    from android_prober.apis.service import register_service
+    from android_prober.apis.flash import register_flash
+
 
-    from .interfaces.BluetoothInterface import register_bluetooth
-    from .interfaces.CallInterface import register_call
-    from .interfaces.TextToSpeechInterface import register_tts
-    from .interfaces.NotificationInterface import register_notify
-    from .interfaces.AudioRecorderInterface import register_audio
-    from .interfaces.GpsInterface import register_gps
-    from .interfaces.BatteryInterface import register_battery
-    from .interfaces.EmailInterface import register_email
-    from .interfaces.BrightnessInterface import register_brightness
-    from .interfaces.CameraInterface import register_camera
-
-    # ANDROID BACKGROUND SERVICE
-    from .interfaces.AndroidServiceInterface import register_android_service
-    register_android_service()
-
-    # ANDROID RUNTIME PERMISSION INTERFACE
-    from .interfaces.RuntimePermissionInterface import register_runpermission
-    register_runpermission()
 
     # REGISTERING THE SERVICE's
 
     register_camera()
     register_audio()
     register_bluetooth()
     register_tts()
     register_notify()
     register_call()
     register_brightness()
     register_gps()
     register_battery()
     register_email()
+    register_flash()
+    register_service()
```

### Comparing `android_prober-0.1.0/android_prober/agents/Android_Agent.py` & `android_prober-0.1.3/android_prober/platforms/android/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from android_prober.utils import Platform # Need's to check after decorator not working
-
 from jnius import autoclass
 from android import mActivity
 
-class AndroidServiceAgent:
+class AndroidService:
     """Using this class we can able to start and stop the service programmtically
     """
 
     def __init__(self) -> None:
         self.service = None
         self.setup_service()
 
@@ -43,8 +41,8 @@
         status = False
         try:
             self.service.start(mActivity,'')
             status = True
         except Exception as e:
             print("EXECPTION:", e.args)
         finally :
-            return status
+            return status
```

### Comparing `android_prober-0.1.0/android_prober/agents/Bluetooth_Agent.py` & `android_prober-0.1.3/android_prober/platforms/android/bluetooth.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 from jnius import autoclass
-from platform import platform
 from typing import Union, Any
 from android_prober.utils.common import Platform
-
-if Platform.is_android():
-    from android.broadcast import BroadcastReceiver
+from android.broadcast import BroadcastReceiver
 
 class BluetoothAgent:
-    if Platform.is_android():
-        BluetoothAdapter = autoclass("android.bluetooth.BluetoothAdapter")
-        BluetoothDevice  = autoclass("android.bluetooth.BluetoothDevice")
-        SERIAL_PORT_PROFILE_UUID = "00001101-0000-1000-8000-00805F9B34FB"
+    BluetoothAdapter = autoclass("android.bluetooth.BluetoothAdapter")
+    BluetoothDevice  = autoclass("android.bluetooth.BluetoothDevice")
+    SERIAL_PORT_PROFILE_UUID = "00001101-0000-1000-8000-00805F9B34FB"
 
     def __init__(self) -> None:
-        if Platform.is_android():
-            self.scanned_devices = set()
-            self.connected_device = None
-            self.is_connected = False
-            self.ble_adapter = self.BluetoothAdapter.getDefaultAdapter()
-            self.FOUND = self.BluetoothDevice.ACTION_FOUND
-            self.STARTED = self.BluetoothAdapter.ACTION_DISCOVERY_STARTED
-            self.FINISHED = self.BluetoothAdapter.ACTION_DISCOVERY_FINISHED
-            self.server_socket = None
+        self.scanned_devices = set()
+        self.connected_device = None
+        self.is_connected = False
+        self.ble_adapter = self.BluetoothAdapter.getDefaultAdapter()
+        self.FOUND = self.BluetoothDevice.ACTION_FOUND
+        self.STARTED = self.BluetoothAdapter.ACTION_DISCOVERY_STARTED
+        self.FINISHED = self.BluetoothAdapter.ACTION_DISCOVERY_FINISHED
+        self.server_socket = None
 
-    @Platform.android
     def on_scanning(self, context, intent):
         action = intent.getAction()
         if action == self.STARTED:
             self.scanned_devices = None
             self.scanned_devices = set()
             print("SCANNING STARTED ")
 
@@ -42,97 +36,86 @@
 
         elif action == self.FINISHED:
             self.ble_adapter.cancelDiscovery()
             self.boardcast_receiver.stop()
             self.boardcast_receiver = None
             print("SCANNING STOPED")
 
-    # @Platform.android
+    # 
     def enable_adapter(self) -> bool:
         status = False
         if (self.ble_adapter and not self.ble_adapter.isEnabled()):
             self.ble_adapter.enable()
             status = self.ble_adapter.isEnabled()
         return status
 
-    @Platform.android
     def disable_adapter(self)->bool:
         if (self.ble_adapter and self.ble_adapter.isEnabled()):
             self.ble_adapter.disable()
         return self.ble_adapter.isEnabled()
 
-    @Platform.android
     def paired_devices(self):
         if self.ble_adapter:
             bounded_devices = self.ble_adapter.getBondedDevices().toArray()
             response = []
             for device in bounded_devices:
                 response.append((device.getName(), device.getAddress()))
         return response
 
-    @Platform.android
     def scan(self):
         actions = [self.FOUND, self.STARTED, self.FINISHED]
         self.boardcast_receiver = BroadcastReceiver(self.on_scanning, actions=actions)
         self.boardcast_receiver.start()
         self.ble_adapter.startDiscovery()
 
-    @Platform.android
     def is_device_paired(self, remote_info: dict) -> bool:
         name = remote_info.get("name", "").lower()
         mac_address = remote_info.get("mac_address","").lower()
         bounded_devices = self.ble_adapter.getBondedDevices().toArray()
 
         def is_equal(device):
             if name == device.getName().lower() or mac_address == device.getAddress().lower():
                 return True
             return False
 
         filtered_devices = filter(is_equal, bounded_devices)
         return (True,filtered_devices[0]) if len(filtered_devices) else (False, None)
 
-    @Platform.android
     def pair(self, mac_address: str):
         if self.ble_adapter and mac_address.strip() != "":
             device = self.ble_adapter.getRemoteDevice(mac_address)
             if device and device.getBondState() != self.BluetoothDevice.BOND_BONDED:
                 device.createBond()
 
-    @Platform.android
     def connect(self, device_info: dict = {}):
         self.connected_device = None
         device = self.ble_adapter.getRemoteDevice(device_info.get("address"))
         if device and device.getBondState()  != self.BluetoothDevice.BOND_NONE:
             UUID = autoclass('java.util.UUID')
             self.connected_device = device.createRfcommSocketToServiceRecord(UUID.fromString(self.SERIAL_PORT_PROFILE_UUID))
             self.connected_device.getInputStream()
             self.connected_device.getOutputStream()
             self.connected_device.connect()
             print("CONNECTED DEVICE : ", self.connected_device.isConnected(), self.connected_device.getRemoteDevice().toString())
 
-    @Platform.android
     def disconnect(self):
         if self.connected_device:
             print("DISCONNECTED : ", self.connected_device.isConnected())
             self.connected_device.close()
             self.is_connected = False
             self.connected_device = None
 
-    @Platform.android
     def unpair(self, address: Union[str, Any]):
         if self.ble_adapter and address.strip():
             device = self.ble_adapter.getRemoteDevice(address)
             if (device.getBondState() == self.BluetoothDevice.BOND_BONDED):
                 device.removeBond();
-
-
     class BleDevice:
         def __init__(self, name ="", address= "") -> None:
             self.name = name
             self.address = address
-
-        @Platform.android
+        
         def __eq__(self, other):
             return isinstance(other, BluetoothAgent.BleDevice) and (self.name == other.name and self.address == other.address)
 
         def __hash__(self):
             return hash((self.name, self.address))
```

### Comparing `android_prober-0.1.0/android_prober/interfaces/AudioRecorderInterface.py` & `android_prober-0.1.3/android_prober/apis/audio.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,16 @@
-from plyer.facades.audio import Audio
-from plyer import audio
 from abc import ABC, abstractmethod
 from typing import Any
-from android_prober.wrappers import get
+from android_prober.wrappers import get , post
 from inspect import getmembers, ismethod
-from android_prober.wrappers import post
 from flask import request
+from android_prober.facades import Audio
+from android_prober import audio
 
-class IAudio(ABC):
-
-    @abstractmethod
-    def stop_record(self) -> dict:
-        pass
-
-    @abstractmethod
-    def start_record(self) -> dict:
-        pass
-
-    @abstractmethod
-    def play_audio(self) -> dict:
-        pass
-
-    @abstractmethod
-    def record_state(self):
-        pass
-
-class AudioRecorderInterface(IAudio):
+class Audio:
 
     def __init__(self) -> None:
         self.audio: Audio = audio
         self.filepath:str = "/sdcard/test_recorder.3gp"
         self.audio.filepath = self.filepath
 
     @get(
@@ -100,10 +81,10 @@
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         for key,value in getmembers(self, predicate= ismethod):
             if not key.startswith('__') and not key.endswith("__"):
                 value()
 
 def register_audio():
-    audioRecorderInterface = AudioRecorderInterface()
+    audioRecorderInterface = Audio()
     audioRecorderInterface()
     return audioRecorderInterface
```

### Comparing `android_prober-0.1.0/android_prober/interfaces/BatteryInterface.py` & `android_prober-0.1.3/android_prober/apis/battery.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,29 @@
 from typing import Any
 from inspect import getmembers, ismethod
-from plyer.facades.battery import Battery
-from plyer import battery
+from android_prober.facades import Battery
+from android_prober import battery
 
-# custom module
 from android_prober.wrappers import get
-from abc import ABC,abstractmethod
 
-class IBattery(ABC):
-
-    @abstractmethod
-    def battery_status(self)->dict:
-        pass
-
-class BatteryInterface(IBattery):
+class Battery:
 
     def __init__(self) -> None:
         self.battery: Battery = battery
 
     @get(
     summary= "Battery Status",
     description= "Using this Api We can able to retrive the battery status in android system",
     response_model=[(200, 'Success'), (500, 'Error')]
     )
-    def battery_status(self) -> dict:
-        status = self.battery.status
-        return {
-            "status": True,
-             **status
-        }
+    def status(self) -> dict:
+        return self.battery.status()
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         for key,value in getmembers(self, predicate= ismethod):
             if not key.startswith('__') and not key.endswith("__"):
                 value()
 
 def register_battery():
-    battery_interface =  BatteryInterface()
+    battery_interface =  Battery()
     battery_interface()
     return battery_interface
```

### Comparing `android_prober-0.1.0/android_prober/interfaces/BrightnessInterface.py` & `android_prober-0.1.3/android_prober/apis/brightness.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,41 @@
 from typing import Any
 from inspect import getmembers, ismethod
 from flask import request
-from plyer.facades.brightness import Brightness
-from plyer import brightness
-
-# custom module
+from android_prober.facades.brightness import Brightness
+from android_prober import brightness
 from android_prober.wrappers import get, post
-from abc import ABC,abstractmethod
-
-class IBrightness(ABC):
-
-    @abstractmethod
-    def brightness(self)->dict:
-        pass
-
-    @abstractmethod
-    def set_brightness(self)->dict:
-        pass
-
-class BrightnessInterface(IBrightness):
+class Brightness:
 
     def __init__(self) -> None:
-        self.bright_ness:Brightness = brightness
+        self.bright_ness: Brightness = brightness
 
+    # FIXME: overrides the class dictionary when createing methods with same name
     @post(
         summary= "Set the Device Brightness",
         description= "Using this Api we can able mutate the device brightness",
         response_model=[(200, 'Success'), (500, 'Error')],
         request_model = {
             "level" : "number"
         }
     )
     def set_brightness(self) -> dict:
-        requested_level:int = request.json.get("level")
-        if requested_level:
-            self.bright_ness.set_level(requested_level)
-        return {
-            "status": True,
-            "level": self.bright_ness.current_level,
-        }
+        requested_level:int = request.json.get("level", 10)
+        return self.bright_ness.set_brightness(requested_level)
 
     @get(
         summary= "Get the Device Brightness",
         description= "Using this Api we can able retrive the device brightness",
         response_model=[(200, 'Success'), (500, 'Error')]
     )
     def brightness(self)->dict:
-        return {
-            "status": True,
-            "level": str(self.bright_ness.current_level),
-        }
+        return self.bright_ness.brightness()
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         for key,value in getmembers(self, predicate= ismethod):
             if not key.startswith('__') and not key.endswith("__"):
                 value()
 
 def register_brightness():
-    brightness_interface =  BrightnessInterface()
+    brightness_interface =  Brightness()
     brightness_interface()
     return brightness_interface
```

### Comparing `android_prober-0.1.0/android_prober/interfaces/CallInterface.py` & `android_prober-0.1.3/android_prober/apis/call.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,31 @@
-from plyer import call
-from plyer.facades.call import Call
 from abc import ABC, abstractmethod
-from typing import Union,Any
+from typing import Any
 from inspect import getmembers, ismethod
 from android_prober.wrappers import get, post
 from flask import request
+from android_prober.facades import Call
+from android_prober import call
 
-class ICall(ABC):
-
-    @abstractmethod
-    def make_call(self, phone_number: int):
-        pass
-
-    @abstractmethod
-    def dial_call(self)-> bool:
-        pass
-
-class CallInterface(ICall):
+class Call:
 
     def __init__(self) -> None:
         self.call: Call = call
 
     @post(
         summary= "Make the Phone Call",
         description= "Using this Api we can able to make call",
         response_model=[(200, 'Success'), (500, 'Error')],
         request_model = {
             "phone_number": "number"
         }
     )
     def make_call(self):
         phone_number = request.json.get("phone_number" , "83973973793")
-        return self.call.makecall(tel = phone_number)
+        return self.call.make_call(tel = phone_number)
 
     @get(
         summary= "Open the Dial Action",
         description= "Using this Api we can able Open the dialer Activity",
         response_model=[(200, 'Success'), (500, 'Error')],
     )
     def dial_call(self) -> bool:
@@ -47,10 +37,10 @@
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         for key,value in getmembers(self, predicate= ismethod):
             if not key.startswith('__') and not key.endswith("__"):
                 value()
 
 def register_call():
-    callInterface = CallInterface()
+    callInterface = Call()
     callInterface()
     return callInterface
```

### Comparing `android_prober-0.1.0/android_prober/interfaces/CameraInterface.py` & `android_prober-0.1.3/android_prober/apis/camera.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,16 @@
 from typing import Any
 from inspect import getmembers, ismethod
 from flask import request
-from plyer.facades.camera import Camera
-from plyer import camera
+from android_prober.facades.camera import Camera
+from android_prober import camera
 from  os.path import exists,join
-# custom module
-from android_prober.wrappers import get,post
-from abc import ABC,abstractmethod
+from android_prober.wrappers import post
 
-class ICamera(ABC):
-
-    @abstractmethod
-    def take_picture(self, filepath:str)-> dict:
-        pass
-
-    @abstractmethod
-    def take_video(self, filepath:str)->dict:
-        pass
-
-class CameraInterface(ICamera):
+class Camera:
 
     def __init__(self) -> None:
         self.camera: Camera = camera
         self.DEFAULT_PATH = ""
         self.DEFAULT_FILENAME = "test_camera.png"
 
     @post(
@@ -89,10 +77,10 @@
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         for key,value in getmembers(self, predicate= ismethod):
             if not key.startswith('__') and not key.endswith("__"):
                 if "callback" not in key:
                     value()
 
 def register_camera():
-    camera_interface =  CameraInterface()
+    camera_interface =  Camera()
     camera_interface()
     return camera_interface
```

### Comparing `android_prober-0.1.0/android_prober/interfaces/EmailInterface.py` & `android_prober-0.1.3/android_prober/apis/email.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from typing import Any
 from inspect import getmembers, ismethod
-from flask import Flask, request
-from plyer.facades.email import Email
-from plyer import email
+from flask import request
+from android_prober.facades.email import Email
+from android_prober import email
 from android_prober.utils.common import Platform
-# custom module
 from android_prober.wrappers import get,post
 from typing import NamedTuple
 
 class EmailMessage(NamedTuple):
     subject: str
     text: str
     recipient : str
     create_chooser: str
 
 
-class EmailInterface:
+class Email:
 
     def __init__(self) -> None:
         self.email: Email = email
 
     @post(
         summary = "Send Email",
         description= "Using this Api Can able to Send Email \n Supported Platform's Android, Linux, Windows, iOS",
@@ -61,10 +60,10 @@
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         for key,value in getmembers(self, predicate= ismethod):
             if not key.startswith('__') and not key.endswith("__"):
                 value()
 
 def register_email():
-    email_interface =  EmailInterface()
+    email_interface =  Email()
     email_interface()
     return email_interface
```

### Comparing `android_prober-0.1.0/android_prober/interfaces/FileChooserInterface.py` & `android_prober-0.1.3/android_prober/apis/filechooser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Any
 from inspect import getmembers, ismethod
 from flask import request
-from plyer import filechooser
-from plyer.facades import FileChooser
+from android_prober import filechooser
+from android_prober.facades import FileChooser
 
 # custom module
-from android_prober.wrappers import get, post
-from abc import ABC,abstractmethod
+from android_prober.wrappers import post
 
 mime_type = {
         "doc": "application/msword",
         "docx": "application/vnd.openxmlformats-officedocument." +
                 "wordprocessingml.document",
         "ppt": "application/vnd.ms-powerpoint",
         "pptx": "application/vnd.openxmlformats-officedocument." +
@@ -22,43 +21,29 @@
         "pdf": "application/pdf",
         "zip": "application/zip",
         "image": "image/*",
         "video": "video/*",
         "audio": "audio/*",
         "application": "application/*"}
 
-class IFileChooser(ABC):
-
-    @abstractmethod
-    def open_file(self):
-        pass
-
-    @abstractmethod
-    def save_file(self):
-        pass
-
-    @abstractmethod
-    def choose_dir(self):
-        pass
-
 from typing import NamedTuple
 
 class FileChooseRequest(NamedTuple):
     path: str = ""
     multiple : bool = False
     filters: list = []
     preview : bool = False
     title: str = "Tester app"
     show_hidden: bool = False
     icon: str = ""
 
-class FileChooserInterface(IFileChooser):
+class FileChooser:
 
     def __init__(self) -> None:
-        self.filechooser = filechooser
+        self.filechooser:FileChooser = filechooser
 
     @post(
         summary= "Open the file chooser window",
         description= "Using this Api we can able open and select the files",
         response_model=[(200, 'Success'), (500, 'Error')],
         request_model = {
             "path": "string",
@@ -145,10 +130,10 @@
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         for key,value in getmembers(self, predicate= ismethod):
             if not key.startswith('__') and not key.endswith("__"):
                 value()
 
 def register_filechooser():
-    filechooser_interface  =  FileChooserInterface()
+    filechooser_interface  =  FileChooser()
     filechooser_interface()
     return filechooser_interface
```

### Comparing `android_prober-0.1.0/android_prober/interfaces/FlashInterface.py` & `android_prober-0.1.3/android_prober/apis/flash.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,13 @@
-from plyer.facades.flash import Flash
-from plyer import flash
-from abc import abstractmethod, ABC
+from android_prober.facades import Flash
+from android_prober import flash
 from android_prober.wrappers import get
 from typing import Any
 from inspect import getmembers, ismethod
-
-class IFlash(ABC):
-
-    @abstractmethod
-    def flash_on(self)->dict:
-        pass
-
-    @abstractmethod
-    def flash_off(self) -> dict:
-        pass
-
-class FlashInterface(IFlash):
+class Flash:
     def __init__(self) -> None:
         self.status = False
         self.flash : Flash = flash
 
     @get(
         summary = "Flash Off",
         description= "Using this Api Can able to Turn off the flash on android device",
@@ -59,10 +47,10 @@
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         for key,value in getmembers(self, predicate= ismethod):
             if not key.startswith('__') and not key.endswith("__"):
                 value()
 
 
 def register_flash():
-    flash_interface = FlashInterface()
+    flash_interface = Flash()
     flash_interface()
     return flash_interface
```

### Comparing `android_prober-0.1.0/android_prober/interfaces/GpsInterface.py` & `android_prober-0.1.3/android_prober/platforms/generics/gps.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,55 @@
-from typing import Any
-from inspect import getmembers, ismethod
-from plyer.facades.gps import GPS
 from plyer import gps
-
-# custom module
-from android_prober.wrappers import get
-from abc import ABC,abstractmethod
-
-class IBattery(ABC):
-
-    @abstractmethod
-    def location(self)->dict:
-        pass
-
-class GpsInterface(IBattery):
+from typing import Any
+from plyer.facades import GPS as PGPS
+from android_prober.facades import GPS
+from functools import lru_cache
+class GenericGps(GPS):
 
     """
     FIXME:
         on next release we need's to create the pub sub pattern for sending the message asynchrously
     """
     def __init__(self) -> None:
-        self.gps: GPS = gps
+        self.gps: PGPS = gps
         self.current_location :dict = dict()
         self.gps.configure(on_location = self.on_location_change, on_status= self.on_status_change)
-
-    @get(
-        summary = "Start the GPS Listener",
-        description= "Using this Api Can able to start the gps listener if the location change's response is given through socket's",
-        response_model =  [(201, "Success"), (500, "Failure")]
-    )
+    
     def gps_start(self):
         """
         Start the listener for location change's
         """
         self.gps.start()
         return {
             "status": True,
             "message": "Gps Listener Started Successfully"
         }
-
-    @get(
-        summary = "Stop the GPS Listener",
-        description= "Using this Api Can able to stop the gps listener if the location change's response is given through socket's",
-        response_model =  [(201, "Success"), (500, "Failure")]
-    )
+    
     def gps_stop(self):
         """
         Stop the Already started Listener which listening for location change's.
         """
         self.gps.stop()
         return {
             "status": True,
             "message": "Gps Listener Stoped Successfully"
         }
 
-    @get(
-        summary = "Get the Current GPS Location",
-        description= "Using this Api Can able to current location",
-        response_model =  [(201, "Success"), (500, "Failure")]
-    )
     def location(self) -> dict:
-        return self.current_location
+        return {
+            "status": True,
+            "message": f"Current Location {self.gps.current_location}"
+        }
+
 
     @staticmethod
     def on_status_change(status: Any):
         print("GPS STATUS CHANGES ", status)
 
     @staticmethod
     def on_location_change(location: dict):
         print("GPS LOCATION : ", location)
 
-    def __call__(self, *args: Any, **kwds: Any) -> Any:
-        for key,value in getmembers(self, predicate= ismethod):
-            if not key.startswith('__') and not key.endswith("__"):
-                if "on" not in key:
-                    value()
-
-def register_gps():
-    gps_interface =  GpsInterface()
-    gps_interface()
+@lru_cache
+def instance():
+    gps_interface =  GenericGps()
     return gps_interface
```

### Comparing `android_prober-0.1.0/android_prober/interfaces/RuntimePermissionInterface.py` & `android_prober-0.1.3/android_prober/apis/runtime_permission.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,17 @@
-from abc import ABC, abstractmethod
 from typing import Any
 from inspect import getmembers, ismethod
-from android_prober.utils import RuntimePermission
 from android_prober.wrappers import get
-from android.runnable import run_on_ui_thread
+from android_prober.facades import RuntimePermission
+from android_prober import runtime_permission
 
-class IRuntimePermission(ABC):
-
-    @abstractmethod
-    def location_permission(self):
-        pass
-
-    @abstractmethod
-    def bluetooth_permission(self):
-        pass
-
-    @abstractmethod
-    def telephony_permission(self):
-        pass
-
-class RunPermissionInterface(IRuntimePermission):
+class Runtime:
 
     def __init__(self) -> None:
-        self.runtime_perm = RuntimePermission()
+        self.runtime_perm: RuntimePermission = runtime_permission
 
     @get(
         summary = "Request Location Permission",
         description = "Using this API we can request the runtime permission for location in android",
         response_model = [(200, "Success"), (400, "Failure")]
     )
     def location_permission(self):
@@ -53,10 +38,10 @@
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         for key,value in getmembers(self, predicate= ismethod):
             if not key.startswith('__') and not key.endswith("__"):
                 value()
 
 def register_runpermission():
-    run_permission = RunPermissionInterface()
+    run_permission = Runtime()
     run_permission()
     return run_permission
```

### Comparing `android_prober-0.1.0/android_prober/services/android_service.py` & `android_prober-0.1.3/android_prober/platforms/android/realtime_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 from time import sleep
 from oscpy.server import OSCThreadServer
 from oscpy.client import OSCClient
 from android.broadcast import BroadcastReceiver
 from json import loads
+from jnius import autoclass,cast, PythonJavaClass, java_method
 
-from android_prober.utils import platform
+PythonActivity = autoclass('org.kivy.android.PythonActivity')
+PythonService = autoclass('org.kivy.android.PythonService')
 
-if platform == 'android':
-    from jnius import autoclass, cast, PythonJavaClass, java_method
-    PythonActivity = autoclass('org.kivy.android.PythonActivity')
-    PythonService = autoclass('org.kivy.android.PythonService')
-    TelephonyManager = autoclass('android.telephony.TelephonyManager')
-    System = autoclass("java.lang.System")
-    Intent = autoclass("android.content.Intent")
-    Context = autoclass("android.content.Context")
-    Executors = autoclass("java.util.concurrent.Executors")
-    PythonService.mService.setAutoRestartService(True)
+telephony_callback = None
+context = PythonService.mService.getApplication().getApplicationContext()
+TelephonyManager = autoclass('android.telephony.TelephonyManager')
+System = autoclass("java.lang.System")
+Intent = autoclass("android.content.Intent")
+Context = autoclass("android.content.Context")
+Executors = autoclass("java.util.concurrent.Executors")
+PythonService.mService.setAutoRestartService(True)
+System.out.println("APPLICATION CONTEXT : " + str(context))
 
 class MyCallStateListener(PythonJavaClass):
-    __javainterfaces__ = ['android.telephony.TelephonyCallback$CallStateListener']
+    __javainterfaces__ = ['android/telephony/TelephonyCallback$CallStateListener']
+    __javacontext__ = "app"
 
     @java_method('(I)V')
     def onCallStateChanged(self, state):
-        print("Call state changed:", state)
+        System.out.println("Call state changed:" + str(state))
         if state == TelephonyManager.CALL_STATE_IDLE:
             System.out.println("Call ended or idle")
         elif state == TelephonyManager.CALL_STATE_RINGING:
             System.out.println("Incoming call ringing from:")
         elif state == TelephonyManager.CALL_STATE_OFFHOOK:
             System.out.println("Outgoing call or call answered")
 
-def call_listener(context):
+def unsubscribe_telephonyservice():
+    if telephony_callback:
+        global telephony_callback
+        telephony_manager =  context.getSystemService(Context.TELEPHONY_SERVICE)
+        telephony_manager.unregisterTelephonyCallback(telephony_callback)
+        telephony_callback = None
+           
+def subscribe_telephony_service():
+    global telephony_callback
     try:
-        System.out.println("TELE MANAGER")
         telephony_manager =  context.getSystemService(Context.TELEPHONY_SERVICE)
-        System.out.println("STATE : " + str(telephony_manager.getCallState()))
-        # telephony_callback = MyCallStateListener()
-        # executor = Executors.newSingleThreadExecutor();
-        # telephony_manager.registerTelephonyCallback(executor , telephony_callback)
+        telephony_manager = cast(TelephonyManager, telephony_manager)
+        telephony_callback = MyCallStateListener()
+        executor = Executors.newSingleThreadExecutor();
+        telephony_manager.registerTelephonyCallback(executor , telephony_callback)
     except Exception as e:
         System.out.println("EXCEPTION IN AFTER START" + str(e.args))
 
 HOST = "0.0.0.0"
 PORT = 8250
 CLIENT_HOST = "192.168.119.122"
 CLIENT = OSCClient(CLIENT_HOST, 3002)
@@ -68,20 +77,20 @@
 
 def on_airplane_mode(extras, intent, context):
     state = extras.get("state")
     System.out.println("AIRPLANE STATE : " + str(state))
     CLIENT.send_message(b"/airplane_mode",[state])
 
 def on_battery_changed(extras, intent, context):
-        System.out.println("ON BATTERY CHANGED")
-        BatteryManager = autoclass("android.os.BatteryManager")
-        level = intent.getIntExtra(BatteryManager.EXTRA_LEVEL, -1)
-        scale = intent.getIntExtra(BatteryManager.EXTRA_SCALE, -1)
-        batteryPercentage = ((level // scale) * 100)
-        CLIENT.send_message(b"/battery_change", [level, scale, batteryPercentage])
+    System.out.println("ON BATTERY CHANGED")
+    BatteryManager = autoclass("android.os.BatteryManager")
+    level = intent.getIntExtra(BatteryManager.EXTRA_LEVEL, -1)
+    scale = intent.getIntExtra(BatteryManager.EXTRA_SCALE, -1)
+    batteryPercentage = ((level // scale) * 100)
+    CLIENT.send_message(b"/battery_change", [level, scale, batteryPercentage])
 
 def on_battery_low(extras, intent, context):
     CLIENT.send_message(b"/battery_low", ["BATTERY LOW".encode()])
 
 def on_battery_okay(extras, intent, context):
     CLIENT.send_message(b"/battey_okay", ["BATTERY OKAY".encode()])
 
@@ -157,18 +166,15 @@
     Intent.ACTION_BATTERY_LOW: on_battery_low,
     Intent.ACTION_BATTERY_OKAY: on_battery_okay,
     Intent.ACTION_MEDIA_BUTTON:on_media_btn,
     Intent.ACTION_SEARCH: on_search
 }
 
 def on_broadcast(context, intent):
-        global registered
         try:
-            System.out.println(context.toString())
-            call_listener(context)
             extras = intent.getExtras()
             action = intent.getAction()
             if action:
                 if callback := ACTIONS.get(action, None):
                     callback(extras, intent, context)
         except Exception as e:
             System.out.println("EXCEPTION :", str(e.args))
@@ -181,14 +187,15 @@
     global server
     server = OSCThreadServer()
     server.listen(address = HOST, port = PORT, default = True)
 
 def stop_service():
     global stopped
     broadcast_receiver.stop()
+    unsubscribe_telephonyservice()
     PythonService.mService.setAutoRestartService(False)
     stopped = False
 
 def change_client(address: bytes):
     System.out.println("CHANGE CLIENT : " + address.decode())
     address_info: dict = loads(address)
     host:str = address_info.get("host")
@@ -208,14 +215,15 @@
 
 def message_loop():
     broadcast_receiver.start()
     while True:
         if stopped:
             break
         sleep(1)
+    unsubscribe_telephonyservice()
     server.terminate_server()
     sleep(0.1)
     server.close()
     server = None
 
 if __name__ == '__main__':
     start_server()
```

### Comparing `android_prober-0.1.0/android_prober/utils/common.py` & `android_prober-0.1.3/android_prober/utils/common.py`

 * *Files identical despite different names*

### Comparing `android_prober-0.1.0/android_prober/wrappers/register_wrapper.py` & `android_prober-0.1.3/android_prober/wrappers/register_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,108 @@
-from android_prober import App
-
-# Need's to move into different module
 from functools import wraps, partial
 from typing import Any, Union
 from swagger_gen.lib.wrappers import swagger_metadata
-
+from android_prober.app import AndroidProber
 
 """
 These methods are using for achiving the same functionality as JSONRPC
 
 NEED's to WORK AROUND
 ====================
 * handle all the exception cases
     * reference same as expressjs
 
 """
 
+def include_apis(cls):
+    for key, value in vars(cls).items():
+        if callable(value) and not (key.startswith("__") or key.endswith("__")):
+            if not key.startswith("_") and key in dir(cls):
+                response = value()
+                setattr(cls, key, response)
+    return cls
+
 def get(func = None, handler_name: str = '', **kwgs):
 
     if func is None:
-        return partial(get,handler_name = handler_name, **kwgs)
+        return partial(get, handler_name = handler_name, **kwgs)
 
     @wraps(func)
-    def get_callback(*args,**kwargs):
+    def get_callback(*args, **kwargs):
         """
         Please pass the very first as instance of the class
         """
         nonlocal handler_name
+        class_name = func.__qualname__.split(".")
+        
+        if any(class_name):
+            class_name = class_name[0].lower()
+        
         if handler_name:
             pass
         else:
             handler_name = func.__name__
 
         if len(args):
             callback = partial(func, args[0])
+
         callback.__name__ = handler_name
-        view_function = App.app.get(f"/{callback.__name__}")
+        if class_name:
+            view_function = AndroidProber.app.get(f"/{class_name}/{callback.__name__}")
+        else:
+            view_function = AndroidProber.app.get(f"/{callback.__name__}")
+        
         fn = view_function(callback)
         swagger_metadata(**kwgs)(callback)
         return fn
 
     return get_callback
 
 def post(func = None, handler_name: str = '', **kwgs):
-
     if func is None:
         return partial(post, handler_name = handler_name ,**kwgs)
 
     @wraps(func)
     def post_callback(*args, **kwargs):
+        callback = None
         """
         Please pass the very first as instance of the class
         """
         nonlocal handler_name
+        class_name = func.__qualname__.split(".")
+        
+        if any(class_name):
+            class_name = class_name[0].lower()
+        
         if handler_name:
             pass
         else:
             handler_name = func.__name__
-
         if len(args):
             callback = partial(func, args[0])
-
+        
         callback.__name__ = handler_name
-        view_function = App.app.post(f"/{callback.__name__}")
+        if class_name:
+            view_function = AndroidProber.app.post(f"/{class_name}/{callback.__name__}")
+        else: 
+            view_function = AndroidProber.app.post(f"/{callback.__name__}")
+
         fn = view_function(callback)
         swagger_metadata(**kwgs)(callback)
         return fn
 
     return post_callback
 
 def error_handler(func = None, exec: Union[int, Exception] = 404):
     if func is None:
         return partial(error_handler, func = func, exec = exec)
-    App.app.errorhandler(exec)(func)
+    AndroidProber.app.errorhandler(exec)(func)
     return func
 
-# just make the visiablity for flask app
+# just make the visibleity for flask app
 def expose_api(class_instance : Union[Any, None] = None):
     for key , fn in vars(class_instance).items():
         if callable(fn) and "__" not in key :
             fn()
 
 # which will use of JSONRPC
 def register(route_handler, rpc_app = None, handler_name:str = ""):
@@ -89,12 +112,13 @@
     @wraps(route_handler)
     def callback(*args, **kwargs):
         if not handler_name:
             handler_name = route_handler.__name__
             if rpc_app is not None:
                 rpc_app.register(route_handler, handler_name)
             else:
-                App.app.register(route_handler, handler_name)
+                AndroidProber.app.register(route_handler, handler_name)
             response = route_handler(*args, **kwargs)
         return response
 
     return callback
+
```

### Comparing `android_prober-0.1.0/android_prober.egg-info/PKG-INFO` & `android_prober-0.1.3/android_prober.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: android-prober
-Version: 0.1.0
+Version: 0.1.3
 Summary: Library for test android api's via service
 Home-page: https://github.com/gunaNeelamegam
 Author: GunaNeelamegam
 Author-email: gunag77730@gmail.com
 License: Apacher License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask
 Requires-Dist: kivy
 Requires-Dist: oscpy
 Requires-Dist: plyer
 Requires-Dist: swagger-gen
+Requires-Dist: pyjnius==1.6.1
 
-# Library mainly Concentrated on Android and iOS Hardware Testing Library
+# Android API Testing 
+[![Upload Python Package](https://github.com/gunaNeelamegam/android-prober/actions/workflows/python-publish.yml/badge.svg)](https://github.com/gunaNeelamegam/android-prober/actions/workflows/python-publish.yml)
+[![build](https://github.com/gunaNeelamegam/android-prober/actions/workflows/build_apk.yml/badge.svg)](https://github.com/gunaNeelamegam/android-prober/actions/workflows/build_apk.yml)
 
-# Supported platform's android, linux, iOS, windows, mac
+## Library to test the AOSP Hardware APIs
 
-
-## Trying to achive
-
-* `Library to test the android internal Hardware Service's`
-
-> Developed and Tested
+> **Currently Available APIs**
 
 * [X]  Bluetooth   ᛒ
     > ABLE TO DO
     * Connect , Disconnect
     * Pair , UnPair
     * Enable, Disable Service Provider
     * look for more..
@@ -55,50 +53,29 @@
 > NOTE  💡
 * Using the Android Background Service API you can able to receive the Android Internal Event Message's
     * Aeroplane mode change's 🛩️
     * Headset adaptor state change's 🎧
     * Incoming Phone Call 📲
     * more...
 
-> NOTE 💡 
-> 
-> `Python Module's`
-  * pyjnius
-  * plyer
-  * flask
-  * kivy
-  * oscpy
-
-##  Build and Run Example's
-
-**Requirements Installation**
+## Installation
 
 ```sh
-pip3 install -r requirements.txt
+pip install android-prober
 ```
 
-**Build Debug APK**
-```sh
-    buildozer android debug
-```
+## Usage
 
-**Build And Run into Target Machine**
-```sh
-    buildozer android debug deploy run
-```
-
-> NOTE Example main file💡  
-## Example `main.py`
+* Create `main.py` like the contents below.
 
 ```python
 from kivy.app import App
 from kivy.lang import Builder
-from hardware_agent.utils.permissions import RuntimePermission
-from hardware_agent import App as TesterApp
-
+from android_prober import AndroidProber
+from requests import get
 
 KV = '''
 BoxLayout:
     orientation: 'vertical'
     BoxLayout:
         size_hint_y: None
         height: '30sp'
@@ -116,59 +93,123 @@
         Label:
             id: label
             size_hint_y: None
             height: self.texture_size[1]
             text_size: self.size[0], None
 '''
 
-class Tester(App):
+class BluetoothTestViaWebService(App):
+    
+    BASE_URL = "http://localhost:5000"
 
     def init(self):
-        self.permission = RuntimePermission()
+        """ while using webservice to invoke the API's """
         TesterApp.use_flaskapp()
 
     def on_pause(self):
         return True
 
     def telephony_permission(self):
-        self.permission.telephony_permission()
+        response = get(f"{BASE_URL}/telephony_permission")
+        print(response.json)
 
     def location_permission(self):
-        self.permission.location_permission()
+        response = get(f"{BASE_URL}/location_permission")
+        print(response.json)
 
     def bluetooth_permission(self):
-        self.permission.blutooth_permission()
+        response = get(f"{BASE_URL}/bluetooth_permission")
+        print(response.json)
 
     def build(self):
         self.init()
         self.root = Builder.load_string(KV)
         return self.root
 
 if __name__ == '__main__':
-    Tester().run()
+    BluetoothTestViaWebService().run()
+
 ```
 
-> `Way to Use Doc's`
 
-* If you are enabled developer mode. adb daemon will start's or started automatically.
+* Create `main.py` without webservice.
 
-* Run the following command.
+```python
+from kivy.app import App
+from kivy.lang import Builder
+from android_prober import AndroidProber
+from android_prober import bluetooth
 
-```bash
-adb forward tcp:5000 tcp:5000
+KV = '''
+BoxLayout:
+    orientation: 'vertical'
+    BoxLayout:
+        size_hint_y: None
+        height: '30sp'
+        Button:
+            text: 'telephony_permission'
+            on_press: app.telephony_permission()
+        Button:
+            text: 'bluetoothPermission'
+            on_press: app.bluetooth_permission()
+        Button:
+            text: 'locationPermission'
+            on_press: app.location_permission()
+
+    ScrollView:
+        Label:
+            id: label
+            size_hint_y: None
+            height: self.texture_size[1]
+            text_size: self.size[0], None
+'''
+
+class BluetoothTest(App):
+
+    def on_pause(self):
+        return True
+
+    def bluetooth_permission(self):
+       response = bluetooth.bluetooth_permission()
+        print(response)
+
+    def build(self):
+        self.root = Builder.load_string(KV)
+        return self.root
+
+if __name__ == '__main__':
+    BluetoothTest().run()
+
+```
+
+##  Build & Run
+
+```sh
+pip install -r requirements.txt
+
+buildozer android debug
 ```
-* `why tcp:5000` ?
-  
-  * Inside the Flask Application service will run on tcp:5000 port. So, we trying to expose the port inside the phone 📱 to desktop or development enviroment.
-
-* Open the any web browser 🌐
-* [API Documentation](http://localhost:5000/docs) 
-* If the previous Link not works try below.
+Install the generated apk into the target device.
+
+
+## Documentation
+
+* python for android webview recipe internally start and serve's web service running on port 5000. 
+
+* You can also test api on Single Click.
+
+![image](./android_prober/docs/images/swagger_ui.png)
+
+* Connect the device using ADB.
+
+* If your using adb via cable, Run this to expose the port `tcp/5000`
 ```bash
-    http://ipaddress:5000/docs (please replace the ip-address with the mobile connected network ip)
+adb forward tcp:5000 tcp:5000
 ```
 
-### `Looking for` 🚀
+## Upcomming updates
+
+-> https://github.com/gunaNeelamegam/android-prober/issues
 
 * Stablity
 * API for All Other Interface's
 * FastAPI Intergration
```

### Comparing `android_prober-0.1.0/setup.py` & `android_prober-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup
 from setuptools import find_namespace_packages
 from pathlib import Path
 from os import path
+from sys import version_info
 
 current_path = Path(__file__).parent
 full_path = path.join(current_path, "README.md")
 long_discription = ""
-version = "0.1.0"
+version = "0.1.3"
 name = "android-prober"
 description = "Library for test android api's via service"
 author = "GunaNeelamegam"
 url = "https://github.com/gunaNeelamegam"
 
 with open(full_path) as fd:
     long_discription = fd.read()
@@ -27,11 +28,11 @@
     url= url,
     author= author,
     author_email="gunag77730@gmail.com",
     long_description= long_discription,
     packages= find_namespace_packages(exclude = excludes),
     long_description_content_type= "text/markdown",
     py_modules = ["android_prober"],
-    install_requires = ["flask","kivy", "oscpy", "plyer", "swagger-gen"]
+    install_requires = ["flask","kivy", "oscpy", "plyer", "swagger-gen", "pyjnius==1.6.1"]
 )
```

