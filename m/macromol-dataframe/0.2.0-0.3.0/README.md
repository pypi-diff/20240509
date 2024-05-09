# Comparing `tmp/macromol_dataframe-0.2.0.tar.gz` & `tmp/macromol_dataframe-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macromol_dataframe-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "macromol_dataframe-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `macromol_dataframe-0.2.0.tar` & `macromol_dataframe-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3977 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/README.md
--rw-r--r--   0        0        0      199 2024-05-01 20:08:43.874938 macromol_dataframe-0.2.0/macromol_dataframe/__init__.py
--rw-r--r--   0        0        0     2389 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/macromol_dataframe/atoms.py
--rw-r--r--   0        0        0     4460 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/macromol_dataframe/coords.py
--rw-r--r--   0        0        0      953 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/macromol_dataframe/error.py
--rw-r--r--   0        0        0    20127 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/macromol_dataframe/mmcif.py
--rw-r--r--   0        0        0     1017 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/macromol_dataframe/pymol.py
--rw-r--r--   0        0        0     7009 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/macromol_dataframe/testing.py
--rw-r--r--   0        0        0     1617 2024-05-01 20:08:43.102941 macromol_dataframe-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5118 1970-01-01 00:00:00.000000 macromol_dataframe-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3977 2024-05-09 15:19:56.937484 macromol_dataframe-0.3.0/README.md
+-rw-r--r--   0        0        0      199 2024-05-09 15:19:57.689485 macromol_dataframe-0.3.0/macromol_dataframe/__init__.py
+-rw-r--r--   0        0        0     2389 2024-05-09 15:19:56.937484 macromol_dataframe-0.3.0/macromol_dataframe/atoms.py
+-rw-r--r--   0        0        0     5121 2024-05-09 15:19:56.937484 macromol_dataframe-0.3.0/macromol_dataframe/coords.py
+-rw-r--r--   0        0        0      953 2024-05-09 15:19:56.937484 macromol_dataframe-0.3.0/macromol_dataframe/error.py
+-rw-r--r--   0        0        0    20127 2024-05-09 15:19:56.937484 macromol_dataframe-0.3.0/macromol_dataframe/mmcif.py
+-rw-r--r--   0        0        0     1017 2024-05-09 15:19:56.937484 macromol_dataframe-0.3.0/macromol_dataframe/pymol.py
+-rw-r--r--   0        0        0     7051 2024-05-09 15:19:56.937484 macromol_dataframe-0.3.0/macromol_dataframe/testing.py
+-rw-r--r--   0        0        0     1617 2024-05-09 15:19:56.937484 macromol_dataframe-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5118 1970-01-01 00:00:00.000000 macromol_dataframe-0.3.0/PKG-INFO
```

### Comparing `macromol_dataframe-0.2.0/README.md` & `macromol_dataframe-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `macromol_dataframe-0.2.0/macromol_dataframe/atoms.py` & `macromol_dataframe-0.3.0/macromol_dataframe/atoms.py`

 * *Files identical despite different names*

### Comparing `macromol_dataframe-0.2.0/macromol_dataframe/coords.py` & `macromol_dataframe-0.3.0/macromol_dataframe/coords.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from scipy.spatial.transform import Rotation
 from numpy.typing import NDArray
-from typing import TypeAlias, Annotated
+from typing import TypeAlias, Annotated, Optional
 
 """\
 Naming conventions
 ==================
 When it's possibly unclear, a suffix should be used to indicate:
 
 - Which coordinate frame a coordinate belongs to.
@@ -34,19 +34,37 @@
     >>> coords_y = transform_coords(coords_x, frame_xy)
 
 We start with a coordinate in frame "X", apply a transformation matrix that 
 goes from "X" to "Y", and end up with a coordinate in frame "Y".
 """
 
 Coord: TypeAlias = Annotated[NDArray[float], (3)]
+Coord3: TypeAlias = Annotated[NDArray[float], (3)]
+Coord4: TypeAlias = Annotated[NDArray[float], (4)]
+Coords: TypeAlias = Annotated[NDArray[float], (-1, 3)]
 Coords3: TypeAlias = Annotated[NDArray[float], (-1, 3)]
 Coords4: TypeAlias = Annotated[NDArray[float], (-1, 4)]
