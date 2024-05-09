# Comparing `tmp/robynpy-0.0.1.tar.gz` & `tmp/robynpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robynpy-0.0.1.tar", last modified: Wed May  8 18:25:04 2024, max compression
+gzip compressed data, was "robynpy-0.0.2.tar", last modified: Thu May  9 05:40:06 2024, max compression
```

## Comparing `robynpy-0.0.1.tar` & `robynpy-0.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-08 18:25:04.799402 robynpy-0.0.1/
--rw-r--r--   0 sandeepmane   (501) staff       (20)     1092 2024-05-02 01:32:30.000000 robynpy-0.0.1/LICENSE
--rw-r--r--   0 sandeepmane   (501) staff       (20)     5401 2024-05-08 18:25:04.797943 robynpy-0.0.1/PKG-INFO
--rw-r--r--   0 sandeepmane   (501) staff       (20)     4383 2024-05-08 06:06:41.000000 robynpy-0.0.1/README.md
--rw-r--r--   0 sandeepmane   (501) staff       (20)     1084 2024-05-08 02:56:50.000000 robynpy-0.0.1/pyproject.toml
--rw-r--r--   0 sandeepmane   (501) staff       (20)       38 2024-05-08 18:25:04.799480 robynpy-0.0.1/setup.cfg
-drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-08 18:25:04.725784 robynpy-0.0.1/src/
-drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-08 18:25:04.746152 robynpy-0.0.1/src/data/
--rw-r--r--   0 sandeepmane   (501) staff       (20)  3909388 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/data/dt_prophet_holidays.csv
--rw-r--r--   0 sandeepmane   (501) staff       (20)  4599493 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/data/dt_prophet_holidays_old.csv
--rw-r--r--   0 sandeepmane   (501) staff       (20)    23287 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/data/dt_simulated_weekly.csv
--rw-r--r--   0 sandeepmane   (501) staff       (20)    22097 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/data/dt_simulated_weekly_old.csv
-drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-08 18:25:04.775889 robynpy-0.0.1/src/robyn/
--rw-r--r--   0 sandeepmane   (501) staff       (20)        0 2024-05-02 01:36:06.000000 robynpy-0.0.1/src/robyn/__init__.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    63320 2024-05-08 18:19:54.000000 robynpy-0.0.1/src/robyn/allocator.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)     2494 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/robyn/auxiliary.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)     8534 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/robyn/calibration.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    60582 2024-05-07 22:07:12.000000 robynpy-0.0.1/src/robyn/checks.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    33701 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/robyn/cluster.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)     8644 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/robyn/convergence.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)     1119 2024-05-08 18:19:54.000000 robynpy-0.0.1/src/robyn/data.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)     5984 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/robyn/exports.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    47589 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/robyn/inputs.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    12425 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/robyn/json.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    63325 2024-05-07 20:20:39.000000 robynpy-0.0.1/src/robyn/model.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    13298 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/robyn/outputs.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    32581 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/robyn/pareto.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    75111 2024-05-07 20:20:39.000000 robynpy-0.0.1/src/robyn/plots.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    15867 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/robyn/refresh.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    13683 2024-05-07 21:59:45.000000 robynpy-0.0.1/src/robyn/response.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    23850 2024-05-02 01:32:30.000000 robynpy-0.0.1/src/robyn/transformation.py
-drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-08 18:25:04.794221 robynpy-0.0.1/src/robynpy.egg-info/
--rw-r--r--   0 sandeepmane   (501) staff       (20)     5401 2024-05-08 18:25:04.000000 robynpy-0.0.1/src/robynpy.egg-info/PKG-INFO
--rw-r--r--   0 sandeepmane   (501) staff       (20)      927 2024-05-08 18:25:04.000000 robynpy-0.0.1/src/robynpy.egg-info/SOURCES.txt
--rw-r--r--   0 sandeepmane   (501) staff       (20)        1 2024-05-08 18:25:04.000000 robynpy-0.0.1/src/robynpy.egg-info/dependency_links.txt
--rw-r--r--   0 sandeepmane   (501) staff       (20)      137 2024-05-08 18:25:04.000000 robynpy-0.0.1/src/robynpy.egg-info/requires.txt
--rw-r--r--   0 sandeepmane   (501) staff       (20)       19 2024-05-08 18:25:04.000000 robynpy-0.0.1/src/robynpy.egg-info/top_level.txt
-drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-08 18:25:04.782590 robynpy-0.0.1/src/scripts/
--rw-r--r--   0 sandeepmane   (501) staff       (20)        0 2024-05-02 01:32:31.000000 robynpy-0.0.1/src/scripts/__init__.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    22580 2024-05-08 18:19:54.000000 robynpy-0.0.1/src/scripts/demo.py
-drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-08 18:25:04.791342 robynpy-0.0.1/tests/
--rw-r--r--   0 sandeepmane   (501) staff       (20)     3845 2024-03-20 02:10:22.000000 robynpy-0.0.1/tests/test_allocator.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)     8481 2024-05-02 05:25:55.000000 robynpy-0.0.1/tests/test_inputs.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)     7791 2024-05-02 05:26:12.000000 robynpy-0.0.1/tests/test_json.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)    15673 2024-03-20 02:10:22.000000 robynpy-0.0.1/tests/test_model.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)     5797 2024-05-02 05:27:22.000000 robynpy-0.0.1/tests/test_outputs.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)     3299 2024-05-02 05:27:33.000000 robynpy-0.0.1/tests/test_refresh.py
--rw-r--r--   0 sandeepmane   (501) staff       (20)     3927 2024-05-02 01:33:26.000000 robynpy-0.0.1/tests/test_response.py
+drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-09 05:40:06.684353 robynpy-0.0.2/
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     1092 2024-05-02 01:32:30.000000 robynpy-0.0.2/LICENSE
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     5423 2024-05-09 05:40:06.683199 robynpy-0.0.2/PKG-INFO
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     4383 2024-05-08 06:06:41.000000 robynpy-0.0.2/README.md
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     1098 2024-05-09 05:39:51.000000 robynpy-0.0.2/pyproject.toml
+-rw-r--r--   0 sandeepmane   (501) staff       (20)       38 2024-05-09 05:40:06.684440 robynpy-0.0.2/setup.cfg
+drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-09 05:40:06.634754 robynpy-0.0.2/src/
+drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-09 05:40:06.653512 robynpy-0.0.2/src/data/
+-rw-r--r--   0 sandeepmane   (501) staff       (20)  3909388 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/data/dt_prophet_holidays.csv
+-rw-r--r--   0 sandeepmane   (501) staff       (20)  4599493 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/data/dt_prophet_holidays_old.csv
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    23287 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/data/dt_simulated_weekly.csv
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    22097 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/data/dt_simulated_weekly_old.csv
+drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-09 05:40:06.670898 robynpy-0.0.2/src/robyn/
+-rw-r--r--   0 sandeepmane   (501) staff       (20)        0 2024-05-02 01:36:06.000000 robynpy-0.0.2/src/robyn/__init__.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    63320 2024-05-08 18:19:54.000000 robynpy-0.0.2/src/robyn/allocator.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     2494 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/robyn/auxiliary.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     8534 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/robyn/calibration.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    60582 2024-05-07 22:07:12.000000 robynpy-0.0.2/src/robyn/checks.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    33701 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/robyn/cluster.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     8644 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/robyn/convergence.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     1121 2024-05-09 05:31:10.000000 robynpy-0.0.2/src/robyn/data.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     5984 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/robyn/exports.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    47589 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/robyn/inputs.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    12425 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/robyn/json.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    63325 2024-05-07 20:20:39.000000 robynpy-0.0.2/src/robyn/model.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    13298 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/robyn/outputs.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    32581 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/robyn/pareto.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    75111 2024-05-07 20:20:39.000000 robynpy-0.0.2/src/robyn/plots.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    15867 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/robyn/refresh.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    13683 2024-05-07 21:59:45.000000 robynpy-0.0.2/src/robyn/response.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    23850 2024-05-02 01:32:30.000000 robynpy-0.0.2/src/robyn/transformation.py
+drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-09 05:40:06.682722 robynpy-0.0.2/src/robynpy.egg-info/
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     5423 2024-05-09 05:40:06.000000 robynpy-0.0.2/src/robynpy.egg-info/PKG-INFO
+-rw-r--r--   0 sandeepmane   (501) staff       (20)      927 2024-05-09 05:40:06.000000 robynpy-0.0.2/src/robynpy.egg-info/SOURCES.txt
+-rw-r--r--   0 sandeepmane   (501) staff       (20)        1 2024-05-09 05:40:06.000000 robynpy-0.0.2/src/robynpy.egg-info/dependency_links.txt
+-rw-r--r--   0 sandeepmane   (501) staff       (20)      144 2024-05-09 05:40:06.000000 robynpy-0.0.2/src/robynpy.egg-info/requires.txt
+-rw-r--r--   0 sandeepmane   (501) staff       (20)       19 2024-05-09 05:40:06.000000 robynpy-0.0.2/src/robynpy.egg-info/top_level.txt
+drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-09 05:40:06.674938 robynpy-0.0.2/src/scripts/
+-rw-r--r--   0 sandeepmane   (501) staff       (20)        0 2024-05-02 01:32:31.000000 robynpy-0.0.2/src/scripts/__init__.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    22580 2024-05-08 21:29:37.000000 robynpy-0.0.2/src/scripts/demo.py
+drwxr-xr-x   0 sandeepmane   (501) staff       (20)        0 2024-05-09 05:40:06.681866 robynpy-0.0.2/tests/
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     3845 2024-03-20 02:10:22.000000 robynpy-0.0.2/tests/test_allocator.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     8481 2024-05-02 05:25:55.000000 robynpy-0.0.2/tests/test_inputs.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     7791 2024-05-02 05:26:12.000000 robynpy-0.0.2/tests/test_json.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)    15673 2024-03-20 02:10:22.000000 robynpy-0.0.2/tests/test_model.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     5797 2024-05-02 05:27:22.000000 robynpy-0.0.2/tests/test_outputs.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     3299 2024-05-02 05:27:33.000000 robynpy-0.0.2/tests/test_refresh.py
+-rw-r--r--   0 sandeepmane   (501) staff       (20)     3927 2024-05-02 01:33:26.000000 robynpy-0.0.2/tests/test_response.py
```

### Comparing `robynpy-0.0.1/LICENSE` & `robynpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/PKG-INFO` & `robynpy-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robynpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Robyn: Continuous & Semi-Automated MMM. The Open Source Marketing Mix Model Package from Meta Marketing Science
 Author-email: Gufeng Zhou <gufeng@meta.com>, Igor Skokan <igorskokan@meta.com>
 Project-URL: Homepage, https://github.com/facebookexperimental/Robyn
 Project-URL: Issues, https://github.com/facebookexperimental/Robyn/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,14 +22,15 @@
 Requires-Dist: nevergrad
 Requires-Dist: PyQt6
 Requires-Dist: nevergrad
 Requires-Dist: seaborn
 Requires-Dist: tqdm
 Requires-Dist: rpy2
 Requires-Dist: pytest
