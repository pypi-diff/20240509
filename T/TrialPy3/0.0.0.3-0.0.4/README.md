# Comparing `tmp/TrialPy3-0.0.0.3.tar.gz` & `tmp/TrialPy3-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrialPy3-0.0.0.3.tar", last modified: Wed May  8 13:55:43 2024, max compression
+gzip compressed data, was "TrialPy3-0.0.4.tar", last modified: Thu May  9 11:39:03 2024, max compression
```

## Comparing `TrialPy3-0.0.0.3.tar` & `TrialPy3-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:55:43.565630 TrialPy3-0.0.0.3/
--rw-rw-rw-   0        0        0    27028 2023-09-16 09:04:03.000000 TrialPy3-0.0.0.3/LICENSE
--rw-rw-rw-   0        0        0     8156 2024-05-08 13:55:43.564633 TrialPy3-0.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7814 2024-05-08 13:54:54.000000 TrialPy3-0.0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 13:55:43.565630 TrialPy3-0.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      931 2024-05-08 13:55:32.000000 TrialPy3-0.0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:55:43.549672 TrialPy3-0.0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 13:55:43.557653 TrialPy3-0.0.0.3/src/TrialPy3/
--rw-rw-rw-   0        0        0   209208 2024-05-07 08:55:46.000000 TrialPy3-0.0.0.3/src/TrialPy3/RCFA.py
--rw-rw-rw-   0        0        0   112808 2023-09-08 08:00:59.000000 TrialPy3-0.0.0.3/src/TrialPy3/_RCSingle.py
--rw-rw-rw-   0        0        0        0 2024-04-30 07:11:25.000000 TrialPy3-0.0.0.3/src/TrialPy3/__init__.py
--rw-rw-rw-   0        0        0    12116 2023-09-08 04:56:21.000000 TrialPy3-0.0.0.3/src/TrialPy3/_arrangeCal.py
--rw-rw-rw-   0        0        0     7726 2023-08-08 11:47:29.000000 TrialPy3-0.0.0.3/src/TrialPy3/_forcesCal.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:55:43.562639 TrialPy3-0.0.0.3/src/TrialPy3.egg-info/
--rw-rw-rw-   0        0        0     8156 2024-05-08 13:55:43.000000 TrialPy3-0.0.0.3/src/TrialPy3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2024-05-08 13:55:43.000000 TrialPy3-0.0.0.3/src/TrialPy3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:55:43.000000 TrialPy3-0.0.0.3/src/TrialPy3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-05-08 13:55:43.000000 TrialPy3-0.0.0.3/src/TrialPy3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 13:55:43.000000 TrialPy3-0.0.0.3/src/TrialPy3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 13:55:43.563636 TrialPy3-0.0.0.3/test/
--rw-rw-rw-   0        0        0    23383 2024-05-08 13:11:46.000000 TrialPy3-0.0.0.3/test/test_RCFA.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:39:03.540304 TrialPy3-0.0.4/
+-rw-rw-rw-   0        0        0    27028 2023-09-16 09:04:03.000000 TrialPy3-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     8439 2024-05-09 11:39:03.540304 TrialPy3-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8099 2024-05-09 11:38:36.000000 TrialPy3-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-09 11:39:03.540304 TrialPy3-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      929 2024-05-09 04:55:33.000000 TrialPy3-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:39:03.524348 TrialPy3-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 11:39:03.532327 TrialPy3-0.0.4/src/TrialPy3/
+-rw-rw-rw-   0        0        0   209208 2024-05-07 08:55:46.000000 TrialPy3-0.0.4/src/TrialPy3/RCFA.py
+-rw-rw-rw-   0        0        0   112808 2023-09-08 08:00:59.000000 TrialPy3-0.0.4/src/TrialPy3/_RCSingle.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 07:11:25.000000 TrialPy3-0.0.4/src/TrialPy3/__init__.py
+-rw-rw-rw-   0        0        0    12116 2023-09-08 04:56:21.000000 TrialPy3-0.0.4/src/TrialPy3/_arrangeCal.py
+-rw-rw-rw-   0        0        0     7726 2023-08-08 11:47:29.000000 TrialPy3-0.0.4/src/TrialPy3/_forcesCal.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:39:03.537313 TrialPy3-0.0.4/src/TrialPy3.egg-info/
+-rw-rw-rw-   0        0        0     8439 2024-05-09 11:39:03.000000 TrialPy3-0.0.4/src/TrialPy3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-05-09 11:39:03.000000 TrialPy3-0.0.4/src/TrialPy3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 11:39:03.000000 TrialPy3-0.0.4/src/TrialPy3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-05-09 11:39:03.000000 TrialPy3-0.0.4/src/TrialPy3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 11:39:03.000000 TrialPy3-0.0.4/src/TrialPy3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 11:39:03.538309 TrialPy3-0.0.4/test/
+-rw-rw-rw-   0        0        0    23318 2024-05-09 04:55:48.000000 TrialPy3-0.0.4/test/test_RCFA.py
```

### Comparing `TrialPy3-0.0.0.3/LICENSE` & `TrialPy3-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TrialPy3-0.0.0.3/PKG-INFO` & `TrialPy3-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 Metadata-Version: 2.1
 Name: TrialPy3
