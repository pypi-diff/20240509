# Comparing `tmp/raster_tools-0.8.1.tar.gz` & `tmp/raster_tools-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster_tools-0.8.1.tar", last modified: Fri Apr 19 23:17:13 2024, max compression
+gzip compressed data, was "raster_tools-0.8.2.tar", last modified: Thu May  9 01:34:50 2024, max compression
```

## Comparing `raster_tools-0.8.1.tar` & `raster_tools-0.8.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-19 23:17:13.010796 raster_tools-0.8.1/
--rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster_tools-0.8.1/LICENSE
--rw-r--r--   0 fred      (1000) fred      (1000)      316 2024-01-18 23:44:47.000000 raster_tools-0.8.1/MANIFEST.in
--rw-r--r--   0 fred      (1000) fred      (1000)     2255 2024-04-19 23:17:13.010796 raster_tools-0.8.1/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2024-01-18 23:44:47.000000 raster_tools-0.8.1/README.md
--rw-r--r--   0 fred      (1000) fred      (1000)     1406 2024-01-25 17:38:15.000000 raster_tools-0.8.1/pyproject.toml
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-19 23:17:13.006796 raster_tools-0.8.1/raster_tools/
--rw-r--r--   0 fred      (1000) fred      (1000)     1052 2024-04-19 22:58:16.000000 raster_tools-0.8.1/raster_tools/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)      383 2024-01-18 23:44:47.000000 raster_tools-0.8.1/raster_tools/_compat.py
--rw-rw-r--   0 fred      (1000) fred      (1000)       22 2024-04-19 22:47:19.000000 raster_tools-0.8.1/raster_tools/_version.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7648 2024-01-25 17:38:15.000000 raster_tools-0.8.1/raster_tools/batch.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6693 2024-04-19 22:47:19.000000 raster_tools-0.8.1/raster_tools/clipping.py
--rw-r--r--   0 fred      (1000) fred      (1000)    11181 2024-01-25 17:38:15.000000 raster_tools-0.8.1/raster_tools/creation.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1600 2024-03-27 01:04:03.000000 raster_tools-0.8.1/raster_tools/dask_utils.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-19 23:17:13.006796 raster_tools-0.8.1/raster_tools/distance/
--rw-r--r--   0 fred      (1000) fred      (1000)      427 2024-01-18 23:44:47.000000 raster_tools-0.8.1/raster_tools/distance/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6737 2024-01-25 17:38:15.000000 raster_tools-0.8.1/raster_tools/distance/_heap.py
--rw-r--r--   0 fred      (1000) fred      (1000)    26525 2024-01-25 17:38:15.000000 raster_tools-0.8.1/raster_tools/distance/cost_distance.py
--rw-r--r--   0 fred      (1000) fred      (1000)    34940 2024-01-18 23:44:47.000000 raster_tools-0.8.1/raster_tools/distance/proximity.py
--rw-r--r--   0 fred      (1000) fred      (1000)     3221 2024-01-18 23:44:47.000000 raster_tools-0.8.1/raster_tools/dtypes.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    21032 2024-01-18 23:44:47.000000 raster_tools-0.8.1/raster_tools/focal.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    44579 2024-04-19 22:58:16.000000 raster_tools-0.8.1/raster_tools/general.py
--rw-r--r--   0 fred      (1000) fred      (1000)    11595 2024-01-25 17:38:15.000000 raster_tools-0.8.1/raster_tools/io.py
--rw-r--r--   0 fred      (1000) fred      (1000)    13317 2024-03-27 01:04:03.000000 raster_tools-0.8.1/raster_tools/line_stats.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2123 2024-01-18 23:44:47.000000 raster_tools-0.8.1/raster_tools/masking.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    76485 2024-04-19 22:58:16.000000 raster_tools-0.8.1/raster_tools/raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)    24204 2024-03-27 01:04:03.000000 raster_tools-0.8.1/raster_tools/rasterize.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4281 2024-01-18 23:44:47.000000 raster_tools-0.8.1/raster_tools/stat_common.py
--rw-r--r--   0 fred      (1000) fred      (1000)    18429 2024-01-25 17:38:15.000000 raster_tools-0.8.1/raster_tools/surface.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4878 2024-04-19 22:58:13.000000 raster_tools-0.8.1/raster_tools/utils.py
--rw-r--r--   0 fred      (1000) fred      (1000)    30090 2024-03-27 00:39:53.000000 raster_tools-0.8.1/raster_tools/vector.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4138 2024-02-06 00:40:10.000000 raster_tools-0.8.1/raster_tools/warp.py
--rw-r--r--   0 fred      (1000) fred      (1000)    21212 2024-03-05 21:17:32.000000 raster_tools-0.8.1/raster_tools/zonal.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-19 23:17:13.010796 raster_tools-0.8.1/raster_tools.egg-info/
--rw-r--r--   0 fred      (1000) fred      (1000)     2255 2024-04-19 23:17:12.000000 raster_tools-0.8.1/raster_tools.egg-info/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1973 2024-04-19 23:17:13.000000 raster_tools-0.8.1/raster_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)        1 2024-04-19 23:17:12.000000 raster_tools-0.8.1/raster_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)      170 2024-04-19 23:17:12.000000 raster_tools-0.8.1/raster_tools.egg-info/requires.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       13 2024-04-19 23:17:12.000000 raster_tools-0.8.1/raster_tools.egg-info/top_level.txt
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-19 23:17:13.006796 raster_tools-0.8.1/requirements/
--rw-r--r--   0 fred      (1000) fred      (1000)      170 2024-03-27 01:04:03.000000 raster_tools-0.8.1/requirements/default.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       38 2024-04-19 23:17:13.010796 raster_tools-0.8.1/setup.cfg
--rw-rw-r--   0 fred      (1000) fred      (1000)     1526 2024-01-18 23:44:47.000000 raster_tools-0.8.1/setup.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-19 23:17:13.010796 raster_tools-0.8.1/tests/
--rw-r--r--   0 fred      (1000) fred      (1000)     4332 2024-04-19 22:47:19.000000 raster_tools-0.8.1/tests/test_clipping.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4832 2024-01-25 17:38:15.000000 raster_tools-0.8.1/tests/test_creation.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7425 2024-01-25 17:38:15.000000 raster_tools-0.8.1/tests/test_distance.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1297 2024-01-18 23:44:48.000000 raster_tools-0.8.1/tests/test_distance__heap.py
--rw-r--r--   0 fred      (1000) fred      (1000)     8183 2024-01-25 17:38:15.000000 raster_tools-0.8.1/tests/test_distance_proximity.py
--rw-r--r--   0 fred      (1000) fred      (1000)    20208 2024-01-25 17:38:15.000000 raster_tools-0.8.1/tests/test_focal.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    31317 2024-04-19 22:58:16.000000 raster_tools-0.8.1/tests/test_general.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2540 2024-01-18 23:44:48.000000 raster_tools-0.8.1/tests/test_io.py
--rw-r--r--   0 fred      (1000) fred      (1000)     8004 2024-03-27 01:04:03.000000 raster_tools-0.8.1/tests/test_line_stats.py
--rw-r--r--   0 fred      (1000) fred      (1000)    85277 2024-03-29 22:22:00.000000 raster_tools-0.8.1/tests/test_raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7679 2024-01-25 17:38:15.000000 raster_tools-0.8.1/tests/test_rasterize.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4141 2024-01-25 17:38:15.000000 raster_tools-0.8.1/tests/test_stat_common.py
--rw-r--r--   0 fred      (1000) fred      (1000)     5005 2024-01-18 23:44:48.000000 raster_tools-0.8.1/tests/test_surface.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9117 2024-01-25 17:38:15.000000 raster_tools-0.8.1/tests/test_vector.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6116 2024-02-06 00:40:10.000000 raster_tools-0.8.1/tests/test_warp.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9453 2024-02-06 00:40:10.000000 raster_tools-0.8.1/tests/test_zonal.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2113 2024-01-25 17:38:15.000000 raster_tools-0.8.1/tests/testdata.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 01:34:50.812147 raster_tools-0.8.2/
+-rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster_tools-0.8.2/LICENSE
+-rw-r--r--   0 fred      (1000) fred      (1000)      316 2024-01-18 23:44:47.000000 raster_tools-0.8.2/MANIFEST.in
+-rw-r--r--   0 fred      (1000) fred      (1000)     2257 2024-05-09 01:34:50.812147 raster_tools-0.8.2/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2024-01-18 23:44:47.000000 raster_tools-0.8.2/README.md
+-rw-r--r--   0 fred      (1000) fred      (1000)     1406 2024-01-25 17:38:15.000000 raster_tools-0.8.2/pyproject.toml
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 01:34:50.808147 raster_tools-0.8.2/raster_tools/
+-rw-r--r--   0 fred      (1000) fred      (1000)     1052 2024-05-09 00:51:08.000000 raster_tools-0.8.2/raster_tools/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)      383 2024-01-18 23:44:47.000000 raster_tools-0.8.2/raster_tools/_compat.py
+-rw-r--r--   0 fred      (1000) fred      (1000)       22 2024-05-09 00:38:49.000000 raster_tools-0.8.2/raster_tools/_version.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7648 2024-01-25 17:38:15.000000 raster_tools-0.8.2/raster_tools/batch.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6693 2024-04-19 22:47:19.000000 raster_tools-0.8.2/raster_tools/clipping.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    11181 2024-01-25 17:38:15.000000 raster_tools-0.8.2/raster_tools/creation.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1600 2024-03-27 01:04:03.000000 raster_tools-0.8.2/raster_tools/dask_utils.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 01:34:50.808147 raster_tools-0.8.2/raster_tools/distance/
+-rw-r--r--   0 fred      (1000) fred      (1000)      427 2024-01-18 23:44:47.000000 raster_tools-0.8.2/raster_tools/distance/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6737 2024-01-25 17:38:15.000000 raster_tools-0.8.2/raster_tools/distance/_heap.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    26525 2024-01-25 17:38:15.000000 raster_tools-0.8.2/raster_tools/distance/cost_distance.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    34945 2024-05-09 00:38:49.000000 raster_tools-0.8.2/raster_tools/distance/proximity.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     3221 2024-01-18 23:44:47.000000 raster_tools-0.8.2/raster_tools/dtypes.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    21032 2024-01-18 23:44:47.000000 raster_tools-0.8.2/raster_tools/focal.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    44579 2024-05-09 00:51:08.000000 raster_tools-0.8.2/raster_tools/general.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    11595 2024-01-25 17:38:15.000000 raster_tools-0.8.2/raster_tools/io.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    13317 2024-03-27 01:04:03.000000 raster_tools-0.8.2/raster_tools/line_stats.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2123 2024-01-18 23:44:47.000000 raster_tools-0.8.2/raster_tools/masking.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    76485 2024-05-09 00:51:08.000000 raster_tools-0.8.2/raster_tools/raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    24204 2024-03-27 01:04:03.000000 raster_tools-0.8.2/raster_tools/rasterize.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4281 2024-01-18 23:44:47.000000 raster_tools-0.8.2/raster_tools/stat_common.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    18429 2024-01-25 17:38:15.000000 raster_tools-0.8.2/raster_tools/surface.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4878 2024-05-09 00:51:08.000000 raster_tools-0.8.2/raster_tools/utils.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    30090 2024-03-27 00:39:53.000000 raster_tools-0.8.2/raster_tools/vector.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4138 2024-02-06 00:40:10.000000 raster_tools-0.8.2/raster_tools/warp.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    21212 2024-03-05 21:17:32.000000 raster_tools-0.8.2/raster_tools/zonal.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 01:34:50.812147 raster_tools-0.8.2/raster_tools.egg-info/
+-rw-r--r--   0 fred      (1000) fred      (1000)     2257 2024-05-09 01:34:50.000000 raster_tools-0.8.2/raster_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1973 2024-05-09 01:34:50.000000 raster_tools-0.8.2/raster_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)        1 2024-05-09 01:34:50.000000 raster_tools-0.8.2/raster_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)      172 2024-05-09 01:34:50.000000 raster_tools-0.8.2/raster_tools.egg-info/requires.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       13 2024-05-09 01:34:50.000000 raster_tools-0.8.2/raster_tools.egg-info/top_level.txt
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 01:34:50.808147 raster_tools-0.8.2/requirements/
+-rw-r--r--   0 fred      (1000) fred      (1000)      172 2024-05-09 01:08:20.000000 raster_tools-0.8.2/requirements/default.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       38 2024-05-09 01:34:50.812147 raster_tools-0.8.2/setup.cfg
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1526 2024-01-18 23:44:47.000000 raster_tools-0.8.2/setup.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 01:34:50.812147 raster_tools-0.8.2/tests/
+-rw-r--r--   0 fred      (1000) fred      (1000)     4332 2024-04-19 22:47:19.000000 raster_tools-0.8.2/tests/test_clipping.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4832 2024-01-25 17:38:15.000000 raster_tools-0.8.2/tests/test_creation.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7425 2024-01-25 17:38:15.000000 raster_tools-0.8.2/tests/test_distance.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1297 2024-01-18 23:44:48.000000 raster_tools-0.8.2/tests/test_distance__heap.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    10034 2024-05-09 00:38:49.000000 raster_tools-0.8.2/tests/test_distance_proximity.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    20208 2024-01-25 17:38:15.000000 raster_tools-0.8.2/tests/test_focal.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    31317 2024-05-09 00:51:08.000000 raster_tools-0.8.2/tests/test_general.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2540 2024-01-18 23:44:48.000000 raster_tools-0.8.2/tests/test_io.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     8004 2024-03-27 01:04:03.000000 raster_tools-0.8.2/tests/test_line_stats.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    85277 2024-03-29 22:22:00.000000 raster_tools-0.8.2/tests/test_raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7679 2024-01-25 17:38:15.000000 raster_tools-0.8.2/tests/test_rasterize.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4141 2024-01-25 17:38:15.000000 raster_tools-0.8.2/tests/test_stat_common.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     5005 2024-01-18 23:44:48.000000 raster_tools-0.8.2/tests/test_surface.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9117 2024-01-25 17:38:15.000000 raster_tools-0.8.2/tests/test_vector.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6116 2024-02-06 00:40:10.000000 raster_tools-0.8.2/tests/test_warp.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9453 2024-02-06 00:40:10.000000 raster_tools-0.8.2/tests/test_zonal.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2113 2024-01-25 17:38:15.000000 raster_tools-0.8.2/tests/testdata.py
```

### Comparing `raster_tools-0.8.1/LICENSE` & `raster_tools-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/PKG-INFO` & `raster_tools-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.8.1
+Version: 0.8.2
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: affine
 Requires-Dist: cfgrib
