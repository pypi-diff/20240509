# Comparing `tmp/sufi-1.0.2.3.tar.gz` & `tmp/sufi-1.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sufi-1.0.2.3.tar", last modified: Wed May  8 23:28:11 2024, max compression
+gzip compressed data, was "sufi-1.0.2.4.tar", last modified: Wed May  8 23:42:18 2024, max compression
```

## Comparing `sufi-1.0.2.3.tar` & `sufi-1.0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:28:11.193495 sufi-1.0.2.3/
--rw-r--r--   0 sunny      (501) staff       (20)     1067 2024-05-02 00:31:02.000000 sufi-1.0.2.3/LICENCE
--rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-08 23:28:11.193314 sufi-1.0.2.3/PKG-INFO
--rw-r--r--   0 sunny      (501) staff       (20)     1798 2024-05-02 00:31:02.000000 sufi-1.0.2.3/README.md
--rw-r--r--   0 sunny      (501) staff       (20)       38 2024-05-08 23:28:11.193561 sufi-1.0.2.3/setup.cfg
--rw-r--r--   0 sunny      (501) staff       (20)      607 2024-05-08 23:27:33.000000 sufi-1.0.2.3/setup.py
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:28:11.191515 sufi-1.0.2.3/sufi/
--rw-r--r--   0 sunny      (501) staff       (20)        2 2024-05-02 00:31:02.000000 sufi-1.0.2.3/sufi/__init__.py
--rw-r--r--   0 sunny      (501) staff       (20)     7085 2024-05-08 22:53:19.000000 sufi-1.0.2.3/sufi/filters.py
--rw-r--r--   0 sunny      (501) staff       (20)   209989 2024-05-08 17:58:28.000000 sufi-1.0.2.3/sufi/pentagram.png
--rw-r--r--   0 sunny      (501) staff       (20)    48339 2023-03-10 20:10:30.000000 sufi-1.0.2.3/sufi/red.png
--rw-r--r--   0 sunny      (501) staff       (20)  1889093 2024-05-05 19:22:41.000000 sufi-1.0.2.3/sufi/shield.png
--rw-r--r--   0 sunny      (501) staff       (20)     4115 2024-05-08 22:41:40.000000 sufi-1.0.2.3/sufi/utility.py
--rw-r--r--   0 sunny      (501) staff       (20)     4926 2024-05-02 00:35:11.000000 sufi-1.0.2.3/sufi/videoProcessing.py
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:28:11.193093 sufi-1.0.2.3/sufi.egg-info/
--rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-08 23:28:11.000000 sufi-1.0.2.3/sufi.egg-info/PKG-INFO
--rw-r--r--   0 sunny      (501) staff       (20)      286 2024-05-08 23:28:11.000000 sufi-1.0.2.3/sufi.egg-info/SOURCES.txt
--rw-r--r--   0 sunny      (501) staff       (20)        1 2024-05-08 23:28:11.000000 sufi-1.0.2.3/sufi.egg-info/dependency_links.txt
--rw-r--r--   0 sunny      (501) staff       (20)       46 2024-05-08 23:28:11.000000 sufi-1.0.2.3/sufi.egg-info/requires.txt
--rw-r--r--   0 sunny      (501) staff       (20)        5 2024-05-08 23:28:11.000000 sufi-1.0.2.3/sufi.egg-info/top_level.txt
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:42:18.299090 sufi-1.0.2.4/
+-rw-r--r--   0 sunny      (501) staff       (20)     1067 2024-05-02 00:31:02.000000 sufi-1.0.2.4/LICENCE
+-rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-08 23:42:18.298950 sufi-1.0.2.4/PKG-INFO
+-rw-r--r--   0 sunny      (501) staff       (20)     1798 2024-05-02 00:31:02.000000 sufi-1.0.2.4/README.md
+-rw-r--r--   0 sunny      (501) staff       (20)       38 2024-05-08 23:42:18.299153 sufi-1.0.2.4/setup.cfg
+-rw-r--r--   0 sunny      (501) staff       (20)      607 2024-05-08 23:41:53.000000 sufi-1.0.2.4/setup.py
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:42:18.297033 sufi-1.0.2.4/sufi/
+-rw-r--r--   0 sunny      (501) staff       (20)        2 2024-05-02 00:31:02.000000 sufi-1.0.2.4/sufi/__init__.py
+-rw-r--r--   0 sunny      (501) staff       (20)     7098 2024-05-08 23:41:46.000000 sufi-1.0.2.4/sufi/filters.py
+-rw-r--r--   0 sunny      (501) staff       (20)   209989 2024-05-08 17:58:28.000000 sufi-1.0.2.4/sufi/pentagram.png
+-rw-r--r--   0 sunny      (501) staff       (20)    48339 2023-03-10 20:10:30.000000 sufi-1.0.2.4/sufi/red.png
+-rw-r--r--   0 sunny      (501) staff       (20)  1889093 2024-05-05 19:22:41.000000 sufi-1.0.2.4/sufi/shield.png
+-rw-r--r--   0 sunny      (501) staff       (20)     4115 2024-05-08 22:41:40.000000 sufi-1.0.2.4/sufi/utility.py
+-rw-r--r--   0 sunny      (501) staff       (20)     4926 2024-05-02 00:35:11.000000 sufi-1.0.2.4/sufi/videoProcessing.py
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:42:18.298496 sufi-1.0.2.4/sufi.egg-info/
+-rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-08 23:42:18.000000 sufi-1.0.2.4/sufi.egg-info/PKG-INFO
+-rw-r--r--   0 sunny      (501) staff       (20)      286 2024-05-08 23:42:18.000000 sufi-1.0.2.4/sufi.egg-info/SOURCES.txt
+-rw-r--r--   0 sunny      (501) staff       (20)        1 2024-05-08 23:42:18.000000 sufi-1.0.2.4/sufi.egg-info/dependency_links.txt
+-rw-r--r--   0 sunny      (501) staff       (20)       46 2024-05-08 23:42:18.000000 sufi-1.0.2.4/sufi.egg-info/requires.txt
+-rw-r--r--   0 sunny      (501) staff       (20)        5 2024-05-08 23:42:18.000000 sufi-1.0.2.4/sufi.egg-info/top_level.txt
```

### Comparing `sufi-1.0.2.3/LICENCE` & `sufi-1.0.2.4/LICENCE`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.3/PKG-INFO` & `sufi-1.0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sufi
-Version: 1.0.2.3
+Version: 1.0.2.4
 Summary: apply different types of filters on image
 Home-page: https://github.com/sunnykumar1516/sufi
 Author: sunny kumar
 Author-email: sunnykumar1516@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sufi-1.0.2.3/README.md` & `sufi-1.0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.3/setup.py` & `sufi-1.0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	description = fh.read()
 
 setuptools.setup(
 	name="sufi",
-	version="1.0.2.3",
+	version="1.0.2.4",
 	author="sunny kumar",
 	author_email="sunnykumar1516@gmail.com",
 	packages=["sufi"],
 	description="apply different types of filters on image",
 	long_description=description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/sunnykumar1516/sufi",
```

