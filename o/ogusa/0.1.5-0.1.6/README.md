# Comparing `tmp/ogusa-0.1.5.tar.gz` & `tmp/ogusa-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogusa-0.1.5.tar", last modified: Fri Apr 12 23:38:47 2024, max compression
+gzip compressed data, was "ogusa-0.1.6.tar", last modified: Thu May  9 00:20:24 2024, max compression
```

## Comparing `ogusa-0.1.5.tar` & `ogusa-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:38:47.534392 ogusa-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-12 23:38:43.000000 ogusa-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-12 23:38:47.534392 ogusa-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-12 23:38:43.000000 ogusa-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:38:47.534392 ogusa-0.1.5/ogusa/
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/bequest_transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/calibrate_chi_n.py
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/deterministic_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/estimate_beta_j.py
--rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/get_micro_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/income.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/labor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/macro_params.py
--rw-r--r--   0 runner    (1001) docker     (127)  2040787 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/ogusa_default_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/psid_data_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/psid_summ_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/transfer_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/wealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/wealthinit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:38:47.534392 ogusa-0.1.5/ogusa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-12 23:38:47.000000 ogusa-0.1.5/ogusa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-12 23:38:47.000000 ogusa-0.1.5/ogusa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 23:38:47.000000 ogusa-0.1.5/ogusa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-12 23:38:47.000000 ogusa-0.1.5/ogusa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 23:38:47.000000 ogusa-0.1.5/ogusa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-12 23:38:44.000000 ogusa-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 23:38:47.534392 ogusa-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-12 23:38:44.000000 ogusa-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:20:24.110449 ogusa-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-09 00:20:19.000000 ogusa-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-09 00:20:24.110449 ogusa-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-09 00:20:19.000000 ogusa-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:20:24.110449 ogusa-0.1.6/ogusa/
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/bequest_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/calibrate_chi_n.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/deterministic_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/estimate_beta_j.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/get_micro_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/income.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/labor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/macro_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2040787 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/ogusa_default_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/psid_data_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/psid_summ_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/transfer_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/wealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/wealthinit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:20:24.110449 ogusa-0.1.6/ogusa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-09 00:20:24.000000 ogusa-0.1.6/ogusa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-09 00:20:24.000000 ogusa-0.1.6/ogusa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:20:24.000000 ogusa-0.1.6/ogusa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-09 00:20:24.000000 ogusa-0.1.6/ogusa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 00:20:24.000000 ogusa-0.1.6/ogusa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 00:20:20.000000 ogusa-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 00:20:24.110449 ogusa-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-09 00:20:20.000000 ogusa-0.1.6/setup.py
```

### Comparing `ogusa-0.1.5/LICENSE` & `ogusa-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/PKG-INFO` & `ogusa-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: ogusa
-Version: 0.1.5
+Version: 0.1.6
 Summary: USA calibration for OG-Core
 Home-page: https://github.com/PSLmodels/OG-USA/
 Download-URL: https://github.com/PSLmodels/OG-USA/
 Author: Jason DeBacker and Richard W. Evans
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Issue Tracker, https://github.com/PSLmodels/OG-USA/issues
 Keywords: USA calibration of large scale overlapping generations model of fiscal policy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Common Public License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7.7, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OG-USA
 
 | | |
 | --- | --- |
 | Org | [![PSL cataloged](https://img.shields.io/badge/PSL-cataloged-a0a0a0.svg)](https://www.PSLmodels.org) [![OS License: CC0-1.0](https://img.shields.io/badge/OS%20License-CC0%201.0-yellow)](https://github.com/PSLmodels/OG-USA/blob/master/LICENSE) [![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](https://pslmodels.github.io/OG-Core/) |
-| Package | [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-3917/) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31013/) [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3116/) [![PyPI Latest Release](https://img.shields.io/pypi/v/ogusa.svg)](https://pypi.org/project/ogusa/) [![PyPI Downloads](https://img.shields.io/pypi/dm/ogusa.svg?label=PyPI%20downloads)](https://pypi.org/project/fiscalsim-us/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
+| Package | [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31013/) [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3116/) [![PyPI Latest Release](https://img.shields.io/pypi/v/ogusa.svg)](https://pypi.org/project/ogusa/) [![PyPI Downloads](https://img.shields.io/pypi/dm/ogusa.svg?label=PyPI%20downloads)](https://pypi.org/project/fiscalsim-us/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
 | Testing | ![example event parameter](https://github.com/PSLmodels/OG-USA/actions/workflows/build_and_test.yml/badge.svg?branch=master) ![example event parameter](https://github.com/PSLmodels/OG-USA/actions/workflows/deploy_docs.yml/badge.svg?branch=master) ![example event parameter](https://github.com/PSLmodels/OG-USA/actions/workflows/check_format.yml/badge.svg?branch=master) [![Codecov](https://codecov.io/gh/PSLmodels/OG-USA/branch/master/graph/badge.svg)](https://codecov.io/gh/PSLmodels/OG-USA) |
 
 OG-USA is an overlapping-generations (OG) model that allows for dynamic general equilibrium analysis of fiscal policy for the United States. OG-USA is built on the [OG-Core](https://github.com/PSLmodels/OG-Core) framework. The model output includes changes in macroeconomic aggregates (GDP, investment, consumption), wages, interest rates, and the stream of tax revenues over time. Regularly updated documentation of the model theory--its output, and solution method--and the Python API is available at [https://pslmodels.github.io/OG-Core](https://pslmodels.github.io/OG-Core) and documentation of the specific United States calibration of the model is available at [https://pslmodels.github.io/OG-USA](https://pslmodels.github.io/OG-USA).
 
 
 ## Disclaimer
```

### Comparing `ogusa-0.1.5/README.md` & `ogusa-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # OG-USA
 
 | | |
 | --- | --- |
 | Org | [![PSL cataloged](https://img.shields.io/badge/PSL-cataloged-a0a0a0.svg)](https://www.PSLmodels.org) [![OS License: CC0-1.0](https://img.shields.io/badge/OS%20License-CC0%201.0-yellow)](https://github.com/PSLmodels/OG-USA/blob/master/LICENSE) [![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](https://pslmodels.github.io/OG-Core/) |
-| Package | [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-3917/) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31013/) [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3116/) [![PyPI Latest Release](https://img.shields.io/pypi/v/ogusa.svg)](https://pypi.org/project/ogusa/) [![PyPI Downloads](https://img.shields.io/pypi/dm/ogusa.svg?label=PyPI%20downloads)](https://pypi.org/project/fiscalsim-us/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
+| Package | [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31013/) [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3116/) [![PyPI Latest Release](https://img.shields.io/pypi/v/ogusa.svg)](https://pypi.org/project/ogusa/) [![PyPI Downloads](https://img.shields.io/pypi/dm/ogusa.svg?label=PyPI%20downloads)](https://pypi.org/project/fiscalsim-us/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
 | Testing | ![example event parameter](https://github.com/PSLmodels/OG-USA/actions/workflows/build_and_test.yml/badge.svg?branch=master) ![example event parameter](https://github.com/PSLmodels/OG-USA/actions/workflows/deploy_docs.yml/badge.svg?branch=master) ![example event parameter](https://github.com/PSLmodels/OG-USA/actions/workflows/check_format.yml/badge.svg?branch=master) [![Codecov](https://codecov.io/gh/PSLmodels/OG-USA/branch/master/graph/badge.svg)](https://codecov.io/gh/PSLmodels/OG-USA) |
 
 OG-USA is an overlapping-generations (OG) model that allows for dynamic general equilibrium analysis of fiscal policy for the United States. OG-USA is built on the [OG-Core](https://github.com/PSLmodels/OG-Core) framework. The model output includes changes in macroeconomic aggregates (GDP, investment, consumption), wages, interest rates, and the stream of tax revenues over time. Regularly updated documentation of the model theory--its output, and solution method--and the Python API is available at [https://pslmodels.github.io/OG-Core](https://pslmodels.github.io/OG-Core) and documentation of the specific United States calibration of the model is available at [https://pslmodels.github.io/OG-USA](https://pslmodels.github.io/OG-USA).
 
 
 ## Disclaimer
```

### Comparing `ogusa-0.1.5/ogusa/bequest_transmission.py` & `ogusa-0.1.6/ogusa/bequest_transmission.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import os
 from ogusa.utils import MVKDE
 
 CURDIR = os.path.split(os.path.abspath(__file__))[0]
 
 
 def get_bequest_matrix(
-    J=7, lambdas=np.array([0.25, 0.25, 0.2, 0.1, 0.1, 0.09, 0.01]), graphs=True
+    J=7,
+    lambdas=np.array([0.25, 0.25, 0.2, 0.1, 0.1, 0.09, 0.01]),
+    graphs=False,
 ):
     """
     Returns S x J matrix representing the fraction of aggregate
     bequests that go to each household by age and lifetime income group.
 
     """
     # Create directory if output directory does not already exist
```

### Comparing `ogusa-0.1.5/ogusa/calibrate.py` & `ogusa-0.1.6/ogusa/calibrate.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,31 +15,54 @@
         self,
         p,
         estimate_tax_functions=False,
         estimate_beta=False,
         estimate_chi_n=False,
         estimate_pop=False,
         tax_func_path=None,
+        iit_baseline=None,
         iit_reform={},
         guid="",
         data="cps",
         client=None,
         num_workers=1,
     ):
+        """
+        Constructor for the Calibration class.  This class is used to find
+        parameter values for the OG-USA model.
+
+        Args:
+            p (OGUSA Parameters object): parameters object
+            estimate_tax_functions (bool): whether to estimate tax functions
+            estimate_beta (bool): whether to estimate beta
+            estimate_chi_n (bool): whether to estimate chi_n
+            estimate_pop (bool): whether to estimate population
+            tax_func_path (str): path to tax function parameters
+            iit_baseline (dict): baseline policy to use
+            iit_reform (dict): reform tax parameters
+            guid (str): id for tax function parameters
+            data (str): data source for microsimulation model
+            client (Dask client object): client
+            num_workers (int): number of workers for Dask client
+
+        Returns:
+            Calibration class object instance
+        """
         self.estimate_tax_functions = estimate_tax_functions
         self.estimate_beta = estimate_beta
         self.estimate_chi_n = estimate_chi_n
         self.estimate_pop = estimate_pop
         if estimate_tax_functions:
             if tax_func_path is not None:
                 run_micro = False
             else:
                 run_micro = True
             self.tax_function_params = self.get_tax_function_parameters(
                 p,
+                iit_baseline,
                 iit_reform,
                 guid,
                 data,
                 client,
                 num_workers,
                 run_micro=run_micro,
                 tax_func_path=tax_func_path,
@@ -64,25 +87,27 @@
                 p.E,
                 p.S,
                 p.T,
                 0,
                 99,
                 initial_data_year=p.start_year - 1,
                 final_data_year=p.start_year,
+                GraphDiag=False,
             )
 
             # demographics for 80 period lives (needed for getting e below)
             demog80 = demographics.get_pop_objs(
                 20,
                 80,
                 p.T,
                 0,
                 99,
                 initial_data_year=p.start_year - 1,
                 final_data_year=p.start_year,
+                GraphDiag=False,
             )
 
             # earnings profiles
             self.e = income.get_e_interp(
                 p.S,
                 self.demographic_params["omega_SS"],
                 demog80["omega_SS"],
@@ -98,28 +123,35 @@
                 plot=False,
             )
 
     # Tax Functions
     def get_tax_function_parameters(
         self,
         p,
+        iit_baseline=None,
         iit_reform={},
         guid="",
         data="",
         client=None,
         num_workers=1,
         run_micro=False,
         tax_func_path=None,
     ):
         """
         Reads pickle file of tax function parameters or estimates the
         parameters from microsimulation model output.
 
         Args:
+            p (OG-Core Parameters object): parameters object
+            iit_baseline (dict): baseline policy to use
+            iit_reform (dict): reform tax parameters
+            guid (string): id for tax function parameters
+            data (string): data source for microsimulation model
             client (Dask client object): client
+            num_workers (int): number of workers for Dask client
             run_micro (bool): whether to estimate parameters from
                 microsimulation model
             tax_func_path (string): path where find or save tax
                 function parameter estimates
 
         Returns:
             None
@@ -146,34 +178,32 @@
                 p, tax_func_path
             )
             taxcalc_version = "Cached tax parameters, no taxcalc version"
         if run_micro:
             micro_data, taxcalc_version = get_micro_data.get_data(
                 baseline=p.baseline,
                 start_year=p.start_year,
-                reform=iit_reform,
+                iit_baseline=iit_baseline,
+                iit_reform=iit_reform,
                 data=data,
                 path=p.output_base,
                 client=client,
                 num_workers=num_workers,
             )
             p.BW = len(micro_data)
             dict_params = txfunc.tax_func_estimate(  # pragma: no cover
                 micro_data,
                 p.BW,
                 p.S,
                 p.starting_age,
                 p.ending_age,
                 start_year=p.start_year,
-                baseline=p.baseline,
                 analytical_mtrs=p.analytical_mtrs,
                 tax_func_type=p.tax_func_type,
                 age_specific=p.age_specific,
-                reform=iit_reform,
-                data=data,
                 client=client,
                 num_workers=num_workers,
                 tax_func_path=tax_func_path,
             )
         mean_income_data = dict_params["tfunc_avginc"][0]
         frac_tax_payroll = np.append(
             dict_params["tfunc_frac_tax_payroll"],
```

### Comparing `ogusa-0.1.5/ogusa/calibrate_chi_n.py` & `ogusa-0.1.6/ogusa/calibrate_chi_n.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/ogusa/constants.py` & `ogusa-0.1.6/ogusa/constants.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/ogusa/deterministic_profiles.py` & `ogusa-0.1.6/ogusa/deterministic_profiles.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/ogusa/estimate_beta_j.py` & `ogusa-0.1.6/ogusa/estimate_beta_j.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/ogusa/get_micro_data.py` & `ogusa-0.1.6/ogusa/get_micro_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 CUR_PATH = os.path.split(os.path.abspath(__file__))[0]
 
 
 def get_calculator(
     baseline,
     calculator_start_year,
-    reform=None,
+    iit_baseline=None,
+    iit_reform=None,
     data=None,
     gfactors=None,
     weights=None,
     records_start_year=PUF_START_YEAR,
 ):
     """
     This function creates the tax calculator object with the policy
@@ -68,55 +69,61 @@
             weights=weights,
             start_year=records_start_year,
         )  # pragma: no cover
     else:  # pragma: no cover
         records1 = Records()  # pragma: no cover
 
     if baseline:
-        if not reform:
+        if iit_baseline is None:
             print("Running current law policy baseline")
         else:
-            print("Baseline policy is: ", reform)
+            print("Baseline policy is: ", iit_baseline)
+            policy1.implement_reform(iit_baseline)
     else:
-        if not reform:
+        if not iit_reform:
             print("Running with current law as reform")
         else:
-            print("Reform policy is: ", reform)
-            print("TYPE", type(reform))
-    policy1.implement_reform(reform)
+            print("Reform policy is: ", iit_reform)
+            if (
+                iit_baseline is not None
+            ):  # if alt baseline, stack reform on that
+                policy1.implement_reform(iit_baseline)
+            policy1.implement_reform(iit_reform)
 
     # the default set up increments year to 2013
     calc1 = Calculator(records=records1, policy=policy1)
 
     # Check that start_year is appropriate
     if calculator_start_year > TC_LAST_YEAR:
         raise RuntimeError("Start year is beyond data extrapolation.")
 
     return calc1
 
 
 def get_data(
     baseline=False,
     start_year=DEFAULT_START_YEAR,
-    reform={},
+    iit_baseline=None,
+    iit_reform={},
     data=None,
     path=CUR_PATH,
     client=None,
     num_workers=1,
 ):
     """
     This function creates dataframes of micro data with marginal tax
     rates and information to compute effective tax rates from the
     Tax-Calculator output.  The resulting dictionary of dataframes is
     returned and saved to disk in a pickle file.
 
     Args:
         baseline (boolean): True if baseline tax policy
         calculator_start_year (int): first year of budget window
-        reform (dictionary): IIT policy reform parameters, None if
+        iit_baseline (dictionary): IIT policy parameters for baseline
+        iit_reform (dictionary): IIT policy reform parameters, None if
             baseline
         data (DataFrame or str): DataFrame or path to datafile for
             Records object
         path (str): path to save microdata files to
         client (Dask Client object): client for Dask multiprocessing
         num_workers (int): number of workers to use for Dask
             multiprocessing
@@ -128,15 +135,17 @@
         taxcalc_version (str): version of Tax-Calculator used
 
     """
     # Compute MTRs and taxes or each year, but not beyond TC_LAST_YEAR
     lazy_values = []
     for year in range(start_year, TC_LAST_YEAR + 1):
         lazy_values.append(
-            delayed(taxcalc_advance)(baseline, start_year, reform, data, year)
+            delayed(taxcalc_advance)(
+                baseline, start_year, iit_baseline, iit_reform, data, year
+            )
         )
     if client:  # pragma: no cover
         futures = client.compute(lazy_values, num_workers=num_workers)
         results = client.gather(futures)
     else:
         results = results = compute(
             *lazy_values,
@@ -163,31 +172,39 @@
 
     # Pull Tax-Calc version for reference
     taxcalc_version = pkg_resources.get_distribution("taxcalc").version
 
     return micro_data_dict, taxcalc_version
 
 
-def taxcalc_advance(baseline, start_year, reform, data, year):
+def taxcalc_advance(
+    baseline, start_year, iit_baseline, iit_reform, data, year
+):
     """
     This function advances the year used in Tax-Calculator, compute
     taxes and rates, and save the results to a dictionary.
 
     Args:
-        calc1 (Tax-Calculator Calculator object): TC calculator
-        year (int): year to begin advancing from
+        baseline (boolean): True if baseline tax policy
+        start_year (int): first year of budget window
+        iit_baseline (dict): IIT policy parameters for baseline
+        iit_reform (dict): IIT policy reform parameters for reform
+        data (DataFrame or str): DataFrame or path to datafile for
+            Records object
+        year (int): year to advance to in Tax-Calculator
 
     Returns:
         tax_dict (dict): a dictionary of microdata with marginal tax
             rates and other information computed in TC
     """
     calc1 = get_calculator(
         baseline=baseline,
         calculator_start_year=start_year,
-        reform=reform,
+        iit_baseline=iit_baseline,
+        iit_reform=iit_reform,
         data=data,
     )
     calc1.advance_to_year(year)
     calc1.calc_all()
     print("Year: ", str(calc1.current_year))
 
     # define market income - taking expanded_income and excluding gov't
```

### Comparing `ogusa-0.1.5/ogusa/income.py` & `ogusa-0.1.6/ogusa/income.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/ogusa/labor.py` & `ogusa-0.1.6/ogusa/labor.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         labor_moments_boot[i, :] = compute_labor_moments(boot, S)
 
     VCV = np.cov(labor_moments_boot.T)
 
     return VCV
 
 
-def labor_data_graphs(weighted, S, J, output_dir):
+def labor_data_graphs(weighted, S, J, output_dir=None):
     """
     Plot labor supply data.
 
     Args:
         weighted (Numpy array):
         S (int): number of periods of economic life for model households
         J (int): number of lifetime income groups
@@ -162,31 +162,38 @@
 
     """
     domain = np.linspace(20, 80, S)
     Jgrid = np.linspace(1, 100, J)
     X, Y = np.meshgrid(domain, Jgrid)
     cmap2 = matplotlib.cm.get_cmap("summer")
 
-    plt.plot(domain, weighted, color="black", label="Data")
-    plt.plot(
-        np.linspace(76, 100, 23),
-        extension,
-        color="black",
-        linestyle="-.",
-        label="Extrapolation",
-    )
-    plt.plot(np.linspace(65, 76, 11), to_dot, linestyle="--", color="black")
-    plt.axvline(x=76, color="black", linestyle="--")
-    plt.xlabel(r"age-$s$")
-    plt.ylabel(r"individual labor supply $/bar{l}_s$")
-    plt.legend()
-    plt.savefig(
-        os.path.join(baseline_dir, "Demographics/labor_dist_data_withfit.png")
-    )
-
-    fig10 = plt.figure()
-    ax10 = fig10.add_subplot(projection="3d")
-    ax10.plot_surface(X, Y, lab_mat_basic.T, rstride=1, cstride=2, cmap=cmap2)
-    ax10.set_xlabel(r"age-$s$")
-    ax10.set_ylabel(r"ability type -$j$")
-    ax10.set_zlabel(r"labor $e_j(s)$")
-    plt.savefig(os.path.join(baseline_dir, "Demographics/data_labor_dist"))
+    if output_dir:
+        plt.plot(domain, weighted, color="black", label="Data")
+        plt.plot(
+            np.linspace(76, 100, 23),
+            extension,
+            color="black",
+            linestyle="-.",
+            label="Extrapolation",
+        )
+        plt.plot(
+            np.linspace(65, 76, 11), to_dot, linestyle="--", color="black"
+        )
+        plt.axvline(x=76, color="black", linestyle="--")
+        plt.xlabel(r"age-$s$")
+        plt.ylabel(r"individual labor supply $/bar{l}_s$")
+        plt.legend()
+        plt.savefig(
+            os.path.join(
+                output_dir, "Demographics/labor_dist_data_withfit.png"
+            )
+        )
+
+        fig10 = plt.figure()
+        ax10 = fig10.add_subplot(projection="3d")
+        ax10.plot_surface(
+            X, Y, lab_mat_basic.T, rstride=1, cstride=2, cmap=cmap2
+        )
+        ax10.set_xlabel(r"age-$s$")
+        ax10.set_ylabel(r"ability type -$j$")
+        ax10.set_zlabel(r"labor $e_j(s)$")
+        plt.savefig(os.path.join(output_dir, "Demographics/data_labor_dist"))
```

### Comparing `ogusa-0.1.5/ogusa/macro_params.py` & `ogusa-0.1.6/ogusa/macro_params.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/ogusa/ogusa_default_parameters.json` & `ogusa-0.1.6/ogusa/ogusa_default_parameters.json`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/ogusa/psid_data_setup.py` & `ogusa-0.1.6/ogusa/psid_data_setup.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/ogusa/psid_summ_stats.py` & `ogusa-0.1.6/ogusa/psid_summ_stats.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/ogusa/transfer_distribution.py` & `ogusa-0.1.6/ogusa/transfer_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import os
 from ogusa.utils import MVKDE
 
 CURDIR = os.path.split(os.path.abspath(__file__))[0]
 
 
 def get_transfer_matrix(
-    J=7, lambdas=np.array([0.25, 0.25, 0.2, 0.1, 0.1, 0.09, 0.01]), graphs=True
+    J=7,
+    lambdas=np.array([0.25, 0.25, 0.2, 0.1, 0.1, 0.09, 0.01]),
+    graphs=False,
 ):
     """
     Compute SxJ matrix representing the distribution of aggregate
     government transfers by age and lifetime income group.
     """
     # Create directory if output directory does not already exist
     CURDIR = os.path.split(os.path.abspath(__file__))[0]
```

### Comparing `ogusa-0.1.5/ogusa/utils.py` & `ogusa-0.1.6/ogusa/utils.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/ogusa/wealth.py` & `ogusa-0.1.6/ogusa/wealth.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/ogusa/wealthinit.py` & `ogusa-0.1.6/ogusa/wealthinit.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/ogusa.egg-info/PKG-INFO` & `ogusa-0.1.6/ogusa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: ogusa
-Version: 0.1.5
+Version: 0.1.6
 Summary: USA calibration for OG-Core
 Home-page: https://github.com/PSLmodels/OG-USA/
 Download-URL: https://github.com/PSLmodels/OG-USA/
 Author: Jason DeBacker and Richard W. Evans
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Issue Tracker, https://github.com/PSLmodels/OG-USA/issues
 Keywords: USA calibration of large scale overlapping generations model of fiscal policy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Common Public License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7.7, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OG-USA
 
 | | |
 | --- | --- |
 | Org | [![PSL cataloged](https://img.shields.io/badge/PSL-cataloged-a0a0a0.svg)](https://www.PSLmodels.org) [![OS License: CC0-1.0](https://img.shields.io/badge/OS%20License-CC0%201.0-yellow)](https://github.com/PSLmodels/OG-USA/blob/master/LICENSE) [![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](https://pslmodels.github.io/OG-Core/) |
-| Package | [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-3917/) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31013/) [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3116/) [![PyPI Latest Release](https://img.shields.io/pypi/v/ogusa.svg)](https://pypi.org/project/ogusa/) [![PyPI Downloads](https://img.shields.io/pypi/dm/ogusa.svg?label=PyPI%20downloads)](https://pypi.org/project/fiscalsim-us/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
+| Package | [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31013/) [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3116/) [![PyPI Latest Release](https://img.shields.io/pypi/v/ogusa.svg)](https://pypi.org/project/ogusa/) [![PyPI Downloads](https://img.shields.io/pypi/dm/ogusa.svg?label=PyPI%20downloads)](https://pypi.org/project/fiscalsim-us/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
 | Testing | ![example event parameter](https://github.com/PSLmodels/OG-USA/actions/workflows/build_and_test.yml/badge.svg?branch=master) ![example event parameter](https://github.com/PSLmodels/OG-USA/actions/workflows/deploy_docs.yml/badge.svg?branch=master) ![example event parameter](https://github.com/PSLmodels/OG-USA/actions/workflows/check_format.yml/badge.svg?branch=master) [![Codecov](https://codecov.io/gh/PSLmodels/OG-USA/branch/master/graph/badge.svg)](https://codecov.io/gh/PSLmodels/OG-USA) |
 
 OG-USA is an overlapping-generations (OG) model that allows for dynamic general equilibrium analysis of fiscal policy for the United States. OG-USA is built on the [OG-Core](https://github.com/PSLmodels/OG-Core) framework. The model output includes changes in macroeconomic aggregates (GDP, investment, consumption), wages, interest rates, and the stream of tax revenues over time. Regularly updated documentation of the model theory--its output, and solution method--and the Python API is available at [https://pslmodels.github.io/OG-Core](https://pslmodels.github.io/OG-Core) and documentation of the specific United States calibration of the model is available at [https://pslmodels.github.io/OG-USA](https://pslmodels.github.io/OG-USA).
 
 
 ## Disclaimer
```

### Comparing `ogusa-0.1.5/ogusa.egg-info/SOURCES.txt` & `ogusa-0.1.6/ogusa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.5/setup.py` & `ogusa-0.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as readme_file:
     longdesc = readme_file.read()
 
 setuptools.setup(
     name="ogusa",
-    version="0.1.5",
+    version="0.1.6",
     author="Jason DeBacker and Richard W. Evans",
     license="CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     description="USA calibration for OG-Core",
     long_description_content_type="text/markdown",
     long_description=longdesc,
     keywords="USA calibration of large scale overlapping generations model of fiscal policy",
     url="https://github.com/PSLmodels/OG-USA/",
@@ -44,15 +44,14 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "License :: OSI Approved :: Common Public License",
         "Operating System :: POSIX",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     tests_require=["pytest"],
 )
```

