# Comparing `tmp/openmc_regular_mesh_plotter-1.2.1.tar.gz` & `tmp/openmc_regular_mesh_plotter-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmc_regular_mesh_plotter-1.2.1.tar", last modified: Thu Feb 29 22:35:46 2024, max compression
+gzip compressed data, was "openmc_regular_mesh_plotter-1.2.2.tar", last modified: Thu May  9 09:55:37 2024, max compression
```

## Comparing `openmc_regular_mesh_plotter-1.2.1.tar` & `openmc_regular_mesh_plotter-1.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:35:46.778695 openmc_regular_mesh_plotter-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:35:46.774695 openmc_regular_mesh_plotter-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:35:46.774695 openmc_regular_mesh_plotter-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/.github/workflows/ci_with_install.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-02-29 22:35:46.778695 openmc_regular_mesh_plotter-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:35:46.778695 openmc_regular_mesh_plotter-1.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/examples/plot_minimal_2d_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/examples/plot_minimal_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/examples/plot_sweep_through_slice_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/examples/plot_two_tallies_combined.py
--rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/examples/plot_with_custom_color_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 22:35:46.778695 openmc_regular_mesh_plotter-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:35:46.774695 openmc_regular_mesh_plotter-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:35:46.778695 openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-29 22:35:46.000000 openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:35:46.778695 openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-02-29 22:35:46.000000 openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-29 22:35:46.000000 openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 22:35:46.000000 openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-29 22:35:46.000000 openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-29 22:35:46.000000 openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:35:46.778695 openmc_regular_mesh_plotter-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-02-29 22:35:35.000000 openmc_regular_mesh_plotter-1.2.1/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:55:37.414204 openmc_regular_mesh_plotter-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:55:37.410204 openmc_regular_mesh_plotter-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:55:37.410204 openmc_regular_mesh_plotter-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/.github/workflows/ci_with_install.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-09 09:55:37.414204 openmc_regular_mesh_plotter-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:55:37.414204 openmc_regular_mesh_plotter-1.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/examples/plot_minimal_2d_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/examples/plot_minimal_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/examples/plot_sweep_through_slice_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/examples/plot_two_tallies_combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/examples/plot_with_custom_color_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:55:37.414204 openmc_regular_mesh_plotter-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:55:37.410204 openmc_regular_mesh_plotter-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:55:37.414204 openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 09:55:37.000000 openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13937 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:55:37.414204 openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-09 09:55:37.000000 openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-09 09:55:37.000000 openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:55:37.000000 openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-09 09:55:37.000000 openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 09:55:37.000000 openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:55:37.414204 openmc_regular_mesh_plotter-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-09 09:55:27.000000 openmc_regular_mesh_plotter-1.2.2/tests/test_units.py
```

### Comparing `openmc_regular_mesh_plotter-1.2.1/.github/workflows/black.yml` & `openmc_regular_mesh_plotter-1.2.2/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `openmc_regular_mesh_plotter-1.2.1/.github/workflows/ci_with_install.yml` & `openmc_regular_mesh_plotter-1.2.2/.github/workflows/ci_with_install.yml`

 * *Files identical despite different names*

### Comparing `openmc_regular_mesh_plotter-1.2.1/.github/workflows/python-publish.yml` & `openmc_regular_mesh_plotter-1.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openmc_regular_mesh_plotter-1.2.1/.gitignore` & `openmc_regular_mesh_plotter-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `openmc_regular_mesh_plotter-1.2.1/CITATION.cff` & `openmc_regular_mesh_plotter-1.2.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `openmc_regular_mesh_plotter-1.2.1/LICENSE.txt` & `openmc_regular_mesh_plotter-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openmc_regular_mesh_plotter-1.2.1/PKG-INFO` & `openmc_regular_mesh_plotter-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc_regular_mesh_plotter
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python package for creating plots of OpenMC regular mesh tallies with the underlying geometry
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2021 Fusion Energy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `openmc_regular_mesh_plotter-1.2.1/README.md` & `openmc_regular_mesh_plotter-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `openmc_regular_mesh_plotter-1.2.1/examples/plot_minimal_2d_example.py` & `openmc_regular_mesh_plotter-1.2.2/examples/plot_minimal_2d_example.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import openmc
 from matplotlib.colors import LogNorm
-from openmc_regular_mesh_plotter import plot_mesh_tally
 
+from openmc_regular_mesh_plotter import plot_mesh_tally
 
 # MATERIALS
 mat_1 = openmc.Material()
 mat_1.add_element("Li", 1)
 mat_1.set_density("g/cm3", 0.45)
 my_materials = openmc.Materials([mat_1])
```

### Comparing `openmc_regular_mesh_plotter-1.2.1/examples/plot_minimal_example.py` & `openmc_regular_mesh_plotter-1.2.2/examples/plot_minimal_example.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import openmc
 from matplotlib.colors import LogNorm
-from openmc_regular_mesh_plotter import plot_mesh_tally
 
