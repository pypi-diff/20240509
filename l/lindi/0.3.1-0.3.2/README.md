# Comparing `tmp/lindi-0.3.1.tar.gz` & `tmp/lindi-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lindi-0.3.1.tar", max compression
+gzip compressed data, was "lindi-0.3.2.tar", max compression
```

## Comparing `lindi-0.3.1.tar` & `lindi-0.3.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.3.1/LICENSE
--rw-r--r--   0        0        0     5697 2024-04-25 13:07:47.575992 lindi-0.3.1/README.md
--rw-r--r--   0        0        0     1314 2024-04-25 20:36:30.815997 lindi-0.3.1/lindi/File/File.py
--rw-r--r--   0        0        0        0 2024-04-25 20:30:55.955999 lindi-0.3.1/lindi/File/__init__.py
--rw-r--r--   0        0        0    29801 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
--rw-r--r--   0        0        0      529 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py
--rw-r--r--   0        0        0      169 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiH5ZarrStore/__init__.py
--rw-r--r--   0        0        0     3112 2024-04-22 18:53:12.519957 lindi-0.3.1/lindi/LindiH5ZarrStore/_util.py
--rw-r--r--   0        0        0     2242 2024-04-19 19:44:06.440621 lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyAttributes.py
--rw-r--r--   0        0        0    11776 2024-04-25 18:34:46.019872 lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyDataset.py
--rw-r--r--   0        0        0    24528 2024-04-25 13:36:35.223981 lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyFile.py
--rw-r--r--   0        0        0     6051 2024-04-19 19:44:06.440621 lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyGroup.py
--rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyLink.py
--rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyReference.py
--rw-r--r--   0        0        0    11183 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
--rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.3.1/lindi/LindiH5pyFile/__init__.py
--rw-r--r--   0        0        0      528 2024-04-19 19:44:06.440621 lindi-0.3.1/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
--rw-r--r--   0        0        0     1941 2024-04-19 19:44:06.440621 lindi-0.3.1/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
--rw-r--r--   0        0        0     6651 2024-04-24 16:16:12.091927 lindi-0.3.1/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
--rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.1/lindi/LindiH5pyFile/writers/__init__.py
--rw-r--r--   0        0        0    16420 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiRemfile/LindiRemfile.py
--rw-r--r--   0        0        0        0 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiRemfile/__init__.py
--rw-r--r--   0        0        0     8848 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LindiStagingStore/LindiStagingStore.py
--rw-r--r--   0        0        0     3506 2024-04-25 13:16:02.363988 lindi-0.3.1/lindi/LindiStagingStore/StagingArea.py
--rw-r--r--   0        0        0       76 2024-04-19 19:44:06.440621 lindi-0.3.1/lindi/LindiStagingStore/__init__.py
--rw-r--r--   0        0        0     2299 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LocalCache/LocalCache.py
--rw-r--r--   0        0        0        0 2024-04-25 13:07:47.575992 lindi-0.3.1/lindi/LocalCache/__init__.py
--rw-r--r--   0        0        0      388 2024-04-25 20:32:45.831998 lindi-0.3.1/lindi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.1/lindi/conversion/__init__.py
--rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.3.1/lindi/conversion/_util.py
--rw-r--r--   0        0        0     5907 2024-04-24 16:16:12.091927 lindi-0.3.1/lindi/conversion/attr_conversion.py
--rw-r--r--   0        0        0    10819 2024-04-24 16:16:12.091927 lindi-0.3.1/lindi/conversion/create_zarr_dataset_from_h5_data.py
--rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.3.1/lindi/conversion/decode_references.py
--rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.3.1/lindi/conversion/h5_filters_to_codecs.py
--rw-r--r--   0        0        0     2041 2024-04-24 16:16:12.091927 lindi-0.3.1/lindi/conversion/h5_ref_to_zarr_attr.py
--rw-r--r--   0        0        0      936 2024-04-18 21:52:00.325839 lindi-0.3.1/lindi/conversion/nan_inf_ninf.py
--rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.3.1/lindi/conversion/reformat_json.py
--rw-r--r--   0        0        0      729 2024-04-26 14:55:53.451922 lindi-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6357 1970-01-01 00:00:00.000000 lindi-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5697 2024-04-25 13:07:47.575992 lindi-0.3.2/README.md
+-rw-r--r--   0        0        0     1314 2024-05-09 02:01:36.071966 lindi-0.3.2/lindi/File/File.py
+-rw-r--r--   0        0        0        0 2024-05-09 02:01:36.071966 lindi-0.3.2/lindi/File/__init__.py
+-rw-r--r--   0        0        0    30075 2024-05-09 02:08:46.387963 lindi-0.3.2/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
+-rw-r--r--   0        0        0      529 2024-05-09 02:00:06.247966 lindi-0.3.2/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py
+-rw-r--r--   0        0        0      169 2024-05-09 02:00:06.247966 lindi-0.3.2/lindi/LindiH5ZarrStore/__init__.py
+-rw-r--r--   0        0        0     3112 2024-04-22 18:53:12.519957 lindi-0.3.2/lindi/LindiH5ZarrStore/_util.py
+-rw-r--r--   0        0        0     2242 2024-04-19 19:44:06.440621 lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyAttributes.py
+-rw-r--r--   0        0        0    11982 2024-05-09 02:12:09.023962 lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyDataset.py
+-rw-r--r--   0        0        0    24707 2024-05-09 02:10:40.435962 lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyFile.py
+-rw-r--r--   0        0        0     6051 2024-04-19 19:44:06.440621 lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyGroup.py
+-rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyLink.py
+-rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyReference.py
+-rw-r--r--   0        0        0    11183 2024-05-09 02:00:32.667966 lindi-0.3.2/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
+-rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.3.2/lindi/LindiH5pyFile/__init__.py
+-rw-r--r--   0        0        0      528 2024-04-19 19:44:06.440621 lindi-0.3.2/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
+-rw-r--r--   0        0        0     1941 2024-05-09 01:58:05.679967 lindi-0.3.2/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
+-rw-r--r--   0        0        0     6651 2024-04-24 16:16:12.091927 lindi-0.3.2/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.2/lindi/LindiH5pyFile/writers/__init__.py
+-rw-r--r--   0        0        0    16420 2024-05-03 16:29:00.915903 lindi-0.3.2/lindi/LindiRemfile/LindiRemfile.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:07:47.575992 lindi-0.3.2/lindi/LindiRemfile/__init__.py
+-rw-r--r--   0        0        0     8848 2024-05-09 02:00:32.671966 lindi-0.3.2/lindi/LindiStagingStore/LindiStagingStore.py
+-rw-r--r--   0        0        0     3506 2024-05-09 02:01:36.075966 lindi-0.3.2/lindi/LindiStagingStore/StagingArea.py
+-rw-r--r--   0        0        0       76 2024-04-19 19:44:06.440621 lindi-0.3.2/lindi/LindiStagingStore/__init__.py
+-rw-r--r--   0        0        0     2299 2024-04-25 13:07:47.575992 lindi-0.3.2/lindi/LocalCache/LocalCache.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:07:47.575992 lindi-0.3.2/lindi/LocalCache/__init__.py
+-rw-r--r--   0        0        0      388 2024-05-09 02:01:36.075966 lindi-0.3.2/lindi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.2/lindi/conversion/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.3.2/lindi/conversion/_util.py
+-rw-r--r--   0        0        0     5907 2024-04-24 16:16:12.091927 lindi-0.3.2/lindi/conversion/attr_conversion.py
+-rw-r--r--   0        0        0    10819 2024-04-24 16:16:12.091927 lindi-0.3.2/lindi/conversion/create_zarr_dataset_from_h5_data.py
+-rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.3.2/lindi/conversion/decode_references.py
+-rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.3.2/lindi/conversion/h5_filters_to_codecs.py
+-rw-r--r--   0        0        0     2041 2024-04-24 16:16:12.091927 lindi-0.3.2/lindi/conversion/h5_ref_to_zarr_attr.py
+-rw-r--r--   0        0        0      936 2024-04-18 21:52:00.325839 lindi-0.3.2/lindi/conversion/nan_inf_ninf.py
+-rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.3.2/lindi/conversion/reformat_json.py
+-rw-r--r--   0        0        0      729 2024-05-09 02:12:30.231962 lindi-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6357 1970-01-01 00:00:00.000000 lindi-0.3.2/PKG-INFO
```

### Comparing `lindi-0.3.1/LICENSE` & `lindi-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/README.md` & `lindi-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/File/File.py` & `lindi-0.3.2/lindi/File/File.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py` & `lindi-0.3.2/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,20 @@
         for i, c in enumerate(chunk_coords):
             if c < 0 or c >= h5_item.shape[i]:
                 raise Exception(
                     f"Chunk coordinates {chunk_coords} out of range for dataset {key_parent} with dtype {h5_item.dtype}"
                 )
         if h5_item.chunks is not None:
             # Get the byte range in the file for the chunk.
