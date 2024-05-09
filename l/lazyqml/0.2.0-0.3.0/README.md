# Comparing `tmp/lazyqml-0.2.0.tar.gz` & `tmp/lazyqml-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyqml-0.2.0.tar", last modified: Tue May  7 10:19:04 2024, max compression
+gzip compressed data, was "lazyqml-0.3.0.tar", last modified: Thu May  9 11:46:40 2024, max compression
```

## Comparing `lazyqml-0.2.0.tar` & `lazyqml-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:19:04.915532 lazyqml-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-07 10:18:54.000000 lazyqml-0.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:19:04.907532 lazyqml-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:19:04.907532 lazyqml-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-07 10:18:54.000000 lazyqml-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 10:18:54.000000 lazyqml-0.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-07 10:18:54.000000 lazyqml-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:19:04.911532 lazyqml-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-07 10:18:54.000000 lazyqml-0.2.0/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-07 10:18:54.000000 lazyqml-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 10:18:54.000000 lazyqml-0.2.0/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-07 10:18:54.000000 lazyqml-0.2.0/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-07 10:18:54.000000 lazyqml-0.2.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-07 10:18:54.000000 lazyqml-0.2.0/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-07 10:18:54.000000 lazyqml-0.2.0/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-07 10:18:54.000000 lazyqml-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 10:18:54.000000 lazyqml-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-07 10:18:54.000000 lazyqml-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 10:18:54.000000 lazyqml-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-07 10:19:04.915532 lazyqml-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 10:18:54.000000 lazyqml-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:19:04.911532 lazyqml-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 10:18:54.000000 lazyqml-0.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 10:18:54.000000 lazyqml-0.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 10:18:54.000000 lazyqml-0.2.0/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-07 10:18:54.000000 lazyqml-0.2.0/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:19:04.911532 lazyqml-0.2.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   827658 2024-05-07 10:18:54.000000 lazyqml-0.2.0/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 10:18:54.000000 lazyqml-0.2.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 10:18:54.000000 lazyqml-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-07 10:18:54.000000 lazyqml-0.2.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 10:18:54.000000 lazyqml-0.2.0/docs/lazyqml.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:19:04.911532 lazyqml-0.2.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 10:18:54.000000 lazyqml-0.2.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-07 10:18:54.000000 lazyqml-0.2.0/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:19:04.915532 lazyqml-0.2.0/lazyqml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-07 10:18:54.000000 lazyqml-0.2.0/lazyqml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-05-07 10:18:54.000000 lazyqml-0.2.0/lazyqml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    32174 2024-05-07 10:18:54.000000 lazyqml-0.2.0/lazyqml/supervised.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:19:04.915532 lazyqml-0.2.0/lazyqml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-07 10:19:04.000000 lazyqml-0.2.0/lazyqml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-07 10:19:04.000000 lazyqml-0.2.0/lazyqml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 10:19:04.000000 lazyqml-0.2.0/lazyqml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-07 10:19:04.000000 lazyqml-0.2.0/lazyqml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-07 10:19:04.000000 lazyqml-0.2.0/lazyqml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 10:19:04.000000 lazyqml-0.2.0/lazyqml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-07 10:18:54.000000 lazyqml-0.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-07 10:18:54.000000 lazyqml-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-07 10:18:54.000000 lazyqml-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-07 10:18:54.000000 lazyqml-0.2.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 10:19:04.915532 lazyqml-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:19:04.915532 lazyqml-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 10:18:54.000000 lazyqml-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-07 10:18:54.000000 lazyqml-0.2.0/tests/test_lazyqml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.513798 lazyqml-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.501797 lazyqml-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.505797 lazyqml-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.505797 lazyqml-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-09 11:46:25.000000 lazyqml-0.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 11:46:25.000000 lazyqml-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 11:46:25.000000 lazyqml-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-09 11:46:40.513798 lazyqml-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 11:46:25.000000 lazyqml-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.509797 lazyqml-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.509797 lazyqml-0.3.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   827658 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/lazyqml.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.509797 lazyqml-0.3.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.509797 lazyqml-0.3.0/lazyqml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-09 11:46:25.000000 lazyqml-0.3.0/lazyqml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31458 2024-05-09 11:46:25.000000 lazyqml-0.3.0/lazyqml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41988 2024-05-09 11:46:25.000000 lazyqml-0.3.0/lazyqml/supervised.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.513798 lazyqml-0.3.0/lazyqml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-09 11:46:40.000000 lazyqml-0.3.0/lazyqml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-09 11:46:40.000000 lazyqml-0.3.0/lazyqml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:46:40.000000 lazyqml-0.3.0/lazyqml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 11:46:40.000000 lazyqml-0.3.0/lazyqml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-09 11:46:40.000000 lazyqml-0.3.0/lazyqml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 11:46:40.000000 lazyqml-0.3.0/lazyqml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-09 11:46:25.000000 lazyqml-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-09 11:46:25.000000 lazyqml-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-09 11:46:25.000000 lazyqml-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-09 11:46:25.000000 lazyqml-0.3.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:46:40.513798 lazyqml-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.509797 lazyqml-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 11:46:25.000000 lazyqml-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-09 11:46:25.000000 lazyqml-0.3.0/tests/test_lazyqml.py
```

### Comparing `lazyqml-0.2.0/.github/workflows/docs-build.yml` & `lazyqml-0.3.0/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/.github/workflows/docs.yml` & `lazyqml-0.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/.github/workflows/installation.yml` & `lazyqml-0.3.0/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/.github/workflows/macos.yml` & `lazyqml-0.3.0/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/.github/workflows/pypi.yml` & `lazyqml-0.3.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/.github/workflows/ubuntu.yml` & `lazyqml-0.3.0/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/.github/workflows/windows.yml` & `lazyqml-0.3.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/.gitignore` & `lazyqml-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/LICENSE` & `lazyqml-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/PKG-INFO` & `lazyqml-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.2.0
+Version: 0.3.0
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -31,14 +31,15 @@
 Requires-Dist: rustworkx==0.12.1
 Requires-Dist: scikit-learn==1.2.0
 Requires-Dist: scipy==1.8.1
 Requires-Dist: threadpoolctl==3.1.0
 Requires-Dist: toolz==0.12.0
 Requires-Dist: wheel
 Requires-Dist: tabulate