+Requires-Dist: plotly
 Requires-Dist: nlopt
 Requires-Dist: cmake
 
 # Robyn: Continuous & Semi-Automated MMM <img src='R/man/figures/logo.png' align="right" height="139px" />
 ### The Open Source Marketing Mix Model Package from Meta Marketing Science
 
 <!-- [![Pypi\_Status\_Badge](https://www.r-pkg.org/badges/version/Robyn)](https://cran.r-project.org/package=Robyn) [![Downloads](https://cranlogs.r-pkg.org/badges/grand-total/Robyn?color=green)](https://cranlogs.r-pkg.org/badges/grand-total/Robyn?color=green) [![Site](https://img.shields.io/badge/site-Robyn-blue.svg)](https://facebookexperimental.github.io/Robyn/) [![Facebook](https://img.shields.io/badge/group-Facebook-blue.svg)](https://www.facebook.com/groups/robynmmm/) [![CodeFactor](https://www.codefactor.io/repository/github/facebookexperimental/robyn/badge)](https://www.codefactor.io/repository/github/facebookexperimental/robyn) -->
```

### Comparing `robynpy-0.0.1/README.md` & `robynpy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/pyproject.toml` & `robynpy-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robynpy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Gufeng Zhou", email="gufeng@meta.com" },
   { name="Igor Skokan", email="igorskokan@meta.com" },
 ]
 description = "Robyn: Continuous & Semi-Automated MMM. The Open Source Marketing Mix Model Package from Meta Marketing Science"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -29,14 +29,15 @@
     "nevergrad",
     "PyQt6",
     "nevergrad",
     "seaborn",
     "tqdm",
     "rpy2",
     "pytest",
+    "plotly",
     "nlopt",
     "cmake",
 ]
 [tool.setuptools.packages.find]
 where = ["src"]
 [tool.setuptools.package-data]
 "*" = ["*.csv"]
