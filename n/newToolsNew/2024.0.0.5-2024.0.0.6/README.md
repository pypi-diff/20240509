# Comparing `tmp/newToolsNew-2024.0.0.5.tar.gz` & `tmp/newToolsNew-2024.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newToolsNew-2024.0.0.5.tar", last modified: Thu May  9 12:50:05 2024, max compression
+gzip compressed data, was "newToolsNew-2024.0.0.6.tar", last modified: Thu May  9 12:52:48 2024, max compression
```

## Comparing `newToolsNew-2024.0.0.5.tar` & `newToolsNew-2024.0.0.6.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 12:50:05.912091 newToolsNew-2024.0.0.5/
--rw-rw-rw-   0        0        0      268 2024-05-09 12:50:05.910086 newToolsNew-2024.0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 12:50:05.907094 newToolsNew-2024.0.0.5/newToolsNew.egg-info/
--rw-rw-rw-   0        0        0      268 2024-05-09 12:50:05.000000 newToolsNew-2024.0.0.5/newToolsNew.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-09 12:50:05.000000 newToolsNew-2024.0.0.5/newToolsNew.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 12:50:05.000000 newToolsNew-2024.0.0.5/newToolsNew.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-09 12:50:05.000000 newToolsNew-2024.0.0.5/newToolsNew.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      101 2024-05-09 12:50:05.000000 newToolsNew-2024.0.0.5/newToolsNew.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 12:50:05.000000 newToolsNew-2024.0.0.5/newToolsNew.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 12:50:05.912091 newToolsNew-2024.0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      806 2024-05-09 12:50:03.000000 newToolsNew-2024.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:52:48.226791 newToolsNew-2024.0.0.6/
+-rw-rw-rw-   0        0        0      268 2024-05-09 12:52:48.224795 newToolsNew-2024.0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 12:52:48.213824 newToolsNew-2024.0.0.6/newToolsNew.egg-info/
+-rw-rw-rw-   0        0        0      268 2024-05-09 12:52:48.000000 newToolsNew-2024.0.0.6/newToolsNew.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-05-09 12:52:48.000000 newToolsNew-2024.0.0.6/newToolsNew.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 12:52:48.000000 newToolsNew-2024.0.0.6/newToolsNew.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-09 12:52:48.000000 newToolsNew-2024.0.0.6/newToolsNew.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      101 2024-05-09 12:52:48.000000 newToolsNew-2024.0.0.6/newToolsNew.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 12:52:48.000000 newToolsNew-2024.0.0.6/newToolsNew.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 12:52:48.220806 newToolsNew-2024.0.0.6/newUtils/
+-rw-rw-rw-   0        0        0      128 2024-05-09 12:52:37.000000 newToolsNew-2024.0.0.6/newUtils/__init__.py
+-rw-rw-rw-   0        0        0      829 2024-05-09 09:47:40.000000 newToolsNew-2024.0.0.6/newUtils/logger.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 12:52:48.226791 newToolsNew-2024.0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      806 2024-05-09 12:52:45.000000 newToolsNew-2024.0.0.6/setup.py
```

### Comparing `newToolsNew-2024.0.0.5/setup.py` & `newToolsNew-2024.0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python 
 # -*- coding:utf-8 -*-
 # @time     : 2024/5/9 17:47
 # @Author   : new
 # @File      : setup.py
 from setuptools import setup, find_packages
 
-GFICLEE_VERSION = '2024.0.0.5'
+GFICLEE_VERSION = '2024.0.0.6'
 
 setup(
     name='newToolsNew',
     version=GFICLEE_VERSION,
     packages=find_packages(),
     include_package_data=True,
     entry_points={
```

