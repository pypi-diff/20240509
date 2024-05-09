# Comparing `tmp/pandorapsf-0.2.3.tar.gz` & `tmp/pandorapsf-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandorapsf-0.2.3.tar", max compression
+gzip compressed data, was "pandorapsf-0.2.4.tar", max compression
```

## Comparing `pandorapsf-0.2.3.tar` & `pandorapsf-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1071 2023-09-22 21:06:08.416872 pandorapsf-0.2.3/LICENSE
--rw-r--r--   0        0        0       15 2023-09-21 17:07:25.661702 pandorapsf-0.2.3/README.md
--rw-r--r--   0        0        0      363 2024-05-08 19:42:02.089691 pandorapsf-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1740 2024-05-08 19:41:51.918384 pandorapsf-0.2.3/src/pandorapsf/__init__.py
--rw-r--r--   0        0        0    14579 2023-10-11 00:00:22.516507 pandorapsf-0.2.3/src/pandorapsf/data/dichroic-transmission.csv
--rw-r--r--   0        0        0   100800 2024-05-03 14:35:17.450737 pandorapsf-0.2.3/src/pandorapsf/data/nirda-wav-solution.fits
--rw-r--r--   0        0        0     2777 2023-09-21 16:57:33.816212 pandorapsf-0.2.3/src/pandorapsf/data/pandora.mplstyle
--rw-r--r--   0        0        0     6452 2023-10-10 23:55:05.530892 pandorapsf-0.2.3/src/pandorapsf/data/pandora_visible_qe.csv
--rw-r--r--   0        0        0    25577 2023-09-22 16:23:38.985186 pandorapsf-0.2.3/src/pandorapsf/data/pixel_vs_wavelength.csv
--rw-r--r--   0        0        0    14400 2024-05-03 14:35:17.463147 pandorapsf-0.2.3/src/pandorapsf/data/visda-wav-solution.fits
--rw-r--r--   0        0        0     7461 2024-05-08 14:32:10.310103 pandorapsf-0.2.3/src/pandorapsf/plotting.py
--rw-r--r--   0        0        0    29360 2024-05-08 19:13:45.641761 pandorapsf-0.2.3/src/pandorapsf/psf.py
--rw-r--r--   0        0        0    30154 2024-05-08 15:43:00.159415 pandorapsf-0.2.3/src/pandorapsf/scene.py
--rw-r--r--   0        0        0     8506 2024-05-08 19:29:04.935549 pandorapsf-0.2.3/src/pandorapsf/sparsewarp.py
--rw-r--r--   0        0        0    22754 2024-05-08 19:05:42.377580 pandorapsf-0.2.3/src/pandorapsf/utils.py
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 pandorapsf-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-09-22 21:06:08.416872 pandorapsf-0.2.4/LICENSE
+-rw-r--r--   0        0        0       15 2023-09-21 17:07:25.661702 pandorapsf-0.2.4/README.md
+-rw-r--r--   0        0        0      363 2024-05-09 14:42:49.751935 pandorapsf-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1734 2024-05-09 14:42:53.261321 pandorapsf-0.2.4/src/pandorapsf/__init__.py
+-rw-r--r--   0        0        0    14579 2023-10-11 00:00:22.516507 pandorapsf-0.2.4/src/pandorapsf/data/dichroic-transmission.csv
+-rw-r--r--   0        0        0   100800 2024-05-03 14:35:17.450737 pandorapsf-0.2.4/src/pandorapsf/data/nirda-wav-solution.fits
+-rw-r--r--   0        0        0     2777 2023-09-21 16:57:33.816212 pandorapsf-0.2.4/src/pandorapsf/data/pandora.mplstyle
+-rw-r--r--   0        0        0     6452 2023-10-10 23:55:05.530892 pandorapsf-0.2.4/src/pandorapsf/data/pandora_visible_qe.csv
+-rw-r--r--   0        0        0    25577 2023-09-22 16:23:38.985186 pandorapsf-0.2.4/src/pandorapsf/data/pixel_vs_wavelength.csv
+-rw-r--r--   0        0        0    14400 2024-05-03 14:35:17.463147 pandorapsf-0.2.4/src/pandorapsf/data/visda-wav-solution.fits
+-rw-r--r--   0        0        0     7461 2024-05-08 14:32:10.310103 pandorapsf-0.2.4/src/pandorapsf/plotting.py
+-rw-r--r--   0        0        0    29360 2024-05-08 19:13:45.641761 pandorapsf-0.2.4/src/pandorapsf/psf.py
+-rw-r--r--   0        0        0    30154 2024-05-08 15:43:00.159415 pandorapsf-0.2.4/src/pandorapsf/scene.py
+-rw-r--r--   0        0        0     8506 2024-05-08 19:29:04.935549 pandorapsf-0.2.4/src/pandorapsf/sparsewarp.py
+-rw-r--r--   0        0        0    22754 2024-05-08 19:05:42.377580 pandorapsf-0.2.4/src/pandorapsf/utils.py
+-rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 pandorapsf-0.2.4/PKG-INFO
```

### Comparing `pandorapsf-0.2.3/LICENSE` & `pandorapsf-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.3/src/pandorapsf/__init__.py` & `pandorapsf-0.2.4/src/pandorapsf/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 # Standard library
 import os  # noqa
 
 PACKAGEDIR = os.path.abspath(os.path.dirname(__file__))
 TESTDIR = "/".join(PACKAGEDIR.split("/")[:-2]) + "/tests/"
 PANDORASTYLE = "{}/data/pandora.mplstyle".format(PACKAGEDIR)
 
