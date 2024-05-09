# Comparing `tmp/mpmaps-0.1.2.tar.gz` & `tmp/mpmaps-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpmaps-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mpmaps-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mpmaps-0.1.2.tar` & `mpmaps-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1542 2024-05-04 15:22:24.391594 mpmaps-0.1.2/LICENSE
--rw-r--r--   0        0        0     2883 2024-05-04 15:22:24.391594 mpmaps-0.1.2/README.md
--rw-r--r--   0        0        0      745 2024-05-04 15:22:24.391594 mpmaps-0.1.2/mpmaps/__init__.py
--rw-r--r--   0        0        0      120 2024-05-04 15:22:24.391594 mpmaps-0.1.2/mpmaps/globals.py
--rw-r--r--   0        0        0    10244 2024-05-04 15:22:24.391594 mpmaps-0.1.2/mpmaps/mpmaps.py
--rw-r--r--   0        0        0     1343 2024-05-04 15:22:24.391594 mpmaps-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4094 1970-01-01 00:00:00.000000 mpmaps-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1542 2024-05-09 14:52:50.696413 mpmaps-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2883 2024-05-09 14:52:50.696413 mpmaps-0.2.0/README.md
+-rw-r--r--   0        0        0      745 2024-05-09 14:52:50.696413 mpmaps-0.2.0/mpmaps/__init__.py
+-rw-r--r--   0        0        0      120 2024-05-09 14:52:50.696413 mpmaps-0.2.0/mpmaps/globals.py
+-rw-r--r--   0        0        0    12458 2024-05-09 14:52:50.696413 mpmaps-0.2.0/mpmaps/mpmaps.py
+-rw-r--r--   0        0        0     1343 2024-05-09 14:52:50.696413 mpmaps-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4094 1970-01-01 00:00:00.000000 mpmaps-0.2.0/PKG-INFO
```

### Comparing `mpmaps-0.1.2/LICENSE` & `mpmaps-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpmaps-0.1.2/README.md` & `mpmaps-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mpmaps-0.1.2/mpmaps/__init__.py` & `mpmaps-0.2.0/mpmaps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __author__ = """Nicolas Aunai"""
 __email__ = "nicolas.aunai@lpp.polytechnique.fr"
-__version__ = '0.1.2'
+__version__ = '0.2.0'
 
 from platformdirs import user_data_dir
 import urllib.request
 import os
 
 from .mpmaps import MPMap
 from .globals import grids
```

### Comparing `mpmaps-0.1.2/mpmaps/mpmaps.py` & `mpmaps-0.2.0/mpmaps/mpmaps.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,48 @@
 import numpy as np
 import pandas as pd
 from scipy import constants as cst
 from scipy.optimize import root
 from platformdirs import user_data_dir
 from .globals import grids
 import os
+import matplotlib.pyplot as plt
 
 
 from spok.models import planetary as smp
 from spok import smath as sm
 from spok.coordinates import coordinates as scc
 from spok import utils as su
 
 
 class MPMap:
     def __init__(self, **kwargs):
+        """
+        Keyword arguments:
+        ------------------
+
+        clock: float, (default:-90)
+                IMF clock angle in degrees, 0 is due north
+
+        cone: float, (default: 55)
+                IMF cone angle in degrees, 0 is radial IMF
+
+        tilt: float, (default: 0)
+                Dipole tilt axis
+
+        bimf: float, (default: 5)
+                IMF amplitude in nT
+
+        nws: float (default 5)
+                solar wind density, in cm^-3
+
+        mp_thick: float, (default 800)
+                Magnetopause thickness in km
+                only used for computing the current density
+        """
         self._grid_path = os.path.join(user_data_dir(), "mpmaps")
         self._clock = kwargs.get("clock", -90)
         self._cone = kwargs.get("cone", 55)
         self._tilt = kwargs.get("tilt", 0)
         self._bimf = kwargs.get("bimf", 5)
         self._nsw = kwargs.get("nsw", 5)
         self._mp_thick = kwargs.get("mp_thick", 800)
