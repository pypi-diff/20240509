# Comparing `tmp/ecoscope-1.7.0.tar.gz` & `tmp/ecoscope-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoscope-1.7.0.tar", last modified: Tue Apr 16 09:39:52 2024, max compression
+gzip compressed data, was "ecoscope-1.7.1.tar", last modified: Thu May  9 09:59:22 2024, max compression
```

## Comparing `ecoscope-1.7.0.tar` & `ecoscope-1.7.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.831373 ecoscope-1.7.0/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2024-04-16 09:37:39.000000 ecoscope-1.7.0/LICENSE
--rw-r--r--   0 gitonga   (1000) gitonga   (1000)     4430 2024-04-16 09:39:52.831373 ecoscope-1.7.0/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2946 2024-04-16 09:37:39.000000 ecoscope-1.7.0/README.rst
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.819373 ecoscope-1.7.0/ecoscope/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3762 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/__init__.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.823373 ecoscope-1.7.0/ecoscope/analysis/
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.823373 ecoscope-1.7.0/ecoscope/analysis/UD/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/UD/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/UD/etd_range.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/astronomy.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3849 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/percentile.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/proximity.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4852 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2725 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/speed.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.823373 ecoscope-1.7.0/ecoscope/base/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/base/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/base/_dataclasses.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25126 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/base/base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7698 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/base/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.827373 ecoscope-1.7.0/ecoscope/contrib/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       61 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/contrib/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/contrib/basemaps.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   123902 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/contrib/foliumap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5197 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/contrib/geemap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2359 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/contrib/legend.txt
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.827373 ecoscope-1.7.0/ecoscope/io/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/io/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    37546 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/io/earthranger.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15218 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/io/eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6616 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/io/raster.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2652 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/io/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.827373 ecoscope-1.7.0/ecoscope/mapping/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      324 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/mapping/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    32305 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/mapping/map.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.827373 ecoscope-1.7.0/ecoscope/plotting/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      268 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/plotting/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7390 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/plotting/plot.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/version.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.831373 ecoscope-1.7.0/ecoscope.egg-info/
--rw-r--r--   0 gitonga   (1000) gitonga   (1000)     4430 2024-04-16 09:39:52.000000 ecoscope-1.7.0/ecoscope.egg-info/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1372 2024-04-16 09:39:52.000000 ecoscope-1.7.0/ecoscope.egg-info/SOURCES.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2024-04-16 09:39:52.000000 ecoscope-1.7.0/ecoscope.egg-info/dependency_links.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2024-04-16 09:39:52.000000 ecoscope-1.7.0/ecoscope.egg-info/not-zip-safe
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      277 2024-04-16 09:39:52.000000 ecoscope-1.7.0/ecoscope.egg-info/requires.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2024-04-16 09:39:52.000000 ecoscope-1.7.0/ecoscope.egg-info/top_level.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2024-04-16 09:37:39.000000 ecoscope-1.7.0/pyproject.toml
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2024-04-16 09:39:52.831373 ecoscope-1.7.0/setup.cfg
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1969 2024-04-16 09:37:39.000000 ecoscope-1.7.0/setup.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.831373 ecoscope-1.7.0/tests/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7044 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6694 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_earthranger_io.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_ecodataframe.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5198 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6126 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_ecomap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5933 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2492 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_io_utils.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      962 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_speed.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2091 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_ud.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      443 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.313376 ecoscope-1.7.1/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2024-05-09 09:56:48.000000 ecoscope-1.7.1/LICENSE
+-rw-r--r--   0 gitonga   (1000) gitonga   (1000)     4438 2024-05-09 09:59:22.313376 ecoscope-1.7.1/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2946 2024-05-09 09:56:48.000000 ecoscope-1.7.1/README.rst
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.305375 ecoscope-1.7.1/ecoscope/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3762 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/__init__.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.305375 ecoscope-1.7.1/ecoscope/analysis/
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.305375 ecoscope-1.7.1/ecoscope/analysis/UD/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/UD/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/UD/etd_range.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/astronomy.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3849 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/percentile.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/proximity.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4852 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2725 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/analysis/speed.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.309376 ecoscope-1.7.1/ecoscope/base/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/base/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/base/_dataclasses.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25126 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/base/base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7698 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/base/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.309376 ecoscope-1.7.1/ecoscope/contrib/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       61 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/contrib/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/contrib/basemaps.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   123902 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/contrib/foliumap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5197 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/contrib/geemap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2359 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/contrib/legend.txt
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.309376 ecoscope-1.7.1/ecoscope/io/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/io/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    39308 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/io/earthranger.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15220 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/io/eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6616 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/io/raster.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2652 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/io/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.309376 ecoscope-1.7.1/ecoscope/mapping/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      324 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/mapping/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    32305 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/mapping/map.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.309376 ecoscope-1.7.1/ecoscope/plotting/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      268 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/plotting/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7390 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/plotting/plot.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2024-05-09 09:56:48.000000 ecoscope-1.7.1/ecoscope/version.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.313376 ecoscope-1.7.1/ecoscope.egg-info/
+-rw-r--r--   0 gitonga   (1000) gitonga   (1000)     4438 2024-05-09 09:59:22.000000 ecoscope-1.7.1/ecoscope.egg-info/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1372 2024-05-09 09:59:22.000000 ecoscope-1.7.1/ecoscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2024-05-09 09:59:22.000000 ecoscope-1.7.1/ecoscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2024-05-09 09:59:22.000000 ecoscope-1.7.1/ecoscope.egg-info/not-zip-safe
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2024-05-09 09:59:22.000000 ecoscope-1.7.1/ecoscope.egg-info/requires.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2024-05-09 09:59:22.000000 ecoscope-1.7.1/ecoscope.egg-info/top_level.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2024-05-09 09:56:48.000000 ecoscope-1.7.1/pyproject.toml
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2024-05-09 09:59:22.313376 ecoscope-1.7.1/setup.cfg
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1977 2024-05-09 09:56:48.000000 ecoscope-1.7.1/setup.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-05-09 09:59:22.313376 ecoscope-1.7.1/tests/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7084 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7182 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_earthranger_io.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_ecodataframe.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5198 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6126 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_ecomap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5933 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2492 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_io_utils.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      962 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_speed.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2091 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_ud.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      443 2024-05-09 09:56:48.000000 ecoscope-1.7.1/tests/test_utils.py
```

### Comparing `ecoscope-1.7.0/LICENSE` & `ecoscope-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/PKG-INFO` & `ecoscope-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.7.0
+Version: 1.7.1
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
@@ -21,15 +21,15 @@
 Requires-Dist: affine
 Requires-Dist: astroplan
 Requires-Dist: backoff
 Requires-Dist: datashader
 Requires-Dist: earthengine-api
 Requires-Dist: earthranger-client
 Requires-Dist: folium
