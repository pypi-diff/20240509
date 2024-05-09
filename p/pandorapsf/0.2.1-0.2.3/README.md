# Comparing `tmp/pandorapsf-0.2.1.tar.gz` & `tmp/pandorapsf-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandorapsf-0.2.1.tar", max compression
+gzip compressed data, was "pandorapsf-0.2.3.tar", max compression
```

## Comparing `pandorapsf-0.2.1.tar` & `pandorapsf-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1071 2023-09-22 21:06:08.416872 pandorapsf-0.2.1/LICENSE
--rw-r--r--   0        0        0       15 2023-09-21 17:07:25.661702 pandorapsf-0.2.1/README.md
--rw-r--r--   0        0        0      830 2024-05-08 15:43:37.799770 pandorapsf-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1672 2024-05-08 15:42:58.562658 pandorapsf-0.2.1/src/pandorapsf/__init__.py
--rw-r--r--   0        0        0    14579 2023-10-11 00:00:22.516507 pandorapsf-0.2.1/src/pandorapsf/data/dichroic-transmission.csv
--rw-r--r--   0        0        0   100800 2024-05-03 14:35:17.450737 pandorapsf-0.2.1/src/pandorapsf/data/nirda-wav-solution.fits
--rw-r--r--   0        0        0     2777 2023-09-21 16:57:33.816212 pandorapsf-0.2.1/src/pandorapsf/data/pandora.mplstyle
--rw-r--r--   0        0        0     6452 2023-10-10 23:55:05.530892 pandorapsf-0.2.1/src/pandorapsf/data/pandora_visible_qe.csv
--rw-r--r--   0        0        0    25577 2023-09-22 16:23:38.985186 pandorapsf-0.2.1/src/pandorapsf/data/pixel_vs_wavelength.csv
--rw-r--r--   0        0        0    14400 2024-05-03 14:35:17.463147 pandorapsf-0.2.1/src/pandorapsf/data/visda-wav-solution.fits
--rw-r--r--   0        0        0     7461 2024-05-08 14:32:10.310103 pandorapsf-0.2.1/src/pandorapsf/plotting.py
--rw-r--r--   0        0        0    29356 2024-05-07 16:23:02.042243 pandorapsf-0.2.1/src/pandorapsf/psf.py
--rw-r--r--   0        0        0    30154 2024-05-08 15:43:00.159415 pandorapsf-0.2.1/src/pandorapsf/scene.py
--rw-r--r--   0        0        0     8472 2024-05-08 15:43:00.055509 pandorapsf-0.2.1/src/pandorapsf/sparsewarp.py
--rw-r--r--   0        0        0    21635 2024-05-08 15:43:00.106434 pandorapsf-0.2.1/src/pandorapsf/utils.py
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 pandorapsf-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-09-22 21:06:08.416872 pandorapsf-0.2.3/LICENSE
+-rw-r--r--   0        0        0       15 2023-09-21 17:07:25.661702 pandorapsf-0.2.3/README.md
+-rw-r--r--   0        0        0      363 2024-05-08 19:42:02.089691 pandorapsf-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1740 2024-05-08 19:41:51.918384 pandorapsf-0.2.3/src/pandorapsf/__init__.py
+-rw-r--r--   0        0        0    14579 2023-10-11 00:00:22.516507 pandorapsf-0.2.3/src/pandorapsf/data/dichroic-transmission.csv
+-rw-r--r--   0        0        0   100800 2024-05-03 14:35:17.450737 pandorapsf-0.2.3/src/pandorapsf/data/nirda-wav-solution.fits
+-rw-r--r--   0        0        0     2777 2023-09-21 16:57:33.816212 pandorapsf-0.2.3/src/pandorapsf/data/pandora.mplstyle
+-rw-r--r--   0        0        0     6452 2023-10-10 23:55:05.530892 pandorapsf-0.2.3/src/pandorapsf/data/pandora_visible_qe.csv
+-rw-r--r--   0        0        0    25577 2023-09-22 16:23:38.985186 pandorapsf-0.2.3/src/pandorapsf/data/pixel_vs_wavelength.csv
+-rw-r--r--   0        0        0    14400 2024-05-03 14:35:17.463147 pandorapsf-0.2.3/src/pandorapsf/data/visda-wav-solution.fits
+-rw-r--r--   0        0        0     7461 2024-05-08 14:32:10.310103 pandorapsf-0.2.3/src/pandorapsf/plotting.py
+-rw-r--r--   0        0        0    29360 2024-05-08 19:13:45.641761 pandorapsf-0.2.3/src/pandorapsf/psf.py
+-rw-r--r--   0        0        0    30154 2024-05-08 15:43:00.159415 pandorapsf-0.2.3/src/pandorapsf/scene.py
+-rw-r--r--   0        0        0     8506 2024-05-08 19:29:04.935549 pandorapsf-0.2.3/src/pandorapsf/sparsewarp.py
+-rw-r--r--   0        0        0    22754 2024-05-08 19:05:42.377580 pandorapsf-0.2.3/src/pandorapsf/utils.py
+-rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 pandorapsf-0.2.3/PKG-INFO
```

### Comparing `pandorapsf-0.2.1/LICENSE` & `pandorapsf-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.1/src/pandorapsf/__init__.py` & `pandorapsf-0.2.3/src/pandorapsf/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-__version__ = "0.2.0"
+__version__ = "0.2.3"
 # Standard library
 import os  # noqa
 
 PACKAGEDIR = os.path.abspath(os.path.dirname(__file__))
 TESTDIR = "/".join(PACKAGEDIR.split("/")[:-2]) + "/tests/"
 PANDORASTYLE = "{}/data/pandora.mplstyle".format(PACKAGEDIR)
 
 # Standard library
 import logging  # noqa: E402
 import shutil  # noqa: E402
 
 # Third-party