+Requires-Dist: logging
 Provides-Extra: all
 Requires-Dist: lazyqml[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # lazyqml
```

### Comparing `lazyqml-0.2.0/docs/contributing.md` & `lazyqml-0.3.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/docs/examples/intro.ipynb` & `lazyqml-0.3.0/docs/examples/intro.ipynb`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/docs/installation.md` & `lazyqml-0.3.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/docs/usage.md` & `lazyqml-0.3.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/lazyqml/common.py` & `lazyqml-0.3.0/lazyqml/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #======================================================================================
 # The common module contains common functions and classes used by the other modules.
 #======================================================================================
 
 """
  Import Packages
 """
-
+import math
+import logging
 import pennylane as qml
 import jax.numpy as jnp
 import optax
 from itertools import combinations
 import pennylane as qml
 import jax
 import numpy as np
@@ -25,22 +26,24 @@
 from sklearn.pipeline import Pipeline
 from sklearn.impute import SimpleImputer, MissingIndicator
 from sklearn.preprocessing import StandardScaler, OneHotEncoder, OrdinalEncoder
 from sklearn.compose import ColumnTransformer
 from sklearn.utils import all_estimators
 from sklearn.base import RegressorMixin
 from sklearn.base import ClassifierMixin
-
+from itertools import product
 from sklearn.metrics import (
     accuracy_score,
     balanced_accuracy_score,
     roc_auc_score,
     f1_score,
 )
 
+
+#jax.config.update("jax_disable_jit",True)
 """
  Embeddings / Feature Maps
 """
 
 def rx_embedding(x, wires):
     """Embeds a quantum state into the quantum device using rotation around the X-axis.
 
@@ -86,26 +89,28 @@
         x (array[float]): array of rotation angles for each qubit
         wires (Sequence[int]): wires that the operation acts on
 
     Returns:
         None
     """    
     nload=min(len(x), len(wires))
+    #nload=len(wires)
+        
     
     for i in range(nload):
         qml.Hadamard(i)
         qml.RZ(2.0*x[i],wires=i)
         
+
     for pair in list(combinations (range(nload), 2)):
         q0=pair[0]
         q1=pair[1]
         
         qml.CZ(wires=[q0,q1])
-        qml.RZ((2.0*(jnp.pi-x[q0])*
-               jnp.pi-x[q1]),wires=q1)
+        qml.RZ(2.0*(jnp.pi-x[q0])*(jnp.pi-x[q1]),wires=q1)
         qml.CZ(wires=[q0,q1])
 
 def amp_embedding (x , wires):
     """Embeds a quantum state into the quantum device using Amplitude Encoding.
 
     Args:
         x (array[float]): array of complex amplitudes
@@ -147,23 +152,23 @@
         embedding (str): embedding type ('rx_embedding', 'ry_embedding', 'rz_embedding', 'ZZ_embedding', or 'amplitude_embedding')
         n_qubits (int): number of qubits
 
     Returns:
         function: quantum kernel function
     """
     jax.config.update("jax_enable_x64", True)
-    embedding_circ = get_embedding(embedding)
+    # embedding_circ = get_embedding(embedding)
 
     device = qml.device("default.qubit.jax", wires = n_qubits)
     
     @jax.jit
     @qml.qnode(device, interface='jax')
     def kernel_circ(a , b):
-        embedding_circ(a , wires=range(n_qubits))
-        qml.adjoint(embedding_circ)(b , wires=range(n_qubits))
+        get_embedding(embedding)(a , wires=range(n_qubits))
+        qml.adjoint(get_embedding(embedding))(b , wires=range(n_qubits))
         return qml.probs(wires = range(n_qubits))
 
     def kernel(A, B):
         return np.array([[kernel_circ(a , b)[0] for b in B]for a in A])
     
     return kernel
 
@@ -185,27 +190,30 @@
     assert len(theta) == 3 * N
     
     for i in range(N):
         qml.RX(theta[3 * i], wires=wires[i])
     
     for i in range(N-1):
         qml.CNOT(wires=[wires[i], wires[i + 1]])
+    qml.CNOT(wires=[wires[N-1],wires[0]])
     
     for i in range(N):
         qml.RZ(theta[3 * i + 1], wires=wires[i])
     
     for i in range(N-1):
         qml.CNOT(wires=[wires[i], wires[i + 1]])
-    
+    qml.CNOT(wires=[wires[N-1],wires[0]])
+
     for i in range(N):
         qml.RX(theta[3 * i + 2], wires=wires[i])
     
     for i in range(N-1):
         qml.CNOT(wires=[wires[i], wires[i + 1]])
-        
+    qml.CNOT(wires=[wires[N-1],wires[0]])
+
 def tree_tensor_ansatz(theta , wires):
     """Implements a tree tensor network ansatz circuit.
 
     Args:
         theta (array[float]): array of parameters for the ansatz circuit
         wires (Sequence[int]): wires that the ansatz circuit acts on
 
@@ -253,14 +261,15 @@
     N=len(wires)
 
     for i in range(N):
         qml.Hadamard(wires = wires[i])
     
     for i in range(N-1):
         qml.CZ(wires=[wires[i], wires[i+1]])
+    qml.CZ(wires=[wires[N-1],wires[0]])
     
     for i in range(N):
         qml.RX(theta[i], wires=wires[i])
 
 def TwoLocal(theta, wires):
     """Implements a two-local ansatz circuit.
 
@@ -286,24 +295,24 @@
 
     Returns:
         tuple: ansatz function and the number of parameters
     """
     if ansatz == 'hardware_efficient':
         return hardware_efficient_ansatz, 3 * n_qubits
     if ansatz == 'tree_tensor':
-        return tree_tensor_ansatz , int(n_param_tree_tensor(n_qubits))
+        return tree_tensor_ansatz , 2**(n_qubits+1)-1
     if ansatz == 'HPzRx':
         return HPzRx , n_qubits
     if ansatz == 'two_local':
         return TwoLocal, n_qubits
 """
  Auxiliary Functions
 """    
 
-def create_circuit(n_qubits,layers,ansatz, n_class, backend='jax'):
+def create_circuit(n_qubits,layers,embedding,ansatz,n_class, backend='jax'):
     """Creates a quantum circuit for classification tasks.
 
     Args:
         n_qubits (int): number of qubits
         layers (int): number of layers in the circuit
         ansatz (str): ansatz type ('hardware_efficient', 'tree_tensor', 'HPzRx', or 'two_local')
         n_class (int): number of classes
@@ -319,27 +328,27 @@
         device = qml.device("default.qubit.jax", wires=n_qubits)
     else:
         raise ValueError(f"Backend {backend} is unknown")
     ansatz, params_per_layer = get_ansatz(ansatz,n_qubits)
     
     @qml.qnode(device, interface = 'jax')
     def circuit(x, theta):
-        get_embedding('amplitude_embedding')(x , wires=range(n_qubits))
+        get_embedding(embedding)(x , wires=range(n_qubits))
 
         for i in range(layers):
             ansatz(theta[i * params_per_layer: (i + 1) * params_per_layer], wires=range(n_qubits))
         observable=[]
         for n in range(n_class):
             observable.append(qml.expval(qml.PauliZ(wires=n)))
         #verboseprint(observable)
         return observable
 
     return jax.jit(circuit)
 
-def create_circuit_binary(n_qubits,layers,ansatz,backend="jax"):
+def create_circuit_binary(n_qubits,layers,embedding,ansatz,backend="jax"):
     """Creates a quantum circuit for binary classification tasks.
 
     Args:
         n_qubits (int): number of qubits
         layers (int): number of layers in the circuit
         ansatz (str): ansatz type ('hardware_efficient', 'tree_tensor', 'HPzRx', or 'two_local')
         backend (str, optional): quantum backend to use ('jax'). Defaults to 'jax'.
@@ -357,15 +366,15 @@
     ansatz, params_per_layer = get_ansatz(ansatz,n_qubits)
 
     state_0=[[1],[0]]
     M=state_0*np.conj(state_0).T
     @qml.qnode(device, interface = 'jax')
     def circuit(x, theta):
         #embedding(x, wires=range(n_qubits))
-        get_embedding('amplitude_embedding')(x , wires=range(n_qubits))
+        get_embedding(embedding)(x , wires=range(n_qubits))
         for i in range(layers):
             #ry_embedding(x, wires=range(n_qubits))
             ansatz(theta[i * params_per_layer: (i + 1) * params_per_layer], wires=range(n_qubits))
         return qml.expval(qml.Hermitian(M, wires=0))
 
     return jax.jit(circuit)#
 
@@ -418,15 +427,14 @@
 
     Returns:
         tuple: predictions, accuracy score, balanced accuracy score, weighted F1 score, ROC AUC score
     """
 
     @jax.jit
     def cross_entropy_loss(y_true, y_pred):
-        
         return -jnp.mean(jnp.sum(jnp.log(y_pred) * y_true, axis=1))
     
     @jax.jit
     def calculate_ce_cost(X, y, theta):
         yp = qnn(X, theta)
         
         yp = jax.nn.softmax(yp)
@@ -437,15 +445,15 @@
     @jax.jit
     def optimizer_update(opt_state, params, x, y):
         loss, grads = jax.value_and_grad(lambda theta: calculate_ce_cost(x, y, theta))(params)
         updates, opt_state = optimizer.update(grads, opt_state)
         params = optax.apply_updates(params, updates)
         return params, opt_state, loss
     
-    y_test_ohe = y_test.copy() 
+    y_test_ohe = y_test.copy()
     y_test = jnp.argmax(y_test, axis=1)
     
     verboseprint(f"QNN_BAG\t{ansatz}")
     verboseprint('='*50)
     for i in range(runs):
         
         # array to gather estimators' predictions
@@ -497,15 +505,15 @@
             verboseprint(f'Error of bagging estimator {j} on test set: {cross_entropy_loss(y_test_ohe,y_predict)}')
             
             y_predict = jnp.argmax(y_predict, axis=1)
             y_predict_train = jnp.argmax(y_predict_train, axis=1)
             y_train_aux = jnp.argmax(y_train_est, axis=1)
             
             
-            verboseprint(f'Accuracy of bagging estimator {j} on test set: {accuracy_score(y_test,y_predict)}\n')
+            verboseprint(f'Accuracy of bagging estimator {j} on test set: {accuracy_score(y_test,y_predict)}')
             
             predictions.append(y_predict)
             predictions_train.append(y_predict_train)
             predictions_softmax.append(y_predict_softmax)
             predictions_softmax_train.append(y_predict_softmax_train)
             
         
@@ -531,16 +539,16 @@
             verboseprint(f'Accuracy of bagging on test set: {accuracy_score(y_test,y_predict)}\n')
         
         else:
             # compute average of estimators' predictions
             y_predict = jnp.mean(predictions_softmax,axis=0).reshape(-1,3)
             y_predict_train = jnp.mean(predictions_softmax_train,axis=0).reshape(-1,3)
             verboseprint(f'Error of bagging on test set: {cross_entropy_loss(y_test_ohe,y_predict)}\n')
-    
             y_predict = jnp.argmax(y_predict, axis=1)
+            
             y_predict_train = jnp.argmax(y_predict_train, axis=1)
             end_time_ts = time.time()-start_time_ts
             verboseprint(f'Accuracy of bagging on test set: {accuracy_score(y_test,y_predict)}\n')
         try:
             roc_auc = roc_auc_score(y_test, y_predict)
         except Exception as exception:
             roc_auc = None
@@ -638,39 +646,39 @@
             end_time_tr = time.time()-start_time_tr
             
             ##### predict #####
             start_time_ts = time.time() 
             y_predict = qnn(X_test[:,random_estimator_features], params)
             y_predict_train = qnn(X_train_est, params)
             
-            verboseprint(f'Error of bagging estimator {j} on test set: {cross_entropy_loss(y_test_ohe,y_predict)}\n')
+            verboseprint(f'Error of bagging estimator {j} on test set: {cross_entropy_loss(y_test_ohe,y_predict)}')
             
             
             end_time_ts = time.time()-start_time_ts
             
 
-            verboseprint(f'Accuracy of bagging estimator {j} on test set: {accuracy_score(y_test,y_predict>=0.5)}\n')
-            verboseprint(f'Accuracy of bagging estimator {j} on train set: {accuracy_score(y_train_est,y_predict_train>=0.5)}\n')
+            verboseprint(f'Accuracy of bagging estimator {j} on test set: {accuracy_score(y_test,y_predict>=0.5)}')
+            verboseprint(f'Accuracy of bagging estimator {j} on train set: {accuracy_score(y_train_est,y_predict_train>=0.5)}')
             predictions.append(y_predict)
             predictions_train.append(y_predict_train)
         
         
         # transform list of predictions into an array
         predictions = np.array(predictions)
         predictions_train = np.array(predictions_train)
 
         ##### predict #####
         
         # compute average of estimators' predictions
         
         y_predict = jnp.mean(predictions, axis=0)
         y_predict_train = jnp.mean(predictions_train, axis=0)
-        verboseprint(f'Error of bagging on test set: {cross_entropy_loss(y_test_ohe,y_predict)}\n')
+        verboseprint(f'Error of bagging on test set: {cross_entropy_loss(y_test_ohe,y_predict)}')
         
-        verboseprint(f'Accuracy of bagging on test set: {accuracy_score(y_test,y_predict>=0.5)}\n')        
+        verboseprint(f'Accuracy of bagging on test set: {accuracy_score(y_test,y_predict>=0.5)}')        
 
         y_predict = y_predict>=0.5
 
         try:
             roc_auc = roc_auc_score(y_test, y_predict)
         except Exception as exception:
             roc_auc = None
@@ -724,15 +732,14 @@
         loss, grads = jax.value_and_grad(lambda theta: calculate_ce_cost(x, y, theta))(params)
         updates, opt_state = optimizer.update(grads, opt_state)
         params = optax.apply_updates(params, updates)
         return params, opt_state, loss
     
     y_test_ohe = y_test.copy() 
     y_test = jnp.argmax(y_test, axis=1)
-
     for i in range(runs):
         # seed
         key = jax.random.PRNGKey(seed)
         
         # get number of circuit params
         _, params_per_layer = get_ansatz(ansatz, n_qubits)
         
@@ -753,14 +760,15 @@
         
         ##### predict #####
         start_time_ts = time.time() 
         y_predict = qnn(X_test, params)
         y_predict = jax.nn.softmax(y_predict)
         verboseprint(f'cross entropy loss: {cross_entropy_loss(y_test_ohe,y_predict)}')
         y_predict = jnp.argmax(y_predict, axis=1)
+        
         end_time_ts = time.time()-start_time_ts
         verboseprint(f'Accuracy of fullmodel on test set: {accuracy_score(y_test,y_predict)}')
 
         try:
             roc_auc = roc_auc_score(y_test, y_predict)
         except Exception as exception:
             roc_auc = None
```

### Comparing `lazyqml-0.2.0/lazyqml.egg-info/PKG-INFO` & `lazyqml-0.3.0/lazyqml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.2.0
+Version: 0.3.0
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -31,14 +31,15 @@
 Requires-Dist: rustworkx==0.12.1
 Requires-Dist: scikit-learn==1.2.0
 Requires-Dist: scipy==1.8.1
 Requires-Dist: threadpoolctl==3.1.0
 Requires-Dist: toolz==0.12.0
 Requires-Dist: wheel
 Requires-Dist: tabulate
+Requires-Dist: logging
 Provides-Extra: all
 Requires-Dist: lazyqml[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # lazyqml
```

### Comparing `lazyqml-0.2.0/lazyqml.egg-info/SOURCES.txt` & `lazyqml-0.3.0/lazyqml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/mkdocs.yml` & `lazyqml-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.2.0/pyproject.toml` & `lazyqml-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lazyqml"
-version = "0.2.0"
+version = "0.3.0"
 dynamic = [
     "dependencies",
 ]
 description = "LazyQML benchmarking utility to test quantum machine learning models."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -46,15 +46,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.2.0"
+current_version = "0.3.0"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `lazyqml-0.2.0/requirements.txt` & `lazyqml-0.3.0/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,11 @@
 threadpoolctl==3.1.0
 #toml==0.10.2
 toolz==0.12.0
 #typing_extensions==4.4.0
 #urllib3==1.26.13
 wheel
 tabulate
+logging
 #xlrd==2.0.1
 #zipp==3.18.1
```

### Comparing `lazyqml-0.2.0/requirements_dev.txt` & `lazyqml-0.3.0/requirements_dev.txt`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 toml==0.10.2
 toolz==0.12.0
 typing_extensions==4.4.0
 urllib3==1.26.13
 wheel==0.41.2
 xlrd==2.0.1
 zipp==3.18.1
+logging
+tabulate
 codespell
 mkdocs
 mkdocs-material
 mkdocstrings
 mkdocs-git-revision-date-localized-plugin
 mkdocs-git-revision-date-plugin
 mkdocs-jupyter
```

### Comparing `lazyqml-0.2.0/tests/test_lazyqml.py` & `lazyqml-0.3.0/tests/test_lazyqml.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,27 +16,27 @@
         from sklearn.model_selection import train_test_split
         data = load_iris()
         X = data.data
         y = data.target
         
         X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.3,random_state =123)  
 
-        q = QuantumClassifier(nqubits=4,classifiers=["qnn_bag"],verbose=0)
+        q = QuantumClassifier(nqubits=4,classifiers=["all"])
 
         scores = q.fit(X_train, X_test, y_train, y_test)
 
         print(scores)
 
     def test_binary(self):
         from sklearn.datasets import load_breast_cancer, load_iris
         from sklearn.model_selection import train_test_split
         data = load_breast_cancer()
         X = data.data
         y = data.target
 
         X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.3,random_state =123)  
 
-        q = QuantumClassifier(nqubits=4,classifiers=["qnn_bag"],verbose=0)
+        q = QuantumClassifier(nqubits=2,classifiers=["all"])
 
         scores = q.fit(X_train, X_test, y_train, y_test)
 
         print(scores)
```