-Requires-Dist: geopandas
+Requires-Dist: geopandas<=0.14.2
 Requires-Dist: igraph
 Requires-Dist: kaleido
 Requires-Dist: mapclassify
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: numba
 Requires-Dist: plotly
```

### Comparing `ecoscope-1.7.0/README.rst` & `ecoscope-1.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/__init__.py` & `ecoscope-1.7.1/ecoscope/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/analysis/UD/etd_range.py` & `ecoscope-1.7.1/ecoscope/analysis/UD/etd_range.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/analysis/astronomy.py` & `ecoscope-1.7.1/ecoscope/analysis/astronomy.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/analysis/ecograph.py` & `ecoscope-1.7.1/ecoscope/analysis/ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/analysis/geofence.py` & `ecoscope-1.7.1/ecoscope/analysis/geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/analysis/immobility.py` & `ecoscope-1.7.1/ecoscope/analysis/immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/analysis/percentile.py` & `ecoscope-1.7.1/ecoscope/analysis/percentile.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/analysis/proximity.py` & `ecoscope-1.7.1/ecoscope/analysis/proximity.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/analysis/seasons.py` & `ecoscope-1.7.1/ecoscope/analysis/seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/analysis/speed.py` & `ecoscope-1.7.1/ecoscope/analysis/speed.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/base/__init__.py` & `ecoscope-1.7.1/ecoscope/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/base/_dataclasses.py` & `ecoscope-1.7.1/ecoscope/base/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/base/base.py` & `ecoscope-1.7.1/ecoscope/base/base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/base/utils.py` & `ecoscope-1.7.1/ecoscope/base/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/contrib/basemaps.py` & `ecoscope-1.7.1/ecoscope/contrib/basemaps.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/contrib/foliumap.py` & `ecoscope-1.7.1/ecoscope/contrib/foliumap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/contrib/geemap.py` & `ecoscope-1.7.1/ecoscope/contrib/geemap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/contrib/legend.txt` & `ecoscope-1.7.1/ecoscope/contrib/legend.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/io/earthranger.py` & `ecoscope-1.7.1/ecoscope/io/earthranger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import datetime
 import pytz
 import json
 import typing
