# Comparing `tmp/marksgeometrys-0.1.tar.gz` & `tmp/marksgeometrys-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marksgeometrys-0.1.tar", last modified: Thu May  9 18:10:42 2024, max compression
+gzip compressed data, was "marksgeometrys-0.1.1.tar", last modified: Thu May  9 18:22:15 2024, max compression
```

## Comparing `marksgeometrys-0.1.tar` & `marksgeometrys-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 18:10:42.333990 marksgeometrys-0.1/
--rw-rw-rw-   0        0        0     1062 2024-05-07 19:04:53.000000 marksgeometrys-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1305 2024-05-09 18:10:42.329989 marksgeometrys-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      627 2024-05-09 18:09:51.000000 marksgeometrys-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 18:10:42.307989 marksgeometrys-0.1/marksgeometrys/
--rw-rw-rw-   0        0        0       37 2024-05-09 18:06:33.000000 marksgeometrys-0.1/marksgeometrys/__init__.py
--rw-rw-rw-   0        0        0    14705 2024-05-09 17:53:03.000000 marksgeometrys-0.1/marksgeometrys/geometry.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:10:42.327989 marksgeometrys-0.1/marksgeometrys.egg-info/
--rw-rw-rw-   0        0        0     1305 2024-05-09 18:10:42.000000 marksgeometrys-0.1/marksgeometrys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-09 18:10:42.000000 marksgeometrys-0.1/marksgeometrys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 18:10:42.000000 marksgeometrys-0.1/marksgeometrys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-09 18:10:42.000000 marksgeometrys-0.1/marksgeometrys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-09 18:10:42.000000 marksgeometrys-0.1/marksgeometrys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 18:10:42.334990 marksgeometrys-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1264 2024-05-09 18:07:33.000000 marksgeometrys-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:22:15.873259 marksgeometrys-0.1.1/
+-rw-rw-rw-   0        0        0     1062 2024-05-07 19:04:53.000000 marksgeometrys-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1286 2024-05-09 18:22:15.869259 marksgeometrys-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2024-05-09 18:09:51.000000 marksgeometrys-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 18:22:15.841256 marksgeometrys-0.1.1/marksgeometrys/
+-rw-rw-rw-   0        0        0       37 2024-05-09 18:06:33.000000 marksgeometrys-0.1.1/marksgeometrys/__init__.py
+-rw-rw-rw-   0        0        0    14705 2024-05-09 17:53:03.000000 marksgeometrys-0.1.1/marksgeometrys/geometry.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:22:15.864258 marksgeometrys-0.1.1/marksgeometrys.egg-info/
+-rw-rw-rw-   0        0        0     1286 2024-05-09 18:22:15.000000 marksgeometrys-0.1.1/marksgeometrys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-09 18:22:15.000000 marksgeometrys-0.1.1/marksgeometrys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 18:22:15.000000 marksgeometrys-0.1.1/marksgeometrys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-09 18:22:15.000000 marksgeometrys-0.1.1/marksgeometrys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 18:22:15.874260 marksgeometrys-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1260 2024-05-09 18:21:52.000000 marksgeometrys-0.1.1/setup.py
```

### Comparing `marksgeometrys-0.1/LICENSE.txt` & `marksgeometrys-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `marksgeometrys-0.1/PKG-INFO` & `marksgeometrys-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: marksgeometrys
-Version: 0.1
+Version: 0.1.1
 Summary: Calculate many figures area or volume
 Home-page: https://github.com/marc1fino/marksgeometrys
 Author: mark. (Marc Pérez)
 Author-email: <marcperezcarrasco2010@gmail.com>
 License: MIT
 Keywords: python,maths,figures,area,volume,mathematical figures
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: math
 
 # marksgeometrys
 
 A mathematical library to calculate many figures area or volume.
 
 Developed by Marc Pérez (c) 2024
```

### Comparing `marksgeometrys-0.1/README.md` & `marksgeometrys-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `marksgeometrys-0.1/marksgeometrys/geometry.py` & `marksgeometrys-0.1.1/marksgeometrys/geometry.py`

 * *Files identical despite different names*

### Comparing `marksgeometrys-0.1/marksgeometrys.egg-info/PKG-INFO` & `marksgeometrys-0.1.1/marksgeometrys.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: marksgeometrys
-Version: 0.1
+Version: 0.1.1
 Summary: Calculate many figures area or volume
 Home-page: https://github.com/marc1fino/marksgeometrys
 Author: mark. (Marc Pérez)
 Author-email: <marcperezcarrasco2010@gmail.com>
 License: MIT
 Keywords: python,maths,figures,area,volume,mathematical figures
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: math
 
 # marksgeometrys
 
 A mathematical library to calculate many figures area or volume.
 
 Developed by Marc Pérez (c) 2024
```

### Comparing `marksgeometrys-0.1/setup.py` & `marksgeometrys-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.1'
+VERSION = '0.1.1'
 DESCRIPTION = 'Calculate many figures area or volume'
 working_directory = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(working_directory, "README.md"), encoding='utf-8') as f:
     long_description1 = f.read()
 # Setting up
 setup(
@@ -14,15 +14,15 @@
     author="mark. (Marc Pérez)",
     author_email="<marcperezcarrasco2010@gmail.com>",
     url='https://github.com/marc1fino/marksgeometrys',
     description=DESCRIPTION,
     long_description=long_description1,
     long_description_content_type='text/markdown',
     packages=find_packages(),
-    install_requires=['math'],
+    install_requires=[],
     license='MIT',
     keywords=['python', 'maths', 'figures', 'area', 'volume', 'mathematical figures'],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

