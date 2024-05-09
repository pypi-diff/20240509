# Comparing `tmp/minq-0.0.1.tar.gz` & `tmp/minq-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minq-0.0.1.tar", last modified: Wed May  8 23:54:10 2024, max compression
+gzip compressed data, was "minq-0.0.2.tar", last modified: Thu May  9 00:06:57 2024, max compression
```

## Comparing `minq-0.0.1.tar` & `minq-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2024-05-08 23:54:10.912704 minq-0.0.1/
--rw-r--r--   0 fredrik    (501) staff       (20)     1061 2024-05-08 23:11:09.000000 minq-0.0.1/LICENSE
--rw-r--r--   0 fredrik    (501) staff       (20)     1942 2024-05-08 23:54:10.912474 minq-0.0.1/PKG-INFO
--rw-r--r--   0 fredrik    (501) staff       (20)      277 2024-05-08 23:12:45.000000 minq-0.0.1/README.md
-drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2024-05-08 23:54:10.911073 minq-0.0.1/minq/
--rw-r--r--   0 fredrik    (501) staff       (20)     1494 2024-05-08 23:49:40.000000 minq-0.0.1/minq/__init__.py
-drwxr-xr-x   0 fredrik    (501) staff       (20)        0 2024-05-08 23:54:10.912228 minq-0.0.1/minq.egg-info/
--rw-r--r--   0 fredrik    (501) staff       (20)     1942 2024-05-08 23:54:10.000000 minq-0.0.1/minq.egg-info/PKG-INFO
--rw-r--r--   0 fredrik    (501) staff       (20)      188 2024-05-08 23:54:10.000000 minq-0.0.1/minq.egg-info/SOURCES.txt
--rw-r--r--   0 fredrik    (501) staff       (20)        1 2024-05-08 23:54:10.000000 minq-0.0.1/minq.egg-info/dependency_links.txt
--rw-r--r--   0 fredrik    (501) staff       (20)       15 2024-05-08 23:54:10.000000 minq-0.0.1/minq.egg-info/requires.txt
--rw-r--r--   0 fredrik    (501) staff       (20)       21 2024-05-08 23:54:10.000000 minq-0.0.1/minq.egg-info/top_level.txt
--rw-r--r--   0 fredrik    (501) staff       (20)      615 2024-05-08 23:08:56.000000 minq-0.0.1/pyproject.toml
--rw-r--r--   0 fredrik    (501) staff       (20)       38 2024-05-08 23:54:10.912747 minq-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:06:57.283899 minq-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-09 00:06:53.000000 minq-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-09 00:06:57.283899 minq-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 00:06:53.000000 minq-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:06:57.279899 minq-0.0.2/minq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-09 00:06:53.000000 minq-0.0.2/minq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:06:57.283899 minq-0.0.2/minq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-09 00:06:57.000000 minq-0.0.2/minq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-09 00:06:57.000000 minq-0.0.2/minq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:06:57.000000 minq-0.0.2/minq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 00:06:57.000000 minq-0.0.2/minq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 00:06:57.000000 minq-0.0.2/minq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-09 00:06:53.000000 minq-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 00:06:57.283899 minq-0.0.2/setup.cfg
```

### Comparing `minq-0.0.1/LICENSE` & `minq-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `minq-0.0.1/PKG-INFO` & `minq-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minq
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tiny quantum gate library based on NumPy
 License: MIT License
         
         Copyright (c) 2024 fwcd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `minq-0.0.1/minq/__init__.py` & `minq-0.0.2/minq/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import reduce
-from numpy.typing import ArrayLike
-from typing import Iterable
+from numpy.typing import ArrayLike, NDArray
+from typing import cast
 
 import numpy as np
 
 I = np.identity(2)
 '''Identity transform'''
 
 X = np.array([
@@ -28,30 +28,28 @@
 def ket(*args: int | str):
     '''Creates a standard basis vector'''
     if len(args) == 0:
         return np.array([1])
     elif isinstance(args[0], int):
         assert all(b == 0 or b == 1 for b in args)
         x = np.zeros(2 ** len(args))
-        x[from_binary(args)] = 1
+        x[from_binary(*cast(tuple[int, ...], args))] = 1
         return x
-    elif isinstance(args[0], str):
+    else:
         assert len(args) == 1
         x = np.zeros(2 ** len(args[0]))
         x[int(args[0], base=2)] = 1
         return x
-    else:
-        raise TypeError('ket(...) takes either int or str')
 
-def kron(*arrays: ArrayLike) -> np.ndarray:
+def kron(*arrays: ArrayLike) -> NDArray:
     '''Computes the Kronecker product (tensor product) of the given arrays'''
     assert len(arrays) > 0
     return reduce(np.kron, arrays)
 
-def kronpow(array: ArrayLike, n: int) -> np.ndarray:
+def kronpow(array: ArrayLike, n: int) -> NDArray:
     '''Applies the Kronecker product n times'''
     assert n > 0
     return reduce(lambda acc, _: np.kron(acc, array), range(n - 1), array)
 
-def from_binary(bits: Iterable[int]) -> int:
+def from_binary(*bits: int) -> int:
     '''Converts a list of bits to the corresponding number when interpreted in base 2'''
     return 0 if len(bits) == 0 else int(''.join(map(str, bits)), base=2)
```

### Comparing `minq-0.0.1/minq.egg-info/PKG-INFO` & `minq-0.0.2/minq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minq
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tiny quantum gate library based on NumPy
 License: MIT License
         
         Copyright (c) 2024 fwcd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `minq-0.0.1/pyproject.toml` & `minq-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "minq"
-version = "0.0.1"
+version = "0.0.2"
 description = "Tiny quantum gate library based on NumPy"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 classifiers = ["Topic :: Scientific/Engineering :: Mathematics"]
 keywords = ["quantum", "computing", "circuit", "gate", "numpy"]
 dependencies = [
```

