# Comparing `tmp/pyflyde-0.0.2.tar.gz` & `tmp/pyflyde-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflyde-0.0.2.tar", last modified: Thu May  9 16:17:28 2024, max compression
+gzip compressed data, was "pyflyde-0.0.3.tar", last modified: Thu May  9 16:52:16 2024, max compression
```

## Comparing `pyflyde-0.0.2.tar` & `pyflyde-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,51 @@
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:17:28.843284 pyflyde-0.0.2/
--rw-r--r--   0 trustmaster   (501) staff       (20)    11345 2024-04-09 17:14:23.000000 pyflyde-0.0.2/LICENSE
--rw-r--r--   0 trustmaster   (501) staff       (20)    15929 2024-05-09 16:17:28.842734 pyflyde-0.0.2/PKG-INFO
--rw-r--r--   0 trustmaster   (501) staff       (20)     1831 2024-05-09 11:09:39.000000 pyflyde-0.0.2/README.md
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:17:28.816622 pyflyde-0.0.2/flyde/
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:17:28.840093 pyflyde-0.0.2/flyde/pyflyde.egg-info/
--rw-r--r--   0 trustmaster   (501) staff       (20)    15929 2024-05-09 16:17:28.000000 pyflyde-0.0.2/flyde/pyflyde.egg-info/PKG-INFO
--rw-r--r--   0 trustmaster   (501) staff       (20)      311 2024-05-09 16:17:28.000000 pyflyde-0.0.2/flyde/pyflyde.egg-info/SOURCES.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)        1 2024-05-09 16:17:28.000000 pyflyde-0.0.2/flyde/pyflyde.egg-info/dependency_links.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)       48 2024-05-09 16:17:28.000000 pyflyde-0.0.2/flyde/pyflyde.egg-info/requires.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)        1 2024-05-09 16:17:28.000000 pyflyde-0.0.2/flyde/pyflyde.egg-info/top_level.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)     1173 2024-05-09 12:58:28.000000 pyflyde-0.0.2/pyproject.toml
--rw-r--r--   0 trustmaster   (501) staff       (20)      162 2024-05-09 16:17:28.844527 pyflyde-0.0.2/setup.cfg
--rw-r--r--   0 trustmaster   (501) staff       (20)       68 2024-05-09 12:59:59.000000 pyflyde-0.0.2/setup.py
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:17:28.836624 pyflyde-0.0.2/tests/
--rw-r--r--   0 trustmaster   (501) staff       (20)     1933 2024-05-09 10:46:21.000000 pyflyde-0.0.2/tests/test_flow.py
--rw-r--r--   0 trustmaster   (501) staff       (20)    10544 2024-05-09 10:46:21.000000 pyflyde-0.0.2/tests/test_io.py
--rw-r--r--   0 trustmaster   (501) staff       (20)    11312 2024-05-09 10:46:21.000000 pyflyde-0.0.2/tests/test_node.py
--rw-r--r--   0 trustmaster   (501) staff       (20)     3754 2024-05-09 10:46:21.000000 pyflyde-0.0.2/tests/test_stdlib.py
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:52:16.908177 pyflyde-0.0.3/
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:52:16.768475 pyflyde-0.0.3/.github/
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:52:16.799784 pyflyde-0.0.3/.github/workflows/
+-rw-r--r--   0 trustmaster   (501) staff       (20)      984 2024-05-09 11:09:26.000000 pyflyde-0.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0 trustmaster   (501) staff       (20)     3197 2024-05-09 10:46:21.000000 pyflyde-0.0.3/.gitignore
+-rw-r--r--   0 trustmaster   (501) staff       (20)    11345 2024-04-09 17:14:23.000000 pyflyde-0.0.3/LICENSE
+-rw-r--r--   0 trustmaster   (501) staff       (20)      999 2024-05-09 16:10:00.000000 pyflyde-0.0.3/Makefile
+-rw-r--r--   0 trustmaster   (501) staff       (20)    16027 2024-05-09 16:52:16.907673 pyflyde-0.0.3/PKG-INFO
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1887 2024-05-09 16:21:19.000000 pyflyde-0.0.3/README.md
+-rw-r--r--   0 trustmaster   (501) staff       (20)   265919 2024-05-09 10:46:21.000000 pyflyde-0.0.3/clustering_example.png
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:52:16.808408 pyflyde-0.0.3/examples/
+-rw-r--r--   0 trustmaster   (501) staff       (20)     4489 2024-05-09 10:46:21.000000 pyflyde-0.0.3/examples/Clustering.flyde
+-rw-r--r--   0 trustmaster   (501) staff       (20)      991 2024-04-09 17:14:23.000000 pyflyde-0.0.3/examples/HelloPy.flyde
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:52:16.809836 pyflyde-0.0.3/examples/datasets/
+-rw-r--r--   0 trustmaster   (501) staff       (20)    11089 2024-04-09 17:14:23.000000 pyflyde-0.0.3/examples/datasets/wine-clustering.csv
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:52:16.828790 pyflyde-0.0.3/examples/mylib/
+-rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-04-09 17:14:23.000000 pyflyde-0.0.3/examples/mylib/__init__.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)      560 2024-04-21 06:51:36.000000 pyflyde-0.0.3/examples/mylib/components.flyde.ts
+-rw-r--r--   0 trustmaster   (501) staff       (20)      725 2024-04-13 14:14:04.000000 pyflyde-0.0.3/examples/mylib/components.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)      684 2024-05-09 10:46:21.000000 pyflyde-0.0.3/examples/mylib/dataframe.flyde.ts
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1353 2024-05-09 10:46:21.000000 pyflyde-0.0.3/examples/mylib/dataframe.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1619 2024-04-09 17:14:23.000000 pyflyde-0.0.3/examples/mylib/kmeans.flyde.ts
+-rw-r--r--   0 trustmaster   (501) staff       (20)     6171 2024-05-06 19:18:33.000000 pyflyde-0.0.3/examples/mylib/kmeans.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)      216 2024-04-09 17:14:23.000000 pyflyde-0.0.3/examples/pyproject.toml
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:52:16.851053 pyflyde-0.0.3/flyde/
+-rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-04-09 17:14:23.000000 pyflyde-0.0.3/flyde/__init__.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)     4559 2024-05-09 10:46:21.000000 pyflyde-0.0.3/flyde/flow.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)     9925 2024-05-09 10:46:21.000000 pyflyde-0.0.3/flyde/io.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)    17280 2024-05-09 10:46:21.000000 pyflyde-0.0.3/flyde/node.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1670 2024-05-09 10:46:21.000000 pyflyde-0.0.3/flyde/stdlib.py
+-rwxr-xr-x   0 trustmaster   (501) staff       (20)     2217 2024-05-04 13:30:20.000000 pyflyde-0.0.3/flyde.py
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:52:16.901977 pyflyde-0.0.3/pyflyde.egg-info/
+-rw-r--r--   0 trustmaster   (501) staff       (20)    16027 2024-05-09 16:52:16.000000 pyflyde-0.0.3/pyflyde.egg-info/PKG-INFO
+-rw-r--r--   0 trustmaster   (501) staff       (20)      926 2024-05-09 16:52:16.000000 pyflyde-0.0.3/pyflyde.egg-info/SOURCES.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)        1 2024-05-09 16:52:16.000000 pyflyde-0.0.3/pyflyde.egg-info/dependency_links.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)       59 2024-05-09 16:52:16.000000 pyflyde-0.0.3/pyflyde.egg-info/requires.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)        1 2024-05-09 16:52:16.000000 pyflyde-0.0.3/pyflyde.egg-info/top_level.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1209 2024-05-09 16:51:26.000000 pyflyde-0.0.3/pyproject.toml
+-rw-r--r--   0 trustmaster   (501) staff       (20)       70 2024-05-09 16:52:16.910292 pyflyde-0.0.3/setup.cfg
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:52:16.897129 pyflyde-0.0.3/tests/
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1744 2024-05-09 10:46:21.000000 pyflyde-0.0.3/tests/Repeat3Times.flyde
+-rw-r--r--   0 trustmaster   (501) staff       (20)      782 2024-04-25 19:45:07.000000 pyflyde-0.0.3/tests/TestInOutFlow.flyde
+-rw-r--r--   0 trustmaster   (501) staff       (20)      820 2024-04-24 22:56:30.000000 pyflyde-0.0.3/tests/TestIsolatedFlow.flyde
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1798 2024-05-09 10:46:21.000000 pyflyde-0.0.3/tests/TestNestedFlow.flyde
+-rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-04-09 17:26:09.000000 pyflyde-0.0.3/tests/__init.py__
+-rw-r--r--   0 trustmaster   (501) staff       (20)      914 2024-05-09 10:46:21.000000 pyflyde-0.0.3/tests/components.flyde.ts
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1185 2024-05-09 10:46:21.000000 pyflyde-0.0.3/tests/components.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1933 2024-05-09 10:46:21.000000 pyflyde-0.0.3/tests/test_flow.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)    10544 2024-05-09 10:46:21.000000 pyflyde-0.0.3/tests/test_io.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)    11312 2024-05-09 10:46:21.000000 pyflyde-0.0.3/tests/test_node.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)     3754 2024-05-09 10:46:21.000000 pyflyde-0.0.3/tests/test_stdlib.py
```

### Comparing `pyflyde-0.0.2/LICENSE` & `pyflyde-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.2/PKG-INFO` & `pyflyde-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflyde
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python SDK and runtime for Flyde - a visual flow-based programming language and IDE.
 Author: Vladimir Sibirov
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,27 +218,28 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
 Provides-Extra: dev
+Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # PyFlyde
 
 ![Build](https://github.com/trustmaster/pyflyde/actions/workflows/python-package.yml/badge.svg)
 
 Python runtime for [Flyde](https://github.com/flydelabs/flyde) with Data Engineering emphasis.
 
-![Example graph running K-means clustering with Pandas and Scikit-learn](./clustering_example.png)
+![Example graph running K-means clustering with Pandas and Scikit-learn](https://github.com/trustmaster/pyflyde/blob/main/clustering_example.png?raw=true)
 
 ## PoC warning
 
 This is a proof-of-concept and not a final implementation. Structure and API may change drastically before public release.
 
 ## Getting started
```

### Comparing `pyflyde-0.0.2/README.md` & `pyflyde-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # PyFlyde
 
 ![Build](https://github.com/trustmaster/pyflyde/actions/workflows/python-package.yml/badge.svg)
 
 Python runtime for [Flyde](https://github.com/flydelabs/flyde) with Data Engineering emphasis.
 
-![Example graph running K-means clustering with Pandas and Scikit-learn](./clustering_example.png)
+![Example graph running K-means clustering with Pandas and Scikit-learn](https://github.com/trustmaster/pyflyde/blob/main/clustering_example.png?raw=true)
 
 ## PoC warning
 
 This is a proof-of-concept and not a final implementation. Structure and API may change drastically before public release.
 
 ## Getting started
```

### Comparing `pyflyde-0.0.2/flyde/pyflyde.egg-info/PKG-INFO` & `pyflyde-0.0.3/pyflyde.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflyde
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python SDK and runtime for Flyde - a visual flow-based programming language and IDE.
 Author: Vladimir Sibirov
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,27 +218,28 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
 Provides-Extra: dev
+Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # PyFlyde
 
 ![Build](https://github.com/trustmaster/pyflyde/actions/workflows/python-package.yml/badge.svg)
 
 Python runtime for [Flyde](https://github.com/flydelabs/flyde) with Data Engineering emphasis.
 
-![Example graph running K-means clustering with Pandas and Scikit-learn](./clustering_example.png)
+![Example graph running K-means clustering with Pandas and Scikit-learn](https://github.com/trustmaster/pyflyde/blob/main/clustering_example.png?raw=true)
 
 ## PoC warning
 
 This is a proof-of-concept and not a final implementation. Structure and API may change drastically before public release.
 
 ## Getting started
```

### Comparing `pyflyde-0.0.2/pyproject.toml` & `pyflyde-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+[build-system]
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
 [project]
 name = "pyflyde"
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">= 3.9"
 authors = [
     {name = "Vladimir Sibirov"}
 ]
 description="Python SDK and runtime for Flyde - a visual flow-based programming language and IDE."
 readme="README.md"
 classifiers = [
@@ -24,22 +28,19 @@
 ]
 license = { file = "LICENSE" }
 
 dependencies = [
     "pyyaml",
 ]
 
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
 [tool.setuptools.packages.find]
 where = ["flyde", "examples/mylib"]
 
 [project.optional-dependencies]
 dev = [
+    "setuptools",
     "build",
     "black",
     "coverage",
     "flake8",
     "twine",
 ]
```

### Comparing `pyflyde-0.0.2/tests/test_flow.py` & `pyflyde-0.0.3/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.2/tests/test_io.py` & `pyflyde-0.0.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.2/tests/test_node.py` & `pyflyde-0.0.3/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.2/tests/test_stdlib.py` & `pyflyde-0.0.3/tests/test_stdlib.py`

 * *Files identical despite different names*

