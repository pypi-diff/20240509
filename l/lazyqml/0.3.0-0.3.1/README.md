# Comparing `tmp/lazyqml-0.3.0.tar.gz` & `tmp/lazyqml-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyqml-0.3.0.tar", last modified: Thu May  9 11:46:40 2024, max compression
+gzip compressed data, was "lazyqml-0.3.1.tar", last modified: Thu May  9 11:50:13 2024, max compression
```

## Comparing `lazyqml-0.3.0.tar` & `lazyqml-0.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.513798 lazyqml-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.501797 lazyqml-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.505797 lazyqml-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.505797 lazyqml-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 11:46:25.000000 lazyqml-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-09 11:46:25.000000 lazyqml-0.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 11:46:25.000000 lazyqml-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 11:46:25.000000 lazyqml-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-09 11:46:40.513798 lazyqml-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 11:46:25.000000 lazyqml-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.509797 lazyqml-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.509797 lazyqml-0.3.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   827658 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/lazyqml.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.509797 lazyqml-0.3.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 11:46:25.000000 lazyqml-0.3.0/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.509797 lazyqml-0.3.0/lazyqml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-09 11:46:25.000000 lazyqml-0.3.0/lazyqml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31458 2024-05-09 11:46:25.000000 lazyqml-0.3.0/lazyqml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    41988 2024-05-09 11:46:25.000000 lazyqml-0.3.0/lazyqml/supervised.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.513798 lazyqml-0.3.0/lazyqml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-09 11:46:40.000000 lazyqml-0.3.0/lazyqml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-09 11:46:40.000000 lazyqml-0.3.0/lazyqml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:46:40.000000 lazyqml-0.3.0/lazyqml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 11:46:40.000000 lazyqml-0.3.0/lazyqml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-09 11:46:40.000000 lazyqml-0.3.0/lazyqml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 11:46:40.000000 lazyqml-0.3.0/lazyqml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-09 11:46:25.000000 lazyqml-0.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-09 11:46:25.000000 lazyqml-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-09 11:46:25.000000 lazyqml-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-09 11:46:25.000000 lazyqml-0.3.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:46:40.513798 lazyqml-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:40.509797 lazyqml-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 11:46:25.000000 lazyqml-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-09 11:46:25.000000 lazyqml-0.3.0/tests/test_lazyqml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:50:13.389841 lazyqml-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 11:50:02.000000 lazyqml-0.3.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:50:13.381841 lazyqml-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:50:13.385841 lazyqml-0.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-09 11:50:02.000000 lazyqml-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 11:50:02.000000 lazyqml-0.3.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-09 11:50:02.000000 lazyqml-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:50:13.385841 lazyqml-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-09 11:50:02.000000 lazyqml-0.3.1/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-09 11:50:02.000000 lazyqml-0.3.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-09 11:50:02.000000 lazyqml-0.3.1/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-09 11:50:02.000000 lazyqml-0.3.1/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 11:50:02.000000 lazyqml-0.3.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-09 11:50:02.000000 lazyqml-0.3.1/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-09 11:50:02.000000 lazyqml-0.3.1/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 11:50:02.000000 lazyqml-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-09 11:50:02.000000 lazyqml-0.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 11:50:02.000000 lazyqml-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 11:50:02.000000 lazyqml-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-09 11:50:13.389841 lazyqml-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 11:50:02.000000 lazyqml-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:50:13.385841 lazyqml-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 11:50:02.000000 lazyqml-0.3.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 11:50:02.000000 lazyqml-0.3.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 11:50:02.000000 lazyqml-0.3.1/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-09 11:50:02.000000 lazyqml-0.3.1/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:50:13.385841 lazyqml-0.3.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   827658 2024-05-09 11:50:02.000000 lazyqml-0.3.1/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 11:50:02.000000 lazyqml-0.3.1/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 11:50:02.000000 lazyqml-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-09 11:50:02.000000 lazyqml-0.3.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 11:50:02.000000 lazyqml-0.3.1/docs/lazyqml.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:50:13.389841 lazyqml-0.3.1/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-09 11:50:02.000000 lazyqml-0.3.1/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 11:50:02.000000 lazyqml-0.3.1/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:50:13.389841 lazyqml-0.3.1/lazyqml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-09 11:50:02.000000 lazyqml-0.3.1/lazyqml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31458 2024-05-09 11:50:02.000000 lazyqml-0.3.1/lazyqml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41989 2024-05-09 11:50:02.000000 lazyqml-0.3.1/lazyqml/supervised.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:50:13.389841 lazyqml-0.3.1/lazyqml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-09 11:50:13.000000 lazyqml-0.3.1/lazyqml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-09 11:50:13.000000 lazyqml-0.3.1/lazyqml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:50:13.000000 lazyqml-0.3.1/lazyqml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 11:50:13.000000 lazyqml-0.3.1/lazyqml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-09 11:50:13.000000 lazyqml-0.3.1/lazyqml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 11:50:13.000000 lazyqml-0.3.1/lazyqml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-09 11:50:02.000000 lazyqml-0.3.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-09 11:50:02.000000 lazyqml-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-09 11:50:02.000000 lazyqml-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-09 11:50:02.000000 lazyqml-0.3.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:50:13.389841 lazyqml-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:50:13.389841 lazyqml-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 11:50:02.000000 lazyqml-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-09 11:50:02.000000 lazyqml-0.3.1/tests/test_lazyqml.py
```

### Comparing `lazyqml-0.3.0/.github/workflows/docs-build.yml` & `lazyqml-0.3.1/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/.github/workflows/docs.yml` & `lazyqml-0.3.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/.github/workflows/installation.yml` & `lazyqml-0.3.1/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/.github/workflows/macos.yml` & `lazyqml-0.3.1/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/.github/workflows/pypi.yml` & `lazyqml-0.3.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/.github/workflows/ubuntu.yml` & `lazyqml-0.3.1/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/.github/workflows/windows.yml` & `lazyqml-0.3.1/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/.gitignore` & `lazyqml-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/LICENSE` & `lazyqml-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/PKG-INFO` & `lazyqml-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.3.0
+Version: 0.3.1
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyqml-0.3.0/docs/contributing.md` & `lazyqml-0.3.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/docs/examples/intro.ipynb` & `lazyqml-0.3.1/docs/examples/intro.ipynb`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/docs/installation.md` & `lazyqml-0.3.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/docs/usage.md` & `lazyqml-0.3.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/lazyqml/common.py` & `lazyqml-0.3.1/lazyqml/common.py`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/lazyqml/supervised.py` & `lazyqml-0.3.1/lazyqml/supervised.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Main Module
 #======================================================================================
 
 """
  Import modules
 """
 
