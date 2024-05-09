# Comparing `tmp/geostructures-0.8.1.tar.gz` & `tmp/geostructures-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geostructures-0.8.1.tar", last modified: Mon Mar 25 16:05:19 2024, max compression
+gzip compressed data, was "geostructures-0.9.1.tar", last modified: Thu May  9 16:41:30 2024, max compression
```

## Comparing `geostructures-0.8.1.tar` & `geostructures-0.9.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:05:19.000722 geostructures-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-25 16:04:39.000000 geostructures-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-03-25 16:05:19.000722 geostructures-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-03-25 16:04:39.000000 geostructures-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:05:18.996722 geostructures-0.8.1/geostructures/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12902 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/calc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26143 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/geohash.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    59952 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:05:19.000722 geostructures-0.8.1/geostructures/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/utils/conditional_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/utils/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:05:19.000722 geostructures-0.8.1/geostructures/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-03-25 16:04:39.000000 geostructures-0.8.1/geostructures/visualization/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:05:19.000722 geostructures-0.8.1/geostructures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-03-25 16:05:18.000000 geostructures-0.8.1/geostructures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-25 16:05:18.000000 geostructures-0.8.1/geostructures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 16:05:18.000000 geostructures-0.8.1/geostructures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-25 16:05:18.000000 geostructures-0.8.1/geostructures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-25 16:05:18.000000 geostructures-0.8.1/geostructures.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 16:05:19.000722 geostructures-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-25 16:04:39.000000 geostructures-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:05:19.000722 geostructures-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-03-25 16:04:39.000000 geostructures-0.8.1/tests/test_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)    32638 2024-03-25 16:04:39.000000 geostructures-0.8.1/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-25 16:04:39.000000 geostructures-0.8.1/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-03-25 16:04:39.000000 geostructures-0.8.1/tests/test_geohash.py
--rw-r--r--   0 runner    (1001) docker     (127)    55496 2024-03-25 16:04:39.000000 geostructures-0.8.1/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-03-25 16:04:39.000000 geostructures-0.8.1/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:30.609830 geostructures-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 16:40:44.000000 geostructures-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-05-09 16:41:30.605830 geostructures-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-05-09 16:40:44.000000 geostructures-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:30.605830 geostructures-0.9.1/geostructures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17665 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26574 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21998 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/geohash.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    59686 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:30.605830 geostructures-0.9.1/geostructures/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/utils/agg_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/utils/conditional_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/utils/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:30.605830 geostructures-0.9.1/geostructures/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-05-09 16:40:44.000000 geostructures-0.9.1/geostructures/visualization/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:30.605830 geostructures-0.9.1/geostructures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-05-09 16:41:30.000000 geostructures-0.9.1/geostructures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-09 16:41:30.000000 geostructures-0.9.1/geostructures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:41:30.000000 geostructures-0.9.1/geostructures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 16:41:30.000000 geostructures-0.9.1/geostructures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 16:41:30.000000 geostructures-0.9.1/geostructures.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 16:41:30.609830 geostructures-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-09 16:40:44.000000 geostructures-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:30.605830 geostructures-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-09 16:40:44.000000 geostructures-0.9.1/tests/test_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32638 2024-05-09 16:40:44.000000 geostructures-0.9.1/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-09 16:40:44.000000 geostructures-0.9.1/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-09 16:40:44.000000 geostructures-0.9.1/tests/test_geohash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55539 2024-05-09 16:40:44.000000 geostructures-0.9.1/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-09 16:40:44.000000 geostructures-0.9.1/tests/test_time.py
```

### Comparing `geostructures-0.8.1/LICENSE` & `geostructures-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geostructures-0.8.1/PKG-INFO` & `geostructures-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geostructures
-Version: 0.8.1
+Version: 0.9.1
 Summary: A lightweight implementation of shapes drawn across a geo-temporal plane.
 Home-page: https://github.com/ccbest/geostructures
 Author: Carl Best
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `geostructures-0.8.1/README.md` & `geostructures-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `geostructures-0.8.1/geostructures/__init__.py` & `geostructures-0.9.1/geostructures/__init__.py`

 * *Files identical despite different names*

### Comparing `geostructures-0.8.1/geostructures/calc.py` & `geostructures-0.9.1/geostructures/calc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,115 @@
 """ Geometric calculations for Coordinates and Geostructures """
 
 __all__ = [
-    'bearing_degrees', 'ensure_edge_bounds', 'haversine_distance_meters',
-    'inverse_haversine_degrees', 'inverse_haversine_radians', 'rotate_coordinates',
-    'find_line_intersection', 'do_edges_intersect'
+    'bearing_degrees', 'dist_xyz_meters', 'circumscribing_circle_for_polygon',
+    'ensure_edge_bounds', 'haversine_distance_meters', 'inverse_haversine_degrees',
+    'inverse_haversine_radians', 'rotate_coordinates', 'find_line_intersection',
+    'do_edges_intersect'
 ]
 
 import math
