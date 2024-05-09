# Comparing `tmp/newToolsNew-2024.0.0.3.tar.gz` & `tmp/newToolsNew-2024.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newToolsNew-2024.0.0.3.tar", last modified: Thu May  9 12:40:46 2024, max compression
+gzip compressed data, was "newToolsNew-2024.0.0.4.tar", last modified: Thu May  9 12:43:41 2024, max compression
```

## Comparing `newToolsNew-2024.0.0.3.tar` & `newToolsNew-2024.0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 12:40:46.127916 newToolsNew-2024.0.0.3/
--rw-rw-rw-   0        0        0      268 2024-05-09 12:40:46.123920 newToolsNew-2024.0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 12:40:46.121948 newToolsNew-2024.0.0.3/newToolsNew.egg-info/
--rw-rw-rw-   0        0        0      268 2024-05-09 12:40:46.000000 newToolsNew-2024.0.0.3/newToolsNew.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-09 12:40:46.000000 newToolsNew-2024.0.0.3/newToolsNew.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 12:40:46.000000 newToolsNew-2024.0.0.3/newToolsNew.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-09 12:40:46.000000 newToolsNew-2024.0.0.3/newToolsNew.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      101 2024-05-09 12:40:46.000000 newToolsNew-2024.0.0.3/newToolsNew.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 12:40:46.000000 newToolsNew-2024.0.0.3/newToolsNew.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 12:40:46.127916 newToolsNew-2024.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      806 2024-05-09 12:39:13.000000 newToolsNew-2024.0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:43:41.199451 newToolsNew-2024.0.0.4/
+-rw-rw-rw-   0        0        0      268 2024-05-09 12:43:41.197458 newToolsNew-2024.0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 12:43:41.194477 newToolsNew-2024.0.0.4/newToolsNew.egg-info/
+-rw-rw-rw-   0        0        0      268 2024-05-09 12:43:41.000000 newToolsNew-2024.0.0.4/newToolsNew.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-09 12:43:41.000000 newToolsNew-2024.0.0.4/newToolsNew.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 12:43:41.000000 newToolsNew-2024.0.0.4/newToolsNew.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-09 12:43:41.000000 newToolsNew-2024.0.0.4/newToolsNew.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      101 2024-05-09 12:43:41.000000 newToolsNew-2024.0.0.4/newToolsNew.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 12:43:41.000000 newToolsNew-2024.0.0.4/newToolsNew.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 12:43:41.199451 newToolsNew-2024.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      806 2024-05-09 12:43:39.000000 newToolsNew-2024.0.0.4/setup.py
```

### Comparing `newToolsNew-2024.0.0.3/setup.py` & `newToolsNew-2024.0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python 
 # -*- coding:utf-8 -*-
 # @time     : 2024/5/9 17:47
 # @Author   : new
 # @File      : setup.py
 from setuptools import setup, find_packages
 
-GFICLEE_VERSION = '2024.0.0.3'
+GFICLEE_VERSION = '2024.0.0.4'
 
 setup(
     name='newToolsNew',
     version=GFICLEE_VERSION,
     packages=find_packages(),
     include_package_data=True,
     entry_points={
```

