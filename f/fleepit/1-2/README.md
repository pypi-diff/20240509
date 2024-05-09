# Comparing `tmp/fleepit-1.tar.gz` & `tmp/fleepit-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleepit-1.tar", last modified: Wed May  8 23:56:06 2024, max compression
+gzip compressed data, was "fleepit-2.tar", last modified: Wed May  8 23:58:17 2024, max compression
```

## Comparing `fleepit-1.tar` & `fleepit-2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pegasko   (1000) pegasko   (1000)        0 2024-05-08 23:56:06.130115 fleepit-1/
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)    11358 2024-05-08 23:36:33.000000 fleepit-1/LICENSE
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      106 2024-05-08 23:46:21.000000 fleepit-1/NOTICE
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      310 2024-05-08 23:56:06.129115 fleepit-1/PKG-INFO
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      441 2024-05-08 23:49:01.000000 fleepit-1/README.md
-drwxr-xr-x   0 pegasko   (1000) pegasko   (1000)        0 2024-05-08 23:56:06.129115 fleepit-1/fleepit.egg-info/
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      310 2024-05-08 23:56:06.000000 fleepit-1/fleepit.egg-info/PKG-INFO
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      202 2024-05-08 23:56:06.000000 fleepit-1/fleepit.egg-info/SOURCES.txt
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)        1 2024-05-08 23:56:06.000000 fleepit-1/fleepit.egg-info/dependency_links.txt
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)       41 2024-05-08 23:56:06.000000 fleepit-1/fleepit.egg-info/entry_points.txt
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)        8 2024-05-08 23:56:06.000000 fleepit-1/fleepit.egg-info/top_level.txt
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)     2642 2024-05-08 23:37:42.000000 fleepit-1/fleepit.py
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)       38 2024-05-08 23:56:06.130115 fleepit-1/setup.cfg
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      452 2024-05-08 23:51:40.000000 fleepit-1/setup.py
+drwxr-xr-x   0 pegasko   (1000) pegasko   (1000)        0 2024-05-08 23:58:17.141579 fleepit-2/
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)    11358 2024-05-08 23:36:33.000000 fleepit-2/LICENSE
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      106 2024-05-08 23:46:21.000000 fleepit-2/NOTICE
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      792 2024-05-08 23:58:17.141579 fleepit-2/PKG-INFO
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      441 2024-05-08 23:49:01.000000 fleepit-2/README.md
+drwxr-xr-x   0 pegasko   (1000) pegasko   (1000)        0 2024-05-08 23:58:17.141579 fleepit-2/fleepit.egg-info/
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      792 2024-05-08 23:58:17.000000 fleepit-2/fleepit.egg-info/PKG-INFO
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      202 2024-05-08 23:58:17.000000 fleepit-2/fleepit.egg-info/SOURCES.txt
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)        1 2024-05-08 23:58:17.000000 fleepit-2/fleepit.egg-info/dependency_links.txt
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)       41 2024-05-08 23:58:17.000000 fleepit-2/fleepit.egg-info/entry_points.txt
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)        8 2024-05-08 23:58:17.000000 fleepit-2/fleepit.egg-info/top_level.txt
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)     2642 2024-05-08 23:37:42.000000 fleepit-2/fleepit.py
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)       38 2024-05-08 23:58:17.141579 fleepit-2/setup.cfg
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      823 2024-05-08 23:58:14.000000 fleepit-2/setup.py
```

### Comparing `fleepit-1/LICENSE` & `fleepit-2/LICENSE`

 * *Files identical despite different names*

### Comparing `fleepit-1/fleepit.py` & `fleepit-2/fleepit.py`

 * *Files identical despite different names*

