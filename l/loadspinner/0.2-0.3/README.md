# Comparing `tmp/loadspinner-0.2.tar.gz` & `tmp/loadspinner-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadspinner-0.2.tar", last modified: Wed May  1 18:05:56 2024, max compression
+gzip compressed data, was "loadspinner-0.3.tar", last modified: Wed May  8 23:06:54 2024, max compression
```

## Comparing `loadspinner-0.2.tar` & `loadspinner-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-01 18:05:56.926883 loadspinner-0.2/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1061 2024-05-01 16:53:43.000000 loadspinner-0.2/LICENSE
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1384 2024-05-01 18:05:56.925882 loadspinner-0.2/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      649 2024-05-01 17:50:10.000000 loadspinner-0.2/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-01 18:05:56.925882 loadspinner-0.2/loadspinner/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2907 2024-05-01 15:29:43.000000 loadspinner-0.2/loadspinner/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     4792 2024-05-01 18:05:46.000000 loadspinner-0.2/loadspinner/_spinners.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-01 18:05:56.925882 loadspinner-0.2/loadspinner/tools/
--rw-r--r--   0 xyz       (1000) xyz       (1000)      476 2024-04-29 18:02:17.000000 loadspinner-0.2/loadspinner/tools/demo.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      283 2024-05-01 10:45:26.000000 loadspinner-0.2/loadspinner/tools/preview.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-01 18:05:56.925882 loadspinner-0.2/loadspinner.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1384 2024-05-01 18:05:56.000000 loadspinner-0.2/loadspinner.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      270 2024-05-01 18:05:56.000000 loadspinner-0.2/loadspinner.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-01 18:05:56.000000 loadspinner-0.2/loadspinner.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       12 2024-05-01 18:05:56.000000 loadspinner-0.2/loadspinner.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-01 18:05:56.926883 loadspinner-0.2/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1060 2024-05-01 07:28:17.000000 loadspinner-0.2/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-08 23:06:54.643984 loadspinner-0.3/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1061 2024-05-01 16:53:43.000000 loadspinner-0.3/LICENSE
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1384 2024-05-08 23:06:54.643984 loadspinner-0.3/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      649 2024-05-01 17:50:10.000000 loadspinner-0.3/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-08 23:06:54.642984 loadspinner-0.3/loadspinner/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2907 2024-05-08 03:58:58.000000 loadspinner-0.3/loadspinner/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     5635 2024-05-08 06:08:01.000000 loadspinner-0.3/loadspinner/_spinners.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-08 23:06:54.643984 loadspinner-0.3/loadspinner/tools/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      476 2024-04-29 18:02:17.000000 loadspinner-0.3/loadspinner/tools/demo.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      284 2024-05-08 23:02:02.000000 loadspinner-0.3/loadspinner/tools/preview.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-08 23:06:54.643984 loadspinner-0.3/loadspinner.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1384 2024-05-08 23:06:54.000000 loadspinner-0.3/loadspinner.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      270 2024-05-08 23:06:54.000000 loadspinner-0.3/loadspinner.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-08 23:06:54.000000 loadspinner-0.3/loadspinner.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       12 2024-05-08 23:06:54.000000 loadspinner-0.3/loadspinner.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-08 23:06:54.643984 loadspinner-0.3/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1060 2024-05-01 07:28:17.000000 loadspinner-0.3/setup.py
```

### Comparing `loadspinner-0.2/LICENSE` & `loadspinner-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loadspinner-0.2/PKG-INFO` & `loadspinner-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadspinner
-Version: 0.2
+Version: 0.3
 Summary: a CLI based loading spinner.
 Home-page: https://github.com/xyzpw/loadspinner/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: loading,loader,progress,throbber,spinner
 Classifier: Programming Language :: Python :: 3
```

### Comparing `loadspinner-0.2/README.md` & `loadspinner-0.3/README.md`

 * *Files identical despite different names*

### Comparing `loadspinner-0.2/loadspinner/__init__.py` & `loadspinner-0.3/loadspinner/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from time import time as getEpoch
 import multiprocessing
 
 __all__ = [
     "Spinner",
 ]
 
-__version__ = "0.2"
+__version__ = "0.3"
 __description__ = "a CLI based loading spinner."
 __author__ = "xyzpw"
 __license__ = "MIT"
 
 class Spinner:
     def __init__(self, spinner_type: str = "classic"):
         self.spinner_type = spinner_type
```

### Comparing `loadspinner-0.2/loadspinner/_spinners.py` & `loadspinner-0.3/loadspinner/_spinners.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
             "   ",
             ".  ",
             ".. ",
             "...",
         ],
         "interval": 1/4,
     },
-    "spinner": {
+    "slash": {
         "frames": ["|", "/", "\u2013", "\\"],
         "interval": 0.5/4,
     },
     "balloon": {
         "frames": [" ", ".", "o", "O", "*", " "],
         "interval": 1.5/6,
     },
@@ -133,14 +133,29 @@
         currentFrame += walls[1]
         frames.append(currentFrame)
     _frames = reversed(frames)
     for _ in _frames:
         frames.append(_)
     return frames
 
+def generateNewtonsCradle(character: str = "\u25cf", walls: tuple = ("|", "|")):
+    frames = []
+    for i in range(5, -1, -1):
+        currentFrame = f"{walls[0]}{' '*i}{character}{' '*(5-i)}{character*4}{' '*5}{walls[1]}"
+        frames.append(currentFrame)
+    for i in range(1, 6):
+        currentFrame = f"{walls[0]}{' '*i}{character}{' '*(5-i)}{character*4}{' '*5}{walls[1]}"
+        frames.append(currentFrame)
+    for i in range(1, 6):
+        currentFrame = f"{walls[0]}{' '*5}{character*4}{' '*i}{character}{' '*(5-i)}{walls[1]}"
+        frames.append(currentFrame)
+    for i in range(4, 0, -1):
+        currentFrame = f"{walls[0]}{' '*5}{character*4}{' '*i}{character}{' '*(5-i)}{walls[1]}"
+        frames.append(currentFrame)
+    return frames
 
 all_spinners["bouncingCircles"] = {
     "frames": generateBounceSpinner("\u25CF", ("(", ")")),
     "interval": 1.5/10,
 }
 all_spinners["bouncingBars"] = {
     "frames": generateBounceSpinner("=", ("[", "]")),
@@ -158,7 +173,11 @@
     "frames": generateSingleCharacterBounceSpinner("=", ("[", "]")),
     "interval": 3/50,
 }
 all_spinners["bouncingHeart"] = {
     "frames": generateSingleCharacterBounceSpinner("\u2665", ("|", "|")),
     "interval": 3/50,
 }
+all_spinners["newton"] = {
+    "frames": generateNewtonsCradle(),
+    "interval": 1/20,
+}
```

### Comparing `loadspinner-0.2/loadspinner.egg-info/PKG-INFO` & `loadspinner-0.3/loadspinner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadspinner
-Version: 0.2
+Version: 0.3
 Summary: a CLI based loading spinner.
 Home-page: https://github.com/xyzpw/loadspinner/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: loading,loader,progress,throbber,spinner
 Classifier: Programming Language :: Python :: 3
```

### Comparing `loadspinner-0.2/setup.py` & `loadspinner-0.3/setup.py`

 * *Files identical despite different names*