@@ -210,14 +234,65 @@
         b1 = B1 * np.sin(np.radians(theta))
         b2 = B2 * np.sin(np.radians(alpha - theta))
         u = (b1 * b2) ** (3 / 2)
         v = np.sqrt((b2 * n1 + b1 * n2) * (b1 + b2))
         R = k * u / v
         return R
 
+    def plot(self, **kwargs):
+        """
+        Keyword arguments
+        -----------------
+
+        value : string ("shear_angle":default, "reconnection_rate", "current_density")
+                the quantity that is plotted
+
+        xlim : tuple, lower bound of the plot area
+        ylim : tuple, upper bound of the plot area
+        filename : string, file name to save the figure on disk
+
+        other keywork arguments: see MPMap
+
+        example : mp.plot(value="shear_angle", tilt=14, xlim=(-18,18), ylim=(-18,18))
+        """
+
+        if "ax" in kwargs:
+            ax = kwargs["ax"]
+            fig = ax.get_figure()
+        else:
+            fig, ax = plt.subplots()
+
+        msh = smp.Magnetosheath()
+        phi = np.arange(0, np.pi * 2 + 0.1, 0.1)
+        theta = np.pi / 2
+        _, y, z = msh.magnetopause(theta, phi)
+        ax.plot(y, z, ls="--", color="k")
+
+        xmin, xmax = kwargs.get("xlim", (self.Y.min(), self.Y.max()))
+        ymin, ymax = kwargs.get("ylim", (self.Z.min(), self.Z.max()))
+
+        ax.set_xlim((xmin, xmax))
+        ax.set_ylim((ymin, ymax))
+        ax.set_xlabel(r"$Y/R_e$")
+        ax.set_ylabel(r"$Z/R_e$")
+
+        self.set_parameters(**kwargs)
+        val = kwargs.get("value", "shear_angle")
+        sa = getattr(self, val)()
+
+        ax.pcolormesh(self.Y, self.Z, sa, cmap="jet")
+        ax.axvline(0, ls="--", color="k")
+        ax.axhline(0, ls="--", color="k")
+        ax.set_aspect("equal")
+
+        if "filename" in kwargs:
+            fig.savefig(kwargs["filename"])
+
+        return fig, ax
+
     def _find_rec_angle_max_rate(self):
         def _dRR_dtheta_local(theta, params):
             n1 = params[:, 0] * 1e6 * cst.m_p
             n2 = params[:, 1] * 1e6 * cst.m_p
             B1 = sm.norm(params[:, 2], params[:, 3], params[:, 4]) * 1e-9
             B2 = sm.norm(params[:, 5], params[:, 6], params[:, 7]) * 1e-9
             alpha = parameters[:, -1]
```

### Comparing `mpmaps-0.1.2/pyproject.toml` & `mpmaps-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core"]
 
 [project]
 name = "mpmaps"
-version = "0.1.2"
+version = "0.2.0"
 description = "magnetopause maps"
 keywords = ["space", "plasma-physics"]
 authors = [
     { name = "Bayane Michotte de Welle", email = "bayane.michotte-de-welle@lpp.polytechnique.fr" },
     { name = "Nicolas Aunai", email = "nicolas.aunai@lpp.polytechnique.fr" }
 ]
```

### Comparing `mpmaps-0.1.2/PKG-INFO` & `mpmaps-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpmaps
-Version: 0.1.2
+Version: 0.2.0
 Summary: magnetopause maps
 Keywords: space,plasma-physics
 Author-email: Bayane Michotte de Welle <bayane.michotte-de-welle@lpp.polytechnique.fr>, Nicolas Aunai <nicolas.aunai@lpp.polytechnique.fr>
 Maintainer-email: Bayane Michotte de Welle <bayane.michotte-de-welle@lpp.polytechnique.fr>, Nicolas Aunai <nicolas.aunai@lpp.polytechnique.fr>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
```

