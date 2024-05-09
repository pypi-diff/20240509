# Comparing `tmp/xarray_ome_ngff-2.1.1.tar.gz` & `tmp/xarray_ome_ngff-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_ome_ngff-2.1.1.tar", max compression
+gzip compressed data, was "xarray_ome_ngff-2.2.0.tar", max compression
```

## Comparing `xarray_ome_ngff-2.1.1.tar` & `xarray_ome_ngff-2.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1511 2024-01-01 11:59:38.523694 xarray_ome_ngff-2.1.1/LICENSE.md
--rw-r--r--   0        0        0     4376 2024-04-03 14:55:35.758166 xarray_ome_ngff-2.1.1/README.md
--rw-r--r--   0        0        0     1201 2024-04-23 19:13:06.541010 xarray_ome_ngff-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     5838 2024-04-23 13:22:32.986586 xarray_ome_ngff-2.1.1/src/xarray_ome_ngff/__init__.py
--rw-r--r--   0        0        0     4122 2024-04-23 13:44:31.635682 xarray_ome_ngff-2.1.1/src/xarray_ome_ngff/array_wrap.py
--rw-r--r--   0        0        0      365 2024-04-23 15:31:13.379841 xarray_ome_ngff-2.1.1/src/xarray_ome_ngff/core.py
--rw-r--r--   0        0        0        0 2024-01-01 11:59:38.527695 xarray_ome_ngff-2.1.1/src/xarray_ome_ngff/py.typed
--rw-r--r--   0        0        0        0 2024-01-01 11:59:38.527695 xarray_ome_ngff-2.1.1/src/xarray_ome_ngff/v04/__init__.py
--rw-r--r--   0        0        0    20892 2024-04-23 14:32:41.155614 xarray_ome_ngff-2.1.1/src/xarray_ome_ngff/v04/multiscale.py
--rw-r--r--   0        0        0     5109 1970-01-01 00:00:00.000000 xarray_ome_ngff-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1511 2024-01-01 11:59:38.523694 xarray_ome_ngff-2.2.0/LICENSE.md
+-rw-r--r--   0        0        0     4376 2024-04-03 14:55:35.758166 xarray_ome_ngff-2.2.0/README.md
+-rw-r--r--   0        0        0     1261 2024-05-09 20:43:08.120593 xarray_ome_ngff-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5838 2024-04-23 13:22:32.986586 xarray_ome_ngff-2.2.0/src/xarray_ome_ngff/__init__.py
+-rw-r--r--   0        0        0     4122 2024-04-23 13:44:31.635682 xarray_ome_ngff-2.2.0/src/xarray_ome_ngff/array_wrap.py
+-rw-r--r--   0        0        0     1989 2024-05-09 20:42:55.096382 xarray_ome_ngff-2.2.0/src/xarray_ome_ngff/core.py
+-rw-r--r--   0        0        0        0 2024-01-01 11:59:38.527695 xarray_ome_ngff-2.2.0/src/xarray_ome_ngff/py.typed
+-rw-r--r--   0        0        0        0 2024-01-01 11:59:38.527695 xarray_ome_ngff-2.2.0/src/xarray_ome_ngff/v04/__init__.py
+-rw-r--r--   0        0        0    20230 2024-05-09 20:42:55.096382 xarray_ome_ngff-2.2.0/src/xarray_ome_ngff/v04/multiscale.py
+-rw-r--r--   0        0        0     5109 1970-01-01 00:00:00.000000 xarray_ome_ngff-2.2.0/PKG-INFO
```

### Comparing `xarray_ome_ngff-2.1.1/LICENSE.md` & `xarray_ome_ngff-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xarray_ome_ngff-2.1.1/README.md` & `xarray_ome_ngff-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `xarray_ome_ngff-2.1.1/pyproject.toml` & `xarray_ome_ngff-2.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xarray-ome-ngff"
-version = "2.1.1"
+version = "2.2.0"
 description = "xarray and ome-ngff"
 authors = ["Davis Vann Bennett <davis.v.bennett@gmail.com>"]
 readme = "README.md"
 packages = [{include = "xarray_ome_ngff", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -49,7 +49,12 @@
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+lint.select = [
+    "I",  # isort formatting.
+]
```

### Comparing `xarray_ome_ngff-2.1.1/src/xarray_ome_ngff/__init__.py` & `xarray_ome_ngff-2.2.0/src/xarray_ome_ngff/__init__.py`

 * *Files identical despite different names*

