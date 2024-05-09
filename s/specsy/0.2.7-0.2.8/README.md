# Comparing `tmp/specsy-0.2.7.tar.gz` & `tmp/specsy-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specsy-0.2.7.tar", last modified: Sat May  4 20:26:19 2024, max compression
+gzip compressed data, was "specsy-0.2.8.tar", last modified: Thu May  9 04:41:05 2024, max compression
```

## Comparing `specsy-0.2.7.tar` & `specsy-0.2.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:26:19.062732 specsy-0.2.7/
--rw-rw-r--   0 vital     (1000) vital     (1000)       17 2024-04-29 21:50:58.000000 specsy-0.2.7/MANIFEST.in
--rw-r--r--   0 vital     (1000) vital     (1000)     1864 2024-05-04 20:26:19.062732 specsy-0.2.7/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)      866 2024-04-29 21:50:58.000000 specsy-0.2.7/README.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)     1228 2024-05-04 20:25:14.000000 specsy-0.2.7/pyproject.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      431 2024-05-04 20:26:19.062732 specsy-0.2.7/setup.cfg
--rw-rw-r--   0 vital     (1000) vital     (1000)     1526 2024-05-04 20:05:09.000000 specsy-0.2.7/setup.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:26:19.058732 specsy-0.2.7/src/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:26:19.058732 specsy-0.2.7/src/specsy/
--rw-rw-r--   0 vital     (1000) vital     (1000)      927 2024-04-30 20:35:13.000000 specsy-0.2.7/src/specsy/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     5802 2024-05-04 20:25:14.000000 specsy-0.2.7/src/specsy/config.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      759 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/core.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:26:19.058732 specsy-0.2.7/src/specsy/inference/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/inference/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    16792 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/inference/emission.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:26:19.058732 specsy-0.2.7/src/specsy/innate/
--rw-rw-r--   0 vital     (1000) vital     (1000)       90 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/innate/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4246 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/innate/interpol_pytensor.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     3830 2024-05-03 19:46:25.000000 specsy-0.2.7/src/specsy/innate/main.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    12984 2024-05-04 20:23:50.000000 specsy-0.2.7/src/specsy/io.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:26:19.058732 specsy-0.2.7/src/specsy/models/
--rw-rw-r--   0 vital     (1000) vital     (1000)      243 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/models/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    17030 2024-05-03 21:54:50.000000 specsy-0.2.7/src/specsy/models/chemistry.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     6541 2024-05-03 21:52:49.000000 specsy-0.2.7/src/specsy/models/chemistry_inference.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    17567 2024-05-04 20:17:50.000000 specsy-0.2.7/src/specsy/models/emissivity.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    22659 2024-05-04 19:52:53.000000 specsy-0.2.7/src/specsy/models/extinction.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/models/fluxes_line.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     8332 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/models/nebular_continuum.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:26:19.058732 specsy-0.2.7/src/specsy/operations/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/operations/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    10770 2024-05-04 20:17:50.000000 specsy-0.2.7/src/specsy/operations/interpolation.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/operations/pytensors.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4631 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/operations/tensors.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     1329 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/operations/tests.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    16155 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/plots.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:26:19.062732 specsy-0.2.7/src/specsy/resources/
--rw-rw-r--   0 vital     (1000) vital     (1000)      419 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/resources/Benjamin1999_OpticalDepthFunctionCoefficients.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    21375 2024-04-29 21:50:58.000000 specsy-0.2.7/src/specsy/resources/HI_t3_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)    44530 2024-04-29 21:50:59.000000 specsy-0.2.7/src/specsy/resources/HeII_t4_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)   326042 2024-04-29 21:50:59.000000 specsy-0.2.7/src/specsy/resources/HeI_t5_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)      451 2024-04-29 21:50:59.000000 specsy-0.2.7/src/specsy/resources/gordon_2003_LMC2_supershell.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      476 2024-04-29 21:50:59.000000 specsy-0.2.7/src/specsy/resources/gordon_2003_LMC_average.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      483 2024-04-29 21:50:59.000000 specsy-0.2.7/src/specsy/resources/gordon_2003_SMC_bar.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)     2887 2024-04-29 21:50:59.000000 specsy-0.2.7/src/specsy/tools.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    10298 2024-05-04 20:18:12.000000 specsy-0.2.7/src/specsy/treatement.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:26:19.062732 specsy-0.2.7/src/specsy/workflow/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:59.000000 specsy-0.2.7/src/specsy/workflow/__init__.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:26:19.058732 specsy-0.2.7/src/specsy.egg-info/
--rw-r--r--   0 vital     (1000) vital     (1000)     1864 2024-05-04 20:26:19.000000 specsy-0.2.7/src/specsy.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     1310 2024-05-04 20:26:19.000000 specsy-0.2.7/src/specsy.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-04 20:26:19.000000 specsy-0.2.7/src/specsy.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      266 2024-05-04 20:26:19.000000 specsy-0.2.7/src/specsy.egg-info/requires.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        7 2024-05-04 20:26:19.000000 specsy-0.2.7/src/specsy.egg-info/top_level.txt
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 04:41:05.159678 specsy-0.2.8/
+-rw-rw-r--   0 vital     (1000) vital     (1000)       17 2024-04-29 21:50:58.000000 specsy-0.2.8/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)     1864 2024-05-09 04:41:05.159678 specsy-0.2.8/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)      866 2024-04-29 21:50:58.000000 specsy-0.2.8/README.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1228 2024-05-09 04:40:37.000000 specsy-0.2.8/pyproject.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      431 2024-05-09 04:41:05.159678 specsy-0.2.8/setup.cfg
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1526 2024-05-04 20:05:09.000000 specsy-0.2.8/setup.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 04:41:05.155678 specsy-0.2.8/src/
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 04:41:05.155678 specsy-0.2.8/src/specsy/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      927 2024-04-30 20:35:13.000000 specsy-0.2.8/src/specsy/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     5802 2024-05-09 04:40:37.000000 specsy-0.2.8/src/specsy/config.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      759 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/core.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 04:41:05.159678 specsy-0.2.8/src/specsy/inference/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/inference/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16792 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/inference/emission.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 04:41:05.159678 specsy-0.2.8/src/specsy/innate/
+-rw-rw-r--   0 vital     (1000) vital     (1000)       90 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/innate/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4246 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/innate/interpol_pytensor.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3957 2024-05-08 19:27:05.000000 specsy-0.2.8/src/specsy/innate/main.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    13101 2024-05-09 04:31:47.000000 specsy-0.2.8/src/specsy/io.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 04:41:05.159678 specsy-0.2.8/src/specsy/models/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      243 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/models/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    19309 2024-05-09 02:59:45.000000 specsy-0.2.8/src/specsy/models/chemistry.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     6541 2024-05-03 21:52:49.000000 specsy-0.2.8/src/specsy/models/chemistry_inference.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17567 2024-05-04 20:17:50.000000 specsy-0.2.8/src/specsy/models/emissivity.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    22659 2024-05-04 19:52:53.000000 specsy-0.2.8/src/specsy/models/extinction.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/models/fluxes_line.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     8332 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/models/nebular_continuum.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 04:41:05.159678 specsy-0.2.8/src/specsy/operations/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/operations/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10770 2024-05-04 20:17:50.000000 specsy-0.2.8/src/specsy/operations/interpolation.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/operations/pytensors.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4631 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/operations/tensors.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1329 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/operations/tests.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16399 2024-05-09 04:24:29.000000 specsy-0.2.8/src/specsy/plots.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 04:41:05.159678 specsy-0.2.8/src/specsy/resources/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      419 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/resources/Benjamin1999_OpticalDepthFunctionCoefficients.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    21375 2024-04-29 21:50:58.000000 specsy-0.2.8/src/specsy/resources/HI_t3_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)    44530 2024-04-29 21:50:59.000000 specsy-0.2.8/src/specsy/resources/HeII_t4_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)   326042 2024-04-29 21:50:59.000000 specsy-0.2.8/src/specsy/resources/HeI_t5_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)      451 2024-04-29 21:50:59.000000 specsy-0.2.8/src/specsy/resources/gordon_2003_LMC2_supershell.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      476 2024-04-29 21:50:59.000000 specsy-0.2.8/src/specsy/resources/gordon_2003_LMC_average.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      483 2024-04-29 21:50:59.000000 specsy-0.2.8/src/specsy/resources/gordon_2003_SMC_bar.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2887 2024-04-29 21:50:59.000000 specsy-0.2.8/src/specsy/tools.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10298 2024-05-04 20:18:12.000000 specsy-0.2.8/src/specsy/treatement.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 04:41:05.159678 specsy-0.2.8/src/specsy/workflow/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:59.000000 specsy-0.2.8/src/specsy/workflow/__init__.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 04:41:05.155678 specsy-0.2.8/src/specsy.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)     1864 2024-05-09 04:41:05.000000 specsy-0.2.8/src/specsy.egg-info/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1310 2024-05-09 04:41:05.000000 specsy-0.2.8/src/specsy.egg-info/SOURCES.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-09 04:41:05.000000 specsy-0.2.8/src/specsy.egg-info/dependency_links.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      266 2024-05-09 04:41:05.000000 specsy-0.2.8/src/specsy.egg-info/requires.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        7 2024-05-09 04:41:05.000000 specsy-0.2.8/src/specsy.egg-info/top_level.txt
```

### Comparing `specsy-0.2.7/PKG-INFO` & `specsy-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsy
-Version: 0.2.7
+Version: 0.2.8
 Summary: Model fitting package for the chemical analysis of astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/specsy
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `specsy-0.2.7/README.rst` & `specsy-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/pyproject.toml` & `specsy-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "specsy"
-version = "0.2.7"
+version = "0.2.8"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "COPYING"}
 authors = [{name = "Vital Fernández", email = "vgf@umich.edu"}]
 description = "Model fitting package for the chemical analysis of astronomical spectra"
 dependencies = ["arviz~=0.18",
                 "astropy~=6.0",
```

