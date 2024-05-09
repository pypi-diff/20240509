# Comparing `tmp/pydantic_numpy-5.0.1.tar.gz` & `tmp/pydantic_numpy-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_numpy-5.0.1.tar", max compression
+gzip compressed data, was "pydantic_numpy-5.0.2.tar", max compression
```

## Comparing `pydantic_numpy-5.0.1.tar` & `pydantic_numpy-5.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1658 2024-04-19 06:32:51.120243 pydantic_numpy-5.0.1/LICENSE
--rw-r--r--   0        0        0     4547 2024-04-19 06:32:51.120243 pydantic_numpy-5.0.1/README.md
--rw-r--r--   0        0        0      199 2024-04-19 06:32:51.120243 pydantic_numpy-5.0.1/pydantic_numpy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 06:32:51.120243 pydantic_numpy-5.0.1/pydantic_numpy/helper/__init__.py
--rw-r--r--   0        0        0    13321 2024-04-19 06:32:51.120243 pydantic_numpy-5.0.1/pydantic_numpy/helper/annotation.py
--rw-r--r--   0        0        0      168 2024-04-19 06:32:51.120243 pydantic_numpy-5.0.1/pydantic_numpy/helper/typing.py
--rw-r--r--   0        0        0     3645 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/helper/validation.py
--rw-r--r--   0        0        0     9736 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/model.py
--rw-r--r--   0        0        0      474 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/__init__.py
--rw-r--r--   0        0        0     4886 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/i_dimensional.py
--rw-r--r--   0        0        0     4981 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/ii_dimensional.py
--rw-r--r--   0        0        0     5076 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/iii_dimensional.py
--rw-r--r--   0        0        0     4810 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/n_dimensional.py
--rw-r--r--   0        0        0        0 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/__init__.py
--rw-r--r--   0        0        0     4086 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/i_dimensional.py
--rw-r--r--   0        0        0     4176 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
--rw-r--r--   0        0        0     4266 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
--rw-r--r--   0        0        0     4019 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/n_dimensional.py
--rw-r--r--   0        0        0     1621 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/util.py
--rw-r--r--   0        0        0     1542 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     5606 1970-01-01 00:00:00.000000 pydantic_numpy-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1658 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/LICENSE
+-rw-r--r--   0        0        0     4547 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/README.md
+-rw-r--r--   0        0        0      199 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/helper/__init__.py
+-rw-r--r--   0        0        0    13321 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/helper/annotation.py
+-rw-r--r--   0        0        0      168 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/helper/typing.py
+-rw-r--r--   0        0        0     3645 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/helper/validation.py
+-rw-r--r--   0        0        0     9703 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/model.py
+-rw-r--r--   0        0        0      474 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/typing/__init__.py
+-rw-r--r--   0        0        0     4886 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/typing/i_dimensional.py
+-rw-r--r--   0        0        0     4981 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/typing/ii_dimensional.py
+-rw-r--r--   0        0        0     5076 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/typing/iii_dimensional.py
+-rw-r--r--   0        0        0     4810 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/typing/n_dimensional.py
+-rw-r--r--   0        0        0        0 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/typing/strict_data_type/__init__.py
+-rw-r--r--   0        0        0     4086 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/typing/strict_data_type/i_dimensional.py
+-rw-r--r--   0        0        0     4176 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
+-rw-r--r--   0        0        0     4266 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
+-rw-r--r--   0        0        0     4019 2024-05-09 19:35:22.233761 pydantic_numpy-5.0.2/pydantic_numpy/typing/strict_data_type/n_dimensional.py
+-rw-r--r--   0        0        0     1621 2024-05-09 19:35:22.237761 pydantic_numpy-5.0.2/pydantic_numpy/util.py
+-rw-r--r--   0        0        0     1562 2024-05-09 19:35:22.237761 pydantic_numpy-5.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5606 1970-01-01 00:00:00.000000 pydantic_numpy-5.0.2/PKG-INFO
```

### Comparing `pydantic_numpy-5.0.1/LICENSE` & `pydantic_numpy-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/README.md` & `pydantic_numpy-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/pydantic_numpy/helper/annotation.py` & `pydantic_numpy-5.0.2/pydantic_numpy/helper/annotation.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/pydantic_numpy/helper/validation.py` & `pydantic_numpy-5.0.2/pydantic_numpy/helper/validation.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/pydantic_numpy/model.py` & `pydantic_numpy-5.0.2/pydantic_numpy/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,32 +41,37 @@
     _dump_compression: ClassVar[str] = "lz4"
     _dump_numpy_savez_file_name: ClassVar[str] = "arrays.npz"
     _dump_non_array_file_stem: ClassVar[str] = "object_info"
 
     _directory_suffix: ClassVar[str] = ".pdnp"
 
     def __eq__(self, other: Any) -> bool:
-        if isinstance(other, NumpyModel):
-            self_type = self.__pydantic_generic_metadata__["origin"] or self.__class__
-            other_type = other.__pydantic_generic_metadata__["origin"] or other.__class__
+        if not isinstance(other, BaseModel):
+            return NotImplemented  # delegate to the other item in the comparison
+
+        self_type = self.__pydantic_generic_metadata__["origin"] or self.__class__
+        other_type = other.__pydantic_generic_metadata__["origin"] or other.__class__
 
