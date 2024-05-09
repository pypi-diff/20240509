# Comparing `tmp/odc-geo-0.4.3.tar.gz` & `tmp/odc_geo-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odc-geo-0.4.3.tar", last modified: Fri Mar  1 05:23:43 2024, max compression
+gzip compressed data, was "odc_geo-0.4.4.tar", last modified: Thu May  9 05:31:21 2024, max compression
```

## Comparing `odc-geo-0.4.3.tar` & `odc_geo-0.4.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 05:23:43.325128 odc-geo-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-01 05:23:33.000000 odc-geo-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-01 05:23:33.000000 odc-geo-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-03-01 05:23:43.325128 odc-geo-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-03-01 05:23:33.000000 odc-geo-0.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 05:23:43.309129 odc-geo-0.4.3/odc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 05:23:43.313129 odc-geo-0.4.3/odc/geo/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/_dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/_interop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/_rgba.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/_xr_interop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 05:23:43.317129 odc-geo-0.4.3/odc/geo/cog/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/cog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/cog/_mpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/cog/_mpu_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15472 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/cog/_rio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/cog/_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/cog/_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)    22443 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/cog/_tifffile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/crs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 05:23:43.317129 odc-geo-0.4.3/odc/geo/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/data/gbox.css
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/data/ocean.geojson.xz
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    48593 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/geobox.py
--rw-r--r--   0 runner    (1001) docker     (127)    46572 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/geom.py
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/gridspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    20777 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    20456 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21941 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/roi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/warp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-01 05:23:33.000000 odc-geo-0.4.3/odc/geo/xr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 05:23:43.321128 odc-geo-0.4.3/odc_geo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-03-01 05:23:43.000000 odc-geo-0.4.3/odc_geo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-01 05:23:43.000000 odc-geo-0.4.3/odc_geo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 05:23:43.000000 odc-geo-0.4.3/odc_geo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 05:23:43.000000 odc-geo-0.4.3/odc_geo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-01 05:23:43.000000 odc-geo-0.4.3/odc_geo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-01 05:23:43.000000 odc-geo-0.4.3/odc_geo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-01 05:23:33.000000 odc-geo-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-01 05:23:43.325128 odc-geo-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 05:23:33.000000 odc-geo-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 05:23:43.321128 odc-geo-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10731 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_cog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_crs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_dask_interop.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_gbox_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    22744 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_geobox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_geoboxtiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    33464 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_gridspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_mpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_mpu_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16607 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_rgba.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_rioxarray_interop.py
--rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_roi.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    22533 2024-03-01 05:23:33.000000 odc-geo-0.4.3/tests/test_xr_interop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.139427 odc_geo-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 05:31:10.000000 odc_geo-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-09 05:31:10.000000 odc_geo-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-09 05:31:21.139427 odc_geo-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-09 05:31:10.000000 odc_geo-0.4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.123427 odc_geo-0.4.4/odc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.127427 odc_geo-0.4.4/odc/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_interop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_rgba.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35059 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/_xr_interop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.127427 odc_geo-0.4.4/odc/geo/cog/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/_mpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/_mpu_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17800 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/_rio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24577 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/cog/_tifffile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/crs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.131427 odc_geo-0.4.4/odc/geo/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/data/gbox.css
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/data/ocean.geojson.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49544 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/geobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46572 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21824 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20456 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21941 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/roi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/warp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-09 05:31:10.000000 odc_geo-0.4.4/odc/geo/xr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.135427 odc_geo-0.4.4/odc_geo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-09 05:31:21.000000 odc_geo-0.4.4/odc_geo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-09 05:31:21.000000 odc_geo-0.4.4/odc_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:31:21.000000 odc_geo-0.4.4/odc_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:31:20.000000 odc_geo-0.4.4/odc_geo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-09 05:31:21.000000 odc_geo-0.4.4/odc_geo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 05:31:21.000000 odc_geo-0.4.4/odc_geo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-09 05:31:10.000000 odc_geo-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-09 05:31:21.139427 odc_geo-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:31:10.000000 odc_geo-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:31:21.135427 odc_geo-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_cog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_dask_interop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_gbox_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_geobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_geoboxtiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33464 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_mpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_mpu_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16607 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_rgba.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_rioxarray_interop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_roi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23073 2024-05-09 05:31:10.000000 odc_geo-0.4.4/tests/test_xr_interop.py
```

### Comparing `odc-geo-0.4.3/LICENSE` & `odc_geo-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/PKG-INFO` & `odc_geo-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-geo
-Version: 0.4.3
+Version: 0.4.4
 Summary: Geometry Classes and Operations (opendatacube)
 Home-page: https://github.com/opendatacube/odc-geo/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc-geo-0.4.3/README.rst` & `odc_geo-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/__init__.py` & `odc_geo-0.4.4/odc/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/_blocks.py` & `odc_geo-0.4.4/odc/geo/_blocks.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/_compress.py` & `odc_geo-0.4.4/odc/geo/_compress.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/_dask.py` & `odc_geo-0.4.4/odc/geo/_dask.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/_interop.py` & `odc_geo-0.4.4/odc/geo/_interop.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/_map.py` & `odc_geo-0.4.4/odc/geo/_map.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/_rgba.py` & `odc_geo-0.4.4/odc/geo/_rgba.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/_xr_interop.py` & `odc_geo-0.4.4/odc/geo/_xr_interop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # This file is part of the Open Data Cube, see https://opendatacube.org for more information
 #
 # Copyright (c) 2015-2020 ODC Contributors
 # SPDX-License-Identifier: Apache-2.0
 """
 Add ``.odc.`` extension to :py:class:`xarray.Dataset` and :class:`xarray.DataArray`.
 """