### Comparing `specsy-0.2.7/setup.py` & `specsy-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/__init__.py` & `specsy-0.2.8/src/specsy/__init__.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/config.toml` & `specsy-0.2.8/src/specsy/config.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = 'specsy'
-version = '0.2.7'
+version = '0.2.8'
 
 [direct_method_cfg]
 temp_zones.high = ["He1", "He2", "O3", "Ar4", "Ne3", "Cl4", "C3"]
 temp_zones.low  = ["H1", "Ar3", "S2", "S3", "N2", "O2", "Fe3", "C2"]
 parameter_list = ["n_e", "T_low", "T_high", "cHbeta", "tau", "Ar3", "Ar4", "N2", "O2", "O3", "S2", "S3", "He1", "He2",
                   "Cl3","Ne3","Fe3","Teff","logU"]
 temp_low_diag = ['S3_6312A']
```

### Comparing `specsy-0.2.7/src/specsy/core.py` & `specsy-0.2.8/src/specsy/core.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/inference/emission.py` & `specsy-0.2.8/src/specsy/inference/emission.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/innate/interpol_pytensor.py` & `specsy-0.2.8/src/specsy/innate/interpol_pytensor.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/innate/main.py` & `specsy-0.2.8/src/specsy/innate/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import numpy as np
 from astropy.io import fits
 from pathlib import Path
 from warnings import catch_warnings, simplefilter
 from arviz import to_netcdf, from_netcdf
 from xarray import Dataset
