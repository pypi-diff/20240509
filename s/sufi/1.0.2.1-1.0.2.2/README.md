# Comparing `tmp/sufi-1.0.2.1.tar.gz` & `tmp/sufi-1.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sufi-1.0.2.1.tar", last modified: Wed May  1 15:36:30 2024, max compression
+gzip compressed data, was "sufi-1.0.2.2.tar", last modified: Wed May  8 23:04:19 2024, max compression
```

## Comparing `sufi-1.0.2.1.tar` & `sufi-1.0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-01 15:36:30.170818 sufi-1.0.2.1/
--rw-r--r--   0 sunny      (501) staff       (20)     1067 2024-04-30 20:35:03.000000 sufi-1.0.2.1/LICENCE
--rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-01 15:36:30.170641 sufi-1.0.2.1/PKG-INFO
--rw-r--r--   0 sunny      (501) staff       (20)     1798 2024-05-01 15:34:14.000000 sufi-1.0.2.1/README.md
--rw-r--r--   0 sunny      (501) staff       (20)       38 2024-05-01 15:36:30.170871 sufi-1.0.2.1/setup.cfg
--rw-r--r--   0 sunny      (501) staff       (20)      522 2024-05-01 15:36:24.000000 sufi-1.0.2.1/setup.py
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-01 15:36:30.168027 sufi-1.0.2.1/sufi/
--rw-r--r--   0 sunny      (501) staff       (20)        2 2024-04-30 20:26:41.000000 sufi-1.0.2.1/sufi/__init__.py
--rw-r--r--   0 sunny      (501) staff       (20)     1926 2024-05-01 15:34:30.000000 sufi-1.0.2.1/sufi/filters.py
--rw-r--r--   0 sunny      (501) staff       (20)     2532 2024-04-30 23:07:19.000000 sufi-1.0.2.1/sufi/utility.py
--rw-r--r--   0 sunny      (501) staff       (20)     4856 2024-05-01 13:42:40.000000 sufi-1.0.2.1/sufi/videoProcessing.py
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-01 15:36:30.170086 sufi-1.0.2.1/sufi.egg-info/
--rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-01 15:36:30.000000 sufi-1.0.2.1/sufi.egg-info/PKG-INFO
--rw-r--r--   0 sunny      (501) staff       (20)      238 2024-05-01 15:36:30.000000 sufi-1.0.2.1/sufi.egg-info/SOURCES.txt
--rw-r--r--   0 sunny      (501) staff       (20)        1 2024-05-01 15:36:30.000000 sufi-1.0.2.1/sufi.egg-info/dependency_links.txt
--rw-r--r--   0 sunny      (501) staff       (20)       28 2024-05-01 15:36:30.000000 sufi-1.0.2.1/sufi.egg-info/requires.txt
--rw-r--r--   0 sunny      (501) staff       (20)        5 2024-05-01 15:36:30.000000 sufi-1.0.2.1/sufi.egg-info/top_level.txt
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:04:19.045965 sufi-1.0.2.2/
+-rw-r--r--   0 sunny      (501) staff       (20)     1067 2024-05-02 00:31:02.000000 sufi-1.0.2.2/LICENCE
+-rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-08 23:04:19.045844 sufi-1.0.2.2/PKG-INFO
+-rw-r--r--   0 sunny      (501) staff       (20)     1798 2024-05-02 00:31:02.000000 sufi-1.0.2.2/README.md
+-rw-r--r--   0 sunny      (501) staff       (20)       38 2024-05-08 23:04:19.046011 sufi-1.0.2.2/setup.cfg
+-rw-r--r--   0 sunny      (501) staff       (20)      547 2024-05-08 23:03:54.000000 sufi-1.0.2.2/setup.py
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:04:19.044891 sufi-1.0.2.2/sufi/
+-rw-r--r--   0 sunny      (501) staff       (20)        2 2024-05-02 00:31:02.000000 sufi-1.0.2.2/sufi/__init__.py
+-rw-r--r--   0 sunny      (501) staff       (20)     7085 2024-05-08 22:53:19.000000 sufi-1.0.2.2/sufi/filters.py
+-rw-r--r--   0 sunny      (501) staff       (20)     4115 2024-05-08 22:41:40.000000 sufi-1.0.2.2/sufi/utility.py
+-rw-r--r--   0 sunny      (501) staff       (20)     4926 2024-05-02 00:35:11.000000 sufi-1.0.2.2/sufi/videoProcessing.py
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:04:19.045684 sufi-1.0.2.2/sufi.egg-info/
+-rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-08 23:04:19.000000 sufi-1.0.2.2/sufi.egg-info/PKG-INFO
+-rw-r--r--   0 sunny      (501) staff       (20)      238 2024-05-08 23:04:19.000000 sufi-1.0.2.2/sufi.egg-info/SOURCES.txt
+-rw-r--r--   0 sunny      (501) staff       (20)        1 2024-05-08 23:04:19.000000 sufi-1.0.2.2/sufi.egg-info/dependency_links.txt
+-rw-r--r--   0 sunny      (501) staff       (20)       46 2024-05-08 23:04:19.000000 sufi-1.0.2.2/sufi.egg-info/requires.txt
+-rw-r--r--   0 sunny      (501) staff       (20)        5 2024-05-08 23:04:19.000000 sufi-1.0.2.2/sufi.egg-info/top_level.txt
```

### Comparing `sufi-1.0.2.1/LICENCE` & `sufi-1.0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.1/PKG-INFO` & `sufi-1.0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sufi
-Version: 1.0.2.1
+Version: 1.0.2.2
 Summary: apply different types of filters on image
 Home-page: https://github.com/sunnykumar1516/sufi
 Author: sunny kumar
 Author-email: sunnykumar1516@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sufi-1.0.2.1/README.md` & `sufi-1.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.1/setup.py` & `sufi-1.0.2.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	description = fh.read()
 
 setuptools.setup(
 	name="sufi",
-	version="1.0.2.1",
+	version="1.0.2.2",
 	author="sunny kumar",
 	author_email="sunnykumar1516@gmail.com",
 	packages=["sufi"],
 	description="apply different types of filters on image",
 	long_description=description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/sunnykumar1516/sufi",
 	license='MIT',
 	python_requires='>=3.8',
 	install_requires=[
         'numpy>= 1.2',
-        'opencv-python>=4'
+        'opencv-python>=4',
+		'mediapipe == 0.10.5'
 
     ]
 )
