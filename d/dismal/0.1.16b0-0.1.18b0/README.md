# Comparing `tmp/dismal-0.1.16b0.tar.gz` & `tmp/dismal-0.1.18b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dismal-0.1.16b0.tar", last modified: Thu May  2 16:13:46 2024, max compression
+gzip compressed data, was "dismal-0.1.18b0.tar", last modified: Thu May  9 12:10:39 2024, max compression
```

## Comparing `dismal-0.1.16b0.tar` & `dismal-0.1.18b0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:13:46.907658 dismal-0.1.16b0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 16:13:05.000000 dismal-0.1.16b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-02 16:13:46.907658 dismal-0.1.16b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-02 16:13:05.000000 dismal-0.1.16b0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:13:46.903658 dismal-0.1.16b0/dismal/
--rw-r--r--   0 runner    (1001) docker     (127)    12044 2024-05-02 16:13:05.000000 dismal-0.1.16b0/dismal/blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:13:05.000000 dismal-0.1.16b0/dismal/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-02 16:13:05.000000 dismal-0.1.16b0/dismal/callset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-02 16:13:05.000000 dismal-0.1.16b0/dismal/demesrepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-05-02 16:13:05.000000 dismal-0.1.16b0/dismal/demographicmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-02 16:13:05.000000 dismal-0.1.16b0/dismal/demography.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-02 16:13:05.000000 dismal-0.1.16b0/dismal/markov_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-05-02 16:13:05.000000 dismal-0.1.16b0/dismal/model_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-02 16:13:05.000000 dismal-0.1.16b0/dismal/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-02 16:13:05.000000 dismal-0.1.16b0/dismal/modelsimulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-02 16:13:05.000000 dismal-0.1.16b0/dismal/multimodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-02 16:13:05.000000 dismal-0.1.16b0/dismal/print_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:13:46.903658 dismal-0.1.16b0/dismal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-02 16:13:46.000000 dismal-0.1.16b0/dismal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-02 16:13:46.000000 dismal-0.1.16b0/dismal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:13:46.000000 dismal-0.1.16b0/dismal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 16:13:46.000000 dismal-0.1.16b0/dismal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 16:13:46.000000 dismal-0.1.16b0/dismal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:13:46.907658 dismal-0.1.16b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-02 16:13:05.000000 dismal-0.1.16b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:13:46.903658 dismal-0.1.16b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-02 16:13:05.000000 dismal-0.1.16b0/tests/test_callset.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 16:13:05.000000 dismal-0.1.16b0/tests/test_demography.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-02 16:13:05.000000 dismal-0.1.16b0/tests/test_markov_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-05-02 16:13:05.000000 dismal-0.1.16b0/tests/test_model_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-02 16:13:05.000000 dismal-0.1.16b0/tests/test_simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:10:39.027124 dismal-0.1.18b0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 12:10:01.000000 dismal-0.1.18b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-09 12:10:39.027124 dismal-0.1.18b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-09 12:10:01.000000 dismal-0.1.18b0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:10:39.027124 dismal-0.1.18b0/dismal/
+-rw-r--r--   0 runner    (1001) docker     (127)    12044 2024-05-09 12:10:01.000000 dismal-0.1.18b0/dismal/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:10:01.000000 dismal-0.1.18b0/dismal/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-09 12:10:01.000000 dismal-0.1.18b0/dismal/callset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-09 12:10:01.000000 dismal-0.1.18b0/dismal/demesrepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-05-09 12:10:01.000000 dismal-0.1.18b0/dismal/demographicmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-09 12:10:01.000000 dismal-0.1.18b0/dismal/demography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-09 12:10:01.000000 dismal-0.1.18b0/dismal/markov_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-05-09 12:10:01.000000 dismal-0.1.18b0/dismal/model_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-09 12:10:01.000000 dismal-0.1.18b0/dismal/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-09 12:10:01.000000 dismal-0.1.18b0/dismal/modelsimulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-09 12:10:01.000000 dismal-0.1.18b0/dismal/multimodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-09 12:10:01.000000 dismal-0.1.18b0/dismal/print_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:10:39.027124 dismal-0.1.18b0/dismal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-09 12:10:39.000000 dismal-0.1.18b0/dismal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-09 12:10:39.000000 dismal-0.1.18b0/dismal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:10:39.000000 dismal-0.1.18b0/dismal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-09 12:10:39.000000 dismal-0.1.18b0/dismal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 12:10:39.000000 dismal-0.1.18b0/dismal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:10:39.027124 dismal-0.1.18b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 12:10:01.000000 dismal-0.1.18b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:10:39.027124 dismal-0.1.18b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-09 12:10:01.000000 dismal-0.1.18b0/tests/test_callset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-09 12:10:01.000000 dismal-0.1.18b0/tests/test_demography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-09 12:10:01.000000 dismal-0.1.18b0/tests/test_markov_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-05-09 12:10:01.000000 dismal-0.1.18b0/tests/test_model_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-09 12:10:01.000000 dismal-0.1.18b0/tests/test_simulate.py
```

### Comparing `dismal-0.1.16b0/LICENSE` & `dismal-0.1.18b0/LICENSE`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/PKG-INFO` & `dismal-0.1.18b0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: dismal
-Version: 0.1.16b0
+Version: 0.1.18b0
+Summary: Demographic inference from the distribution of pairwise segregating sites
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: setuptools
 Requires-Dist: pyranges
 Requires-Dist: scikit-allel
 Requires-Dist: demes
 Requires-Dist: demesdraw
 Requires-Dist: matplotlib
 Requires-Dist: msprime
 Requires-Dist: seaborn
 Requires-Dist: tqdm
 Requires-Dist: tskit
 Requires-Dist: prettytable
+Requires-Dist: joblib
 
 DISMaL: Demographic Inference under the Structured Coalescent using Maximum Likelihood
 ======================================================================================
 
 ``DISMaL`` is a Python package for inferring historical demographies
 (specifically, population sizes, gene flow, and split times) from
 sequence data. It is an implementation of the *Generalised
@@ -33,13 +35,10 @@
 
 Documentation is hosted on ReadTheDocs: https://dismal.readthedocs.io/en/latest/
 
 
 Installation
 ------------
 
-DISMaL is currently only available as a pre-release from this GitHub
-repo. Install using:
+Install latest full release with Pip: `pip install dismal`
 
-::
-
-   pip install git+https://github.com/simonharnqvist/DISMaL.git#egg=dismal
+Or the development version from GitHub: `pip install git+https://github.com/simonharnqvist/DISMaL.git#egg=dismal`
```

### Comparing `dismal-0.1.16b0/README.rst` & `dismal-0.1.18b0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -15,13 +15,10 @@
 
 Documentation is hosted on ReadTheDocs: https://dismal.readthedocs.io/en/latest/
 
 
 Installation
 ------------
 