-from common import *
+from .common import *
 import warnings
 warnings.filterwarnings("ignore")
 
 """
  Classifiers
 """
 
@@ -107,101 +107,101 @@
     >>> X = data.data
     >>> y= data.target
     >>> X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.5,random_state =123)
     >>> clf = QuantumClassifier(verbose=0,ignore_warnings=True, customMetric=None)
     >>> models,predictions = clf.fit(X_train, X_test, y_train, y_test)
     >>> model_dictionary = clf.provide_models(X_train,X_test,y_train,y_test)
     >>> models
-    | Model       | Embedding           | Ansatz             |   Accuracy |   Balanced Accuracy | ROC AUC   |   F1 Score |   Time taken |
-    |:------------|:--------------------|:-------------------|-----------:|--------------------:|:----------|-----------:|-------------:|
-    | qsvm        | rx_embedding        |                    |   0.955556 |            0.960784 |           |  0.956187  |      3.00024 |
-    | qsvm        | rz_embedding        |                    |   0.955556 |            0.960784 |           |  0.956187  |      2.93275 |
-    | qsvm        | ry_embedding        |                    |   0.955556 |            0.960784 |           |  0.956187  |      2.98143 |
-    | qnn         | amplitude_embedding | hardware_efficient |   0.733333 |            0.754248 |           |  0.723993  |     11.207   |
-    | qnn         | ZZ_embedding        | two_local          |   0.733333 |            0.754248 |           |  0.723993  |      2.9692  |
-    | qnn         | rz_embedding        | two_local          |   0.733333 |            0.754248 |           |  0.723993  |      2.94752 |
-    | qnn         | rx_embedding        | two_local          |   0.733333 |            0.754248 |           |  0.723993  |      3.07974 |
-    | qnn         | ry_embedding        | two_local          |   0.733333 |            0.754248 |           |  0.723993  |      2.94321 |
-    | qnn         | amplitude_embedding | HPzRx              |   0.733333 |            0.753159 |           |  0.717882  |      2.32015 |
-    | qsvm        | amplitude_embedding |                    |   0.711111 |            0.734641 |           |  0.697691  |      3.99333 |
-    | qnn         | rx_embedding        | HPzRx              |   0.666667 |            0.681699 |           |  0.650911  |      2.2885  |
-    | qnn         | ZZ_embedding        | HPzRx              |   0.666667 |            0.681699 |           |  0.650911  |      2.09387 |
-    | qnn         | rz_embedding        | HPzRx              |   0.666667 |            0.681699 |           |  0.650911  |      2.31533 |
-    | qnn         | ry_embedding        | HPzRx              |   0.666667 |            0.681699 |           |  0.650911  |      2.29481 |
-    | qnn_bag_0.8 | amplitude_embedding | tree_tensor        |   0.622222 |            0.676471 |           |  0.609367  |      5.76442 |
-    | qnn         | amplitude_embedding | two_local          |   0.622222 |            0.663834 |           |  0.610864  |      2.72723 |
-    | qnn_bag_0.8 | amplitude_embedding | HPzRx              |   0.6      |            0.657952 |           |  0.586446  |      3.39962 |
-    | qnn         | rz_embedding        | hardware_efficient |   0.622222 |            0.656209 |           |  0.580471  |     11.0559  |
-    | qnn         | ZZ_embedding        | hardware_efficient |   0.622222 |            0.656209 |           |  0.580471  |     11.0533  |
-    | qnn         | rx_embedding        | hardware_efficient |   0.622222 |            0.656209 |           |  0.580471  |     11.5151  |
-    | qnn         | ry_embedding        | hardware_efficient |   0.622222 |            0.656209 |           |  0.580471  |     11.1438  |
-    | qnn_bag_0.8 | amplitude_embedding | two_local          |   0.6      |            0.644227 |           |  0.589402  |      3.95424 |
-    | qnn_bag_0.8 | amplitude_embedding | hardware_efficient |   0.6      |            0.643137 |           |  0.591346  |     13.716   |
-    | qnn         | ZZ_embedding        | tree_tensor        |   0.6      |            0.636601 |           |  0.547036  |      4.11366 |
-    | qnn         | rz_embedding        | tree_tensor        |   0.6      |            0.636601 |           |  0.547036  |      4.28233 |
-    | qnn         | ry_embedding        | tree_tensor        |   0.6      |            0.636601 |           |  0.547036  |      4.25941 |
-    | qnn         | rx_embedding        | tree_tensor        |   0.6      |            0.636601 |           |  0.547036  |      4.38062 |
-    | qsvm        | ZZ_embedding        |                    |   0.622222 |            0.636383 |           |  0.641239  |      3.32188 |
-    | qnn         | amplitude_embedding | tree_tensor        |   0.577778 |            0.616993 |           |  0.511375  |      4.40494 |
-    | qnn_bag_0.5 | amplitude_embedding | HPzRx              |   0.488889 |            0.508279 |           |  0.48642   |      3.33889 |
-    | qnn_bag_0.5 | amplitude_embedding | tree_tensor        |   0.444444 |            0.471242 |           |  0.410935  |      6.13786 |
-    | qnn_bag_0.5 | amplitude_embedding | hardware_efficient |   0.444444 |            0.471242 |           |  0.410935  |     13.5337  |
-    | qnn_bag_0.5 | amplitude_embedding | two_local          |   0.422222 |            0.452723 |           |  0.372047  |      3.86997 |
-    | qnn_bag_0.8 | rz_embedding        | HPzRx              |   0.4      |            0.399129 |           |  0.423165  |      3.32705 |
-    | qnn_bag_0.8 | ZZ_embedding        | HPzRx              |   0.4      |            0.399129 |           |  0.423165  |      3.50388 |
-    | qnn_bag_0.8 | rx_embedding        | hardware_efficient |   0.4      |            0.399129 |           |  0.423165  |     14.2781  |
-    | qnn_bag_0.8 | ry_embedding        | HPzRx              |   0.4      |            0.399129 |           |  0.423165  |      4.21789 |
-    | qnn_bag_0.8 | ry_embedding        | hardware_efficient |   0.4      |            0.399129 |           |  0.423165  |     13.5693  |
-    | qnn_bag_0.8 | rx_embedding        | HPzRx              |   0.4      |            0.399129 |           |  0.423165  |      3.30752 |
-    | qnn_bag_0.8 | ZZ_embedding        | hardware_efficient |   0.4      |            0.399129 |           |  0.423165  |     13.6998  |
-    | qnn_bag_0.8 | rz_embedding        | hardware_efficient |   0.4      |            0.399129 |           |  0.423165  |     13.7134  |
-    | qnn_bag_0.5 | rz_embedding        | hardware_efficient |   0.333333 |            0.390196 |           |  0.275556  |     13.5766  |
-    | qnn_bag_0.5 | ZZ_embedding        | HPzRx              |   0.333333 |            0.390196 |           |  0.275556  |      3.42679 |
-    | qnn_bag_0.5 | ry_embedding        | two_local          |   0.333333 |            0.390196 |           |  0.275556  |      4.44122 |
-    | qnn_bag_0.5 | rx_embedding        | tree_tensor        |   0.333333 |            0.390196 |           |  0.275556  |      5.3968  |
-    | qnn_bag_0.5 | rx_embedding        | hardware_efficient |   0.333333 |            0.390196 |           |  0.275556  |     13.53    |
-    | qnn_bag_0.5 | ZZ_embedding        | two_local          |   0.333333 |            0.390196 |           |  0.275556  |      4.51936 |
-    | qnn_bag_0.5 | ZZ_embedding        | tree_tensor        |   0.333333 |            0.390196 |           |  0.275556  |      5.96975 |
-    | qnn_bag_0.5 | rz_embedding        | HPzRx              |   0.333333 |            0.390196 |           |  0.275556  |      3.95576 |
-    | qnn_bag_0.5 | ry_embedding        | HPzRx              |   0.333333 |            0.390196 |           |  0.275556  |      3.33663 |
-    | qnn_bag_0.5 | rz_embedding        | tree_tensor        |   0.333333 |            0.390196 |           |  0.275556  |      5.62083 |
-    | qnn_bag_0.5 | rz_embedding        | two_local          |   0.333333 |            0.390196 |           |  0.275556  |      4.47015 |
-    | qnn_bag_0.5 | ZZ_embedding        | hardware_efficient |   0.333333 |            0.390196 |           |  0.275556  |     13.4961  |
-    | qnn_bag_0.5 | ry_embedding        | tree_tensor        |   0.333333 |            0.390196 |           |  0.275556  |      5.50221 |
-    | qnn_bag_0.5 | rx_embedding        | HPzRx              |   0.333333 |            0.390196 |           |  0.275556  |      3.32873 |
-    | qnn_bag_0.5 | ry_embedding        | hardware_efficient |   0.333333 |            0.390196 |           |  0.275556  |     13.6979  |
-    | qnn_bag_0.5 | rx_embedding        | two_local          |   0.333333 |            0.390196 |           |  0.275556  |      4.4354  |
-    | qnn_bag_0.8 | rx_embedding        | tree_tensor        |   0.377778 |            0.38061  |           |  0.410005  |      5.84894 |
-    | qnn_bag_0.8 | ZZ_embedding        | tree_tensor        |   0.377778 |            0.38061  |           |  0.410005  |      5.47199 |
-    | qnn_bag_0.8 | rz_embedding        | tree_tensor        |   0.377778 |            0.38061  |           |  0.410005  |      5.97184 |
-    | qnn_bag_0.8 | ry_embedding        | tree_tensor        |   0.377778 |            0.38061  |           |  0.410005  |      5.88461 |
-    | qnn_bag_0.8 | ry_embedding        | two_local          |   0.355556 |            0.362092 |           |  0.3898    |      3.90912 |
-    | qnn_bag_0.8 | rx_embedding        | two_local          |   0.355556 |            0.362092 |           |  0.3898    |      3.94093 |
-    | qnn_bag_0.8 | rz_embedding        | two_local          |   0.355556 |            0.362092 |           |  0.3898    |      3.89387 |
-    | qnn_bag_0.8 | ZZ_embedding        | two_local          |   0.355556 |            0.362092 |           |  0.3898    |      3.92849 |
-    | qnn_bag_0.3 | ry_embedding        | HPzRx              |   0.222222 |            0.333333 |           |  0.0808081 |      3.34121 |
-    | qnn_bag_0.3 | rx_embedding        | HPzRx              |   0.222222 |            0.333333 |           |  0.0808081 |      3.46206 |
-    | qnn_bag_0.3 | rz_embedding        | HPzRx              |   0.222222 |            0.333333 |           |  0.0808081 |      3.39287 |
-    | qnn_bag_0.3 | ZZ_embedding        | HPzRx              |   0.222222 |            0.333333 |           |  0.0808081 |      4.083   |
-    | qnn_bag_0.3 | rx_embedding        | tree_tensor        |   0.222222 |            0.333333 |           |  0.0808081 |      5.86537 |
-    | qnn_bag_0.3 | amplitude_embedding | two_local          |   0.222222 |            0.333333 |           |  0.0808081 |      4.51937 |
-    | qnn_bag_0.3 | ZZ_embedding        | two_local          |   0.222222 |            0.333333 |           |  0.0808081 |      3.939   |
-    | qnn_bag_0.3 | rz_embedding        | two_local          |   0.222222 |            0.333333 |           |  0.0808081 |      3.9069  |
-    | qnn_bag_0.3 | ry_embedding        | two_local          |   0.222222 |            0.333333 |           |  0.0808081 |      3.88555 |
-    | qnn_bag_0.3 | rx_embedding        | two_local          |   0.222222 |            0.333333 |           |  0.0808081 |      3.95736 |
-    | qnn_bag_0.3 | amplitude_embedding | tree_tensor        |   0.222222 |            0.333333 |           |  0.0808081 |      5.45911 |
-    | qnn_bag_0.3 | ZZ_embedding        | tree_tensor        |   0.222222 |            0.333333 |           |  0.0808081 |      5.95279 |
-    | qnn_bag_0.3 | rz_embedding        | tree_tensor        |   0.222222 |            0.333333 |           |  0.0808081 |      6.21761 |
-    | qnn_bag_0.3 | ry_embedding        | tree_tensor        |   0.222222 |            0.333333 |           |  0.0808081 |      5.92094 |
-    | qnn_bag_0.3 | amplitude_embedding | hardware_efficient |   0.222222 |            0.333333 |           |  0.0808081 |     13.4813  |
-    | qnn_bag_0.3 | ZZ_embedding        | hardware_efficient |   0.222222 |            0.333333 |           |  0.0808081 |     13.408   |
-    | qnn_bag_0.3 | rz_embedding        | hardware_efficient |   0.222222 |            0.333333 |           |  0.0808081 |     13.3913  |
-    | qnn_bag_0.3 | ry_embedding        | hardware_efficient |   0.222222 |            0.333333 |           |  0.0808081 |     13.354   |
-    | qnn_bag_0.3 | rx_embedding        | hardware_efficient |   0.222222 |            0.333333 |           |  0.0808081 |     13.8513  |
-    | qnn_bag_0.3 | amplitude_embedding | HPzRx              |   0.222222 |            0.333333 |           |  0.0808081 |      3.33983 |
+    | Model       | Embedding           | Ansatz             |   Accuracy |   Balanced Accuracy |   ROC AUC |   F1 Score |   Time taken |
+    |:------------|:--------------------|:-------------------|-----------:|--------------------:|----------:|-----------:|-------------:|
+    | qsvm        | amplitude_embedding | ~                  |   0.807018 |            0.782339 |  0.782339 |   0.802547 |     43.7487  |
+    | qnn         | amplitude_embedding | hardware_efficient |   0.77193  |            0.743218 |  0.743218 |   0.765533 |      7.92101 |
+    | qnn         | ry_embedding        | hardware_efficient |   0.71345  |            0.689677 |  0.689677 |   0.709295 |      8.00107 |
+    | qnn         | rz_embedding        | HPzRx              |   0.707602 |            0.687322 |  0.687322 |   0.704992 |      1.61301 |
+    | qnn         | rx_embedding        | hardware_efficient |   0.707602 |            0.687322 |  0.687322 |   0.704992 |      7.95751 |
+    | qnn         | rz_embedding        | hardware_efficient |   0.707602 |            0.677327 |  0.677327 |   0.700129 |      7.7675  |
+    | qnn         | amplitude_embedding | HPzRx              |   0.707602 |            0.677327 |  0.677327 |   0.700129 |      1.84443 |
+    | qnn         | ry_embedding        | HPzRx              |   0.690058 |            0.672758 |  0.672758 |   0.688787 |      1.78982 |
+    | qnn         | rx_embedding        | HPzRx              |   0.701754 |            0.662479 |  0.662479 |   0.688319 |      1.74136 |
+    | qnn         | rx_embedding        | two_local          |   0.672515 |            0.648201 |  0.648201 |   0.668402 |      1.97186 |
+    | qsvm        | ry_embedding        | ~                  |   0.684211 |            0.647915 |  0.647915 |   0.672813 |     42.0951  |
+    | qsvm        | rx_embedding        | ~                  |   0.684211 |            0.647915 |  0.647915 |   0.672813 |     42.0835  |
+    | qsvm        | rz_embedding        | ~                  |   0.684211 |            0.647915 |  0.647915 |   0.672813 |     42.0728  |
+    | qnn         | amplitude_embedding | two_local          |   0.660819 |            0.645988 |  0.645988 |   0.660819 |      1.862   |
+    | qnn_bag_0.5 | amplitude_embedding | tree_tensor        |   0.684211 |            0.642918 |  0.642918 |   0.668975 |      2.29442 |
+    | qnn         | rx_embedding        | tree_tensor        |   0.654971 |            0.641134 |  0.641134 |   0.655388 |      1.44079 |
+    | qnn         | rz_embedding        | two_local          |   0.660819 |            0.630997 |  0.630997 |   0.653742 |      1.92491 |
+    | qnn         | rz_embedding        | tree_tensor        |   0.637427 |            0.629069 |  0.629069 |   0.639648 |      1.43276 |
+    | qnn         | ry_embedding        | tree_tensor        |   0.649123 |            0.628784 |  0.628784 |   0.647148 |      1.49096 |
+    | qnn         | amplitude_embedding | tree_tensor        |   0.643275 |            0.623929 |  0.623929 |   0.641812 |      1.48968 |
+    | qnn_bag_0.8 | ry_embedding        | HPzRx              |   0.666667 |            0.613364 |  0.613364 |   0.639261 |      3.05536 |
+    | qnn_bag_0.8 | ry_embedding        | two_local          |   0.643275 |            0.601442 |  0.601442 |   0.627205 |      3.4717  |
+    | qnn_bag_0.8 | amplitude_embedding | tree_tensor        |   0.614035 |            0.592162 |  0.592162 |   0.611863 |      2.0676  |
+    | qnn_bag_0.8 | amplitude_embedding | two_local          |   0.614035 |            0.589663 |  0.589663 |   0.61059  |      2.88992 |
+    | qnn_bag_0.8 | amplitude_embedding | HPzRx              |   0.625731 |            0.58438  |  0.58438  |   0.610027 |      3.10873 |
+    | qnn_bag_0.8 | amplitude_embedding | hardware_efficient |   0.625731 |            0.579383 |  0.579383 |   0.605158 |     10.7474  |
+    | qnn_bag_0.5 | amplitude_embedding | hardware_efficient |   0.619883 |            0.577027 |  0.577027 |   0.602759 |     10.5239  |
+    | qnn_bag_0.8 | rx_embedding        | two_local          |   0.608187 |            0.574814 |  0.574814 |   0.599111 |      3.0376  |
+    | qnn_bag_0.5 | amplitude_embedding | HPzRx              |   0.614035 |            0.574672 |  0.574672 |   0.600105 |      2.94314 |
+    | qnn         | ry_embedding        | two_local          |   0.590643 |            0.572744 |  0.572744 |   0.590643 |      2.03271 |
+    | qnn_bag_0.3 | ry_embedding        | two_local          |   0.614035 |            0.564677 |  0.564677 |   0.590048 |      2.89546 |
+    | qnn_bag_0.5 | ry_embedding        | two_local          |   0.614035 |            0.564677 |  0.564677 |   0.590048 |      2.87825 |
+    | qnn_bag_0.3 | rx_embedding        | hardware_efficient |   0.614035 |            0.564677 |  0.564677 |   0.590048 |     10.398   |
+    | qnn_bag_0.5 | rx_embedding        | hardware_efficient |   0.614035 |            0.564677 |  0.564677 |   0.590048 |     10.4352  |
+    | qnn_bag_0.5 | rz_embedding        | hardware_efficient |   0.608187 |            0.559823 |  0.559823 |   0.585266 |     10.5017  |
+    | qnn_bag_0.3 | rz_embedding        | hardware_efficient |   0.608187 |            0.559823 |  0.559823 |   0.585266 |     10.459   |
+    | qnn_bag_0.8 | rz_embedding        | two_local          |   0.608187 |            0.559823 |  0.559823 |   0.585266 |      2.90858 |
+    | qnn_bag_0.5 | ry_embedding        | HPzRx              |   0.602339 |            0.557467 |  0.557467 |   0.583154 |      3.34753 |
+    | qnn_bag_0.3 | ry_embedding        | HPzRx              |   0.602339 |            0.557467 |  0.557467 |   0.583154 |      2.8865  |
+    | qnn_bag_0.8 | rx_embedding        | hardware_efficient |   0.614035 |            0.557182 |  0.557182 |   0.580603 |     10.668   |
+    | qnn_bag_0.8 | rz_embedding        | tree_tensor        |   0.578947 |            0.55554  |  0.55554  |   0.576578 |      2.0455  |
+    | qnn_bag_0.5 | rz_embedding        | tree_tensor        |   0.578947 |            0.55554  |  0.55554  |   0.576578 |      2.01763 |
+    | qnn_bag_0.3 | rz_embedding        | tree_tensor        |   0.578947 |            0.55554  |  0.55554  |   0.576578 |      2.42137 |
+    | qnn_bag_0.3 | ry_embedding        | hardware_efficient |   0.602339 |            0.554969 |  0.554969 |   0.58048  |     10.53    |
+    | qnn_bag_0.5 | ry_embedding        | hardware_efficient |   0.602339 |            0.554969 |  0.554969 |   0.58048  |     10.0354  |
+    | qnn_bag_0.5 | rz_embedding        | HPzRx              |   0.608187 |            0.554826 |  0.554826 |   0.579267 |      2.89535 |
+    | qnn_bag_0.3 | rz_embedding        | HPzRx              |   0.608187 |            0.554826 |  0.554826 |   0.579267 |      3.23855 |
+    | qnn_bag_0.3 | ry_embedding        | tree_tensor        |   0.608187 |            0.554826 |  0.554826 |   0.579267 |      2.06946 |
+    | qnn_bag_0.8 | rz_embedding        | hardware_efficient |   0.608187 |            0.554826 |  0.554826 |   0.579267 |     10.5748  |
+    | qnn_bag_0.5 | ry_embedding        | tree_tensor        |   0.608187 |            0.554826 |  0.554826 |   0.579267 |      2.06709 |
+    | qnn_bag_0.8 | ry_embedding        | tree_tensor        |   0.608187 |            0.554826 |  0.554826 |   0.579267 |      2.49849 |
+    | qnn_bag_0.8 | ry_embedding        | hardware_efficient |   0.608187 |            0.552327 |  0.552327 |   0.575973 |     10.6611  |
+    | qnn_bag_0.8 | rz_embedding        | HPzRx              |   0.584795 |            0.5504   |  0.5504   |   0.575177 |      2.91932 |
+    | qnn_bag_0.3 | rx_embedding        | HPzRx              |   0.590643 |            0.547758 |  0.547758 |   0.573467 |      3.04813 |
+    | qnn_bag_0.5 | rx_embedding        | HPzRx              |   0.590643 |            0.547758 |  0.547758 |   0.573467 |      2.8814  |
+    | qnn_bag_0.8 | rx_embedding        | HPzRx              |   0.608187 |            0.54733  |  0.54733  |   0.56875  |      3.32461 |
+    | qnn_bag_0.5 | amplitude_embedding | two_local          |   0.573099 |            0.535694 |  0.535694 |   0.561126 |      2.8526  |
+    | qnn_bag_0.8 | rx_embedding        | tree_tensor        |   0.584795 |            0.530411 |  0.530411 |   0.554148 |      2.35702 |
+    | qnn_bag_0.5 | rz_embedding        | two_local          |   0.584795 |            0.530411 |  0.530411 |   0.554148 |      2.83122 |
+    | qnn_bag_0.3 | rz_embedding        | two_local          |   0.584795 |            0.530411 |  0.530411 |   0.554148 |      3.22892 |
+    | qnn_bag_0.5 | rx_embedding        | two_local          |   0.584795 |            0.530411 |  0.530411 |   0.554148 |      3.22437 |
+    | qnn_bag_0.3 | rx_embedding        | two_local          |   0.584795 |            0.530411 |  0.530411 |   0.554148 |      2.85127 |
+    | qnn_bag_0.5 | rx_embedding        | tree_tensor        |   0.584795 |            0.530411 |  0.530411 |   0.554148 |      2.05024 |
+    | qnn_bag_0.3 | rx_embedding        | tree_tensor        |   0.584795 |            0.530411 |  0.530411 |   0.554148 |      2.18715 |
+    | qnn_bag_0.8 | ZZ_embedding        | hardware_efficient |   0.590643 |            0.515277 |  0.515277 |   0.523392 |     10.3795  |
+    | qnn         | ZZ_embedding        | HPzRx              |   0.508772 |            0.504783 |  0.504783 |   0.513787 |      1.94063 |
+    | qnn_bag_0.8 | ZZ_embedding        | tree_tensor        |   0.602339 |            0.5      |  0.5      |   0.452854 |      2.57792 |
+    | qnn_bag_0.5 | ZZ_embedding        | hardware_efficient |   0.602339 |            0.5      |  0.5      |   0.452854 |     10.6524  |
+    | qnn_bag_0.3 | ZZ_embedding        | hardware_efficient |   0.602339 |            0.5      |  0.5      |   0.452854 |     10.6306  |
+    | qnn_bag_0.5 | ZZ_embedding        | two_local          |   0.602339 |            0.5      |  0.5      |   0.452854 |      2.86801 |
+    | qnn_bag_0.3 | ZZ_embedding        | two_local          |   0.602339 |            0.5      |  0.5      |   0.452854 |      2.87458 |
+    | qsvm        | ZZ_embedding        | ~                  |   0.602339 |            0.5      |  0.5      |   0.452854 |     43.0182  |
+    | qnn_bag_0.3 | ZZ_embedding        | HPzRx              |   0.602339 |            0.5      |  0.5      |   0.452854 |      2.89995 |
+    | qnn_bag_0.5 | ZZ_embedding        | HPzRx              |   0.602339 |            0.5      |  0.5      |   0.452854 |      3.35156 |
+    | qnn_bag_0.3 | amplitude_embedding | tree_tensor        |   0.602339 |            0.5      |  0.5      |   0.452854 |      2.16821 |
+    | qnn_bag_0.3 | ZZ_embedding        | tree_tensor        |   0.602339 |            0.5      |  0.5      |   0.452854 |      2.1247  |
+    | qnn_bag_0.5 | ZZ_embedding        | tree_tensor        |   0.602339 |            0.5      |  0.5      |   0.452854 |      2.07843 |
+    | qnn_bag_0.8 | ZZ_embedding        | two_local          |   0.590643 |            0.49279  |  0.49279  |   0.457223 |      3.03675 |
+    | qnn_bag_0.8 | ZZ_embedding        | HPzRx              |   0.561404 |            0.478512 |  0.478512 |   0.473343 |      3.07628 |
+    | qnn_bag_0.3 | amplitude_embedding | hardware_efficient |   0.532164 |            0.474229 |  0.474229 |   0.495696 |     10.6454  |
+    | qnn         | ZZ_embedding        | tree_tensor        |   0.48538  |            0.470374 |  0.470374 |   0.488533 |      1.41871 |
+    | qnn_bag_0.3 | amplitude_embedding | HPzRx              |   0.526316 |            0.466876 |  0.466876 |   0.48737  |      3.63382 |
+    | qnn_bag_0.3 | amplitude_embedding | two_local          |   0.526316 |            0.466876 |  0.466876 |   0.48737  |      3.10482 |
+    | qnn         | ZZ_embedding        | hardware_efficient |   0.467836 |            0.463307 |  0.463307 |   0.473372 |      8.22384 |
+    | qnn         | ZZ_embedding        | two_local          |   0.461988 |            0.455954 |  0.455954 |   0.467481 |      2.13294 |
     """
 
     
     def __init__(self, nqubits=8, randomstate=1234, predictions=False, ignoreWarnings=True, numPredictors=10, numLayers=5, customMetric=None, customImputerNum=None, customImputerCat=None, classifiers=["all"],ansatzs=["all"],embeddings=["all"],features=[0.3,0.5,0.8],verbose=False,optimizer=None,learningRate=0.01,epochs=100,runs=1,maxSamples=1.0):
         errors = 0
         errormsg = []
```

### Comparing `lazyqml-0.3.0/lazyqml.egg-info/PKG-INFO` & `lazyqml-0.3.1/lazyqml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.3.0
+Version: 0.3.1
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>, Fernando Álvaro Plou Llorente <ploufernando@uniovi.es>, Alejandro Leal Castaño <lealcalejandro@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyqml-0.3.0/lazyqml.egg-info/SOURCES.txt` & `lazyqml-0.3.1/lazyqml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/mkdocs.yml` & `lazyqml-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/pyproject.toml` & `lazyqml-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lazyqml"
-version = "0.3.0"
+version = "0.3.1"
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
-current_version = "0.3.0"
+current_version = "0.3.1"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `lazyqml-0.3.0/requirements.txt` & `lazyqml-0.3.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/requirements_dev.txt` & `lazyqml-0.3.1/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `lazyqml-0.3.0/tests/test_lazyqml.py` & `lazyqml-0.3.1/tests/test_lazyqml.py`

 * *Files identical despite different names*