```

### Comparing `robynpy-0.0.1/src/data/dt_prophet_holidays.csv` & `robynpy-0.0.2/src/data/dt_prophet_holidays.csv`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/data/dt_prophet_holidays_old.csv` & `robynpy-0.0.2/src/data/dt_prophet_holidays_old.csv`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/data/dt_simulated_weekly.csv` & `robynpy-0.0.2/src/data/dt_simulated_weekly.csv`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/data/dt_simulated_weekly_old.csv` & `robynpy-0.0.2/src/data/dt_simulated_weekly_old.csv`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/allocator.py` & `robynpy-0.0.2/src/robyn/allocator.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/auxiliary.py` & `robynpy-0.0.2/src/robyn/auxiliary.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/calibration.py` & `robynpy-0.0.2/src/robyn/calibration.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/checks.py` & `robynpy-0.0.2/src/robyn/checks.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/cluster.py` & `robynpy-0.0.2/src/robyn/cluster.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/convergence.py` & `robynpy-0.0.2/src/robyn/convergence.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/data.py` & `robynpy-0.0.2/src/robyn/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 import pandas as pd
 
 ### Manually Generated
 
 
 def dt_simulated_weekly():
-    csv_file = os.getcwd() + "../data/dt_simulated_weekly.csv"
+    csv_file = os.getcwd() + "/../data/dt_simulated_weekly.csv"
     return pd.read_csv(csv_file)
 
 
 def dt_prophet_holidays():
