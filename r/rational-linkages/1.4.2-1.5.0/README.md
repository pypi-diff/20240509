# Comparing `tmp/rational-linkages-1.4.2.tar.gz` & `tmp/rational_linkages-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rational-linkages-1.4.2.tar", last modified: Fri Mar 15 10:45:56 2024, max compression
+gzip compressed data, was "rational_linkages-1.5.0.tar", last modified: Thu May  9 16:43:29 2024, max compression
```

## Comparing `rational-linkages-1.4.2.tar` & `rational_linkages-1.5.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 10:45:56.661090 rational-linkages-1.4.2/
--rw-rw-rw-   0        0        0    35784 2024-01-13 16:52:17.000000 rational-linkages-1.4.2/LICENSE
--rw-rw-rw-   0        0        0    46787 2024-03-15 10:45:56.660053 rational-linkages-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     4158 2024-03-11 08:09:32.000000 rational-linkages-1.4.2/README.md
--rw-rw-rw-   0        0        0     2086 2024-03-15 10:42:44.000000 rational-linkages-1.4.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-15 10:45:56.623367 rational-linkages-1.4.2/python/
-drwxrwxrwx   0        0        0        0 2024-03-15 10:45:56.646171 rational-linkages-1.4.2/python/rational_linkages/
--rw-rw-rw-   0        0        0     1348 2024-02-07 10:07:32.000000 rational-linkages-1.4.2/python/rational_linkages/AffineMatrix.py
--rw-rw-rw-   0        0        0     4328 2024-02-07 10:07:32.000000 rational-linkages-1.4.2/python/rational_linkages/AffineMetric.py
--rw-rw-rw-   0        0        0     1128 2024-01-10 11:50:48.000000 rational-linkages-1.4.2/python/rational_linkages/ButtonID.py
--rw-rw-rw-   0        0        0    12300 2024-03-08 10:41:39.000000 rational-linkages-1.4.2/python/rational_linkages/CollisionFreeOptimization.py
--rw-rw-rw-   0        0        0    22369 2024-03-11 10:09:07.000000 rational-linkages-1.4.2/python/rational_linkages/DualQuaternion.py
--rw-rw-rw-   0        0        0     4133 2024-03-01 12:15:49.000000 rational-linkages-1.4.2/python/rational_linkages/DualQuaternionAction.py
--rw-rw-rw-   0        0        0     5444 2024-03-05 15:01:34.000000 rational-linkages-1.4.2/python/rational_linkages/ExudynAnalysis.py
--rw-rw-rw-   0        0        0     6489 2024-03-05 14:07:44.000000 rational-linkages-1.4.2/python/rational_linkages/FactorizationProvider.py
--rw-rw-rw-   0        0        0     8693 2024-02-12 16:40:21.000000 rational-linkages-1.4.2/python/rational_linkages/Linkage.py
--rw-rw-rw-   0        0        0     4171 2024-01-11 07:35:34.000000 rational-linkages-1.4.2/python/rational_linkages/MiniBall.py
--rw-rw-rw-   0        0        0     2772 2024-02-07 10:07:32.000000 rational-linkages-1.4.2/python/rational_linkages/MotionApproximation.py
--rw-rw-rw-   0        0        0    16019 2024-02-23 13:55:36.000000 rational-linkages-1.4.2/python/rational_linkages/MotionFactorization.py
--rw-rw-rw-   0        0        0    13419 2024-03-08 10:04:36.000000 rational-linkages-1.4.2/python/rational_linkages/MotionInterpolation.py
--rw-rw-rw-   0        0        0    14270 2024-03-07 12:24:11.000000 rational-linkages-1.4.2/python/rational_linkages/NormalizedLine.py
--rw-rw-rw-   0        0        0    25013 2024-03-08 08:46:18.000000 rational-linkages-1.4.2/python/rational_linkages/Plotter.py
--rw-rw-rw-   0        0        0     8077 2024-03-06 10:28:25.000000 rational-linkages-1.4.2/python/rational_linkages/PointHomogeneous.py
--rw-rw-rw-   0        0        0     4902 2024-03-01 10:37:26.000000 rational-linkages-1.4.2/python/rational_linkages/Quaternion.py
--rw-rw-rw-   0        0        0     5190 2024-02-07 10:07:32.000000 rational-linkages-1.4.2/python/rational_linkages/RationalBezier.py
--rw-rw-rw-   0        0        0    13806 2024-03-08 13:31:05.000000 rational-linkages-1.4.2/python/rational_linkages/RationalCurve.py
--rw-rw-rw-   0        0        0     1487 2024-02-07 10:07:32.000000 rational-linkages-1.4.2/python/rational_linkages/RationalDualQuaternion.py
--rw-rw-rw-   0        0        0    32443 2024-03-15 10:18:02.000000 rational-linkages-1.4.2/python/rational_linkages/RationalMechanism.py
--rw-rw-rw-   0        0        0     1899 2024-02-23 12:29:08.000000 rational-linkages-1.4.2/python/rational_linkages/SingularityAnalysis.py
--rw-rw-rw-   0        0        0    14902 2024-03-15 10:18:02.000000 rational-linkages-1.4.2/python/rational_linkages/TransfMatrix.py
--rw-rw-rw-   0        0        0      884 2024-03-05 15:01:34.000000 rational-linkages-1.4.2/python/rational_linkages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 10:45:56.655911 rational-linkages-1.4.2/python/rational_linkages/data/
--rw-rw-rw-   0        0        0    40058 2024-01-23 14:32:29.000000 rational-linkages-1.4.2/python/rational_linkages/data/bennett_ark24.pkl
--rw-rw-rw-   0        0        0    73944 2024-02-06 14:55:17.000000 rational-linkages-1.4.2/python/rational_linkages/data/collisions_free_6r.pkl
--rw-rw-rw-   0        0        0    48044 2024-03-06 15:32:40.000000 rational-linkages-1.4.2/python/rational_linkages/data/plane_fold_6r.pkl
--rw-rw-rw-   0        0        0     1964 2024-03-08 13:40:08.000000 rational-linkages-1.4.2/python/rational_linkages/models.py
-drwxrwxrwx   0        0        0        0 2024-03-15 10:45:56.656971 rational-linkages-1.4.2/python/rational_linkages.egg-info/
--rw-rw-rw-   0        0        0    46787 2024-03-15 10:45:56.000000 rational-linkages-1.4.2/python/rational_linkages.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1501 2024-03-15 10:45:56.000000 rational-linkages-1.4.2/python/rational_linkages.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 10:45:56.000000 rational-linkages-1.4.2/python/rational_linkages.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2024-03-15 10:45:56.000000 rational-linkages-1.4.2/python/rational_linkages.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-15 10:45:56.000000 rational-linkages-1.4.2/python/rational_linkages.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-15 10:45:56.661090 rational-linkages-1.4.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 16:43:29.014231 rational_linkages-1.5.0/
+-rw-rw-rw-   0        0        0    35784 2024-01-13 16:52:17.000000 rational_linkages-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0    46803 2024-05-09 16:43:29.014231 rational_linkages-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4182 2024-05-03 13:07:20.000000 rational_linkages-1.5.0/README.md
+-rw-rw-rw-   0        0        0     2028 2024-05-09 16:41:11.000000 rational_linkages-1.5.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-09 16:43:28.982314 rational_linkages-1.5.0/python/
+drwxrwxrwx   0        0        0        0 2024-05-09 16:43:29.003694 rational_linkages-1.5.0/python/rational_linkages/
+-rw-rw-rw-   0        0        0     6545 2024-05-09 16:39:04.000000 rational_linkages-1.5.0/python/rational_linkages/AffineMetric.py
+-rw-rw-rw-   0        0        0     1128 2024-01-10 11:50:48.000000 rational_linkages-1.5.0/python/rational_linkages/ButtonID.py
+-rw-rw-rw-   0        0        0     1071 2024-05-09 12:40:39.000000 rational_linkages-1.5.0/python/rational_linkages/CollisionAnalyser.py
+-rw-rw-rw-   0        0        0    12300 2024-03-08 10:41:39.000000 rational_linkages-1.5.0/python/rational_linkages/CollisionFreeOptimization.py
+-rw-rw-rw-   0        0        0    23160 2024-05-09 12:04:32.000000 rational_linkages-1.5.0/python/rational_linkages/DualQuaternion.py
+-rw-rw-rw-   0        0        0     4133 2024-03-01 12:15:49.000000 rational_linkages-1.5.0/python/rational_linkages/DualQuaternionAction.py
+-rw-rw-rw-   0        0        0     5739 2024-04-22 09:34:12.000000 rational_linkages-1.5.0/python/rational_linkages/ExudynAnalysis.py
+-rw-rw-rw-   0        0        0     6400 2024-05-09 11:18:34.000000 rational_linkages-1.5.0/python/rational_linkages/FactorizationProvider.py
+-rw-rw-rw-   0        0        0     9487 2024-05-09 12:40:39.000000 rational_linkages-1.5.0/python/rational_linkages/Linkage.py
+-rw-rw-rw-   0        0        0     4497 2024-05-09 12:40:39.000000 rational_linkages-1.5.0/python/rational_linkages/MiniBall.py
+-rw-rw-rw-   0        0        0     2772 2024-02-07 10:07:32.000000 rational_linkages-1.5.0/python/rational_linkages/MotionApproximation.py
+-rw-rw-rw-   0        0        0    16140 2024-04-22 09:34:12.000000 rational_linkages-1.5.0/python/rational_linkages/MotionFactorization.py
+-rw-rw-rw-   0        0        0    20096 2024-05-09 12:40:39.000000 rational_linkages-1.5.0/python/rational_linkages/MotionInterpolation.py
+-rw-rw-rw-   0        0        0    14339 2024-05-09 09:29:07.000000 rational_linkages-1.5.0/python/rational_linkages/NormalizedLine.py
+-rw-rw-rw-   0        0        0    28500 2024-05-09 12:40:39.000000 rational_linkages-1.5.0/python/rational_linkages/Plotter.py
+-rw-rw-rw-   0        0        0    11166 2024-05-09 12:40:39.000000 rational_linkages-1.5.0/python/rational_linkages/PointHomogeneous.py
+-rw-rw-rw-   0        0        0     4902 2024-03-01 10:37:26.000000 rational_linkages-1.5.0/python/rational_linkages/Quaternion.py
+-rw-rw-rw-   0        0        0     7799 2024-05-09 16:33:53.000000 rational_linkages-1.5.0/python/rational_linkages/RationalBezier.py
+-rw-rw-rw-   0        0        0    18684 2024-05-09 12:40:39.000000 rational_linkages-1.5.0/python/rational_linkages/RationalCurve.py
+-rw-rw-rw-   0        0        0     1487 2024-02-07 10:07:32.000000 rational_linkages-1.5.0/python/rational_linkages/RationalDualQuaternion.py
+-rw-rw-rw-   0        0        0    33930 2024-05-09 12:40:39.000000 rational_linkages-1.5.0/python/rational_linkages/RationalMechanism.py
+-rw-rw-rw-   0        0        0     1899 2024-05-02 08:49:34.000000 rational_linkages-1.5.0/python/rational_linkages/SingularityAnalysis.py
+-rw-rw-rw-   0        0        0    15109 2024-05-09 11:28:49.000000 rational_linkages-1.5.0/python/rational_linkages/TransfMatrix.py
+-rw-rw-rw-   0        0        0      989 2024-05-09 12:40:39.000000 rational_linkages-1.5.0/python/rational_linkages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:43:29.014231 rational_linkages-1.5.0/python/rational_linkages/data/
+-rw-rw-rw-   0        0        0    40058 2024-01-23 14:32:29.000000 rational_linkages-1.5.0/python/rational_linkages/data/bennett_ark24.pkl
+-rw-rw-rw-   0        0        0    73944 2024-02-06 14:55:17.000000 rational_linkages-1.5.0/python/rational_linkages/data/collisions_free_6r.pkl
+-rw-rw-rw-   0        0        0    48044 2024-03-06 15:32:40.000000 rational_linkages-1.5.0/python/rational_linkages/data/plane_fold_6r.pkl
+-rw-rw-rw-   0        0        0     5738 2024-05-09 12:40:39.000000 rational_linkages-1.5.0/python/rational_linkages/models.py
+-rw-rw-rw-   0        0        0      273 2024-04-22 09:34:12.000000 rational_linkages-1.5.0/python/rational_linkages/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:43:29.014231 rational_linkages-1.5.0/python/rational_linkages.egg-info/
+-rw-rw-rw-   0        0        0    46803 2024-05-09 16:43:28.000000 rational_linkages-1.5.0/python/rational_linkages.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1540 2024-05-09 16:43:28.000000 rational_linkages-1.5.0/python/rational_linkages.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 16:43:28.000000 rational_linkages-1.5.0/python/rational_linkages.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      228 2024-05-09 16:43:28.000000 rational_linkages-1.5.0/python/rational_linkages.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-09 16:43:28.000000 rational_linkages-1.5.0/python/rational_linkages.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 16:43:29.014231 rational_linkages-1.5.0/setup.cfg
```

### Comparing `rational-linkages-1.4.2/LICENSE` & `rational_linkages-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rational-linkages-1.4.2/PKG-INFO` & `rational_linkages-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rational-linkages
-Version: 1.4.2
-Summary: Rational Linkages Toolbox
+Version: 1.5.0
+Summary: Rational Linkages
 Author-email: Daniel Huczala <daniel.huczala@uibk.ac.at>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -707,25 +707,26 @@
 Requires-Dist: flake8-pyproject; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 [![build](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/badges/main/pipeline.svg)](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/-/jobs)
 [![Documentation Status](https://readthedocs.org/projects/rational-linkages/badge/?version=latest)](https://rational-linkages.readthedocs.io/?badge=latest)
-[![PyPI version](https://img.shields.io/pypi/v/rational-linkages.svg)](https://pypi.org/project/rational-linkages/)[![coverage](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/badges/main/coverage.svg?job=run_tests)](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/-/jobs)
+[![PyPI version](https://img.shields.io/pypi/v/rational-linkages.svg)](https://pypi.org/project/rational-linkages/)
+[![coverage](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/badges/main/coverage.svg?job=test_coverage)](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/-/jobs)
 [![GitHub issues](https://img.shields.io/github/issues/hucik14/rl-issues)](https://github.com/hucik14/rl-issues/issues)
 [![Python](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue.svg)]()
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/hucik14/rl-issues/HEAD?labpath=jupyter_ntbs%2Fsynthesis_bennett.ipynb)
 
 
 # Rational Linkages
 
-Python-based toolbox for synthesis and rapid-prototyping of rational linkages, 
+Python-based package for synthesis and rapid-prototyping of rational linkages, 
 developed by the Unit of Geometry and Surveying, University of Innsbruck, Austria. 
-The documentation is hosted on Read the Docs, available here: 
+The **documentation with examples** is hosted on Read the Docs, available here: 
 [Rational Linkages Documentation](https://rational-linkages.readthedocs.io/).
 
 ## Intallation instuctions
 
 Recommended Python version is **3.11**, when it provides the smoothest plotting 
 (but 3.10 or higher are supported). Python 3.11 is also the version used for 
 development.
@@ -742,15 +743,15 @@
     
     <code>git clone https://git.uibk.ac.at/geometrie-vermessung/rational-linkages.git </code>
 
 2. Navigate to the repository folder
 
     <code>cd rational-linkages</code>
 
-3. Install the *editable* version of the pakcage using pip:
+3. Install the *editable* version of the package using pip:
 
     <code>pip install -e .</code>
 
 ## Tutorials, issues, usage, and contributions
 
 See the [documentation examples](https://rational-linkages.readthedocs.io/latest/general/overview.html) 
 for tutorials and usage examples.
```

### Comparing `rational-linkages-1.4.2/README.md` & `rational_linkages-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [![build](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/badges/main/pipeline.svg)](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/-/jobs)
 [![Documentation Status](https://readthedocs.org/projects/rational-linkages/badge/?version=latest)](https://rational-linkages.readthedocs.io/?badge=latest)
-[![PyPI version](https://img.shields.io/pypi/v/rational-linkages.svg)](https://pypi.org/project/rational-linkages/)[![coverage](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/badges/main/coverage.svg?job=run_tests)](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/-/jobs)
+[![PyPI version](https://img.shields.io/pypi/v/rational-linkages.svg)](https://pypi.org/project/rational-linkages/)
+[![coverage](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/badges/main/coverage.svg?job=test_coverage)](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/-/jobs)
 [![GitHub issues](https://img.shields.io/github/issues/hucik14/rl-issues)](https://github.com/hucik14/rl-issues/issues)
 [![Python](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue.svg)]()
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/hucik14/rl-issues/HEAD?labpath=jupyter_ntbs%2Fsynthesis_bennett.ipynb)
 
 
 # Rational Linkages
 
-Python-based toolbox for synthesis and rapid-prototyping of rational linkages, 
+Python-based package for synthesis and rapid-prototyping of rational linkages, 
 developed by the Unit of Geometry and Surveying, University of Innsbruck, Austria. 
-The documentation is hosted on Read the Docs, available here: 
+The **documentation with examples** is hosted on Read the Docs, available here: 
 [Rational Linkages Documentation](https://rational-linkages.readthedocs.io/).
 
 ## Intallation instuctions
 
 Recommended Python version is **3.11**, when it provides the smoothest plotting 
 (but 3.10 or higher are supported). Python 3.11 is also the version used for 
 development.
@@ -31,15 +32,15 @@
     
     <code>git clone https://git.uibk.ac.at/geometrie-vermessung/rational-linkages.git </code>
 
 2. Navigate to the repository folder
 
     <code>cd rational-linkages</code>
 
-3. Install the *editable* version of the pakcage using pip:
+3. Install the *editable* version of the package using pip:
 
     <code>pip install -e .</code>
 
 ## Tutorials, issues, usage, and contributions
 
 See the [documentation examples](https://rational-linkages.readthedocs.io/latest/general/overview.html) 
 for tutorials and usage examples.
```

### Comparing `rational-linkages-1.4.2/pyproject.toml` & `rational_linkages-1.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,129 +3,125 @@
 00000020: 7570 746f 6f6c 733e 3d36 312e 3022 2c20  uptools>=61.0", 
 00000030: 2277 6865 656c 225d 0d0a 6275 696c 642d  "wheel"]..build-
 00000040: 6261 636b 656e 6420 3d20 2273 6574 7570  backend = "setup
 00000050: 746f 6f6c 732e 6275 696c 645f 6d65 7461  tools.build_meta
 00000060: 220d 0a0d 0a5b 7072 6f6a 6563 745d 0d0a  "....[project]..
 00000070: 6e61 6d65 203d 2022 7261 7469 6f6e 616c  name = "rational
 00000080: 2d6c 696e 6b61 6765 7322 0d0a 7665 7273  -linkages"..vers
-00000090: 696f 6e20 3d20 2231 2e34 2e32 220d 0a64  ion = "1.4.2"..d
+00000090: 696f 6e20 3d20 2231 2e35 2e30 220d 0a64  ion = "1.5.0"..d
 000000a0: 6573 6372 6970 7469 6f6e 203d 2022 5261  escription = "Ra
-000000b0: 7469 6f6e 616c 204c 696e 6b61 6765 7320  tional Linkages 
-000000c0: 546f 6f6c 626f 7822 0d0a 6175 7468 6f72  Toolbox"..author
-000000d0: 7320 3d20 5b0d 0a20 2020 207b 6e61 6d65  s = [..    {name
-000000e0: 203d 2022 4461 6e69 656c 2048 7563 7a61   = "Daniel Hucza
-000000f0: 6c61 222c 2065 6d61 696c 203d 2022 6461  la", email = "da
-00000100: 6e69 656c 2e68 7563 7a61 6c61 4075 6962  niel.huczala@uib
-00000110: 6b2e 6163 2e61 7422 7d2c 0d0a 5d0d 0a72  k.ac.at"},..]..r
-00000120: 6571 7569 7265 732d 7079 7468 6f6e 203d  equires-python =
-00000130: 2022 3e3d 332e 3130 220d 0a6c 6963 656e   ">=3.10"..licen
-00000140: 7365 203d 207b 2266 696c 6522 3d20 224c  se = {"file"= "L
-00000150: 4943 454e 5345 227d 0d0a 7265 6164 6d65  ICENSE"}..readme
-00000160: 203d 2022 5245 4144 4d45 2e6d 6422 0d0a   = "README.md"..
-00000170: 636c 6173 7369 6669 6572 7320 3d20 5b0d  classifiers = [.
-00000180: 0a20 2020 2022 5072 6f67 7261 6d6d 696e  .    "Programmin
-00000190: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001a0: 7468 6f6e 203a 3a20 3322 2c0d 0a20 2020  thon :: 3",..   
-000001b0: 2022 4c69 6365 6e73 6520 3a3a 204f 5349   "License :: OSI
-000001c0: 2041 7070 726f 7665 6420 3a3a 2047 4e55   Approved :: GNU
-000001d0: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-000001e0: 4c69 6365 6e73 6520 7633 206f 7220 6c61  License v3 or la
-000001f0: 7465 7220 2847 504c 7633 2b29 222c 0d0a  ter (GPLv3+)",..
-00000200: 2020 2020 224f 7065 7261 7469 6e67 2053      "Operating S
-00000210: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-00000220: 7065 6e64 656e 7422 2c0d 0a5d 0d0a 0d0a  pendent",..]....
-00000230: 6465 7065 6e64 656e 6369 6573 203d 205b  dependencies = [
-00000240: 0d0a 2020 2020 2273 6369 7079 203e 3d20  ..    "scipy >= 
-00000250: 312e 3130 2e30 222c 0d0a 2020 2020 2273  1.10.0",..    "s
-00000260: 796d 7079 203e 3d20 312e 3130 2e30 222c  ympy >= 1.10.0",
-00000270: 0d0a 2020 2020 226d 6174 706c 6f74 6c69  ..    "matplotli
-00000280: 6220 3e3d 2033 2e37 2e30 222c 0d0a 2020  b >= 3.7.0",..  
-00000290: 2020 2262 6971 7561 7465 726e 696f 6e2d    "biquaternion-
-000002a0: 7079 203e 3d20 312e 322e 3022 2c0d 0a20  py >= 1.2.0",.. 
-000002b0: 2020 2022 5079 5174 3520 3e3d 2035 2e31     "PyQt5 >= 5.1
-000002c0: 352e 3130 222c 0d0a 5d0d 0a0d 0a5b 7072  5.10",..]....[pr
-000002d0: 6f6a 6563 742e 6f70 7469 6f6e 616c 2d64  oject.optional-d
-000002e0: 6570 656e 6465 6e63 6965 735d 0d0a 646f  ependencies]..do
-000002f0: 6320 3d20 5b0d 0a20 2020 2022 7370 6869  c = [..    "sphi
-00000300: 6e78 222c 0d0a 2020 2020 2273 7068 696e  nx",..    "sphin
-00000310: 782d 7274 642d 7468 656d 6522 2c0d 0a20  x-rtd-theme",.. 
-00000320: 2020 2022 6e62 7370 6869 6e78 222c 0d0a     "nbsphinx",..
-00000330: 2020 2020 2273 7068 696e 7863 6f6e 7472      "sphinxcontr
-00000340: 6962 2d62 6962 7465 7822 2c0d 0a20 2020  ib-bibtex",..   
-00000350: 2022 746f 6d6c 222c 0d0a 2020 2020 2270   "toml",..    "p
-00000360: 616e 646f 6322 2c0d 0a5d 0d0a 6465 7620  andoc",..]..dev 
-00000370: 3d20 5b0d 0a20 2020 2022 6275 696c 6422  = [..    "build"
-00000380: 2c0d 0a20 2020 2022 636f 7665 7261 6765  ,..    "coverage
-00000390: 222c 0d0a 2020 2020 2270 7974 6573 7422  ",..    "pytest"
-000003a0: 2c0d 0a20 2020 2022 666c 616b 6538 222c  ,..    "flake8",
-000003b0: 0d0a 2020 2020 2266 6c61 6b65 382d 7079  ..    "flake8-py
-000003c0: 7072 6f6a 6563 7422 2c0d 0a20 2020 2022  project",..    "
-000003d0: 626c 6163 6b22 2c0d 0a20 2020 2022 6973  black",..    "is
-000003e0: 6f72 7422 2c0d 0a20 2020 2022 7477 696e  ort",..    "twin
-000003f0: 6522 0d0a 5d0d 0a0d 0a5b 746f 6f6c 2e73  e"..]....[tool.s
-00000400: 6574 7570 746f 6f6c 732e 7061 636b 6167  etuptools.packag
-00000410: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-00000420: 3d20 5b22 7079 7468 6f6e 225d 0d0a 696e  = ["python"]..in
-00000430: 636c 7564 6520 3d20 5b22 7261 7469 6f6e  clude = ["ration
-00000440: 616c 5f6c 696e 6b61 6765 732a 225d 0d0a  al_linkages*"]..
-00000450: 0d0a 5b74 6f6f 6c2e 7365 7475 7074 6f6f  ..[tool.setuptoo
-00000460: 6c73 2e70 6163 6b61 6765 2d64 6174 615d  ls.package-data]
-00000470: 0d0a 2272 6174 696f 6e61 6c5f 6c69 6e6b  .."rational_link
-00000480: 6167 6573 2e64 6174 6122 203d 205b 222a  ages.data" = ["*
-00000490: 2e70 6b6c 225d 0d0a 0d0a 5b70 726f 6a65  .pkl"]....[proje
-000004a0: 6374 2e75 726c 735d 0d0a 486f 6d65 7061  ct.urls]..Homepa
-000004b0: 6765 203d 2022 6874 7470 733a 2f2f 6769  ge = "https://gi
-000004c0: 742e 7569 626b 2e61 632e 6174 2f67 656f  t.uibk.ac.at/geo
-000004d0: 6d65 7472 6965 2d76 6572 6d65 7373 756e  metrie-vermessun
-000004e0: 672f 7261 7469 6f6e 616c 2d6c 696e 6b61  g/rational-linka
-000004f0: 6765 7322 0d0a 446f 6375 6d65 6e74 6174  ges"..Documentat
-00000500: 696f 6e20 3d20 2268 7474 703a 2f2f 7261  ion = "http://ra
-00000510: 7469 6f6e 616c 2d6c 696e 6b61 6765 732e  tional-linkages.
-00000520: 7265 6164 7468 6564 6f63 732e 696f 2f22  readthedocs.io/"
-00000530: 0d0a 4973 7375 6573 203d 2022 6874 7470  ..Issues = "http
-00000540: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
-00000550: 7563 696b 3134 2f72 6c2d 6973 7375 6573  ucik14/rl-issues
-00000560: 2f69 7373 7565 7322 0d0a 0d0a 5b74 6f6f  /issues"....[too
-00000570: 6c2e 626c 6163 6b5d 0d0a 6c69 6e65 2d6c  l.black]..line-l
-00000580: 656e 6774 6820 3d20 3838 0d0a 7461 7267  ength = 88..targ
-00000590: 6574 2d76 6572 7369 6f6e 203d 205b 2270  et-version = ["p
-000005a0: 7933 3131 225d 0d0a 6578 636c 7564 6520  y311"]..exclude 
-000005b0: 3d20 2228 2e67 6974 7c2e 6964 6561 7c64  = "(.git|.idea|d
-000005c0: 6f63 737c 6469 7374 7c72 6174 696f 6e61  ocs|dist|rationa
-000005d0: 6c5f 6c69 6e6b 6167 6573 2e65 6767 2d69  l_linkages.egg-i
-000005e0: 6e66 6f29 2f2e 2a22 0d0a 0d0a 5b74 6f6f  nfo)/.*"....[too
-000005f0: 6c2e 6973 6f72 745d 0d0a 7072 6f66 696c  l.isort]..profil
-00000600: 6520 3d20 2262 6c61 636b 220d 0a6c 696e  e = "black"..lin
-00000610: 655f 6c65 6e67 7468 203d 2038 380d 0a73  e_length = 88..s
-00000620: 6b69 7020 3d20 5b22 2e67 6974 222c 2022  kip = [".git", "
-00000630: 2e69 6465 6122 2c20 2264 6f63 7322 2c20  .idea", "docs", 
-00000640: 2264 6973 7422 2c20 2272 6174 696f 6e61  "dist", "rationa
-00000650: 6c5f 6c69 6e6b 6167 6573 2e65 6767 2d69  l_linkages.egg-i
-00000660: 6e66 6f22 5d0d 0a6b 6e6f 776e 5f66 6972  nfo"]..known_fir
-00000670: 7374 5f70 6172 7479 203d 205b 2272 6174  st_party = ["rat
-00000680: 696f 6e61 6c5f 6c69 6e6b 6167 6573 225d  ional_linkages"]
-00000690: 0d0a 666f 7263 655f 746f 5f74 6f70 203d  ..force_to_top =
-000006a0: 205b 2272 6174 696f 6e61 6c5f 6c69 6e6b   ["rational_link
-000006b0: 6167 6573 225d 0d0a 0d0a 5b74 6f6f 6c2e  ages"]....[tool.
-000006c0: 666c 616b 6538 5d0d 0a6d 6178 2d6c 696e  flake8]..max-lin
-000006d0: 652d 6c65 6e67 7468 203d 2027 3838 270d  e-length = '88'.
-000006e0: 0a69 676e 6f72 6520 3d20 5b22 4535 3031  .ignore = ["E501
-000006f0: 225d 0d0a 6578 636c 7564 6520 3d20 222e  "]..exclude = ".
-00000700: 6769 742c 202e 6964 6561 2c20 646f 6373  git, .idea, docs
-00000710: 2c20 6469 7374 2c20 7261 7469 6f6e 616c  , dist, rational
-00000720: 5f6c 696e 6b61 6765 732e 6567 672d 696e  _linkages.egg-in
-00000730: 666f 220d 0a0d 0a5b 746f 6f6c 2e63 6f76  fo"....[tool.cov
-00000740: 6572 6167 652e 7275 6e5d 0d0a 636f 6d6d  erage.run]..comm
-00000750: 616e 645f 6c69 6e65 203d 2022 2d6d 2070  and_line = "-m p
-00000760: 7974 6573 7420 7079 7468 6f6e 2f74 6573  ytest python/tes
-00000770: 7473 220d 0a6f 6d69 7420 3d20 5b0d 0a20  ts"..omit = [.. 
-00000780: 2020 2022 2a2f 7465 7374 2a22 2c0d 0a20     "*/test*",.. 
-00000790: 2020 2022 2a5f 5f69 6e69 745f 5f2e 7079     "*__init__.py
-000007a0: 222c 0d0a 2020 2020 222a 506c 6f74 7465  ",..    "*Plotte
-000007b0: 722e 7079 222c 0d0a 2020 2020 222a 4275  r.py",..    "*Bu
-000007c0: 7474 6f6e 4944 2e70 7922 2c0d 0a20 2020  ttonID.py",..   
-000007d0: 2022 2a41 6666 696e 654d 6174 7269 782e   "*AffineMatrix.
-000007e0: 7079 222c 0d0a 2020 2020 222a 4166 6669  py",..    "*Affi
-000007f0: 6e65 4d65 7472 6963 2e70 7922 2c0d 0a20  neMetric.py",.. 
-00000800: 2020 2022 2a4d 6f74 696f 6e41 7070 726f     "*MotionAppro
-00000810: 7869 6d61 7469 6f6e 2e70 7922 2c0d 0a20  ximation.py",.. 
-00000820: 2020 205d 0d0a                              ]..
+000000b0: 7469 6f6e 616c 204c 696e 6b61 6765 7322  tional Linkages"
+000000c0: 0d0a 6175 7468 6f72 7320 3d20 5b0d 0a20  ..authors = [.. 
+000000d0: 2020 207b 6e61 6d65 203d 2022 4461 6e69     {name = "Dani
+000000e0: 656c 2048 7563 7a61 6c61 222c 2065 6d61  el Huczala", ema
+000000f0: 696c 203d 2022 6461 6e69 656c 2e68 7563  il = "daniel.huc
+00000100: 7a61 6c61 4075 6962 6b2e 6163 2e61 7422  zala@uibk.ac.at"
+00000110: 7d2c 0d0a 5d0d 0a72 6571 7569 7265 732d  },..]..requires-
+00000120: 7079 7468 6f6e 203d 2022 3e3d 332e 3130  python = ">=3.10
+00000130: 220d 0a6c 6963 656e 7365 203d 207b 2266  "..license = {"f
+00000140: 696c 6522 3d20 224c 4943 454e 5345 227d  ile"= "LICENSE"}
+00000150: 0d0a 7265 6164 6d65 203d 2022 5245 4144  ..readme = "READ
+00000160: 4d45 2e6d 6422 0d0a 636c 6173 7369 6669  ME.md"..classifi
+00000170: 6572 7320 3d20 5b0d 0a20 2020 2022 5072  ers = [..    "Pr
+00000180: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000190: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000001a0: 3322 2c0d 0a20 2020 2022 4c69 6365 6e73  3",..    "Licens
+000001b0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000001c0: 6420 3a3a 2047 4e55 2047 656e 6572 616c  d :: GNU General
+000001d0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+000001e0: 7633 206f 7220 6c61 7465 7220 2847 504c  v3 or later (GPL
+000001f0: 7633 2b29 222c 0d0a 2020 2020 224f 7065  v3+)",..    "Ope
+00000200: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000210: 204f 5320 496e 6465 7065 6e64 656e 7422   OS Independent"
+00000220: 2c0d 0a5d 0d0a 0d0a 6465 7065 6e64 656e  ,..]....dependen
+00000230: 6369 6573 203d 205b 0d0a 2020 2020 2273  cies = [..    "s
+00000240: 6369 7079 203e 3d20 312e 3130 2e30 222c  cipy >= 1.10.0",
+00000250: 0d0a 2020 2020 2273 796d 7079 203e 3d20  ..    "sympy >= 
+00000260: 312e 3130 2e30 222c 0d0a 2020 2020 226d  1.10.0",..    "m
+00000270: 6174 706c 6f74 6c69 6220 3e3d 2033 2e37  atplotlib >= 3.7
+00000280: 2e30 222c 0d0a 2020 2020 2262 6971 7561  .0",..    "biqua
+00000290: 7465 726e 696f 6e2d 7079 203e 3d20 312e  ternion-py >= 1.
+000002a0: 322e 3022 2c0d 0a20 2020 2022 5079 5174  2.0",..    "PyQt
+000002b0: 3520 3e3d 2035 2e31 352e 3130 222c 0d0a  5 >= 5.15.10",..
+000002c0: 5d0d 0a0d 0a5b 7072 6f6a 6563 742e 6f70  ]....[project.op
+000002d0: 7469 6f6e 616c 2d64 6570 656e 6465 6e63  tional-dependenc
+000002e0: 6965 735d 0d0a 646f 6320 3d20 5b0d 0a20  ies]..doc = [.. 
+000002f0: 2020 2022 7370 6869 6e78 222c 0d0a 2020     "sphinx",..  
+00000300: 2020 2273 7068 696e 782d 7274 642d 7468    "sphinx-rtd-th
+00000310: 656d 6522 2c0d 0a20 2020 2022 6e62 7370  eme",..    "nbsp
+00000320: 6869 6e78 222c 0d0a 2020 2020 2273 7068  hinx",..    "sph
+00000330: 696e 7863 6f6e 7472 6962 2d62 6962 7465  inxcontrib-bibte
+00000340: 7822 2c0d 0a20 2020 2022 746f 6d6c 222c  x",..    "toml",
+00000350: 0d0a 2020 2020 2270 616e 646f 6322 2c0d  ..    "pandoc",.
+00000360: 0a5d 0d0a 6465 7620 3d20 5b0d 0a20 2020  .]..dev = [..   
+00000370: 2022 6275 696c 6422 2c0d 0a20 2020 2022   "build",..    "
+00000380: 636f 7665 7261 6765 222c 0d0a 2020 2020  coverage",..    
+00000390: 2270 7974 6573 7422 2c0d 0a20 2020 2022  "pytest",..    "
+000003a0: 666c 616b 6538 222c 0d0a 2020 2020 2266  flake8",..    "f
+000003b0: 6c61 6b65 382d 7079 7072 6f6a 6563 7422  lake8-pyproject"
+000003c0: 2c0d 0a20 2020 2022 626c 6163 6b22 2c0d  ,..    "black",.
+000003d0: 0a20 2020 2022 6973 6f72 7422 2c0d 0a20  .    "isort",.. 
+000003e0: 2020 2022 7477 696e 6522 0d0a 5d0d 0a0d     "twine"..]...
+000003f0: 0a5b 746f 6f6c 2e73 6574 7570 746f 6f6c  .[tool.setuptool
+00000400: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000410: 0d0a 7768 6572 6520 3d20 5b22 7079 7468  ..where = ["pyth
+00000420: 6f6e 225d 0d0a 696e 636c 7564 6520 3d20  on"]..include = 
+00000430: 5b22 7261 7469 6f6e 616c 5f6c 696e 6b61  ["rational_linka
+00000440: 6765 732a 225d 0d0a 0d0a 5b74 6f6f 6c2e  ges*"]....[tool.
+00000450: 7365 7475 7074 6f6f 6c73 2e70 6163 6b61  setuptools.packa
+00000460: 6765 2d64 6174 615d 0d0a 2272 6174 696f  ge-data].."ratio
+00000470: 6e61 6c5f 6c69 6e6b 6167 6573 2e64 6174  nal_linkages.dat
+00000480: 6122 203d 205b 222a 2e70 6b6c 225d 0d0a  a" = ["*.pkl"]..
+00000490: 0d0a 5b70 726f 6a65 6374 2e75 726c 735d  ..[project.urls]
+000004a0: 0d0a 486f 6d65 7061 6765 203d 2022 6874  ..Homepage = "ht
+000004b0: 7470 733a 2f2f 6769 742e 7569 626b 2e61  tps://git.uibk.a
+000004c0: 632e 6174 2f67 656f 6d65 7472 6965 2d76  c.at/geometrie-v
+000004d0: 6572 6d65 7373 756e 672f 7261 7469 6f6e  ermessung/ration
+000004e0: 616c 2d6c 696e 6b61 6765 7322 0d0a 446f  al-linkages"..Do
+000004f0: 6375 6d65 6e74 6174 696f 6e20 3d20 2268  cumentation = "h
+00000500: 7474 703a 2f2f 7261 7469 6f6e 616c 2d6c  ttp://rational-l
+00000510: 696e 6b61 6765 732e 7265 6164 7468 6564  inkages.readthed
+00000520: 6f63 732e 696f 2f22 0d0a 4973 7375 6573  ocs.io/"..Issues
+00000530: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
+00000540: 7562 2e63 6f6d 2f68 7563 696b 3134 2f72  ub.com/hucik14/r
+00000550: 6c2d 6973 7375 6573 2f69 7373 7565 7322  l-issues/issues"
+00000560: 0d0a 0d0a 5b74 6f6f 6c2e 626c 6163 6b5d  ....[tool.black]
+00000570: 0d0a 6c69 6e65 2d6c 656e 6774 6820 3d20  ..line-length = 
+00000580: 3838 0d0a 7461 7267 6574 2d76 6572 7369  88..target-versi
+00000590: 6f6e 203d 205b 2270 7933 3131 225d 0d0a  on = ["py311"]..
+000005a0: 6578 636c 7564 6520 3d20 2228 2e67 6974  exclude = "(.git
+000005b0: 7c2e 6964 6561 7c64 6f63 737c 6469 7374  |.idea|docs|dist
+000005c0: 7c72 6174 696f 6e61 6c5f 6c69 6e6b 6167  |rational_linkag
+000005d0: 6573 2e65 6767 2d69 6e66 6f29 2f2e 2a22  es.egg-info)/.*"
+000005e0: 0d0a 0d0a 5b74 6f6f 6c2e 6973 6f72 745d  ....[tool.isort]
+000005f0: 0d0a 7072 6f66 696c 6520 3d20 2262 6c61  ..profile = "bla
+00000600: 636b 220d 0a6c 696e 655f 6c65 6e67 7468  ck"..line_length
+00000610: 203d 2038 380d 0a73 6b69 7020 3d20 5b22   = 88..skip = ["
+00000620: 2e67 6974 222c 2022 2e69 6465 6122 2c20  .git", ".idea", 
+00000630: 2264 6f63 7322 2c20 2264 6973 7422 2c20  "docs", "dist", 
+00000640: 2272 6174 696f 6e61 6c5f 6c69 6e6b 6167  "rational_linkag
+00000650: 6573 2e65 6767 2d69 6e66 6f22 5d0d 0a6b  es.egg-info"]..k
+00000660: 6e6f 776e 5f66 6972 7374 5f70 6172 7479  nown_first_party
+00000670: 203d 205b 2272 6174 696f 6e61 6c5f 6c69   = ["rational_li
+00000680: 6e6b 6167 6573 225d 0d0a 666f 7263 655f  nkages"]..force_
+00000690: 746f 5f74 6f70 203d 205b 2272 6174 696f  to_top = ["ratio
+000006a0: 6e61 6c5f 6c69 6e6b 6167 6573 225d 0d0a  nal_linkages"]..
+000006b0: 0d0a 5b74 6f6f 6c2e 666c 616b 6538 5d0d  ..[tool.flake8].
+000006c0: 0a6d 6178 2d6c 696e 652d 6c65 6e67 7468  .max-line-length
+000006d0: 203d 2027 3838 270d 0a69 676e 6f72 6520   = '88'..ignore 
+000006e0: 3d20 5b22 4535 3031 225d 0d0a 6578 636c  = ["E501"]..excl
+000006f0: 7564 6520 3d20 222e 6769 742c 202e 6964  ude = ".git, .id
+00000700: 6561 2c20 646f 6373 2c20 6469 7374 2c20  ea, docs, dist, 
+00000710: 7261 7469 6f6e 616c 5f6c 696e 6b61 6765  rational_linkage
+00000720: 732e 6567 672d 696e 666f 220d 0a0d 0a5b  s.egg-info"....[
+00000730: 746f 6f6c 2e63 6f76 6572 6167 652e 7275  tool.coverage.ru
+00000740: 6e5d 0d0a 636f 6d6d 616e 645f 6c69 6e65  n]..command_line
+00000750: 203d 2022 2d6d 2070 7974 6573 7420 7079   = "-m pytest py
+00000760: 7468 6f6e 2f74 6573 7473 220d 0a6f 6d69  thon/tests"..omi
+00000770: 7420 3d20 5b0d 0a20 2020 2022 2a2f 7465  t = [..    "*/te
+00000780: 7374 2a22 2c0d 0a20 2020 2022 2a5f 5f69  st*",..    "*__i
+00000790: 6e69 745f 5f2e 7079 222c 0d0a 2020 2020  nit__.py",..    
+000007a0: 222a 506c 6f74 7465 722e 7079 222c 0d0a  "*Plotter.py",..
+000007b0: 2020 2020 222a 4275 7474 6f6e 4944 2e70      "*ButtonID.p
+000007c0: 7922 2c0d 0a20 2020 2022 2a4d 6f74 696f  y",..    "*Motio
+000007d0: 6e41 7070 726f 7869 6d61 7469 6f6e 2e70  nApproximation.p
+000007e0: 7922 2c0d 0a20 2020 205d 0d0a            y",..    ]..
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/AffineMetric.py` & `rational_linkages-1.5.0/python/rational_linkages/AffineMetric.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,64 +5,81 @@
 from .RationalCurve import RationalCurve
 
 
 class AffineMetric:
     """
     Class of affine metric in R12
 
-    For more information, see M. Hofer's dissertation thesis titled "Variational Motion
-    Design in the Presence of Obstacles", section 2.2 on page 6.
+    :references:
+        M. Hofer, "Variational Motion Design in the Presence of Obstacles",
+        dissertation thesis (2004), Page 7, Equation 2.4
+
+        Schroecker, Weber, "Guaranteed collision detection with toleranced
+        motions", Computer Aided Geometric Design (2014), Equation 3. DOI:
+        http://dx.doi.org/10.1016/j.cagd.2014.08.001
+
     """
     def __init__(self, motion_curve: RationalCurve, points: list[PointHomogeneous]):
         """
         Construct the affine metric of a motion from the given points in the 3D space
 
         :param motion_curve: RationalCurve - rational curve representing the motion
         :param points: list[PointHomogeneous] - points in the 3D space
         """
         self.motion_curve = motion_curve
         self.points = points
         self.number_of_points = len(points)
 
-        self.matrix = self.create_affine_metric()
+        # By Hofer
+        self.pose_distance_matrix = self.create_affine_metric()
+
+        # By Schroecker, Weber
+        self.inertia_matrix = np.sum([p[0] ** 2 * np.outer(p[1:], p[1:])
+                                      for p in self.points], axis=0)
+        self.inertia_eigen_vals = np.linalg.eigvals(self.inertia_matrix)
+        self.total_mass = np.sum([p[0] for p in self.points])
 
     def __repr__(self):
-        return f"{self.matrix}"
+        return f"{self.pose_distance_matrix}"
 
     def create_affine_metric(self) -> np.ndarray:
         """
         Create the affine metric of the motion
 
         This function computes the metric matrix for a homogeneous 3D point based on
         the formulation from M. Hofer's dissertation thesis titled "Variational Motion
         Design in the Presence of Obstacles", specifically on page 7, equation 2.4.
 
-        :return: np.ndarray - affine metric matrix in R12x12
+        :return: affine metric matrix in R12x12
+        :rtype: np.ndarray
 
         :references:
-            - M. Hofer, "Variational Motion Design in the Presence of Obstacles",
+            M. Hofer, "Variational Motion Design in the Presence of Obstacles",
             dissertation thesis (2004), Page 7, Equation 2.4
+
         """
         metric_matrix = np.zeros((12, 12))
         for i in range(self.number_of_points):
             metric_matrix += self.get_point_metric_matrix(self.points[i])
         return metric_matrix
 
     @staticmethod
     def get_point_metric_matrix(point: PointHomogeneous) -> np.ndarray:
         """
         Get the metric matrix of the given point
 
         :param point: PointHomogeneous - point in the 3D space
 
-        :return: np.ndarray - metric matrix of a single point in R12x12
+        :return: metric matrix of a single point in R12x12
+        :rtype: np.ndarray
 
         :references:
-            - M. Hofer, "Variational Motion Design in the Presence of Obstacles",
+            M. Hofer, "Variational Motion Design in the Presence of Obstacles",
             dissertation thesis (2004), Page 7, Equation 2.4
+
         """
         p = point.normalized_in_3d()
         i = np.eye(3)
 
         m00 = i
         m01 = p[0] * i
         m02 = p[1] * i
@@ -84,47 +101,96 @@
 
         return metric_matrix
 
     def get_curve_transformations(self) -> list[DualQuaternion]:
         """
         Get the transformations of the curve
 
-        :return: list[DualQuaternion] - transformations of the curve
+        :return: transformations of the curve
+        :rtype: list[DualQuaternion]
         """
 
         # tranformation at -1
         dq_1 = self.motion_curve.evaluate(-1)
-        # transformation at 1
-        dq_2 = self.motion_curve.evaluate(1)
         # transformation at infinity
         dq_inf = self.motion_curve.evaluate(0, inverted_part=True)
 
-        return [DualQuaternion(dq_1), DualQuaternion(dq_2), DualQuaternion(dq_inf)]
+        return [DualQuaternion(dq_1), DualQuaternion(dq_inf)]
 
-    def distance(self, a: np.ndarray, b: np.ndarray) -> float:
+    def distance_via_matrix(self, a: DualQuaternion, b: DualQuaternion) -> float:
         """
         Distance between two affine displacements
 
-        :param a:
-        :param b:
+        :param DualQuaternion a: displacement
+        :param DualQuaternion b: displacement
+
+        :return: distance between a and b
+        :rtype: float
+        """
+        a12 = a.as_12d_vector()
+        b12 = b.as_12d_vector()
+        ab = a12 - b12
+        return np.sqrt(ab @ self.pose_distance_matrix @ ab)
+
+    def squared_distance_pr12_points(self, a: np.ndarray, b: np.ndarray) -> float:
+        """
+        Squared distance between two points in R12
+
+        :param np.ndarray a: point in PR12
+        :param np.ndarray b: point in PR12
+
+        :return: squared distance between a and b
+        :rtype: float
+        """
+        a12 = a[1:]
+        b12 = b[1:]
+
+        ab = a12 - b12
+        return ab @ self.pose_distance_matrix @ ab
+
+    def distance(self, a: DualQuaternion, b: DualQuaternion) -> float:
+        """
+        Distance between two affine displacements
+
+        :param DualQuaternion a: displacement
+        :param DualQuaternion b: displacement
+
         :return: float - distance between a and b
+        :rtype: float
         """
-        return np.sqrt(self.inner_product(a - b, a - b))
+        return np.sqrt(self.inner_product(a, b))
 
-    def inner_product(self, dq_a: DualQuaternion, dq_b: DualQuaternion):
+    def squared_distance(self, a: DualQuaternion, b: DualQuaternion) -> float:
         """
-        Inner product of two DualQuaternions
+        Squared distance between two affine displacements
+
+        :param DualQuaternion a: displacement
+        :param DualQuaternion b: displacement
+
+        :return: float - squared distance between a and b
+        :rtype: float
+        """
+        return self.inner_product(a, b)
+
+    def inner_product(self, a: DualQuaternion, b: DualQuaternion):
+        """
+        Inner product of two DualQuaternions in the affine space
+
+        It is calculated as the sum of usual dot products of acted points, after the two
+        dual quaternions act on the points that define the metric.
 
-        :param dq_a: DualQuaternion
-        :param dq_b: DualQuaternion
+        :param DualQuaternion a: displacement
+        :param DualQuaternion b: displacement
 
-        :return: float - inner product of dq_a and dq_b
+        :return: inner product of dq_a and dq_b
+        :rtype: float
         """
-        inner_product = np.zeros(4)
+        inner_product = 0
         for i in range(self.number_of_points):
-            a_point = dq_a.act(self.points[i])
-            b_point = dq_b.act(self.points[i])
+            a_point = a.act(self.points[i])
+            b_point = b.act(self.points[i])
 
-            point = np.dot(a_point.array(), b_point.array())
-            inner_product += point
+            scalar = np.dot(a_point.normalized_in_3d() - b_point.normalized_in_3d(),
+                            a_point.normalized_in_3d() - b_point.normalized_in_3d())
+            inner_product += scalar
 
         return inner_product
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/ButtonID.py` & `rational_linkages-1.5.0/python/rational_linkages/ButtonID.py`

 * *Files identical despite different names*

### Comparing `rational-linkages-1.4.2/python/rational_linkages/CollisionFreeOptimization.py` & `rational_linkages-1.5.0/python/rational_linkages/CollisionFreeOptimization.py`

 * *Files identical despite different names*

### Comparing `rational-linkages-1.4.2/python/rational_linkages/DualQuaternion.py` & `rational_linkages-1.5.0/python/rational_linkages/DualQuaternion.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,26 +380,30 @@
         The back projection, or also known as fiber projection, is a method to project
         a dual quaternion onto the Study quadric, i.e. to obtain a proper rigid body
         displacement that it represents.
 
         :return: DualQuaternion
         :rtype: DualQuaternion
         """
-        primal = self.p
-        dual = self.d
+        if self.is_on_study_quadric():
+            return self
 
-        primal_2norm = 2 * primal.norm()
-        new_primal = Quaternion(np.array([primal_2norm, 0, 0, 0]))
-        new_dual = -1 * (primal * dual.conjugate() - dual * primal.conjugate())
-
-        dq = (DualQuaternion.from_two_quaternions(new_primal, new_dual)
-              * DualQuaternion.from_two_quaternions(primal, Quaternion(np.zeros(4)))
-              ) / 2
+        else:
+            primal = self.p
+            dual = self.d
+
+            primal_2norm = 2 * primal.norm()
+            new_primal = Quaternion(np.array([primal_2norm, 0, 0, 0]))
+            new_dual = -1 * (primal * dual.conjugate() - dual * primal.conjugate())
+
+            dq = (DualQuaternion.from_two_quaternions(new_primal, new_dual)
+                  * DualQuaternion.from_two_quaternions(primal, Quaternion(np.zeros(4)))
+                  ) / 2
 
-        return dq
+            return dq
 
     def array(self) -> np.ndarray:
         """
         DualQuaternion to numpy array (8-vector of study parameters)
 
         :return: DualQuaternion as numpy array
         :rtype: np.ndarray
@@ -459,20 +463,26 @@
         Check if the DualQuaternion is on the study quadric
 
         :return: True if the DualQuaternion is on the study quadric, False otherwise
         :rtype: bool
         """
         study_condition = (self.p[0] * self.d[0] + self.p[1] * self.d[1]
                            + self.p[2] * self.d[2] + self.p[3] * self.d[3])
-        return np.isclose(study_condition, 0)
+        study_condition = np.asarray(study_condition, dtype="float64")
+        return np.isclose(study_condition, 0.0, atol=1e-20)
 
-    def dq2matrix(self):
+    def dq2matrix(self, normalize: bool = True) -> np.ndarray:
         """
         Dual Quaternion to SE(3) transformation matrix
 
+        The transformation matrix is normalized by the first element of the matrix.
+
+        :param bool normalize: if True, the transformation matrix is normalized by the
+            first element of the matrix. Defaults to True.
+
         :return: 4x4 transformation matrix
         :rtype: np.ndarray
         """
         p0 = self[0]
         p1 = self[1]
         p2 = self[2]
         p3 = self[3]
@@ -494,25 +504,20 @@
         r31 = 2 * (p1 * p3 - p0 * p2)
         r32 = 2 * (p2 * p3 + p0 * p1)
 
         r14 = 2 * (-p0 * d1 + p1 * d0 - p2 * d3 + p3 * d2)
         r24 = 2 * (-p0 * d2 + p1 * d3 + p2 * d0 - p3 * d1)
         r34 = 2 * (-p0 * d3 - p1 * d2 + p2 * d1 + p3 * d0)
 
-        tr = np.array(
-            [
-                [r44, 0, 0, 0],
-                [r14, r11, r12, r13],
-                [r24, r21, r22, r23],
-                [r34, r31, r32, r33],
-            ]
-        )
+        tr = np.array([[r44, 0, 0, 0],
+                       [r14, r11, r12, r13],
+                       [r24, r21, r22, r23],
+                       [r34, r31, r32, r33]])
 
-        # Normalization
-        output_matrix = tr / tr[0, 0]
+        output_matrix = tr / tr[0, 0] if normalize else tr
         return output_matrix
 
     def dq2point_via_matrix(self) -> np.ndarray:
         """
         Dual Quaternion to point via SE(3) transformation matrix
 
         :return: array of 3-coordinates of point
@@ -619,14 +624,24 @@
 
         :return: array of 3-coordinates of point
         :rtype: np.ndarray
         """
         direction, moment = self.dq2line_vectors()
         return np.cross(direction, moment)
 
+    def as_12d_vector(self) -> np.ndarray:
+        """
+        Return the DualQuaternion as a 12D vector of normalized transformation matrix
+
+        :return: 12D vector of the DualQuaternion
+        :rtype: np.ndarray
+        """
+        mat = self.dq2matrix()
+        return np.hstack((mat[1:4, 0], mat[1:4, 1], mat[1:4, 2], mat[1:4, 3]))
+
     def act(
         self,
         affected_object: Union["DualQuaternion", "NormalizedLine", "PointHomogeneous"],
     ) -> Union["NormalizedLine", "PointHomogeneous"]:
         """
         Act on a line or point with the DualQuaternion
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/DualQuaternionAction.py` & `rational_linkages-1.5.0/python/rational_linkages/DualQuaternionAction.py`

 * *Files identical despite different names*

### Comparing `rational-linkages-1.4.2/python/rational_linkages/ExudynAnalysis.py` & `rational_linkages-1.5.0/python/rational_linkages/ExudynAnalysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import numpy as np
 from typing import Union
 
+from .utils import is_package_installed
 from .RationalMechanism import RationalMechanism
 
 
+if not is_package_installed('exudyn'):
+    print("Warning: The Exudyn package is not installed, since it is not "
+          "a dependency. To use this functionality, please install it "
+          "manually from PyPI using 'pip install exudyn'.")
+
+
 class ExudynAnalysis:
     """
     Class for dynamics analysis using Exudyn package.
 
     The Exudyn packages is not listed in this project's requirements, please install
     it manually. More information can be found in :ref:`documentation <exudyn_info>`
     or the Exudyn homepage: https://github.com/jgerstmayr/EXUDYN
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/FactorizationProvider.py` & `rational_linkages-1.5.0/python/rational_linkages/FactorizationProvider.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,30 +108,26 @@
         """
         # Calculate the norm polynomial. To avoid numerical problems, extract
         # the scalar part, since the norm should be purely real
         norm_poly = poly.norm()
         norm_poly = biquaternion_py.polynomials.Poly(norm_poly.poly.scal,
                                                      *norm_poly.indets)
 
-        print('Factorization is running...')
-
         # Calculate the irreducible factors, that determine the different factorizations
         _, factors = biquaternion_py.irreducible_factors(norm_poly, domain='RR')
 
         # The different permutations of the irreducible factors then generate
         # the different factorizations of the motion.
 
         if len(factors) <= 1:
             raise ValueError('The factorization failed for the given input.')
 
         factorization1 = biquaternion_py.factorize_from_list(poly, factors)
         factorization2 = biquaternion_py.factorize_from_list(poly, factors[::-1])
 
-        print('Factorization ended.')
-
         return [factorization1, factorization2]
 
     @staticmethod
     def factor2rotation_axis(factor: biquaternion_py.polynomials.Poly) -> (
             DualQuaternion):
         """
         Converts the given factor to a dual quaternion representing the rotation axis
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/Linkage.py` & `rational_linkages-1.5.0/python/rational_linkages/Linkage.py`

 * *Files 6% similar despite different names*

```diff
@@ -182,16 +182,16 @@
     :ivar PointHomogeneous point1: The equation of the second point of the line segment
     :ivar str type: The type of the line segment (b - base, j - joint, l - link,
         t - tool)
     :ivar int factorization_idx: The index of the factorization the line segment
         belongs to
     :ivar int idx: The index of the line segment in the factorization
     """
-    def __init__(self, eqation, point0, point1, linkage_type, f_idx, idx):
-        self.equation = eqation
+    def __init__(self, equation, point0, point1, linkage_type, f_idx, idx):
+        self.equation = equation
         self.point0 = point0
         self.point1 = point1
         self.type = linkage_type
         self.factorization_idx = f_idx
         self.idx = idx
 
     def __repr__(self):
@@ -221,8 +221,34 @@
         d1 = np.linalg.norm(p1.normalized_in_3d() - point.normalized_in_3d())
 
         if np.allclose(l, d0 + d1):
             return True
         else:
             return False
 
+    def get_plot_data(self) -> tuple:
+        """
+        Returns the plot data of the line segment.
+
+        :return: The plot data
+        :rtype: tuple
+        """
+        steps = 30
+        t_space = np.tan(np.linspace(-np.pi/2, np.pi/2, steps + 1))
+        p0 = np.array([self.point0.evaluate(t_val).normalized_in_3d() for t_val in t_space])
+        p1 = np.array([self.point1.evaluate(t_val).normalized_in_3d() for t_val in t_space])
+
+        # Separate the x, y, and z coordinates
+        x0, y0, z0 = p0[:, 0], p0[:, 1], p0[:, 2]
+        x1, y1, z1 = p1[:, 0], p1[:, 1], p1[:, 2]
+
+        # Create a meshgrid for the moving line segment
+        x = np.array([x0, x1])
+        y = np.array([y0, y1])
+        z = np.array([z0, z1])
+
+        return x, y, z
+
+
+
+
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/MiniBall.py` & `rational_linkages-1.5.0/python/rational_linkages/MiniBall.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,73 @@
 import numpy as np
-from matplotlib import pyplot as plt
 from scipy.optimize import minimize
 
 from .PointHomogeneous import PointHomogeneous
 
 
 class MiniBall:
-    def __init__(self, points: list, metric: str = "euclidean"):
+    def __init__(self,
+                 points: list[PointHomogeneous],
+                 metric: "AffineMetric" = None):
         """
         Initialize the MiniBall class
-        :param points: np.ndarray - array of points in the space
+
+        :param list[PointHomogeneous] points: array of points in the space
+        :param AffineMetric metric: alternative metric to be used for the ball
         """
         self.points = points
-        self.metric = metric
 
         self.number_of_points = len(self.points)
         self.dimension = self.points[0].coordinates.size
+
+        self.metric = metric
+
+        if metric is None:
+            self.metric = 'euclidean'
+            self.metric_obj = None
+        else:
+            metric = 'hofer'
+            self.metric_obj = metric
+
         self.center = np.zeros(self.dimension)
         self.radius = 10.0
 
         self.optimization_results = self.get_ball()
-        self.center = PointHomogeneous(self.optimization_results.x[: self.dimension])
-        self.radius = self.optimization_results.x[self.dimension]
+        self.center = PointHomogeneous(self.optimization_results.x[:-1])
+        self.radius = self.optimization_results.x[-1]
 
     def get_ball(self):
         """
         Find the smallest ball containing all given points in Euclidean metric
         """
 
         def objective_function(x):
             """
             Objective function to minimize the squared radius r^2 of the ball
             """
             return x[-1] ** 2
 
         # Prepare constraint equations based on the metric
         if self.metric == "hofer":
-
             def constraint_equations(x):
                 """
                 For Hofer metric, constraint equations must satisfy the ball by:
                 r - radius of the sphere, x - one of given points,
                 c - center of the sphere
                 """
-                return NotImplemented
+                constraints = np.zeros(self.number_of_points)
 
+                for i in range(self.number_of_points):
+                    squared_distance = sum(self.metric_obj.squared_distance_pr12_points(
+                        self.points[i].normalize(), x[j])
+                        for j in range(self.dimension)
+                    )
+                    constraints[i] = x[-1] ** 2 - squared_distance
+                return constraints
         else:
-
             def constraint_equations(x):
                 """
                 For Euclidean metric, constraint equations must satisfy the ball by:
                 r^2 - (x - c)^2 >= 0
                 r - radius of the sphere, x - one of given points,
                 c - center of the sphere
                 """
@@ -73,43 +90,31 @@
         initial_guess[0] = 1.0
         initial_guess[-1] = self.radius
 
         # Perform optimization
         result = minimize(objective_function, initial_guess, constraints=ineq_con)
         return result
 
-    def plot_ball(self, ax=None, color="red", alpha=0.15):
+    def get_plot_data(self) -> tuple:
         """
-        Plot the ball in 3D space
-        :param ax: matplotlib.axes.Axes object
-        :param color: color of the ball
-        :param alpha: transparency of the ball
-        """
-        # check dimension
-        if not self.dimension == 4:
-            raise ValueError(
-                "Cannot plot ball with dimension other than 3 (4 in homogenoeus coordinates)"
-            )
-        else:
-            if ax is None:
-                ax = plt.figure().add_subplot(projection="3d")
-            else:
-                ax = ax
+        Get data for plotting in 3D space
+
+        :return: x, y, z coordinates of the ball surface
+        :rtype: tuple
 
+        :raises ValueError: if the dimension is not 4 or 13
+        """
+        if self.dimension == 4 or self.dimension == 13:
             # Create the 3D sphere representing the circle
-            u = np.linspace(0, 2 * np.pi, 100)
-            v = np.linspace(0, np.pi, 100)
-            x = (
-                self.radius * np.outer(np.cos(u), np.sin(v))
-                + self.center.normalized_in_3d()[0]
-            )
-            y = (
-                self.radius * np.outer(np.sin(u), np.sin(v))
-                + self.center.normalized_in_3d()[1]
-            )
-            z = (
-                self.radius * np.outer(np.ones(np.size(u)), np.cos(v))
-                + self.center.normalized_in_3d()[2]
-            )
-            ax.plot_surface(x, y, z, color=color, alpha=alpha)
+            u = np.linspace(0, 2 * np.pi, 30)
+            v = np.linspace(0, np.pi, 30)
+
+            x = (self.radius * np.outer(np.cos(u), np.sin(v))
+                 + self.center.normalized_in_3d()[0])
+            y = (self.radius * np.outer(np.sin(u), np.sin(v))
+                 + self.center.normalized_in_3d()[1])
+            z = (self.radius * np.outer(np.ones(np.size(u)), np.cos(v))
+                 + self.center.normalized_in_3d()[2])
+        else:
+            raise ValueError("Cannot plot ball due to incompatible dimension.")
 
-        return ax
+        return x, y, z
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/MotionApproximation.py` & `rational_linkages-1.5.0/python/rational_linkages/MotionApproximation.py`

 * *Files identical despite different names*

### Comparing `rational-linkages-1.4.2/python/rational_linkages/MotionFactorization.py` & `rational_linkages-1.5.0/python/rational_linkages/MotionFactorization.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,14 +150,17 @@
         """
         linkage_points = []
         for i in range(self.number_of_factors):
             linkage_points.append(self.linkage[i].points)
 
         for i in range(self.number_of_factors - 1):
             if inverted_part:
+                if t_numerical == 0:  # avoid division by zero
+                    t_numerical = np.finfo(float).eps
+
                 pts_acted = [self.act(linkage_points[i + 1][j],
                                       end_idx=i, param=1/t_numerical) for j in range(2)]
             else:
                 pts_acted = [self.act(linkage_points[i + 1][j],
                                       end_idx=i, param=t_numerical) for j in range(2)]
             linkage_points[i + 1] = pts_acted
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/NormalizedLine.py` & `rational_linkages-1.5.0/python/rational_linkages/NormalizedLine.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
             direction = np.asarray(unit_screw[0:3])
             moment = np.asarray(unit_screw[3:6])
             # Check if the direction vector is normalized
             if round(np.linalg.norm(direction), 6) == 1.0:
                 self.direction = direction
                 self.moment = moment
             elif np.abs(np.linalg.norm(direction)) > 1e-10:
+                # TODO handle when np.linalg.norm(direction) == inf
                 self.direction = direction / np.linalg.norm(direction)
                 self.moment = moment / np.linalg.norm(direction)
             else:
                 warn("Direction vector has zero norm!")
                 self.direction = np.asarray(direction)
                 self.moment = np.asarray(moment)
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/Plotter.py` & `rational_linkages-1.5.0/python/rational_linkages/Plotter.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.widgets import Slider, TextBox
 
 from .DualQuaternion import DualQuaternion
 from .MotionFactorization import MotionFactorization
 from .NormalizedLine import NormalizedLine
-from .PointHomogeneous import PointHomogeneous
+from .PointHomogeneous import PointHomogeneous, PointOrbit
 from .RationalBezier import RationalBezier
 from .RationalCurve import RationalCurve
 from .RationalMechanism import RationalMechanism
 from .TransfMatrix import TransfMatrix
+from .MiniBall import MiniBall
+from .Linkage import LineSegment
 
 
 class Plotter:
     def __init__(self,
                  interactive: bool = False,
                  jupyter_notebook: bool = False,
                  interval=(-1, 1),
@@ -25,18 +27,20 @@
                  arrows_length: float = 1.0,
                  joint_range_lim: float = 1.0):
         """
         Initialize the plotter
 
         :param interactive: activate interactive mode
         :param jupyter_notebook: activate jupyter notebook mode
-        :param interval: interval for plotting
         :param steps: number of steps for plotting
         :param arrows_length: length of quiver arrows for poses and frames
         :param joint_range_lim: limit for joint sliders, will be +/- value
+        :param interval: interval for plotting, in case of a curve can be specified as interval = 'closed' for
+            full parametrization
+        :with_poses: plot the poses along the curve
         """
         # use Qt5Agg backend for interactive plotting
         if interactive and not jupyter_notebook:
             matplotlib.use("Qt5Agg")
 
         self.fig = plt.figure()
         self.ax = self.fig.add_subplot(projection="3d")
@@ -77,24 +81,45 @@
         self.j_sliders_limit = joint_range_lim
 
         # length of quiver arrows for poses and frames
         self.arrows_length = arrows_length
 
         self.plotted = {}
 
-    def plot(self, object_to_plot, **kwargs):
+    def plot(self, objects_to_plot, **kwargs):
+        """
+        Plot the object
+
+        :param objects_to_plot: NormalizedLine, PointHomogeneous, RationalMechanism,
+            MotionFactorization, DualQuaternion, TransfMatrix, RationalCurve,
+            RationalBezier, MiniBall, or list of those
+        :param kwargs: plotting options following matplotlib standards and syntax
+        """
+        # if list of objects, plot each object separately
+        if isinstance(objects_to_plot, list):
+            # check for label list
+            label_list = kwargs.pop('label', None)
+
+            for i, obj in enumerate(objects_to_plot):
+                if label_list is not None:
+                    kwargs['label'] = label_list[i]
+                self._plot(obj, **kwargs)
+
+        # if single object, plot it
+        else:
+            self._plot(objects_to_plot, **kwargs)
+
+    def _plot(self, object_to_plot, **kwargs):
         """
         Plot the object
 
         :param object_to_plot: NormalizedLine, PointHomogeneous, RationalMechanism,
-            MotionFactorization, DualQuaternion, TransfMatrix, RationalCurve
+            MotionFactorization, DualQuaternion, TransfMatrix, RationalCurve, MiniBall,
             or RationalBezier
         :param kwargs: plotting options following matplotlib standards and syntax
-
-        :return: matplotlib axis
         """
         type_to_plot = self.analyze_object(object_to_plot)
 
         match type_to_plot:
             case "is_line":
                 self._plot_line(object_to_plot, **kwargs)
             case "is_point":
@@ -109,14 +134,20 @@
                 self._plot_rational_curve(object_to_plot, **kwargs)
             case "is_rational_bezier":
                 self._plot_rational_bezier(object_to_plot, **kwargs)
             case "is_rational_mechanism":
                 self._plot_rational_mechanism(object_to_plot, **kwargs)
             case "is_interactive":
                 self._plot_interactive(object_to_plot, **kwargs)
+            case "is_miniball":
+                self._plot_miniball(object_to_plot, **kwargs)
+            case "is_line_segment":
+                self._plot_line_segment(object_to_plot, **kwargs)
+            case "is_point_orbit":
+                self._plot_point_orbit(object_to_plot, **kwargs)
 
     def analyze_object(self, object_to_plot):
         """
         Analyze the object to plot
 
         :param object_to_plot: NormalizedLine, PointHomogeneous, RationalMechanism,
             MotionFactorization, DualQuaternion, TransfMatrix, RationalCurve
@@ -139,14 +170,20 @@
             return "is_rational_bezier"
         elif isinstance(object_to_plot, RationalCurve):
             return "is_rational_curve"
         elif isinstance(object_to_plot, DualQuaternion):
             return "is_dq"
         elif isinstance(object_to_plot, TransfMatrix):
             return "is_transf_matrix"
+        elif isinstance(object_to_plot, MiniBall):
+            return "is_miniball"
+        elif isinstance(object_to_plot, LineSegment):
+            return "is_line_segment"
+        elif isinstance(object_to_plot, PointOrbit):
+            return "is_point_orbit"
         else:
             raise TypeError(
                 "Other types than NormalizedLine, PointHomogeneous, RationalMechanism, "
                 "MotionFactorization or DualQuaternion not yet implemented"
             )
 
     @staticmethod
@@ -249,42 +286,61 @@
         """
         if 'interval' in kwargs:
             interval = kwargs['interval']
             kwargs.pop('interval')
         else:
             interval = (0, 1)
 
+        if 'with_poses' in kwargs and kwargs['with_poses'] is True:
+            kwargs.pop('with_poses')
+
+            if interval == 'closed':
+                # tangent half-angle substitution for closed curves
+                t_space = np.tan(np.linspace(-np.pi / 2, np.pi / 2, 51))
+            else:
+                t_space = np.linspace(interval[0], interval[1], 50)
+
+            for t in t_space:
+                pose_dq = DualQuaternion(curve.evaluate(t))
+                self._plot_dual_quaternion(pose_dq)
+
         x, y, z = curve.get_plot_data(interval, self.steps)
 
         if 'label' not in kwargs:
             kwargs['label'] = 'curve'
 
         self.ax.plot(x, y, z, **kwargs)
 
     @_plotting_decorator
-    def _plot_rational_bezier(self, bezier: RationalBezier, **kwargs):
+    def _plot_rational_bezier(self,
+                              bezier: RationalBezier,
+                              plot_control_points: bool = True,
+                              **kwargs):
         """
         Plot a rational Bezier curve
 
         :param bezier: RationalBezier
+        :param plot_control_points: plot control points
         :param kwargs: interval and matplotlib options
         """
         if 'interval' in kwargs:
             interval = kwargs['interval']
             kwargs.pop('interval')
         else:
             interval = (0, 1)
 
         x, y, z, x_cp, y_cp, z_cp = bezier.get_plot_data(interval, self.steps)
 
         if 'label' not in kwargs:
             kwargs['label'] = "bezier curve"
 
         self.ax.plot(x, y, z, **kwargs)
-        self.ax.plot(x_cp, y_cp, z_cp, "ro:")
+
+        if plot_control_points:
+            self.ax.plot(x_cp, y_cp, z_cp, "ro:")
 
     @_plotting_decorator
     def _plot_motion_factorization(self, factorization: MotionFactorization, **kwargs):
         """
         Plot a motion factorization
 
         :param factorization: MotionFactorization
@@ -332,14 +388,15 @@
             kwargs['label'] = "end effector"
 
         x, y, z = zip(*ee_points)
         self.ax.plot(x, y, z, **kwargs)
 
         self._plot_tool_path(mechanism, **kwargs)
 
+    @_plotting_decorator
     def _plot_tool_path(self, mechanism: RationalMechanism, **kwargs):
         # plot end effector path
         t_lin = np.linspace(0, 2 * np.pi, self.steps)
         t = [mechanism.factorizations[0].joint_angle_to_t_param(t_lin[i])
              for i in range(self.steps)]
 
         ee_points = [mechanism.factorizations[0].direct_kinematics_of_tool(
@@ -347,14 +404,52 @@
 
         kwargs['label'] = "tool path"
 
         x, y, z = zip(*ee_points)
         self.ax.plot(x, y, z, **kwargs)
 
     @_plotting_decorator
+    def _plot_miniball(self, ball: MiniBall, **kwargs):
+        """
+        Plot a ball
+        """
+        if 'label' not in kwargs:
+            kwargs['label'] = "Miniball of Bezier curve"
+        if 'alpha' not in kwargs:
+            kwargs['alpha'] = 0.15
+
+        x, y, z = ball.get_plot_data()
+
+        self.ax.plot_surface(x, y, z, **kwargs)
+
+    @_plotting_decorator
+    def _plot_point_orbit(self, orbit: PointOrbit, **kwargs):
+        """
+        Plot a sphere of given point orbit
+        """
+        if 'alpha' not in kwargs:
+            kwargs['alpha'] = 0.15
+
+        x, y, z = orbit.get_plot_data()
+
+        self.ax.plot_surface(x, y, z, **kwargs)
+
+    @_plotting_decorator
+    def _plot_line_segment(self, segment: LineSegment, **kwargs):
+        """
+        Plot a line segment
+        """
+        x, y, z = segment.get_plot_data()
+
+        if 'alpha' not in kwargs:
+            kwargs['alpha'] = 0.2
+
+        self.ax.plot_surface(x, y, z, **kwargs)
+
+    @_plotting_decorator
     def _plot_interactive(self,
                           mechanism: RationalMechanism,
                           show_tool: bool = True,
                           **kwargs):
         """
         Plot a mechanism in interactive mode
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/PointHomogeneous.py` & `rational_linkages-1.5.0/python/rational_linkages/PointHomogeneous.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from math import isclose
-
 import numpy as np
 
 from .TransfMatrix import TransfMatrix
 
 # Forward declarations for class names
 DualQuaternion = "DualQuaternion"
 
@@ -52,27 +50,29 @@
                 self.coordinates = np.asarray(point, dtype='float64')
             except Exception:
                 self.coordinates = point
                 self.is_real = False
         else:
             self.coordinates = np.asarray(point, dtype='float64')
 
-        if self.is_real and isclose(self.coordinates[0], 0.0):  # point at infinity
+        if self.is_real and np.allclose(np.array([self.coordinates[0]]), np.array([0.0])):  # point at infinity
             self.is_at_infinity = True
             self.coordinates_normalized = None
         elif self.is_real:
             self.is_at_infinity = False
             self.coordinates_normalized = self.normalize()
         else:
             self.is_at_infinity = False
             self.coordinates_normalized = None
 
         #if len(self.coordinates_normalized) == 4:  # point in PR3
         #    self.as_dq_array = self.point2dq_array()
 
+        self.orbit = None
+
     @classmethod
     def at_origin_in_2d(cls):
         """
         Create homogeneous point at origin in 2D
 
         :return: PointHomogeneous
         """
@@ -181,14 +181,28 @@
         :rtype: np.ndarray
         """
         mat = np.eye(4)
         if len(self.coordinates_normalized) == 3:  # point in PR2
             mat[1:3, 0] = self.coordinates_normalized[1:3]
         elif len(self.coordinates_normalized) == 4:
             mat[1:4, 0] = self.coordinates_normalized[1:4]
+
+        # affine displacement in R12
+        elif len(self.coordinates_normalized) == 12:
+            mat[1:4, 0] = self.coordinates_normalized[0:3]
+            mat[1:4, 1] = self.coordinates_normalized[3:6]
+            mat[1:4, 2] = self.coordinates_normalized[6:9]
+            mat[1:4, 3] = self.coordinates_normalized[9:12]
+
+        # affine displacement in PR12
+        elif len(self.coordinates_normalized) == 13:
+            mat[1:4, 0] = self.coordinates_normalized[1:4]
+            mat[1:4, 1] = self.coordinates_normalized[4:7]
+            mat[1:4, 2] = self.coordinates_normalized[7:10]
+            mat[1:4, 3] = self.coordinates_normalized[10:13]
         else:
             raise ValueError("PointHomogeneous: point has to be in PR2 or PR3")
 
         return mat
 
     def point2dq_array(self) -> np.ndarray:
         """
@@ -262,7 +276,75 @@
 
         point_expr = [Expr(coord) if not isinstance(coord, Number) else coord
                       for coord in self.coordinates]
         point = [coord.subs(t, t_param).evalf().args[0]
                  if not isinstance(coord, Number) else coord
                  for coord in point_expr]
         return PointHomogeneous(np.asarray(point, dtype="float64"))
+
+    def get_point_orbit(self,
+                        acting_center: "PointHomogeneous",
+                        acting_radius: float,
+                        metric: "AffineMetric",
+                        ) -> tuple[np.ndarray, float]:
+        """
+        Get point orbit
+
+
+
+        :param PointHomogeneous acting_center: center of the acting ball
+        :param float acting_radius: radius of the orbit ball
+        :param AffineMetric metric: metric of the curve
+
+        :return: point center and radius squared
+        :rtype: tuple[np.ndarray, float]
+        """
+        point_center = acting_center.point2matrix() @ self.coordinates_normalized
+
+        coords_3d = self.normalized_in_3d()
+        radius_squared = acting_radius ** 2 * (1/metric.total_mass + np.sum([(coord ** 2 / metric.inertia_eigen_vals[i]) for i, coord in enumerate(coords_3d)]))
+
+        radius = np.sqrt(radius_squared)
+        self.set_point_orbit(point_center, radius)
+        return point_center, radius
+
+    def set_point_orbit(self, orbit_center: "PointHomogeneous", orbit_radius: float):
+        """
+        Set the orbit of the point
+        """
+        self.orbit = PointOrbit(orbit_center, orbit_radius)
+
+
+class PointOrbit:
+    def __init__(self, point_center, radius):
+        """
+
+        """
+        if not isinstance(point_center, PointHomogeneous):
+            self.center = PointHomogeneous(point_center)
+        else:
+            self.center = point_center
+
+        self.radius = radius
+
+    def get_plot_data(self) -> tuple:
+        """
+        Get data for plotting in 3D space
+
+        :return: surface coordinates
+        :rtype: tuple
+        """
+        if len(self.center.coordinates) == 4:
+            # Create the 3D sphere representing the circle
+            u = np.linspace(0, 2 * np.pi, 10)
+            v = np.linspace(0, np.pi, 10)
+
+            x = (self.radius * np.outer(np.cos(u), np.sin(v))
+                 + self.center.normalized_in_3d()[0])
+            y = (self.radius * np.outer(np.sin(u), np.sin(v))
+                 + self.center.normalized_in_3d()[1])
+            z = (self.radius * np.outer(np.ones(np.size(u)), np.cos(v))
+                 + self.center.normalized_in_3d()[2])
+        else:
+            raise ValueError("Cannot plot ball due to incompatible dimension.")
+
+        return x, y, z
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/Quaternion.py` & `rational_linkages-1.5.0/python/rational_linkages/Quaternion.py`

 * *Files identical despite different names*

### Comparing `rational-linkages-1.4.2/python/rational_linkages/RationalCurve.py` & `rational_linkages-1.5.0/python/rational_linkages/RationalCurve.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from copy import deepcopy
 from typing import Union
 
 import numpy as np
 import sympy as sp
 
 from .PointHomogeneous import PointHomogeneous
+from .DualQuaternion import DualQuaternion
 
 MotionFactorization = "MotionFactorization"
 
 
 class RationalCurve:
     """
     Class representing rational curves in n-dimensional space, where the first row is
@@ -17,14 +18,19 @@
     This class allows you to work with rational curves defined by parametric equations.
 
     :ivar coeffs: Coefficients of parametric equations of the curve.
     :ivar dimension: The dimension of the curve, excluding the homogeneous coordinate.
     :ivar degree: The degree of the curve.
     :ivar symbolic: Symbolic expressions for the parametric equations of the curve.
     :ivar set_of_polynomials: A set of polynomials representing the curve.
+    :ivar symbolic_inversed: Symbolic expressions for the parametric equations of the
+        inversed curve.
+    :ivar set_of_polynomials_inversed: A set of polynomials representing the inversed
+        curve.
+    :ivar is_motion: True if the curve is a motion curve, False otherwise.
 
     :examples:
 
     .. testcode::
 
         # Limancon of Pascal -- from polynomial equations
 
@@ -67,14 +73,18 @@
 
         self.coeffs = self.get_coeffs()
         self.symbolic, _ = self.get_symbolic_expressions(self.coeffs)
 
         self.coeffs_inversed = self.inverse_coeffs()
         self.symbolic_inversed, self.set_of_polynomials_inversed = self.get_symbolic_expressions(self.coeffs_inversed)
 
+        # check if the curve is a motion curve
+        self.is_motion = self.dimension == 7
+        self.is_affine_motion = self.dimension == 12
+
     @classmethod
     def from_coeffs(cls, coeffs: np.ndarray) -> "RationalCurve":
         """
         Construct rational curve from coefficients
 
         :coeffs: np.ndarray - coefficients of the curve
 
@@ -136,15 +146,17 @@
                         self.set_of_polynomials[i].all_coeffs()
                     )
         return coeffs
 
     def __repr__(self):
         return f"RationalCurve({self.symbolic})"
 
-    def curve2bezier(self, reparametrization: bool = False) -> list[PointHomogeneous]:
+    def curve2bezier_control_points(self,
+                                    reparametrization: bool = False
+                                    ) -> list[PointHomogeneous]:
         """
         Convert a curve to a Bezier curve using the Bernstein polynomials
 
         :param bool reparametrization: if True, the curve is mapped to the [-1,1]
 
         :return: list of Bezier control points
         :rtype: list[PointHomogeneous]
@@ -174,16 +186,16 @@
         # Flatten the list
         equations_coeffs = [coeff for coeffs in equations_coeffs for coeff in coeffs]
 
         # Solve the equations
         points_sol = sp.linsolve(equations_coeffs, points_flattened)
         # Convert the solutions to numpy arrays (get points)
         points_array = np.array(points_sol.args[0], dtype="float64").reshape(
-            self.degree + 1, self.dimension + 1
-        )
+            self.degree + 1, self.dimension + 1)
+
         points_objects = [PointHomogeneous()] * (self.degree + 1)
         for i in range(self.degree + 1):
             points_objects[i] = PointHomogeneous(points_array[i, :])
 
         return points_objects
 
     def get_bernstein_polynomial_equations(
@@ -215,15 +227,17 @@
 
         # Initialize the polynomial expression list
         expr = []
 
         # Generate the polynomial expression using the Bernstein polynomials
         for i in range(degree + 1):
             polynomial_expr = sp.binomial(degree, i) * t**i * (1 - t) ** (degree - i)
-            expr.append(sp.simplify(polynomial_expr))
+            #expr.append(sp.simplify(polynomial_expr))
+            expr.append(polynomial_expr)
+            # TODO: simplify bottleneck
 
         return expr
 
     def inverse_coeffs(self) -> np.ndarray:
         """
         Get the coefficients of the inverse curve
 
@@ -333,16 +347,14 @@
         :param Union[str, tuple] interval: interval of the parameter t, if 'closed',
             the closed-loop curve is parametrized using tangent half-angle substitution
         :param int steps: number of numerical steps in the interval
 
         :return: tuple of np.ndarray - (x, y, z) coordinates of the curve
         :rtype: tuple[np.ndarray, np.ndarray, np.ndarray]
         """
-        from .DualQuaternion import DualQuaternion
-
         t = sp.Symbol("t")
 
         if interval == 'closed':
             # tangent half-angle substitution for closed curves
             t_space = np.tan(np.linspace(-np.pi/2, np.pi/2, steps + 1))
         else:
             t_space = np.linspace(interval[0], interval[1], steps)
@@ -355,15 +367,121 @@
 
         # plot the curve
         curve_points = [PointHomogeneous()] * steps
         for i in range(steps):
             point = self.evaluate(t_space[i])
 
             # if it is a pose in SE3, convert it to a point via matrix mapping
-            if self.dimension == 7:
+            if self.is_motion:
                 point = DualQuaternion(point).dq2point_via_matrix()
                 point = np.concatenate((np.array([1]), point))
+            elif self.is_affine_motion:
+                point = point[:4]
 
             curve_points[i] = PointHomogeneous([point[0], point[-3], point[-2], point[-1]])
         x, y, z = zip(*[curve_points[i].normalized_in_3d() for i in range(steps)])
         return x, y, z
 
+    def get_curve_in_pr12(self) -> "RationalCurve":
+        """
+        Get the representation of the curve in PR12
+
+        :return: curve in PR12
+        :rtype: RationalCurve
+        """
+        if not self.is_motion:
+            raise ValueError("The curve is not a motion curve, cannot convert to PR12")
+
+        t = sp.Symbol("t")
+
+        # convert the motion curve to a dual quaternion, then map to matrix
+        curve_matrix = DualQuaternion(self.symbolic).dq2matrix(normalize=False)
+
+        # save the not normalized coordinate
+        curve_p = curve_matrix[0, 0]
+        # transpose the matrix so the flatten() provides right order (vector by vector)
+        curve_r12 = curve_matrix[1:4, :].T.flatten()
+
+        # create PR12 vector of polynomial equations
+        curve_pr12 = np.concatenate((np.array([curve_p]), curve_r12))
+        curve_poly = [sp.Poly(curve, t) for curve in curve_pr12]
+
+        return RationalCurve(curve_poly)
+
+    def split_in_beziers(self,
+                         metric: Union[str, "AffineMetric"] = "euclidean",
+                         min_splits: int = 0) -> list["BezierSegment"]:
+        """
+        Split the curve into Bezier curves with positive weights of control points.
+
+        The curve is split into Bezier curves using the De Casteljau algorithm.
+
+        :param int min_splits: minimal number of splits to be performed
+        :param Union[str, AffineMetric] metric: metric for the optimization
+
+        :return: list of RationalBezier objects
+        :rtype: list[RationalBezier]
+        """
+        if self.is_motion:
+            curve = self.get_curve_in_pr12()
+        else:
+            raise ValueError("The curve is not a motion curve, cannot "
+                             "split into Bezier curves")
+
+        from .RationalBezier import BezierSegment  # method import
+
+        # obtain Bezier curves for the curve and its reparametrized inverse part
+        bezier_curve_segments = [
+            # reparametrize the curve from the intervals [-1, 1]
+            BezierSegment(curve.curve2bezier_control_points(reparametrization=True),
+                          metric=metric,
+                          t_param=(False, [-1.0, 1.0])),
+            BezierSegment(curve.inverse_curve().curve2bezier_control_points(
+                reparametrization=True),
+                          metric=metric,
+                          t_param=(True, [-1.0, 1.0]))
+        ]
+
+        # split the Bezier curves until all control points have positive weights
+        while True:
+            new_segments = [
+                part for b_curve in bezier_curve_segments
+                for part in (
+                    b_curve.split_de_casteljau(metric=metric) if b_curve.check_for_control_points_at_infinity() or b_curve.check_for_negative_weights() else [b_curve])
+            ]
+
+            if not any(
+                    b_curve.check_for_control_points_at_infinity() or b_curve.check_for_negative_weights()
+                    for b_curve in new_segments):
+                if len(new_segments) < min_splits:
+                    new_segments = [
+                        part for b_curve in new_segments
+                        for part in b_curve.split_de_casteljau(metric=metric)
+                    ]
+                else:
+                    bezier_curve_segments = new_segments
+                    break
+
+            bezier_curve_segments = new_segments
+
+        return bezier_curve_segments
+
+    def get_path_length(self, num_of_points: int = 100) -> float:
+        """
+        Get the length of the curve path
+
+        Evaluates the curve in the given number of points and sums the distances between.
+
+        :param int num_of_points: number of discrete points to evaluate the curve
+
+        :return: length of the curve path
+        :rtype: float
+        """
+        t_space = np.tan(np.linspace(-np.pi/2, np.pi/2, num_of_points))
+        poses = [self.evaluate(t) for t in t_space]
+
+        points = [DualQuaternion(p).dq2point_via_matrix()
+                  for p in poses]
+
+        return np.sum(np.linalg.norm(np.diff(points, axis=0), axis=1))
+
+
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/RationalDualQuaternion.py` & `rational_linkages-1.5.0/python/rational_linkages/RationalDualQuaternion.py`

 * *Files identical despite different names*

### Comparing `rational-linkages-1.4.2/python/rational_linkages/RationalMechanism.py` & `rational_linkages-1.5.0/python/rational_linkages/RationalMechanism.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import sympy as sp
 
 from .DualQuaternion import DualQuaternion
 from .MotionFactorization import MotionFactorization
 from .NormalizedLine import NormalizedLine
 from .RationalCurve import RationalCurve
 from .TransfMatrix import TransfMatrix
-
-PointHomogeneous = 'PointHomogeneous'
+from .PointHomogeneous import PointHomogeneous
 
 
 class RationalMechanism(RationalCurve):
     """
     Class representing rational mechanisms in dual quaternion space.
 
     :ivar factorizations: list of MotionFactorization objects
@@ -71,16 +70,18 @@
         self.factorizations = factorizations
         self.num_joints = sum([f.number_of_factors for f in factorizations])
 
         self.is_linkage = True if len(self.factorizations) == 2 else False
 
         self.tool_frame = self._determine_tool(tool)
 
+        self.segments = None
+
         if self.is_linkage:
-            self.segments = self._get_line_segments_of_linkage()
+            self.update_segments()
 
     @classmethod
     def from_saved_file(cls, filename: str):
         """
         Load a linkage object from a file.
 
         :param str filename: name of the file to load the linkage object from
@@ -112,14 +113,17 @@
         if filename is None:
             filename = 'saved_mechanism.pkl'
         elif filename[-4:] == '.pkl':
             pass
         else:
             filename = filename + '.pkl'
 
+        # update the line segments (physical realization of the linkage) before saving
+        self.update_segments()
+
         with open(filename, 'wb') as file:
             pickle.dump(self, file)
 
     def _determine_tool(self, tool: Union[DualQuaternion, None, str]) -> DualQuaternion:
         """
         Determine the tool frame of the mechanism.
 
@@ -438,15 +442,15 @@
         :return: list of collision check colliding parameter values
         :rtype: list[float]
         """
         start_time = time()
         print("Collision check started...")
 
         # update the line segments (physical realization of the linkage)
-        self.segments = self._get_line_segments_of_linkage()
+        self.update_segments()
 
         iters = []
         # iterate over all line segments
         for ii in range(len(self.segments)):
             # for each line segment, iterate over all other line segments that are not
             # its immediate neighbors
             for jj in range(ii + 2, len(self.segments)):
@@ -656,14 +660,20 @@
             # common perpendicular to the two lines - there is none since they
             # intersect, therefore from the list of two points only 1 is needed
             inters_points, d, c = l0e.common_perpendicular_to_other_line(l1e)
             intersection_points[i] = PointHomogeneous.from_3d_point(inters_points[0])
 
         return intersection_points
 
+    def update_segments(self):
+        """
+        Update the line segments of the linkage.
+        """
+        self.segments = self._get_line_segments_of_linkage()
+
     def _get_line_segments_of_linkage(self) -> list:
         """
         Return the line segments of the linkage.
 
         Line segments are the physical realization of the linkage. This method obtains
         their motion equations using default connection points of the factorizations
         (default meaning the static points in the home configuration).
@@ -787,7 +797,36 @@
                                              min_joint_segment_length=min_joint_segment_length,
                                              max_iters=max_iters,
                                              **kwargs)
             case _:
                 raise ValueError("Invalid method.")
 
         return results
+
+    def points_at_parameter(self,
+                            t: float,
+                            inverted_part: bool = False,
+                            only_links: bool = False) -> list[PointHomogeneous]:
+        """
+        Get the points of the mechanism at the given parameter.
+
+        :param float t: parameter value
+        :param bool inverted_part: if True, return the evaluated points for the inverted
+            part of the mechanism
+        :param bool only_links: if True, instead of two points per joint segment,
+            return only the first one
+
+        :return: list of connection points of the mechanism
+        :rtype: list[PointHomogeneous]
+        """
+
+        branch0 = self.factorizations[0].direct_kinematics(t,
+                                                           inverted_part=inverted_part)
+        branch1 = self.factorizations[1].direct_kinematics(t,
+                                                           inverted_part=inverted_part)
+
+        points = branch0 + branch1[::-1]
+
+        if only_links:
+            points = [points[i] for i in range(0, len(points), 2)]
+
+        return [PointHomogeneous.from_3d_point(p) for p in points]
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/SingularityAnalysis.py` & `rational_linkages-1.5.0/python/rational_linkages/SingularityAnalysis.py`

 * *Files identical despite different names*

### Comparing `rational-linkages-1.4.2/python/rational_linkages/TransfMatrix.py` & `rational_linkages-1.5.0/python/rational_linkages/TransfMatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,23 @@
         mat[2, 1:4] = [np.sin(theta),
                        np.cos(theta) * np.cos(alpha),
                        -np.cos(theta) * np.sin(alpha)]
         mat[3, 1:4] = [0, np.sin(alpha), np.cos(alpha)]
 
         return cls(mat)
 
+    def array(self) -> np.array:
+        """
+        Return transformation matrix as 4x4 numpy array
+
+        :return: 4x4 numpy array
+        :rtype: np.array
+        """
+        return self.matrix
+
     def is_rotation(self):
         """
         Check if matrix is rotation matrix with determinant equal to 1
 
         :return: True if matrix is rotation
         """
         if np.isclose(np.linalg.det(self.rot_matrix()), 1):
@@ -386,15 +395,14 @@
         inv_translation = -inv_rotation @ self.t
 
         m = np.eye(4)
         m[1:4, 1:4] = inv_rotation
         m[1:4, 0] = inv_translation
         return TransfMatrix(m)
 
-
     def get_plot_data(self):
         """
         Return three quiver coordinates for plotting
 
         :return: 6-dimensional numpy array of point and vector direction
         """
         x_vec = np.concatenate((self.t, self.n))
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/__init__.py` & `rational_linkages-1.5.0/python/rational_linkages/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from .AffineMetric import AffineMetric
 from .CollisionFreeOptimization import CollisionFreeOptimization, CombinatorialSearch
 from .DualQuaternion import DualQuaternion
 from .DualQuaternionAction import DualQuaternionAction
 from .ExudynAnalysis import ExudynAnalysis
 from .FactorizationProvider import FactorizationProvider
 from .Linkage import LineSegment, Linkage, PointsConnection
 from .MiniBall import MiniBall
 from .MotionFactorization import MotionFactorization
 from .MotionInterpolation import MotionInterpolation
 from .NormalizedLine import NormalizedLine
 from .Plotter import Plotter
 from .PointHomogeneous import PointHomogeneous
 from .Quaternion import Quaternion
-from .RationalBezier import RationalBezier
+from .RationalBezier import RationalBezier, BezierSegment
 from .RationalCurve import RationalCurve
 from .RationalDualQuaternion import RationalDualQuaternion
 from .RationalMechanism import RationalMechanism
 from .TransfMatrix import TransfMatrix
+from .CollisionAnalyser import CollisionAnalyser
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages/data/bennett_ark24.pkl` & `rational_linkages-1.5.0/python/rational_linkages/data/bennett_ark24.pkl`

 * *Files identical despite different names*

### Comparing `rational-linkages-1.4.2/python/rational_linkages/data/collisions_free_6r.pkl` & `rational_linkages-1.5.0/python/rational_linkages/data/collisions_free_6r.pkl`

 * *Files identical despite different names*

### Comparing `rational-linkages-1.4.2/python/rational_linkages/data/plane_fold_6r.pkl` & `rational_linkages-1.5.0/python/rational_linkages/data/plane_fold_6r.pkl`

 * *Files identical despite different names*

### Comparing `rational-linkages-1.4.2/python/rational_linkages.egg-info/PKG-INFO` & `rational_linkages-1.5.0/python/rational_linkages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rational-linkages
-Version: 1.4.2
-Summary: Rational Linkages Toolbox
+Version: 1.5.0
+Summary: Rational Linkages
 Author-email: Daniel Huczala <daniel.huczala@uibk.ac.at>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -707,25 +707,26 @@
 Requires-Dist: flake8-pyproject; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 [![build](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/badges/main/pipeline.svg)](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/-/jobs)
 [![Documentation Status](https://readthedocs.org/projects/rational-linkages/badge/?version=latest)](https://rational-linkages.readthedocs.io/?badge=latest)
-[![PyPI version](https://img.shields.io/pypi/v/rational-linkages.svg)](https://pypi.org/project/rational-linkages/)[![coverage](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/badges/main/coverage.svg?job=run_tests)](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/-/jobs)
+[![PyPI version](https://img.shields.io/pypi/v/rational-linkages.svg)](https://pypi.org/project/rational-linkages/)
+[![coverage](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/badges/main/coverage.svg?job=test_coverage)](https://git.uibk.ac.at/geometrie-vermessung/rational-linkages/-/jobs)
 [![GitHub issues](https://img.shields.io/github/issues/hucik14/rl-issues)](https://github.com/hucik14/rl-issues/issues)
 [![Python](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue.svg)]()
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/hucik14/rl-issues/HEAD?labpath=jupyter_ntbs%2Fsynthesis_bennett.ipynb)
 
 
 # Rational Linkages
 
-Python-based toolbox for synthesis and rapid-prototyping of rational linkages, 
+Python-based package for synthesis and rapid-prototyping of rational linkages, 
 developed by the Unit of Geometry and Surveying, University of Innsbruck, Austria. 
-The documentation is hosted on Read the Docs, available here: 
+The **documentation with examples** is hosted on Read the Docs, available here: 
 [Rational Linkages Documentation](https://rational-linkages.readthedocs.io/).
 
 ## Intallation instuctions
 
 Recommended Python version is **3.11**, when it provides the smoothest plotting 
 (but 3.10 or higher are supported). Python 3.11 is also the version used for 
 development.
@@ -742,15 +743,15 @@
     
     <code>git clone https://git.uibk.ac.at/geometrie-vermessung/rational-linkages.git </code>
 
 2. Navigate to the repository folder
 
     <code>cd rational-linkages</code>
 
-3. Install the *editable* version of the pakcage using pip:
+3. Install the *editable* version of the package using pip:
 
     <code>pip install -e .</code>
 
 ## Tutorials, issues, usage, and contributions
 
 See the [documentation examples](https://rational-linkages.readthedocs.io/latest/general/overview.html) 
 for tutorials and usage examples.
```

### Comparing `rational-linkages-1.4.2/python/rational_linkages.egg-info/SOURCES.txt` & `rational_linkages-1.5.0/python/rational_linkages.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
-python/rational_linkages/AffineMatrix.py
 python/rational_linkages/AffineMetric.py
 python/rational_linkages/ButtonID.py
+python/rational_linkages/CollisionAnalyser.py
 python/rational_linkages/CollisionFreeOptimization.py
 python/rational_linkages/DualQuaternion.py
 python/rational_linkages/DualQuaternionAction.py
 python/rational_linkages/ExudynAnalysis.py
 python/rational_linkages/FactorizationProvider.py
 python/rational_linkages/Linkage.py
 python/rational_linkages/MiniBall.py
@@ -22,14 +22,15 @@
 python/rational_linkages/RationalCurve.py
 python/rational_linkages/RationalDualQuaternion.py
 python/rational_linkages/RationalMechanism.py
 python/rational_linkages/SingularityAnalysis.py
 python/rational_linkages/TransfMatrix.py
 python/rational_linkages/__init__.py
 python/rational_linkages/models.py
+python/rational_linkages/utils.py
 python/rational_linkages.egg-info/PKG-INFO
 python/rational_linkages.egg-info/SOURCES.txt
 python/rational_linkages.egg-info/dependency_links.txt
 python/rational_linkages.egg-info/requires.txt
 python/rational_linkages.egg-info/top_level.txt
 python/rational_linkages/data/bennett_ark24.pkl
 python/rational_linkages/data/collisions_free_6r.pkl
```

