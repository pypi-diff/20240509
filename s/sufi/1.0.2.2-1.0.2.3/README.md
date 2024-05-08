# Comparing `tmp/sufi-1.0.2.2.tar.gz` & `tmp/sufi-1.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sufi-1.0.2.2.tar", last modified: Wed May  8 23:04:19 2024, max compression
+gzip compressed data, was "sufi-1.0.2.3.tar", last modified: Wed May  8 23:28:11 2024, max compression
```

## Comparing `sufi-1.0.2.2.tar` & `sufi-1.0.2.3.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:04:19.045965 sufi-1.0.2.2/
--rw-r--r--   0 sunny      (501) staff       (20)     1067 2024-05-02 00:31:02.000000 sufi-1.0.2.2/LICENCE
--rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-08 23:04:19.045844 sufi-1.0.2.2/PKG-INFO
--rw-r--r--   0 sunny      (501) staff       (20)     1798 2024-05-02 00:31:02.000000 sufi-1.0.2.2/README.md
--rw-r--r--   0 sunny      (501) staff       (20)       38 2024-05-08 23:04:19.046011 sufi-1.0.2.2/setup.cfg
--rw-r--r--   0 sunny      (501) staff       (20)      547 2024-05-08 23:03:54.000000 sufi-1.0.2.2/setup.py
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:04:19.044891 sufi-1.0.2.2/sufi/
--rw-r--r--   0 sunny      (501) staff       (20)        2 2024-05-02 00:31:02.000000 sufi-1.0.2.2/sufi/__init__.py
--rw-r--r--   0 sunny      (501) staff       (20)     7085 2024-05-08 22:53:19.000000 sufi-1.0.2.2/sufi/filters.py
--rw-r--r--   0 sunny      (501) staff       (20)     4115 2024-05-08 22:41:40.000000 sufi-1.0.2.2/sufi/utility.py
--rw-r--r--   0 sunny      (501) staff       (20)     4926 2024-05-02 00:35:11.000000 sufi-1.0.2.2/sufi/videoProcessing.py
-drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:04:19.045684 sufi-1.0.2.2/sufi.egg-info/
--rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-08 23:04:19.000000 sufi-1.0.2.2/sufi.egg-info/PKG-INFO
--rw-r--r--   0 sunny      (501) staff       (20)      238 2024-05-08 23:04:19.000000 sufi-1.0.2.2/sufi.egg-info/SOURCES.txt
--rw-r--r--   0 sunny      (501) staff       (20)        1 2024-05-08 23:04:19.000000 sufi-1.0.2.2/sufi.egg-info/dependency_links.txt
--rw-r--r--   0 sunny      (501) staff       (20)       46 2024-05-08 23:04:19.000000 sufi-1.0.2.2/sufi.egg-info/requires.txt
--rw-r--r--   0 sunny      (501) staff       (20)        5 2024-05-08 23:04:19.000000 sufi-1.0.2.2/sufi.egg-info/top_level.txt
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:28:11.193495 sufi-1.0.2.3/
+-rw-r--r--   0 sunny      (501) staff       (20)     1067 2024-05-02 00:31:02.000000 sufi-1.0.2.3/LICENCE
+-rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-08 23:28:11.193314 sufi-1.0.2.3/PKG-INFO
+-rw-r--r--   0 sunny      (501) staff       (20)     1798 2024-05-02 00:31:02.000000 sufi-1.0.2.3/README.md
+-rw-r--r--   0 sunny      (501) staff       (20)       38 2024-05-08 23:28:11.193561 sufi-1.0.2.3/setup.cfg
+-rw-r--r--   0 sunny      (501) staff       (20)      607 2024-05-08 23:27:33.000000 sufi-1.0.2.3/setup.py
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:28:11.191515 sufi-1.0.2.3/sufi/
+-rw-r--r--   0 sunny      (501) staff       (20)        2 2024-05-02 00:31:02.000000 sufi-1.0.2.3/sufi/__init__.py
+-rw-r--r--   0 sunny      (501) staff       (20)     7085 2024-05-08 22:53:19.000000 sufi-1.0.2.3/sufi/filters.py
+-rw-r--r--   0 sunny      (501) staff       (20)   209989 2024-05-08 17:58:28.000000 sufi-1.0.2.3/sufi/pentagram.png
+-rw-r--r--   0 sunny      (501) staff       (20)    48339 2023-03-10 20:10:30.000000 sufi-1.0.2.3/sufi/red.png
+-rw-r--r--   0 sunny      (501) staff       (20)  1889093 2024-05-05 19:22:41.000000 sufi-1.0.2.3/sufi/shield.png
+-rw-r--r--   0 sunny      (501) staff       (20)     4115 2024-05-08 22:41:40.000000 sufi-1.0.2.3/sufi/utility.py
+-rw-r--r--   0 sunny      (501) staff       (20)     4926 2024-05-02 00:35:11.000000 sufi-1.0.2.3/sufi/videoProcessing.py
+drwxr-xr-x   0 sunny      (501) staff       (20)        0 2024-05-08 23:28:11.193093 sufi-1.0.2.3/sufi.egg-info/
+-rw-r--r--   0 sunny      (501) staff       (20)     2107 2024-05-08 23:28:11.000000 sufi-1.0.2.3/sufi.egg-info/PKG-INFO
+-rw-r--r--   0 sunny      (501) staff       (20)      286 2024-05-08 23:28:11.000000 sufi-1.0.2.3/sufi.egg-info/SOURCES.txt
+-rw-r--r--   0 sunny      (501) staff       (20)        1 2024-05-08 23:28:11.000000 sufi-1.0.2.3/sufi.egg-info/dependency_links.txt
+-rw-r--r--   0 sunny      (501) staff       (20)       46 2024-05-08 23:28:11.000000 sufi-1.0.2.3/sufi.egg-info/requires.txt
+-rw-r--r--   0 sunny      (501) staff       (20)        5 2024-05-08 23:28:11.000000 sufi-1.0.2.3/sufi.egg-info/top_level.txt
```

### Comparing `sufi-1.0.2.2/LICENCE` & `sufi-1.0.2.3/LICENCE`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.2/PKG-INFO` & `sufi-1.0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sufi
-Version: 1.0.2.2
+Version: 1.0.2.3
 Summary: apply different types of filters on image
 Home-page: https://github.com/sunnykumar1516/sufi
 Author: sunny kumar
 Author-email: sunnykumar1516@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sufi-1.0.2.2/README.md` & `sufi-1.0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.2/setup.py` & `sufi-1.0.2.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	description = fh.read()
 
 setuptools.setup(
 	name="sufi",
-	version="1.0.2.2",
+	version="1.0.2.3",
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
         'opencv-python>=4',
 		'mediapipe == 0.10.5'
 
-    ]
+    ],
+	include_package_data=True,
+	package_data={'': ['*.png']}
+
 )
```

### Comparing `sufi-1.0.2.2/sufi/filters.py` & `sufi-1.0.2.3/sufi/filters.py`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.2/sufi/utility.py` & `sufi-1.0.2.3/sufi/utility.py`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.2/sufi/videoProcessing.py` & `sufi-1.0.2.3/sufi/videoProcessing.py`

 * *Files identical despite different names*

### Comparing `sufi-1.0.2.2/sufi.egg-info/PKG-INFO` & `sufi-1.0.2.3/sufi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sufi
-Version: 1.0.2.2
+Version: 1.0.2.3
 Summary: apply different types of filters on image
 Home-page: https://github.com/sunnykumar1516/sufi
 Author: sunny kumar
 Author-email: sunnykumar1516@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