+from __future__ import annotations
+
 import functools
 import warnings
 from dataclasses import dataclass
 from datetime import datetime
 from typing import (
     Any,
     Callable,
@@ -29,15 +31,20 @@
 
 from ._interop import have, is_dask_collection
 from ._rgba import colorize, to_rgba
 from .crs import CRS, CRSError, SomeCRS, norm_crs_or_error
 from .gcp import GCPGeoBox, GCPMapping
 from .geobox import Coordinate, GeoBox, GeoboxAnchor
 from .geom import Geometry
-from .math import affine_from_axis, maybe_int, resolution_from_affine
+from .math import (
+    affine_from_axis,
+    approx_equal_affine,
+    maybe_int,
+    resolution_from_affine,
+)
 from .overlap import compute_output_geobox
 from .roi import roi_is_empty
 from .types import Resolution, SomeResolution, SomeShape, xy_
 
 # pylint: disable=import-outside-toplevel
 # pylint: disable=too-many-lines
 if have.rasterio:
@@ -170,15 +177,15 @@
     epsg = 0 if crs.epsg is None else crs.epsg
     crs_wkt = cf.get("crs_wkt", None) or crs.wkt
 
     if gcps is not None:
         cf["gcps"] = _gcps_to_json(gcps)
 
     if transform is not None:
-        cf["GeoTransform"] = " ".join(map(str, transform.to_gdal()))
+        cf["GeoTransform"] = _render_geo_transform(transform, precision=24)
 
     return xarray.DataArray(
         numpy.asarray(epsg, "int32"),
         name=name,
         dims=(),
         attrs={"spatial_ref": crs_wkt, **cf},
     )
@@ -479,48 +486,60 @@
         c, a, b, f, d, e = map(float, geo_transfrom_parts)
     except ValueError:
         return None
 
     return Affine.from_gdal(c, a, b, f, d, e)
 
 
+def _render_geo_transform(transform: Affine, precision: int = 24) -> str:
+    return " ".join(
+        map(lambda x: f"{x:.{precision}f}".rstrip("0").rstrip("."), transform.to_gdal())
+    )
+
+
 def _extract_transform(
     src: XarrayObject,
     sdims: Tuple[str, str],
     crs_coord: Optional[xarray.DataArray],
     gcp: bool,
 ) -> Optional[Affine]:
     if any(dim not in src.coords for dim in sdims):
         # special case of no spatial dims at all
         # happens for GCP/rotated sources loaded by rioxarray
         if gcp or crs_coord is None:
             return None
         return _extract_geo_transform(crs_coord)
 
     _yy, _xx = (src[dim] for dim in sdims)
+    original_transform: Affine | None = None
+    if crs_coord is not None:
+        original_transform = _extract_geo_transform(crs_coord)
 
     # First try to compute from 1-D X/Y coords
     try:
         transform = affine_from_axis(_xx.values, _yy.values)
     except ValueError:
         # This can fail when any dimension is shorter than 2 elements
         # Figure out fallback resolution if possible and try again
-        if crs_coord is None:
-            return None
-        if (original_transform := _extract_geo_transform(crs_coord)) is None:
+        if crs_coord is None or original_transform is None:
             return None
         try:
             transform = affine_from_axis(
                 _xx.values,
                 _yy.values,
                 resolution_from_affine(original_transform),
             )
         except ValueError:
             return None
 
+    if original_transform is not None and approx_equal_affine(
+        transform, original_transform
+    ):
+        transform = original_transform
+
     if not gcp and (_pix2world := _xx.encoding.get("_transform", None)) is not None:
         # non-axis aligned geobox detected
         # adjust transform
         #  world <- pix' <- pix
         transform = Affine(*_pix2world) * transform
     return transform
 
@@ -881,14 +900,19 @@
         ODCExtension.__init__(self, _locate_geo_info(xx))
         self._xx = xx
 
     @property
     def uncached(self) -> "ODCExtensionDa":
         return ODCExtensionDa(self._xx)
 
+    def reload(self) -> xarray.DataArray:
+        """Reload geospatial state info in-place."""
+        self._state = _locate_geo_info(self._xx)
+        return self._xx
+
     @property
     def ydim(self) -> int:
         """Index of the Y dimension."""
         if (sdims := self.spatial_dims) is not None:
             return self._xx.dims.index(sdims[0])
         raise ValueError("Can't locate spatial dimensions")
 
@@ -931,14 +955,19 @@
     ODC extension for :py:class:`xarray.Dataset`.
     """
 
     def __init__(self, ds: xarray.Dataset):
         ODCExtension.__init__(self, _locate_geo_info(ds))
         self._xx = ds
 
+    def reload(self) -> xarray.Dataset:
+        """Reload geospatial state info in-place."""
+        self._state = _locate_geo_info(self._xx)
+        return self._xx
+
     @property
     def uncached(self) -> "ODCExtensionDs":
         return ODCExtensionDs(self._xx)
 
     def assign_crs(
         self, crs: SomeCRS, crs_coord_name: str = _DEFAULT_CRS_COORD_NAME
     ) -> xarray.Dataset:
```

### Comparing `odc-geo-0.4.3/odc/geo/cog/_mpu.py` & `odc_geo-0.4.4/odc/geo/cog/_mpu.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/cog/_mpu_fs.py` & `odc_geo-0.4.4/odc/geo/cog/_mpu_fs.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/cog/_rio.py` & `odc_geo-0.4.4/odc/geo/cog/_rio.py`

 * *Files 21% similar despite different names*

```diff
@@ -79,26 +79,61 @@
             return {"compress": default_compress, "zlevel": default_zlevel}
         return {"compress": None}
     if isinstance(compression, str):
         compression = {"compress": compression}
     return compression
 
 
+def _get_gdal_metadata(
+    xx: xr.DataArray | list[xr.DataArray],
+    tags: Optional[Dict[str, Any]],
+) -> Dict[str, Any]:
+    """
+    Extract metadata from xarray for GDAL.
+
+    :param xx: xarray.DataArray
+    :return: Dictionary of metadata
+    """
+    meta: Dict[str, Any] = {"tags": tags}
+    if not isinstance(xx, list):
+        xx = [xx]
+
+    # The logic for this is to fill the lists with
+    # None values if the attribute is not present
+    # as only some bands may have scale and offset
+    # and we need to know which ones...
+    scales, offsets, units = [], [], []
+    for x in xx:
+        scales.append(x.attrs.get("scales", None))
+        offsets.append(x.attrs.get("offsets", None))
+        units.append(x.attrs.get("units", None))
+
+    if any(v is not None for v in scales):
+        meta["scales"] = scales
+    if any(v is not None for v in offsets):
+        meta["offsets"] = offsets
+    if any(v is not None for v in units):
+        meta["units"] = units
+
+    return meta
+
+
 def _write_cog(
     pix: np.ndarray,
     geobox: GeoBox,
     fname: Union[Path, str],
     nodata: MaybeNodata = None,
     overwrite: bool = False,
     blocksize: Optional[int] = None,
     overview_resampling: Optional[str] = None,
     overview_levels: Optional[List[int]] = None,
     ovr_blocksize: Optional[int] = None,
     use_windowed_writes: bool = False,
     intermediate_compression: Union[bool, str, Dict[str, Any]] = False,
+    gdal_metadata: Optional[Dict[str, Any]] = None,
     **extra_rio_opts,
 ) -> Union[Path, bytes]:
     if blocksize is None:
         blocksize = 512
     if ovr_blocksize is None:
         ovr_blocksize = blocksize
     if overview_resampling is None:
@@ -154,23 +189,41 @@
         rio_opts.update(nodata=nodata)
 
     rio_opts.update(extra_rio_opts)
 
     def _write(pix, band, dst):
         if not use_windowed_writes:
             dst.write(pix, band)
-            return
-
-        for _, win in dst.block_windows():
-            if pix.ndim == 2:
-                block = pix[win.toslices()]
-            else:
-                block = pix[(slice(None),) + win.toslices()]
-
-            dst.write(block, indexes=band, window=win)
+        else:
+            for _, win in dst.block_windows():
+                if pix.ndim == 2:
+                    block = pix[win.toslices()]
+                else:
+                    block = pix[(slice(None),) + win.toslices()]
+
+                dst.write(block, indexes=band, window=win)
+
+        if gdal_metadata is not None:
+            # Add scales, offsets and units if present
+            scales = gdal_metadata.get("scales", None)
+            if scales is not None:
+                dst.scales = scales
+
+            offsets = gdal_metadata.get("offsets", None)
+            if offsets is not None:
+                dst.offsets = offsets
+
+            units = gdal_metadata.get("units", None)
+            if units is not None:
+                dst.units = units
+
+            # Add any tags that are present
+            tags = gdal_metadata.get("tags", None)
+            if tags is not None:
+                dst.update_tags(**tags)
 
     # Deal efficiently with "no overviews needed case"
     if len(overview_levels) == 0:
         if fname == ":mem:":
             with rasterio.MemoryFile() as mem:
                 with mem.open(driver="GTiff", **rio_opts) as dst:
                     _write(pix, band, dst)
@@ -223,14 +276,15 @@
     blocksize: Optional[int] = None,
     ovr_blocksize: Optional[int] = None,
     overviews: Optional[Iterable[xr.DataArray]] = None,
     overview_resampling: Optional[str] = None,
     overview_levels: Optional[List[int]] = None,
     use_windowed_writes: bool = False,
     intermediate_compression: Union[bool, str, Dict[str, Any]] = False,
+    tags: Optional[Dict[str, Any]] = None,
     **extra_rio_opts,
 ) -> Union[Path, bytes]:
     """
     Save ``xarray.DataArray`` to a file in Cloud Optimized GeoTiff format.
 
     :param geo_im: ``xarray.DataArray`` with crs
     :param fname: Output path or ``":mem:"`` in which case compress to RAM and return bytes
@@ -240,15 +294,18 @@
     :param overviews: Write pre-computed overviews if supplied
     :param overview_resampling: Use this resampling when computing overviews
     :param overview_levels: List of shrink factors to compute overiews for: [2,4,8,16,32],
                             to disable overviews supply empty list ``[]``
     :param nodata: Set ``nodata`` flag to this value if supplied, by default ``nodata`` is
                    read from the attributes of the input array (``geo_im.attrs['nodata']``).
     :param use_windowed_writes: Write image block by block (might need this for large images)
-    :param intermediate_compression: Configure compression settings for first pass write, default is no compression
+    :param intermediate_compression: Configure compression settings for first pass write
+                    , default is no compression
+    :param tags: Dictionary of tags to write into the output file. These are written as
+                    GDAL Metadata items in the GeoTIFF file.
     :param extra_rio_opts: Any other option is passed to ``rasterio.open``
 
     :returns: Path to which output was written
     :returns: Bytes if ``fname=":mem:"``
 
     .. note ::
 
@@ -269,14 +326,15 @@
             layers,
             fname,
             overwrite=overwrite,
             blocksize=blocksize,
             ovr_blocksize=ovr_blocksize,
             use_windowed_writes=use_windowed_writes,
             intermediate_compression=intermediate_compression,
+            tags=tags,
             **extra_rio_opts,
         )
         assert result is not None
         return result
 
     pix = geo_im.data
     geobox = geo_im.odc.geobox
