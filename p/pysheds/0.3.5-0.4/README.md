# Comparing `tmp/pysheds-0.3.5.tar.gz` & `tmp/pysheds-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysheds-0.3.5.tar", last modified: Tue May 16 20:26:09 2023, max compression
+gzip compressed data, was "pysheds-0.4.tar", last modified: Thu May  9 18:16:58 2024, max compression
```

## Comparing `pysheds-0.3.5.tar` & `pysheds-0.4.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:26:09.151716 pysheds-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-16 20:25:58.000000 pysheds-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 20:25:58.000000 pysheds-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 20:26:09.151716 pysheds-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-05-16 20:25:58.000000 pysheds-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:26:09.151716 pysheds-0.3.5/pysheds/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71744 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/_sgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/_sview.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/io.py
--rw-r--r--   0 runner    (1001) docker     (123)   169233 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/pgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/pview.py
--rw-r--r--   0 runner    (1001) docker     (123)    24804 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/rfsm.py
--rw-r--r--   0 runner    (1001) docker     (123)   115201 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/sgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    39016 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/sview.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:26:09.151716 pysheds-0.3.5/pysheds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 20:26:09.000000 pysheds-0.3.5/pysheds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-16 20:26:09.000000 pysheds-0.3.5/pysheds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:26:09.000000 pysheds-0.3.5/pysheds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-16 20:26:09.000000 pysheds-0.3.5/pysheds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 20:26:09.000000 pysheds-0.3.5/pysheds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 20:26:09.151716 pysheds-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-16 20:25:58.000000 pysheds-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:26:09.151716 pysheds-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-16 20:25:58.000000 pysheds-0.3.5/tests/test_grid.py
+drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2024-05-09 18:16:58.333433 pysheds-0.4/
+-rw-r--r--   0 mdbartos   (501) staff       (20)    35141 2024-05-09 18:16:34.000000 pysheds-0.4/LICENSE
+-rw-r--r--   0 mdbartos   (501) staff       (20)       34 2024-05-09 18:16:34.000000 pysheds-0.4/MANIFEST.in
+-rw-r--r--   0 mdbartos   (501) staff       (20)     1212 2024-05-09 18:16:58.333133 pysheds-0.4/PKG-INFO
+-rw-r--r--   0 mdbartos   (501) staff       (20)    16904 2024-05-09 18:16:34.000000 pysheds-0.4/README.md
+drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2024-05-09 18:16:58.331518 pysheds-0.4/pysheds/
+-rw-r--r--   0 mdbartos   (501) staff       (20)       20 2024-05-09 18:16:34.000000 pysheds-0.4/pysheds/__init__.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)    76845 2024-05-09 18:16:34.000000 pysheds-0.4/pysheds/_sgrid.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)     5453 2024-05-09 18:16:34.000000 pysheds-0.4/pysheds/_sview.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)      231 2024-05-09 18:16:34.000000 pysheds-0.4/pysheds/grid.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)    12488 2024-05-09 18:16:34.000000 pysheds-0.4/pysheds/io.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)   169228 2024-05-09 18:16:34.000000 pysheds-0.4/pysheds/pgrid.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)     3609 2024-05-09 18:16:34.000000 pysheds-0.4/pysheds/projection.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)    14881 2024-05-09 18:16:34.000000 pysheds-0.4/pysheds/pview.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)    24804 2024-05-09 18:16:34.000000 pysheds-0.4/pysheds/rfsm.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)   114667 2024-05-09 18:16:34.000000 pysheds-0.4/pysheds/sgrid.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)    39024 2024-05-09 18:16:34.000000 pysheds-0.4/pysheds/sview.py
+-rw-r--r--   0 mdbartos   (501) staff       (20)      333 2024-05-09 18:16:34.000000 pysheds-0.4/pysheds/view.py
+drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2024-05-09 18:16:58.332347 pysheds-0.4/pysheds.egg-info/
+-rw-r--r--   0 mdbartos   (501) staff       (20)     1212 2024-05-09 18:16:58.000000 pysheds-0.4/pysheds.egg-info/PKG-INFO
+-rw-r--r--   0 mdbartos   (501) staff       (20)      400 2024-05-09 18:16:58.000000 pysheds-0.4/pysheds.egg-info/SOURCES.txt
+-rw-r--r--   0 mdbartos   (501) staff       (20)        1 2024-05-09 18:16:58.000000 pysheds-0.4/pysheds.egg-info/dependency_links.txt
+-rw-r--r--   0 mdbartos   (501) staff       (20)      158 2024-05-09 18:16:58.000000 pysheds-0.4/pysheds.egg-info/requires.txt
+-rw-r--r--   0 mdbartos   (501) staff       (20)        8 2024-05-09 18:16:58.000000 pysheds-0.4/pysheds.egg-info/top_level.txt
+-rw-r--r--   0 mdbartos   (501) staff       (20)       38 2024-05-09 18:16:58.333502 pysheds-0.4/setup.cfg
+-rw-r--r--   0 mdbartos   (501) staff       (20)     1645 2024-05-09 18:16:34.000000 pysheds-0.4/setup.py
```

### Comparing `pysheds-0.3.5/LICENSE` & `pysheds-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysheds-0.3.5/PKG-INFO` & `pysheds-0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: pysheds
-Version: 0.3.5
+Version: 0.4
 Summary: 🌎 Simple and fast watershed delineation in python.
 Home-page: http://open-storm.org
 Author: Matt Bartos
 Author-email: mdbartos@umich.edu
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: recipes
 License-File: LICENSE
 
 🌎 Simple and fast watershed delineation in python.
+
```

### Comparing `pysheds-0.3.5/README.md` & `pysheds-0.4/README.md`

 * *Files identical despite different names*

### Comparing `pysheds-0.3.5/pysheds/_sgrid.py` & `pysheds-0.4/pysheds/_sgrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,44 @@
-from heapq import heappop, heappush
+from heapq import heappop, heappush, heapify
+import math
 import numpy as np
-from numba import njit, prange
+from functools import wraps
+from numba import njit, prange, from_dtype
 from numba.types import float64, int64, uint32, uint16, uint8, boolean, UniTuple, Tuple, List, DictType, void
+from numba.typed import typedlist
 
 # Functions for 'flowdir'
 
 @njit(int64[:,:](float64[:,:], float64, float64, UniTuple(int64, 8), boolean[:,:],
                  int64, int64, int64),
       parallel=True,
       cache=True)
 def _d8_flowdir_numba(dem, dx, dy, dirmap, nodata_cells, nodata_out, flat=-1, pit=-2):
-    fdir = np.zeros(dem.shape, dtype=np.int64)
+    fdir = np.full(dem.shape, nodata_out, dtype=np.int64)
     m, n = dem.shape