-from astropy.utils.data import download_file  # noqa: E402
 from rich.logging import RichHandler  # noqa: E402
 
 logging.basicConfig()
 log = logging.getLogger("pandora-psf")
 log.addHandler(RichHandler(markup=True))
 log.setLevel("INFO")
 
 if not os.path.isfile(f"{PACKAGEDIR}/data/pandora_vis_20220506.fits"):
+    from astropy.utils.data import download_file  # noqa: E402
+
     # Download vis PSF
-    log.warning("No PSF file found. Downloading 100MB VIS PSF file.")
+    log.warning("No PSF file found. Downloading 2GB VIS PSF file.")
     p = download_file(
-        "https://zenodo.org/record/7596336/files/pandora_vis_20220506.fits?download=1",
+        "https://zenodo.org/records/11153153/files/pandora_vis_2024-05.fits?download=1",
         pkgname="pandora-psf",
     )
     shutil.move(p, f"{PACKAGEDIR}/data/pandora_vis_20220506.fits")
     log.warning(f"VIS PSF downloaded to {PACKAGEDIR}/data/pandora_vis_20220506.fits.")
 
 if not os.path.isfile(f"{PACKAGEDIR}/data/pandora_nir_20220506.fits"):
+    from astropy.utils.data import download_file  # noqa: E402
+
     # Download nir PSF
-    log.warning("No PSF file found. Downloading 10MB NIR PSF")
+    log.warning("No PSF file found. Downloading 2GB NIR PSF")
     p = download_file(
-        "https://zenodo.org/record/7596336/files/pandora_nir_20220506.fits?download=1",
+        "https://zenodo.org/records/11153153/files/pandora_nir_2024-05.fits?download=1",
         pkgname="pandora-psf",
     )
     shutil.move(p, f"{PACKAGEDIR}/data/pandora_nir_20220506.fits")
     log.warning(f"NIR PSF downloaded to {PACKAGEDIR}/data/pandora_nir_20220506.fits.")
 
 from .psf import PSF  # noqa: F401, E402
 from .scene import ROIScene, Scene, TraceScene  # noqa: F401, E402
