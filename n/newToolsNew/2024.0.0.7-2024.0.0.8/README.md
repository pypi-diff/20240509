# Comparing `tmp/newToolsNew-2024.0.0.7.tar.gz` & `tmp/newToolsNew-2024.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newToolsNew-2024.0.0.7.tar", last modified: Thu May  9 13:08:46 2024, max compression
+gzip compressed data, was "newToolsNew-2024.0.0.8.tar", last modified: Thu May  9 13:19:14 2024, max compression
```

## Comparing `newToolsNew-2024.0.0.7.tar` & `newToolsNew-2024.0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 13:08:46.550805 newToolsNew-2024.0.0.7/
--rw-rw-rw-   0        0        0      268 2024-05-09 13:08:46.548785 newToolsNew-2024.0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 13:08:46.542801 newToolsNew-2024.0.0.7/newToolsNew.egg-info/
--rw-rw-rw-   0        0        0      268 2024-05-09 13:08:46.000000 newToolsNew-2024.0.0.7/newToolsNew.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-05-09 13:08:46.000000 newToolsNew-2024.0.0.7/newToolsNew.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 13:08:46.000000 newToolsNew-2024.0.0.7/newToolsNew.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-09 13:08:46.000000 newToolsNew-2024.0.0.7/newToolsNew.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      101 2024-05-09 13:08:46.000000 newToolsNew-2024.0.0.7/newToolsNew.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 13:08:46.000000 newToolsNew-2024.0.0.7/newToolsNew.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 13:08:46.545794 newToolsNew-2024.0.0.7/newUtils/
--rw-rw-rw-   0        0        0      875 2024-05-09 12:56:12.000000 newToolsNew-2024.0.0.7/newUtils/logger.py
--rw-rw-rw-   0        0        0       42 2024-05-09 13:08:46.550805 newToolsNew-2024.0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      806 2024-05-09 13:08:39.000000 newToolsNew-2024.0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:19:14.338225 newToolsNew-2024.0.0.8/
+-rw-rw-rw-   0        0        0      268 2024-05-09 13:19:14.336231 newToolsNew-2024.0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 13:19:14.329249 newToolsNew-2024.0.0.8/newToolsNew.egg-info/
+-rw-rw-rw-   0        0        0      268 2024-05-09 13:19:14.000000 newToolsNew-2024.0.0.8/newToolsNew.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-05-09 13:19:14.000000 newToolsNew-2024.0.0.8/newToolsNew.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 13:19:14.000000 newToolsNew-2024.0.0.8/newToolsNew.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-09 13:19:14.000000 newToolsNew-2024.0.0.8/newToolsNew.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      101 2024-05-09 13:19:14.000000 newToolsNew-2024.0.0.8/newToolsNew.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 13:19:14.000000 newToolsNew-2024.0.0.8/newToolsNew.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 13:19:14.333238 newToolsNew-2024.0.0.8/newUtils/
+-rw-rw-rw-   0        0        0      875 2024-05-09 12:56:12.000000 newToolsNew-2024.0.0.8/newUtils/logger.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 13:19:14.338225 newToolsNew-2024.0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      806 2024-05-09 13:19:09.000000 newToolsNew-2024.0.0.8/setup.py
```

### Comparing `newToolsNew-2024.0.0.7/newUtils/logger.py` & `newToolsNew-2024.0.0.8/newUtils/logger.py`

 * *Files identical despite different names*

### Comparing `newToolsNew-2024.0.0.7/setup.py` & `newToolsNew-2024.0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python 
 # -*- coding:utf-8 -*-
 # @time     : 2024/5/9 17:47
 # @Author   : new
 # @File      : setup.py
 from setuptools import setup, find_packages
 
-GFICLEE_VERSION = '2024.0.0.7'
+GFICLEE_VERSION = '2024.0.0.8'
 
 setup(
     name='newToolsNew',
     version=GFICLEE_VERSION,
     packages=find_packages(),
     include_package_data=True,
     entry_points={
```

