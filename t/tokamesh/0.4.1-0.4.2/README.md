# Comparing `tmp/tokamesh-0.4.1.tar.gz` & `tmp/tokamesh-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokamesh-0.4.1.tar", last modified: Sat Nov 18 12:55:29 2023, max compression
+gzip compressed data, was "tokamesh-0.4.2.tar", last modified: Thu May  9 08:08:10 2024, max compression
```

## Comparing `tokamesh-0.4.1.tar` & `tokamesh-0.4.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:55:29.464849 tokamesh-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:55:29.452849 tokamesh-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:55:29.456849 tokamesh-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-11-18 12:55:11.000000 tokamesh-0.4.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-18 12:55:11.000000 tokamesh-0.4.1/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-11-18 12:55:11.000000 tokamesh-0.4.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2023-11-18 12:55:11.000000 tokamesh-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      544 2023-11-18 12:55:11.000000 tokamesh-0.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-11-18 12:55:11.000000 tokamesh-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2023-11-18 12:55:29.464849 tokamesh-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-11-18 12:55:11.000000 tokamesh-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:55:29.456849 tokamesh-0.4.1/demos/
--rw-r--r--   0 runner    (1001) docker     (127)   139442 2023-11-18 12:55:11.000000 tokamesh-0.4.1/demos/geometry_matrix_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   472564 2023-11-18 12:55:11.000000 tokamesh-0.4.1/demos/mesh_construction_demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:55:29.456849 tokamesh-0.4.1/demos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2023-11-18 12:55:11.000000 tokamesh-0.4.1/demos/scripts/geometry_matrix_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2023-11-18 12:55:11.000000 tokamesh-0.4.1/demos/scripts/geometry_matrix_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:55:29.456849 tokamesh-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-18 12:55:11.000000 tokamesh-0.4.1/docs/docs_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:55:29.456849 tokamesh-0.4.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-11-18 12:55:11.000000 tokamesh-0.4.1/docs/source/TriangularMesh.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2023-11-18 12:55:11.000000 tokamesh-0.4.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-18 12:55:11.000000 tokamesh-0.4.1/docs/source/construction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-11-18 12:55:11.000000 tokamesh-0.4.1/docs/source/construction_refinement.rst
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-11-18 12:55:11.000000 tokamesh-0.4.1/docs/source/geometry.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2023-11-18 12:55:11.000000 tokamesh-0.4.1/docs/source/geometry_background.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-11-18 12:55:11.000000 tokamesh-0.4.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-11-18 12:55:11.000000 tokamesh-0.4.1/docs/source/operators.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-11-18 12:55:11.000000 tokamesh-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-18 12:55:29.464849 tokamesh-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-18 12:55:11.000000 tokamesh-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:55:29.460849 tokamesh-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tests/test_TriangularMesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12464 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tests/test_construction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tests/test_intersection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tests/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:55:29.460849 tokamesh-0.4.1/tokamesh/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tokamesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-18 12:55:29.000000 tokamesh-0.4.1/tokamesh/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    26881 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tokamesh/construction.py
--rw-r--r--   0 runner    (1001) docker     (127)    23258 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tokamesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tokamesh/intersection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20399 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tokamesh/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tokamesh/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:55:29.460849 tokamesh-0.4.1/tokamesh/tokamaks/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tokamesh/tokamaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tokamesh/tokamaks/mastu_boundary_data.npz
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2023-11-18 12:55:11.000000 tokamesh-0.4.1/tokamesh/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:55:29.460849 tokamesh-0.4.1/tokamesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2023-11-18 12:55:29.000000 tokamesh-0.4.1/tokamesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-11-18 12:55:29.000000 tokamesh-0.4.1/tokamesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 12:55:29.000000 tokamesh-0.4.1/tokamesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-11-18 12:55:29.000000 tokamesh-0.4.1/tokamesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-18 12:55:29.000000 tokamesh-0.4.1/tokamesh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.678048 tokamesh-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.666047 tokamesh-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.670047 tokamesh-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-09 08:07:59.000000 tokamesh-0.4.2/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-09 08:07:59.000000 tokamesh-0.4.2/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-09 08:07:59.000000 tokamesh-0.4.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-09 08:07:59.000000 tokamesh-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 08:07:59.000000 tokamesh-0.4.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-09 08:07:59.000000 tokamesh-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-09 08:08:10.678048 tokamesh-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-09 08:07:59.000000 tokamesh-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.670047 tokamesh-0.4.2/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)   139442 2024-05-09 08:07:59.000000 tokamesh-0.4.2/demos/geometry_matrix_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   472564 2024-05-09 08:07:59.000000 tokamesh-0.4.2/demos/mesh_construction_demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.670047 tokamesh-0.4.2/demos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-09 08:07:59.000000 tokamesh-0.4.2/demos/scripts/geometry_matrix_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-09 08:07:59.000000 tokamesh-0.4.2/demos/scripts/geometry_matrix_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.670047 tokamesh-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/docs_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.674048 tokamesh-0.4.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/TriangularMesh.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/construction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/construction_refinement.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/geometry_background.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/operators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-09 08:07:59.000000 tokamesh-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:08:10.678048 tokamesh-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:07:59.000000 tokamesh-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.674048 tokamesh-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tests/test_TriangularMesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tests/test_construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tests/test_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tests/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.674048 tokamesh-0.4.2/tokamesh/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 08:08:10.000000 tokamesh-0.4.2/tokamesh/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26881 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23700 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20399 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.678048 tokamesh-0.4.2/tokamesh/tokamaks/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/tokamaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/tokamaks/mastu_boundary_data.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.678048 tokamesh-0.4.2/tokamesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-09 08:08:10.000000 tokamesh-0.4.2/tokamesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-09 08:08:10.000000 tokamesh-0.4.2/tokamesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:08:10.000000 tokamesh-0.4.2/tokamesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 08:08:10.000000 tokamesh-0.4.2/tokamesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 08:08:10.000000 tokamesh-0.4.2/tokamesh.egg-info/top_level.txt
```

### Comparing `tokamesh-0.4.1/.github/workflows/black.yml` & `tokamesh-0.4.2/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/.github/workflows/python_publish.yml` & `tokamesh-0.4.2/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/.github/workflows/tests.yml` & `tokamesh-0.4.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/.gitignore` & `tokamesh-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/.readthedocs.yaml` & `tokamesh-0.4.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/LICENSE` & `tokamesh-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/PKG-INFO` & `tokamesh-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokamesh
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python tools for constructing meshes and geometry matrices used in tomography problems
 Author-email: Chris Bowman <chris.bowman.physics@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Chris Bowman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tokamesh-0.4.1/README.md` & `tokamesh-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/demos/geometry_matrix_demo.ipynb` & `tokamesh-0.4.2/demos/geometry_matrix_demo.ipynb`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/demos/mesh_construction_demo.ipynb` & `tokamesh-0.4.2/demos/mesh_construction_demo.ipynb`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/demos/scripts/geometry_matrix_benchmark.py` & `tokamesh-0.4.2/demos/scripts/geometry_matrix_benchmark.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/demos/scripts/geometry_matrix_demo.py` & `tokamesh-0.4.2/demos/scripts/geometry_matrix_demo.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/docs/source/conf.py` & `tokamesh-0.4.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/docs/source/geometry_background.rst` & `tokamesh-0.4.2/docs/source/geometry_background.rst`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/docs/source/index.rst` & `tokamesh-0.4.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/pyproject.toml` & `tokamesh-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/tests/test_TriangularMesh.py` & `tokamesh-0.4.2/tests/test_TriangularMesh.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/tests/test_construction.py` & `tokamesh-0.4.2/tests/test_construction.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/tests/test_geometry.py` & `tokamesh-0.4.2/tests/test_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from tokamesh.geometry import radius_hyperbolic_integral
 from tokamesh.utilities import build_edge_map, Camera
 
 
 def test_BarycentricGeometryMatrix():
     # build a basic mesh out of equilateral triangles
     R, z, triangles = equilateral_mesh(
-        resolution=0.01, R_range=[0, 0.2], z_range=[0, 0.2]
+        resolution=0.01, R_range=[0, 0.2], z_range=[-0.2, 0.2]
     )
     mesh = TriangularMesh(R, z, triangles)
 
     # generate a random test field using a gaussian process
     distance = sqrt((R[:, None] - R[None, :]) ** 2 + (z[:, None] - z[None, :]) ** 2)
     scale = 0.04
     covariance = sinc(distance / scale) ** 2
@@ -47,18 +47,18 @@
     entry_values = matrix_data["entry_values"]
     row_values = matrix_data["row_indices"]
     col_values = matrix_data["col_indices"]
     shape = matrix_data["shape"]
     G = csc_matrix((entry_values, (row_values, col_values)), shape=shape)
 
     # get the geometry matrix prediction of the line-integrals
-    matrix_integrals = G.dot(field)
+    matrix_integrals = G @ field
 
     # manually calculate the line integrals for comparison
-    L = linspace(0, 0.5, 3000)  # build a distance axis for the integrals
+    L = linspace(0, 1.0, 3000)  # build a distance axis for the integrals
     # get the position of each ray at each distance
     R_projection, z_projection = cam.project_rays(L)
     # directly integrate along each ray
     direct_integrals = zeros(R_projection.shape[1])
     for i in range(R_projection.shape[1]):
         samples = mesh.interpolate(
             R_projection[:, i], z_projection[:, i], vertex_values=field
```