-            byte_offset, byte_count = _get_chunk_byte_range(h5_item, chunk_coords)
+            try:
+                byte_offset, byte_count = _get_chunk_byte_range(h5_item, chunk_coords)
+            except Exception as e:
+                raise Exception(
+                    f"Error getting byte range for chunk {key_parent}/{key_name}. Shape: {h5_item.shape}, Chunks: {h5_item.chunks}, Chunk coords: {chunk_coords}: {e}"
+                )
         else:
             # In this case (contiguous dataset), we need to check that the chunk
             # coordinates are (0, 0, 0, ...)
             if chunk_coords != (0,) * h5_item.ndim:
                 raise Exception(
                     f"Chunk coordinates {chunk_coords} are not (0, 0, 0, ...) for contiguous dataset {key_parent} with dtype {h5_item.dtype} and shape {h5_item.shape}"
                 )
```

### Comparing `lindi-0.3.1/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py` & `lindi-0.3.2/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/LindiH5ZarrStore/_util.py` & `lindi-0.3.2/lindi/LindiH5ZarrStore/_util.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyAttributes.py` & `lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyAttributes.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyDataset.py` & `lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyDataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,15 +209,17 @@
                 )
 
         # We use zarr's slicing, except in the case of a scalar dataset
         if self.ndim == 0:
             # make sure selection is ()
             if selection != ():
                 raise TypeError(f'Cannot slice a scalar dataset with {selection}')
