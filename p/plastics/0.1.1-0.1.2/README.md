# Comparing `tmp/plastics-0.1.1.tar.gz` & `tmp/plastics-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plastics-0.1.1.tar", last modified: Thu May  9 01:09:03 2024, max compression
+gzip compressed data, was "plastics-0.1.2.tar", last modified: Thu May  9 14:40:41 2024, max compression
```

## Comparing `plastics-0.1.1.tar` & `plastics-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 01:09:03.395832 plastics-0.1.1/
--rw-rw-rw-   0        0        0     1082 2024-05-08 03:02:34.000000 plastics-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2336 2024-05-09 01:09:03.395832 plastics-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1435 2024-05-08 15:48:34.000000 plastics-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-09 01:09:03.332414 plastics-0.1.1/plastics/
--rw-rw-rw-   0        0        0       92 2023-09-22 17:17:37.000000 plastics-0.1.1/plastics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 01:09:03.395832 plastics-0.1.1/plastics/strap/
--rw-rw-rw-   0        0        0      790 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/__init__.py
--rw-rw-rw-   0        0        0     2380 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/dissolution_steps.py
--rw-rw-rw-   0        0        0     2904 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/precipitation_steps.py
--rw-rw-rw-   0        0        0     9553 2024-05-08 16:59:06.000000 plastics-0.1.1/plastics/strap/process_model.py
--rw-rw-rw-   0        0        0     1410 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/process_settings.py
--rw-rw-rw-   0        0        0     1688 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/property_package.py
--rw-rw-rw-   0        0        0    17156 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/simulation.py
--rw-rw-rw-   0        0        0    19328 2024-05-08 17:16:43.000000 plastics-0.1.1/plastics/strap/systems.py
--rw-rw-rw-   0        0        0    12304 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/tea.py
--rw-rw-rw-   0        0        0    18667 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/units.py
-drwxrwxrwx   0        0        0        0 2024-05-09 01:09:03.364043 plastics-0.1.1/plastics.egg-info/
--rw-rw-rw-   0        0        0     2336 2024-05-09 01:09:03.000000 plastics-0.1.1/plastics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2024-05-09 01:09:03.000000 plastics-0.1.1/plastics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 01:09:03.000000 plastics-0.1.1/plastics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-09 01:09:03.000000 plastics-0.1.1/plastics.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 01:09:03.000000 plastics-0.1.1/plastics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 01:09:03.395832 plastics-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1543 2024-05-09 01:08:20.000000 plastics-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:40:41.951450 plastics-0.1.2/
+-rw-rw-rw-   0        0        0     1082 2024-05-08 03:02:34.000000 plastics-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2336 2024-05-09 14:40:41.951450 plastics-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1435 2024-05-08 15:48:34.000000 plastics-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-09 14:40:41.913521 plastics-0.1.2/plastics/
+-rw-rw-rw-   0        0        0       92 2023-09-22 17:17:37.000000 plastics-0.1.2/plastics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:40:41.950389 plastics-0.1.2/plastics/strap/
+-rw-rw-rw-   0        0        0      813 2024-05-09 14:38:54.000000 plastics-0.1.2/plastics/strap/__init__.py
+-rw-rw-rw-   0        0        0     2380 2024-05-08 13:43:02.000000 plastics-0.1.2/plastics/strap/dissolution_steps.py
+-rw-rw-rw-   0        0        0     2904 2024-05-08 13:43:02.000000 plastics-0.1.2/plastics/strap/precipitation_steps.py
+-rw-rw-rw-   0        0        0     9553 2024-05-08 16:59:06.000000 plastics-0.1.2/plastics/strap/process_model.py
+-rw-rw-rw-   0        0        0     1410 2024-05-08 13:43:02.000000 plastics-0.1.2/plastics/strap/process_settings.py
+-rw-rw-rw-   0        0        0     1688 2024-05-08 13:43:02.000000 plastics-0.1.2/plastics/strap/property_package.py
+-rw-rw-rw-   0        0        0    17160 2024-05-09 14:38:30.000000 plastics-0.1.2/plastics/strap/simulation.py
+-rw-rw-rw-   0        0        0    19328 2024-05-08 17:16:43.000000 plastics-0.1.2/plastics/strap/systems.py
+-rw-rw-rw-   0        0        0    12304 2024-05-08 13:43:02.000000 plastics-0.1.2/plastics/strap/tea.py
+-rw-rw-rw-   0        0        0    18667 2024-05-08 13:43:02.000000 plastics-0.1.2/plastics/strap/units.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:40:41.939255 plastics-0.1.2/plastics.egg-info/
+-rw-rw-rw-   0        0        0     2336 2024-05-09 14:40:41.000000 plastics-0.1.2/plastics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2024-05-09 14:40:41.000000 plastics-0.1.2/plastics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 14:40:41.000000 plastics-0.1.2/plastics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-09 14:40:41.000000 plastics-0.1.2/plastics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 14:40:41.000000 plastics-0.1.2/plastics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 14:40:41.951450 plastics-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1543 2024-05-09 14:39:32.000000 plastics-0.1.2/setup.py
```

### Comparing `plastics-0.1.1/LICENSE` & `plastics-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plastics-0.1.1/PKG-INFO` & `plastics-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plastics
-Version: 0.1.1
+Version: 0.1.2
 Summary: Plastic processing models in BioSTEAM
 Home-page: https://github.com/yoelcortes/plastics
 Download-URL: https://github.com/yoelcortes/plastics
 Author: Yoel Cortes-Pena
 Author-email: yoelcortes@gmail.com
 License: MIT
 Keywords: chemical process simulation plastic bioprocess engineering STRAP solvent targeted dissolution precipitation