-Requires-Dist: dask<=2024.2
+Requires-Dist: dask<=2024.2.1
 Requires-Dist: dask-geopandas
 Requires-Dist: dask-image
 Requires-Dist: fiona
 Requires-Dist: geopandas
 Requires-Dist: netcdf4
 Requires-Dist: numba
 Requires-Dist: numpy>=1.22
```

### Comparing `raster_tools-0.8.1/README.md` & `raster_tools-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/pyproject.toml` & `raster_tools-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/__init__.py` & `raster_tools-0.8.2/raster_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/batch.py` & `raster_tools-0.8.2/raster_tools/batch.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/clipping.py` & `raster_tools-0.8.2/raster_tools/clipping.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/creation.py` & `raster_tools-0.8.2/raster_tools/creation.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/dask_utils.py` & `raster_tools-0.8.2/raster_tools/dask_utils.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/distance/_heap.py` & `raster_tools-0.8.2/raster_tools/distance/_heap.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/distance/cost_distance.py` & `raster_tools-0.8.2/raster_tools/distance/cost_distance.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/distance/proximity.py` & `raster_tools-0.8.2/raster_tools/distance/proximity.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     max_dist_sqr = max_distance * max_distance
     max_dist_sqr_2 = max_dist_sqr * 2.0
 
     for ipixel in range(start, end, step):
         is_target = False
         if nt > 0:
             for j in range(nt):
