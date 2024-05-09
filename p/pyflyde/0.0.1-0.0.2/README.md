# Comparing `tmp/pyflyde-0.0.1.tar.gz` & `tmp/pyflyde-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflyde-0.0.1.tar", last modified: Thu May  9 12:08:28 2024, max compression
+gzip compressed data, was "pyflyde-0.0.2.tar", last modified: Thu May  9 16:17:28 2024, max compression
```

## Comparing `pyflyde-0.0.1.tar` & `pyflyde-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 12:08:28.072039 pyflyde-0.0.1/
--rw-r--r--   0 trustmaster   (501) staff       (20)    11345 2024-04-09 17:14:23.000000 pyflyde-0.0.1/LICENSE
--rw-r--r--   0 trustmaster   (501) staff       (20)    15923 2024-05-09 12:08:28.071616 pyflyde-0.0.1/PKG-INFO
--rw-r--r--   0 trustmaster   (501) staff       (20)     1831 2024-05-09 11:09:39.000000 pyflyde-0.0.1/README.md
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 12:08:28.066276 pyflyde-0.0.1/pyflyde.egg-info/
--rw-r--r--   0 trustmaster   (501) staff       (20)    15923 2024-05-09 12:08:27.000000 pyflyde-0.0.1/pyflyde.egg-info/PKG-INFO
--rw-r--r--   0 trustmaster   (501) staff       (20)      272 2024-05-09 12:08:28.000000 pyflyde-0.0.1/pyflyde.egg-info/SOURCES.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)        1 2024-05-09 12:08:27.000000 pyflyde-0.0.1/pyflyde.egg-info/dependency_links.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)       42 2024-05-09 12:08:27.000000 pyflyde-0.0.1/pyflyde.egg-info/requires.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)        1 2024-05-09 12:08:27.000000 pyflyde-0.0.1/pyflyde.egg-info/top_level.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)     1112 2024-05-09 12:07:57.000000 pyflyde-0.0.1/pyproject.toml
--rw-r--r--   0 trustmaster   (501) staff       (20)       70 2024-05-09 12:08:28.073013 pyflyde-0.0.1/setup.cfg
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 12:08:28.058842 pyflyde-0.0.1/tests/
--rw-r--r--   0 trustmaster   (501) staff       (20)     1933 2024-05-09 10:46:21.000000 pyflyde-0.0.1/tests/test_flow.py
--rw-r--r--   0 trustmaster   (501) staff       (20)    10544 2024-05-09 10:46:21.000000 pyflyde-0.0.1/tests/test_io.py
--rw-r--r--   0 trustmaster   (501) staff       (20)    11312 2024-05-09 10:46:21.000000 pyflyde-0.0.1/tests/test_node.py
--rw-r--r--   0 trustmaster   (501) staff       (20)     3754 2024-05-09 10:46:21.000000 pyflyde-0.0.1/tests/test_stdlib.py
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:17:28.843284 pyflyde-0.0.2/
+-rw-r--r--   0 trustmaster   (501) staff       (20)    11345 2024-04-09 17:14:23.000000 pyflyde-0.0.2/LICENSE
+-rw-r--r--   0 trustmaster   (501) staff       (20)    15929 2024-05-09 16:17:28.842734 pyflyde-0.0.2/PKG-INFO
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1831 2024-05-09 11:09:39.000000 pyflyde-0.0.2/README.md
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:17:28.816622 pyflyde-0.0.2/flyde/
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:17:28.840093 pyflyde-0.0.2/flyde/pyflyde.egg-info/
+-rw-r--r--   0 trustmaster   (501) staff       (20)    15929 2024-05-09 16:17:28.000000 pyflyde-0.0.2/flyde/pyflyde.egg-info/PKG-INFO
+-rw-r--r--   0 trustmaster   (501) staff       (20)      311 2024-05-09 16:17:28.000000 pyflyde-0.0.2/flyde/pyflyde.egg-info/SOURCES.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)        1 2024-05-09 16:17:28.000000 pyflyde-0.0.2/flyde/pyflyde.egg-info/dependency_links.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)       48 2024-05-09 16:17:28.000000 pyflyde-0.0.2/flyde/pyflyde.egg-info/requires.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)        1 2024-05-09 16:17:28.000000 pyflyde-0.0.2/flyde/pyflyde.egg-info/top_level.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1173 2024-05-09 12:58:28.000000 pyflyde-0.0.2/pyproject.toml
+-rw-r--r--   0 trustmaster   (501) staff       (20)      162 2024-05-09 16:17:28.844527 pyflyde-0.0.2/setup.cfg
+-rw-r--r--   0 trustmaster   (501) staff       (20)       68 2024-05-09 12:59:59.000000 pyflyde-0.0.2/setup.py
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 16:17:28.836624 pyflyde-0.0.2/tests/
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1933 2024-05-09 10:46:21.000000 pyflyde-0.0.2/tests/test_flow.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)    10544 2024-05-09 10:46:21.000000 pyflyde-0.0.2/tests/test_io.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)    11312 2024-05-09 10:46:21.000000 pyflyde-0.0.2/tests/test_node.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)     3754 2024-05-09 10:46:21.000000 pyflyde-0.0.2/tests/test_stdlib.py
```

### Comparing `pyflyde-0.0.1/LICENSE` & `pyflyde-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.1/PKG-INFO` & `pyflyde-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyflyde
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SDK and runtime for Flyde - a visual flow-based programming language and IDE.
-Author-email: Vladimir Sibirov <trustmaster@kodigy.com>
+Author: Vladimir Sibirov
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -222,14 +222,15 @@
 License-File: LICENSE
 Requires-Dist: pyyaml
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 # PyFlyde
 
 ![Build](https://github.com/trustmaster/pyflyde/actions/workflows/python-package.yml/badge.svg)
 
 Python runtime for [Flyde](https://github.com/flydelabs/flyde) with Data Engineering emphasis.
```

### Comparing `pyflyde-0.0.1/README.md` & `pyflyde-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.1/pyflyde.egg-info/PKG-INFO` & `pyflyde-0.0.2/flyde/pyflyde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyflyde
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SDK and runtime for Flyde - a visual flow-based programming language and IDE.
-Author-email: Vladimir Sibirov <trustmaster@kodigy.com>
+Author: Vladimir Sibirov
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -222,14 +222,15 @@
 License-File: LICENSE
 Requires-Dist: pyyaml
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 # PyFlyde
 
 ![Build](https://github.com/trustmaster/pyflyde/actions/workflows/python-package.yml/badge.svg)
 
 Python runtime for [Flyde](https://github.com/flydelabs/flyde) with Data Engineering emphasis.
```

### Comparing `pyflyde-0.0.1/pyproject.toml` & `pyflyde-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "pyflyde"
-version = "0.0.1"
+version = "0.0.2"
 requires-python = ">= 3.9"
 authors = [
-    {name = "Vladimir Sibirov", email = "trustmaster@kodigy.com"}
+    {name = "Vladimir Sibirov"}
 ]
 description="Python SDK and runtime for Flyde - a visual flow-based programming language and IDE."
 readme="README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
@@ -24,17 +24,22 @@
 ]
 license = { file = "LICENSE" }
 
 dependencies = [
     "pyyaml",
 ]
 
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
 [tool.setuptools.packages.find]
 where = ["flyde", "examples/mylib"]
 
 [project.optional-dependencies]
 dev = [
     "build",
     "black",
     "coverage",
     "flake8",
+    "twine",
 ]
```

### Comparing `pyflyde-0.0.1/tests/test_flow.py` & `pyflyde-0.0.2/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.1/tests/test_io.py` & `pyflyde-0.0.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.1/tests/test_node.py` & `pyflyde-0.0.2/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.1/tests/test_stdlib.py` & `pyflyde-0.0.2/tests/test_stdlib.py`

 * *Files identical despite different names*