```

### Comparing `plastics-0.1.1/README.rst` & `plastics-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `plastics-0.1.1/plastics/strap/__init__.py` & `plastics-0.1.2/plastics/strap/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 """
+__version__ = '0.1.2'
+
 from . import dissolution_steps
 from . import precipitation_steps
 from . import process_settings
 from . import property_package
 from . import process_model
 from . import systems
 from . import tea
@@ -29,8 +31,7 @@
     *process_settings.__all__,
     *property_package.__all__,
     *process_model.__all__,
     *systems.__all__,
     *tea.__all__,
 )
 
-
```

### Comparing `plastics-0.1.1/plastics/strap/dissolution_steps.py` & `plastics-0.1.2/plastics/strap/dissolution_steps.py`

 * *Files identical despite different names*

### Comparing `plastics-0.1.1/plastics/strap/precipitation_steps.py` & `plastics-0.1.2/plastics/strap/precipitation_steps.py`

 * *Files identical despite different names*

### Comparing `plastics-0.1.1/plastics/strap/process_model.py` & `plastics-0.1.2/plastics/strap/process_model.py`

 * *Files identical despite different names*

### Comparing `plastics-0.1.1/plastics/strap/process_settings.py` & `plastics-0.1.2/plastics/strap/process_settings.py`

 * *Files identical despite different names*

### Comparing `plastics-0.1.1/plastics/strap/property_package.py` & `plastics-0.1.2/plastics/strap/property_package.py`

 * *Files identical despite different names*

### Comparing `plastics-0.1.1/plastics/strap/simulation.py` & `plastics-0.1.2/plastics/strap/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import biosteam as bst
 import numpy as np
 import pandas as pd
 import os
 from thermosteam.units_of_measure import format_units
 from thermosteam.utils import roundsigfigs
 from matplotlib import pyplot as plt
-from SALib.analyze import sobol
 import matplotlib.patches as mpatches
 from colorpalette import Color
 import yaml
 
 __all__ = ('run_monte_carlo', 'plot_spearman', 'plot_kde',
            'plot_MSP_GWP_across_dissolution_capacity_boiling_point',
            'run_monte_carlo_across_polymer_composition',
@@ -234,14 +233,15 @@
         if i.index not in pm.model.table: pm.model._metrics.remove(i)
     pm.model.table = pm.model.table.dropna(how='any', axis=0)
     rho, p = pm.model.spearman_r(filter='omit nan')
     file = spearman_file(pm.name)
     rho.to_excel(file)
 
 def sobol_analysis():
+    from SALib.analyze import sobol
     filterwarnings('ignore', category=bst.exceptions.DesignWarning)
     filterwarnings('ignore', category=bst.exceptions.CostWarning)
     pm = sp.SingleDissolutionSTRAPModel(simulate=False)
     pm.model.exception_hook = 'raise'
     for kind, params, metric in [('tea', pm.tea_parameters, pm.MSP), ('lca', pm.lca_parameters, pm.GWP)]:
         file = sobol_file('_'.join([pm.name, kind]))
         pm.model.parameters = params
```

### Comparing `plastics-0.1.1/plastics/strap/systems.py` & `plastics-0.1.2/plastics/strap/systems.py`

 * *Files identical despite different names*

### Comparing `plastics-0.1.1/plastics/strap/tea.py` & `plastics-0.1.2/plastics/strap/tea.py`

 * *Files identical despite different names*

### Comparing `plastics-0.1.1/plastics/strap/units.py` & `plastics-0.1.2/plastics/strap/units.py`

 * *Files identical despite different names*

### Comparing `plastics-0.1.1/plastics.egg-info/PKG-INFO` & `plastics-0.1.2/plastics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plastics
-Version: 0.1.1
+Version: 0.1.2
 Summary: Plastic processing models in BioSTEAM
 Home-page: https://github.com/yoelcortes/plastics
 Download-URL: https://github.com/yoelcortes/plastics
 Author: Yoel Cortes-Pena
 Author-email: yoelcortes@gmail.com
 License: MIT
 Keywords: chemical process simulation plastic bioprocess engineering STRAP solvent targeted dissolution precipitation
```

### Comparing `plastics-0.1.1/setup.py` & `plastics-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # for license details.
 from setuptools import setup
 
 setup(
     name='plastics',
     packages=['plastics'],
     license='MIT',
-    version='0.1.1',
+    version='0.1.2',
     description="Plastic processing models in BioSTEAM",
     long_description=open('README.rst', encoding='utf-8').read(),
     author='Yoel Cortes-Pena',
     install_requires=['biosteam>=2.44.0,<2.45.0'],
     python_requires=">=3.9",
     package_data={
         'plastics': [
```