-                is_target |= scan_line[j] == targets[j]
+                is_target |= scan_line[ipixel] == targets[j]
         else:
             # No targets so assume all finite and non-zero pixels are targets
             is_target = (scan_line[ipixel] != 0) & np.isfinite(
                 scan_line[ipixel]
             )
         # Are we on a target?
         if is_target:
```

### Comparing `raster_tools-0.8.1/raster_tools/dtypes.py` & `raster_tools-0.8.2/raster_tools/dtypes.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/focal.py` & `raster_tools-0.8.2/raster_tools/focal.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/general.py` & `raster_tools-0.8.2/raster_tools/general.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/io.py` & `raster_tools-0.8.2/raster_tools/io.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/line_stats.py` & `raster_tools-0.8.2/raster_tools/line_stats.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/masking.py` & `raster_tools-0.8.2/raster_tools/masking.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/raster.py` & `raster_tools-0.8.2/raster_tools/raster.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/rasterize.py` & `raster_tools-0.8.2/raster_tools/rasterize.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/stat_common.py` & `raster_tools-0.8.2/raster_tools/stat_common.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/surface.py` & `raster_tools-0.8.2/raster_tools/surface.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/utils.py` & `raster_tools-0.8.2/raster_tools/utils.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/vector.py` & `raster_tools-0.8.2/raster_tools/vector.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/warp.py` & `raster_tools-0.8.2/raster_tools/warp.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools/zonal.py` & `raster_tools-0.8.2/raster_tools/zonal.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/raster_tools.egg-info/PKG-INFO` & `raster_tools-0.8.2/raster_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.8.1
+Version: 0.8.2
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: affine
 Requires-Dist: cfgrib
