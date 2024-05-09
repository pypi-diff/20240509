# Comparing `tmp/delaunay_triangulation_and_its_dual_2d-0.1.2.tar.gz` & `tmp/delaunay_triangulation_and_its_dual_2d-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delaunay_triangulation_and_its_dual_2d-0.1.2.tar", last modified: Sun May  5 04:12:56 2024, max compression
+gzip compressed data, was "delaunay_triangulation_and_its_dual_2d-0.1.3.tar", last modified: Thu May  9 14:47:00 2024, max compression
```

## Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2.tar` & `delaunay_triangulation_and_its_dual_2d-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 04:12:56.631075 delaunay_triangulation_and_its_dual_2d-0.1.2/
--rw-rw-rw-   0        0        0     3318 2024-05-05 03:33:40.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/.gitignore
--rw-rw-rw-   0        0        0     1086 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6089 2024-05-05 04:12:56.630077 delaunay_triangulation_and_its_dual_2d-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4084 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 04:12:56.605140 delaunay_triangulation_and_its_dual_2d-0.1.2/assets/
--rw-rw-rw-   0        0        0    66443 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/assets/time_to_compute_voronoi_tessellation.png
-drwxrwxrwx   0        0        0        0 2024-05-05 04:12:56.613021 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/
--rw-rw-rw-   0        0        0       32 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/__init__.py
--rw-rw-rw-   0        0        0      427 2024-05-05 04:12:56.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/_version.py
--rw-rw-rw-   0        0        0    17815 2024-05-05 04:11:33.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/delaunay.py
--rw-rw-rw-   0        0        0       58 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-05 04:12:56.625075 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/geometry/
--rw-rw-rw-   0        0        0      142 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/geometry/__init__.py
--rw-rw-rw-   0        0        0     1673 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py
--rw-rw-rw-   0        0        0      220 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/geometry/centroid.py
--rw-rw-rw-   0        0        0     2758 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py
-drwxrwxrwx   0        0        0        0 2024-05-05 04:12:56.626076 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/util/
--rw-rw-rw-   0        0        0       65 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/util/__init__.py
--rw-rw-rw-   0        0        0      865 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py
-drwxrwxrwx   0        0        0        0 2024-05-05 04:12:56.629076 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d.egg-info/
--rw-rw-rw-   0        0        0     6089 2024-05-05 04:12:56.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1066 2024-05-05 04:12:56.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 04:12:56.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-05-05 04:12:56.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       39 2024-05-05 04:12:56.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1319 2024-05-05 04:11:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 04:12:56.631075 delaunay_triangulation_and_its_dual_2d-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 04:12:56.602045 delaunay_triangulation_and_its_dual_2d-0.1.2/tests/
-drwxrwxrwx   0        0        0        0 2024-05-05 04:12:56.628132 delaunay_triangulation_and_its_dual_2d-0.1.2/tests/delaunay/
--rw-rw-rw-   0        0        0     2484 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/tests/delaunay/performance.py
--rw-rw-rw-   0        0        0      481 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/tests/delaunay/profiling.py
--rw-rw-rw-   0        0        0     6180 2024-05-05 03:48:22.000000 delaunay_triangulation_and_its_dual_2d-0.1.2/tests/delaunay/test_all.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:47:00.415526 delaunay_triangulation_and_its_dual_2d-0.1.3/
+-rw-rw-rw-   0        0        0     3318 2024-05-05 03:33:40.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/.gitignore
+-rw-rw-rw-   0        0        0     1086 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6089 2024-05-09 14:47:00.415526 delaunay_triangulation_and_its_dual_2d-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4084 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 14:47:00.388470 delaunay_triangulation_and_its_dual_2d-0.1.3/assets/
+-rw-rw-rw-   0        0        0    66443 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/assets/time_to_compute_voronoi_tessellation.png
+drwxrwxrwx   0        0        0        0 2024-05-09 14:47:00.394985 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/
+-rw-rw-rw-   0        0        0       32 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/__init__.py
+-rw-rw-rw-   0        0        0      427 2024-05-09 14:47:00.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/_version.py
+-rw-rw-rw-   0        0        0    22443 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/delaunay.py
+-rw-rw-rw-   0        0        0       58 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:47:00.408000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/geometry/
+-rw-rw-rw-   0        0        0      142 2024-05-09 13:57:34.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/geometry/__init__.py
+-rw-rw-rw-   0        0        0     3932 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py
+-rw-rw-rw-   0        0        0      220 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/geometry/centroid.py
+-rw-rw-rw-   0        0        0     2758 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:47:00.409000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/util/
+-rw-rw-rw-   0        0        0       65 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/util/__init__.py
+-rw-rw-rw-   0        0        0      865 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:47:00.414526 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d.egg-info/
+-rw-rw-rw-   0        0        0     6089 2024-05-09 14:47:00.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2024-05-09 14:47:00.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 14:47:00.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-05-09 14:47:00.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       39 2024-05-09 14:47:00.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1319 2024-05-05 04:11:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 14:47:00.415526 delaunay_triangulation_and_its_dual_2d-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 14:47:00.386468 delaunay_triangulation_and_its_dual_2d-0.1.3/tests/
+drwxrwxrwx   0        0        0        0 2024-05-09 14:47:00.412518 delaunay_triangulation_and_its_dual_2d-0.1.3/tests/delaunay/
+-rw-rw-rw-   0        0        0        0 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/tests/delaunay/__init__.py
+-rw-rw-rw-   0        0        0     2484 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/tests/delaunay/performance.py
+-rw-rw-rw-   0        0        0      481 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/tests/delaunay/profiling.py
+-rw-rw-rw-   0        0        0     6180 2024-05-05 03:48:22.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/tests/delaunay/test_all.py
+-rw-rw-rw-   0        0        0     2651 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/tests/delaunay/try.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:47:00.413526 delaunay_triangulation_and_its_dual_2d-0.1.3/tests/geometry/
+-rw-rw-rw-   0        0        0        0 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.3/tests/geometry/__init__.py
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/.gitignore` & `delaunay_triangulation_and_its_dual_2d-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/LICENSE` & `delaunay_triangulation_and_its_dual_2d-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/PKG-INFO` & `delaunay_triangulation_and_its_dual_2d-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay-triangulation-and-its-dual-2d
-Version: 0.1.2
+Version: 0.1.3
 License: MIT License
         
         Copyright (c) 2024 M.H. Luk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/README.md` & `delaunay_triangulation_and_its_dual_2d-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/assets/time_to_compute_voronoi_tessellation.png` & `delaunay_triangulation_and_its_dual_2d-0.1.3/assets/time_to_compute_voronoi_tessellation.png`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/delaunay.py` & `delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/delaunay.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC, abstractmethod
 from collections import defaultdict, deque
 import logging
