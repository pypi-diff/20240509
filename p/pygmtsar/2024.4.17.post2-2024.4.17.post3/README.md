# Comparing `tmp/pygmtsar-2024.4.17.post2.tar.gz` & `tmp/pygmtsar-2024.4.17.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtsar-2024.4.17.post2.tar", last modified: Sun Apr 28 10:50:08 2024, max compression
+gzip compressed data, was "pygmtsar-2024.4.17.post3.tar", last modified: Thu May  9 08:12:10 2024, max compression
```

## Comparing `pygmtsar-2024.4.17.post2.tar` & `pygmtsar-2024.4.17.post3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-28 10:50:08.169320 pygmtsar-2024.4.17.post2/
--rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17.post2/LICENSE.txt
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-28 10:50:08.169031 pygmtsar-2024.4.17.post2/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17.post2/README.md
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-28 10:50:08.167301 pygmtsar-2024.4.17.post2/pygmtsar/
--rw-r--r--   0 mbg        (501) staff       (20)    18153 2024-04-26 09:12:06.000000 pygmtsar-2024.4.17.post2/pygmtsar/ASF.py
--rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17.post2/pygmtsar/AWS.py
--rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17.post2/pygmtsar/GMT.py
--rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17.post2/pygmtsar/IO.py
--rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17.post2/pygmtsar/NCubeVTK.py
--rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17.post2/pygmtsar/PRM.py
--rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17.post2/pygmtsar/PRM_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17.post2/pygmtsar/S1.py
--rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack.py
--rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_align.py
--rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_base.py
--rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_dem.py
--rw-r--r--   0 mbg        (501) staff       (20)    44173 2024-02-08 18:53:49.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_detrend.py
--rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_export.py
--rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_geocode.py
--rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_incidence.py
--rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_landmask.py
--rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_multilooking.py
--rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_orbits.py
--rw-r--r--   0 mbg        (501) staff       (20)    47295 2024-03-29 07:29:11.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_phasediff.py
--rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_prm.py
--rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_ps.py
--rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_reframe.py
--rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_reframe_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    46640 2024-04-11 04:05:10.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_sbas.py
--rw-r--r--   0 mbg        (501) staff       (20)     9103 2024-04-26 15:00:33.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_stl.py
--rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_tidal.py
--rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_topo.py
--rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_trans.py
--rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_trans_inv.py
--rw-r--r--   0 mbg        (501) staff       (20)    27198 2024-04-28 10:15:51.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_unwrap.py
--rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17.post2/pygmtsar/Stack_unwrap_snaphu.py
--rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17.post2/pygmtsar/Tiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.4.17.post2/pygmtsar/XYZTiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17.post2/pygmtsar/_Stack_merge.py
--rw-r--r--   0 mbg        (501) staff       (20)     1040 2024-04-28 10:49:46.000000 pygmtsar-2024.4.17.post2/pygmtsar/__init__.py
--rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17.post2/pygmtsar/datagrid.py
--rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17.post2/pygmtsar/tqdm_dask.py
--rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17.post2/pygmtsar/tqdm_joblib.py
--rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17.post2/pygmtsar/utils.py
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-28 10:50:08.168640 pygmtsar-2024.4.17.post2/pygmtsar.egg-info/
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-28 10:50:08.000000 pygmtsar-2024.4.17.post2/pygmtsar.egg-info/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-04-28 10:50:08.000000 pygmtsar-2024.4.17.post2/pygmtsar.egg-info/SOURCES.txt
--rw-r--r--   0 mbg        (501) staff       (20)        1 2024-04-28 10:50:08.000000 pygmtsar-2024.4.17.post2/pygmtsar.egg-info/dependency_links.txt
--rw-r--r--   0 mbg        (501) staff       (20)      330 2024-04-28 10:50:08.000000 pygmtsar-2024.4.17.post2/pygmtsar.egg-info/requires.txt
--rw-r--r--   0 mbg        (501) staff       (20)        9 2024-04-28 10:50:08.000000 pygmtsar-2024.4.17.post2/pygmtsar.egg-info/top_level.txt
--rw-r--r--   0 mbg        (501) staff       (20)       38 2024-04-28 10:50:08.169374 pygmtsar-2024.4.17.post2/setup.cfg
--rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-04-11 03:27:25.000000 pygmtsar-2024.4.17.post2/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-09 08:12:10.448568 pygmtsar-2024.4.17.post3/
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17.post3/LICENSE.txt
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-09 08:12:10.448246 pygmtsar-2024.4.17.post3/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17.post3/README.md
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-09 08:12:10.446506 pygmtsar-2024.4.17.post3/pygmtsar/
+-rw-r--r--   0 mbg        (501) staff       (20)    18153 2024-04-26 09:12:06.000000 pygmtsar-2024.4.17.post3/pygmtsar/ASF.py
+-rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17.post3/pygmtsar/AWS.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17.post3/pygmtsar/GMT.py
+-rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17.post3/pygmtsar/IO.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17.post3/pygmtsar/NCubeVTK.py
+-rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17.post3/pygmtsar/PRM.py
+-rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17.post3/pygmtsar/PRM_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17.post3/pygmtsar/S1.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack.py
+-rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_align.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_dem.py
+-rw-r--r--   0 mbg        (501) staff       (20)    44539 2024-05-08 11:23:30.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_detrend.py
+-rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_export.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_geocode.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_incidence.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_landmask.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_multilooking.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_orbits.py
+-rw-r--r--   0 mbg        (501) staff       (20)    47608 2024-05-07 07:53:29.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_phasediff.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_prm.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_ps.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_reframe.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_reframe_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    46858 2024-05-01 05:44:48.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_sbas.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9103 2024-04-26 15:00:33.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_stl.py
+-rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_tidal.py
+-rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_topo.py
+-rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_trans.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_trans_inv.py
+-rw-r--r--   0 mbg        (501) staff       (20)    27198 2024-04-28 10:15:51.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_unwrap.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17.post3/pygmtsar/Stack_unwrap_snaphu.py
+-rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17.post3/pygmtsar/Tiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.4.17.post3/pygmtsar/XYZTiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17.post3/pygmtsar/_Stack_merge.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1040 2024-05-08 11:26:31.000000 pygmtsar-2024.4.17.post3/pygmtsar/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17.post3/pygmtsar/datagrid.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17.post3/pygmtsar/tqdm_dask.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17.post3/pygmtsar/tqdm_joblib.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17.post3/pygmtsar/utils.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-09 08:12:10.447869 pygmtsar-2024.4.17.post3/pygmtsar.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-09 08:12:10.000000 pygmtsar-2024.4.17.post3/pygmtsar.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-05-09 08:12:10.000000 pygmtsar-2024.4.17.post3/pygmtsar.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2024-05-09 08:12:10.000000 pygmtsar-2024.4.17.post3/pygmtsar.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      330 2024-05-09 08:12:10.000000 pygmtsar-2024.4.17.post3/pygmtsar.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2024-05-09 08:12:10.000000 pygmtsar-2024.4.17.post3/pygmtsar.egg-info/top_level.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       38 2024-05-09 08:12:10.448630 pygmtsar-2024.4.17.post3/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-04-11 03:27:25.000000 pygmtsar-2024.4.17.post3/setup.py
```

### Comparing `pygmtsar-2024.4.17.post2/LICENSE.txt` & `pygmtsar-2024.4.17.post3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/PKG-INFO` & `pygmtsar-2024.4.17.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.4.17.post2
+Version: 2024.4.17.post3
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.4.17.post2/README.md` & `pygmtsar-2024.4.17.post3/README.md`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/ASF.py` & `pygmtsar-2024.4.17.post3/pygmtsar/ASF.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/AWS.py` & `pygmtsar-2024.4.17.post3/pygmtsar/AWS.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/GMT.py` & `pygmtsar-2024.4.17.post3/pygmtsar/GMT.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/IO.py` & `pygmtsar-2024.4.17.post3/pygmtsar/IO.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/NCubeVTK.py` & `pygmtsar-2024.4.17.post3/pygmtsar/NCubeVTK.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/PRM.py` & `pygmtsar-2024.4.17.post3/pygmtsar/PRM.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/PRM_gmtsar.py` & `pygmtsar-2024.4.17.post3/pygmtsar/PRM_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/S1.py` & `pygmtsar-2024.4.17.post3/pygmtsar/S1.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_align.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_align.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_base.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_base.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_dem.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_dem.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_detrend.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_detrend.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,16 +152,16 @@
         strat_sbas = sbas.regression(unwrap_sbas.phase,
                 [topo,    topo*yy,    topo*xx,    topo*yy*xx,
                  topo**2, topo**2*yy, topo**2*xx, topo**2*yy*xx,
                  topo**3, topo**3*yy, topo**3*xx, topo**3*yy*xx,
                  yy, xx,
                  yy**2, xx**2, yy*xx,
                  yy**3, xx**3, yy**2*xx, xx**2*yy], corr_sbas)
-
-
+    
+    
         topo = sbas.interferogram(topophase)
         inc = decimator(sbas.incidence_angle())
         yy, xx = xr.broadcast(topo.y, topo.x)
         variables = [topo,  topo*yy,  topo*xx, topo*yy*xx]
         trend_sbas = sbas.regression(intf_sbas, variables, corr_sbas)
         """
         import numpy as np
@@ -169,51 +169,51 @@
         import dask
         # 'linear'
         from sklearn.linear_model import LinearRegression
         # 'sgd'
         from sklearn.linear_model import SGDRegressor
         from sklearn.pipeline import make_pipeline
         from sklearn.preprocessing import StandardScaler
-
+    
         # find stack dim
         stackvar = data.dims[0] if len(data.dims) >= 3 else 'stack'
         #print ('stackvar', stackvar)
         shape2d = data.shape[1:] if len(data.dims) == 3 else data.shape
         #print ('shape2d', shape2d)
         chunk2d = data.chunks[1:] if len(data.dims) == 3 else data.chunks
         #print ('chunk2d', chunk2d)
-
+    
         def regression_block(data, weight, *args, **kwargs):
             #assert 0, stack.shape
             data_values  = data.ravel().astype(np.float64)
             # manage variable number of variables
             variables_stack = np.stack([arg[0] if arg.ndim==3 else arg for arg in args])
             #variables_values = variables_stack.reshape(-1, variables_stack.shape[0]).T
             variables_values = variables_stack.reshape(variables_stack.shape[0], -1)
             del variables_stack
             #assert 0, f'TEST: {data_values.shape}, {variables_values.shape}'
-
+    
             nanmask_data = ~np.isfinite(data_values)
             nanmask_values = np.any(~np.isfinite(variables_values), axis=0)
             if weight.size > 1:
                 weight_values = weight.ravel().astype(np.float64)
                 nanmask_weight = ~np.isfinite(weight_values)
                 nanmask = nanmask_data | nanmask_values | nanmask_weight
                 #assert 0, f'TEST weight: {data_values.shape}, {variables_values.shape}, {weight_values.shape}'
             else:
                 weight_values = None
                 nanmask_weight = None
                 nanmask = nanmask_data | nanmask_values
-
+    
             # regression requires enough amount of valid pixels
             if data_values.size - np.sum(nanmask) < valid_pixels_threshold:
                 del data_values, variables_values, weight_values
                 del nanmask_data, nanmask_values, nanmask_weight, nanmask
                 return np.nan * np.zeros(data.shape)
-
+    
             # build prediction model with or without plane removal (fit_intercept)
             algorithm = kwargs.pop('algorithm', 'linear')
             if algorithm == 'sgd':
                 regr = make_pipeline(StandardScaler(), SGDRegressor(**kwargs))
                 fit_params = {'sgdregressor__sample_weight': weight_values[~nanmask]} if weight.size > 1 else {}
             elif algorithm == 'linear':
                 regr = make_pipeline(StandardScaler(), LinearRegression(**kwargs, copy_X=False, n_jobs=1))
@@ -223,32 +223,41 @@
             regr.fit(variables_values[:, ~nanmask].T, data_values[~nanmask], **fit_params)
             del weight_values, data_values
             model = np.full_like(data, np.nan).ravel()
             model[~nanmask_values] = regr.predict(variables_values[:, ~nanmask_values].T)
             del variables_values, regr
             del nanmask_data, nanmask_values, nanmask_weight, nanmask
             return model.reshape(data.shape).astype(np.float32)
-
+    
         dshape = data[0].shape if data.ndim==3 else data.shape
         if isinstance(variables, (list, tuple)):
             vshapes = [v[0].shape if v.ndim==3 else v.shape for v in variables]
             equals = np.all([vshape == dshape for vshape in vshapes])
-            assert equals, f'ERROR: shapes of variables slices {vshapes} and data slice {dshape} differ.'
+            if not equals:
+                print (f'NOTE: shapes of variables slices {vshapes} and data slice {dshape} differ.')
             #assert equals, f'{dshape} {vshapes}, {equals}'
-            variables_stack = [v.chunk(dict(y=chunk2d[0], x=chunk2d[1])) for v in variables]
+            variables_stack = [v.reindex_like(data).chunk(dict(y=chunk2d[0], x=chunk2d[1]))  for v in variables]
         else:
             vshape = variables[0].shape if variables.ndim==3 else variables.shape
-            assert {vshape} == {dshape}, f'ERROR: shapes of variables slice {vshape} and data slice {dshape} differ.'
-            variables_stack = [variables.chunk(dict(y=chunk2d[0], x=chunk2d[1]))]
+            if not {vshape} == {dshape}:
+                print (f'NOTE: shapes of variables slice {vshape} and data slice {dshape} differ.')
+            variables_stack = [variables.reindex_like(data).chunk(dict(y=chunk2d[0], x=chunk2d[1]))]
+    
+        if weight is not None:
+            if not weight.shape == data.shape:
+                print (f'NOTE: shapes of weight {weight.shape} and data {data.shape} differ.')
+            weight_stack = weight.reindex_like(data).chunk(dict(y=chunk2d[0], x=chunk2d[1]))
+        else:
+            weight_stack = None
 
         # xarray wrapper
         model = xr.apply_ufunc(
             regression_block,
             data,
-            weight.chunk(dict(y=chunk2d[0], x=chunk2d[1])) if weight is not None else weight,
+            weight_stack,
             *variables_stack,
             dask='parallelized',
             vectorize=False,
             output_dtypes=[np.float32],
             dask_gufunc_kwargs={**kwargs},
         )
         del variables_stack
```

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_export.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_export.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_geocode.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_geocode.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_incidence.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_incidence.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_landmask.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_landmask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_multilooking.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_multilooking.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_orbits.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_orbits.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_phasediff.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_phasediff.py`

 * *Files 2% similar despite different names*

```diff
@@ -938,42 +938,47 @@
             col_wrap=cols, size=size, aspect=aspect,
             vmin=0, vmax=1, cmap=cmap
         )
         fg.set_axis_labels('Range', 'Azimuth')
         fg.set_ticks(max_xticks=nbins, max_yticks=nbins)
         fg.fig.suptitle(caption, y=y)
 