```

### Comparing `pandorapsf-0.2.1/src/pandorapsf/data/dichroic-transmission.csv` & `pandorapsf-0.2.3/src/pandorapsf/data/dichroic-transmission.csv`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.1/src/pandorapsf/data/nirda-wav-solution.fits` & `pandorapsf-0.2.3/src/pandorapsf/data/nirda-wav-solution.fits`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.1/src/pandorapsf/data/pandora.mplstyle` & `pandorapsf-0.2.3/src/pandorapsf/data/pandora.mplstyle`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.1/src/pandorapsf/data/pandora_visible_qe.csv` & `pandorapsf-0.2.3/src/pandorapsf/data/pandora_visible_qe.csv`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.1/src/pandorapsf/data/pixel_vs_wavelength.csv` & `pandorapsf-0.2.3/src/pandorapsf/data/pixel_vs_wavelength.csv`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.1/src/pandorapsf/data/visda-wav-solution.fits` & `pandorapsf-0.2.3/src/pandorapsf/data/visda-wav-solution.fits`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.1/src/pandorapsf/plotting.py` & `pandorapsf-0.2.3/src/pandorapsf/plotting.py`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.1/src/pandorapsf/psf.py` & `pandorapsf-0.2.3/src/pandorapsf/psf.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,15 +434,15 @@
                     rotation=45,
                     color="grey",
                 )
         return ax
 
     def __repr__(self):
         freeze_dictionary = (
-            f" (Frozen: {', '.join([f'{key}: {item}' for key, item in self.freeze_dictionary.items()])})"
+            f" (Frozen: {', '.join([f'{key}: {item:.3f}' for key, item in self.freeze_dictionary.items()])})"
             if len(self.freeze_dictionary) != 0
             else ""
         )
         return f"{self.ndims}D PSF Model [{', '.join(self.dimension_names)}]{freeze_dictionary}"
 
     @staticmethod
     def from_name(
```

### Comparing `pandorapsf-0.2.1/src/pandorapsf/scene.py` & `pandorapsf-0.2.3/src/pandorapsf/scene.py`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.1/src/pandorapsf/sparsewarp.py` & `pandorapsf-0.2.3/src/pandorapsf/sparsewarp.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
                     (row >= rmin) & (row < rmax) & (column >= cmin) & (column < cmax)
                 )
             return np.asarray(mask)
 
         return get_ROI_masks
 
     def __repr__(self):
-        return f"<{(*self.imshape, self.nvecs)} ROISparseWarp3D array of type {self.dtype}>"
+        return f"<{(*self.imshape, self.nvecs)} ROISparseWarp3D array of type {self.dtype}, {self.nROIs} Regions of Interest>"
 
     def _get_submask(self, offset=(0, 0)):
         # find where the data is within the array bounds
         kr = ((self.subrow + offset[0]) < self.imshape[0]) & (
             (self.subrow + offset[0]) >= 0
         )
         kc = ((self.subcol + offset[1]) < self.imshape[1]) & (
```

### Comparing `pandorapsf-0.2.1/src/pandorapsf/utils.py` & `pandorapsf-0.2.3/src/pandorapsf/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,19 +150,18 @@
     )
     hdu.header.append(
         fits.Card("CORRUNIT", corr.unit.to_string(), "units of correction")
     )
     hdu.writeto(f"{PACKAGEDIR}/data/visda-wav-solution.fits", overwrite=True)
 
 
-def _open_LLNL_file(filename):
+def _open_LLNL_file(filename, pixel_size, downsample=None, trim=None):
     """This opens the newest file format from LLNL. They might change it, so watch out."""
     d = loadmat(filename)
     subpixel_size = d["dx"][0][0] * u.micron / u.pix