+from typing import Literal
 
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy.typing import NDArray
 import scipy
 from scipy.spatial import voronoi_plot_2d
 
@@ -40,14 +41,21 @@
         self._triangles: NDArray[np.intc]
         self._ridge_points: NDArray[np.int32]
         self._ridge_vertices: list[list[int]]
         self._regions: list[list[int]]
         self._voronoi_vertices: NDArray[np.float_]
         self._barycentric_dual_vertices: NDArray[np.float_]
 
+        self._delaunay_edge_to_triangle_indices_mapping: dict[
+            tuple[int, int], list[int]
+        ]
+        self._dual_edges_to_delaunay_edges_mapping: dict[
+            tuple[int, int], tuple[int, int]
+        ]
+
     @property
     def points(self) -> NDArray[np.float_]:
         return self._points
 
     @property
     def bounding_box(self) -> BoundingBox2d:
         return self._bounding_box
@@ -78,14 +86,21 @@
         return self._voronoi_vertices
 
     @property
     def barycentric_dual_vertices(self) -> NDArray[np.float_]:
         self.compute_barycentric_dual()
         return self._barycentric_dual_vertices
 
+    @property
+    def dual_edges_to_delaunay_edges_mapping(
+        self,
+    ) -> dict[tuple[int, int], tuple[int, int]]:
+        self._compute_dual_edges_to_delaunay_edges_mapping()
+        return self._dual_edges_to_delaunay_edges_mapping
+
     @staticmethod
     def _check_points_validity(points: NDArray[np.float_]) -> bool:
         return (
             points.ndim == 2 and points.shape[0] > 2 and points.shape[1] == 2
         )
 
     @staticmethod
@@ -232,14 +247,94 @@
     def compute_barycentric_dual(self) -> None:
         pass
 
     @abstractmethod
     def _compute_ridges_and_regions(self) -> None:
         pass
 