### Comparing `xarray_ome_ngff-2.1.1/src/xarray_ome_ngff/array_wrap.py` & `xarray_ome_ngff-2.2.0/src/xarray_ome_ngff/array_wrap.py`

 * *Files identical despite different names*

### Comparing `xarray_ome_ngff-2.1.1/src/xarray_ome_ngff/v04/multiscale.py` & `xarray_ome_ngff-2.2.0/src/xarray_ome_ngff/v04/multiscale.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from __future__ import annotations
-from pydantic_ome_ngff.v04.multiscale import Group as MultiscaleGroup
+
 from typing import TYPE_CHECKING, Literal
 
-from xarray_ome_ngff.array_wrap import ArrayWrapperSpec, DaskArrayWrapper
-from xarray_ome_ngff.array_wrap import ZarrArrayWrapper
-from xarray_ome_ngff.array_wrap import parse_wrapper
+from pydantic_ome_ngff.v04.multiscale import Group as MultiscaleGroup
+
+from xarray_ome_ngff.array_wrap import (
+    ArrayWrapperSpec,
+    DaskArrayWrapper,
+    ZarrArrayWrapper,
+    parse_wrapper,
+)
+from xarray_ome_ngff.core import get_parent
 
 if TYPE_CHECKING:
     from typing import Any, Dict, Sequence
 
+import os
+import warnings
+
 import numpy as np
-from xarray import DataArray
+import zarr
+from numcodecs import Zstd
+from numcodecs.abc import Codec
 from pydantic_ome_ngff.v04.axis import Axis
 from pydantic_ome_ngff.v04.multiscale import Dataset, MultiscaleMetadata
 from pydantic_ome_ngff.v04.transform import (
     VectorScale,
     VectorTranslation,
 )
-import warnings
-from xarray_ome_ngff.core import CoordinateAttrs, ureg
-import zarr
+from xarray import DataArray
 from zarr.storage import BaseStore
-from numcodecs.abc import Codec
-from numcodecs import Zstd
 
-import os
+from xarray_ome_ngff.core import CoordinateAttrs, ureg
 
 
 def multiscale_metadata(
     arrays: dict[str, DataArray],
     name: str | None = None,
     type: str | None = None,
     metadata: Dict[str, Any] | None = None,
@@ -276,15 +283,14 @@
 
 def normalize_transforms(
     base_transforms: (
         None | tuple[()] | tuple[VectorScale] | tuple[VectorScale, VectorTranslation]
     ),
     dset_transforms: tuple[VectorScale] | tuple[VectorScale, VectorTranslation],
 ) -> tuple[VectorScale, VectorTranslation]:
-
     if base_transforms is None or len(base_transforms) == 0:
         out_scale = dset_transforms[0]
         if len(dset_transforms) == 1:
             out_trans = VectorTranslation(translation=(0,) * len(out_scale.scale))
         else:
             out_trans = dset_transforms[1]
     else:
@@ -461,30 +467,14 @@
         )
         arr_out = DataArray(data=arr_wrapped, coords=coords)
         result[dset.path] = arr_out
 
     return result
 
 
-def get_parent(node: zarr.Group | zarr.Array) -> zarr.Group:
-    """
-    Get the parent node of a Zarr array or group
-    """
-    if hasattr(node.store, "path"):
-        store_path = node.store.path
-        if node.path == "":
-            new_full_path, new_node_path = os.path.split(os.path.split(store_path)[0])
-        else:
-            full_path, _ = os.path.split(os.path.join(store_path, node.path))
-            new_full_path, new_node_path = os.path.split(full_path)
-        return zarr.open_group(type(node.store)(new_full_path), path=new_node_path)
-    else:
-        return zarr.open_group(store=node.store, path=os.path.split(node.path)[0])
-
-
 def read_array(
     array: zarr.Array,
     *,
     array_wrapper: (
         ZarrArrayWrapper | DaskArrayWrapper | ArrayWrapperSpec
     ) = ZarrArrayWrapper(),
 ) -> DataArray:
```

### Comparing `xarray_ome_ngff-2.1.1/PKG-INFO` & `xarray_ome_ngff-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-ome-ngff
-Version: 2.1.1
+Version: 2.2.0
 Summary: xarray and ome-ngff
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