-    pixel_size = 6.5 * u.micron / u.pix
 
     wvl = np.unique(d["wvl"]) * u.micron
     nwav = wvl.shape[0]
     #    npoints = int(d["x"].shape[1] / nwav)
 
     TC, TR = np.meshgrid(
         np.unique(d["Tx"][0, ::nwav]), np.unique(d["Ty"][0, ::nwav]), indexing="xy"
@@ -225,37 +224,71 @@
     wavelength = wvl[None, None, :] * np.ones((*TR.shape, nwav))
     subpixel_row = ((sR[:, 0] - sR.shape[0] / 2) * u.pixel * subpixel_size)[
         :, None
     ] * np.ones(d["PSF"].shape[:2])
     subpixel_column = ((sC[0] - sC.shape[0] / 2) * u.pixel * subpixel_size)[
         None
     ] * np.ones(d["PSF"].shape[:2])
+
+    if downsample is not None:
+        n = downsample
+        PSF = np.sum(
+            [PSF[idx::n, jdx::n] for idx in range(n) for jdx in range(n)], axis=0
+        )
+        subpixel_column = (
+            np.mean(
+                [
+                    subpixel_column.value[idx::n, jdx::n]
+                    for idx in range(n)
+                    for jdx in range(n)
+                ],
+                axis=0,
+            )
+            * subpixel_column.unit
+        )
+        subpixel_row = (
+            np.mean(
+                [
+                    subpixel_row.value[idx::n, jdx::n]
+                    for idx in range(n)
+                    for jdx in range(n)
+                ],
+                axis=0,
+            )
+            * subpixel_row.unit
+        )
+
+    if trim is not None:
+        PSF = PSF[trim:-trim, trim:-trim]
+        subpixel_column = subpixel_column[trim:-trim, trim:-trim]
+        subpixel_row = subpixel_row[trim:-trim, trim:-trim]
+
     return (
         subpixel_size,
         subpixel_row,
         subpixel_column,
         row,
         column,
         wavelength,
         PSF,
         str(d["__header__"]).split("Created on: ")[-1][:-1],
     )
 
 
-def make_PSF_fits_files(filename, suffix, pixel_size):
+def make_PSF_fits_files(filename, suffix, pixel_size, downsample=None, trim=None):
     (
         subpixel_size,
         subpixel_row,
         subpixel_column,
         row,
         column,
         wavelength,
         PSF,
         created_on,
-    ) = _open_LLNL_file(filename)
+    ) = _open_LLNL_file(filename, pixel_size, downsample=downsample, trim=trim)
     pixel_size = u.Quantity(pixel_size, u.micron / u.pixel)
     subpixel_row, subpixel_column, row, column = (
         (subpixel_row / pixel_size).to(u.pixel),
         (subpixel_column / pixel_size).to(u.pixel),
         (row / pixel_size).to(u.pixel),
         (column / pixel_size).to(u.pixel),
     )
@@ -280,18 +313,18 @@
             ),
         ]
     )
     primaryhdu = fits.PrimaryHDU(header=hdr)
     hdu = fits.HDUList(
         [
             primaryhdu,
-            fits.ImageHDU(PSF, name="PSF"),
-            fits.ImageHDU(row.value, name="ROW"),
-            fits.ImageHDU(column.value, name="COLUMN"),
-            fits.ImageHDU(wavelength.value, name="WAVELENGTH"),
+            fits.ImageHDU(PSF.astype(np.float32), name="PSF"),
+            fits.ImageHDU(row.value.astype(np.float32), name="ROW"),
+            fits.ImageHDU(column.value.astype(np.float32), name="COLUMN"),
+            fits.ImageHDU(wavelength.value.astype(np.float32), name="WAVELENGTH"),
         ]
     )
     hdu[2].header["UNIT"] = row.unit.to_string()
     hdu[3].header["UNIT"] = column.unit.to_string()
     hdu[4].header["UNIT"] = wavelength.unit.to_string()
     hdu.writeto(
         PACKAGEDIR
```