+        if not (
+            self_type == other_type
+            and getattr(self, "__pydantic_private__", None) == getattr(other, "__pydantic_private__", None)
+            and self.__pydantic_extra__ == other.__pydantic_extra__
+        ):
+            return False
+
+        if isinstance(other, NumpyModel):
             self_ndarray_field_to_array, self_other_field_to_value = self._dump_numpy_split_dict()
             other_ndarray_field_to_array, other_other_field_to_value = other._dump_numpy_split_dict()
 
-            return (
-                self_type == other_type
-                and self_other_field_to_value == other_other_field_to_value
-                and self.__pydantic_private__ == other.__pydantic_private__
-                and self.__pydantic_extra__ == other.__pydantic_extra__
-                and _compare_np_array_dicts(self_ndarray_field_to_array, other_ndarray_field_to_array)
+            return self_other_field_to_value == other_other_field_to_value and _compare_np_array_dicts(
+                self_ndarray_field_to_array, other_ndarray_field_to_array
             )
-        elif isinstance(other, BaseModel):
-            return super().__eq__(other)
-        else:
-            return NotImplemented  # delegate to the other item in the comparison
+
+        # Self is NumpyModel, other is not; likely unequal; checking anyway.
+        return super().__eq__(other)
 
     @classmethod
     @validate_call
     def model_directory_path(cls, output_directory: DirectoryPath, object_id: str) -> DirectoryPath:
         return output_directory / f"{object_id}.{cls.__name__}{cls._directory_suffix}"
 
     @classmethod
@@ -152,18 +157,18 @@
 
         return dump_directory_path
 
     def _dump_numpy_split_dict(self) -> tuple[dict, dict]:
         ndarray_field_to_array = {}
         other_field_to_value = {}
 
-        for k, v in self.model_dump(exclude_unset=True).items():
+        for k, v in self.model_dump().items():
             if isinstance(v, np.ndarray):
                 ndarray_field_to_array[k] = v
-            else:
+            elif v:
                 other_field_to_value[k] = v
 
         return ndarray_field_to_array, other_field_to_value
 
     @classmethod  # type: ignore[misc]
     @computed_field(return_type=str)
     @property
@@ -255,23 +260,20 @@
     Boolean value for each key, True if corresponding arrays are close, else False.
     """
 
     keys1 = frozenset(dict_a.keys())
     keys2 = frozenset(dict_b.keys())
 
     if keys1 != keys2:
-        raise ValueError("Dictionaries have different keys")
+        return False
 
     for key in keys1:
         arr_a = dict_a[key]
         arr_b = dict_b[key]
 
-        if arr_a.shape != arr_b.shape:
-            raise ValueError(f"Arrays for key '{key}' have different shapes")
-
-        if not np_general_all_close(arr_a, arr_b, rtol, atol):
+        if arr_a.shape != arr_b.shape or not np_general_all_close(arr_a, arr_b, rtol, atol):
             return False
 
     return True
 
 
 __all__ = ["NumpyModel", "MultiArrayNumpyFile", "model_agnostic_load"]
```

### Comparing `pydantic_numpy-5.0.1/pydantic_numpy/typing/i_dimensional.py` & `pydantic_numpy-5.0.2/pydantic_numpy/typing/i_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/pydantic_numpy/typing/ii_dimensional.py` & `pydantic_numpy-5.0.2/pydantic_numpy/typing/ii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/pydantic_numpy/typing/iii_dimensional.py` & `pydantic_numpy-5.0.2/pydantic_numpy/typing/iii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/pydantic_numpy/typing/n_dimensional.py` & `pydantic_numpy-5.0.2/pydantic_numpy/typing/n_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/i_dimensional.py` & `pydantic_numpy-5.0.2/pydantic_numpy/typing/strict_data_type/i_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/ii_dimensional.py` & `pydantic_numpy-5.0.2/pydantic_numpy/typing/strict_data_type/ii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/iii_dimensional.py` & `pydantic_numpy-5.0.2/pydantic_numpy/typing/strict_data_type/iii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/n_dimensional.py` & `pydantic_numpy-5.0.2/pydantic_numpy/typing/strict_data_type/n_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/pydantic_numpy/util.py` & `pydantic_numpy-5.0.2/pydantic_numpy/util.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.1/pyproject.toml` & `pydantic_numpy-5.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic_numpy"
-version = "5.0.1"
+version = "5.0.2"
 description = "Pydantic Model integration of the NumPy array"
 authors = ["Can H. Tartanoglu", "Christoph Heindl"]
 maintainers = ["Can H. Tartanoglu <python@rotas.mozmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/caniko/pydantic-numpy"
 license = "BSD-4"
 
@@ -26,14 +26,15 @@
 pydantic = "^2.0"
 semver = "^3.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 parameterized = "^0.9.0"
 orjson = "*"
+coverage = "^7.5.1"
 
 [tool.poetry.group.format.dependencies]
 black = "^23.7.0"
 isort = "^5.12.0"
 ruff = "*"
 
 [tool.poetry.group.typecheck.dependencies]
```

### Comparing `pydantic_numpy-5.0.1/PKG-INFO` & `pydantic_numpy-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic_numpy
-Version: 5.0.1
+Version: 5.0.2
 Summary: Pydantic Model integration of the NumPy array
 Home-page: https://github.com/caniko/pydantic-numpy
 License: BSD-4
 Keywords: pydantic,numpy,typing,validation
 Author: Can H. Tartanoglu
 Maintainer: Can H. Tartanoglu
 Maintainer-email: python@rotas.mozmail.com
```