@@ -295,27 +353,29 @@
         overwrite=overwrite,
         blocksize=blocksize,
         ovr_blocksize=ovr_blocksize,
         overview_resampling=overview_resampling,
         overview_levels=overview_levels,
         use_windowed_writes=use_windowed_writes,
         intermediate_compression=intermediate_compression,
+        gdal_metadata=_get_gdal_metadata(geo_im, tags),
         **extra_rio_opts,
     )
 
 
 def to_cog(
     geo_im: xr.DataArray,
     blocksize: Optional[int] = None,
     ovr_blocksize: Optional[int] = None,
     overviews: Optional[Iterable[xr.DataArray]] = None,
     overview_resampling: Optional[str] = None,
     overview_levels: Optional[List[int]] = None,
     use_windowed_writes: bool = False,
     intermediate_compression: Union[bool, str, Dict[str, Any]] = False,
+    tags: Optional[Dict[str, Any]] = None,
     **extra_rio_opts,
 ) -> bytes:
     """
     Compress ``xarray.DataArray`` into Cloud Optimized GeoTiff bytes in memory.
 
     This function doesn't write to disk, it compresses in RAM, which is useful
     for saving data to S3 or other cloud object stores.
@@ -325,15 +385,18 @@
     :param ovr_blocksize: Size of internal tiles in overview images (defaults to blocksize)
     :param overviews: Write pre-computed overviews if supplied
     :param overview_resampling: Use this resampling when computing overviews
     :param overview_levels: List of shrink factors to compute overiews for: [2,4,8,16,32]
     :param nodata: Set ``nodata`` flag to this value if supplied, by default ``nodata`` is
                    read from the attributes of the input array (``geo_im.attrs['nodata']``).
     :param use_windowed_writes: Write image block by block (might need this for large images)
-    :param intermediate_compression: Configure compression settings for first pass write, default is no compression
+    :param intermediate_compression: Configure compression settings for first pass write
+                    , default is no compression
+    :param tags: Dictionary of tags to write into the output file. These are written as
+                    GDAL Metadata items in the GeoTIFF file.
     :param extra_rio_opts: Any other option is passed to ``rasterio.open``
 
     :returns: In-memory GeoTiff file as bytes
 
     """
     bb = write_cog(
         geo_im,
@@ -341,14 +404,15 @@
         blocksize=blocksize,
         ovr_blocksize=ovr_blocksize,
         overviews=overviews,
         overview_resampling=overview_resampling,
         overview_levels=overview_levels,
         use_windowed_writes=use_windowed_writes,
         intermediate_compression=intermediate_compression,
+        tags=tags,
         **extra_rio_opts,
     )
 
     assert isinstance(
         bb, (bytes,)
     )  # for mypy sake for :mem: output it bytes or delayed bytes
     return bb
@@ -377,14 +441,15 @@
     layers: Iterable[xr.DataArray],
     dst: Union[str, Path] = ":mem:",
     overwrite: bool = False,
     blocksize: Optional[int] = None,
     ovr_blocksize: Optional[int] = None,
     intermediate_compression: Union[bool, str, Dict[str, Any]] = False,
     use_windowed_writes: bool = False,
