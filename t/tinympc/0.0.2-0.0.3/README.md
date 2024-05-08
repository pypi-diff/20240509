# Comparing `tmp/tinympc-0.0.2.tar.gz` & `tmp/tinympc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinympc-0.0.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "tinympc-0.0.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `tinympc-0.0.2.tar` & `tinympc-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     3139 2022-11-09 12:37:21.000000 tinympc-0.0.2/.gitignore
--rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 tinympc-0.0.2/.gitmodules
--rw-r--r--   0        0        0      828 2022-11-09 12:37:21.000000 tinympc-0.0.2/CMakeLists.txt
--rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 tinympc-0.0.2/LICENSE
--rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 tinympc-0.0.2/README.md
--rw-r--r--   0        0        0      566 2022-11-09 12:37:21.000000 tinympc-0.0.2/examples/cartpole_example_code_generation.py
--rw-r--r--   0        0        0     1163 2022-11-09 12:37:21.000000 tinympc-0.0.2/examples/cartpole_example_mpc.py
--rw-r--r--   0        0        0     1333 2022-11-09 12:37:21.000000 tinympc-0.0.2/examples/cartpole_example_mpc_reference_constrained.py
--rw-r--r--   0        0        0      512 2022-11-09 12:37:21.000000 tinympc-0.0.2/examples/cartpole_example_one_solve.py
--rw-r--r--   0        0        0     1129 2022-11-09 12:37:21.000000 tinympc-0.0.2/examples/test_generated_code.py
--rw-r--r--   0        0        0      861 2022-11-09 12:37:21.000000 tinympc-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8434 2022-11-09 12:37:21.000000 tinympc-0.0.2/src/bindings.cpp
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 tinympc-0.0.2/src/tinympc/__init__.py
--rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 tinympc-0.0.2/src/tinympc/codegen/__init__.py
--rw-r--r--   0        0        0      888 2022-11-09 12:37:21.000000 tinympc-0.0.2/src/tinympc/codegen/pywrapper/CMakeLists.txt
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 tinympc-0.0.2/src/tinympc/codegen/pywrapper/__init__.py
--rw-r--r--   0        0        0     2430 2022-11-09 12:37:21.000000 tinympc-0.0.2/src/tinympc/codegen/pywrapper/bindings.cpp
--rw-r--r--   0        0        0     2110 2022-11-09 12:37:21.000000 tinympc-0.0.2/src/tinympc/codegen/pywrapper/setup.py
--rw-r--r--   0        0        0    10557 2022-11-09 12:37:21.000000 tinympc-0.0.2/src/tinympc/interface.py
--rw-r--r--   0        0        0      391 2022-11-09 12:37:21.000000 tinympc-0.0.2/tests/test_cache.py
--rw-r--r--   0        0        0      406 2022-11-09 12:37:21.000000 tinympc-0.0.2/tests/test_settings.py
--rw-r--r--   0        0        0     1976 2022-11-09 12:37:21.000000 tinympc-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3139 2022-11-09 12:37:21.000000 tinympc-0.0.3/.gitignore
+-rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 tinympc-0.0.3/.gitmodules
+-rw-r--r--   0        0        0      828 2022-11-09 12:37:21.000000 tinympc-0.0.3/CMakeLists.txt
+-rw-r--r--   0        0        0     1071 2022-11-09 12:37:21.000000 tinympc-0.0.3/LICENSE
+-rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 tinympc-0.0.3/README.md
+-rw-r--r--   0        0        0      519 2022-11-09 12:37:21.000000 tinympc-0.0.3/examples/cartpole_example_code_generation.py
+-rw-r--r--   0        0        0     1163 2022-11-09 12:37:21.000000 tinympc-0.0.3/examples/cartpole_example_mpc.py
+-rw-r--r--   0        0        0     1333 2022-11-09 12:37:21.000000 tinympc-0.0.3/examples/cartpole_example_mpc_reference_constrained.py
+-rw-r--r--   0        0        0      512 2022-11-09 12:37:21.000000 tinympc-0.0.3/examples/cartpole_example_one_solve.py
+-rw-r--r--   0        0        0     1129 2022-11-09 12:37:21.000000 tinympc-0.0.3/examples/test_generated_code.py
+-rw-r--r--   0        0        0      861 2022-11-09 12:37:21.000000 tinympc-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8434 2022-11-09 12:37:21.000000 tinympc-0.0.3/src/bindings.cpp
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 tinympc-0.0.3/src/tinympc/__init__.py
+-rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 tinympc-0.0.3/src/tinympc/codegen/__init__.py
+-rw-r--r--   0        0        0      888 2022-11-09 12:37:21.000000 tinympc-0.0.3/src/tinympc/codegen/pywrapper/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 tinympc-0.0.3/src/tinympc/codegen/pywrapper/__init__.py
+-rw-r--r--   0        0        0     2430 2022-11-09 12:37:21.000000 tinympc-0.0.3/src/tinympc/codegen/pywrapper/bindings.cpp
+-rw-r--r--   0        0        0     2110 2022-11-09 12:37:21.000000 tinympc-0.0.3/src/tinympc/codegen/pywrapper/setup.py
+-rw-r--r--   0        0        0    10557 2022-11-09 12:37:21.000000 tinympc-0.0.3/src/tinympc/interface.py
+-rw-r--r--   0        0        0      391 2022-11-09 12:37:21.000000 tinympc-0.0.3/tests/test_cache.py
+-rw-r--r--   0        0        0      406 2022-11-09 12:37:21.000000 tinympc-0.0.3/tests/test_settings.py
+-rw-r--r--   0        0        0     1976 2022-11-09 12:37:21.000000 tinympc-0.0.3/PKG-INFO
```

### Comparing `tinympc-0.0.2/.gitignore` & `tinympc-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tinympc-0.0.2/CMakeLists.txt` & `tinympc-0.0.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tinympc-0.0.2/LICENSE` & `tinympc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tinympc-0.0.2/examples/cartpole_example_code_generation.py` & `tinympc-0.0.3/examples/cartpole_example_code_generation.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,11 +16,8 @@
 
 prob = tinympc.TinyMPC()
 
 u_min = np.array([-0.5])
 u_max = np.array([0.5])
 prob.setup(A, B, Q, R, N, rho=1, max_iter=10, u_min=u_min, u_max=u_max)
 
