# Comparing `tmp/myrt_desk_api-1.0.6.tar.gz` & `tmp/myrt_desk_api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myrt_desk_api-1.0.6.tar", last modified: Thu Jan 25 12:34:19 2024, max compression
+gzip compressed data, was "myrt_desk_api-1.0.7.tar", last modified: Thu May  9 09:26:27 2024, max compression
```

## Comparing `myrt_desk_api-1.0.6.tar` & `myrt_desk_api-1.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-01-25 12:34:19.215614 myrt_desk_api-1.0.6/
--rw-r--r--   0 mishamyrt   (501) staff       (20)    35149 2023-02-15 17:21:40.000000 myrt_desk_api-1.0.6/LICENSE
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1201 2024-01-25 12:34:19.215343 myrt_desk_api-1.0.6/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)      847 2023-02-15 17:21:40.000000 myrt_desk_api-1.0.6/README.md
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-01-25 12:34:19.209642 myrt_desk_api-1.0.6/myrt_desk_api/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2409 2023-12-23 20:26:43.000000 myrt_desk_api-1.0.6/myrt_desk_api/__init__.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-01-25 12:34:19.210255 myrt_desk_api-1.0.6/myrt_desk_api/backlight/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      177 2023-12-05 18:03:56.000000 myrt_desk_api-1.0.6/myrt_desk_api/backlight/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     3613 2023-12-23 20:43:33.000000 myrt_desk_api-1.0.6/myrt_desk_api/backlight/domain.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2767 2023-12-05 17:51:46.000000 myrt_desk_api-1.0.6/myrt_desk_api/backlight/firmware.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      949 2023-12-23 20:25:59.000000 myrt_desk_api-1.0.6/myrt_desk_api/backlight/types.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-01-25 12:34:19.211307 myrt_desk_api-1.0.6/myrt_desk_api/cli/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      134 2023-03-08 12:09:16.000000 myrt_desk_api-1.0.6/myrt_desk_api/cli/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      177 2023-02-15 17:21:40.000000 myrt_desk_api-1.0.6/myrt_desk_api/cli/assert_val.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)       82 2023-03-08 11:20:37.000000 myrt_desk_api-1.0.6/myrt_desk_api/cli/convert.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      509 2023-02-15 17:21:40.000000 myrt_desk_api-1.0.6/myrt_desk_api/cli/progress.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1508 2023-12-23 20:36:36.000000 myrt_desk_api-1.0.6/myrt_desk_api/domain.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-01-25 12:34:19.211747 myrt_desk_api-1.0.6/myrt_desk_api/legs/
--rw-r--r--   0 mishamyrt   (501) staff       (20)       54 2023-12-10 20:06:31.000000 myrt_desk_api-1.0.6/myrt_desk_api/legs/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1508 2024-01-09 12:11:56.000000 myrt_desk_api-1.0.6/myrt_desk_api/legs/domain.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      227 2024-01-09 12:08:42.000000 myrt_desk_api-1.0.6/myrt_desk_api/legs/types.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-01-25 12:34:19.212485 myrt_desk_api-1.0.6/myrt_desk_api/system/
--rw-r--r--   0 mishamyrt   (501) staff       (20)       58 2023-12-05 20:55:16.000000 myrt_desk_api-1.0.6/myrt_desk_api/system/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1688 2023-12-05 21:00:36.000000 myrt_desk_api-1.0.6/myrt_desk_api/system/domain.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2355 2023-12-10 22:02:13.000000 myrt_desk_api-1.0.6/myrt_desk_api/system/ota.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      205 2023-12-05 20:45:26.000000 myrt_desk_api-1.0.6/myrt_desk_api/system/types.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-01-25 12:34:19.213699 myrt_desk_api-1.0.6/myrt_desk_api/transport/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      215 2023-12-05 16:43:59.000000 myrt_desk_api-1.0.6/myrt_desk_api/transport/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      350 2023-03-08 10:37:55.000000 myrt_desk_api-1.0.6/myrt_desk_api/transport/bytes.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)       74 2023-12-05 16:42:19.000000 myrt_desk_api-1.0.6/myrt_desk_api/transport/constants.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2473 2023-12-23 20:21:48.000000 myrt_desk_api-1.0.6/myrt_desk_api/transport/persistent_stream.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      225 2023-12-03 23:02:54.000000 myrt_desk_api-1.0.6/myrt_desk_api/transport/ping.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     5196 2023-12-23 20:35:00.000000 myrt_desk_api-1.0.6/myrt_desk_api/transport/socket_stream.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      364 2023-12-05 16:38:52.000000 myrt_desk_api-1.0.6/myrt_desk_api/transport/types.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      105 2023-02-15 17:21:40.000000 myrt_desk_api-1.0.6/myrt_desk_api/version.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-01-25 12:34:19.214528 myrt_desk_api-1.0.6/myrt_desk_api.egg-info/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1201 2024-01-25 12:34:18.000000 myrt_desk_api-1.0.6/myrt_desk_api.egg-info/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1095 2024-01-25 12:34:19.000000 myrt_desk_api-1.0.6/myrt_desk_api.egg-info/SOURCES.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2024-01-25 12:34:18.000000 myrt_desk_api-1.0.6/myrt_desk_api.egg-info/dependency_links.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)       84 2024-01-25 12:34:19.000000 myrt_desk_api-1.0.6/myrt_desk_api.egg-info/requires.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)       14 2024-01-25 12:34:19.000000 myrt_desk_api-1.0.6/myrt_desk_api.egg-info/top_level.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)      397 2023-03-07 21:24:01.000000 myrt_desk_api-1.0.6/pyproject.toml
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-01-25 12:34:19.214966 myrt_desk_api-1.0.6/scripts/
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)     4162 2024-01-09 12:22:16.000000 myrt_desk_api-1.0.6/scripts/myrt_desk
--rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2024-01-25 12:34:19.215687 myrt_desk_api-1.0.6/setup.cfg
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1070 2024-01-25 12:26:59.000000 myrt_desk_api-1.0.6/setup.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-05-09 09:26:27.368244 myrt_desk_api-1.0.7/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)    35149 2023-02-15 17:21:40.000000 myrt_desk_api-1.0.7/LICENSE
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1346 2024-05-09 09:26:27.367999 myrt_desk_api-1.0.7/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      847 2023-02-15 17:21:40.000000 myrt_desk_api-1.0.7/README.md
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-05-09 09:26:27.358988 myrt_desk_api-1.0.7/myrt_desk_api/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2409 2023-12-23 20:26:43.000000 myrt_desk_api-1.0.7/myrt_desk_api/__init__.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-05-09 09:26:27.360285 myrt_desk_api-1.0.7/myrt_desk_api/backlight/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      177 2023-12-05 18:03:56.000000 myrt_desk_api-1.0.7/myrt_desk_api/backlight/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     3613 2023-12-23 20:43:33.000000 myrt_desk_api-1.0.7/myrt_desk_api/backlight/domain.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2767 2023-12-05 17:51:46.000000 myrt_desk_api-1.0.7/myrt_desk_api/backlight/firmware.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      949 2023-12-23 20:25:59.000000 myrt_desk_api-1.0.7/myrt_desk_api/backlight/types.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-05-09 09:26:27.361657 myrt_desk_api-1.0.7/myrt_desk_api/cli/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      134 2023-03-08 12:09:16.000000 myrt_desk_api-1.0.7/myrt_desk_api/cli/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      177 2023-02-15 17:21:40.000000 myrt_desk_api-1.0.7/myrt_desk_api/cli/assert_val.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       82 2023-03-08 11:20:37.000000 myrt_desk_api-1.0.7/myrt_desk_api/cli/convert.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      509 2023-02-15 17:21:40.000000 myrt_desk_api-1.0.7/myrt_desk_api/cli/progress.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1508 2023-12-23 20:36:36.000000 myrt_desk_api-1.0.7/myrt_desk_api/domain.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-05-09 09:26:27.362547 myrt_desk_api-1.0.7/myrt_desk_api/legs/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       54 2023-12-10 20:06:31.000000 myrt_desk_api-1.0.7/myrt_desk_api/legs/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1508 2024-01-09 12:11:56.000000 myrt_desk_api-1.0.7/myrt_desk_api/legs/domain.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      227 2024-01-09 12:08:42.000000 myrt_desk_api-1.0.7/myrt_desk_api/legs/types.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-05-09 09:26:27.363642 myrt_desk_api-1.0.7/myrt_desk_api/system/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       58 2023-12-05 20:55:16.000000 myrt_desk_api-1.0.7/myrt_desk_api/system/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1688 2023-12-05 21:00:36.000000 myrt_desk_api-1.0.7/myrt_desk_api/system/domain.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2355 2023-12-10 22:02:13.000000 myrt_desk_api-1.0.7/myrt_desk_api/system/ota.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      205 2023-12-05 20:45:26.000000 myrt_desk_api-1.0.7/myrt_desk_api/system/types.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-05-09 09:26:27.366026 myrt_desk_api-1.0.7/myrt_desk_api/transport/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      215 2023-12-05 16:43:59.000000 myrt_desk_api-1.0.7/myrt_desk_api/transport/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      350 2023-03-08 10:37:55.000000 myrt_desk_api-1.0.7/myrt_desk_api/transport/bytes.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       74 2023-12-05 16:42:19.000000 myrt_desk_api-1.0.7/myrt_desk_api/transport/constants.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2473 2023-12-23 20:21:48.000000 myrt_desk_api-1.0.7/myrt_desk_api/transport/persistent_stream.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      225 2023-12-03 23:02:54.000000 myrt_desk_api-1.0.7/myrt_desk_api/transport/ping.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     5196 2023-12-23 20:35:00.000000 myrt_desk_api-1.0.7/myrt_desk_api/transport/socket_stream.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      364 2023-12-05 16:38:52.000000 myrt_desk_api-1.0.7/myrt_desk_api/transport/types.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      105 2023-02-15 17:21:40.000000 myrt_desk_api-1.0.7/myrt_desk_api/version.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-05-09 09:26:27.367718 myrt_desk_api-1.0.7/myrt_desk_api.egg-info/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1346 2024-05-09 09:26:27.000000 myrt_desk_api-1.0.7/myrt_desk_api.egg-info/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1095 2024-05-09 09:26:27.000000 myrt_desk_api-1.0.7/myrt_desk_api.egg-info/SOURCES.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2024-05-09 09:26:27.000000 myrt_desk_api-1.0.7/myrt_desk_api.egg-info/dependency_links.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       85 2024-05-09 09:26:27.000000 myrt_desk_api-1.0.7/myrt_desk_api.egg-info/requires.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       14 2024-05-09 09:26:27.000000 myrt_desk_api-1.0.7/myrt_desk_api.egg-info/top_level.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      397 2023-03-07 21:24:01.000000 myrt_desk_api-1.0.7/pyproject.toml
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2024-05-09 09:26:27.367220 myrt_desk_api-1.0.7/scripts/
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)     4162 2024-01-09 12:22:16.000000 myrt_desk_api-1.0.7/scripts/myrt_desk
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2024-05-09 09:26:27.368290 myrt_desk_api-1.0.7/setup.cfg
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1071 2024-05-09 09:19:40.000000 myrt_desk_api-1.0.7/setup.py
```

### Comparing `myrt_desk_api-1.0.6/LICENSE` & `myrt_desk_api-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/PKG-INFO` & `myrt_desk_api-1.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: myrt_desk_api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Library for controlling smart bulbs that are controlled by the DoIT protocol
 Author: Mikhael Khrustik
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: asyncio-datagram==1.4.0
+Requires-Dist: arrrgs==3.1.0
+Requires-Dist: typing-extensions==4.11.0
+Requires-Dist: async_timeout==4.0.3
 
 # MyrtDesk API [![PyPI version](https://badge.fury.io/py/myrt-desk-api.svg)](https://pypi.org/project/myrt-desk-api/)
 
 Library for controlling smart table functions with my own [firmware](https://github.com/mishamyrt/myrt_desk_firmware).
 
 * **Fully asynchronous**
 * Automatic detection
```

### Comparing `myrt_desk_api-1.0.6/README.md` & `myrt_desk_api-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/myrt_desk_api/__init__.py` & `myrt_desk_api-1.0.7/myrt_desk_api/__init__.py`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/myrt_desk_api/backlight/domain.py` & `myrt_desk_api-1.0.7/myrt_desk_api/backlight/domain.py`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/myrt_desk_api/backlight/firmware.py` & `myrt_desk_api-1.0.7/myrt_desk_api/backlight/firmware.py`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/myrt_desk_api/backlight/types.py` & `myrt_desk_api-1.0.7/myrt_desk_api/backlight/types.py`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/myrt_desk_api/domain.py` & `myrt_desk_api-1.0.7/myrt_desk_api/domain.py`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/myrt_desk_api/legs/domain.py` & `myrt_desk_api-1.0.7/myrt_desk_api/legs/domain.py`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/myrt_desk_api/system/domain.py` & `myrt_desk_api-1.0.7/myrt_desk_api/system/domain.py`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/myrt_desk_api/system/ota.py` & `myrt_desk_api-1.0.7/myrt_desk_api/system/ota.py`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/myrt_desk_api/transport/persistent_stream.py` & `myrt_desk_api-1.0.7/myrt_desk_api/transport/persistent_stream.py`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/myrt_desk_api/transport/socket_stream.py` & `myrt_desk_api-1.0.7/myrt_desk_api/transport/socket_stream.py`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/myrt_desk_api.egg-info/PKG-INFO` & `myrt_desk_api-1.0.7/myrt_desk_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
-Name: myrt-desk-api
-Version: 1.0.6
+Name: myrt_desk_api
+Version: 1.0.7
 Summary: Library for controlling smart bulbs that are controlled by the DoIT protocol
 Author: Mikhael Khrustik
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: asyncio-datagram==1.4.0
+Requires-Dist: arrrgs==3.1.0
+Requires-Dist: typing-extensions==4.11.0
+Requires-Dist: async_timeout==4.0.3
 
 # MyrtDesk API [![PyPI version](https://badge.fury.io/py/myrt-desk-api.svg)](https://pypi.org/project/myrt-desk-api/)
 
 Library for controlling smart table functions with my own [firmware](https://github.com/mishamyrt/myrt_desk_firmware).
 
 * **Fully asynchronous**
 * Automatic detection
```

### Comparing `myrt_desk_api-1.0.6/myrt_desk_api.egg-info/SOURCES.txt` & `myrt_desk_api-1.0.7/myrt_desk_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/scripts/myrt_desk` & `myrt_desk_api-1.0.7/scripts/myrt_desk`

 * *Files identical despite different names*

### Comparing `myrt_desk_api-1.0.6/setup.py` & `myrt_desk_api-1.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,14 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
     install_requires=[
         'asyncio-datagram==1.4.0',
         'arrrgs==3.1.0',
-        'typing-extensions==4.9.0',
+        'typing-extensions==4.11.0',
         'async_timeout==4.0.3'
     ],
     python_requires='>=3.7',
     package_dir={'':'.'},
     scripts=['scripts/myrt_desk']
 )
```