-    def plot_correlation_stack(self, corr_stack, threshold='auto', caption='Correlation Stack', bins=100, cmap='auto'):
+    def plot_correlation_stack(self, corr_stack, threshold=None, caption='Correlation Stack', bins=100, cmap='auto'):
         import numpy as np
         import matplotlib.pyplot as plt
         import matplotlib.colors as mcolors
-
+    
         if isinstance(cmap, str) and cmap == 'auto':
             cmap = mcolors.LinearSegmentedColormap.from_list(
                 name='custom_gray', 
                 colors=['black', 'whitesmoke']
             )
-
+    
         data = corr_stack.values.flatten()
-        median_value = np.nanmedian(data)
-        if isinstance(threshold, str) and threshold == 'auto':
-            threshold = median_value
-
+    
         fig, axs = plt.subplots(1, 2)
-
+    
         ax2 = axs[0].twinx()
         axs[0].hist(data, range=(0, 1), bins=bins, density=False, cumulative=False, color='gray', edgecolor='black', alpha=0.5)
         ax2.hist(data, range=(0, 1), bins=bins, density=False, cumulative=True, color='orange', edgecolor='black', alpha=0.25)
-
-        axs[0].axvline(median_value, color='red', linestyle='dashed')
+    
+        mean_value = np.nanmean(data)
+        axs[0].axvline(mean_value, color='b', label=f'Average {mean_value:0.3f}')
+        median_value = np.nanmedian(data)
+        axs[0].axvline(median_value, color='g', label=f'Median {median_value:0.3f}')
         axs[0].set_xlim([0, 1])
         axs[0].grid()
