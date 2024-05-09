# Comparing `tmp/sufi-1.0.2.5.tar.gz` & `tmp/sufi-1.0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sufi-1.0.2.5.tar", last modified: Thu May  9 12:55:04 2024, max compression
+gzip compressed data, was "sufi-1.0.2.6.tar", last modified: Thu May  9 14:28:20 2024, max compression
```

## Comparing `sufi-1.0.2.5.tar` & `sufi-1.0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-09 12:55:04.746297 sufi-1.0.2.5/
--rw-r--r--   0 sunny      (501) staff       (20)     1067 2024-05-02 00:31:02.000000 sufi-1.0.2.5/LICENCE
--rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-09 12:55:04.746169 sufi-1.0.2.5/PKG-INFO
--rw-r--r--   0 sunny      (501) staff       (20)     1798 2024-05-02 00:31:02.000000 sufi-1.0.2.5/README.md
--rw-r--r--   0 sunny      (501) staff       (20)       38 2024-05-09 12:55:04.746371 sufi-1.0.2.5/setup.cfg
--rw-r--r--   0 sunny      (501) staff       (20)      607 2024-05-09 12:54:01.000000 sufi-1.0.2.5/setup.py
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-09 12:55:04.744633 sufi-1.0.2.5/sufi/
--rw-r--r--   0 sunny      (501) staff       (20)        2 2024-05-02 00:31:02.000000 sufi-1.0.2.5/sufi/__init__.py
--rw-r--r--   0 sunny      (501) staff       (20)     7416 2024-05-09 12:52:55.000000 sufi-1.0.2.5/sufi/filters.py
--rw-r--r--   0 sunny      (501) staff       (20)   209989 2024-05-08 17:58:28.000000 sufi-1.0.2.5/sufi/pentagram.png
--rw-r--r--   0 sunny      (501) staff       (20)    48339 2023-03-10 20:10:30.000000 sufi-1.0.2.5/sufi/red.png
--rw-r--r--   0 sunny      (501) staff       (20)  1889093 2024-05-05 19:22:41.000000 sufi-1.0.2.5/sufi/shield.png
--rw-r--r--   0 sunny      (501) staff       (20)     4115 2024-05-08 22:41:40.000000 sufi-1.0.2.5/sufi/utility.py
--rw-r--r--   0 sunny      (501) staff       (20)     4926 2024-05-02 00:35:11.000000 sufi-1.0.2.5/sufi/videoProcessing.py
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-09 12:55:04.745994 sufi-1.0.2.5/sufi.egg-info/
--rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-09 12:55:04.000000 sufi-1.0.2.5/sufi.egg-info/PKG-INFO
--rw-r--r--   0 sunny      (501) staff       (20)      286 2024-05-09 12:55:04.000000 sufi-1.0.2.5/sufi.egg-info/SOURCES.txt
--rw-r--r--   0 sunny      (501) staff       (20)        1 2024-05-09 12:55:04.000000 sufi-1.0.2.5/sufi.egg-info/dependency_links.txt
--rw-r--r--   0 sunny      (501) staff       (20)       46 2024-05-09 12:55:04.000000 sufi-1.0.2.5/sufi.egg-info/requires.txt
--rw-r--r--   0 sunny      (501) staff       (20)        5 2024-05-09 12:55:04.000000 sufi-1.0.2.5/sufi.egg-info/top_level.txt
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-09 14:28:20.891818 sufi-1.0.2.6/
+-rw-r--r--   0 sunny      (501) staff       (20)     1067 2024-05-02 00:31:02.000000 sufi-1.0.2.6/LICENCE
+-rw-r--r--   0 sunny      (501) staff       (20)     2506 2024-05-09 14:28:20.891697 sufi-1.0.2.6/PKG-INFO
+-rw-r--r--   0 sunny      (501) staff       (20)     2197 2024-05-09 13:58:17.000000 sufi-1.0.2.6/README.md
+-rw-r--r--   0 sunny      (501) staff       (20)       38 2024-05-09 14:28:20.891869 sufi-1.0.2.6/setup.cfg
+-rw-r--r--   0 sunny      (501) staff       (20)      607 2024-05-09 14:28:14.000000 sufi-1.0.2.6/setup.py
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-09 14:28:20.889305 sufi-1.0.2.6/sufi/
+-rw-r--r--   0 sunny      (501) staff       (20)        2 2024-05-02 00:31:02.000000 sufi-1.0.2.6/sufi/__init__.py
+-rw-r--r--   0 sunny      (501) staff       (20)     7416 2024-05-09 12:52:55.000000 sufi-1.0.2.6/sufi/filters.py
+-rw-r--r--   0 sunny      (501) staff       (20)   209989 2024-05-08 17:58:28.000000 sufi-1.0.2.6/sufi/pentagram.png
+-rw-r--r--   0 sunny      (501) staff       (20)    48339 2023-03-10 20:10:30.000000 sufi-1.0.2.6/sufi/red.png
+-rw-r--r--   0 sunny      (501) staff       (20)  1889093 2024-05-05 19:22:41.000000 sufi-1.0.2.6/sufi/shield.png
+-rw-r--r--   0 sunny      (501) staff       (20)     4115 2024-05-08 22:41:40.000000 sufi-1.0.2.6/sufi/utility.py
+-rw-r--r--   0 sunny      (501) staff       (20)     4926 2024-05-02 00:35:11.000000 sufi-1.0.2.6/sufi/videoProcessing.py
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-09 14:28:20.891525 sufi-1.0.2.6/sufi.egg-info/
+-rw-r--r--   0 sunny      (501) staff       (20)     2506 2024-05-09 14:28:20.000000 sufi-1.0.2.6/sufi.egg-info/PKG-INFO
+-rw-r--r--   0 sunny      (501) staff       (20)      286 2024-05-09 14:28:20.000000 sufi-1.0.2.6/sufi.egg-info/SOURCES.txt
+-rw-r--r--   0 sunny      (501) staff       (20)        1 2024-05-09 14:28:20.000000 sufi-1.0.2.6/sufi.egg-info/dependency_links.txt
+-rw-r--r--   0 sunny      (501) staff       (20)       46 2024-05-09 14:28:20.000000 sufi-1.0.2.6/sufi.egg-info/requires.txt
+-rw-r--r--   0 sunny      (501) staff       (20)        5 2024-05-09 14:28:20.000000 sufi-1.0.2.6/sufi.egg-info/top_level.txt
```

### Comparing `sufi-1.0.2.5/LICENCE` & `sufi-1.0.2.6/LICENCE`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.5/PKG-INFO` & `sufi-1.0.2.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1
-Name: sufi
-Version: 1.0.2.5
-Summary: apply different types of filters on image
-Home-page: https://github.com/sunnykumar1516/sufi
-Author: sunny kumar
-Author-email: sunnykumar1516@gmail.com
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # sufi : Do image and video manipulation ||apply filters|| extract frames||
 
 
+
 # how to use 
 ## install
 
     pip install sufi
     
    ## import and use
 
     from sufi import filters
+
+  # apply spell filters
+  	from sufi import filters
+	from sufi import utility
+
+	filters.apply_spell() # casting spell
+
+  # sample output
+<img width="1277" alt="spell" src="https://github.com/sunnykumar1516/sufi/assets/25007015/adfaae00-3ea4-4f98-a443-f0420ac41a49">
+<img width="1275" alt="shield" src="https://github.com/sunnykumar1516/sufi/assets/25007015/d8633d11-d084-47dc-96e3-1679e90cebd6">
+
 # original image
 
 <img width="560" alt="Screenshot 2023-03-16 at 12 45 51 AM" src="https://github.com/sunnykumar1516/sufi/assets/25007015/22e16e9b-674a-4eb1-8b70-bf850fc2d2ea">
 
 # convert  image to digital art
```