-from typing import List, Optional, Set, Tuple
+import random
+from typing import cast, List, Optional, Set, Tuple
 
 import numpy as np
+from numpy.linalg import norm
 
 from geostructures.coordinates import Coordinate
 from geostructures.utils.functions import round_half_up
 
 
 _EARTH_RADIUS = 6_371_000  # meters - WGS84
 
 
+def _circumscribing_circle_for_triangle(
+    points: List[Coordinate]
+) -> Tuple[Optional[Coordinate], Optional[float]]:
+    """
+    Supporting function for circumscribing_circle_for_polygon().
+
+    Can be called with up to three points to return the center and radius of the
+    circumscribing circle.
+
+    Zero points returns None center and radius (will fail check in calling function).
+
+    One point returns itself as center and zero radius (will also fail check).
+
+    Two points returns the midpoint as center and half the distance as radius.
+
+    Three points checks every point pair as a possible diameter for the circle. If no
+    pair qualifies, uses the circumcenter formula from
+    https://brsr.github.io/2021/05/02/spherical-triangle-centers.html
+
+    Args:
+        points:
+            A list of Coordinates. Will error if more than three.
+
+    Returns:
+        (Coordinate, float) tuple of (Circumcenter, Radius in meters)
+
+    """
+    assert len(points) <= 3
+    if len(points) == 0:
+        return (None, None)
+    if len(points) == 1:
+        return (points[0], 0.0)
+    if len(points) == 2:
+        midp = [(v1+v2)/2 for v1, v2 in zip(points[0].xyz, points[1].xyz)]
+        midp_norm = norm(midp)
+        midp_coord = Coordinate._from_xyz([i/midp_norm for i in midp])
+        rad = dist_xyz_meters(midp_coord, points[0])
+        return (midp_coord, rad)
+
+    if not _test_counter_clockwise(points):
+        points = points[::-1]
+
+    # Test for trivial circle
+    for i in range(3):
+        p = points[i]
+        other_p = points[:i] + points[i+1:]
+        midp = [(v1+v2)/2 for v1, v2 in zip(other_p[0].xyz, other_p[1].xyz)]
+        midp_norm = norm(midp)
+        midp_coord = Coordinate._from_xyz([i/midp_norm for i in midp])
+        rad = dist_xyz_meters(midp_coord, other_p[0])
+        # If this is true, the midpoint of one side is the center
+        # (i.e. any obtuse/right triangle) and we are done
+        if rad >= dist_xyz_meters(midp_coord, p):
+            return (midp_coord, rad)
+
+    [a, b, c] = [p.xyz for p in points]
+    cc_num = np.cross(a, b) + np.cross(b, c) + np.cross(c, a)
+    cc_norm = norm(cc_num)
+    ctr = Coordinate._from_xyz([i/cc_norm for i in cc_num])
+    rad = math.acos(np.dot(a, np.cross(b, c))/cc_norm) * _EARTH_RADIUS
+    return (ctr, rad)
+
+
+def _test_counter_clockwise(bounds: List[Coordinate]) -> bool:
+    """
+    Tests a polygon to determine whether it's defined in a counterclockwise
+    (or mostly, for complex shapes) order.
+
+    Args:
+        bounds:
+            A list of Coordinates, in order
+
+    Returns:
+        bool
+    """
+    ans = sum(
+        (y.longitude - x.longitude) * (y.latitude + x.latitude)
+        for x, y in map(
+            lambda x: ensure_edge_bounds(x[0], x[1]),
+            zip(bounds, [*bounds[1:], bounds[0]])
+        )
+    )
+    return ans <= 0
+
+
 def bearing_degrees(coord1: Coordinate, coord2: Coordinate, **kwargs) -> float:
     """
     Calculate the bearing in degrees between lon1/lat1 and lon2/lat2
 
     Args:
         coord1:
             The start point Coordinate
@@ -47,14 +135,71 @@
     ) * math.cos(
         math.radians(d_lon)
     )
     bearing = (math.degrees(math.atan2(x_val, y_val)) + 360) % 360
     return round_half_up(bearing, kwargs.get('precision', 5))
 
 
+def circumscribing_circle_for_polygon(
+    all_points: List[Coordinate],
+    known_points: List[Coordinate]
+) -> Tuple[Optional[Coordinate], Optional[float]]:
+    """
+    Implements Welzl's algorithm to determine the circumscribing circle
+    for a set of points.
+
+    Args:
+        points:
+            A list of Coordinates. Will error if more than three.
+        known_points:
+            A list of Coordinates. Must be initialized with empty list.
+            Used by recursive calls after initialization.
+
+    Returns:
+        (Coordinate, float) tuple of (Circumcenter, Radius in meters)
+    """
+    if len(known_points) == 3:
+        return _circumscribing_circle_for_triangle(known_points)
+    if len(all_points) == 0:
+        return _circumscribing_circle_for_triangle(known_points)
+    i = random.randrange(0, len(all_points))
+    p = all_points[i]
+    other_p = all_points[:i] + all_points[i+1:]
+    ctr, rad = circumscribing_circle_for_polygon(
+        other_p,
+        known_points.copy()
+    )
+    if ctr is not None:
+        ctr = cast(Coordinate, ctr)
+        rad = cast(float, rad)
+        if rad >= dist_xyz_meters(p, ctr):
+            return (ctr, rad)
+    known_points.append(p)
+    return circumscribing_circle_for_polygon(other_p, known_points.copy())
+
+
+def dist_xyz_meters(coord1: Coordinate, coord2: Coordinate) -> float:
+    """
+    Great circle distance formula that works with the cached .xyz
+    property. Faster than haversine_distance_meters if each Coordinate
+    is used in distance calculations more than twice on average.
+
+    Args:
+        coord1:
+            A coordinate
+
+        coord2:
+            A second coordinate
+
+    Returns:
+        (float) the distance in meters
+    """
+    return math.acos(sum([an*bn for an, bn in zip(coord1.xyz, coord2.xyz)])) * _EARTH_RADIUS
+
+
 def do_edges_intersect(
     edges_a: List[Tuple[Coordinate, Coordinate]],
     edges_b: List[Tuple[Coordinate, Coordinate]],
 ) -> bool:
     """
     Tests whether two shape edges ever intersect. Uses the sweep line algorithm
     to minimize the number of intersections calculated.