+    tags: Optional[Dict[str, Any]] = None,
     **extra_rio_opts,
 ) -> Union[Path, bytes, None]:
     """
     Write COG from externally computed overviews.
 
     Generates in-memory image with multiple side-car overviews, then re-encodes to destination with
     copy overviews flag set.
@@ -413,14 +478,15 @@
     rio_opts.update(extra_rio_opts)
 
     first_pass_cfg: Dict[str, Any] = {
         "num_threads": "ALL_CPUS",
         "blocksize": blocksize,
         "nodata": rio_opts.get("nodata", None),
         "use_windowed_writes": use_windowed_writes,
+        "gdal_metadata": _get_gdal_metadata(xx, tags),
         **_norm_compression_opts(intermediate_compression),
     }
 
     with _memfiles_ovr(len(xx)) as mm:
         temp_fname = mm[0].name
 
         # write each layer into mem image
```

### Comparing `odc-geo-0.4.3/odc/geo/cog/_s3.py` & `odc_geo-0.4.4/odc/geo/cog/_s3.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/cog/_shared.py` & `odc_geo-0.4.4/odc/geo/cog/_shared.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/cog/_tifffile.py` & `odc_geo-0.4.4/odc/geo/cog/_tifffile.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 from __future__ import annotations
 
 import itertools
 from functools import partial
 from io import BytesIO
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
+from xml.sax.saxutils import escape as xml_escape
 
 import numpy as np
 import xarray as xr
 
 from .._interop import have
 from ..geobox import GeoBox
 from ..types import MaybeNodata, Shape2d, Unset, shape_
@@ -35,31 +36,39 @@
     import dask.bag
     from dask.delayed import Delayed
 
 # pylint: disable=too-many-locals,too-many-branches,too-many-arguments,too-many-statements,too-many-instance-attributes
 
 
 def _render_gdal_metadata(
-    band_stats: list[dict[str, float]] | dict[str, float],
+    band_stats: list[dict[str, float]] | dict[str, float] | None,
     precision: int = 10,
     pad: int = 0,
     eol: str = "",
+    gdal_metadata_extra: Optional[List[str]] = None,
 ) -> str:
     def _item(sample: int, stats: dict[str, float]) -> str:
         return eol.join(
             [
                 f'<Item name="STATISTICS_{k.upper()}" sample="{sample:d}">{v:{pad}.{precision}f}</Item>'
                 for k, v in stats.items()
             ]
         )
 
+    if band_stats is None:
+        band_stats = []
     if isinstance(band_stats, dict):
         band_stats = [band_stats]
 
-    body = eol.join([_item(sample, stats) for sample, stats in enumerate(band_stats)])
+    gdal_metadata_extra = [] if gdal_metadata_extra is None else gdal_metadata_extra
+
+    body = eol.join(
+        [_item(sample, stats) for sample, stats in enumerate(band_stats)]
+        + gdal_metadata_extra
+    )
     return eol.join(["<GDALMetadata>", body, "</GDALMetadata>"])
 
 
 def _unwrap_stats(stats, ndim):
     if ndim == 2:
         return [{k: float(v) for k, v in stats.items()}]
 
@@ -74,41 +83,30 @@
     from dask import array as da
     from dask import delayed
 
     unwrap = delayed(_unwrap_stats, pure=True, traverse=True)
 
     axis = (yaxis, yaxis + 1)
     npix = pix.shape[yaxis] * pix.shape[yaxis + 1]
-    if nodata is not None:
-        dd = da.ma.masked_equal(pix, nodata)
-        return unwrap(
-            {
-                "minimum": dd.min(axis=axis),
-                "maximum": dd.max(axis=axis),
-                "mean": dd.mean(axis=axis),
-                "stddev": dd.std(axis=axis),
-                "valid_percent": da.isfinite(dd).sum(axis=axis) * (100 / npix),
-            },
-            pix.ndim,
-        )
 
-    if pix.dtype.kind == "f":
+    if nodata is None or np.isnan(nodata):
         dd = pix
         return unwrap(
             {
                 "minimum": da.nanmin(dd, axis=axis),
                 "maximum": da.nanmax(dd, axis=axis),
                 "mean": da.nanmean(dd, axis=axis),
                 "stddev": da.nanstd(dd, axis=axis),
                 "valid_percent": da.isfinite(dd).sum(axis=axis) * (100 / npix),
             },
             pix.ndim,
         )
 
-    dd = pix
+    # Exclude both nodata and invalid (e.g. NaN) values from statistics computation
+    dd = da.ma.masked_where((pix == nodata) | ~(np.isfinite(pix)), pix)
     return unwrap(
         {
             "minimum": dd.min(axis=axis),
             "maximum": dd.max(axis=axis),
             "mean": dd.mean(axis=axis),
             "stddev": dd.std(axis=axis),
             "valid_percent": da.isfinite(dd).sum(axis=axis) * (100 / npix),
@@ -153,24 +151,26 @@
 
     if isinstance(blocksize, int):
         blocksize = [blocksize]
 
     ax, yaxis = yaxis_from_shape(shape, gbox)
     im_shape = shape_(shape[yaxis : yaxis + 2])
     photometric = PHOTOMETRIC.MINISBLACK
-    planarconfig = PLANARCONFIG.SEPARATE
+    planarconfig: Optional[PLANARCONFIG] = PLANARCONFIG.SEPARATE
     if ax == "YX":
         nsamples = 1
     elif ax == "YXS":
         nsamples = shape[-1]
         planarconfig = PLANARCONFIG.CONTIG
         if nsamples in (3, 4):
             photometric = PHOTOMETRIC.RGB
     else:
         nsamples = shape[0]
+        if nsamples == 1:
+            planarconfig = None
 
     buf = BytesIO()
 
     opts_common = {
         "dtype": dtype,
         "photometric": photometric,
         "planarconfig": planarconfig,
@@ -465,28 +465,31 @@
 
 
 def _patch_hdr(
     tiles: List[Tuple[int, Tuple[int, int, int, int]]],
     meta: CogMeta,
     hdr0: bytes,
     stats: Optional[list[dict[str, float]]] = None,
+    gdal_metadata_extra: Optional[List[str]] = None,
 ) -> bytes:
     # pylint: disable=import-outside-toplevel,import-error
     from tifffile import TiffFile, TiffPage
 
     _tiles = [(*idx, sz) for sz, idx in tiles]
     tile_info = _extract_tile_info(meta, _tiles, 0)
 
     _bio = BytesIO(hdr0)
     with TiffFile(_bio, mode="r+", name=":mem:") as tr:
         assert len(tile_info) == len(tr.pages)
-        if stats is not None:
+        if stats is not None or gdal_metadata_extra:
             md_tag = tr.pages.first.tags.get(42112, None)
             assert md_tag is not None
-            gdal_metadata = _render_gdal_metadata(stats, precision=6)
+            gdal_metadata = _render_gdal_metadata(
+                stats, precision=6, gdal_metadata_extra=gdal_metadata_extra
+            )
             md_tag.overwrite(gdal_metadata)
 
         hdr_sz = len(_bio.getbuffer())
 
         # 324 -- offsets
         # 325 -- byte counts
         for info, page in zip(tile_info, tr.pages):
@@ -569,14 +572,48 @@
     if isinstance(predictor, Unset):
         predictor = compression in ("ADOBE_DEFLATE", "ZSTD", "LZMA")
 
     predictor = _norm_predictor(predictor, dtype)
     return (predictor, compression, compressionargs)
 
 
+def _gdal_sample_description(sample: int, description: str) -> str:
+    """Make XML line of GDAL metadata.
+
+    :param band: Sample / band number in data array.
+    :param description: Band name in data array.
+
+    :return: GDAL XML metadata line to place in TIFF file.
+    """
+    # GDAL does double escaping; see frmts/gtiff/geotiff.cpp.
+    # We also double escape to maximize compatibility with tools expecting GDAL-generated metadata.
+    double_escaped_description = xml_escape(xml_escape(description))
+    return f'<Item name="DESCRIPTION" sample="{sample}" role="description">{double_escaped_description}</Item>'
+
+
+def _band_names(xx: xr.DataArray) -> List[str]:
+    if "band" in xx.coords and xx.coords["band"].dtype.type is np.str_:
+        return list(xx["band"].values)
+    if "long_name" in xx.attrs:
+        long_name = xx.attrs["long_name"]
+        return [long_name] if isinstance(long_name, str) else long_name
+    return []
+
+
+def _gdal_sample_descriptions(descriptions: List[str]) -> List[str]:
+    """Convert band names to GDAL sample descriptions.
+
+    :return: List of GDAL XML metadata lines to place in TIFF file.
+    """
+    return [
+        _gdal_sample_description(sample, description)
+        for sample, description in enumerate(descriptions)
+    ]
+
+
 def save_cog_with_dask(
     xx: xr.DataArray,
     dst: str = "",
     *,
     compression: Union[str, Unset] = Unset(),
     compressionargs: Any = None,
     level: Optional[Union[int, float]] = None,
@@ -631,15 +668,18 @@
     assert isinstance(xx_odc.geobox, GeoBox) or xx_odc.geobox is None
 
     ydim = xx_odc.ydim
     data_chunks: Tuple[int, int] = xx.data.chunksize[ydim : ydim + 2]
     if isinstance(blocksize, Unset):
         blocksize = [data_chunks, int(max(*data_chunks) // 2)]
 
-    gdal_metadata = None if stats is False else ""
+    band_names = _band_names(xx)
+    sample_descriptions_metadata = _gdal_sample_descriptions(band_names)
+    no_metadata = (stats is False) and not band_names
+    gdal_metadata = None if no_metadata else ""
 
     meta, hdr0 = _make_empty_cog(
         xx.shape,
         xx.dtype,
         xx_odc.geobox,
         predictor=predictor,
         compression=compression,
@@ -648,14 +688,19 @@
         bigtiff=bigtiff,
         nodata=xx_odc.nodata,
         gdal_metadata=gdal_metadata,
         **kw,
     )
     hdr0 = bytes(hdr0)
 
+    if band_names and len(band_names) != meta.nsamples:
+        raise ValueError(
+            f"Found {len(band_names)} band names ({band_names}) but there are {meta.nsamples} bands."
+        )
+
     layers = _pyramids_from_cog_metadata(xx, meta, resampling=overview_resampling)
 
     if stats is True:
         stats = len(layers) // 2
 
     _stats: "Delayed" | None = None
     if stats is not False:
@@ -691,30 +736,40 @@
     if not bucket:
         # assume disk output
         write = MPUFileSink(dst, parts_base=parts_base)
         return mpu_write(
             tiles_write_order,
             write,
             mk_header=_patch_hdr,
-            user_kw={"meta": meta, "hdr0": hdr0, "stats": _stats},
+            user_kw={
+                "meta": meta,
+                "hdr0": hdr0,
+                "stats": _stats,
+                "gdal_metadata_extra": sample_descriptions_metadata,
+            },
             **upload_params,
         )
 
     upload_params["ContentType"] = (
         "image/tiff;application=geotiff;profile=cloud-optimized"
     )
 
     cleanup = aws.pop("cleanup", False)
     s3_sink = MultiPartUpload(bucket, key, **aws)
     if cleanup:
         s3_sink.cancel("all")
     return s3_sink.upload(
         tiles_write_order,
         mk_header=_patch_hdr,
-        user_kw={"meta": meta, "hdr0": hdr0, "stats": _stats},
+        user_kw={
+            "meta": meta,
+            "hdr0": hdr0,
+            "stats": _stats,
+            "gdal_metadata_extra": sample_descriptions_metadata,
+        },
         client=client,
         **upload_params,
     )
 
 
 def geotiff_metadata(
     geobox: GeoBox,
```

### Comparing `odc-geo-0.4.3/odc/geo/converters.py` & `odc_geo-0.4.4/odc/geo/converters.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/crs.py` & `odc_geo-0.4.4/odc/geo/crs.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/data/__init__.py` & `odc_geo-0.4.4/odc/geo/data/__init__.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/data/gbox.css` & `odc_geo-0.4.4/odc/geo/data/gbox.css`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/data/ocean.geojson.xz` & `odc_geo-0.4.4/odc/geo/data/ocean.geojson.xz`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/gcp.py` & `odc_geo-0.4.4/odc/geo/gcp.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/geobox.py` & `odc_geo-0.4.4/odc/geo/geobox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is part of the Open Data Cube, see https://opendatacube.org for more information
 #
 # Copyright (c) 2015-2020 ODC Contributors
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
+
 import importlib
 import itertools
 import math
 from collections import OrderedDict, namedtuple
 from typing import (
     Any,
     Callable,
@@ -24,14 +26,15 @@
 from affine import Affine
 
 from . import geom
 from .crs import CRS, MaybeCRS, SomeCRS, norm_crs
 from .geom import BoundingBox, Geometry, bbox_intersection, bbox_union
 from .math import (
     clamp,
+    extract_anchor,
     is_affine_st,
     is_almost_int,
     maybe_zero,
     resolution_from_affine,
     snap_affine,
     snap_grid,
     split_translation,
@@ -118,14 +121,19 @@
 
         self._shape = shape
         self._affine = affine
         self._crs = norm_crs(crs)
         self._extent: Optional[Geometry] = None
         self._lazy_ui = None
 
+        if self.shape.x < 0 or self.shape.y < 0:
+            raise ValueError(
+                f"Got shape {self._shape.yx!r}: negative sizes are not allowed."
+            )
+
     @property
     def width(self) -> int:
         """Width in pixels (nx)."""
         return self._shape.x
 
     @property
     def height(self) -> int:
@@ -186,19 +194,33 @@
 
     @property
     def alignment(self) -> XY[float]:
         """
         Alignment of pixel boundaries in CRS units.
 
         This is usally ``(0,0)``.
