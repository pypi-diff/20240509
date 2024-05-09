# Comparing `tmp/minq-0.0.2.tar.gz` & `tmp/minq-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minq-0.0.2.tar", last modified: Thu May  9 00:06:57 2024, max compression
+gzip compressed data, was "minq-0.0.3.tar", last modified: Thu May  9 00:19:06 2024, max compression
```

## Comparing `minq-0.0.2.tar` & `minq-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:06:57.283899 minq-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-09 00:06:53.000000 minq-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-09 00:06:57.283899 minq-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 00:06:53.000000 minq-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:06:57.279899 minq-0.0.2/minq/
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-09 00:06:53.000000 minq-0.0.2/minq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:06:57.283899 minq-0.0.2/minq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-09 00:06:57.000000 minq-0.0.2/minq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-09 00:06:57.000000 minq-0.0.2/minq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:06:57.000000 minq-0.0.2/minq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 00:06:57.000000 minq-0.0.2/minq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 00:06:57.000000 minq-0.0.2/minq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-09 00:06:53.000000 minq-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 00:06:57.283899 minq-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:19:06.061248 minq-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-09 00:18:56.000000 minq-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-09 00:19:06.057248 minq-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-09 00:18:56.000000 minq-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:19:06.057248 minq-0.0.3/minq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-09 00:18:56.000000 minq-0.0.3/minq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:19:06.057248 minq-0.0.3/minq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-09 00:19:06.000000 minq-0.0.3/minq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-09 00:19:06.000000 minq-0.0.3/minq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:19:06.000000 minq-0.0.3/minq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 00:19:06.000000 minq-0.0.3/minq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 00:19:06.000000 minq-0.0.3/minq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-09 00:18:56.000000 minq-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 00:19:06.061248 minq-0.0.3/setup.cfg
```

### Comparing `minq-0.0.2/LICENSE` & `minq-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `minq-0.0.2/PKG-INFO` & `minq-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minq
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tiny quantum gate library based on NumPy
 License: MIT License
         
         Copyright (c) 2024 fwcd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -32,10 +32,9 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy<2,>=1.26
 
 # Minq
 
 [![PyPI](https://img.shields.io/pypi/v/minq)](https://pypi.org/project/minq)
-[![Typecheck](https://github.com/fwcd/minq/actions/workflows/typecheck.yml/badge.svg)](https://github.com/fwcd/minq/actions/workflows/typecheck.yml)
 
 Tiny quantum gate library based on NumPy.
```

### Comparing `minq-0.0.2/minq/__init__.py` & `minq-0.0.3/minq/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import reduce
 from numpy.typing import ArrayLike, NDArray
-from typing import cast
+from typing import Any, cast
 
 import numpy as np
 
 I = np.identity(2)
 '''Identity transform'''
 
 X = np.array([
@@ -36,20 +36,20 @@
         return x
     else:
         assert len(args) == 1
         x = np.zeros(2 ** len(args[0]))
         x[int(args[0], base=2)] = 1
         return x
 
-def kron(*arrays: ArrayLike) -> NDArray:
+def kron(*arrays: ArrayLike) -> NDArray[Any]:
     '''Computes the Kronecker product (tensor product) of the given arrays'''
     assert len(arrays) > 0
     return reduce(np.kron, arrays)
 
-def kronpow(array: ArrayLike, n: int) -> NDArray:
+def kronpow(array: ArrayLike, n: int) -> NDArray[Any]:
     '''Applies the Kronecker product n times'''
     assert n > 0
     return reduce(lambda acc, _: np.kron(acc, array), range(n - 1), array)
 
 def from_binary(*bits: int) -> int:
     '''Converts a list of bits to the corresponding number when interpreted in base 2'''
     return 0 if len(bits) == 0 else int(''.join(map(str, bits)), base=2)
```

### Comparing `minq-0.0.2/minq.egg-info/PKG-INFO` & `minq-0.0.3/minq.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minq
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tiny quantum gate library based on NumPy
 License: MIT License
         
         Copyright (c) 2024 fwcd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -32,10 +32,9 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy<2,>=1.26
 
 # Minq
 
 [![PyPI](https://img.shields.io/pypi/v/minq)](https://pypi.org/project/minq)
-[![Typecheck](https://github.com/fwcd/minq/actions/workflows/typecheck.yml/badge.svg)](https://github.com/fwcd/minq/actions/workflows/typecheck.yml)
 
 Tiny quantum gate library based on NumPy.
```

### Comparing `minq-0.0.2/pyproject.toml` & `minq-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "minq"
-version = "0.0.2"
+version = "0.0.3"
 description = "Tiny quantum gate library based on NumPy"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 classifiers = ["Topic :: Scientific/Engineering :: Mathematics"]
 keywords = ["quantum", "computing", "circuit", "gate", "numpy"]
 dependencies = [
@@ -17,10 +17,7 @@
 
 [project.urls]
 Homepage = "https://github.com/fwcd/minq"
 Repository = "https://github.com/fwcd/minq"
 
 [tool.setuptools.packages]
 find = {}
-
-[tool.pyright]
-include = ["minq"]
```