-    csv_file = os.getcwd() + "../data/dt_prophet_holidays.csv"
+    csv_file = os.getcwd() + "/../data/dt_prophet_holidays.csv"
     return pd.read_csv(csv_file)
 
 # def dt_simulated_weekly():
 #     csv_file = os.getcwd() + "/python/src/data/dt_simulated_weekly.csv"
 #     dir_path = os.path.dirname(os.path.realpath(__file__))
 #     csv_file = os.path.join(dir_path, '..', 'data', 'dt_simulated_weekly.csv')
 #     return pd.read_csv(csv_file)
```

### Comparing `robynpy-0.0.1/src/robyn/exports.py` & `robynpy-0.0.2/src/robyn/exports.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/inputs.py` & `robynpy-0.0.2/src/robyn/inputs.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/json.py` & `robynpy-0.0.2/src/robyn/json.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/model.py` & `robynpy-0.0.2/src/robyn/model.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/outputs.py` & `robynpy-0.0.2/src/robyn/outputs.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/pareto.py` & `robynpy-0.0.2/src/robyn/pareto.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/plots.py` & `robynpy-0.0.2/src/robyn/plots.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/refresh.py` & `robynpy-0.0.2/src/robyn/refresh.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/response.py` & `robynpy-0.0.2/src/robyn/response.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robyn/transformation.py` & `robynpy-0.0.2/src/robyn/transformation.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/robynpy.egg-info/PKG-INFO` & `robynpy-0.0.2/src/robynpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robynpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Robyn: Continuous & Semi-Automated MMM. The Open Source Marketing Mix Model Package from Meta Marketing Science
 Author-email: Gufeng Zhou <gufeng@meta.com>, Igor Skokan <igorskokan@meta.com>
 Project-URL: Homepage, https://github.com/facebookexperimental/Robyn
 Project-URL: Issues, https://github.com/facebookexperimental/Robyn/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,14 +22,15 @@
 Requires-Dist: nevergrad
 Requires-Dist: PyQt6
 Requires-Dist: nevergrad
 Requires-Dist: seaborn
 Requires-Dist: tqdm
 Requires-Dist: rpy2
 Requires-Dist: pytest
+Requires-Dist: plotly
 Requires-Dist: nlopt
 Requires-Dist: cmake
 
 # Robyn: Continuous & Semi-Automated MMM <img src='R/man/figures/logo.png' align="right" height="139px" />
 ### The Open Source Marketing Mix Model Package from Meta Marketing Science
 
 <!-- [![Pypi\_Status\_Badge](https://www.r-pkg.org/badges/version/Robyn)](https://cran.r-project.org/package=Robyn) [![Downloads](https://cranlogs.r-pkg.org/badges/grand-total/Robyn?color=green)](https://cranlogs.r-pkg.org/badges/grand-total/Robyn?color=green) [![Site](https://img.shields.io/badge/site-Robyn-blue.svg)](https://facebookexperimental.github.io/Robyn/) [![Facebook](https://img.shields.io/badge/group-Facebook-blue.svg)](https://www.facebook.com/groups/robynmmm/) [![CodeFactor](https://www.codefactor.io/repository/github/facebookexperimental/robyn/badge)](https://www.codefactor.io/repository/github/facebookexperimental/robyn) -->
```

### Comparing `robynpy-0.0.1/src/robynpy.egg-info/SOURCES.txt` & `robynpy-0.0.2/src/robynpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/src/scripts/demo.py` & `robynpy-0.0.2/src/scripts/demo.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/tests/test_allocator.py` & `robynpy-0.0.2/tests/test_allocator.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/tests/test_inputs.py` & `robynpy-0.0.2/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/tests/test_json.py` & `robynpy-0.0.2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/tests/test_model.py` & `robynpy-0.0.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/tests/test_outputs.py` & `robynpy-0.0.2/tests/test_outputs.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/tests/test_refresh.py` & `robynpy-0.0.2/tests/test_refresh.py`

 * *Files identical despite different names*

### Comparing `robynpy-0.0.1/tests/test_response.py` & `robynpy-0.0.2/tests/test_response.py`

 * *Files identical despite different names*