```

### Comparing `sufi-1.0.2.1/sufi/videoProcessing.py` & `sufi-1.0.2.2/sufi/videoProcessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import cv2 as cv
 import numpy as np
 
-
+# adding constant values
 vignette_filter_level = 9
 blur_filter_kernel = 5
 HDR_filter_sigma_s = 10
 HDR_filter_sigma_r = 0.2
 sharpening_filter_K = 9
 digital_art_filter_sigma_s = 10
 digital_art_filter_sigma_r = 0.3
 digital_art_filter_blur = 7
 sketch_filter_blur = 5
 canny_filter_lw = 100
 canny_filter_up = 120
 bright_filter_level = 3
 
 
+#display image function
 def display_image_at_path(path):
     img = cv.imread(path)
     cv.imshow("img", img)
     cv.waitKey(0)
 
+# save image function
 def save_image(img=None,filename="test.jpg"):
     cv.imwrite(filename, img)
 
 def display_image(img):
     cv.imshow("img", img)
     cv.waitKey(0)
```

### Comparing `sufi-1.0.2.1/sufi.egg-info/PKG-INFO` & `sufi-1.0.2.2/sufi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sufi
-Version: 1.0.2.1
+Version: 1.0.2.2
 Summary: apply different types of filters on image
 Home-page: https://github.com/sunnykumar1516/sufi
 Author: sunny kumar
 Author-email: sunnykumar1516@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