-            return zarr_array[0]
+            # For some reason, with the newest version of zarr (2.18.0) we need to use [:][0] rather than just [0].
+            # Otherwise we get an error "ValueError: buffer source array is read-only"
+            return zarr_array[:][0]
         return decode_references(zarr_array[selection])
 
     def _get_external_hdf5_client(self, url: str) -> h5py.File:
         if url not in _external_hdf5_clients:
             if url.startswith("http://") or url.startswith("https://"):
                 ff = LindiRemfile(url, local_cache=self._file._local_cache)
             else:
```

### Comparing `lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyFile.py` & `lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
                 assert isinstance(data, dict)  # prevent infinite recursion
                 return LindiH5pyFile.from_reference_file_system(data, mode=mode, staging_area=staging_area, local_cache=local_cache, local_file_path=local_file_path)
         elif isinstance(rfs, dict):
             # This store does not need to be closed
             store = LindiReferenceFileSystemStore(rfs, local_cache=local_cache)
             if staging_area:
                 store = LindiStagingStore(base_store=store, staging_area=staging_area)
-            return LindiH5pyFile.from_zarr_store(store, mode=mode, local_file_path=local_file_path)
+            return LindiH5pyFile.from_zarr_store(store, mode=mode, local_file_path=local_file_path, local_cache=local_cache)
         else:
             raise Exception(f"Unhandled type for rfs: {type(rfs)}")
 
     @staticmethod
     def from_zarr_store(zarr_store: ZarrStore, mode: LindiFileMode = "r", local_cache: Union[LocalCache, None] = None, local_file_path: Union[str, None] = None):
         """
         Create a LindiH5pyFile from a zarr store.
@@ -278,26 +278,28 @@
                     v[0] = url2
         with tempfile.TemporaryDirectory() as tmpdir:
             rfs_fname = f"{tmpdir}/rfs.lindi.json"
             LindiReferenceFileSystemStore.use_templates_in_rfs(rfs)
             _write_rfs_to_file(rfs=rfs, output_file_name=rfs_fname)
             return on_upload_main(rfs_fname)
 
-    def write_lindi_file(self, filename: str):
+    def write_lindi_file(self, filename: str, *, generation_metadata: Union[dict, None] = None):
         """
         Write the reference file system to a .lindi.json file.
 
         Parameters
         ----------
         filename : str
             The filename to write to. It must end with '.lindi.json'.
         """
         if not filename.endswith(".lindi.json"):
             raise Exception("Filename must end with '.lindi.json'")
         rfs = self.to_reference_file_system()
+        if generation_metadata is not None:
+            rfs['generationMetadata'] = generation_metadata
         _write_rfs_to_file(rfs=rfs, output_file_name=filename)
 
     @property
     def attrs(self):  # type: ignore
         return LindiH5pyAttributes(self._zarr_group.attrs, readonly=self.mode == "r")
 
     @property
```

### Comparing `lindi-0.3.1/lindi/LindiH5pyFile/LindiH5pyGroup.py` & `lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyGroup.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py` & `lindi-0.3.2/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py` & `lindi-0.3.2/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py` & `lindi-0.3.2/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py` & `lindi-0.3.2/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/LindiRemfile/LindiRemfile.py` & `lindi-0.3.2/lindi/LindiRemfile/LindiRemfile.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/LindiStagingStore/LindiStagingStore.py` & `lindi-0.3.2/lindi/LindiStagingStore/LindiStagingStore.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/LindiStagingStore/StagingArea.py` & `lindi-0.3.2/lindi/LindiStagingStore/StagingArea.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/LocalCache/LocalCache.py` & `lindi-0.3.2/lindi/LocalCache/LocalCache.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/conversion/attr_conversion.py` & `lindi-0.3.2/lindi/conversion/attr_conversion.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/conversion/create_zarr_dataset_from_h5_data.py` & `lindi-0.3.2/lindi/conversion/create_zarr_dataset_from_h5_data.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/conversion/decode_references.py` & `lindi-0.3.2/lindi/conversion/decode_references.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/conversion/h5_filters_to_codecs.py` & `lindi-0.3.2/lindi/conversion/h5_filters_to_codecs.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/conversion/h5_ref_to_zarr_attr.py` & `lindi-0.3.2/lindi/conversion/h5_ref_to_zarr_attr.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/lindi/conversion/nan_inf_ninf.py` & `lindi-0.3.2/lindi/conversion/nan_inf_ninf.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.1/pyproject.toml` & `lindi-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lindi"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = [
     "Jeremy Magland <jmagland@flatironinstitute.org>",
     "Ryan Ly <rly@lbl.gov>",
     "Oliver Ruebel <oruebel@lbl.gov>"
 ]
 readme = "README.md"
```

### Comparing `lindi-0.3.1/PKG-INFO` & `lindi-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lindi
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