+from os import PathLike
 from .interpol_pytensor import interpolation_selection
 import h5netcdf
 
 
 def load_inference_data(fname):
 
     # Load the data
-    with catch_warnings():
-        simplefilter("ignore", UserWarning)
-        inference_data = from_netcdf(fname)
+    if isinstance(fname, (str, PathLike, bytes)):
+        with catch_warnings():
+            simplefilter("ignore", UserWarning)
+            inference_data = from_netcdf(fname)
+    else:
+        inference_data = fname
 
     return inference_data
 
 
 def save_inference_data(fname, inference_data, **kwargs):
 
     if kwargs is not None:
```

### Comparing `specsy-0.2.7/src/specsy/io.py` & `specsy-0.2.8/src/specsy/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import os
 import numpy as np
 import configparser
 from pathlib import Path
+
+import pandas as pd
+
 from lime.transitions import label_decomposition
 import lime
 from lime.io import load_cfg, save_cfg, save_frame, check_file_dataframe, check_fit_conf
 from collections.abc import Sequence
 from astropy.io import fits
 
 
@@ -25,15 +28,18 @@
 
 
 # Load log
 def load_frame(file_address, page: str ='LINELOG', sample_levels: list =['id', 'line'], flux_type=None, lines_list=None,
                norm_line=None):
 
     # Return