### Comparing `sufi-1.0.2.3/sufi/filters.py` & `sufi-1.0.2.4/sufi/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,20 +74,21 @@
 
 
 mp_pose = mp.solutions.hands
 mp_drawing = mp.solutions.drawing_utils
 mp_drawing_styles = mp.solutions.drawing_styles
 mp_hands = mp.solutions.hands
 hands = mp_pose.Hands()
-circle = cv.imread("red.png", -1)
-full_circle = cv.imread("pentagram.png", -1)
-shield = cv.imread("shield.png", -1)
+
 
 
 def apply_spell():
+    circle = cv.imread("red.png", -1)
+    full_circle = cv.imread("pentagram.png", -1)
+    shield = cv.imread("shield.png", -1)
     rotation = 0
     
     cap = cv.VideoCapture(0)
     cap.set(3, 1280)
     cap.set(4, 720)
     while cap.isOpened():
         size = (300, 300)
```

### Comparing `sufi-1.0.2.3/sufi/pentagram.png` & `sufi-1.0.2.4/sufi/pentagram.png`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.3/sufi/red.png` & `sufi-1.0.2.4/sufi/red.png`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.3/sufi/shield.png` & `sufi-1.0.2.4/sufi/shield.png`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.3/sufi/utility.py` & `sufi-1.0.2.4/sufi/utility.py`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.3/sufi/videoProcessing.py` & `sufi-1.0.2.4/sufi/videoProcessing.py`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.3/sufi.egg-info/PKG-INFO` & `sufi-1.0.2.4/sufi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sufi
-Version: 1.0.2.3
+Version: 1.0.2.4
 Summary: apply different types of filters on image
 Home-page: https://github.com/sunnykumar1516/sufi
 Author: sunny kumar
 Author-email: sunnykumar1516@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