+import math
 
+import numpy as np
 import geopandas as gpd
 import pandas as pd
 import requests
+from dateutil import parser
 from erclient.client import ERClient, ERClientException, ERClientNotFound
 from tqdm.auto import tqdm
 
 import ecoscope
 from ecoscope.io.utils import pack_columns, to_hex
 
 
@@ -118,52 +121,55 @@
         assert not df.empty
         return df
 
     def get_subjects(
         self,
         include_inactive=None,
         bbox=None,
-        subject_group=None,
+        subject_group_id=None,
         name=None,
         updated_since=None,
         tracks=None,
         id=None,
         updated_until=None,
-        group_name=None,
+        subject_group_name=None,
+        max_ids_per_request=50,
         **addl_kwargs,
     ):
         """
         Parameters
         ----------
         include_inactive: Include inactive subjects in list.
         bbox: Include subjects having track data within this bounding box defined by a 4-tuple of coordinates marking
             west, south, east, north.
-        subject_group: Indicate a subject group for which Subjects should be listed.
+        subject_group_id: Indicate a subject group id for which Subjects should be listed.
+            This is translated to the subject_group parameter in the ER backend
         name : Find subjects with the given name
         updated_since: Return Subject that have been updated since the given timestamp.
         tracks: Indicate whether to render each subject's recent tracks.
         id: A comma-delimited list of Subject IDs.
         updated_until
-        group_name
+        subject_group_name: A subject group name for which Subjects should be listed.
+            This is translated to the group_name parameter in the ER backend
         Returns
         -------
         subjects : pd.DataFrame
         """
 
         params = self._clean_kwargs(
             addl_kwargs,
             include_inactive=include_inactive,
             bbox=bbox,
-            subject_group=subject_group,
+            subject_group=subject_group_id,
             name=name,
             updated_since=updated_since,
             tracks=tracks,
             id=id,
             updated_until=updated_until,
-            group_name=group_name,
+            group_name=subject_group_name,
         )
 
         assert params.get("subject_group") is None or params.get("group_name") is None
 
         if params.get("group_name") is not None:
             try:
                 params["subject_group"] = self._get(
@@ -174,19 +180,40 @@
                         "include_hidden": True,
                         "flat": True,
                     },
                 )[0]["id"]
             except IndexError:
                 raise KeyError("`group_name` not found")
 
-        df = pd.DataFrame(
-            self.get_objects_multithreaded(
-                object="subjects/", threads=self.tcp_limit, page_size=self.sub_page_size, **params
+        if params.get("id") is not None:
+            params["id"] = params.get("id").split(",")
+
+            def partial_subjects(subjects):
+                params["id"] = ",".join(subjects)
+                return pd.DataFrame(
+                    self.get_objects_multithreaded(
+                        object="subjects/", threads=self.tcp_limit, page_size=self.sub_page_size, **params
+                    )
+                )
+
+            df = pd.concat(
+                [
+                    partial_subjects(s)
+                    for s in np.array_split(params["id"], math.ceil(len(params["id"]) / max_ids_per_request))
+                ],
+                ignore_index=True,
             )
-        )
+
+        else:
+            df = pd.DataFrame(
+                self.get_objects_multithreaded(
+                    object="subjects/", threads=self.tcp_limit, page_size=self.sub_page_size, **params
+                )
+            )
+
         assert not df.empty
 
         df["hex"] = df["additional"].str["rgb"].map(to_hex) if "additional" in df else "#ff0000"
 
         return df
 
     def get_subjectsources(self, subjects=None, sources=None, **addl_kwargs):
@@ -346,16 +373,16 @@
         relocations=True,
         **kwargs,
     ):
         """
         Get observations for each listed subject and create a `Relocations` object.
         Parameters
         ----------
-        subject_ids : str or list[str]
-            List of subject UUIDs
+        subject_ids : str or list[str] or pd.DataFrame
+            List of subject UUIDs, or a DataFrame of subjects
         include_source_details : bool, optional
             Whether to merge source info into dataframe
         include_subject_details : bool, optional
             Whether to merge subject info into dataframe
         include_subjectsource_details : bool, optional
             Whether to merge subjectsource info into dataframe
         kwargs
@@ -365,32 +392,43 @@
         -------
         relocations : ecoscope.base.Relocations
             Observations in `Relocations` format
         """
 
         if isinstance(subject_ids, str):
             subject_ids = [subject_ids]