-    dd = np.sqrt(dx**2 + dy**2)
+    dd = math.sqrt(dx**2 + dy**2)
     row_offsets = np.array([-1, -1, 0, 1, 1, 1, 0, -1])
     col_offsets = np.array([0, 1, 1, 1, 0, -1, -1, -1])
     distances = np.array([dy, dd, dx, dd, dy, dd, dx, dd])
-    for i in prange(1, m - 1):
-        for j in prange(1, n - 1):
-            if nodata_cells[i, j]:
-                fdir[i, j] = nodata_out
-            else:
+    for i in prange(m):
+        for j in prange(n):
+            if not nodata_cells[i, j]:
                 elev = dem[i, j]
                 max_slope = -np.inf
                 for k in range(8):
-                    row_offset = row_offsets[k]
-                    col_offset = col_offsets[k]
+                    row = i + row_offsets[k]
+                    col = j + col_offsets[k]
+                    if row < 0 or row >= m or col < 0 or col >= n:
+                        # out of bounds, skip
+                        continue
+                    elif nodata_cells[row, col]:
+                        # this neighbor is nodata, skip
+                        continue
                     distance = distances[k]
-                    slope = (elev - dem[i + row_offset, j + col_offset]) / distance
+                    slope = (elev - dem[row, col]) / distance
                     if slope > max_slope:
                         fdir[i, j] = dirmap[k]
                         max_slope = slope
                 if max_slope == 0:
                     fdir[i, j] = flat
                 elif max_slope < 0:
                     fdir[i, j] = pit
@@ -39,34 +46,38 @@
 
 @njit(int64[:,:](float64[:,:], float64[:,:], float64[:,:], UniTuple(int64, 8), boolean[:,:],
                  int64, int64, int64),
       parallel=True,
       cache=True)
 def _d8_flowdir_irregular_numba(dem, x_arr, y_arr, dirmap, nodata_cells,
                                 nodata_out, flat=-1, pit=-2):
-    fdir = np.zeros(dem.shape, dtype=np.int64)
+    fdir = np.full(dem.shape, nodata_out, dtype=np.int64)
     m, n = dem.shape
     row_offsets = np.array([-1, -1, 0, 1, 1, 1, 0, -1])
     col_offsets = np.array([0, 1, 1, 1, 0, -1, -1, -1])
-    for i in prange(1, m - 1):
-        for j in prange(1, n - 1):
-            if nodata_cells[i, j]:
-                fdir[i, j] = nodata_out
-            else:
+    for i in prange(m):
+        for j in prange(n):
+            if not nodata_cells[i, j]:
                 elev = dem[i, j]
                 x_center = x_arr[i, j]
                 y_center = y_arr[i, j]
                 max_slope = -np.inf
                 for k in range(8):
-                    row_offset = row_offsets[k]
-                    col_offset = col_offsets[k]
-                    dh = elev - dem[i + row_offset, j + col_offset]
-                    dx = np.abs(x_center - x_arr[i + row_offset, j + col_offset])
-                    dy = np.abs(y_center - y_arr[i + row_offset, j + col_offset])
-                    distance = np.sqrt(dx**2 + dy**2)
+                    row = i + row_offsets[k]
+                    col = j + col_offsets[k]
+                    if row < 0 or row >= m or col < 0 or col >= n:
+                        # out of bounds, skip
+                        continue
+                    elif nodata_cells[row, col]:
+                        # this neighbor is nodata, skip
+                        continue
+                    dh = elev - dem[row, col]
+                    dx = abs(x_center - x_arr[row, col])
+                    dy = abs(y_center - y_arr[row, col])
+                    distance = math.sqrt(dx**2 + dy**2)
                     slope = dh / distance
                     if slope > max_slope:
                         fdir[i, j] = dirmap[k]
                         max_slope = slope
                 if max_slope == 0:
                     fdir[i, j] = flat
                 elif max_slope < 0:
@@ -74,18 +85,18 @@
     return fdir
 
 @njit(UniTuple(float64, 2)(float64, float64, float64, float64, float64),
       cache=True)
 def _facet_flow(e0, e1, e2, d1=1., d2=1.):
     s1 = (e0 - e1) / d1
     s2 = (e1 - e2) / d2
-    r = np.arctan2(s2, s1)
-    s = np.hypot(s1, s2)
-    diag_angle    = np.arctan2(d2, d1)
-    diag_distance = np.hypot(d1, d2)
+    r = math.atan2(s2, s1)
+    s = math.hypot(s1, s2)
+    diag_angle = math.atan2(d2, d1)
+    diag_distance = math.hypot(d1, d2)
     b0 = (r < 0)
     b1 = (r > diag_angle)
     if b0:
         r = 0
         s = s1
     if b1:
         r = diag_angle
@@ -100,15 +111,15 @@
     e1s = np.array([0, 2, 2, 4, 4, 6, 6, 0])
     e2s = np.array([1, 1, 3, 3, 5, 5, 7, 7])
     d1s = np.array([0, 2, 2, 4, 4, 6, 6, 0])
     d2s = np.array([2, 0, 4, 2, 6, 4, 0, 6])
     ac = np.array([0, 1, 1, 2, 2, 3, 3, 4])
     af = np.array([1, -1, 1, -1, 1, -1, 1, -1])
     angle = np.full(dem.shape, nodata, dtype=np.float64)
-    diag_dist = np.sqrt(x_dist**2 + y_dist**2)
+    diag_dist = math.sqrt(x_dist**2 + y_dist**2)
     cell_dists = np.array([x_dist, diag_dist, y_dist, diag_dist,
                            x_dist, diag_dist, y_dist, diag_dist])
     row_offsets = np.array([0, -1, -1, -1, 0, 1, 1, 1])
     col_offsets = np.array([1, 1, 0, -1, -1, -1, 0, 1])
     for i in prange(1, m - 1):
         for j in prange(1, n - 1):
             e0 = dem[i, j]
@@ -174,16 +185,16 @@
                 col_offset_2 = col_offsets[edge_2]
                 e1 = dem[i + row_offset_1, j + col_offset_1]
                 e2 = dem[i + row_offset_2, j + col_offset_2]
                 x1 = x_arr[i + row_offset_1, j + col_offset_1]
                 x2 = x_arr[i + row_offset_2, j + col_offset_2]
                 y1 = y_arr[i + row_offset_1, j + col_offset_1]
                 y2 = y_arr[i + row_offset_2, j + col_offset_2]