-Requires-Dist: dask<=2024.2
+Requires-Dist: dask<=2024.2.1
 Requires-Dist: dask-geopandas
 Requires-Dist: dask-image
 Requires-Dist: fiona
 Requires-Dist: geopandas
 Requires-Dist: netcdf4
 Requires-Dist: numba
 Requires-Dist: numpy>=1.22
```

### Comparing `raster_tools-0.8.1/raster_tools.egg-info/SOURCES.txt` & `raster_tools-0.8.2/raster_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/setup.py` & `raster_tools-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_clipping.py` & `raster_tools-0.8.2/tests/test_clipping.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_creation.py` & `raster_tools-0.8.2/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_distance.py` & `raster_tools-0.8.2/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_distance__heap.py` & `raster_tools-0.8.2/tests/test_distance__heap.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_focal.py` & `raster_tools-0.8.2/tests/test_focal.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_general.py` & `raster_tools-0.8.2/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_io.py` & `raster_tools-0.8.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_line_stats.py` & `raster_tools-0.8.2/tests/test_line_stats.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_raster.py` & `raster_tools-0.8.2/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_rasterize.py` & `raster_tools-0.8.2/tests/test_rasterize.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_stat_common.py` & `raster_tools-0.8.2/tests/test_stat_common.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_surface.py` & `raster_tools-0.8.2/tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_vector.py` & `raster_tools-0.8.2/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_warp.py` & `raster_tools-0.8.2/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/test_zonal.py` & `raster_tools-0.8.2/tests/test_zonal.py`

 * *Files identical despite different names*

### Comparing `raster_tools-0.8.1/tests/testdata.py` & `raster_tools-0.8.2/tests/testdata.py`

 * *Files identical despite different names*