+
+        .. seealso:: :py:meth:`~odc.geo.geobox.GeoBoxBase.anchor`
         """
+        # TODO: deprecate alignment method
         rx, _, tx, _, ry, ty, *_ = self._affine
         return xy_(tx % abs(rx), ty % abs(ry))
 
     @property
+    def anchor(self) -> XY[float] | AnchorEnum:
+        """
+        Anchor point in pixel coordinates.
+
+        This is only valid for linear sources.
+        """
+        if not self.linear:
+            return AnchorEnum.FLOATING
+        return extract_anchor(self._affine)
+
+    @property
     def linear(self) -> bool:
         return True
 
     def wld2pix(self, x, y):
         return (~self._affine) * (x, y)
 
     def pix2wld(self, x, y):
@@ -572,14 +594,25 @@
             return GeoBox((ny, nx), crs=bbox.crs, affine=affine)
 
         if shape is None:
             raise ValueError("Must supply shape or resolution")
 
         shape = shape_(shape)
         nx, ny = shape.wh
+
+        if nx == 0 or ny == 0:
+            raise ValueError(
+                f"Got zero size in ({nx}, {ny}): cannot calculate resolution."
+            )
+
+        if nx < 0 or ny < 0:
+            raise ValueError(
+                f"Got negative size in ({nx}, {ny}): negative dimensions are not allowed."
+            )
+
         rx = bbox.span_x / nx
         ry = -bbox.span_y / ny
 
         if _snap is None:
             offx, offy = bbox.left, bbox.top
         else:
             offx, _ = snap_grid(bbox.left, bbox.right, rx, _snap.x, tol=tol)
```

### Comparing `odc-geo-0.4.3/odc/geo/geom.py` & `odc_geo-0.4.4/odc/geo/geom.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/gridspec.py` & `odc_geo-0.4.4/odc/geo/gridspec.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/math.py` & `odc_geo-0.4.4/odc/geo/math.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # Copyright (c) 2015-2020 ODC Contributors
 # SPDX-License-Identifier: Apache-2.0
 """
 Various mathy helpers.
 
 Minimal dependencies in this module.
 """
+from __future__ import annotations
+
 from math import ceil, floor, fmod, isfinite, log2
 from typing import (
     Any,
     Iterator,
     List,
     Literal,
     Optional,
@@ -20,15 +22,25 @@
     Union,
 )
 
 import numpy as np
 from affine import Affine
 from numpy.polynomial.polynomial import polygrid2d, polyval2d
 
-from .types import XY, Resolution, SomeResolution, SomeShape, res_, resxy_, shape_, xy_
+from .types import (
+    XY,
+    AnchorEnum,
+    Resolution,
+    SomeResolution,
+    SomeShape,
+    res_,
+    resxy_,
+    shape_,
+    xy_,
+)
 
 AffineX = TypeVar("AffineX", np.ndarray, Affine)
 
 
 def maybe_zero(x: float, tol: float) -> float:
     """Turn almost zeros to actual zeros."""
     if abs(x) < tol:
@@ -224,26 +236,34 @@
     Compute resolution and offset from x/y axis data.
 
     Only uses first two coordinate values, assumes that data is regularly
     sampled.
 
     :returns: ``(resolution, offset)``
     """
+    if not isinstance(data, np.ndarray):
+        data = data.values
+
     if data.size < 2:
         if data.size < 1:
             raise ValueError("Can't calculate resolution for empty data")
         if fallback_resolution is None:
             raise ValueError("Can't calculate resolution with data size < 2")
         res = fallback_resolution
-    else:
-        _res = (data[data.size - 1] - data[0]) / (data.size - 1.0)
-        res = _res.item()
+        off = data[0] - 0.5 * res
+        return res, float(off)
 
