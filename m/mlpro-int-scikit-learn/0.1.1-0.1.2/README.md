# Comparing `tmp/mlpro_int_scikit_learn-0.1.1.tar.gz` & `tmp/mlpro_int_scikit_learn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro_int_scikit_learn-0.1.1.tar", last modified: Thu Apr 18 19:40:40 2024, max compression
+gzip compressed data, was "mlpro_int_scikit_learn-0.1.2.tar", last modified: Thu May  9 06:56:29 2024, max compression
```

## Comparing `mlpro_int_scikit_learn-0.1.1.tar` & `mlpro_int_scikit_learn-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:40.504948 mlpro_int_scikit_learn-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-18 19:40:36.000000 mlpro_int_scikit_learn-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-18 19:40:40.504948 mlpro_int_scikit_learn-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-18 19:40:36.000000 mlpro_int_scikit_learn-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 19:40:36.000000 mlpro_int_scikit_learn-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-18 19:40:40.504948 mlpro_int_scikit_learn-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:40.500949 mlpro_int_scikit_learn-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:40.504948 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_scikit_learn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-18 19:40:40.000000 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_scikit_learn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-18 19:40:40.000000 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_scikit_learn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:40:40.000000 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_scikit_learn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 19:40:40.000000 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_scikit_learn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 19:40:40.000000 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_scikit_learn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:40.500949 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:36.000000 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_sklearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:40.504948 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_sklearn/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-18 19:40:36.000000 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_sklearn/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-18 19:40:36.000000 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_sklearn/wrappers/anomalydetectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-18 19:40:36.000000 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_sklearn/wrappers/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10749 2024-04-18 19:40:36.000000 mlpro_int_scikit_learn-0.1.1/src/mlpro_int_sklearn/wrappers/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:40.504948 mlpro_int_scikit_learn-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-18 19:40:36.000000 mlpro_int_scikit_learn-0.1.1/test/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:56:29.438198 mlpro_int_scikit_learn-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-09 06:56:29.438198 mlpro_int_scikit_learn-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-09 06:56:29.438198 mlpro_int_scikit_learn-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:56:29.430198 mlpro_int_scikit_learn-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:56:29.434198 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_scikit_learn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-09 06:56:29.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_scikit_learn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-09 06:56:29.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_scikit_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:56:29.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_scikit_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 06:56:29.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_scikit_learn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 06:56:29.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_scikit_learn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:56:29.434198 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:56:29.434198 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:56:29.434198 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/wrappers/anomalydetectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/wrappers/anomalydetectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/wrappers/anomalydetectors/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/wrappers/anomalydetectors/isof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/wrappers/anomalydetectors/lof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/wrappers/anomalydetectors/ocsvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/wrappers/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10749 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/wrappers/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:56:29.434198 mlpro_int_scikit_learn-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-09 06:56:21.000000 mlpro_int_scikit_learn-0.1.2/test/test_examples.py
```

### Comparing `mlpro_int_scikit_learn-0.1.1/LICENSE` & `mlpro_int_scikit_learn-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro_int_scikit_learn-0.1.1/PKG-INFO` & `mlpro_int_scikit_learn-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mlpro-int-scikit-learn
-Version: 0.1.1
+Version: 0.1.2
 Summary: MLPro: Integration scikit-learn
 Home-page: https://mlpro-int-scikit-learn.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-scikit-learn.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.3; extra == "full"
 Requires-Dist: scikit-learn>=1.4.1; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-Scikit-learn/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-Scikit-learn/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-scikit-learn/badge/?version=latest)](https://mlpro-int-scikit-learn.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-openml.svg)](https://badge.fury.io/py/mlpro-int-openml)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-openml/mlpro-int-openml/badges/version.svg)](https://anaconda.org/mlpro-int-openml/mlpro)
```

### Comparing `mlpro_int_scikit_learn-0.1.1/README.md` & `mlpro_int_scikit_learn-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mlpro_int_scikit_learn-0.1.1/setup.cfg` & `mlpro_int_scikit_learn-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro-int-scikit-learn
-version = 0.1.1
+version = 0.1.2
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro: Integration scikit-learn
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro-int-scikit-learn.readthedocs.io
 project_urls = 
@@ -22,14 +22,14 @@
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 full = 
-	mlpro[full]>=1.4.0
+	mlpro[full]>=1.4.3
 	scikit-learn>=1.4.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mlpro_int_scikit_learn-0.1.1/src/mlpro_int_scikit_learn.egg-info/PKG-INFO` & `mlpro_int_scikit_learn-0.1.2/src/mlpro_int_scikit_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mlpro-int-scikit-learn
-Version: 0.1.1
+Version: 0.1.2
 Summary: MLPro: Integration scikit-learn
 Home-page: https://mlpro-int-scikit-learn.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-scikit-learn.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.3; extra == "full"
 Requires-Dist: scikit-learn>=1.4.1; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-Scikit-learn/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-Scikit-learn/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-scikit-learn/badge/?version=latest)](https://mlpro-int-scikit-learn.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-openml.svg)](https://badge.fury.io/py/mlpro-int-openml)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-openml/mlpro-int-openml/badges/version.svg)](https://anaconda.org/mlpro-int-openml/mlpro)
```

### Comparing `mlpro_int_scikit_learn-0.1.1/src/mlpro_int_scikit_learn.egg-info/SOURCES.txt` & `mlpro_int_scikit_learn-0.1.2/src/mlpro_int_scikit_learn.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,12 +4,17 @@
 setup.cfg
 src/mlpro_int_scikit_learn.egg-info/PKG-INFO
 src/mlpro_int_scikit_learn.egg-info/SOURCES.txt
 src/mlpro_int_scikit_learn.egg-info/dependency_links.txt
 src/mlpro_int_scikit_learn.egg-info/requires.txt
 src/mlpro_int_scikit_learn.egg-info/top_level.txt
 src/mlpro_int_sklearn/__init__.py
+src/mlpro_int_sklearn/test.py
 src/mlpro_int_sklearn/wrappers/__init__.py
-src/mlpro_int_sklearn/wrappers/anomalydetectors.py
 src/mlpro_int_sklearn/wrappers/basics.py
 src/mlpro_int_sklearn/wrappers/streams.py
+src/mlpro_int_sklearn/wrappers/anomalydetectors/__init__.py
+src/mlpro_int_sklearn/wrappers/anomalydetectors/basics.py
+src/mlpro_int_sklearn/wrappers/anomalydetectors/isof.py
+src/mlpro_int_sklearn/wrappers/anomalydetectors/lof.py
+src/mlpro_int_sklearn/wrappers/anomalydetectors/ocsvm.py
 test/test_examples.py
```

### Comparing `mlpro_int_scikit_learn-0.1.1/src/mlpro_int_sklearn/wrappers/basics.py` & `mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/wrappers/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro_int_scikit_learn-0.1.1/src/mlpro_int_sklearn/wrappers/streams.py` & `mlpro_int_scikit_learn-0.1.2/src/mlpro_int_sklearn/wrappers/streams.py`

 * *Files identical despite different names*

### Comparing `mlpro_int_scikit_learn-0.1.1/test/test_examples.py` & `mlpro_int_scikit_learn-0.1.2/test/test_examples.py`

 * *Files identical despite different names*