+from openmc_regular_mesh_plotter import plot_mesh_tally
 
 # MATERIALS
 mat_1 = openmc.Material()
 mat_1.add_element("Li", 1)
 mat_1.set_density("g/cm3", 0.45)
 my_materials = openmc.Materials([mat_1])
```

### Comparing `openmc_regular_mesh_plotter-1.2.1/examples/plot_sweep_through_slice_indexes.py` & `openmc_regular_mesh_plotter-1.2.2/examples/plot_sweep_through_slice_indexes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # this example is used to make the animation in the readme.
 # It is also set up to accept any geometry and the mesh tally will adapt to the geometry dimensions
 
 
-import openmc
+import matplotlib
 import numpy as np
+import openmc
+from matplotlib import cm
 from matplotlib.colors import LogNorm
+
 from openmc_regular_mesh_plotter import plot_mesh_tally
-from matplotlib import cm
-import matplotlib
 
 # sets the font for the axis
 matplotlib.rc("font", **{"family": "normal", "size": 22})
 
 # MATERIALS
 
 breeder_material = openmc.Material()  # Pb84.2Li15.8
```

### Comparing `openmc_regular_mesh_plotter-1.2.1/examples/plot_two_tallies_combined.py` & `openmc_regular_mesh_plotter-1.2.2/examples/plot_two_tallies_combined.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import openmc
 from matplotlib.colors import LogNorm
-from openmc_regular_mesh_plotter import plot_mesh_tally
 
+from openmc_regular_mesh_plotter import plot_mesh_tally
 
 # MATERIALS
 mat_1 = openmc.Material()
 mat_1.add_element("Li", 1)
 mat_1.set_density("g/cm3", 0.1)
 my_materials = openmc.Materials([mat_1])
```

### Comparing `openmc_regular_mesh_plotter-1.2.1/examples/plot_with_custom_color_map.py` & `openmc_regular_mesh_plotter-1.2.2/examples/plot_with_custom_color_map.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # this example is used to make the animation in the readme.
 # It is also set up to accept any geometry and the mesh tally will adapt to the geometry dimensions
 
 
+import matplotlib.pyplot as plt
 import openmc
-from matplotlib.colors import LogNorm
-from openmc_regular_mesh_plotter import plot_mesh_tally
 from matplotlib import cm
-import matplotlib.pyplot as plt
+from matplotlib.colors import LogNorm
 
+from openmc_regular_mesh_plotter import plot_mesh_tally
 
 # materials
 mat_concrete = openmc.Material()
 mat_concrete.add_element("H", 0.168759)
 mat_concrete.add_element("C", 0.001416)
 mat_concrete.add_element("O", 0.562524)
 mat_concrete.add_element("Na", 0.011838)
```

### Comparing `openmc_regular_mesh_plotter-1.2.1/pyproject.toml` & `openmc_regular_mesh_plotter-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter/core.py` & `openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import math
+import typing
 from pathlib import Path
 from tempfile import TemporaryDirectory
-import typing
-import openmc
+
+import matplotlib.pyplot as plt
 import numpy as np
 import openmc
 import openmc.checkvalue as cv
-import matplotlib.pyplot as plt
-
 from packaging import version
 
 if version.parse(openmc.__version__) < version.parse("0.13.3"):
     msg = (
         "openmc_regular_mesh_plotter package requires OpenMC version 0.13.4 "
         f"or newer. You currently have OpenMC version {openmc.__version__}"
     )
@@ -178,14 +177,21 @@
         )
 
     im = axes.imshow(data, extent=(x_min, x_max, y_min, y_max), **default_imshow_kwargs)
 
     if colorbar:
         fig.colorbar(im, **colorbar_kwargs)
 
+    if outline and geometry is None:
+        msg = (
+            "When calling plot_mesh_tally with outline=True the geometry "
+            "should also be provided. Either set outline to False or set "
+            "the geometry to and openmc.Geometry object"
+        )
+        raise ValueError(msg)
     if outline and geometry is not None:
         import matplotlib.image as mpimg
 
         # code to make sure geometry outline is in the middle of the mesh voxel
         # two of the three dimensions are just in the center of the mesh
         # but the slice can move one axis off the center so this needs calculating
         x0, y0, z0 = mesh.lower_left
```

### Comparing `openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter.egg-info/PKG-INFO` & `openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc_regular_mesh_plotter
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python package for creating plots of OpenMC regular mesh tallies with the underlying geometry
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2021 Fusion Energy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `openmc_regular_mesh_plotter-1.2.1/src/openmc_regular_mesh_plotter.egg-info/SOURCES.txt` & `openmc_regular_mesh_plotter-1.2.2/src/openmc_regular_mesh_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmc_regular_mesh_plotter-1.2.1/tests/test_units.py` & `openmc_regular_mesh_plotter-1.2.2/tests/test_units.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import openmc
+import pytest
 from matplotlib.colors import LogNorm
+
 from openmc_regular_mesh_plotter import plot_mesh_tally
-import pytest
 
 
 @pytest.fixture()
 def model():
     mat1 = openmc.Material()
     mat1.add_nuclide("Li6", 1, percent_type="ao")
     mats = openmc.Materials([mat1])
```