-    off = data[0] - 0.5 * res
-    return res, off.item()
+    x0, x1 = map(float, data[:2])
+
+    # x0 = 0*s + t + s/2
+    # x1 = 1*s + t + s/2
+    ####################
+    # s   = x1 - x0
+    # 2*t = 3*x0 - x1
+    return x1 - x0, (3 * x0 - x1) / 2
 
 
 def affine_from_axis(
     xx, yy, fallback_resolution: Optional[SomeResolution] = None
 ) -> Affine:
     """
     Compute Affine transform from axis.
@@ -285,15 +305,15 @@
 
     if fallback_resolution is not None:
         frx, fry = res_(fallback_resolution).xy
 
     xres, xoff = data_resolution_and_offset(xx, frx)
     yres, yoff = data_resolution_and_offset(yy, fry)
 
-    return Affine.translation(xoff, yoff) * Affine.scale(xres, yres)
+    return Affine(xres, 0.0, xoff, 0.0, yres, yoff)
 
 
 def apply_affine(
     A: Affine, x: np.ndarray, y: np.ndarray
 ) -> Tuple[np.ndarray, np.ndarray]:
     """
     Broadcast ``A*(x_i, y_i)`` across all elements of ``x/y``.
@@ -345,14 +365,22 @@
     :return: ``False`` if there is non-zero rotation or skew
     """
     (_, wx, _, wy, _, _, *_) = A
 
     return abs(wx) < tol and abs(wy) < tol
 
 
+def approx_equal_affine(a: Affine, b: Affine, tol: float = 1e-6) -> bool:
+    """
+    Check if two affine matrices are approximately equal.
+    """
+    sx, z1, tx, z2, sy, ty = map(lambda v: maybe_int(v, tol), (~a * b)[:6])
+    return (sx, z1, tx, z2, sy, ty) == (1, 0, 0, 0, 1, 0)
+
+
 def snap_affine(
     A: Affine, ttol: float = 1e-3, stol: float = 1e-6, tol: float = 1e-8
 ) -> Affine:
     """
     Snap scale and translation parts to integer when close enough.
 
     When scale is less than 1 then attempt snapping to ``1/<int>``.
@@ -791,7 +819,22 @@
         # denorm output side, assumes `sx==sy`
         s, _, tx, _, _, ty, *_ = ~Ab
         cc = cc * s
         cc[0, :2] += (tx, ty)
         cc = np.vstack([cc, np.asarray([0, 0])]).reshape(2, 2, 2)
 
         return Poly2d(cc, Ain)
+
+
+def extract_anchor(pix2wld: Affine, tol: float = 1e-3) -> AnchorEnum | XY[float]:
+    def _anchor(px: float, tol: float) -> float:
+        _, x = split_float(px)  # x in (-0.5, +0.5)
+        x = (1 + x) if x < 0 else x  # x in [0, 1)
+        x = snap_scale(maybe_zero(x, tol), tol)
+        return 0 if x >= 1 else x
+
+    anchor = tuple(_anchor(px, tol) for px in (~pix2wld) * (0, 0))
+    if anchor == (0, 0):
+        return AnchorEnum.EDGE
+    if anchor == (0.5, 0.5):
+        return AnchorEnum.CENTER
+    return xy_(anchor)
```

### Comparing `odc-geo-0.4.3/odc/geo/overlap.py` & `odc_geo-0.4.4/odc/geo/overlap.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/roi.py` & `odc_geo-0.4.4/odc/geo/roi.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/testutils.py` & `odc_geo-0.4.4/odc/geo/testutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import xarray as xr
 from affine import Affine
 
 from . import CRS
 from .geobox import GeoBox
 from .gridspec import GridSpec
-from .math import apply_affine, maybe_int
+from .math import apply_affine, approx_equal_affine
 
 # pylint: disable=invalid-name,
 
 epsg4326 = CRS("EPSG:4326")
 epsg3577 = CRS("EPSG:3577")
 epsg3857 = CRS("EPSG:3857")
 esri54019 = CRS("ESRI:54019")
@@ -225,17 +225,12 @@
         data=da.from_array(xx.data, **kw),
         dims=xx.dims,
         coords=xx.coords,
         attrs=xx.attrs,
     )
 
 
-def approx_equal_affine(a: Affine, b: Affine, tol: float = 1e-6) -> bool:
-    sx, z1, tx, z2, sy, ty = map(lambda v: maybe_int(v, tol), (~a * b)[:6])
-    return (sx, z1, tx, z2, sy, ty) == (1, 0, 0, 0, 1, 0)
-
-
 def approx_equal_geobox(a: GeoBox, b: GeoBox, tol: float = 1e-6) -> bool:
     if a.shape != b.shape or a.crs != b.crs:
         return False
 
     return approx_equal_affine(a.transform, b.transform, tol)
```

### Comparing `odc-geo-0.4.3/odc/geo/types.py` & `odc_geo-0.4.4/odc/geo/types.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/ui.py` & `odc_geo-0.4.4/odc/geo/ui.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/warp.py` & `odc_geo-0.4.4/odc/geo/warp.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc/geo/xr.py` & `odc_geo-0.4.4/odc/geo/xr.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/odc_geo.egg-info/PKG-INFO` & `odc_geo-0.4.4/odc_geo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-geo
-Version: 0.4.3
+Version: 0.4.4
 Summary: Geometry Classes and Operations (opendatacube)
 Home-page: https://github.com/opendatacube/odc-geo/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc-geo-0.4.3/odc_geo.egg-info/SOURCES.txt` & `odc_geo-0.4.4/odc_geo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/pyproject.toml` & `odc_geo-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/setup.cfg` & `odc_geo-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_bbox.py` & `odc_geo-0.4.4/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_blocks.py` & `odc_geo-0.4.4/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_cog.py` & `odc_geo-0.4.4/tests/test_cog.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 import itertools
 from io import BytesIO
 from pathlib import Path
 from typing import Optional, Tuple
 
+import numpy as np
 import pytest
 
+_ = pytest.importorskip("tifffile")
+_ = pytest.importorskip("rasterio")
+
+from dask import array as da
+from rasterio import MemoryFile
+from rasterio import open as rio_open
+
 from odc.geo.cog import CogMeta, cog_gbox, save_cog_with_dask
 from odc.geo.cog._shared import compute_cog_spec, num_overviews
 from odc.geo.cog._tifffile import (
     GEOTIFF_TAGS,
+    _band_names,
+    _gdal_sample_description,
+    _gdal_sample_descriptions,
     _make_empty_cog,
     _norm_compression_tifffile,
+    _stats_from_layer,
     geotiff_metadata,
 )
 from odc.geo.geobox import GeoBox
 from odc.geo.gridspec import GridSpec
 from odc.geo.types import Unset, wh_
 from odc.geo.xr import xr_zeros
 
@@ -45,14 +57,59 @@
 
     img_bytes2 = img.odc.write_cog(
         ":mem:", blocksize=32, overview_levels=[2], use_windowed_writes=True
     )
     assert len(img_bytes) == len(img_bytes2)
 
 
+@pytest.mark.parametrize(
+    ["scales", "offsets", "units"],
+    [
+        (0.1, 999, "fridges"),
+        (0.1, 999, None),
+    ],
+)
+def test_write_metadata(gbox: GeoBox, scales, offsets, units):
+    RANDOM = "random_value"
+    img = xr_zeros(gbox, dtype="uint16")
+    assert img.odc.geobox == gbox
+
+    img.attrs.update(scales=scales, offsets=offsets, units=units)
+
+    assert img.attrs["scales"] == scales
+
+    img_bytes = img.odc.to_cog(
+        blocksize=32,
+        tags=dict(random_tag=RANDOM),
+    )
+    with MemoryFile(img_bytes) as memfile:
+        with rio_open(memfile) as src:
+            # Make sure values are set and retrieved correctly
+            if isinstance(scales, (list, tuple)):
+                assert src.scales == tuple(scales)
+            else:
+                assert src.scales[0] == scales
+
+            if isinstance(offsets, (list, tuple)):
+                assert src.offsets == tuple(offsets)
+            else:
+                assert src.offsets[0] == offsets
+
+            if isinstance(units, (list, tuple)):
+                assert src.units == tuple(units)
+            else:
+                assert src.units[0] == units
+
+            # Check tags stick
+            assert src.tags()["random_tag"] == RANDOM
+
+            # Check the underlying data asn't altered
+            assert (src.read() == img.data).all()
+
+
 def test_write_cog_ovr(gbox: GeoBox):
     img = xr_zeros(gbox, dtype="uint16")
     assert img.odc.geobox == gbox
     ovrs = [img[::2, ::2], img[::4, ::4]]
 
     img_bytes = img.odc.to_cog(blocksize=32, overviews=ovrs)
     assert isinstance(img_bytes, bytes)