-        axs[0].set_title(f'Histogram Median={median_value:.3f}')
         axs[0].set_xlabel('Correlation')
         axs[0].set_ylabel('Count')
         ax2.set_ylabel('Cumulative Count', color='orange')
-
-        corr_stack.where(corr_stack >= threshold).plot.imshow(cmap=cmap, vmin=0, vmax=1, ax=axs[1])
-        axs[1].set_title(f'Threshold >= {threshold:0.3f}')
-
+    
+        axs[0].set_title('Histogram')
+        if threshold is not None:
+            corr_stack.where(corr_stack > threshold).plot.imshow(cmap=cmap, vmin=0, vmax=1, ax=axs[1])
+            axs[1].set_title(f'Threshold = {threshold:0.3f}')
+            axs[0].axvline(threshold, linestyle='dashed', color='black', label=f'Threshold {threshold:0.3f}')
+        else:
+            corr_stack.where(corr_stack).plot.imshow(cmap=cmap, vmin=0, vmax=1, ax=axs[1])
+    
+        axs[0].legend()
         plt.suptitle(caption)
         plt.tight_layout()
```

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_prm.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_prm.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_ps.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_ps.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_reframe.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_reframe.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_reframe_gmtsar.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_reframe_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_sbas.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_sbas.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,40 +331,44 @@
                 df = df[(df['ref'].isin(dates))&(df['rep'].isin(dates))]
 
         if limit[1] is not None:
             print ('TODO: process upper limit')
 
         return df
 
-    def sbas_pairs(self, days=100, meters=None, invert=False, dates=None):
+    def sbas_pairs(self, days=None, meters=None, invert=False, dates=None):
         """
         Generates a sorted list of baseline pairs based on specified temporal and spatial criteria.
     
         This function creates a list of baseline pairs for Sentinel-1 data, considering the given
         temporal and spatial constraints. The list includes pairs that meet the specified days and
         meters criteria.
     
         Parameters
         ----------
         days : int, optional
-            Maximum temporal separation between image pairs in days (default is 100).
+            Maximum temporal separation between image pairs in days (default is None).
         meters : int, optional
             Maximum spatial separation between image pairs in meters (default is None).
         invert : bool, optional
             If True, invert the order of reference and repeat images (default is False).
     
         Returns
         -------
         pandas.DataFrame
             A DataFrame containing the sorted list of baseline pairs with reference and repeat dates,
             timelines, and baselines.
     
         """
         import numpy as np
         import pandas as pd
+        
+        if days is None:
+            # use large number for unlimited time interval in days
+            days = 1e6
     
         def baseline_table(dates):
             """
             Generates a baseline table for Sentinel-1 data, containing dates, times, and baseline components.
     
             This function creates a baseline table for Sentinel-1 data by processing the PRM files, which
             contain metadata for each image. The table includes dates, times, and parallel and perpendicular
@@ -403,14 +407,15 @@
                                  'ref_baseline': np.round(line1.BPR, 2),
                                  'rep_baseline': np.round(line2.BPR, 2)})
                 else:
                     data.append({'ref':line2.Index, 'rep': line1.Index,
                                  'ref_baseline': np.round(line2.BPR, 2),
                                  'rep_baseline': np.round(line1.BPR, 2)})
     
+        assert len(data) > 0, 'ERROR: No baseline pairs exist for the specified parameters'
         df = pd.DataFrame(data).sort_values(['ref', 'rep'])
         return df.assign(pair=[f'{ref} {rep}' for ref, rep in zip(df['ref'].dt.date, df['rep'].dt.date)],
                          baseline=df.rep_baseline - df.ref_baseline,
                          duration=(df['rep'] - df['ref']).dt.days,
                          rel=np.datetime64('nat'))
 
     def sbas_pairs_extend(self, baseline_pairs):
```

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_stl.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_stl.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_tidal.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_tidal.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_topo.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_topo.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_trans.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_trans.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_trans_inv.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_trans_inv.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_unwrap.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_unwrap.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Stack_unwrap_snaphu.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Stack_unwrap_snaphu.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/Tiles.py` & `pygmtsar-2024.4.17.post3/pygmtsar/Tiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/XYZTiles.py` & `pygmtsar-2024.4.17.post3/pygmtsar/XYZTiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/_Stack_merge.py` & `pygmtsar-2024.4.17.post3/pygmtsar/_Stack_merge.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/__init__.py` & `pygmtsar-2024.4.17.post3/pygmtsar/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 
 # This file is part of the PyGMTSAR project: https://github.com/mobigroup/gmtsar
 # 
 # Copyright (c) 2023, Alexey Pechnikov
 # 
 # Licensed under the BSD 3-Clause License (see LICENSE for details)
 # ----------------------------------------------------------------------------
-__version__ = '2024.4.17.post2'
+__version__ = '2024.4.17.post3'
 
 # unified progress indicators
 from .tqdm_joblib import tqdm_joblib
 from .tqdm_dask import tqdm_dask
 # base NetCDF operations and parameters on NetCDF grid
 from .datagrid import datagrid
 # top level module classes
```

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/datagrid.py` & `pygmtsar-2024.4.17.post3/pygmtsar/datagrid.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/tqdm_dask.py` & `pygmtsar-2024.4.17.post3/pygmtsar/tqdm_dask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/tqdm_joblib.py` & `pygmtsar-2024.4.17.post3/pygmtsar/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar/utils.py` & `pygmtsar-2024.4.17.post3/pygmtsar/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar.egg-info/PKG-INFO` & `pygmtsar-2024.4.17.post3/pygmtsar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.4.17.post2
+Version: 2024.4.17.post3
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.4.17.post2/pygmtsar.egg-info/SOURCES.txt` & `pygmtsar-2024.4.17.post3/pygmtsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post2/setup.py` & `pygmtsar-2024.4.17.post3/setup.py`

 * *Files identical despite different names*