+        elif isinstance(subject_ids, pd.DataFrame):
+            subject_ids = subject_ids.id.tolist()
+        elif not isinstance(subject_ids, list):
+            raise ValueError(f"subject_ids must be either a str or list[str] or pd.DataFrame, not {type(subject_ids)}")
 
         observations = self._get_observations(subject_ids=subject_ids, **kwargs)
 
         if observations.empty:
             return gpd.GeoDataFrame()
 
         if include_source_details:
             observations = observations.merge(
                 self.get_sources(id=",".join(observations["source"].unique())).add_prefix("source__"),
                 left_on="source",
                 right_on="source__id",
             )
         if include_subject_details:
-            observations = observations.merge(
-                self.get_subjects(id=",".join(subject_ids), include_inactive=True).add_prefix("subject__"),
-                left_on="subject_id",
-                right_on="subject__id",
-            )
+            if isinstance(subject_ids, pd.DataFrame):
+                observations = observations.merge(
+                    subject_ids.add_prefix("subject__"),
+                    left_on="subject_id",
+                    right_on="subject__id",
+                )
+            else:
+                observations = observations.merge(
+                    self.get_subjects(id=",".join(subject_ids), include_inactive=True).add_prefix("subject__"),
+                    left_on="subject_id",
+                    right_on="subject__id",
+                )
 
         if include_subjectsource_details:
             observations = observations.merge(
                 self.get_subjectsources(subjects=",".join(observations["subject_id"].unique())).add_prefix(
                     "subjectsource__"
                 ),
                 left_on=["subject_id", "source"],
@@ -452,41 +490,43 @@
                 groupby_col="subjectsource_id",
                 uuid_col="id",
                 time_col="recorded_at",
             )
         else:
             return observations
 
-    def get_subjectgroup_observations(self, subject_group=None, group_name=None, include_inactive=True, **kwargs):
+    def get_subjectgroup_observations(
+        self, subject_group_id=None, subject_group_name=None, include_inactive=True, **kwargs
+    ):
         """
         Parameters
         ----------
-        subject_group : str
+        subject_group_id : str
             UUID of subject group to filter by
-        group_name : str
+        subject_group_name : str
             Common name of subject group to filter by
         include_inactive : bool, optional
             Whether to get observations for Subjects marked inactive by EarthRanger
         kwargs
             Additional arguments to pass in the request to `get_subject_observations`. See the docstring of
             `get_subject_observations` for info.
         Returns
         -------
         relocations : ecoscope.base.Relocations
             Observations in `Relocations` format
         """
 
-        assert (subject_group is None) != (group_name is None)
+        assert (subject_group_id is None) != (subject_group_name is None)
 
-        if subject_group:
-            subject_ids = self.get_subjects(subject_group=subject_group, include_inactive=include_inactive).id.tolist()
+        if subject_group_id:
+            subjects = self.get_subjects(subject_group_id=subject_group_id, include_inactive=include_inactive)
         else:
-            subject_ids = self.get_subjects(group_name=group_name, include_inactive=include_inactive).id.tolist()
+            subjects = self.get_subjects(subject_group_name=subject_group_name, include_inactive=include_inactive)
 
