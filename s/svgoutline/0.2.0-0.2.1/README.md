# Comparing `tmp/svgoutline-0.2.0.tar.gz` & `tmp/svgoutline-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgoutline-0.2.0.tar", last modified: Mon Nov 27 08:47:42 2023, max compression
+gzip compressed data, was "svgoutline-0.2.1.tar", last modified: Thu May  9 07:07:52 2024, max compression
```

## Comparing `svgoutline-0.2.0.tar` & `svgoutline-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-11-27 08:47:42.632893 svgoutline-0.2.0/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     7653 2019-01-21 20:12:15.000000 svgoutline-0.2.0/LICENSE
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      832 2023-11-27 08:47:42.632893 svgoutline-0.2.0/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     4414 2023-11-27 08:43:30.000000 svgoutline-0.2.0/README.md
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2023-11-27 08:47:42.632893 svgoutline-0.2.0/setup.cfg
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1057 2023-11-17 16:13:05.000000 svgoutline-0.2.0/setup.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-11-27 08:47:42.629561 svgoutline-0.2.0/svgoutline/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      308 2019-01-21 20:12:16.000000 svgoutline-0.2.0/svgoutline/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    13699 2023-11-27 08:43:30.000000 svgoutline-0.2.0/svgoutline/outline_painter.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5037 2023-11-27 08:43:30.000000 svgoutline-0.2.0/svgoutline/svg_to_outlines.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     6136 2023-11-27 08:43:30.000000 svgoutline-0.2.0/svgoutline/svg_utils.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       22 2023-11-27 08:47:07.000000 svgoutline-0.2.0/svgoutline/version.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-11-27 08:47:42.632893 svgoutline-0.2.0/svgoutline.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      832 2023-11-27 08:47:42.000000 svgoutline-0.2.0/svgoutline.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      408 2023-11-27 08:47:42.000000 svgoutline-0.2.0/svgoutline.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2023-11-27 08:47:42.000000 svgoutline-0.2.0/svgoutline.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       15 2023-11-27 08:47:42.000000 svgoutline-0.2.0/svgoutline.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       11 2023-11-27 08:47:42.000000 svgoutline-0.2.0/svgoutline.egg-info/top_level.txt
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-11-27 08:47:42.632893 svgoutline-0.2.0/tests/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    13166 2023-11-27 08:43:30.000000 svgoutline-0.2.0/tests/test_outline_painter.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    15627 2023-11-27 08:43:30.000000 svgoutline-0.2.0/tests/test_svg_to_outlines.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    14035 2023-11-27 08:43:30.000000 svgoutline-0.2.0/tests/test_svg_utils.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-05-09 07:07:52.041584 svgoutline-0.2.1/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     7653 2019-01-21 20:12:15.000000 svgoutline-0.2.1/LICENSE
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      832 2024-05-09 07:07:52.041584 svgoutline-0.2.1/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     4414 2023-11-27 08:43:30.000000 svgoutline-0.2.1/README.md
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-05-09 07:07:52.041584 svgoutline-0.2.1/setup.cfg
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1057 2023-11-17 16:13:05.000000 svgoutline-0.2.1/setup.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-05-09 07:07:52.038251 svgoutline-0.2.1/svgoutline/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      308 2019-01-21 20:12:16.000000 svgoutline-0.2.1/svgoutline/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    13731 2024-05-09 06:49:57.000000 svgoutline-0.2.1/svgoutline/outline_painter.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5037 2023-11-27 08:43:30.000000 svgoutline-0.2.1/svgoutline/svg_to_outlines.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     6136 2023-11-27 08:43:30.000000 svgoutline-0.2.1/svgoutline/svg_utils.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       22 2024-05-09 07:03:24.000000 svgoutline-0.2.1/svgoutline/version.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-05-09 07:07:52.038251 svgoutline-0.2.1/svgoutline.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      832 2024-05-09 07:07:52.000000 svgoutline-0.2.1/svgoutline.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      408 2024-05-09 07:07:52.000000 svgoutline-0.2.1/svgoutline.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-05-09 07:07:52.000000 svgoutline-0.2.1/svgoutline.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       15 2024-05-09 07:07:52.000000 svgoutline-0.2.1/svgoutline.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       11 2024-05-09 07:07:52.000000 svgoutline-0.2.1/svgoutline.egg-info/top_level.txt
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-05-09 07:07:52.038251 svgoutline-0.2.1/tests/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    13166 2024-05-09 06:50:49.000000 svgoutline-0.2.1/tests/test_outline_painter.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    15627 2023-11-27 08:43:30.000000 svgoutline-0.2.1/tests/test_svg_to_outlines.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    14035 2023-11-27 08:43:30.000000 svgoutline-0.2.1/tests/test_svg_utils.py
```

### Comparing `svgoutline-0.2.0/LICENSE` & `svgoutline-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `svgoutline-0.2.0/PKG-INFO` & `svgoutline-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgoutline
-Version: 0.2.0
+Version: 0.2.1
 Summary: Convert SVG files (including text) into simple lines and curves for plotters.
 Home-page: https://github.com/mossblaser/svgoutline
 Author: Jonathan Heathcote
 License: LGPLv3
 Keywords: svg outline plotter cutter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `svgoutline-0.2.0/README.md` & `svgoutline-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `svgoutline-0.2.0/setup.py` & `svgoutline-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `svgoutline-0.2.0/svgoutline/outline_painter.py` & `svgoutline-0.2.1/svgoutline/outline_painter.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,10 +359,10 @@
         elif num == QPaintDevice.PdmPhysicalDpiX:
             return mm_per_inch * self._ppmm
         elif num == QPaintDevice.PdmPhysicalDpiY:
             return mm_per_inch * self._ppmm
         elif num == QPaintDevice.PdmDevicePixelRatio:
             return 1
         elif num == QPaintDevice.PdmDevicePixelRatioScaled:
-            return 1
+            return 1 * self.devicePixelRatioFScale()
         else:
             raise NotImplementedError("Unknown metric {}".format(num))
```

### Comparing `svgoutline-0.2.0/svgoutline/svg_to_outlines.py` & `svgoutline-0.2.1/svgoutline/svg_to_outlines.py`

 * *Files identical despite different names*

### Comparing `svgoutline-0.2.0/svgoutline/svg_utils.py` & `svgoutline-0.2.1/svgoutline/svg_utils.py`

 * *Files identical despite different names*

### Comparing `svgoutline-0.2.0/svgoutline.egg-info/PKG-INFO` & `svgoutline-0.2.1/svgoutline.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgoutline
-Version: 0.2.0
+Version: 0.2.1
 Summary: Convert SVG files (including text) into simple lines and curves for plotters.
 Home-page: https://github.com/mossblaser/svgoutline
 Author: Jonathan Heathcote
 License: LGPLv3
 Keywords: svg outline plotter cutter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `svgoutline-0.2.0/tests/test_outline_painter.py` & `svgoutline-0.2.1/tests/test_outline_painter.py`

 * *Files identical despite different names*

### Comparing `svgoutline-0.2.0/tests/test_svg_to_outlines.py` & `svgoutline-0.2.1/tests/test_svg_to_outlines.py`

 * *Files identical despite different names*

### Comparing `svgoutline-0.2.0/tests/test_svg_utils.py` & `svgoutline-0.2.1/tests/test_svg_utils.py`

 * *Files identical despite different names*