+Matrix33: TypeAlias = Annotated[NDArray[float], (3, 3)]
 Frame: TypeAlias = Annotated[NDArray[float], (4, 4)]
 
-def make_coord_frame(origin: Coord, rot_vec_rad: Coord) -> Frame:
+def make_coord_frame(
+        origin: Coord,
+        rotation: Optional[Rotation] = None,
+) -> Frame:
+    if rotation is None:
+        rot_mat = np.eye(3)
+    else:
+        rot_mat = rotation.as_matrix()
+
+    return make_coord_frame_from_rotation_matrix(origin, rot_mat)
+
+def make_coord_frame_from_rotation_vector(
+        origin: Coord,
+        rot_vec_rad: Coord,
+) -> Frame:
     """\
     Provide a convenient way to construct coordinate frame matrices.
 
     For the purposes of describing how exactly this function works, let us 
     define that the matrix returned by this function will transform coordinates 
     from a coordinate frame labeled "X" to one labeled "Y".
 
@@ -68,21 +86,25 @@
             For example, consider a frame Y that is rotated 90° around the 
             z-axis relative to frame X.  If you transform (1,0,0), you'll get 
             (0,-1,0).  Note that if we looked at these two coordinates in the 
             same frame, the second would appear to be a -90° rotation or the 
             first.  This happens because it's the *coordinate frame* that's 
             being rotated by 90°, not the coordinates themselves.
     """
-    assert origin.size == 3
-    assert rot_vec_rad.size == 3
+    return make_coord_frame(origin, Rotation.from_rotvec(rot_vec_rad))
 
-    rot = Rotation.from_rotvec(rot_vec_rad).as_matrix()
+def make_coord_frame_from_rotation_matrix(
+        origin: Coord,
+        rot_matrix: Matrix33,
+):
+    assert origin.size == 3
+    assert rot_matrix.shape == (3, 3)
 
     frame_yx = np.eye(4)
-    frame_yx[0:3, 0:3] = rot
+    frame_yx[0:3, 0:3] = rot_matrix
     frame_yx[0:3,   3] = origin.ravel()
 
     # We need to invert the matrix, because the arguments are both from the 
     # perspective of frame X, but the actual components of the matrix have to 
     # be from the perspective of frame Y.
 
     return invert_coord_frame(frame_yx)
```

### Comparing `macromol_dataframe-0.2.0/macromol_dataframe/error.py` & `macromol_dataframe-0.3.0/macromol_dataframe/error.py`

 * *Files identical despite different names*

### Comparing `macromol_dataframe-0.2.0/macromol_dataframe/mmcif.py` & `macromol_dataframe-0.3.0/macromol_dataframe/mmcif.py`

 * *Files identical despite different names*

### Comparing `macromol_dataframe-0.2.0/macromol_dataframe/pymol.py` & `macromol_dataframe-0.3.0/macromol_dataframe/pymol.py`

 * *Files identical despite different names*

### Comparing `macromol_dataframe-0.2.0/macromol_dataframe/testing.py` & `macromol_dataframe-0.3.0/macromol_dataframe/testing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import polars as pl
 import numpy as np
 import math
 
-from .coords import make_coord_frame
+from .coords import make_coord_frame_from_rotation_vector
 from .error import TidyError
 from io import StringIO
 from functools import partial
 
 NOT_GIVEN = object()
 
 def matrix(params):
@@ -15,15 +15,15 @@
 
 def vector(params):
     return np.array([eval(x, math.__dict__) for x in params.split()])
 
 def frame(params):
     origin = coord(params['origin'])
     rot_vec_rad = vector(params['rot_vec_rad'])
-    return make_coord_frame(origin, rot_vec_rad)
+    return make_coord_frame_from_rotation_vector(origin, rot_vec_rad)
 
 def frames(params):
     return [frame(x) for x in params]
 
 def coord(params):
     return matrix(params)
```

### Comparing `macromol_dataframe-0.2.0/pyproject.toml` & `macromol_dataframe-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `macromol_dataframe-0.2.0/PKG-INFO` & `macromol_dataframe-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macromol_dataframe
-Version: 0.2.0
+Version: 0.3.0
 Summary: Manipulate macromolecular coordinate data using data frames.
 Author-email: Kale Kundert <kale@thekunderts.net>
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: gemmi
 Requires-Dist: numpy
```