+    @abstractmethod
+    def _compute_dual_edges_to_delaunay_edges_mapping(self) -> None:
+        pass
+
+    # @staticmethod
+    # def _are_line_segments_within_rectangle(
+    #     min_x: float,
+    #     min_y: float,
+    #     max_x: float,
+    #     max_y: float,
+    #     line_segments: NDArray[np.float_],
+    # ) -> NDArray[np.bool_]:
+    #     """
+    #     Args:
+    #         line_segments: numpy array of shape (N, 2, 2), where N is the
+    #         number of line segments, the 1st "2" denotes the start and end
+    #         points of the each line segment and the 2nd "2" denotes the
+    #         (x, y) coordinates of the points.
+    #     """
+    #     bounds = np.array([[min_x, min_y], [max_x, max_y]])
+    #     return np.all(
+    #         (line_segments >= bounds[0]) & (line_segments <= bounds[1]),
+    #         axis=(1, 2),
+    #     )
+
+    def _compute_bounded_line_segments_of_dual(
+        self, dual: Literal["voronoi", "barycentric"]
+    ) -> NDArray[np.float_]:
+        if dual == "voronoi":
+            dual_vertices = self.voronoi_vertices
+        elif dual == "barycentric":
+            dual_vertices = self.barycentric_dual_vertices
+        else:
+            raise ValueError(
+                f"Unexpected value for dual: {dual}. Expected either 'voronoi' or 'barycentric'."
+            )
+        self._compute_ridges_and_regions()
+        ridge_vertices = np.array(self._ridge_vertices, dtype=np.int_)
+        mask = ridge_vertices[:, 1] == -1
+        target_indices = ridge_vertices[mask, 0]
+        target_vertices = dual_vertices[target_indices]
+        num_of_vertices = len(target_vertices)
+        min_x = self._bounding_box.min_x
+        min_y = self._bounding_box.min_y
+        max_x = self._bounding_box.max_x
+        max_y = self._bounding_box.max_y
+        candidates = np.empty((num_of_vertices, 4, 2), dtype=np.float_)
+        candidates[:, 0] = np.column_stack(
+            (target_vertices[:, 0], np.full(num_of_vertices, min_y))
+        )
+        candidates[:, 1] = np.column_stack(
+            (target_vertices[:, 0], np.full(num_of_vertices, max_y))
+        )
+        candidates[:, 2] = np.column_stack(
+            (np.full(num_of_vertices, min_x), target_vertices[:, 1])
+        )
+        candidates[:, 3] = np.column_stack(
+            (np.full(num_of_vertices, max_x), target_vertices[:, 1])
+        )
+        distances_between_targets_and_candidates = np.linalg.norm(
+            np.expand_dims(target_vertices, axis=1) - candidates, axis=2
+        )
+        chosen_candidates_index = np.argmin(
+            distances_between_targets_and_candidates, axis=1
+        )
+        chosen_candidates = candidates[
+            np.arange(num_of_vertices), chosen_candidates_index, :
+        ]
+        unbounded_line_segments = np.empty(
+            (len(ridge_vertices), 2, 2), dtype=np.float_
+        )
+        unbounded_line_segments[mask] = np.stack(
+            (target_vertices, chosen_candidates), axis=1
+        )
+        unbounded_line_segments[~mask] = dual_vertices[ridge_vertices[~mask]]
+        bounded_line_segments = self._bounding_box.clip_line_segments(
+            line_segments=unbounded_line_segments
+        )
+        return bounded_line_segments
+
     def get_mocked_scipy_spatial_delaunay(self) -> util.MockedDelaunay:
         """Get an object to be used as the argument in
         `scipy.spatial.delaunay_plot_2d`.
         """
         self.compute_delaunay_triangulation()
         return util.MockedDelaunay(
             points=self._points, simplices=self._triangles
@@ -426,16 +521,36 @@
                 else [triangle_indices[0], -1]
             )
         ridge_points = np.array(ridge_points)
 
         self._ridge_points = ridge_points
         self._ridge_vertices = ridge_vertices
         self._regions = regions
+        self._delaunay_edge_to_triangle_indices_mapping = dict(
+            delaunay_edge_to_triangle_indices_mapping
+        )
         self._ridges_and_regions_computed = True
 
+    def _compute_dual_edges_to_delaunay_edges_mapping(self) -> None:
+        self._compute_ridges_and_regions()
+        dual_edges_to_delaunay_edges_mapping = {}
+        for (
+            delaunay_edge,
+            triangle_indices,
+        ) in self._delaunay_edge_to_triangle_indices_mapping.items():
+            if len(triangle_indices) == 1:
+                continue
+            assert len(triangle_indices) == 2
+            dual_edges_to_delaunay_edges_mapping[
+                (triangle_indices[0], triangle_indices[1])
+            ] = delaunay_edge
+        self._dual_edges_to_delaunay_edges_mapping = (
+            dual_edges_to_delaunay_edges_mapping
+        )
+
     def compute_delaunay_triangulation(self) -> None:
         if self._delaunay_triangulation_computed:
             return
         delaunay_graph = scipy.spatial.Delaunay(points=self._points)
         triangles = delaunay_graph.simplices
         self._triangles = triangles
         self._delaunay_triangulation_computed = True
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py` & `delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py` & `delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO` & `delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay-triangulation-and-its-dual-2d
-Version: 0.1.2
+Version: 0.1.3
 License: MIT License
         
         Copyright (c) 2024 M.H. Luk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt` & `delaunay_triangulation_and_its_dual_2d-0.1.3/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,10 +14,13 @@
 delaunay_triangulation_and_its_dual_2d.egg-info/top_level.txt
 delaunay_triangulation_and_its_dual_2d/geometry/__init__.py
 delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py
 delaunay_triangulation_and_its_dual_2d/geometry/centroid.py
 delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py
 delaunay_triangulation_and_its_dual_2d/util/__init__.py
 delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py
+tests/delaunay/__init__.py
 tests/delaunay/performance.py
 tests/delaunay/profiling.py
-tests/delaunay/test_all.py
+tests/delaunay/test_all.py
+tests/delaunay/try.py
+tests/geometry/__init__.py
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/pyproject.toml` & `delaunay_triangulation_and_its_dual_2d-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/tests/delaunay/performance.py` & `delaunay_triangulation_and_its_dual_2d-0.1.3/tests/delaunay/performance.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.2/tests/delaunay/test_all.py` & `delaunay_triangulation_and_its_dual_2d-0.1.3/tests/delaunay/test_all.py`

 * *Files identical despite different names*

