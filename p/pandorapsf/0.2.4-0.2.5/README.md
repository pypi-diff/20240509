# Comparing `tmp/pandorapsf-0.2.4.tar.gz` & `tmp/pandorapsf-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandorapsf-0.2.4.tar", max compression
+gzip compressed data, was "pandorapsf-0.2.5.tar", max compression
```

## Comparing `pandorapsf-0.2.4.tar` & `pandorapsf-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1071 2023-09-22 21:06:08.416872 pandorapsf-0.2.4/LICENSE
--rw-r--r--   0        0        0       15 2023-09-21 17:07:25.661702 pandorapsf-0.2.4/README.md
--rw-r--r--   0        0        0      363 2024-05-09 14:42:49.751935 pandorapsf-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1734 2024-05-09 14:42:53.261321 pandorapsf-0.2.4/src/pandorapsf/__init__.py
--rw-r--r--   0        0        0    14579 2023-10-11 00:00:22.516507 pandorapsf-0.2.4/src/pandorapsf/data/dichroic-transmission.csv
--rw-r--r--   0        0        0   100800 2024-05-03 14:35:17.450737 pandorapsf-0.2.4/src/pandorapsf/data/nirda-wav-solution.fits
--rw-r--r--   0        0        0     2777 2023-09-21 16:57:33.816212 pandorapsf-0.2.4/src/pandorapsf/data/pandora.mplstyle
--rw-r--r--   0        0        0     6452 2023-10-10 23:55:05.530892 pandorapsf-0.2.4/src/pandorapsf/data/pandora_visible_qe.csv
--rw-r--r--   0        0        0    25577 2023-09-22 16:23:38.985186 pandorapsf-0.2.4/src/pandorapsf/data/pixel_vs_wavelength.csv
--rw-r--r--   0        0        0    14400 2024-05-03 14:35:17.463147 pandorapsf-0.2.4/src/pandorapsf/data/visda-wav-solution.fits
--rw-r--r--   0        0        0     7461 2024-05-08 14:32:10.310103 pandorapsf-0.2.4/src/pandorapsf/plotting.py
--rw-r--r--   0        0        0    29360 2024-05-08 19:13:45.641761 pandorapsf-0.2.4/src/pandorapsf/psf.py
--rw-r--r--   0        0        0    30154 2024-05-08 15:43:00.159415 pandorapsf-0.2.4/src/pandorapsf/scene.py
--rw-r--r--   0        0        0     8506 2024-05-08 19:29:04.935549 pandorapsf-0.2.4/src/pandorapsf/sparsewarp.py
--rw-r--r--   0        0        0    22754 2024-05-08 19:05:42.377580 pandorapsf-0.2.4/src/pandorapsf/utils.py
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 pandorapsf-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-09-22 21:06:08.416872 pandorapsf-0.2.5/LICENSE
+-rw-r--r--   0        0        0       15 2023-09-21 17:07:25.661702 pandorapsf-0.2.5/README.md
+-rw-r--r--   0        0        0      363 2024-05-09 15:46:39.793117 pandorapsf-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1734 2024-05-09 15:29:00.839309 pandorapsf-0.2.5/src/pandorapsf/__init__.py
+-rw-r--r--   0        0        0    14579 2023-10-11 00:00:22.516507 pandorapsf-0.2.5/src/pandorapsf/data/dichroic-transmission.csv
+-rw-r--r--   0        0        0   100800 2024-05-03 14:35:17.450737 pandorapsf-0.2.5/src/pandorapsf/data/nirda-wav-solution.fits
+-rw-r--r--   0        0        0     2777 2023-09-21 16:57:33.816212 pandorapsf-0.2.5/src/pandorapsf/data/pandora.mplstyle
+-rw-r--r--   0        0        0     6452 2023-10-10 23:55:05.530892 pandorapsf-0.2.5/src/pandorapsf/data/pandora_visible_qe.csv
+-rw-r--r--   0        0        0    25577 2023-09-22 16:23:38.985186 pandorapsf-0.2.5/src/pandorapsf/data/pixel_vs_wavelength.csv
+-rw-r--r--   0        0        0    14400 2024-05-03 14:35:17.463147 pandorapsf-0.2.5/src/pandorapsf/data/visda-wav-solution.fits
+-rw-r--r--   0        0        0     7461 2024-05-08 14:32:10.310103 pandorapsf-0.2.5/src/pandorapsf/plotting.py
+-rw-r--r--   0        0        0    29360 2024-05-09 15:29:04.711409 pandorapsf-0.2.5/src/pandorapsf/psf.py
+-rw-r--r--   0        0        0    30154 2024-05-08 15:43:00.159415 pandorapsf-0.2.5/src/pandorapsf/scene.py
+-rw-r--r--   0        0        0     8506 2024-05-08 19:29:04.935549 pandorapsf-0.2.5/src/pandorapsf/sparsewarp.py
+-rw-r--r--   0        0        0    22754 2024-05-08 19:05:42.377580 pandorapsf-0.2.5/src/pandorapsf/utils.py
+-rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 pandorapsf-0.2.5/PKG-INFO
```

### Comparing `pandorapsf-0.2.4/LICENSE` & `pandorapsf-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.4/src/pandorapsf/__init__.py` & `pandorapsf-0.2.5/src/pandorapsf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 # Standard library
 import os  # noqa
 
 PACKAGEDIR = os.path.abspath(os.path.dirname(__file__))
 TESTDIR = "/".join(PACKAGEDIR.split("/")[:-2]) + "/tests/"
 PANDORASTYLE = "{}/data/pandora.mplstyle".format(PACKAGEDIR)
```

### Comparing `pandorapsf-0.2.4/src/pandorapsf/data/dichroic-transmission.csv` & `pandorapsf-0.2.5/src/pandorapsf/data/dichroic-transmission.csv`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.4/src/pandorapsf/data/nirda-wav-solution.fits` & `pandorapsf-0.2.5/src/pandorapsf/data/nirda-wav-solution.fits`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.4/src/pandorapsf/data/pandora.mplstyle` & `pandorapsf-0.2.5/src/pandorapsf/data/pandora.mplstyle`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.4/src/pandorapsf/data/pandora_visible_qe.csv` & `pandorapsf-0.2.5/src/pandorapsf/data/pandora_visible_qe.csv`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.4/src/pandorapsf/data/pixel_vs_wavelength.csv` & `pandorapsf-0.2.5/src/pandorapsf/data/pixel_vs_wavelength.csv`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.4/src/pandorapsf/data/visda-wav-solution.fits` & `pandorapsf-0.2.5/src/pandorapsf/data/visda-wav-solution.fits`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.4/src/pandorapsf/plotting.py` & `pandorapsf-0.2.5/src/pandorapsf/plotting.py`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.4/src/pandorapsf/psf.py` & `pandorapsf-0.2.5/src/pandorapsf/psf.py`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.4/src/pandorapsf/scene.py` & `pandorapsf-0.2.5/src/pandorapsf/scene.py`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.4/src/pandorapsf/sparsewarp.py` & `pandorapsf-0.2.5/src/pandorapsf/sparsewarp.py`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.4/src/pandorapsf/utils.py` & `pandorapsf-0.2.5/src/pandorapsf/utils.py`

 * *Files identical despite different names*

