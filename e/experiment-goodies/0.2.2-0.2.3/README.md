# Comparing `tmp/experiment_goodies-0.2.2.tar.gz` & `tmp/experiment_goodies-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment_goodies-0.2.2.tar", max compression
+gzip compressed data, was "experiment_goodies-0.2.3.tar", max compression
```

## Comparing `experiment_goodies-0.2.2.tar` & `experiment_goodies-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1172 2024-03-21 18:20:53.347022 experiment_goodies-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-03-21 12:43:40.830253 experiment_goodies-0.2.2/experiment_goodies/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 18:20:53.347022 experiment_goodies-0.2.2/experiment_goodies/geo/__init__.py
--rw-r--r--   0        0        0     9840 2024-05-03 20:03:01.570334 experiment_goodies-0.2.2/experiment_goodies/geo/raster.py
--rw-r--r--   0        0        0     5571 2024-03-21 18:20:53.347022 experiment_goodies-0.2.2/experiment_goodies/geo/vector.py
--rw-r--r--   0        0        0      268 2024-03-21 12:43:40.830253 experiment_goodies-0.2.2/experiment_goodies/logger/__init__.py
--rw-r--r--   0        0        0     4189 2024-04-10 14:47:21.255719 experiment_goodies-0.2.2/experiment_goodies/logger/experiment_logger.py
--rw-r--r--   0        0        0     5850 2024-03-21 12:43:40.830253 experiment_goodies-0.2.2/experiment_goodies/logger/rainbow_logger.py
--rw-r--r--   0        0        0     1101 2024-05-03 20:04:39.842826 experiment_goodies-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 experiment_goodies-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1172 2024-03-21 18:20:53.347022 experiment_goodies-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-21 12:43:40.830253 experiment_goodies-0.2.3/experiment_goodies/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:20:53.347022 experiment_goodies-0.2.3/experiment_goodies/geo/__init__.py
+-rw-r--r--   0        0        0     9864 2024-05-09 16:55:17.103927 experiment_goodies-0.2.3/experiment_goodies/geo/raster.py
+-rw-r--r--   0        0        0     6728 2024-05-09 16:55:17.103927 experiment_goodies-0.2.3/experiment_goodies/geo/vector.py
+-rw-r--r--   0        0        0      268 2024-03-21 12:43:40.830253 experiment_goodies-0.2.3/experiment_goodies/logger/__init__.py
+-rw-r--r--   0        0        0     4189 2024-04-10 14:47:21.255719 experiment_goodies-0.2.3/experiment_goodies/logger/experiment_logger.py
+-rw-r--r--   0        0        0     5850 2024-03-21 12:43:40.830253 experiment_goodies-0.2.3/experiment_goodies/logger/rainbow_logger.py
+-rw-r--r--   0        0        0     1123 2024-05-09 16:57:43.456064 experiment_goodies-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 experiment_goodies-0.2.3/PKG-INFO
```

### Comparing `experiment_goodies-0.2.2/README.md` & `experiment_goodies-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `experiment_goodies-0.2.2/experiment_goodies/geo/raster.py` & `experiment_goodies-0.2.3/experiment_goodies/geo/raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,8 +279,9 @@
     """
     polygons = []
     for geom, val in rasterio.features.shapes(mask, transform=transform):
         if val == 0:
             continue
         for g in geom["coordinates"]:
             polygons.append(Polygon(g))
-    return GeoSeries(polygons, crs=crs)
+    polygons = GeoSeries(polygons, crs=crs)
+    return polygons
```

### Comparing `experiment_goodies-0.2.2/experiment_goodies/geo/vector.py` & `experiment_goodies-0.2.3/experiment_goodies/geo/vector.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import math
 import random
 
 import geopandas
 import numpy as np
 import pandas as pd
+import shapely
 from geopandas import GeoDataFrame, GeoSeries
 from pyproj import Transformer
 from rasterio.features import rasterize
 from shapely import Geometry, affinity
 
 
 def load_geometries_from_paths(
@@ -145,14 +146,43 @@
             crs=4326,
         )
         tiles.append(group_tiles)
     tiles = pd.concat(tiles)
     return tiles
 
 
+def create_cell_grid(
+    bounds: tuple[float, float, float, float],
+    n_cells_x: int,
+    n_cells_y: int,
+    out_crs: str = "EPSG:4326",
+) -> geopandas.GeoDataFrame:
+    """Create a cell grid of size (n_cells_x,n_cells_y) within given bounds.
+
+    Args:
+        bounds (tuple[float, float, float, float]): bounds in which to create the grid in the format west, north, east, south
+        n_cells_x (int): number of cells in x direction
+        n_cells_y (int): number of cells in y direction
+        out_crs (_type_, optional): Output Coordinate Reference System. Defaults to "EPSG:4326".
+
+    Returns:
+        geopandas.GeoDataFrame: grid cell as a geodataframe
+    """
+    xmin, ymin, xmax, ymax = bounds
+    cell_size_x = (xmax - xmin) / n_cells_x
+    cell_size_y = (ymax - ymin) / n_cells_y
+    grid_cells = []
+    for x0 in np.arange(xmin, xmax, cell_size_x):
+        for y0 in np.arange(ymin, ymax, cell_size_y):
+            x1 = x0 - cell_size_x
+            y1 = y0 + cell_size_y
+            grid_cells.append(shapely.geometry.box(x0, y0, x1, y1))
+    return geopandas.GeoDataFrame(grid_cells, columns=["geometry"], crs=out_crs)
+
+
 def find_best_utm_code(lon: float, lat: float) -> str:
     """finds the best matching UTM code for given lat-long coordinates
 
     Args:
         lon (float): longitude
         lat (float): ñatitude
```

### Comparing `experiment_goodies-0.2.2/experiment_goodies/logger/experiment_logger.py` & `experiment_goodies-0.2.3/experiment_goodies/logger/experiment_logger.py`

 * *Files identical despite different names*

### Comparing `experiment_goodies-0.2.2/experiment_goodies/logger/rainbow_logger.py` & `experiment_goodies-0.2.3/experiment_goodies/logger/rainbow_logger.py`

 * *Files identical despite different names*

### Comparing `experiment_goodies-0.2.2/pyproject.toml` & `experiment_goodies-0.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "experiment-goodies"
-version = "0.2.2"
+version = "0.2.3"
 description = "Useful helpers, callbacks and more for experimenting with ml models"
 authors = ["Javier Smith <javier.smith.dlc@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 logutils = "^0.3.5"
@@ -17,14 +17,15 @@
 rio-cogeo = {version = "^5.2.0", optional = true}
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 dvc = {extras = ["s3"], version = "^3.48.4"}
 pre-commit = "^3.6.2"
+contextily = "^1.6.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
```

### Comparing `experiment_goodies-0.2.2/PKG-INFO` & `experiment_goodies-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-goodies
-Version: 0.2.2
+Version: 0.2.3
 Summary: Useful helpers, callbacks and more for experimenting with ml models
 Author: Javier Smith
 Author-email: javier.smith.dlc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