-        return self.get_subject_observations(subject_ids, **kwargs)
+        return self.get_subject_observations(subjects, **kwargs)
 
     def get_event_types(self, include_inactive=False, **addl_kwargs):
         params = self._clean_kwargs(addl_kwargs, include_inactive=include_inactive)
 
         return pd.DataFrame(self._get("activity/events/eventtypes", **params))
 
     def get_events(
@@ -589,15 +629,16 @@
         df = pd.DataFrame(
             self.get_objects_multithreaded(
                 object="activity/events/", threads=self.tcp_limit, page_size=self.sub_page_size, **params
             )
         )
 
         assert not df.empty
-        df["time"] = pd.to_datetime(df["time"])
+
+        df["time"] = df["time"].apply(lambda x: pd.to_datetime(parser.parse(x)))
 
         gdf = gpd.GeoDataFrame(df)
         if gdf.loc[0, "location"] is not None:
             gdf.loc[~gdf["geojson"].isna(), "geometry"] = gpd.GeoDataFrame.from_features(
                 gdf.loc[~gdf["geojson"].isna(), "geojson"]
             )["geometry"]
             gdf.set_crs(4326, inplace=True)
```

### Comparing `ecoscope-1.7.0/ecoscope/io/eetools.py` & `ecoscope-1.7.1/ecoscope/io/eetools.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         raise ValueError("n_before and n_after must be 0 or greater")
     img_data = img_coll.reduceColumns(ee.Reducer.toList(2), ["system:index", "system:time_start"]).get("list").getInfo()
     img_data = np.array(img_data)
     img_data = (
         pd.DataFrame(
             {
                 "img_id": img_data[:, 0],
-                "img_date": pd.to_datetime(img_data[:, 1].astype("int"), unit="ms").tz_localize("UTC"),
+                "img_date": pd.to_datetime(img_data[:, 1].astype("int64"), unit="ms").tz_localize("UTC"),
             }
         )
         .sort_values("img_date")
         .set_index("img_date")
     )
 
     # Step 2: determine the closest image IDs to a given feature date
```

### Comparing `ecoscope-1.7.0/ecoscope/io/raster.py` & `ecoscope-1.7.1/ecoscope/io/raster.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/io/utils.py` & `ecoscope-1.7.1/ecoscope/io/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/mapping/map.py` & `ecoscope-1.7.1/ecoscope/mapping/map.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope/plotting/plot.py` & `ecoscope-1.7.1/ecoscope/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/ecoscope.egg-info/PKG-INFO` & `ecoscope-1.7.1/ecoscope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.7.0
+Version: 1.7.1
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
@@ -21,15 +21,15 @@
 Requires-Dist: affine
 Requires-Dist: astroplan
 Requires-Dist: backoff
 Requires-Dist: datashader
 Requires-Dist: earthengine-api
 Requires-Dist: earthranger-client
 Requires-Dist: folium
-Requires-Dist: geopandas
+Requires-Dist: geopandas<=0.14.2
 Requires-Dist: igraph
 Requires-Dist: kaleido
 Requires-Dist: mapclassify
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: numba
 Requires-Dist: plotly
```

### Comparing `ecoscope-1.7.0/ecoscope.egg-info/SOURCES.txt` & `ecoscope-1.7.1/ecoscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/pyproject.toml` & `ecoscope-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/setup.py` & `ecoscope-1.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "affine",
     "astroplan",
     "backoff",
     "datashader",
     "earthengine-api",
     "earthranger-client",
     "folium",
-    "geopandas",
+    "geopandas<=0.14.2",
     "igraph",
     "kaleido",
     "mapclassify",
     "matplotlib",
     "networkx",
     "numba",
     "plotly",
```

### Comparing `ecoscope-1.7.0/tests/test_base.py` & `ecoscope-1.7.1/tests/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,50 +7,50 @@
 
 import ecoscope
 
 
 @pytest.mark.skipif(not pytest.earthranger, reason="No connection to EarthRanger")
 def test_trajectory_is_not_empty(er_io):
     # test there is actually data in trajectory
-    relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
+    relocations = er_io.get_subjectgroup_observations(subject_group_name=er_io.GROUP_NAME)
     trajectory = ecoscope.base.Trajectory.from_relocations(relocations)
     assert not trajectory.empty
 
 
 @pytest.mark.skipif(not pytest.earthranger, reason="No connection to EarthRanger")
 def test_redundant_columns_in_trajectory(er_io):
     # test there is no redundant column in trajectory
-    relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
+    relocations = er_io.get_subjectgroup_observations(subject_group_name=er_io.GROUP_NAME)
     trajectory = ecoscope.base.Trajectory.from_relocations(relocations)
     assert "extra__fixtime" not in trajectory
     assert "extra___fixtime" not in trajectory
     assert "extra___geometry" not in trajectory
 
 
 @pytest.mark.skipif(not pytest.earthranger, reason="No connection to EarthRanger")
 def test_relocs_speedfilter(er_io):
-    relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
+    relocations = er_io.get_subjectgroup_observations(subject_group_name=er_io.GROUP_NAME)
     relocs_speed_filter = ecoscope.base.RelocsSpeedFilter(max_speed_kmhr=8)
     relocs_after_filter = relocations.apply_reloc_filter(relocs_speed_filter)
     relocs_after_filter.remove_filtered(inplace=True)
     assert relocations.shape[0] != relocs_after_filter.shape[0]
 
 
 @pytest.mark.skipif(not pytest.earthranger, reason="No connection to EarthRanger")
 def test_relocs_distancefilter(er_io):
-    relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
+    relocations = er_io.get_subjectgroup_observations(subject_group_name=er_io.GROUP_NAME)
     relocs_speed_filter = ecoscope.base.RelocsDistFilter(min_dist_km=1.0, max_dist_km=6.0)
     relocs_after_filter = relocations.apply_reloc_filter(relocs_speed_filter)
     relocs_after_filter.remove_filtered(inplace=True)
     assert relocations.shape[0] != relocs_after_filter.shape[0]
 
 
 @pytest.mark.skipif(not pytest.earthranger, reason="No connection to EarthRanger")
 def test_relocations_from_gdf_preserve_fields(er_io):
-    relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
+    relocations = er_io.get_subjectgroup_observations(subject_group_name=er_io.GROUP_NAME)
     gpd.testing.assert_geodataframe_equal(relocations, ecoscope.base.Relocations.from_gdf(relocations))
 
 
 def test_displacement_property(movbank_relocations):
     trajectory = ecoscope.base.Trajectory.from_relocations(movbank_relocations)
     expected = pd.Series(
         [2633.760505, 147749.545621],
```

### Comparing `ecoscope-1.7.0/tests/test_earthranger_io.py` & `ecoscope-1.7.1/tests/test_earthranger_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,16 +62,17 @@
         subjectsource_ids=str(uuid.uuid4()),
         include_source_details=True,
     )
     assert relocations.empty
 
 
 def test_get_subjectgroup_observations(er_io):
-    relocations = er_io.get_subjectgroup_observations(group_name=er_io.GROUP_NAME)
+    relocations = er_io.get_subjectgroup_observations(subject_group_name=er_io.GROUP_NAME)
     assert "groupby_col" in relocations
+    assert len(relocations["extra__subject_id"].unique()) == 2
 
 
 def test_get_events(er_events_io):
     events = er_events_io.get_events(event_type=["e00ce1f6-f9f1-48af-93c9-fb89ec493b8a"])
     assert not events.empty
 
 
@@ -186,14 +187,15 @@
     )
 
     result = er_io.patch_event(event_id=event_id, events=updated_event)
     result = result[["priority", "state", "location"]]
     pd.testing.assert_frame_equal(result, updated_event)
 
 