### Comparing `sufi-1.0.2.5/setup.py` & `sufi-1.0.2.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	description = fh.read()
 
 setuptools.setup(
 	name="sufi",
-	version="1.0.2.5",
+	version="1.0.2.6",
 	author="sunny kumar",
 	author_email="sunnykumar1516@gmail.com",
 	packages=["sufi"],
 	description="apply different types of filters on image",
 	long_description=description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/sunnykumar1516/sufi",
```

### Comparing `sufi-1.0.2.5/sufi/filters.py` & `sufi-1.0.2.6/sufi/filters.py`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.5/sufi/pentagram.png` & `sufi-1.0.2.6/sufi/pentagram.png`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.5/sufi/red.png` & `sufi-1.0.2.6/sufi/red.png`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.5/sufi/shield.png` & `sufi-1.0.2.6/sufi/shield.png`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.5/sufi/utility.py` & `sufi-1.0.2.6/sufi/utility.py`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.5/sufi/videoProcessing.py` & `sufi-1.0.2.6/sufi/videoProcessing.py`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.5/sufi.egg-info/PKG-INFO` & `sufi-1.0.2.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 Metadata-Version: 2.1
 Name: sufi
-Version: 1.0.2.5
+Version: 1.0.2.6
 Summary: apply different types of filters on image
 Home-page: https://github.com/sunnykumar1516/sufi
 Author: sunny kumar
 Author-email: sunnykumar1516@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # sufi : Do image and video manipulation ||apply filters|| extract frames||
 
 
+
 # how to use 
 ## install
 
     pip install sufi
     
    ## import and use
 
     from sufi import filters
+
+  # apply spell filters
+  	from sufi import filters
+	from sufi import utility
+
+	filters.apply_spell() # casting spell
+
+  # sample output
+<img width="1277" alt="spell" src="https://github.com/sunnykumar1516/sufi/assets/25007015/adfaae00-3ea4-4f98-a443-f0420ac41a49">
+<img width="1275" alt="shield" src="https://github.com/sunnykumar1516/sufi/assets/25007015/d8633d11-d084-47dc-96e3-1679e90cebd6">
+
 # original image
 
 <img width="560" alt="Screenshot 2023-03-16 at 12 45 51 AM" src="https://github.com/sunnykumar1516/sufi/assets/25007015/22e16e9b-674a-4eb1-8b70-bf850fc2d2ea">
 
 # convert  image to digital art
```