-x0 = np.array([0.5, 0, 0, 0])
-prob.set_x0(x0)
-
 prob.codegen("out", verbose=1)
```

### Comparing `tinympc-0.0.2/examples/cartpole_example_mpc.py` & `tinympc-0.0.3/examples/cartpole_example_mpc.py`

 * *Files identical despite different names*

### Comparing `tinympc-0.0.2/examples/cartpole_example_mpc_reference_constrained.py` & `tinympc-0.0.3/examples/cartpole_example_mpc_reference_constrained.py`

 * *Files identical despite different names*

### Comparing `tinympc-0.0.2/examples/cartpole_example_one_solve.py` & `tinympc-0.0.3/examples/cartpole_example_one_solve.py`

 * *Files identical despite different names*

### Comparing `tinympc-0.0.2/examples/test_generated_code.py` & `tinympc-0.0.3/examples/test_generated_code.py`

 * *Files identical despite different names*

### Comparing `tinympc-0.0.2/pyproject.toml` & `tinympc-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "tinympc"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Sam Schoedel", email="seschoedel@gmail.com" },
   { name="Khai Nguyen", email="khai.nx1201@gmail.com" },
 ]
 description = "Python wrapper for TinyMPC"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `tinympc-0.0.2/src/bindings.cpp` & `tinympc-0.0.3/src/bindings.cpp`

 * *Files identical despite different names*

### Comparing `tinympc-0.0.2/src/tinympc/codegen/pywrapper/CMakeLists.txt` & `tinympc-0.0.3/src/tinympc/codegen/pywrapper/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tinympc-0.0.2/src/tinympc/codegen/pywrapper/bindings.cpp` & `tinympc-0.0.3/src/tinympc/codegen/pywrapper/bindings.cpp`

 * *Files identical despite different names*

### Comparing `tinympc-0.0.2/src/tinympc/codegen/pywrapper/setup.py` & `tinympc-0.0.3/src/tinympc/codegen/pywrapper/setup.py`

 * *Files identical despite different names*

### Comparing `tinympc-0.0.2/src/tinympc/interface.py` & `tinympc-0.0.3/src/tinympc/interface.py`

 * *Files identical despite different names*

### Comparing `tinympc-0.0.2/PKG-INFO` & `tinympc-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinympc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper for TinyMPC
 Author-Email: Sam Schoedel <seschoedel@gmail.com>, Khai Nguyen <khai.nx1201@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Khai Nguyen]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