+@pytest.mark.skip(reason="Known issue: https://github.com/wildlife-dynamics/ecoscope/issues/109")
 def test_get_patrol_observations(er_io):
     patrols = er_io.get_patrols()
     observations = er_io.get_patrol_observations(
         patrols,
         include_source_details=False,
         include_subject_details=False,
         include_subjectsource_details=False,
@@ -212,7 +214,15 @@
 
 
 def test_get_spatial_features_group(er_io):
     spatial_features = er_io.get_spatial_features_group(
         spatial_features_group_id="15698426-7e0f-41df-9bc3-495d87e2e097"
     )
     assert not spatial_features.empty
+
+
+def test_get_subjects_chunking(er_io):
+    subject_ids = ",".join(er_io.SUBJECT_IDS)
+    single_request_result = er_io.get_subjects(id=subject_ids)
+    chunked_request_result = er_io.get_subjects(id=subject_ids, max_ids_per_request=1)
+
+    pd.testing.assert_frame_equal(single_request_result, chunked_request_result)
```

### Comparing `ecoscope-1.7.0/tests/test_ecodataframe.py` & `ecoscope-1.7.1/tests/test_ecodataframe.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/tests/test_ecograph.py` & `ecoscope-1.7.1/tests/test_ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/tests/test_ecomap.py` & `ecoscope-1.7.1/tests/test_ecomap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/tests/test_eetools.py` & `ecoscope-1.7.1/tests/test_eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/tests/test_geofence.py` & `ecoscope-1.7.1/tests/test_geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/tests/test_immobility.py` & `ecoscope-1.7.1/tests/test_immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/tests/test_io_utils.py` & `ecoscope-1.7.1/tests/test_io_utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/tests/test_seasons.py` & `ecoscope-1.7.1/tests/test_seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.7.0/tests/test_ud.py` & `ecoscope-1.7.1/tests/test_ud.py`

 * *Files identical despite different names*