@@ -327,14 +384,85 @@
         else:
             assert md["GTModelTypeGeoKey"] == 2
             assert md["GeographicTypeGeoKey"] == gbox.crs.epsg
     else:
         assert md["GTModelTypeGeoKey"] == 32767
 
 
+@pytest.mark.parametrize(
+    ("sample", "description", "expected"),
+    [
+        (
+            0,
+            "easy",
+            '<Item name="DESCRIPTION" sample="0" role="description">easy</Item>',
+        ),
+        (
+            1,
+            "<",
+            '<Item name="DESCRIPTION" sample="1" role="description">&amp;lt;</Item>',
+        ),
+        (
+            2,
+            ">",
+            '<Item name="DESCRIPTION" sample="2" role="description">&amp;gt;</Item>',
+        ),
+        (
+            3,
+            "&",
+            '<Item name="DESCRIPTION" sample="3" role="description">&amp;amp;</Item>',
+        ),
+        (
+            4,
+            "& <a>",
+            '<Item name="DESCRIPTION" sample="4" role="description">&amp;amp; &amp;lt;a&amp;gt;</Item>',
+        ),
+    ],
+)
+def test_gdal_sample_description(sample: int, description: str, expected: str):
+    assert _gdal_sample_description(sample, description) == expected
+
+
+def test_gdal_sample_descriptions():
+    assert _gdal_sample_descriptions(["red", "green", "blue"]) == [
+        '<Item name="DESCRIPTION" sample="0" role="description">red</Item>',
+        '<Item name="DESCRIPTION" sample="1" role="description">green</Item>',
+        '<Item name="DESCRIPTION" sample="2" role="description">blue</Item>',
+    ]
+
+
+def test_band_names(gbox: GeoBox):
+    gbox = gbox.zoom_to(1024)
+    dtype = "float32"
+    n = 512
+    nodata = -9999
+
+    img = xr_zeros(gbox, dtype, chunks=(n, n), nodata=nodata)
+    img.attrs["long_name"] = []
+
+    assert _band_names(img) == []
+
+    img.attrs["long_name"] = "first band"
+    assert _band_names(img) == ["first band"]
+
+    img.attrs["long_name"] = ["first band"]
+    assert _band_names(img) == ["first band"]
+
+    img = img.odc.colorize()
+    assert img.ndim == 3
+
+    # Obtain descriptions from strings in "band" coordinate
+    assert _band_names(img) == ["r", "g", "b", "a"]
+
+    # Obtain descriptions from "long_names" attribute
+    img["band"] = [0, 1, 2, 3]
+    img.attrs["long_name"] = ["red", "green", "blue", "alpha"]
+    assert _band_names(img) == ["red", "green", "blue", "alpha"]
+
+
 @pytest.mark.parametrize("dtype", ["int16", "float32"])
 def test_cog_with_dask_smoke_test(gbox: GeoBox, tmp_path: Path, dtype):
     gbox = gbox.zoom_to(1024)
     assert gbox.shape == (1024, 1024)
     n = 512
     nodata = -9999
 
@@ -351,15 +479,95 @@
     assert img.odc.ydim == 0
 
     fname = str(tmp_path / "cog-rgba.tif")
     fut = save_cog_with_dask(img, fname, compression="deflate", level=2)
     rr = fut.compute()
     assert str(rr) == fname
 
-    # SYX
+    # SYX, one band
+    img = xr_zeros(gbox, dtype, chunks=(1, n, n), time=["2000"])
+    assert img.ndim == 3
+    assert img.odc.ydim == 1
+    fname = str(tmp_path / "cog-syx-one-band.tif")
+    fut = save_cog_with_dask(img, fname, compression="deflate", level=2)
+    rr = fut.compute()
+    assert str(rr) == fname
+
+    # SYX, multiple bands
     img = xr_zeros(gbox, dtype, chunks=(1, n, n), time=["2000", "2001"])
     assert img.ndim == 3
     assert img.odc.ydim == 1
     fname = str(tmp_path / "cog-syx.tif")
     fut = save_cog_with_dask(img, fname, compression="deflate", level=2)
     rr = fut.compute()
     assert str(rr) == fname
+
+    # Band names
+    img.attrs["long_name"] = ["2000", "2001"]
+    fname = str(tmp_path / "cog-bandnames.tif")
+    fut = save_cog_with_dask(img, fname, compression="deflate", level=2)
+    rr = fut.compute()
+    assert str(rr) == fname
+
+    # Incorrect number of band names
+    img.attrs["long_name"] = ["red", "green", "blue"]
+    fname = str(tmp_path / "cog-bandnames-incorrect.tif")
+    with pytest.raises(ValueError):
+        save_cog_with_dask(img, fname, compression="deflate", level=2)
+
+
+@pytest.mark.parametrize(
+    ("array", "nodata", "minimum", "maximum", "mean", "stddev", "valid_percent"),
+    [
+        pytest.param([[1, 1], [1, 1]], None, 1, 1, 1, 0, 100, id="basic int"),
+        pytest.param(
+            [[1.0, 1.0], [1.0, 1.0]], None, 1.0, 1.0, 1.0, 0.0, 100, id="basic float"
+        ),
+        pytest.param([[1, 0], [0, 1]], 0, 1, 1, 1, 0, 50, id="int with numeric nodata"),
+        pytest.param(
+            [[1.0, 0.0], [0.0, 1.0]], 0, 1, 1, 1, 0, 50, id="float with numeric nodata"
+        ),
+        pytest.param(
+            [[1.0, np.nan], [np.nan, 1.0]],
+            None,
+            1,
+            1,
+            1,
+            0,
+            50,
+            id="float with nan, None nodata",
+        ),
+        pytest.param(
+            [[1.0, np.nan], [np.nan, 1.0]],
+            np.nan,
+            1,
+            1,
+            1,
+            0,
+            50,
+            id="float with nan, nan nodata",
+        ),
+        pytest.param(
+            [
+                [1.0, np.nan],
+                [0.0, 9.0],
+            ],
+            0,
+            1,
+            9.0,
+            5.0,
+            4.0,
+            50,
+            id="float with nan, numeric nodata",
+        ),
+    ],
+)
+def test_stats_from_layer(array, nodata, minimum, maximum, mean, stddev, valid_percent):
+    x = da.from_array(array)
+    stats = _stats_from_layer(x, nodata).compute()[0]
+
+    assert stats["minimum"] == minimum
+    assert stats["maximum"] == maximum
+    assert stats["mean"] == mean
+    assert stats["stddev"] == stddev
+    assert stats["valid_percent"] == valid_percent
+    assert stats["valid_percent"] == valid_percent
```

### Comparing `odc-geo-0.4.3/tests/test_converters.py` & `odc_geo-0.4.4/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_crs.py` & `odc_geo-0.4.4/tests/test_crs.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_dask_interop.py` & `odc_geo-0.4.4/tests/test_dask_interop.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_datasets.py` & `odc_geo-0.4.4/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_gbox_ops.py` & `odc_geo-0.4.4/tests/test_gbox_ops.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_gcp.py` & `odc_geo-0.4.4/tests/test_gcp.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 import numpy as np
 import pytest
 
 from odc.geo import geom
 from odc.geo.gcp import GCPGeoBox, GCPMapping