@@ -14,34 +14,34 @@
 from rich.logging import RichHandler  # noqa: E402
 
 logging.basicConfig()
 log = logging.getLogger("pandora-psf")
 log.addHandler(RichHandler(markup=True))
 log.setLevel("INFO")
 
-if not os.path.isfile(f"{PACKAGEDIR}/data/pandora_vis_20220506.fits"):
+if not os.path.isfile(f"{PACKAGEDIR}/data/pandora_vis_2024-05.fits"):
     from astropy.utils.data import download_file  # noqa: E402
 
     # Download vis PSF
     log.warning("No PSF file found. Downloading 2GB VIS PSF file.")
     p = download_file(
         "https://zenodo.org/records/11153153/files/pandora_vis_2024-05.fits?download=1",
         pkgname="pandora-psf",
     )
-    shutil.move(p, f"{PACKAGEDIR}/data/pandora_vis_20220506.fits")
-    log.warning(f"VIS PSF downloaded to {PACKAGEDIR}/data/pandora_vis_20220506.fits.")
+    shutil.move(p, f"{PACKAGEDIR}/data/pandora_vis_2024-05.fits")
+    log.warning(f"VIS PSF downloaded to {PACKAGEDIR}/data/pandora_vis_2024-05.fits.")
 
-if not os.path.isfile(f"{PACKAGEDIR}/data/pandora_nir_20220506.fits"):
+if not os.path.isfile(f"{PACKAGEDIR}/data/pandora_nir_2024-05.fits"):
     from astropy.utils.data import download_file  # noqa: E402
 
     # Download nir PSF
     log.warning("No PSF file found. Downloading 2GB NIR PSF")
     p = download_file(
         "https://zenodo.org/records/11153153/files/pandora_nir_2024-05.fits?download=1",
         pkgname="pandora-psf",
     )
-    shutil.move(p, f"{PACKAGEDIR}/data/pandora_nir_20220506.fits")
-    log.warning(f"NIR PSF downloaded to {PACKAGEDIR}/data/pandora_nir_20220506.fits.")
+    shutil.move(p, f"{PACKAGEDIR}/data/pandora_nir_2024-05.fits")
+    log.warning(f"NIR PSF downloaded to {PACKAGEDIR}/data/pandora_nir_2024-05.fits.")
 
 from .psf import PSF  # noqa: F401, E402
 from .scene import ROIScene, Scene, TraceScene  # noqa: F401, E402
 from .sparsewarp import ROISparseWarp3D, SparseWarp3D  # noqa: F401, E402
```

### Comparing `pandorapsf-0.2.3/src/pandorapsf/data/dichroic-transmission.csv` & `pandorapsf-0.2.4/src/pandorapsf/data/dichroic-transmission.csv`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.3/src/pandorapsf/data/nirda-wav-solution.fits` & `pandorapsf-0.2.4/src/pandorapsf/data/nirda-wav-solution.fits`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.3/src/pandorapsf/data/pandora.mplstyle` & `pandorapsf-0.2.4/src/pandorapsf/data/pandora.mplstyle`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.3/src/pandorapsf/data/pandora_visible_qe.csv` & `pandorapsf-0.2.4/src/pandorapsf/data/pandora_visible_qe.csv`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.3/src/pandorapsf/data/pixel_vs_wavelength.csv` & `pandorapsf-0.2.4/src/pandorapsf/data/pixel_vs_wavelength.csv`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.3/src/pandorapsf/data/visda-wav-solution.fits` & `pandorapsf-0.2.4/src/pandorapsf/data/visda-wav-solution.fits`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.3/src/pandorapsf/plotting.py` & `pandorapsf-0.2.4/src/pandorapsf/plotting.py`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.3/src/pandorapsf/psf.py` & `pandorapsf-0.2.4/src/pandorapsf/psf.py`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.3/src/pandorapsf/scene.py` & `pandorapsf-0.2.4/src/pandorapsf/scene.py`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.3/src/pandorapsf/sparsewarp.py` & `pandorapsf-0.2.4/src/pandorapsf/sparsewarp.py`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.3/src/pandorapsf/utils.py` & `pandorapsf-0.2.4/src/pandorapsf/utils.py`

 * *Files identical despite different names*