```

### Comparing `geostructures-0.8.1/geostructures/collections.py` & `geostructures-0.9.1/geostructures/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,27 +159,42 @@
             raise ValueError('Malformed GeoJSON; expected FeatureCollection')
 
         shapes: List[GeoShape] = []
         for feature in gjson.get('features', []):
             geom_type = feature.get('geometry', {}).get('type')
             if geom_type == 'Point':
                 shapes.append(
-                    GeoPoint.from_geojson(feature, time_start_property, time_end_property)
+                    GeoPoint.from_geojson(
+                        feature,
+                        time_start_property,
+                        time_end_property,
+                        time_format=time_format
+                    )
                 )
                 continue
 
             if geom_type == 'LineString':
                 shapes.append(
-                    GeoLineString.from_geojson(feature, time_start_property, time_end_property)
+                    GeoLineString.from_geojson(
+                        feature,
+                        time_start_property,
+                        time_end_property,
+                        time_format=time_format
+                    )
                 )
                 continue
 
             if geom_type == 'Polygon':
                 shapes.append(
-                    GeoPolygon.from_geojson(feature, time_start_property, time_end_property)
+                    GeoPolygon.from_geojson(
+                        feature,
+                        time_start_property,
+                        time_end_property,
+                        time_format=time_format
+                    )
                 )
 
         return cls(shapes)
 
     @classmethod
     def from_geopandas(
         cls,
@@ -750,15 +765,15 @@
         # Currently only points are supported, so just average the lon/lats
         new_pings = []
         for _ts, ping_group in _timestamp_grouping.items():
             if len(ping_group) == 1:
                 new_pings.append(ping_group[0])
                 continue
 
-            _lons, _lats = list(zip(*[x.center.to_float() for x in ping_group]))
+            _lons, _lats = list(zip(*[x.centroid.to_float() for x in ping_group]))
             new_pings.append(
                 GeoPoint(
                     Coordinate(sum(_lons)/len(_lons), sum(_lats)/len(_lats)),
                     _ts
                 )
             )
```

### Comparing `geostructures-0.8.1/geostructures/coordinates.py` & `geostructures-0.9.1/geostructures/coordinates.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Representation of a specific point on earth
 """
 
 __all__ = ['Coordinate']
 
-from typing import Tuple, Union
+from functools import cached_property
+import math
+from typing import List, Tuple, Union
 
 from geostructures.utils.functions import round_half_up
 
 
 class Coordinate:
     """Representation of a coordinate on the globe (i.e., a lon/lat pair)"""
 
@@ -44,14 +46,32 @@
 
     def __hash__(self):
         return hash((self.longitude, self.latitude))
 
     def __repr__(self):
         return f'<Coordinate({self.longitude}, {self.latitude})>'
 
+    @cached_property
+    def xyz(self):
+        """Converts lat/lon to unit coordinates [x,y,z]"""
+        r_lat = math.radians(self.latitude)
+        r_lon = math.radians(self.longitude)
+        return [
+            math.cos(r_lat) * math.cos(r_lon),
+            math.cos(r_lat) * math.sin(r_lon),
+            math.sin(r_lat)
+        ]
+
+    @classmethod
+    def _from_xyz(cls, xyz: List[float]):
+        assert len(xyz) == 3
+        latitude = math.asin(xyz[2])
+        longitude = math.atan2(xyz[1], xyz[0])
+        return Coordinate(math.degrees(longitude), math.degrees(latitude))
+
     @classmethod
     def from_dms(cls, lon: Tuple[int, int, float, str], lat: Tuple[int, int, float, str]):
         """
         Creates a Coordinate from a Degree Minutes Seconds (lon, lat) pair.
 
         The quadrant value should consist of either 'E'/'W' (longitude) or 'N'/'S' (latitude)
```

### Comparing `geostructures-0.8.1/geostructures/geohash.py` & `geostructures-0.9.1/geostructures/geohash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """
 Module for geohash transformers
 """
 
+
 __all__ = [
     'H3Hasher', 'HasherBase', 'NiemeyerHasher',
-    'niemeyer_to_geobox'
+    'niemeyer_to_geobox', 'convert_hashmap'
 ]
 
+
 import abc
 from collections import defaultdict
 from typing import Any, Dict, List, Optional, Sequence, Set, Tuple, TypedDict
 
-from geostructures import Coordinate, GeoBox, GeoLineString, GeoPoint
+from geostructures import Coordinate, GeoBox, GeoLineString, GeoPoint, GeoPolygon
 from geostructures.structures import GeoShape
-from geostructures.collections import ShapeCollection
+from geostructures.collections import FeatureCollection, ShapeCollection
 from geostructures.calc import find_line_intersection
+from geostructures.utils.functions import round_half_up
+from h3 import h3_to_geo_boundary
 
 
 _NIEMEYER_CONFIG_TYPE = TypedDict(
     '_NIEMEYER_CONFIG_TYPE',
     {
         'bits': Tuple,
         'charset': str,
@@ -664,7 +668,31 @@
         if isinstance(shape, GeoPoint):
             return self._hash_point(shape.centroid)
 
         if isinstance(shape, GeoLineString):
             return self._hash_linestring(shape)
 
         return self._hash_polygon(shape)
+
+
+def convert_hashmap(hexmap: Dict[str, float]):
+    """
+    Converts an H3 hashmap into a geostructure FeatureCollection
+
+    Args:
+        hexmap:
+            A dictionary of h3 hexagon ids to their corresponding weights.
+    """
+    polygon_hex_list: List[GeoShape] = []
+    for hex in hexmap:
+        coordList = []
+        points = []
+        coordList = h3_to_geo_boundary(hex, geo_json=True)
+        points = [Coordinate(round_half_up(coord[0], 8), round_half_up(coord[1], 8)) for coord in coordList]
+        if isinstance(hexmap, dict):
+            polgon_hex = GeoPolygon(points, properties={'weight': hexmap.get(hex)})
+        else:
+            polgon_hex = GeoPolygon(points)
+
+        polygon_hex_list.append(polgon_hex)
+
+    return FeatureCollection(polygon_hex_list)
```

### Comparing `geostructures-0.8.1/geostructures/structures.py` & `geostructures-0.9.1/geostructures/structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from typing import cast, Any, Dict, List, Optional, Tuple, TypeVar, Union
 
 import numpy as np
 
 from geostructures import LOGGER
 from geostructures.coordinates import Coordinate
 from geostructures.calc import (
-    ensure_edge_bounds,
+    _test_counter_clockwise,
+    circumscribing_circle_for_polygon,
     inverse_haversine_radians,
     inverse_haversine_degrees,
     haversine_distance_meters,
     bearing_degrees,
     find_line_intersection,
     do_edges_intersect
 )
@@ -366,16 +367,28 @@
                 For shapes with smooth curves, increasing k increases the number of
                 points generated along the curve
 
         Returns:
             bool
         """
 
+        bbox_tested = False
+        if kwargs.get('k', 0) > 4:
+            if self.contains_shape(shape.circumscribing_rectangle()):
+                return True
+            else:
+                bbox_tested = True
+
         s_edges = self.edges(**kwargs)
         o_edges = shape.edges(**kwargs)
+
+        if not bbox_tested and len(o_edges) > 4:
+            if self.contains_shape(shape.circumscribing_rectangle()):
+                return True
+
         if do_edges_intersect(
             [x for edge_ring in s_edges for x in edge_ring],
             [x for edge_ring in o_edges for x in edge_ring]
         ):
             # At least one edge pair intersects - cannot be contained
             return False
 
@@ -666,15 +679,15 @@
         if not outline[0] == outline[-1]:
             LOGGER.warning(
                 'Polygon outlines must be self-closing; your final point will be '
                 'connected to your starting point.'
             )
             outline = [*outline, outline[0]]
 
-        if not self._test_counter_clockwise(outline) ^ _is_hole:
+        if not _test_counter_clockwise(outline) ^ _is_hole:
             self.warn_once(
                 'Polygon violates the right hand rule. Inverting coordinate '
                 'order; this warning will not repeat.'
             )
             outline = outline[::-1]
 
         self.outline = outline
@@ -789,45 +802,20 @@
 
             if include_boundary or not intersection[1]:
                 # If boundaries are allowed, or is not a boundary intersection
                 _intersections += 1
 
         return _intersections > 0 and _intersections % 2 != 0
 
-    @staticmethod
-    def _test_counter_clockwise(bounds: List[Coordinate]) -> bool:
-        """
-        Tests a polygon to determine whether it's defined in a counterclockwise
-        (or mostly, for complex shapes) order.
-
-        Args:
-            bounds:
-                A list of Coordinates, in order
-
-        Returns:
-            bool
-        """
-        ans = sum(
-            (y.longitude - x.longitude) * (y.latitude + x.latitude)
-            for x, y in map(
-                lambda x: ensure_edge_bounds(x[0], x[1]),
-                zip(bounds, [*bounds[1:], bounds[0]])
-            )
-        )
-        return ans <= 0
-
     def bounding_coords(self, **kwargs) -> List[Coordinate]:
         return self.outline
 
     def circumscribing_circle(self) -> 'GeoCircle':
-        centroid = self.centroid
-        max_dist = max(
-            haversine_distance_meters(x, centroid) for x in self.outline[:-1]
-        )
-        return GeoCircle(centroid, max_dist, dt=self.dt)
+        ctr, rad = circumscribing_circle_for_polygon(self.outline[:-1], [])
+        return GeoCircle(cast(Coordinate, ctr), cast(float, rad), dt=self.dt)
 
     def contains_coordinate(self, coord: Coordinate) -> bool:
         # First see if the point even falls inside the circumscribing rectangle
         lon_bounds, lat_bounds = self.bounds
         if not (
             lon_bounds[0] <= coord.longitude <= lon_bounds[1] and
             lat_bounds[0] <= coord.latitude <= lat_bounds[1]
@@ -1162,81 +1150,81 @@
 
 
 class GeoEllipse(GeoShape):
 
     """
     An ellipsoid shape (or oval), represented by:
         * a Coordinate center
-        * a major axis (the radius at its greatest value)
-        * a minor axis (the radius at its least value)
+        * a semi major axis (the radius at its greatest value)
+        * a semi minor axis (the radius at its least value)
         * rotation (the major axis's degree offset from North)
 
     Args:
         center: (Coordinate)
             The centroid of the ellipse
 
-        major_axis: (float)
+        semi_major: (float)
             The maximum radius value
 
-        minor_axis: (float)
+        semi_minor: (float)
             The minimum radius value
 
         rotation: (float)
             The major axis's degree offset from North (expressed as East of North)
 
     """
 
     def __init__(  # pylint: disable=R0913
         self,
         center: Coordinate,
-        major_axis: float,
-        minor_axis: float,
+        semi_major: float,
+        semi_minor: float,
         rotation: float,
         holes: Optional[List[GeoShape]] = None,
         dt: Optional[_GEOTIME_TYPE] = None,
         properties: Optional[Dict] = None,
     ):
         super().__init__(holes=holes, dt=dt, properties=properties)
 
         self.center = center
-        self.major_axis = major_axis
-        self.minor_axis = minor_axis
+        self.semi_major = semi_major
+        self.semi_minor = semi_minor
         self.rotation = rotation
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, GeoEllipse):
             return False
 
         return (
             self.center == other.center
-            and self.major_axis == other.major_axis
-            and self.minor_axis == other.minor_axis
+            and self.semi_major == other.semi_major
+            and self.semi_minor == other.semi_minor
             and self.rotation == other.rotation
             and self.dt == other.dt
         )
 
     def __hash__(self) -> int:
         return hash(
-            (self.centroid, self.minor_axis, self.major_axis, self.rotation, self.dt)
+            (self.centroid, self.semi_minor, self.semi_major, self.rotation, self.dt)
         )
 
     def __repr__(self) -> str:
         return (
             f'<GeoEllipse at {self.center.to_float()}; '
-            f'radius {self.major_axis}/{self.minor_axis}; '
+            f'radius {self.semi_major}/{self.semi_minor}; '
             f'rotation {self.rotation}>'
         )
 
     @cached_property
     def bounds(self) -> Tuple[Tuple[float, float], Tuple[float, float]]:
         rot_rad = math.radians(self.rotation)
         cos_rot_sq = math.cos(rot_rad)**2
         sin_rot_sq = math.sin(rot_rad)**2
-        semi_major_sq = (self.major_axis)**2
-        semi_minor_sq = (self.minor_axis)**2
+        semi_major_sq = (self.semi_major)**2
+        semi_minor_sq = (self.semi_minor)**2
 
         dx = math.sqrt(semi_major_sq * sin_rot_sq + semi_minor_sq * cos_rot_sq)
         dy = math.sqrt(semi_major_sq * cos_rot_sq + semi_minor_sq * sin_rot_sq)
 
         _, max_lat = inverse_haversine_degrees(self.centroid, 0, dy).to_float()
         max_lon, _ = inverse_haversine_degrees(self.centroid, 90, dx).to_float()
         _, min_lat = inverse_haversine_degrees(self.centroid, 180, dy).to_float()
@@ -1256,39 +1244,39 @@
             angle:
                 The angle of direction from the ellipse center
 
         Returns:
             float
         """
         return (
-            self.major_axis
-            * self.minor_axis
+            self.semi_major
+            * self.semi_minor
             / math.sqrt(
-                (self.major_axis**2) * (math.sin(angle) ** 2)
-                + (self.minor_axis**2) * (math.cos(angle) ** 2)
+                (self.semi_major**2) * (math.sin(angle) ** 2)
+                + (self.semi_minor**2) * (math.cos(angle) ** 2)
             )
         )
 
     def bounding_coords(self, **kwargs) -> List[Coordinate]:
-        k = kwargs.get('k') or math.ceil(36 * self.major_axis / self.minor_axis)
+        k = kwargs.get('k') or math.ceil(36 * self.semi_major / self.semi_minor)
         coords = []
         rotation = math.radians(self.rotation)
 
         for i in range(k, -1, -1):
             angle = (math.pi * 2 / k) * i
             radius = self._radius_at_angle(angle)
             coord = inverse_haversine_radians(
                 self.center, angle + rotation, radius
             )
             coords.append(coord)
 
         return coords
 
     def circumscribing_circle(self) -> GeoCircle:
-        return GeoCircle(self.center, self.major_axis, dt=self.dt)
+        return GeoCircle(self.center, self.semi_major, dt=self.dt)
 
     def contains_coordinate(self, coord: Coordinate) -> bool:
         bearing = bearing_degrees(self.center, coord)
         radius = self._radius_at_angle(math.radians(bearing - self.rotation))
         if not haversine_distance_meters(self.center, coord) <= radius:
             return False
 
@@ -1297,16 +1285,16 @@
                 return False
 
         return True
 
     def copy(self) -> 'GeoEllipse':
         return GeoEllipse(
             self.center,
-            self.major_axis,
-            self.minor_axis,
+            self.semi_major,
+            self.semi_minor,
             self.rotation,
             holes=self.holes.copy(),
             dt=self.dt.copy() if self.dt else None,
             properties=copy.deepcopy(self._properties)
         )
 
     def to_polygon(self, **kwargs) -> GeoPolygon:
```

### Comparing `geostructures-0.8.1/geostructures/time.py` & `geostructures-0.9.1/geostructures/time.py`

 * *Files identical despite different names*

### Comparing `geostructures-0.8.1/geostructures/utils/conditional_imports.py` & `geostructures-0.9.1/geostructures/utils/conditional_imports.py`

 * *Files identical despite different names*

### Comparing `geostructures-0.8.1/geostructures/utils/mixins.py` & `geostructures-0.9.1/geostructures/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `geostructures-0.8.1/geostructures/visualization/plotly.py` & `geostructures-0.9.1/geostructures/visualization/plotly.py`

 * *Files identical despite different names*

### Comparing `geostructures-0.8.1/geostructures.egg-info/PKG-INFO` & `geostructures-0.9.1/geostructures.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geostructures
-Version: 0.8.1
+Version: 0.9.1
 Summary: A lightweight implementation of shapes drawn across a geo-temporal plane.
 Home-page: https://github.com/ccbest/geostructures
 Author: Carl Best
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `geostructures-0.8.1/geostructures.egg-info/SOURCES.txt` & `geostructures-0.9.1/geostructures.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 geostructures/time.py
 geostructures.egg-info/PKG-INFO
 geostructures.egg-info/SOURCES.txt
 geostructures.egg-info/dependency_links.txt
 geostructures.egg-info/requires.txt
 geostructures.egg-info/top_level.txt
 geostructures/utils/__init__.py
+geostructures/utils/agg_functions.py
 geostructures/utils/conditional_imports.py
 geostructures/utils/functions.py
 geostructures/utils/logging.py
 geostructures/utils/mixins.py
 geostructures/visualization/__init__.py
 geostructures/visualization/plotly.py
 tests/test_calc.py
```

### Comparing `geostructures-0.8.1/setup.py` & `geostructures-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `geostructures-0.8.1/tests/test_calc.py` & `geostructures-0.9.1/tests/test_calc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,45 @@
 
 import math
 
 from geostructures.calc import *
 from geostructures.coordinates import Coordinate
+from geostructures.utils.functions import round_half_up
 
 
 def test_bearing_degrees():
     assert bearing_degrees(Coordinate(0.0, 0.0), Coordinate(0.001, 0.001)) == 45.
     assert bearing_degrees(Coordinate(0.0, 0.0), Coordinate(0.001, 0.001), precision=9) == 44.999999996
 
+def test_circumscribing_circle_for_polygon():
+    points =[
+        Coordinate(0,5),
+        Coordinate(0,0),
+        Coordinate(2,1),
+        Coordinate(4,3)
+    ]
+    cc = circumscribing_circle_for_polygon(points, [])
+    assert round_half_up(cc[0].latitude, 6) == 2.499407
+    assert round_half_up(cc[0].longitude, 6) == 1.248383
+    assert round_half_up(cc[1], 0) == 310640
+
+def test_dist_xyz_meters():
+    # Sourced from haversine package
+    actual_dist_meters = 157.25359
+    calc_dist = dist_xyz_meters(Coordinate(0.0, 0.0), Coordinate(0.001, 0.001))
+    assert round(actual_dist_meters) == round(calc_dist)
+
+    actual_dist_meters = 157_249.59847
+    calc_dist = dist_xyz_meters(Coordinate(0.0, 0.0), Coordinate(1.0, 1.0))
+    assert abs(round(actual_dist_meters) - round(calc_dist)) < 2
+
+    # Antimeridian test
+    actual_dist_meters = 222390
+    calc_dist = dist_xyz_meters(Coordinate(179., 0.), Coordinate(-179., 0.))
+    assert round(calc_dist) == actual_dist_meters
 
 def test_do_edges_intersect():
     edge_a = [
         (Coordinate(179, -1), Coordinate(-179, 1)),
     ]
     edge_b = [
         (Coordinate(178, -1), Coordinate(-178, 1))
```

### Comparing `geostructures-0.8.1/tests/test_collections.py` & `geostructures-0.9.1/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `geostructures-0.8.1/tests/test_coordinates.py` & `geostructures-0.9.1/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `geostructures-0.8.1/tests/test_geohash.py` & `geostructures-0.9.1/tests/test_geohash.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 
 import pytest
+from datetime import datetime
 
-from geostructures import Coordinate, GeoBox, GeoCircle, GeoLineString, GeoPoint
+from geostructures import Coordinate, GeoBox, GeoCircle, GeoLineString, GeoPoint, GeoPolygon
 from geostructures.collections import FeatureCollection
 from geostructures.geohash import (
     _coord_to_niemeyer, _get_niemeyer_subhashes, niemeyer_to_geobox,
-    H3Hasher, NiemeyerHasher
+    H3Hasher, NiemeyerHasher, convert_hashmap
 )
+from geostructures.time import TimeInterval
+from geostructures.utils.agg_functions import *
 
 
 def test_coord_to_niemeyer():
     coord = Coordinate(0.1, -0.1)
     assert _coord_to_niemeyer(coord, 8, 16) == '95555659'
 
     with pytest.raises(ValueError):
@@ -117,14 +120,62 @@
     }
 
     with pytest.raises(ValueError):
         hasher = H3Hasher()
         hasher.hash_collection(fcol)
 
 
+def test_hash_collection_with_total_time():
+    shape = GeoCircle(Coordinate(0.0, 0.0), 600, 
+                      dt=TimeInterval(datetime(2024,1,1), datetime(2024,1,1,1)))
+    shape2 = GeoCircle(Coordinate(0.0, 0.0), 300,
+                      dt=TimeInterval(datetime(2024,1,1), datetime(2024,1,1,2)))
+    fcol = FeatureCollection([shape, shape2])
+    hasher = H3Hasher(resolution=9)
+
+    assert hasher.hash_collection(fcol, agg_fn=total_time) == {
+        '89754e64d2fffff': 10800.0,
+        '89754e64d2bffff': 3600.0,
+        '89754e64983ffff': 3600.0,
+        '89754e64987ffff': 3600.0,
+        '89754e64993ffff': 10800.0,
+        '89754e64997ffff': 10800.0,
+        '89754e64d27ffff': 3600.0,
+        '89754e64d67ffff': 3600.0,
+        '89754a9324bffff': 3600.0,
+        '89754e64d23ffff': 3600.0,
+        '89754a9325bffff': 3600.0,
+        '89754e6499bffff': 3600.0
+    }
+
+def test_hash_collection_with_unique_entities():
+    shape = GeoCircle(Coordinate(0.0, 0.0), 600, 
+                      properties={'entity': 1})
+    shape2 = GeoCircle(Coordinate(0.0, 0.0), 300,
+                      properties={'entity': 2})
+    shape3 = GeoCircle(Coordinate(0.0, 0.0), 450,
+                      properties={'entity': 1})
+    fcol = FeatureCollection([shape, shape2, shape3])
+    hasher = H3Hasher(resolution=9)
+
+    assert hasher.hash_collection(fcol, agg_fn=unique_entities) == {
+        '89754e64d2fffff': 2,
+        '89754e64d2bffff': 1,
+        '89754e64983ffff': 1,
+        '89754e64987ffff': 1,
+        '89754e64993ffff': 2,
+        '89754e64997ffff': 2,
+        '89754e64d27ffff': 1,
+        '89754e64d67ffff': 1,
+        '89754a9324bffff': 1,
+        '89754e64d23ffff': 1,
+        '89754a9325bffff': 1,
+        '89754e6499bffff': 1
+    }
+
 def test_niemeyer_hash_collection():
     hasher = NiemeyerHasher(8, 16)
     col = FeatureCollection([
         GeoCircle(Coordinate(0.0, 0.0), 700),
         GeoPoint(Coordinate(0.0, 0.0)),
         GeoLineString([Coordinate(0.0, 0.0), Coordinate(0.02, 0.03), Coordinate(0.04, 0.0)])
     ])
@@ -189,10 +240,24 @@
     assert hasher.hash_shape(shape) == {
         '3fffffff', '6aaaaaaa', '95555555', '9555557f', 'c0000000', 'c0000001',
         'c0000003', 'c0000006', 'c0000007', 'c000000c', 'c000000d', 'c0000018',
         'c000001a', 'c000001b', 'c0000023', 'c0000025', 'c0000026', 'c0000027',
         'c0000028', 'c0000029', 'c000002a', 'c0000030'
     }
 
+
     # test that small shapes still produce a single geohash
     shape = GeoCircle(Coordinate(0.0001, 0.0001), 5)
     assert hasher.hash_shape(shape) == {'c0000000'}
+
+
+def test_convert_hashmap():
+    testhashmap={'87195da49ffffff'}
+    polygon = GeoPolygon(
+    [
+        Coordinate(-0.14556039, 51.52194368), Coordinate(-0.16020368, 51.51507904), 
+        Coordinate(-0.15716008, 51.50284849), Coordinate(-0.13948088, 51.49748360),
+        Coordinate(-0.12484221, 51.50434724), Coordinate(-0.12787812, 51.51657678),
+        Coordinate(-0.14556039, 51.52194368) 
+    ]
+)
+    assert convert_hashmap(testhashmap) == FeatureCollection([polygon])
```

### Comparing `geostructures-0.8.1/tests/test_structures.py` & `geostructures-0.9.1/tests/test_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -637,19 +637,18 @@
 
 
 def test_polygon_to_geojson(geopolygon):
     shapely.geometry.shape(geopolygon.to_geojson()['geometry'])
 
 
 def test_geopolygon_circumscribing_circle(geopolygon):
-    assert geopolygon.circumscribing_circle() == GeoCircle(
-        center=Coordinate(0.5, 0.5),
-        radius=78626.18767687456,
-        dt=default_test_datetime
-    )
+    gc = geopolygon.circumscribing_circle()
+    assert round_half_up(gc.center.latitude, 4) == 0.5
+    assert round_half_up(gc.center.longitude, 4) == 0.5
+    assert round_half_up(gc.radius, 0) == 78625
 
 
 def test_geopolygon_circumscribing_rectangle(geopolygon):
     assert geopolygon.circumscribing_rectangle() == GeoBox(
         Coordinate(0.0, 1.0),
         Coordinate(1.0, 0.0),
         dt=default_test_datetime
@@ -1073,16 +1072,16 @@
         Coordinate(0.0089932, -0.0044966),
         dt=default_test_datetime
     )
 
 
 def test_geoellipse_circumscribing_circle(geoellipse):
     assert geoellipse.circumscribing_circle() == GeoCircle(
-        geoellipse.center,
-        geoellipse.major_axis,
+        geoellipse.centroid,
+        geoellipse.semi_major,
         dt=default_test_datetime
     )
 
 
 def test_geoellipse_centroid(geoellipse):
     assert geoellipse.centroid == geoellipse.center
 
@@ -1195,18 +1194,18 @@
 
 def test_georing_to_geojson(georing):
     shapely.geometry.shape(georing.to_geojson()['geometry'])
 
 
 def test_georing_circumscribing_rectangle(georing, geowedge):
 
-    max_lon, _ = inverse_haversine_degrees(georing.center, 90, 1000).to_float()
-    min_lon, _ = inverse_haversine_degrees(georing.center, -90, 1000).to_float()
-    _, max_lat = inverse_haversine_degrees(georing.center, 0, 1000).to_float()
-    _, min_lat = inverse_haversine_degrees(georing.center, 180, 1000).to_float()
+    max_lon, _ = inverse_haversine_degrees(georing.centroid, 90, 1000).to_float()
+    min_lon, _ = inverse_haversine_degrees(georing.centroid, -90, 1000).to_float()
+    _, max_lat = inverse_haversine_degrees(georing.centroid, 0, 1000).to_float()
+    _, min_lat = inverse_haversine_degrees(georing.centroid, 180, 1000).to_float()
 
     assert georing.circumscribing_rectangle() == GeoBox(
         Coordinate(min_lon, max_lat),
         Coordinate(max_lon, min_lat),
         dt=default_test_datetime
     )
```

### Comparing `geostructures-0.8.1/tests/test_time.py` & `geostructures-0.9.1/tests/test_time.py`

 * *Files identical despite different names*