-    log = lime.load_frame(file_address, page, sample_levels)
+    if isinstance(file_address, pd.DataFrame):
+        log = file_address.copy()
+    else:
+        log = lime.load_frame(file_address, page, sample_levels)
 
     extra_column = 'line_extract' if norm_line is not None else 'line_flux'
 
     # Create new column for the lines flux with the requested type (None for user to introduce "line_flux")
     if flux_type is not None:
         lime.tools.extract_fluxes(log, flux_type=flux_type, column_name=extra_column)
```

### Comparing `specsy-0.2.7/src/specsy/models/chemistry.py` & `specsy-0.2.8/src/specsy/models/chemistry.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
 try:
     import pyneb as pn
     pyneb_check = True
 except ImportError:
     pyneb_check = False
 
+f_lambda_dict = {'Ne5_3426A': 0.39007327642328193, 'H1_3704A': 0.3140805693603108, 'O2_3726A_m': 0.3067768458982876, 'O2_3726A': 0.3067768458982876, 'O2_3729A': 0.3058662813859485, 'H1_3750A': 0.2989658287267065, 'H1_3771A': 0.2923988864345617, 'H1_3798A': 0.28376476642417625, 'H1_3835A': 0.27209526905153303, 'Ne3_3869A': 0.2618967220857926, 'H1_3889A': 0.2557809891273626, 'H1_3970A': 0.23198534354014377, 'He1_4026A': 0.21606552409784063, 'S2_4069A': 0.2043275716588584, 'H1_4102A': 0.19532246622634286, 'H1_4340A': 0.1345184866324025, 'O3_4363A': 0.12907397984854385, 'He1_4471A': 0.10008316812687346, 'Fe3_4658A': 0.05008559375773025, 'He2_4685A': 0.04306145401678374, 'Ar4_4711A': 0.03656608779554027, 'Ar4_4740A': 0.029353696058204592, 'H1_4861A': 0.0, 'He1_4922A': -0.01413318511741013, 'O3_4959A': -0.022588313009073047, 'O3_5007A': -0.03336167870361706, 'N2_5755A': -0.18418774041199926, 'He1_5876A': -0.20680077428006316, 'O1_6300A': -0.27936359987068493, 'S3_6312A': -0.28123411434673595, 'N2_6548A': -0.3173469917409416, 'H1_6563A': -0.31952058255138915, 'N2_6583A': -0.32254097821555716, 'He1_6678A': -0.3361647881852353, 'S2_6716A': -0.3415641010661673, 'S2_6731A': -0.34357533413787533, 'He1_7065A': -0.3880517953849959, 'Ar3_7136A': -0.3969061757103082, 'O2_7319A_m': -0.41908454023400266, 'O2_7319A': -0.41908454023400266, 'O2_7330A': -0.42035048955048104, 'Ar3_7751A': -0.4672699048137039, 'H1_8392A': -0.5296236462812575, 'H1_8413A': -0.5314977585865324, 'H1_8438A': -0.5336928162672543, 'H1_8467A': -0.5362865949831361, 'H1_8502A': -0.5393816101427606, 'H1_8545A': -0.543116195197769, 'H1_8598A': -0.5476792555250717, 'H1_8665A': -0.5533353188659278, 'H1_8750A': -0.5604637553180236, 'H1_8863A': -0.5696232832294517, 'H1_9015A': -0.5816662195724203, 'S3_9068A': -0.5858209361879336, 'H1_9229A': -0.5979429077869078, 'S3_9530A': -0.6196286670577644, 'H1_9546A': -0.6206981718255229}
+
+
 _logger = logging.getLogger('SpecSy')
 
 
 def TOIII_from_TSIII_relation(T_low):
     # From Hagele et al 2006
     return (0.8403 * T_low / 10000.0 + 0.2689) * 10000.0
 