-Version: 0.0.0.3
+Version: 0.0.4
 Summary: Object Oriented Structural Analysis
 License: GNU LESSER GENERAL PUBLIC LICENSE v2.1 or later (GNU LGPLv2.1)
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # StrucPy
 
-[![LGPLv2.1 License](https://img.shields.io/badge/unittest-passing-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html)
-
-[![Unit Tests](https://img.shields.io/badge/tests-passing-green.svg)]()
-
-[![Documentation Status](https://readthedocs.org/projects/strucpy/badge/?version=latest)](https://strucpy.readthedocs.io/en/latest/?badge=latest)
-
-[![LGPLv2.1 License](https://img.shields.io/badge/License-LGPL%20v2.1-yellow.svg)](https://opensource.org/licenses/)
+[![Unit Tests](https://github.com/TabishIzhar/StrucPy/actions/workflows/python-app.yml/badge.svg)](https://github.com/TabishIzhar/StrucPy/actions/workflows/python-app.yml) [![Documentation Status](https://readthedocs.org/projects/strucpy/badge/?version=latest)](https://strucpy.readthedocs.io/en/latest/?badge=latest) [![LGPLv2.1 License](https://img.shields.io/badge/unittest-passing-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html)
 
 **StrucPy** is a powerful python library for structural analysis. It gives complete control over the results of structure analysis. StrucPy is originally developed for the students and researchers working in field of civil engineering. It will be highly helpful for structural analysis, structural design, design optimization, visualizing the structural behavior, learning, application of machine learning in structural analysis, etc.
 
 ------------------------------------------------------------------------------------------------------------
 ## Modules 
 
 * **RCFA** - Structural analysis module for Reinforced Concrete Framed Structures 
@@ -80,34 +74,43 @@
 * P-delta analysis of structure.
 * Inclusion of Wind Loads as per IS 875 part 3.
 * Dynamic Seismic Analysis
 
 -----------------------------------------------------------------------------------------------------------
 ## StrucPy Coordinate System 
 
-Follow left-hand rule for coordinate system, the left thumb points along the y-axis in the positive direction. Gravity loads acting along y-axis.
-
-![](https://ibb.co/FqRKbxP)
+Follow left-hand rule for coordinate system, the left thumb points along the y-axis in the positive direction. Gravity load acts along y-axis.
 
+![](https://drive.google.com/file/d/11R0xjPRELNxWBfIFui6kXTP1_RKK-gW8/view?usp=sharing)
 
 
 ------------------------------------------------------------------------------------------------------------
 
 ## StrucPy Documentation
 
 https://strucpy.readthedocs.io/
 
 ------------------------------------------------------------------------------------------------------------
 
 ## Installation 
 
+Always create a virtual environment to install `StrucPy` and its dependencies.
+
+1) Creating Virtual environment
+```
+    $ py -3 -m venv venv
+```
+2) Activate virtual environment from cmd
+```
+    .\venv\Scripts\activate.bat
+```
+3) Install `StrucPy`
 ```
     $ py -3 -m pip install StrucPy
 ```
-
 ------------------------------------------------------------------------------------------------------------
 
 ## Cloning Git repository
 
 1) Clone the repository using **https://github.com/TabishIzhar/StrucPy.git**
 
 2) Form a virtual environment using
```

### Comparing `TrialPy3-0.0.0.3/README.md` & `TrialPy3-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 # StrucPy
 
-[![LGPLv2.1 License](https://img.shields.io/badge/unittest-passing-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html)
-
-[![Unit Tests](https://img.shields.io/badge/tests-passing-green.svg)]()
-
-[![Documentation Status](https://readthedocs.org/projects/strucpy/badge/?version=latest)](https://strucpy.readthedocs.io/en/latest/?badge=latest)
-
-[![LGPLv2.1 License](https://img.shields.io/badge/License-LGPL%20v2.1-yellow.svg)](https://opensource.org/licenses/)
+[![Unit Tests](https://github.com/TabishIzhar/StrucPy/actions/workflows/python-app.yml/badge.svg)](https://github.com/TabishIzhar/StrucPy/actions/workflows/python-app.yml) [![Documentation Status](https://readthedocs.org/projects/strucpy/badge/?version=latest)](https://strucpy.readthedocs.io/en/latest/?badge=latest) [![LGPLv2.1 License](https://img.shields.io/badge/unittest-passing-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html)
 
 **StrucPy** is a powerful python library for structural analysis. It gives complete control over the results of structure analysis. StrucPy is originally developed for the students and researchers working in field of civil engineering. It will be highly helpful for structural analysis, structural design, design optimization, visualizing the structural behavior, learning, application of machine learning in structural analysis, etc.
 
 ------------------------------------------------------------------------------------------------------------
 ## Modules 
 
 * **RCFA** - Structural analysis module for Reinforced Concrete Framed Structures 
@@ -69,34 +63,43 @@
 * P-delta analysis of structure.
 * Inclusion of Wind Loads as per IS 875 part 3.
 * Dynamic Seismic Analysis
 
 -----------------------------------------------------------------------------------------------------------
 ## StrucPy Coordinate System 
 
-Follow left-hand rule for coordinate system, the left thumb points along the y-axis in the positive direction. Gravity loads acting along y-axis.
-
-![](https://ibb.co/FqRKbxP)
+Follow left-hand rule for coordinate system, the left thumb points along the y-axis in the positive direction. Gravity load acts along y-axis.
 
+![](https://drive.google.com/file/d/11R0xjPRELNxWBfIFui6kXTP1_RKK-gW8/view?usp=sharing)
 
 
 ------------------------------------------------------------------------------------------------------------
 
 ## StrucPy Documentation
 
 https://strucpy.readthedocs.io/
 
 ------------------------------------------------------------------------------------------------------------
 
 ## Installation 
 
+Always create a virtual environment to install `StrucPy` and its dependencies.
+
+1) Creating Virtual environment
+```
+    $ py -3 -m venv venv
+```
+2) Activate virtual environment from cmd
+```
+    .\venv\Scripts\activate.bat
+```
+3) Install `StrucPy`
 ```
     $ py -3 -m pip install StrucPy
 ```
-
 ------------------------------------------------------------------------------------------------------------
 
 ## Cloning Git repository
 
 1) Clone the repository using **https://github.com/TabishIzhar/StrucPy.git**
 
 2) Form a virtual environment using
```

### Comparing `TrialPy3-0.0.0.3/setup.py` & `TrialPy3-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description= f.read()
 
 setup(
     name="TrialPy3",
-    version="0.0.0.3",
+    version="0.0.4",
     description="Object Oriented Structural Analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/TabishIzhar/StrucPy.git",
     # author="Tabish Izhar",
     # author_email="tizhar@iul.ac.in",
     license="GNU LESSER GENERAL PUBLIC LICENSE v2.1 or later (GNU LGPLv2.1)",
```

### Comparing `TrialPy3-0.0.0.3/src/TrialPy3/RCFA.py` & `TrialPy3-0.0.4/src/TrialPy3/RCFA.py`

 * *Files identical despite different names*

### Comparing `TrialPy3-0.0.0.3/src/TrialPy3/_RCSingle.py` & `TrialPy3-0.0.4/src/TrialPy3/_RCSingle.py`

 * *Files identical despite different names*

### Comparing `TrialPy3-0.0.0.3/src/TrialPy3/_arrangeCal.py` & `TrialPy3-0.0.4/src/TrialPy3/_arrangeCal.py`

 * *Files identical despite different names*

### Comparing `TrialPy3-0.0.0.3/src/TrialPy3/_forcesCal.py` & `TrialPy3-0.0.4/src/TrialPy3/_forcesCal.py`

 * *Files identical despite different names*

### Comparing `TrialPy3-0.0.0.3/src/TrialPy3.egg-info/PKG-INFO` & `TrialPy3-0.0.4/src/TrialPy3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 Metadata-Version: 2.1
 Name: TrialPy3
-Version: 0.0.0.3
+Version: 0.0.4
 Summary: Object Oriented Structural Analysis
 License: GNU LESSER GENERAL PUBLIC LICENSE v2.1 or later (GNU LGPLv2.1)
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # StrucPy
 
-[![LGPLv2.1 License](https://img.shields.io/badge/unittest-passing-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html)
-
-[![Unit Tests](https://img.shields.io/badge/tests-passing-green.svg)]()
-
-[![Documentation Status](https://readthedocs.org/projects/strucpy/badge/?version=latest)](https://strucpy.readthedocs.io/en/latest/?badge=latest)
-
-[![LGPLv2.1 License](https://img.shields.io/badge/License-LGPL%20v2.1-yellow.svg)](https://opensource.org/licenses/)
+[![Unit Tests](https://github.com/TabishIzhar/StrucPy/actions/workflows/python-app.yml/badge.svg)](https://github.com/TabishIzhar/StrucPy/actions/workflows/python-app.yml) [![Documentation Status](https://readthedocs.org/projects/strucpy/badge/?version=latest)](https://strucpy.readthedocs.io/en/latest/?badge=latest) [![LGPLv2.1 License](https://img.shields.io/badge/unittest-passing-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html)
 
 **StrucPy** is a powerful python library for structural analysis. It gives complete control over the results of structure analysis. StrucPy is originally developed for the students and researchers working in field of civil engineering. It will be highly helpful for structural analysis, structural design, design optimization, visualizing the structural behavior, learning, application of machine learning in structural analysis, etc.
 
 ------------------------------------------------------------------------------------------------------------
 ## Modules 
 
 * **RCFA** - Structural analysis module for Reinforced Concrete Framed Structures 
@@ -80,34 +74,43 @@
 * P-delta analysis of structure.
 * Inclusion of Wind Loads as per IS 875 part 3.
 * Dynamic Seismic Analysis
 
 -----------------------------------------------------------------------------------------------------------
 ## StrucPy Coordinate System 
 
-Follow left-hand rule for coordinate system, the left thumb points along the y-axis in the positive direction. Gravity loads acting along y-axis.
-
-![](https://ibb.co/FqRKbxP)
+Follow left-hand rule for coordinate system, the left thumb points along the y-axis in the positive direction. Gravity load acts along y-axis.
 
+![](https://drive.google.com/file/d/11R0xjPRELNxWBfIFui6kXTP1_RKK-gW8/view?usp=sharing)
 
 
 ------------------------------------------------------------------------------------------------------------
 
 ## StrucPy Documentation
 
 https://strucpy.readthedocs.io/
 
 ------------------------------------------------------------------------------------------------------------
 
 ## Installation 
 
+Always create a virtual environment to install `StrucPy` and its dependencies.
+
+1) Creating Virtual environment
+```
+    $ py -3 -m venv venv
+```
+2) Activate virtual environment from cmd
+```
+    .\venv\Scripts\activate.bat
+```
+3) Install `StrucPy`
 ```
     $ py -3 -m pip install StrucPy
 ```
-
 ------------------------------------------------------------------------------------------------------------
 
 ## Cloning Git repository
 
 1) Clone the repository using **https://github.com/TabishIzhar/StrucPy.git**
 
 2) Form a virtual environment using
```

### Comparing `TrialPy3-0.0.0.3/test/test_RCFA.py` & `TrialPy3-0.0.4/test/test_RCFA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#Example 1: Analysis of fixed Beam With multiple point loads using :class:`StrucPy.RCFA.RCF`.
+# Unit Tests on StrucPy RCFA
 
 from src.TrialPy3.RCFA import RCF
 from src.TrialPy3.RCFA import RCFenv
 import pandas as pd
 import numpy as np
 import pytest
```

