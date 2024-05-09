# Comparing `tmp/MpNM-0.0.0.tar.gz` & `tmp/MpNM-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MpNM-0.0.0.tar", last modified: Thu May  9 12:16:00 2024, max compression
+gzip compressed data, was "MpNM-0.1.0.tar", last modified: Thu May  9 12:11:16 2024, max compression
```

## Comparing `MpNM-0.0.0.tar` & `MpNM-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 12:16:00.189234 MpNM-0.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-09 12:16:00.182234 MpNM-0.0.0/MpNM/
--rw-rw-rw-   0        0        0      414 2024-01-16 13:04:43.000000 MpNM-0.0.0/MpNM/Base.py
--rw-rw-rw-   0        0        0      268 2024-05-09 12:02:23.000000 MpNM-0.0.0/MpNM/__init__.py
--rw-rw-rw-   0        0        0    56085 2024-05-09 11:38:08.000000 MpNM-0.0.0/MpNM/algorithm.py
--rw-rw-rw-   0        0        0    13948 2024-05-08 11:56:10.000000 MpNM-0.0.0/MpNM/network.py
--rw-rw-rw-   0        0        0     2382 2024-05-08 06:04:09.000000 MpNM-0.0.0/MpNM/phase.py
--rw-rw-rw-   0        0        0    13945 2024-05-08 06:04:09.000000 MpNM-0.0.0/MpNM/tools_numba.py
--rw-rw-rw-   0        0        0    51012 2024-05-08 06:04:09.000000 MpNM-0.0.0/MpNM/topotools.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:16:00.187235 MpNM-0.0.0/MpNM.egg-info/
--rw-rw-rw-   0        0        0     2214 2024-05-09 12:16:00.000000 MpNM-0.0.0/MpNM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-09 12:16:00.000000 MpNM-0.0.0/MpNM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 12:16:00.000000 MpNM-0.0.0/MpNM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-09 12:16:00.000000 MpNM-0.0.0/MpNM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2214 2024-05-09 12:16:00.188234 MpNM-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1596 2024-04-26 09:38:50.000000 MpNM-0.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-09 12:16:00.189234 MpNM-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     3904 2024-05-09 12:15:58.000000 MpNM-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:11:16.963915 MpNM-0.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-09 12:11:16.957915 MpNM-0.1.0/MpNM/
+-rw-rw-rw-   0        0        0      414 2024-01-16 13:04:43.000000 MpNM-0.1.0/MpNM/Base.py
+-rw-rw-rw-   0        0        0      268 2024-05-09 12:02:23.000000 MpNM-0.1.0/MpNM/__init__.py
+-rw-rw-rw-   0        0        0    56085 2024-05-09 11:38:08.000000 MpNM-0.1.0/MpNM/algorithm.py
+-rw-rw-rw-   0        0        0    13948 2024-05-08 11:56:10.000000 MpNM-0.1.0/MpNM/network.py
+-rw-rw-rw-   0        0        0     2382 2024-05-08 06:04:09.000000 MpNM-0.1.0/MpNM/phase.py
+-rw-rw-rw-   0        0        0    13945 2024-05-08 06:04:09.000000 MpNM-0.1.0/MpNM/tools_numba.py
+-rw-rw-rw-   0        0        0    51012 2024-05-08 06:04:09.000000 MpNM-0.1.0/MpNM/topotools.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:11:16.961915 MpNM-0.1.0/MpNM.egg-info/
+-rw-rw-rw-   0        0        0     2214 2024-05-09 12:11:16.000000 MpNM-0.1.0/MpNM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-09 12:11:16.000000 MpNM-0.1.0/MpNM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 12:11:16.000000 MpNM-0.1.0/MpNM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-09 12:11:16.000000 MpNM-0.1.0/MpNM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2214 2024-05-09 12:11:16.962915 MpNM-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1596 2024-04-26 09:38:50.000000 MpNM-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-09 12:11:16.963915 MpNM-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3904 2024-05-09 12:10:36.000000 MpNM-0.1.0/setup.py
```

### Comparing `MpNM-0.0.0/MpNM/algorithm.py` & `MpNM-0.1.0/MpNM/algorithm.py`

 * *Files identical despite different names*

### Comparing `MpNM-0.0.0/MpNM/network.py` & `MpNM-0.1.0/MpNM/network.py`

 * *Files identical despite different names*

### Comparing `MpNM-0.0.0/MpNM/phase.py` & `MpNM-0.1.0/MpNM/phase.py`

 * *Files identical despite different names*

### Comparing `MpNM-0.0.0/MpNM/tools_numba.py` & `MpNM-0.1.0/MpNM/tools_numba.py`

 * *Files identical despite different names*

### Comparing `MpNM-0.0.0/MpNM/topotools.py` & `MpNM-0.1.0/MpNM/topotools.py`

 * *Files identical despite different names*

### Comparing `MpNM-0.0.0/MpNM.egg-info/PKG-INFO` & `MpNM-0.1.0/MpNM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MpNM
-Version: 0.0.0
+Version: 0.1.0
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `MpNM-0.0.0/PKG-INFO` & `MpNM-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MpNM
-Version: 0.0.0
+Version: 0.1.0
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `MpNM-0.0.0/README.md` & `MpNM-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `MpNM-0.0.0/setup.py` & `MpNM-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'MpNM'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.0'
+VERSION = '0.1.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