### Comparing `tokamesh-0.4.1/tests/test_intersection.py` & `tokamesh-0.4.2/tests/test_intersection.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/tests/test_operators.py` & `tokamesh-0.4.2/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/tokamesh/construction.py` & `tokamesh-0.4.2/tokamesh/construction.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/tokamesh/geometry.py` & `tokamesh-0.4.2/tokamesh/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,21 @@
         )
         self.lam2_coeffs = (
             0.5
             * stack([z3 - z1, R1 - R3, R3 * z1 - R1 * z3], axis=1)
             / self.area[:, None]
         )
 
+        # for edges in the mesh which are very close to horizontal, the regular
+        # intersection calculation becomes inaccurate. Here we set a lower-limit
+        # on the allowed size of the z-component of the edge unit vector. Edges
+        # with a z-component below this limit will instead use a different
+        # intersection calculation for horizontal edges.
+        self.min_z_component = 1e-12
+
     def calculate(self, save_file=None) -> dict:
         """
         Calculate the geometry matrix.
 
         :keyword str save_file: \
             A string specifying a file path to which the geometry matrix data will be
             saved using the numpy ``.npz`` format. If not specified, the geometry matrix
@@ -253,15 +260,17 @@
         # loop over each triangle edge and check for intersections
         edges = self.triangle_edges[tri_index, :]
         for j, edge in enumerate(edges):
             R0 = self.R_edge_mid[edge]
             z0 = self.z_edge_mid[edge]
             uR, uz = self.edge_drn[edge, :]
             w = self.edge_lengths[edge]
-            if uz == 0.0:  # if the edge is horizontal, a simplified method can be used
+
+            # if the edge is horizontal, a simplified method can be used
+            if abs(uz) < self.min_z_component:
                 intersections[:, 2 * j] = self.horizontal_hyperbola_intersections(
                     R0, z0, uR, uz, w
                 )
                 intersections[:, 2 * j + 1] = nan
             else:  # else we need the general intersection calculation
                 intersections[:, 2 * j : 2 * j + 2] = self.edge_hyperbola_intersections(
                     R0, z0, uR, uz, w
@@ -282,19 +291,17 @@
         for j in range(3):
             equal = intersections[:, 2 * j] == intersections[:, 2 * j + 1]
             if equal.any():  # discard any pairs with equal distance values
                 intersections[equal, 2 * j : 2 * j + 2] = nan
 
         # re-sort the intersections
         intersections.sort(axis=1)
-
         # check where valid intersections exist, and count how many there are per ray
         valid_intersections = isfinite(intersections)
         intersection_count = valid_intersections.sum(axis=1)
-
         # At this point, each ray should have an even number of intersections, if any
         # have an odd number then something has gone wrong, so raise an error.
         if (intersection_count % 2 == 1).any():
             raise ValueError(
                 f"""\n\n
                 \r[ BarycentricGeometryMatrix error ]
                 \r>> One or more rays has an odd number of intersections with
```

### Comparing `tokamesh-0.4.1/tokamesh/intersection.py` & `tokamesh-0.4.2/tokamesh/intersection.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/tokamesh/mesh.py` & `tokamesh-0.4.2/tokamesh/mesh.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/tokamesh/operators.py` & `tokamesh-0.4.2/tokamesh/operators.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/tokamesh/tokamaks/__init__.py` & `tokamesh-0.4.2/tokamesh/tokamaks/__init__.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/tokamesh/tokamaks/mastu_boundary_data.npz` & `tokamesh-0.4.2/tokamesh/tokamaks/mastu_boundary_data.npz`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/tokamesh/utilities.py` & `tokamesh-0.4.2/tokamesh/utilities.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.1/tokamesh.egg-info/PKG-INFO` & `tokamesh-0.4.2/tokamesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokamesh
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python tools for constructing meshes and geometry matrices used in tomography problems
 Author-email: Chris Bowman <chris.bowman.physics@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Chris Bowman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tokamesh-0.4.1/tokamesh.egg-info/SOURCES.txt` & `tokamesh-0.4.2/tokamesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

