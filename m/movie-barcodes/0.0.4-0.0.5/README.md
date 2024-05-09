# Comparing `tmp/movie-barcodes-0.0.4.tar.gz` & `tmp/movie-barcodes-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movie-barcodes-0.0.4.tar", last modified: Wed May  8 14:57:42 2024, max compression
+gzip compressed data, was "movie-barcodes-0.0.5.tar", last modified: Thu May  9 09:41:22 2024, max compression
```

## Comparing `movie-barcodes-0.0.4.tar` & `movie-barcodes-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:57:42.442002 movie-barcodes-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-08 14:57:42.442002 movie-barcodes-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:57:42.442002 movie-barcodes-0.0.4/movie_barcodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-08 14:57:42.000000 movie-barcodes-0.0.4/movie_barcodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 14:57:42.000000 movie-barcodes-0.0.4/movie_barcodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:57:42.000000 movie-barcodes-0.0.4/movie_barcodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 14:57:42.000000 movie-barcodes-0.0.4/movie_barcodes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 14:57:42.000000 movie-barcodes-0.0.4/movie_barcodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 14:57:42.000000 movie-barcodes-0.0.4/movie_barcodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 14:57:42.442002 movie-barcodes-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:57:42.442002 movie-barcodes-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/src/barcode_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/src/color_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/src/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/src/video_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:57:42.442002 movie-barcodes-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/tests/test_barcode_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/tests/test_color_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/tests/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/tests/test_video_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:41:22.749369 movie-barcodes-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-09 09:41:22.749369 movie-barcodes-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:41:22.745369 movie-barcodes-0.0.5/movie_barcodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-09 09:41:22.000000 movie-barcodes-0.0.5/movie_barcodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 09:41:22.000000 movie-barcodes-0.0.5/movie_barcodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:41:22.000000 movie-barcodes-0.0.5/movie_barcodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 09:41:22.000000 movie-barcodes-0.0.5/movie_barcodes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 09:41:22.000000 movie-barcodes-0.0.5/movie_barcodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 09:41:22.000000 movie-barcodes-0.0.5/movie_barcodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-09 09:41:22.749369 movie-barcodes-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:41:22.745369 movie-barcodes-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/src/barcode_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/src/color_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/src/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/src/video_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:41:22.749369 movie-barcodes-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/tests/test_barcode_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/tests/test_color_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-05-09 09:41:04.000000 movie-barcodes-0.0.5/tests/test_video_processing.py
```

### Comparing `movie-barcodes-0.0.4/LICENSE` & `movie-barcodes-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.4/PKG-INFO` & `movie-barcodes-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movie-barcodes
-Version: 0.0.4
+Version: 0.0.5
 Summary: Compress every frame of a movie in a single color barcode.Transform entire movies into stunning single-barcode visualizations.Capture the essence of cinematic storytelling through dominant color extraction from each frame.
 Home-page: https://github.com/Wazzabeee/movie-barcodes
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
@@ -17,16 +17,21 @@
 # Movie Barcodes
 The Lodger: A Story of the London Fog (1927) - Alfred Hitchcock - [Public Domain](https://archive.org/details/TheLodgerAStoryOfTheLondonFog_579)
 
 Circular Barcode           |  Horizontal Barcode
 :-------------------------:|:-------------------------:
 ![](https://github.com/Wazzabeee/movie_color_barcode/blob/main/examples/thelodgerastoryofthelondonfog_circular.png?raw=true)  |  ![](https://github.com/Wazzabeee/movie_color_barcode/blob/main/examples/thelodgerastoryofthelondonfog_horizontal.png?raw=true)
 
-![PyPI - Version](https://img.shields.io/pypi/v/movie-barcodes) ![PyPI - License](https://img.shields.io/pypi/l/movie-barcodes)
+![PyPI - Version](https://img.shields.io/pypi/v/movie-barcodes)
+![PyPI - License](https://img.shields.io/pypi/l/movie-barcodes)
 ![Python](https://img.shields.io/badge/python-3.11-blue)
+![Status](https://img.shields.io/pypi/status/movie-barcodes.svg)
+![Codecov](https://codecov.io/gh/Wazzabeee/movie-barcodes/branch/main/graph/badge.svg)
+![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
+![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # Overview
 
 Compress every frame of a movie in a single color barcode.
 
 This project is a robust and highly configurable utility designed to extract dominant colors from video files and generate color barcodes. Built with Python and OpenCV, the tool offers multiple algorithms for color extraction, including average color, K-means clustering, and HSV/BGR histograms. The output can be generated in various forms, like horizontal and circular barcodes, providing a visually intuitive summary of the color distribution in the video.
```

### Comparing `movie-barcodes-0.0.4/README.md` & `movie-barcodes-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # Movie Barcodes
 The Lodger: A Story of the London Fog (1927) - Alfred Hitchcock - [Public Domain](https://archive.org/details/TheLodgerAStoryOfTheLondonFog_579)
 
 Circular Barcode           |  Horizontal Barcode
 :-------------------------:|:-------------------------:
 ![](https://github.com/Wazzabeee/movie_color_barcode/blob/main/examples/thelodgerastoryofthelondonfog_circular.png?raw=true)  |  ![](https://github.com/Wazzabeee/movie_color_barcode/blob/main/examples/thelodgerastoryofthelondonfog_horizontal.png?raw=true)
 
-![PyPI - Version](https://img.shields.io/pypi/v/movie-barcodes) ![PyPI - License](https://img.shields.io/pypi/l/movie-barcodes)
+![PyPI - Version](https://img.shields.io/pypi/v/movie-barcodes)
+![PyPI - License](https://img.shields.io/pypi/l/movie-barcodes)
 ![Python](https://img.shields.io/badge/python-3.11-blue)
+![Status](https://img.shields.io/pypi/status/movie-barcodes.svg)
+![Codecov](https://codecov.io/gh/Wazzabeee/movie-barcodes/branch/main/graph/badge.svg)
+![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
+![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # Overview
 
 Compress every frame of a movie in a single color barcode.
 
 This project is a robust and highly configurable utility designed to extract dominant colors from video files and generate color barcodes. Built with Python and OpenCV, the tool offers multiple algorithms for color extraction, including average color, K-means clustering, and HSV/BGR histograms. The output can be generated in various forms, like horizontal and circular barcodes, providing a visually intuitive summary of the color distribution in the video.
```

### Comparing `movie-barcodes-0.0.4/movie_barcodes.egg-info/PKG-INFO` & `movie-barcodes-0.0.5/movie_barcodes.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movie-barcodes
-Version: 0.0.4
+Version: 0.0.5
 Summary: Compress every frame of a movie in a single color barcode.Transform entire movies into stunning single-barcode visualizations.Capture the essence of cinematic storytelling through dominant color extraction from each frame.
 Home-page: https://github.com/Wazzabeee/movie-barcodes
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
@@ -17,16 +17,21 @@
 # Movie Barcodes
 The Lodger: A Story of the London Fog (1927) - Alfred Hitchcock - [Public Domain](https://archive.org/details/TheLodgerAStoryOfTheLondonFog_579)
 
 Circular Barcode           |  Horizontal Barcode
 :-------------------------:|:-------------------------:
 ![](https://github.com/Wazzabeee/movie_color_barcode/blob/main/examples/thelodgerastoryofthelondonfog_circular.png?raw=true)  |  ![](https://github.com/Wazzabeee/movie_color_barcode/blob/main/examples/thelodgerastoryofthelondonfog_horizontal.png?raw=true)
 
-![PyPI - Version](https://img.shields.io/pypi/v/movie-barcodes) ![PyPI - License](https://img.shields.io/pypi/l/movie-barcodes)
+![PyPI - Version](https://img.shields.io/pypi/v/movie-barcodes)
+![PyPI - License](https://img.shields.io/pypi/l/movie-barcodes)
 ![Python](https://img.shields.io/badge/python-3.11-blue)
+![Status](https://img.shields.io/pypi/status/movie-barcodes.svg)
+![Codecov](https://codecov.io/gh/Wazzabeee/movie-barcodes/branch/main/graph/badge.svg)
+![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
+![Black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # Overview
 
 Compress every frame of a movie in a single color barcode.
 
 This project is a robust and highly configurable utility designed to extract dominant colors from video files and generate color barcodes. Built with Python and OpenCV, the tool offers multiple algorithms for color extraction, including average color, K-means clustering, and HSV/BGR histograms. The output can be generated in various forms, like horizontal and circular barcodes, providing a visually intuitive summary of the color distribution in the video.
```

### Comparing `movie-barcodes-0.0.4/movie_barcodes.egg-info/SOURCES.txt` & `movie-barcodes-0.0.5/movie_barcodes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.4/setup.py` & `movie-barcodes-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.4/src/barcode_generation.py` & `movie-barcodes-0.0.5/src/barcode_generation.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.4/src/color_extraction.py` & `movie-barcodes-0.0.5/src/color_extraction.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.4/src/main.py` & `movie-barcodes-0.0.5/src/main.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.4/src/utility.py` & `movie-barcodes-0.0.5/src/utility.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.4/src/video_processing.py` & `movie-barcodes-0.0.5/src/video_processing.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.4/tests/test_barcode_generation.py` & `movie-barcodes-0.0.5/tests/test_barcode_generation.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.4/tests/test_color_extraction.py` & `movie-barcodes-0.0.5/tests/test_color_extraction.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.4/tests/test_integration.py` & `movie-barcodes-0.0.5/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.4/tests/test_utility.py` & `movie-barcodes-0.0.5/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.4/tests/test_video_processing.py` & `movie-barcodes-0.0.5/tests/test_video_processing.py`

 * *Files identical despite different names*