-                d1 = np.sqrt(x1**2 + y1**2)
-                d2 = np.sqrt(x2**2 + y2**2)
+                d1 = math.sqrt(x1**2 + y1**2)
+                d2 = math.sqrt(x2**2 + y2**2)
                 r, s = _facet_flow(e0, e1, e2, d1, d2)
                 if s > s_max:
                     s_max = s
                     k_max = k
                     r_max = r
             if s_max < 0:
                 angle[i, j] = pit
@@ -254,31 +265,35 @@
     return fdirs_0, fdirs_1, props_0, props_1
 
 @njit(float64[:,:,:](float64[:,:], float64, float64, boolean[:,:], float64, int64),
       parallel=True,
       cache=True)
 def _mfd_flowdir_numba(dem, dx, dy, nodata_cells, nodata_out, p=1):
     m, n = dem.shape
-    fdir = np.zeros((8, m, n), dtype=np.float64)
+    fdir = np.full((8, m, n), nodata_out, dtype=np.float64)
     row_offsets = np.array([-1, -1, 0, 1, 1, 1, 0, -1])
     col_offsets = np.array([0, 1, 1, 1, 0, -1, -1, -1])
-    dd = np.sqrt(dx**2 + dy**2)
+    dd = math.sqrt(dx**2 + dy**2)
     distances = np.array([dy, dd, dx, dd, dy, dd, dx, dd])
-    for i in prange(1, m - 1):
-        for j in prange(1, n - 1):
-            if nodata_cells[i, j]:
-                fdir[:, i, j] = nodata_out
-            else:
+    for i in prange(m):
+        for j in prange(n):
+            if not nodata_cells[i, j]:
                 elev = dem[i, j]
                 den = 0.
                 for k in range(8):
-                    row_offset = row_offsets[k]
-                    col_offset = col_offsets[k]
+                    row = i + row_offsets[k]
+                    col = j + col_offsets[k]
+                    if row < 0 or row >= m or col < 0 or col >= n:
+                        # out of bounds, skip
+                        continue
+                    elif nodata_cells[row, col]:
+                        # this neighbor is nodata, skip
+                        continue
                     distance = distances[k]
-                    num = (elev - dem[i + row_offset, j + col_offset])**p / distance
+                    num = (elev - dem[row, col])**p / distance
                     if num > 0:
                         fdir[k, i, j] = num
                         den += num
                 if den > 0:
                     fdir[:, i, j] /= den
     return fdir
 
@@ -296,29 +311,29 @@
             points_to = (fdir.flat[neighbor] == r_dirmap[k])
             if points_to:
                 _d8_catchment_recursion(neighbor, catch, fdir, offsets, r_dirmap)
 
 @njit(boolean[:,:](int64[:,:], UniTuple(int64, 2), UniTuple(int64, 8)),
       cache=True)
 def _d8_catchment_recur_numba(fdir, pour_point, dirmap):
-    catch = np.zeros(fdir.shape, dtype=np.bool8)
+    catch = np.zeros(fdir.shape, dtype=np.bool_)
     offset = fdir.shape[1]
     i, j = pour_point
     ix = (i * offset) + j
     offsets = np.array([-offset, 1 - offset, 1, 1 + offset,
                         offset, - 1 + offset, - 1, - 1 - offset])
     r_dirmap = np.array([dirmap[4], dirmap[5], dirmap[6],
                          dirmap[7], dirmap[0], dirmap[1],
                          dirmap[2], dirmap[3]])
     _d8_catchment_recursion(ix, catch, fdir, offsets, r_dirmap)
     return catch
 
 @njit(boolean[:,:](int64[:,:], UniTuple(int64, 2), UniTuple(int64, 8)))
 def _d8_catchment_iter_numba(fdir, pour_point, dirmap):
-    catch = np.zeros(fdir.shape, dtype=np.bool8)
+    catch = np.zeros(fdir.shape, dtype=np.bool_)
     offset = fdir.shape[1]
     i, j = pour_point
     ix = (i * offset) + j
     offsets = np.array([-offset, 1 - offset, 1, 1 + offset,
                         offset, - 1 + offset, - 1, - 1 - offset])
     r_dirmap = np.array([dirmap[4], dirmap[5], dirmap[6],
                          dirmap[7], dirmap[0], dirmap[1],
@@ -353,15 +368,15 @@
             points_to = points_to_0 or points_to_1
             if points_to:
                 _dinf_catchment_recursion(neighbor, catch, fdir_0, fdir_1, offsets, r_dirmap)
 
 @njit(boolean[:,:](int64[:,:], int64[:,:], UniTuple(int64, 2), UniTuple(int64, 8)),
       cache=True)
 def _dinf_catchment_recur_numba(fdir_0, fdir_1, pour_point, dirmap):
-    catch = np.zeros(fdir_0.shape, dtype=np.bool8)
+    catch = np.zeros(fdir_0.shape, dtype=np.bool_)
     dirmap = np.array(dirmap)
     offset = fdir_0.shape[1]
     i, j = pour_point
     ix = (i * offset) + j
     offsets = np.array([-offset, 1 - offset, 1,
                         1 + offset, offset, - 1 + offset,
                         - 1, - 1 - offset])
@@ -370,15 +385,15 @@
                          dirmap[2], dirmap[3]])
     _dinf_catchment_recursion(ix, catch, fdir_0, fdir_1, offsets, r_dirmap)
     return catch
 
 @njit(boolean[:,:](int64[:,:], int64[:,:], UniTuple(int64, 2), UniTuple(int64, 8)),
       cache=True)
 def _dinf_catchment_iter_numba(fdir_0, fdir_1, pour_point, dirmap):
-    catch = np.zeros(fdir_0.shape, dtype=np.bool8)
+    catch = np.zeros(fdir_0.shape, dtype=np.bool_)
     dirmap = np.array(dirmap)
     offset = fdir_0.shape[1]
     i, j = pour_point
     ix = (i * offset) + j
     offsets = np.array([-offset, 1 - offset, 1,
                         1 + offset, offset, - 1 + offset,
                         - 1, - 1 - offset])
@@ -404,15 +419,15 @@
     return catch
 
 @njit(boolean[:,:](float64[:,:,:], UniTuple(int64, 2)),
       cache=True)
 def _mfd_catchment_iter_numba(fdir, pour_point):
     _, m, n = fdir.shape
     mn = m * n
-    catch = np.zeros((m, n), dtype=np.bool8)
+    catch = np.zeros((m, n), dtype=np.bool_)
     i, j = pour_point
     ix = (i * n) + j
     offsets = np.array([-n, 1 - n, 1,
                         1 + n, n, - 1 + n,
                         - 1, - 1 - n])
     r_dirmap = np.array([4, 5, 6, 7,
                          0, 1, 2, 3])