-DISMaL is currently only available as a pre-release from this GitHub
-repo. Install using:
+Install latest full release with Pip: `pip install dismal`
 
-::
-
-   pip install git+https://github.com/simonharnqvist/DISMaL.git#egg=dismal
+Or the development version from GitHub: `pip install git+https://github.com/simonharnqvist/DISMaL.git#egg=dismal`
```

### Comparing `dismal-0.1.16b0/dismal/blocking.py` & `dismal-0.1.18b0/dismal/blocking.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/dismal/callset.py` & `dismal-0.1.18b0/dismal/callset.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/dismal/demesrepresentation.py` & `dismal-0.1.18b0/dismal/demesrepresentation.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/dismal/demographicmodel.py` & `dismal-0.1.18b0/dismal/demographicmodel.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/dismal/demography.py` & `dismal-0.1.18b0/dismal/demography.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/dismal/markov_matrices.py` & `dismal-0.1.18b0/dismal/markov_matrices.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/dismal/model_instance.py` & `dismal-0.1.18b0/dismal/model_instance.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/dismal/models.py` & `dismal-0.1.18b0/dismal/models.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/dismal/modelsimulation.py` & `dismal-0.1.18b0/dismal/modelsimulation.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/dismal/multimodel.py` & `dismal-0.1.18b0/dismal/multimodel.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/dismal/print_results.py` & `dismal-0.1.18b0/dismal/print_results.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/dismal.egg-info/PKG-INFO` & `dismal-0.1.18b0/dismal.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: dismal
-Version: 0.1.16b0
+Version: 0.1.18b0
+Summary: Demographic inference from the distribution of pairwise segregating sites
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: setuptools
 Requires-Dist: pyranges
 Requires-Dist: scikit-allel
 Requires-Dist: demes
 Requires-Dist: demesdraw
 Requires-Dist: matplotlib
 Requires-Dist: msprime
 Requires-Dist: seaborn
 Requires-Dist: tqdm
 Requires-Dist: tskit
 Requires-Dist: prettytable
+Requires-Dist: joblib
 
 DISMaL: Demographic Inference under the Structured Coalescent using Maximum Likelihood
 ======================================================================================
 
 ``DISMaL`` is a Python package for inferring historical demographies
 (specifically, population sizes, gene flow, and split times) from
 sequence data. It is an implementation of the *Generalised
@@ -33,13 +35,10 @@
 
 Documentation is hosted on ReadTheDocs: https://dismal.readthedocs.io/en/latest/
 
 
 Installation
 ------------
 
-DISMaL is currently only available as a pre-release from this GitHub
-repo. Install using:
+Install latest full release with Pip: `pip install dismal`
 
-::
-
-   pip install git+https://github.com/simonharnqvist/DISMaL.git#egg=dismal
+Or the development version from GitHub: `pip install git+https://github.com/simonharnqvist/DISMaL.git#egg=dismal`
```

### Comparing `dismal-0.1.16b0/dismal.egg-info/SOURCES.txt` & `dismal-0.1.18b0/dismal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/tests/test_callset.py` & `dismal-0.1.18b0/tests/test_callset.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/tests/test_demography.py` & `dismal-0.1.18b0/tests/test_demography.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/tests/test_markov_matrices.py` & `dismal-0.1.18b0/tests/test_markov_matrices.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/tests/test_model_instance.py` & `dismal-0.1.18b0/tests/test_model_instance.py`

 * *Files identical despite different names*

### Comparing `dismal-0.1.16b0/tests/test_simulate.py` & `dismal-0.1.18b0/tests/test_simulate.py`

 * *Files identical despite different names*