@@ -241,17 +244,26 @@
         self.lines = self.frame.index.to_numpy()
         self.particles = self.frame.particle.to_numpy()
         self.fluxes = self.frame.line_flux.to_numpy()
         self.errs = self.frame.line_flux_err.to_numpy()
         self.wave = self.frame.wavelength.to_numpy()
 
         # Compute the extinction # TODO normalization for multiple lines
-        norm_line = np.unique(self.frame.norm_line.to_numpy())[0]
-        line = lime.Line(norm_line)
-        self.f_lambda = flambda_calc(self.wave, R_v, extinction_law, line.wavelength)
+        # if pyneb_check:
+        #     norm_line = np.unique(self.frame.norm_line.to_numpy())[0]
+        #     line = lime.Line(norm_line)
+        #     self.f_lambda = flambda_calc(self.wave, R_v, extinction_law, line.wavelength)
+        # else:
+        #     self.f_lambda = np.zeros(self.lines.size)
+        #     for i, line in enumerate(self.lines):
+        #         self.f_lambda[i] = f_lambda_dict[line]
+
+        self.f_lambda = np.zeros(self.lines.size)
+        for i, line in enumerate(self.lines):
+            self.f_lambda[i] = f_lambda_dict[line]
 
         return
 
     def review_model(self, emissivity_grid, prior_dict, temp_zones, verbose=True):
 
         # Check that the lines are present in the dataframe
         if emissivity_grid is not None:
```

### Comparing `specsy-0.2.7/src/specsy/models/chemistry_inference.py` & `specsy-0.2.8/src/specsy/models/chemistry_inference.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/models/emissivity.py` & `specsy-0.2.8/src/specsy/models/emissivity.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/models/extinction.py` & `specsy-0.2.8/src/specsy/models/extinction.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/models/fluxes_line.py` & `specsy-0.2.8/src/specsy/models/fluxes_line.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/models/nebular_continuum.py` & `specsy-0.2.8/src/specsy/models/nebular_continuum.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/operations/interpolation.py` & `specsy-0.2.8/src/specsy/operations/interpolation.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/operations/pytensors.py` & `specsy-0.2.8/src/specsy/operations/pytensors.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/operations/tensors.py` & `specsy-0.2.8/src/specsy/operations/tensors.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/operations/tests.py` & `specsy-0.2.8/src/specsy/operations/tests.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/plots.py` & `specsy-0.2.8/src/specsy/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,17 @@
     plot_cfg = theme.fig_defaults(size_conf, fig_type='traces')
     ax_cfg = theme.ax_defaults(fig_type='traces')
 
     # Initialize the figure
     with (rc_context(plot_cfg)):
 
         # Plot format
-        fig = plt.figure()
+        # Generate the figure if not provided
+        if in_fig is None:
+            in_fig = plt.figure()
         gs = gridspec.GridSpec(n_traces * 2, 4)
         gs.update(wspace=0.2, hspace=1.8)
 
         # Colors
         colorNorm = colors.Normalize(0, n_traces)
         cmap = cm.get_cmap(name=theme.colors['mask_map'])
 
@@ -165,19 +167,21 @@
 
             if i < n_traces:
 
                 param = input_params[i]
                 trace_array = infer_db.posterior[param].values
                 trace_array = trace_array.reshape(-1)
 
+                print(trace_array)
+
                 mean_value = np.mean(trace_array)
                 std_dev = np.std(trace_array)
 
