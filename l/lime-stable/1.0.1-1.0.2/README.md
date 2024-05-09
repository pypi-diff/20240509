# Comparing `tmp/lime-stable-1.0.1.tar.gz` & `tmp/lime-stable-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lime-stable-1.0.1.tar", last modified: Sat May  4 19:09:01 2024, max compression
+gzip compressed data, was "lime-stable-1.0.2.tar", last modified: Thu May  9 05:04:03 2024, max compression
```

## Comparing `lime-stable-1.0.1.tar` & `lime-stable-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:09:01.453855 lime-stable-1.0.1/
--rw-rw-r--   0 vital     (1000) vital     (1000)    35608 2024-04-25 13:12:45.000000 lime-stable-1.0.1/LICENSE.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)       63 2024-04-25 13:06:20.000000 lime-stable-1.0.1/MANIFEST.in
--rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-04 19:09:01.453855 lime-stable-1.0.1/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     2647 2024-04-25 13:09:22.000000 lime-stable-1.0.1/README.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)     1148 2024-05-04 18:56:19.000000 lime-stable-1.0.1/pyproject.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      433 2024-05-04 19:09:01.453855 lime-stable-1.0.1/setup.cfg
--rw-rw-r--   0 vital     (1000) vital     (1000)     1187 2024-04-25 13:12:39.000000 lime-stable-1.0.1/setup.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:09:01.449855 lime-stable-1.0.1/src/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:09:01.449855 lime-stable-1.0.1/src/lime/
--rw-rw-r--   0 vital     (1000) vital     (1000)     1307 2024-04-25 21:14:21.000000 lime-stable-1.0.1/src/lime/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    12833 2024-05-01 21:07:04.000000 lime-stable-1.0.1/src/lime/config.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)    31483 2024-05-03 20:18:23.000000 lime-stable-1.0.1/src/lime/io.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2795 2024-04-24 14:30:56.000000 lime-stable-1.0.1/src/lime/logo.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    38372 2024-04-29 17:41:51.000000 lime-stable-1.0.1/src/lime/model.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    73354 2024-05-01 22:06:07.000000 lime-stable-1.0.1/src/lime/observations.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    82220 2024-05-01 21:21:43.000000 lime-stable-1.0.1/src/lime/plots.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    70627 2024-04-29 17:28:58.000000 lime-stable-1.0.1/src/lime/plots_interactive.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    33579 2024-05-01 21:18:18.000000 lime-stable-1.0.1/src/lime/read_fits.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    24985 2024-05-01 23:08:37.000000 lime-stable-1.0.1/src/lime/recognition.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:09:01.453855 lime-stable-1.0.1/src/lime/resources/
--rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:04:12.000000 lime-stable-1.0.1/src/lime/resources/parent_bands.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:03:27.000000 lime-stable-1.0.1/src/lime/resources/parent_bands_BackUp.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    10111 2024-04-22 21:42:02.000000 lime-stable-1.0.1/src/lime/resources/types_params.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    14146 2024-04-25 13:02:58.000000 lime-stable-1.0.1/src/lime/tables.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    34912 2024-05-04 18:53:12.000000 lime-stable-1.0.1/src/lime/tools.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    29081 2024-04-25 14:14:19.000000 lime-stable-1.0.1/src/lime/transitions.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    37147 2024-04-29 02:03:22.000000 lime-stable-1.0.1/src/lime/workflow.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:09:01.453855 lime-stable-1.0.1/src/lime_stable.egg-info/
--rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-04 19:09:01.000000 lime-stable-1.0.1/src/lime_stable.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)      853 2024-05-04 19:09:01.000000 lime-stable-1.0.1/src/lime_stable.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-04 19:09:01.000000 lime-stable-1.0.1/src/lime_stable.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      252 2024-05-04 19:09:01.000000 lime-stable-1.0.1/src/lime_stable.egg-info/requires.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        5 2024-05-04 19:09:01.000000 lime-stable-1.0.1/src/lime_stable.egg-info/top_level.txt
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:09:01.453855 lime-stable-1.0.1/tests/
--rw-rw-r--   0 vital     (1000) vital     (1000)      994 2024-04-24 14:46:28.000000 lime-stable-1.0.1/tests/test_astro.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7088 2024-04-16 20:37:49.000000 lime-stable-1.0.1/tests/test_cube.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     3550 2024-04-24 14:46:41.000000 lime-stable-1.0.1/tests/test_io.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7795 2024-04-24 16:03:41.000000 lime-stable-1.0.1/tests/test_line.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4345 2024-04-25 13:05:21.000000 lime-stable-1.0.1/tests/test_model.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4624 2024-04-24 15:30:23.000000 lime-stable-1.0.1/tests/test_read_fits.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2013 2024-04-10 16:19:13.000000 lime-stable-1.0.1/tests/test_sample.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    11180 2024-04-24 14:43:43.000000 lime-stable-1.0.1/tests/test_spectrum.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    13391 2024-04-24 14:25:22.000000 lime-stable-1.0.1/tests/test_tools.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 05:04:03.705969 lime-stable-1.0.2/
+-rw-rw-r--   0 vital     (1000) vital     (1000)    35608 2024-04-25 13:12:45.000000 lime-stable-1.0.2/LICENSE.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)       63 2024-04-25 13:06:20.000000 lime-stable-1.0.2/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-09 05:04:03.705969 lime-stable-1.0.2/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2647 2024-04-25 13:09:22.000000 lime-stable-1.0.2/README.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1148 2024-05-09 04:48:30.000000 lime-stable-1.0.2/pyproject.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      433 2024-05-09 05:04:03.705969 lime-stable-1.0.2/setup.cfg
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1187 2024-04-25 13:12:39.000000 lime-stable-1.0.2/setup.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 05:04:03.701969 lime-stable-1.0.2/src/
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 05:04:03.701969 lime-stable-1.0.2/src/lime/
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1307 2024-04-25 21:14:21.000000 lime-stable-1.0.2/src/lime/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    31483 2024-05-03 20:18:23.000000 lime-stable-1.0.2/src/lime/io.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2795 2024-04-24 14:30:56.000000 lime-stable-1.0.2/src/lime/logo.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    38372 2024-04-29 17:41:51.000000 lime-stable-1.0.2/src/lime/model.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    73354 2024-05-01 22:06:07.000000 lime-stable-1.0.2/src/lime/observations.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    82241 2024-05-06 01:21:46.000000 lime-stable-1.0.2/src/lime/plots.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    70627 2024-04-29 17:28:58.000000 lime-stable-1.0.2/src/lime/plots_interactive.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    33847 2024-05-08 16:58:08.000000 lime-stable-1.0.2/src/lime/read_fits.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    24985 2024-05-01 23:08:37.000000 lime-stable-1.0.2/src/lime/recognition.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 05:04:03.701969 lime-stable-1.0.2/src/lime/resources/
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:04:12.000000 lime-stable-1.0.2/src/lime/resources/parent_bands.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:03:27.000000 lime-stable-1.0.2/src/lime/resources/parent_bands_BackUp.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10111 2024-04-22 21:42:02.000000 lime-stable-1.0.2/src/lime/resources/types_params.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    14146 2024-04-25 13:02:58.000000 lime-stable-1.0.2/src/lime/tables.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    34912 2024-05-04 18:53:12.000000 lime-stable-1.0.2/src/lime/tools.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    29081 2024-04-25 14:14:19.000000 lime-stable-1.0.2/src/lime/transitions.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    37147 2024-04-29 02:03:22.000000 lime-stable-1.0.2/src/lime/workflow.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 05:04:03.705969 lime-stable-1.0.2/src/lime_stable.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-09 05:04:03.000000 lime-stable-1.0.2/src/lime_stable.egg-info/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)      832 2024-05-09 05:04:03.000000 lime-stable-1.0.2/src/lime_stable.egg-info/SOURCES.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-09 05:04:03.000000 lime-stable-1.0.2/src/lime_stable.egg-info/dependency_links.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      252 2024-05-09 05:04:03.000000 lime-stable-1.0.2/src/lime_stable.egg-info/requires.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        5 2024-05-09 05:04:03.000000 lime-stable-1.0.2/src/lime_stable.egg-info/top_level.txt
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-09 05:04:03.705969 lime-stable-1.0.2/tests/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      994 2024-04-24 14:46:28.000000 lime-stable-1.0.2/tests/test_astro.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7088 2024-04-16 20:37:49.000000 lime-stable-1.0.2/tests/test_cube.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3550 2024-04-24 14:46:41.000000 lime-stable-1.0.2/tests/test_io.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7795 2024-04-24 16:03:41.000000 lime-stable-1.0.2/tests/test_line.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4345 2024-04-25 13:05:21.000000 lime-stable-1.0.2/tests/test_model.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4624 2024-04-24 15:30:23.000000 lime-stable-1.0.2/tests/test_read_fits.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2013 2024-04-10 16:19:13.000000 lime-stable-1.0.2/tests/test_sample.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    11180 2024-04-24 14:43:43.000000 lime-stable-1.0.2/tests/test_spectrum.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    13391 2024-04-24 14:25:22.000000 lime-stable-1.0.2/tests/test_tools.py
```

### Comparing `lime-stable-1.0.1/LICENSE.rst` & `lime-stable-1.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/PKG-INFO` & `lime-stable-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 1.0.1
+Version: 1.0.2
 Summary: Line measuring algorithm for astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lime-stable-1.0.1/README.rst` & `lime-stable-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/pyproject.toml` & `lime-stable-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lime-stable"
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "COPYING"}
 authors = [{name = "Vital Fernández", email = "vgf@umich.edu"}]
 description = "Line measuring algorithm for astronomical spectra"
 
 dependencies = ["asdf~=3.0",
```

### Comparing `lime-stable-1.0.1/setup.py` & `lime-stable-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/__init__.py` & `lime-stable-1.0.2/src/lime/__init__.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/io.py` & `lime-stable-1.0.2/src/lime/io.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/logo.py` & `lime-stable-1.0.2/src/lime/logo.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/model.py` & `lime-stable-1.0.2/src/lime/model.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/observations.py` & `lime-stable-1.0.2/src/lime/observations.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/plots.py` & `lime-stable-1.0.2/src/lime/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         return fig_conf
 
     def ax_defaults(self, user_ax, units_wave, units_flux, norm_flux, fig_type='default', **kwargs):
 
         # Default wavelength and flux
         if fig_type == 'default':
 
-            # Spectrum labels x-wavelegth, y-flux
+            # Spectrum labels x-wavelegth, y-flux # TODO without units
             x_label, y_label = spectrum_figure_labels(units_wave, units_flux, norm_flux)
             ax_cfg = {'xlabel': x_label, 'ylabel': y_label}
 
             # Update with the user configuration
             ax_cfg = ax_cfg if user_ax is None else {**ax_cfg, **user_ax}
 
         # Spatial cubes
```

### Comparing `lime-stable-1.0.1/src/lime/plots_interactive.py` & `lime-stable-1.0.2/src/lime/plots_interactive.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/read_fits.py` & `lime-stable-1.0.2/src/lime/read_fits.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,15 +538,15 @@
 
         # Spectrum properties
         params_dict = SPECTRUM_FITS_PARAMS['osiris']
 
         return wave_array, flux_array, err_array, header_list, params_dict
 
     @staticmethod
-    def sdss(fits_address, data_ext_list=(1, 2), hdr_ext_list=0, pixel_mask=None):
+    def sdss(fits_address, data_ext_list=(1, 2), hdr_ext_list=(0), pixel_mask=None):
 
         """
 
         This method returns the spectrum array data and headers from a SDSS observation.
 
         The function returns numpy arrays with the wavelength, flux and uncertainty flux (if available this is the
         standard deviation available), a list with the requested headers and a dictionary with the parameters to
@@ -565,27 +565,35 @@
         :return: wavelength array, flux array, uncertainty array, header list, observation parameter dict
 
         """
 
         # Get data table and header dict lists
         data_list, header_list = load_fits(fits_address, data_ext_list, hdr_ext_list, url_check=False)
 
-        # Re-construct spectrum arrays # TODO add error
+        # Re-construct spectrum arrays
         wave_array = 10.0 ** data_list[0]['loglam']
         flux_array = data_list[0]['flux']
         ivar_array = data_list[0]['ivar']
 
+        # Recover the redshift
+        try:
+            redshift = data_list[1]['Z'][0]
+        except:
+            redshift = None
+            _logger.warning(f'The SDSS redshift could not be read. ZWARNING = {data_list[1]["ZWARNING"]}')
+
         # Convert ivar = 0 to nan
         ivar_array[ivar_array == 0] = np.nan
 
         # Get standard deviation cube
         err_array = np.sqrt(1 / ivar_array)
 
         # Spectrum properties
         params_dict = SPECTRUM_FITS_PARAMS['sdss']
+        params_dict['redshift'] = redshift
 
         return wave_array, flux_array, err_array, header_list, params_dict
 
     @staticmethod
     def manga(fits_address, data_ext_list=('WAVE', 'FLUX', 'IVAR'), hdr_ext_list=('FLUX'), pixel_mask=None):
 
         """
```

### Comparing `lime-stable-1.0.1/src/lime/recognition.py` & `lime-stable-1.0.2/src/lime/recognition.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/resources/parent_bands.txt` & `lime-stable-1.0.2/src/lime/resources/parent_bands.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/resources/parent_bands_BackUp.txt` & `lime-stable-1.0.2/src/lime/resources/parent_bands_BackUp.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/resources/types_params.txt` & `lime-stable-1.0.2/src/lime/resources/types_params.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/tables.py` & `lime-stable-1.0.2/src/lime/tables.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/tools.py` & `lime-stable-1.0.2/src/lime/tools.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/transitions.py` & `lime-stable-1.0.2/src/lime/transitions.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime/workflow.py` & `lime-stable-1.0.2/src/lime/workflow.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/src/lime_stable.egg-info/PKG-INFO` & `lime-stable-1.0.2/src/lime_stable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 1.0.1
+Version: 1.0.2
 Summary: Line measuring algorithm for astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lime-stable-1.0.1/src/lime_stable.egg-info/SOURCES.txt` & `lime-stable-1.0.2/src/lime_stable.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE.rst
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 src/lime/__init__.py
-src/lime/config.toml
 src/lime/io.py
 src/lime/logo.py
 src/lime/model.py
 src/lime/observations.py
 src/lime/plots.py
 src/lime/plots_interactive.py
 src/lime/read_fits.py
```

### Comparing `lime-stable-1.0.1/tests/test_astro.py` & `lime-stable-1.0.2/tests/test_astro.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/tests/test_cube.py` & `lime-stable-1.0.2/tests/test_cube.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/tests/test_io.py` & `lime-stable-1.0.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/tests/test_line.py` & `lime-stable-1.0.2/tests/test_line.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/tests/test_model.py` & `lime-stable-1.0.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/tests/test_read_fits.py` & `lime-stable-1.0.2/tests/test_read_fits.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/tests/test_sample.py` & `lime-stable-1.0.2/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/tests/test_spectrum.py` & `lime-stable-1.0.2/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.1/tests/test_tools.py` & `lime-stable-1.0.2/tests/test_tools.py`

 * *Files identical despite different names*