@@ -525,15 +540,15 @@
 
 @njit(float64[:,:](float64[:,:], int64[:,:], int64[:,:], uint8[:], int64[:],
                    float64[:,:], float64[:,:]),
       cache=True)
 def _dinf_accumulation_recur_numba(acc, fdir_0, fdir_1, indegree, startnodes,
                                    props_0, props_1):
     n = startnodes.size
-    visited = np.zeros(acc.shape, dtype=np.bool8)
+    visited = np.zeros(acc.shape, dtype=np.bool_)
     for k in range(n):
         startnode = startnodes.flat[k]
         endnode_0 = fdir_0.flat[startnode]
         endnode_1 = fdir_1.flat[startnode]
         prop_0 = props_0.flat[startnode]
         prop_1 = props_1.flat[startnode]
         _dinf_accumulation_recursion(startnode, endnode_0, acc, fdir_0, fdir_1,
@@ -594,15 +609,15 @@
 
 @njit(float64[:,:](float64[:,:], int64[:,:], int64[:,:], uint8[:], int64[:],
                    float64[:,:], float64[:,:], float64[:,:]),
       cache=True)
 def _dinf_accumulation_eff_numba(acc, fdir_0, fdir_1, indegree, startnodes,
                                  props_0, props_1, eff):
     n = startnodes.size
-    visited = np.zeros(acc.shape, dtype=np.bool8)
+    visited = np.zeros(acc.shape, dtype=np.bool_)
     for k in range(n):
         startnode = startnodes.flat[k]
         endnode_0 = fdir_0.flat[startnode]
         endnode_1 = fdir_1.flat[startnode]
         prop_0 = props_0.flat[startnode]
         prop_1 = props_1.flat[startnode]
         _dinf_accumulation_eff_recursion(startnode, endnode_0, acc, fdir_0, fdir_1,
@@ -725,15 +740,15 @@
                 next_inc = inc + weights.flat[neighbor]
                 _d8_flow_distance_recursion(neighbor, fdir, visits, dist, weights,
                                             r_dirmap, next_inc, offsets)
 
 @njit(float64[:,:](int64[:,:], float64[:,:], UniTuple(int64, 2), UniTuple(int64, 8)),
       cache=True)
 def _d8_flow_distance_recur_numba(fdir, weights, pour_point, dirmap):
-    visits = np.zeros(fdir.shape, dtype=np.bool8)
+    visits = np.zeros(fdir.shape, dtype=np.bool_)
     dist = np.full(fdir.shape, np.inf, dtype=np.float64)
     r_dirmap = np.array([dirmap[4], dirmap[5], dirmap[6],
                          dirmap[7], dirmap[0], dirmap[1],
                          dirmap[2], dirmap[3]])
     m, n = fdir.shape
     offsets = np.array([-n, 1 - n, 1,
                         1 + n, n, - 1 + n,
@@ -743,15 +758,15 @@
     _d8_flow_distance_recursion(ix, fdir, visits, dist, weights,
                                 r_dirmap, 0., offsets)
     return dist
 
 @njit(float64[:,:](int64[:,:], float64[:,:], UniTuple(int64, 2), UniTuple(int64, 8)),
       cache=True)
 def _d8_flow_distance_iter_numba(fdir, weights, pour_point, dirmap):
-    visits = np.zeros(fdir.shape, dtype=np.bool8)
+    visits = np.zeros(fdir.shape, dtype=np.bool_)
     dist = np.full(fdir.shape, np.inf, dtype=np.float64)
     r_dirmap = np.array([dirmap[4], dirmap[5], dirmap[6],
                          dirmap[7], dirmap[0], dirmap[1],
                          dirmap[2], dirmap[3]])
     m, n = fdir.shape
     offsets = np.array([-n, 1 - n, 1,
                         1 + n, n, - 1 + n,
@@ -801,15 +816,15 @@
                                               offsets)
 
 @njit(float64[:,:](int64[:,:], int64[:,:], float64[:,:], float64[:,:],
                    UniTuple(int64, 2), UniTuple(int64, 8)),
       cache=True)
 def _dinf_flow_distance_recur_numba(fdir_0, fdir_1, weights_0, weights_1,
                               pour_point, dirmap):
-    visits = np.zeros(fdir_0.shape, dtype=np.bool8)
+    visits = np.zeros(fdir_0.shape, dtype=np.bool_)
     dist = np.full(fdir_0.shape, np.inf, dtype=np.float64)
     r_dirmap = np.array([dirmap[4], dirmap[5], dirmap[6],
                          dirmap[7], dirmap[0], dirmap[1],
                          dirmap[2], dirmap[3]])
     m, n = fdir_0.shape
     offsets = np.array([-n, 1 - n, 1,
                         1 + n, n, - 1 + n,
@@ -822,15 +837,15 @@
 
 @njit(float64[:,:](int64[:,:], int64[:,:], float64[:,:], float64[:,:],
                    UniTuple(int64, 2), UniTuple(int64, 8)),
       cache=True)
 def _dinf_flow_distance_iter_numba(fdir_0, fdir_1, weights_0, weights_1,
                                    pour_point, dirmap):
     dist = np.full(fdir_0.shape, np.inf, dtype=np.float64)
-    visited = np.zeros(fdir_0.shape, dtype=np.bool8)
+    visited = np.zeros(fdir_0.shape, dtype=np.bool_)
     r_dirmap = np.array([dirmap[4], dirmap[5], dirmap[6],
                          dirmap[7], dirmap[0], dirmap[1],
                          dirmap[2], dirmap[3]])
     m, n = fdir_0.shape
     offsets = np.array([-n, 1 - n, 1,
                         1 + n, n, - 1 + n,
                         - 1, - 1 - n])
@@ -866,15 +881,15 @@
 # neighbor_dist = parent_dist + weights.flat[kix]
 @njit(float64[:,:](float64[:,:,:], UniTuple(int64, 2), float64[:,:]),
       cache=True)
 def _mfd_flow_distance_iter_numba(fdir, pour_point, weights):
     _, m, n = fdir.shape
     mn = m * n
     dist = np.full((m, n), np.inf, dtype=np.float64)
-    visited = np.zeros((m, n), dtype=np.bool8)
+    visited = np.zeros((m, n), dtype=np.bool_)
     i, j = pour_point
     ix = (i * n) + j
     offsets = np.array([-n, 1 - n, 1,
                         1 + n, n, - 1 + n,
                         - 1, - 1 - n])
     r_dirmap = np.array([4, 5, 6, 7,
                          0, 1, 2, 3])
@@ -1003,17 +1018,17 @@
 
 @njit(UniTuple(boolean[:,:], 3)(float64[:,:], int64[:]),
       parallel=True,
       cache=True)
 def _par_get_candidates_numba(dem, inside):
     n = inside.size
     offset = dem.shape[1]
-    fdirs_defined = np.zeros(dem.shape, dtype=np.bool8)
-    flats = np.zeros(dem.shape, dtype=np.bool8)
-    higher_cells = np.zeros(dem.shape, dtype=np.bool8)
+    fdirs_defined = np.zeros(dem.shape, dtype=np.bool_)
+    flats = np.zeros(dem.shape, dtype=np.bool_)
+    higher_cells = np.zeros(dem.shape, dtype=np.bool_)
     offsets = np.array([-offset, 1 - offset, 1,
                         1 + offset, offset, - 1 + offset,
                         - 1, - 1 - offset])
     for i in prange(n):
         k = inside[i]
         inner_neighbors = (k + offsets)
         fdir_defined = False
@@ -1545,15 +1560,15 @@
 
 @njit(float64[:,:](int64[:,:], UniTuple(int64, 8), float64, float64),
       parallel=True,
       cache=True)
 def _d8_cell_distances_numba(fdir, dirmap, dx, dy):
     n = fdir.size
     cdist = np.zeros(fdir.shape, dtype=np.float64)
-    dd = np.sqrt(dx**2 + dy**2)
+    dd = math.sqrt(dx**2 + dy**2)
     distances = (dy, dd, dx, dd, dy, dd, dx, dd)
     dist_map = {0 : 0.}
     for i in range(8):
         dist_map[dirmap[i]] = distances[i]
     for k in prange(n):
         fdir_k = fdir.flat[k]
         cdist.flat[k] = dist_map[fdir_k]
@@ -1562,15 +1577,15 @@
 @njit(float64[:,:](int64[:,:], int64[:,:], float64[:,:], float64[:,:], UniTuple(int64, 8),
                    float64, float64),
       parallel=True,
       cache=True)
 def _dinf_cell_distances_numba(fdir_0, fdir_1, prop_0, prop_1, dirmap, dx, dy):
     n = fdir_0.size
     cdist = np.zeros(fdir_0.shape, dtype=np.float64)
-    dd = np.sqrt(dx**2 + dy**2)
+    dd = math.sqrt(dx**2 + dy**2)
     distances = (dy, dd, dx, dd, dy, dd, dx, dd)
     dist_map = {0 : 0.}
     for i in range(8):
         dist_map[dirmap[i]] = distances[i]
     for k in prange(n):
         fdir_k_0 = fdir_0.flat[k]
         fdir_k_1 = fdir_1.flat[k]
@@ -1585,15 +1600,15 @@
 @njit(float64[:,:](int64[:,:], int64[:,:,:], float64[:,:,:], float64, float64),
       parallel=True,
       cache=True)
 def _mfd_cell_distances_numba(startnodes, endnodes, props, dx, dy):
     k, m, n = props.shape
     mn = m * n
     N = startnodes.size
-    dd = np.sqrt(dx**2 + dy**2)
+    dd = math.sqrt(dx**2 + dy**2)
     distances = (dy, dd, dx, dd, dy, dd, dx, dd)
     cdist = np.zeros((m, n), dtype=np.float64)
     for i in prange(N):
         startnode = startnodes.flat[i]
         for j in prange(k):
             kix = startnode + (j * mn)
             endnode = endnodes.flat[kix]
@@ -1639,15 +1654,15 @@
         _dinf_fix_cycles_recursion(right, fdir_0, fdir_1, ancestor,
                                    depth + 1, max_cycle_size, visited)
 
 @njit(void(int64[:,:], int64[:,:], int64),
       cache=True)
 def _dinf_fix_cycles_numba(fdir_0, fdir_1, max_cycle_size):
     n = fdir_0.size
-    visited = np.zeros(fdir_0.shape, dtype=np.bool8)
+    visited = np.zeros(fdir_0.shape, dtype=np.bool_)
     depth = 0
     for node in range(n):
         _dinf_fix_cycles_recursion(node, fdir_0, fdir_1, node,
                                    depth, max_cycle_size, visited)
         visited.flat[node] = True
 
 # TODO: Assumes pits and flats are removed
@@ -1803,15 +1818,15 @@
 
 @njit(boolean[:,:](float64[:,:], int64[:]),
       parallel=True,
       cache=True)
 def _find_pits_numba(dem, inside):
     n = inside.size
     offset = dem.shape[1]
-    pits = np.zeros(dem.shape, dtype=np.bool8)
+    pits = np.zeros(dem.shape, dtype=np.bool_)
     offsets = np.array([-offset, 1 - offset, 1,
                         1 + offset, offset, - 1 + offset,
                         - 1, - 1 - offset])
     for i in prange(n):
         k = inside[i]
         inner_neighbors = (k + offsets)
         is_pit = True
@@ -1839,7 +1854,153 @@
         adjustment = max_diff
         for j in prange(8):
             neighbor = inner_neighbors[j]
             diff = dem.flat[neighbor] - dem.flat[k]
             adjustment = min(diff, adjustment)
         pits_filled.flat[k] += (adjustment)
     return pits_filled
+
+@njit(boundscheck=True, cache=True)
+def _first_true1d(arr, start=0, end=None, step=1, invert=False):
+    if end is None:
+        end = len(arr)
+
+    if invert:
+        for i in range(start, end, step):
+            if not arr[i]:
+                return i
+        else:
+            return -1
+    else:
+        for i in range(start, end, step):
+            if arr[i]:
+                return i
+        else:
+            return -1
+
+@njit(parallel=True, cache=True)
+def _top(mask):
+    nc = mask.shape[1]
+    rv = np.zeros(nc, dtype='int64')
+    for i in prange(nc):
+        rv[i] = _first_true1d(mask[:, i], invert=True)
+    return rv
+
+@njit(parallel=True, cache=True)
+def _bottom(mask):
+    nr, nc = mask.shape[0], mask.shape[1]
+    rv = np.zeros(nc, dtype='int64')
+    for i in prange(nc):
+        rv[i] = _first_true1d(mask[:, i], start=nr - 1, end=-1, step=-1, invert=True)
+    return rv
+
+@njit(parallel=True, cache=True)
+def _left(mask):
+    nr = mask.shape[0]
+    rv = np.zeros(nr, dtype='int64')
+    for i in prange(nr):
+        rv[i] = _first_true1d(mask[i, :], invert=True)
+    return rv
+
+@njit(parallel=True, cache=True)
+def _right(mask):
+    nr, nc = mask.shape[0], mask.shape[1]
+    rv = np.zeros(nr, dtype='int64')
+    for i in prange(nr):
+        rv[i] = _first_true1d(mask[i, :], start=nc - 1, end=-1, step=-1, invert=True)
+    return rv
+
+
+@njit(cache=True)
+def count(start=0, step=1):
+    # Numba accelerated count() from itertools
+    # count(10) --> 10 11 12 13 14 ...
+    # count(2.5, 0.5) --> 2.5 3.0 3.5 ...
+    n = start
+    while True:
+        yield n
+        n += step
+
+
+def pfwrapper(func):
+    # Implemenation detail of priority-flood algorithm
+    # Needed to define the types used in priority queue
+    @wraps(func)
+    def _wrapper(dem, mask, *args):
+        # Tuple elements:
+        # 0: dem data type (for elevation priority)
+        # 1: int64 for insertion index (to maintain total ordering)
+        # 2: int64 for row index
+        # 3: int64 for col index
+        tuple_type = Tuple([from_dtype(dem.dtype), int64, int64, int64])
+        return func(dem, mask, tuple_type, *args)
+    return _wrapper
+
+
+@pfwrapper
+@njit(cache=True)
+def _priority_flood(dem, dem_mask, tuple_type):
+    open_cells = typedlist.List.empty_list(tuple_type)  # Priority queue
+    pits = typedlist.List.empty_list(tuple_type)  # FIFO queue
+    closed_cells = dem_mask.copy()
+    isertn = count()
+
+    # Push the edges onto priority queue
+    y, x = dem.shape
+
+    edge = _left(dem_mask)[:-1]
+    for row, col in zip(count(), edge):
+        if col >= 0:
+            open_cells.append((dem[row, col], next(isertn), row, col))
+            closed_cells[row, col] = True
+    edge = _bottom(dem_mask)[:-1]
+    for row, col in zip(edge, count()):
+        if row >= 0:
+            open_cells.append((dem[row, col], next(isertn), row, col))
+            closed_cells[row, col] = True
+    edge = np.flip(_right(dem_mask))[:-1]
+    for row, col in zip(count(y - 1, step=-1), edge):
+        if col >= 0:
+            open_cells.append((dem[row, col], next(isertn), row, col))
+            closed_cells[row, col] = True
+    edge = np.flip(_top(dem_mask))[:-1]
+    for row, col in zip(edge, count(x - 1, step=-1)):
+        if row >= 0:
+            open_cells.append((dem[row, col], next(isertn), row, col))
+            closed_cells[row, col] = True
+    heapify(open_cells)
+
+    row_offsets = np.array([-1, -1, 0, 1, 1, 1, 0, -1])
+    col_offsets = np.array([0, 1, 1, 1, 0, -1, -1, -1])
+
+    pits_pos = 0
+    while open_cells or pits_pos < len(pits):
+        if pits_pos < len(pits):
+            elv, _, i, j = pits[pits_pos]
+            pits_pos += 1
+        else:
+            elv, _, i, j = heappop(open_cells)
+
+        for n in range(8):
+            row = i + row_offsets[n]
+            col = j + col_offsets[n]
+
+            if row < 0 or row >= y or col < 0 or col >= x:
+                continue
+
+            if dem_mask[row, col] or closed_cells[row, col]:
+                continue
+
+            if dem[row, col] <= elv:
+                dem[row, col] = elv
+                pits.append((elv, next(isertn), row, col))
+            else:
+                heappush(open_cells, (dem[row, col], next(isertn), row, col))
+            closed_cells[row, col] = True
+
+        # pits book-keeping
+        if pits_pos == len(pits) and len(pits) > 1024:
+            # Queue is empty, lets clear it out
+            pits.clear()
+            pits_pos = 0
+
+    return dem
```

### Comparing `pysheds-0.3.5/pysheds/_sview.py` & `pysheds-0.4/pysheds/_sview.py`

 * *Files identical despite different names*

### Comparing `pysheds-0.3.5/pysheds/io.py` & `pysheds-0.4/pysheds/io.py`

 * *Files identical despite different names*

### Comparing `pysheds-0.3.5/pysheds/pgrid.py` & `pysheds-0.4/pysheds/pgrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import ast
 import warnings
 import pyproj
 import numpy as np
 import pandas as pd
 import geojson
 from affine import Affine
-from distutils.version import LooseVersion
+from looseversion import LooseVersion
 try:
     import scipy.sparse
     import scipy.spatial
     from scipy.sparse import csgraph
     import scipy.interpolate
     _HAS_SCIPY = True
 except (ModuleNotFoundError, ImportError):
```

### Comparing `pysheds-0.3.5/pysheds/projection.py` & `pysheds-0.4/pysheds/projection.py`

 * *Files identical despite different names*

### Comparing `pysheds-0.3.5/pysheds/pview.py` & `pysheds-0.4/pysheds/pview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from scipy import spatial
 from scipy import interpolate
 import pyproj
 from affine import Affine
-from distutils.version import LooseVersion
+from looseversion import LooseVersion
 
 _OLD_PYPROJ = LooseVersion(pyproj.__version__) < LooseVersion('2.2')
 _pyproj_init = '+init=epsg:4326' if _OLD_PYPROJ else 'epsg:4326'
 
 class Raster(np.ndarray):
     def __new__(cls, input_array, viewfinder, metadata=None):
         obj = np.asarray(input_array).view(cls)
```

### Comparing `pysheds-0.3.5/pysheds/rfsm.py` & `pysheds-0.4/pysheds/rfsm.py`

 * *Files identical despite different names*

### Comparing `pysheds-0.3.5/pysheds/sgrid.py` & `pysheds-0.4/pysheds/sgrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import ast
 import copy
 # import pyproj
 import numpy as np
 import pandas as pd
 import geojson
 from affine import Affine
+from numba.types import Tuple, int64
+from numba import from_dtype
+
 try:
     import skimage.measure
-    import skimage.morphology
     _HAS_SKIMAGE = True
 except ModuleNotFoundError:
     _HAS_SKIMAGE = False
 try:
     import rasterio
     import rasterio.features
     _HAS_RASTERIO = True
@@ -702,15 +704,15 @@
 
         Additional keyword arguments (**kwargs) are passed to self.view.
 
         Returns
         -------
         catch : Raster
                 Raster indicating cells that lie in the catchment. The dtype will be
-                np.bool8, unless `pour_value` is specified, in which case the dtype will
+                np.bool_, unless `pour_value` is specified, in which case the dtype will
                 be the smallest dtype capable of representing the pour value.
         """
         if routing.lower() == 'd8':
             input_overrides = {'dtype' : np.int64, 'nodata' : fdir.nodata}
         elif routing.lower() == 'dinf':
             input_overrides = {'dtype' : np.float64, 'nodata' : fdir.nodata}
         elif routing.lower() == 'mfd':
@@ -1278,15 +1280,15 @@
         elif routing.lower() == 'dinf':
             fdir_overrides = {'dtype' : np.float64, 'nodata' : fdir.nodata}
         elif routing.lower() == 'mfd':
             fdir_overrides = {'dtype' : np.float64, 'nodata' : fdir.nodata}
         else:
             raise ValueError('Routing method must be one of: `d8`, `dinf`, `mfd`')
         dem_overrides = {'dtype' : np.float64, 'nodata' : dem.nodata}
-        mask_overrides = {'dtype' : np.bool8, 'nodata' : False}
+        mask_overrides = {'dtype' : np.bool_, 'nodata' : False}
         kwargs.update(fdir_overrides)
         fdir = self._input_handler(fdir, **kwargs)
         kwargs.update(dem_overrides)
         dem = self._input_handler(dem, **kwargs)
         kwargs.update(mask_overrides)
         mask = self._input_handler(mask, **kwargs)
         # Set default nodata for hand index and hand
@@ -1408,15 +1410,15 @@
               A geojson feature collection of river segments. Each array contains the cell
               indices of junctions in the segment.
         """
         if routing.lower() == 'd8':
             fdir_overrides = {'dtype' : np.int64, 'nodata' : fdir.nodata}
         else:
             raise NotImplementedError('Only implemented for `d8` routing.')
-        mask_overrides = {'dtype' : np.bool8, 'nodata' : False}
+        mask_overrides = {'dtype' : np.bool_, 'nodata' : False}
         kwargs.update(fdir_overrides)
         fdir = self._input_handler(fdir, **kwargs)
         kwargs.update(mask_overrides)
         mask = self._input_handler(mask, **kwargs)
         # Find nodata cells and invalid cells
         nodata_cells = self._get_nodata_cells(fdir)
         invalid_cells = ~np.in1d(fdir.ravel(), dirmap).reshape(fdir.shape)
@@ -1491,15 +1493,15 @@
                       the value represents the index of the downstream profile that it drains to.
                       Indices correspond to the ordered elements of the `profiles` object.
         """
         if routing.lower() == 'd8':
             fdir_overrides = {'dtype' : np.int64, 'nodata' : fdir.nodata}
         else:
             raise NotImplementedError('Only implemented for `d8` routing.')
-        mask_overrides = {'dtype' : np.bool8, 'nodata' : False}
+        mask_overrides = {'dtype' : np.bool_, 'nodata' : False}
         kwargs.update(fdir_overrides)
         fdir = self._input_handler(fdir, **kwargs)
         kwargs.update(mask_overrides)
         mask = self._input_handler(mask, **kwargs)
         # Find nodata cells and invalid cells
         nodata_cells = self._get_nodata_cells(fdir)
         invalid_cells = ~np.in1d(fdir.ravel(), dirmap).reshape(fdir.shape)
@@ -1555,15 +1557,15 @@
         order : Raster
                 Raster indicating Strahler stream order of each cell
         """
         if routing.lower() == 'd8':
             fdir_overrides = {'dtype' : np.int64, 'nodata' : fdir.nodata}
         else:
             raise NotImplementedError('Only implemented for `d8` routing.')
-        mask_overrides = {'dtype' : np.bool8, 'nodata' : False}
+        mask_overrides = {'dtype' : np.bool_, 'nodata' : False}
         kwargs.update(fdir_overrides)
         fdir = self._input_handler(fdir, **kwargs)
         kwargs.update(mask_overrides)
         mask = self._input_handler(mask, **kwargs)
         # Find nodata cells and invalid cells
         nodata_cells = self._get_nodata_cells(fdir)
         invalid_cells = ~np.in1d(fdir.ravel(), dirmap).reshape(fdir.shape)
@@ -2109,21 +2111,19 @@
         Additional keyword arguments (**kwargs) are passed to self.view.
 
         Returns
         -------
         depressions : Raster
                       Boolean Raster indicating locations of depressions.
         """
-        if not _HAS_SKIMAGE:
-            raise ImportError('detect_depressions requires skimage.morphology module')
         input_overrides = {'dtype' : np.float64, 'nodata' : dem.nodata}
         kwargs.update(input_overrides)
         dem = self._input_handler(dem, **kwargs)
         filled_dem = self.fill_depressions(dem, **kwargs)
-        depressions = np.zeros(filled_dem.shape, dtype=np.bool8)
+        depressions = np.zeros(filled_dem.shape, dtype=np.bool_)
         depressions[dem != filled_dem] = True
         depressions[np.isnan(dem) | np.isnan(filled_dem)] = False
         depressions = self._output_handler(data=depressions,
                                            viewfinder=filled_dem.viewfinder,
                                            metadata=filled_dem.metadata,
                                            nodata=False)
         return depressions
@@ -2144,31 +2144,21 @@
 
         Returns
         -------
         flooded_dem : Raster
                       Raster representing digital elevation data with multi-celled
                       depressions removed.
         """
-        if not _HAS_SKIMAGE:
-            raise ImportError('resolve_flats requires skimage.morphology module')
-        input_overrides = {'dtype' : np.float64, 'nodata' : dem.nodata}
-        kwargs.update(input_overrides)
-        dem = self._input_handler(dem, **kwargs)
         dem_mask = self._get_nodata_cells(dem)
-        dem_mask[0, :] = True
-        dem_mask[-1, :] = True
-        dem_mask[:, 0] = True
-        dem_mask[:, -1] = True
-        # Make sure nothing flows to the nodata cells
-        seed = np.copy(dem)
-        seed[~dem_mask] = np.nanmax(dem)
-        dem_out = skimage.morphology.reconstruction(seed, dem, method='erosion')
-        dem_out = self._output_handler(data=dem_out, viewfinder=dem.viewfinder,
-                                     metadata=dem.metadata, nodata=nodata_out)
-        return dem_out
+        result = _self._priority_flood(dem, dem_mask)
+        dem_filled = self._output_handler(data=result,
+                                        viewfinder=dem.viewfinder,
+                                        metadata=dem.metadata,
+                                        nodata=dem.nodata)
+        return dem_filled
 
     def detect_flats(self, dem, **kwargs):
         """
         Detect flats in a digital elevation dataset.
 
         Parameters
         ----------
@@ -2378,15 +2368,15 @@
         dist : np.ndarray with shape (N,), (optional)
                Distances from points in xy to xy_new
         """
         try:
             assert isinstance(mask, Raster)
         except:
             raise TypeError('`mask` must be a Raster instance.')
-        mask_overrides = {'dtype' : np.bool8, 'nodata' : False}
+        mask_overrides = {'dtype' : np.bool_, 'nodata' : False}
         kwargs.update(mask_overrides)
         mask = self._input_handler(mask, **kwargs)
         affine = mask.affine
         return View.snap_to_mask(mask, xy, affine=affine,
                                  return_dist=return_dist)
 
     def _input_handler(self, data, **kwargs):
@@ -2412,17 +2402,17 @@
     def _get_nodata_cells(self, data):
         try:
             assert (isinstance(data, Raster))
         except:
             raise TypeError('Data must be a Raster.')
         nodata = data.nodata
         if np.isnan(nodata):
-            nodata_cells = np.isnan(data).astype(np.bool8)
+            nodata_cells = np.isnan(data).astype(np.bool_)
         else:
-            nodata_cells = (data == nodata).astype(np.bool8)
+            nodata_cells = (data == nodata).astype(np.bool_)
         return nodata_cells
 
     def _pop_rim(self, data, nodata=0):
         left, right, top, bottom = (data[:,0].copy(), data[:,-1].copy(),
                                     data[0,:].copy(), data[-1,:].copy())
         data[...,  :,  0] = nodata
         data[...,  :, -1] = nodata
```

### Comparing `pysheds-0.3.5/pysheds/sview.py` & `pysheds-0.4/pysheds/sview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import numpy as np
 from . import projection
 from affine import Affine
-from distutils.version import LooseVersion
+from looseversion import LooseVersion
 try:
     import scipy.spatial
     _HAS_SCIPY = True
 except ModuleNotFoundError:
     _HAS_SCIPY = False
 
 import pysheds._sview as _self
@@ -78,15 +78,15 @@
         # Test typing of array
         try:
             assert not np.issubdtype(obj.dtype, np.object_)
             assert not np.issubdtype(obj.dtype, np.flexible)
         except:
             raise TypeError('`object` and `flexible` dtypes not allowed.')
         try:
-            assert np.min_scalar_type(viewfinder.nodata) <= obj.dtype
+            assert np.can_cast(viewfinder.nodata, obj.dtype, casting='safe')
         except:
             raise TypeError('`nodata` value not representable in dtype of array.')
         # Don't allow original viewfinder and metadata to be modified
         viewfinder = viewfinder.copy()
         metadata = metadata.copy()
         # Set attributes of array
         obj._viewfinder = viewfinder
@@ -284,15 +284,15 @@
         # Test typing of array
         try:
             assert not np.issubdtype(obj.dtype, np.object_)
             assert not np.issubdtype(obj.dtype, np.flexible)
         except:
             raise TypeError('`object` and `flexible` dtypes not allowed.')
         try:
-            assert np.min_scalar_type(viewfinder.nodata) <= obj.dtype
+            assert np.can_cast(viewfinder.nodata, obj.dtype, casting='safe')
         except:
             raise TypeError('`nodata` value not representable in dtype of array.')
         # Don't allow original viewfinder and metadata to be modified
         viewfinder = viewfinder.copy()
         metadata = metadata.copy()
         # Set attributes of array
         obj._viewfinder = viewfinder
@@ -330,15 +330,15 @@
     """
     def __init__(self, affine=Affine(1., 0., 0., 0., 1., 0.), shape=(1,1),
                  nodata=0, mask=None, crs=projection.init()):
         self.affine = affine
         self.crs = crs
         self.nodata = nodata
         if mask is None:
-            self.mask = np.ones(shape, dtype=np.bool8)
+            self.mask = np.ones(shape, dtype=np.bool_)
         else:
             self.mask = mask
 
     def __eq__(self, other):
         if isinstance(other, ViewFinder):
             is_eq = True
             is_eq &= (self.affine == other.affine)
@@ -381,18 +381,18 @@
     @property
     def mask(self):
         return self._mask
 
     @mask.setter
     def mask(self, new_mask):
         try:
-            assert (np.min_scalar_type(new_mask) <= np.dtype(np.bool8))
+            assert (np.min_scalar_type(new_mask) <= np.dtype(np.bool_))
         except:
             raise TypeError('`mask` must be of boolean type')
-        new_mask = np.asarray(new_mask).astype(np.bool8)
+        new_mask = np.asarray(new_mask).astype(np.bool_)
         self._mask = new_mask
 
     @property
     def nodata(self):
         return self._nodata
 
     @nodata.setter
@@ -617,15 +617,15 @@
 
     @classmethod
     def _view_multiraster(cls, data, target_view, data_view=None, interpolation='nearest',
                           apply_output_mask=True, dtype=None, out=None):
         k, m, n = data.shape
         if out is None:
             out = np.empty((k, *target_view.shape), dtype=dtype)
-        out_mask = np.ones((k, *target_view.shape), dtype=np.bool8)
+        out_mask = np.ones((k, *target_view.shape), dtype=np.bool_)
         for i in range(k):
             slice_viewfinder = ViewFinder(affine=data_view.affine, mask=data_view.mask[i],
                                           nodata=data_view.nodata, crs=data_view.crs)
             data_i = Raster(np.asarray(data[i]), viewfinder=slice_viewfinder)
             # Write to out array in-place
             view_i = cls._view_raster(data_i, target_view, slice_viewfinder,
                                       interpolation=interpolation,
@@ -967,8 +967,7 @@
         if interpolation == 'nearest':
             view = _self._view_fill_by_entries_nearest_numba(data, view, y_ix, x_ix, nodata)
         elif interpolation == 'linear':
             view = _self._view_fill_by_entries_linear_numba(data, view, y_ix, x_ix, nodata)
         else:
             raise ValueError('Interpolation method must be one of: `nearest`, `linear`')
         return view
-
```

### Comparing `pysheds-0.3.5/pysheds.egg-info/PKG-INFO` & `pysheds-0.4/pysheds.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: pysheds
-Version: 0.3.5
+Version: 0.4
 Summary: 🌎 Simple and fast watershed delineation in python.
 Home-page: http://open-storm.org
 Author: Matt Bartos
 Author-email: mdbartos@umich.edu
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: recipes
 License-File: LICENSE
 
 🌎 Simple and fast watershed delineation in python.
+
```

### Comparing `pysheds-0.3.5/setup.py` & `pysheds-0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
     name="pysheds",
-    version="0.3.5",
+    version="0.4",
     description="🌎 Simple and fast watershed delineation in python.",
     long_description="🌎 Simple and fast watershed delineation in python.",
     long_description_content_type="text/x-rst",
     author="Matt Bartos",
     author_email="mdbartos@umich.edu",
     url="http://open-storm.org",
     packages=["pysheds"],
@@ -22,21 +22,23 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering :: GIS",
         "Topic :: Scientific/Engineering :: Hydrology",
     ],
     include_package_data=True,
     install_requires=[
         "affine",
         "geojson",
+        "looseversion",
         "numba",
         "numpy",
         "pandas",
         "pyproj",
         "rasterio>=1",
         "scikit-image",
         "scipy",
```