-from odc.geo.geobox import GeoBox
+from odc.geo.geobox import AnchorEnum, GeoBox
 from odc.geo.xr import xr_zeros
 
 rasterio = pytest.importorskip("rasterio")
 
 
 @pytest.fixture()
 def au_gcp_rio(data_dir: Path):
@@ -101,14 +101,16 @@
     assert _mapping.crs is None
     gbox_ = GCPGeoBox(gbox.shape, _mapping)
     assert gbox_.crs is None
     p1, p2 = gbox_.map_bounds()
     assert p1 == pytest.approx((-44.50301336231415, 109.39806656168265))
     assert p2 == pytest.approx((-9.47177497427409, 157.04711254391185))
 
+    assert gbox.anchor == AnchorEnum.FLOATING
+
 
 def test_gcp_geobox_xr(au_gcp_geobox: GCPGeoBox):
     gbox = au_gcp_geobox
     xx = xr_zeros(gbox)
     _gbox = xx.odc.geobox
     assert _gbox.shape == gbox.shape
     assert _gbox.crs == gbox.crs
```

### Comparing `odc-geo-0.4.3/tests/test_geobox.py` & `odc_geo-0.4.4/tests/test_geobox.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Copyright (c) 2015-2020 ODC Contributors
 # SPDX-License-Identifier: Apache-2.0
 
 import numpy as np
 import pytest
 from affine import Affine
 
-from odc.geo._interop import have
 from odc.geo import CRS, geom, ixy_, resxy_, resyx_, wh_, xy_
+from odc.geo._interop import have
 from odc.geo.geobox import (
     AnchorEnum,
     GeoBox,
     bounding_box_in_pixel_domain,
     gbox_boundary,
     geobox_intersection_conservative,
     geobox_union_conservative,
@@ -662,15 +662,15 @@
         GeoBox.from_bbox((-10, -2, 5, 4), "epsg:3857", tight=True, resolution=1),
         GeoBox.from_bbox(
             (-10, -2, 5, 4), "epsg:3857", tight=True, resolution=resxy_(1, 2)
         ),
     ],
 )
 def test_explore_geobox(geobox):
-    from folium import Map, GeoJson
+    from folium import GeoJson, Map
 
     # Test explore on dataset input and verify that output is a folium map
     # that contains a GeoJson layer
     m = geobox.explore()
     assert isinstance(m, Map)
     assert sum(isinstance(child, GeoJson) for child in m._children.values()) == 2
 
@@ -681,7 +681,57 @@
     # Verify that passing a custom map works correctly
     m_external = Map()
     geobox.explore(map=m_external)
     assert isinstance(m_external, Map)
     assert (
         sum(isinstance(child, GeoJson) for child in m_external._children.values()) == 2
     )
+
+
+@pytest.mark.parametrize(
+    ("shape", "allowed"),
+    [
+        pytest.param((100, 100), True, id="positive xy: normal"),
+        pytest.param((0, 100), False, id="zero x: can't calculate resolution"),
+        pytest.param((100, 0), False, id="zero y: can't calculate resolution"),
+        pytest.param((-100, 100), False, id="negative x: not allowed"),
+        pytest.param((100, -100), False, id="negative y: not allowed"),
+        pytest.param((-100, -100), False, id="both negative: not allowed"),
+    ],
+)
+def test_shape(shape, allowed):
+    if allowed:
+        GeoBox.from_bbox((-3, -4, 3, 4), epsg4326, shape=shape)
+    else:
+        with pytest.raises(ValueError):
+            GeoBox.from_bbox((-3, -4, 3, 4), epsg4326, shape=shape)
+
+
+@pytest.mark.parametrize(
+    "gbox, expected_anchor",
+    [
+        (
+            GeoBox.from_bbox((3, 4, 5, 7), epsg4326, resolution=0.25, anchor="edge"),
+            AnchorEnum.EDGE,
+        ),
+        (
+            GeoBox.from_bbox((-3, -4, 5, 7), epsg4326, resolution=0.25),
+            AnchorEnum.EDGE,
+        ),
+        (
+            GeoBox.from_bbox(
+                (-3, -4, 5, 7), epsg4326, resolution=0.25, anchor="center"
+            ),
+            AnchorEnum.CENTER,
+        ),
+        (
+            GeoBox.from_bbox((35, 40, 50, 70), epsg3857, resolution=10, tight=True),
+            xy_(0.5, 0.0),
+        ),
+        (
+            GeoBox.from_bbox((-31, 40, 50, 72), epsg3857, resolution=10, tight=True),
+            xy_(0.1, 0.2),
+        ),
+    ],
+)
+def test_geobox_anchor(gbox, expected_anchor):
+    assert gbox.anchor == expected_anchor
```

### Comparing `odc-geo-0.4.3/tests/test_geoboxtiles.py` & `odc_geo-0.4.4/tests/test_geoboxtiles.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_geom.py` & `odc_geo-0.4.4/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_gridspec.py` & `odc_geo-0.4.4/tests/test_gridspec.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_map.py` & `odc_geo-0.4.4/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_math.py` & `odc_geo-0.4.4/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_mpu.py` & `odc_geo-0.4.4/tests/test_mpu.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_mpu_fs.py` & `odc_geo-0.4.4/tests/test_mpu_fs.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_overlap.py` & `odc_geo-0.4.4/tests/test_overlap.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_rgba.py` & `odc_geo-0.4.4/tests/test_rgba.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_rioxarray_interop.py` & `odc_geo-0.4.4/tests/test_rioxarray_interop.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_roi.py` & `odc_geo-0.4.4/tests/test_roi.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_types.py` & `odc_geo-0.4.4/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_ui.py` & `odc_geo-0.4.4/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.3/tests/test_xr_interop.py` & `odc_geo-0.4.4/tests/test_xr_interop.py`

 * *Files 5% similar despite different names*

```diff
@@ -503,14 +503,33 @@
 
     bad_attr_coord = xx.spatial_ref.copy()
     bad_attr_coord.attrs["GeoTransform"] = bad_geo_transform
     assert _extract_geo_transform(bad_attr_coord) is None
 
 
 @pytest.mark.parametrize("geobox", TEST_GEOBOXES_SMALL_AXIS_ALIGNED)
+def test_reload(geobox):
+    xx = xr_zeros(geobox, dtype="int16")
+    assert xx.odc.geobox == geobox
+    assert xx.odc.reload() is xx
+    assert xx.odc.geobox == geobox
+
+    ds = xx.to_dataset(name="test")
+    assert ds.odc.geobox == geobox
+    assert ds.odc.reload() is ds
+    assert ds.odc.geobox == geobox
+
+    # change coords in-place
+    coord = xx[list(xx.coords)[0]]
+    coord.data[:] += 0.337
+    assert xx.odc.reload() is xx
+    assert xx.odc.geobox != geobox
+
+
+@pytest.mark.parametrize("geobox", TEST_GEOBOXES_SMALL_AXIS_ALIGNED)
 @pytest.mark.parametrize(
     "roi",
     [
         np.s_[:1, :1],
         np.s_[-1:, -1:],
         np.s_[1:2, 3:4],
         np.s_[1:2, :5],
```