-                axTrace = fig.add_subplot(gs[2 * i:2 * (1 + i), :3])
-                axPoterior = fig.add_subplot(gs[2 * i:2 * (1 + i), 3])
+                axTrace = in_fig.add_subplot(gs[2 * i:2 * (1 + i), :3])
+                axPoterior = in_fig.add_subplot(gs[2 * i:2 * (1 + i), 3])
 
                 param_latex = _setup_cfg['latex'][param]
                 label_measurement = parameter_notation(param, mean_value, std_dev)
 
                 # Plot the traces
                 axTrace.plot(trace_array, label=label_measurement, color=cmap(colorNorm(i)))
                 axTrace.axhline(y=mean_value, color=cmap(colorNorm(i)), linestyle='--')
@@ -283,15 +287,19 @@
         # Generate the color dict
         input_ions = np.unique(ion_array)
         colorNorm = colors.Normalize(0, input_ions.size)
         cmap = cm.get_cmap(name=theme.colors['mask_map'])
         color_dict = dict(zip(input_ions, np.arange(input_ions.size)))
 
         # self.FigConf(plotSize=size_dict, Figtype='Grid', n_columns=n_columns, n_rows=n_rows)
-        fig, axes = plt.subplots(n_rows, n_cols)
+        if in_fig is None:
+            in_fig = plt.figure()
+
+        axes = in_fig.subplots(n_rows, n_cols)
+        # axes = plt.subplots(n_rows, n_cols)
         axes = axes.ravel()
 
         # Plot individual traces
         for i in range(n_cells):
 
             if i < n_lines:
 
@@ -317,15 +325,15 @@
 
                 # Plot formating
                 axes[i].get_yaxis().set_visible(False)
                 axes[i].set_yticks([])
                 axes[i].set_title(latexLabel_array[i])
 
             else:
-                fig.delaxes(axes[i])
+                in_fig.delaxes(axes[i])
 
         # Show or save the image
         in_fig = save_close_fig_swicth(output_address, 'tight', in_fig, maximize, display_check)
 
     return in_fig
 
 
@@ -363,24 +371,24 @@
             true_array.append(true_values[param])
 
     # Change to numpy and transpose
     labels_list, traces_list = np.array(labels_list), np.array(traces_list).T
     true_array = None if true_array is None else np.array(true_array)
 
     # Set the plot format where the user's overwrites the default
-    plot_cfg = theme.fig_defaults()
+    plot_cfg = theme.fig_defaults(fig_cfg)
     ax_cfg = theme.ax_defaults()
 
     # Initialize the figure
     with (rc_context(plot_cfg)):
 
         # Generate the plot
-        fig = corner.corner(traces_list, fontsize=30, labels=labels_list, quantiles=[0.16, 0.5, 0.84],
+        corner.corner(traces_list, fontsize=30, labels=labels_list, quantiles=[0.16, 0.5, 0.84],
                             show_titles=True, title_args={"fontsize": 200}, truths=true_array,
-                            truth_color=theme.colors['fg'], title_fmt='0.3f')
+                            truth_color=theme.colors['fg'], title_fmt='0.3f', fig=in_fig)
 
         # Show or save the image
         in_fig = save_close_fig_swicth(output_address, 'tight', in_fig, maximize, display_check)
 
 
     # Dark models
     # # Declare figure format
```

### Comparing `specsy-0.2.7/src/specsy/resources/HI_t3_elec.ascii` & `specsy-0.2.8/src/specsy/resources/HI_t3_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/resources/HeII_t4_elec.ascii` & `specsy-0.2.8/src/specsy/resources/HeII_t4_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/resources/HeI_t5_elec.ascii` & `specsy-0.2.8/src/specsy/resources/HeI_t5_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/tools.py` & `specsy-0.2.8/src/specsy/tools.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy/treatement.py` & `specsy-0.2.8/src/specsy/treatement.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.7/src/specsy.egg-info/PKG-INFO` & `specsy-0.2.8/src/specsy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsy
-Version: 0.2.7
+Version: 0.2.8
 Summary: Model fitting package for the chemical analysis of astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/specsy
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `specsy-0.2.7/src/specsy.egg-info/SOURCES.txt` & `specsy-0.2.8/src/specsy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

