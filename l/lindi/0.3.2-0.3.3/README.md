# Comparing `tmp/lindi-0.3.2.tar.gz` & `tmp/lindi-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lindi-0.3.2.tar", max compression
+gzip compressed data, was "lindi-0.3.3.tar", max compression
```

## Comparing `lindi-0.3.2.tar` & `lindi-0.3.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.3.2/LICENSE
--rw-r--r--   0        0        0     5697 2024-04-25 13:07:47.575992 lindi-0.3.2/README.md
--rw-r--r--   0        0        0     1314 2024-05-09 02:01:36.071966 lindi-0.3.2/lindi/File/File.py
--rw-r--r--   0        0        0        0 2024-05-09 02:01:36.071966 lindi-0.3.2/lindi/File/__init__.py
--rw-r--r--   0        0        0    30075 2024-05-09 02:08:46.387963 lindi-0.3.2/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
--rw-r--r--   0        0        0      529 2024-05-09 02:00:06.247966 lindi-0.3.2/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py
--rw-r--r--   0        0        0      169 2024-05-09 02:00:06.247966 lindi-0.3.2/lindi/LindiH5ZarrStore/__init__.py
--rw-r--r--   0        0        0     3112 2024-04-22 18:53:12.519957 lindi-0.3.2/lindi/LindiH5ZarrStore/_util.py
--rw-r--r--   0        0        0     2242 2024-04-19 19:44:06.440621 lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyAttributes.py
--rw-r--r--   0        0        0    11982 2024-05-09 02:12:09.023962 lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyDataset.py
--rw-r--r--   0        0        0    24707 2024-05-09 02:10:40.435962 lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyFile.py
--rw-r--r--   0        0        0     6051 2024-04-19 19:44:06.440621 lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyGroup.py
--rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyLink.py
--rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyReference.py
--rw-r--r--   0        0        0    11183 2024-05-09 02:00:32.667966 lindi-0.3.2/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
--rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.3.2/lindi/LindiH5pyFile/__init__.py
--rw-r--r--   0        0        0      528 2024-04-19 19:44:06.440621 lindi-0.3.2/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
--rw-r--r--   0        0        0     1941 2024-05-09 01:58:05.679967 lindi-0.3.2/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
--rw-r--r--   0        0        0     6651 2024-04-24 16:16:12.091927 lindi-0.3.2/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
--rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.2/lindi/LindiH5pyFile/writers/__init__.py
--rw-r--r--   0        0        0    16420 2024-05-03 16:29:00.915903 lindi-0.3.2/lindi/LindiRemfile/LindiRemfile.py
--rw-r--r--   0        0        0        0 2024-04-25 13:07:47.575992 lindi-0.3.2/lindi/LindiRemfile/__init__.py
--rw-r--r--   0        0        0     8848 2024-05-09 02:00:32.671966 lindi-0.3.2/lindi/LindiStagingStore/LindiStagingStore.py
--rw-r--r--   0        0        0     3506 2024-05-09 02:01:36.075966 lindi-0.3.2/lindi/LindiStagingStore/StagingArea.py
--rw-r--r--   0        0        0       76 2024-04-19 19:44:06.440621 lindi-0.3.2/lindi/LindiStagingStore/__init__.py
--rw-r--r--   0        0        0     2299 2024-04-25 13:07:47.575992 lindi-0.3.2/lindi/LocalCache/LocalCache.py
--rw-r--r--   0        0        0        0 2024-04-25 13:07:47.575992 lindi-0.3.2/lindi/LocalCache/__init__.py
--rw-r--r--   0        0        0      388 2024-05-09 02:01:36.075966 lindi-0.3.2/lindi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.2/lindi/conversion/__init__.py
--rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.3.2/lindi/conversion/_util.py
--rw-r--r--   0        0        0     5907 2024-04-24 16:16:12.091927 lindi-0.3.2/lindi/conversion/attr_conversion.py
--rw-r--r--   0        0        0    10819 2024-04-24 16:16:12.091927 lindi-0.3.2/lindi/conversion/create_zarr_dataset_from_h5_data.py
--rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.3.2/lindi/conversion/decode_references.py
--rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.3.2/lindi/conversion/h5_filters_to_codecs.py
--rw-r--r--   0        0        0     2041 2024-04-24 16:16:12.091927 lindi-0.3.2/lindi/conversion/h5_ref_to_zarr_attr.py
--rw-r--r--   0        0        0      936 2024-04-18 21:52:00.325839 lindi-0.3.2/lindi/conversion/nan_inf_ninf.py
--rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.3.2/lindi/conversion/reformat_json.py
--rw-r--r--   0        0        0      729 2024-05-09 02:12:30.231962 lindi-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     6357 1970-01-01 00:00:00.000000 lindi-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.3.3/LICENSE
+-rw-r--r--   0        0        0     5609 2024-05-09 12:18:43.907992 lindi-0.3.3/README.md
+-rw-r--r--   0        0        0     1314 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/File/File.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/File/__init__.py
+-rw-r--r--   0        0        0    30075 2024-05-09 10:57:01.315955 lindi-0.3.3/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
+-rw-r--r--   0        0        0      529 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py
+-rw-r--r--   0        0        0      169 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiH5ZarrStore/__init__.py
+-rw-r--r--   0        0        0     3112 2024-04-22 18:53:12.519957 lindi-0.3.3/lindi/LindiH5ZarrStore/_util.py
+-rw-r--r--   0        0        0     2242 2024-04-19 19:44:06.440621 lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyAttributes.py
+-rw-r--r--   0        0        0    11982 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyDataset.py
+-rw-r--r--   0        0        0    25313 2024-05-09 12:18:43.907992 lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyFile.py
+-rw-r--r--   0        0        0     6051 2024-04-19 19:44:06.440621 lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyGroup.py
+-rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyLink.py
+-rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyReference.py
+-rw-r--r--   0        0        0    11404 2024-05-09 12:18:43.907992 lindi-0.3.3/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
+-rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.3.3/lindi/LindiH5pyFile/__init__.py
+-rw-r--r--   0        0        0      528 2024-04-19 19:44:06.440621 lindi-0.3.3/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
+-rw-r--r--   0        0        0     1941 2024-05-09 01:58:05.679967 lindi-0.3.3/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
+-rw-r--r--   0        0        0     6651 2024-04-24 16:16:12.091927 lindi-0.3.3/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.3/lindi/LindiH5pyFile/writers/__init__.py
+-rw-r--r--   0        0        0    16420 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiRemfile/LindiRemfile.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiRemfile/__init__.py
+-rw-r--r--   0        0        0     8848 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiStagingStore/LindiStagingStore.py
+-rw-r--r--   0        0        0     3506 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LindiStagingStore/StagingArea.py
+-rw-r--r--   0        0        0       76 2024-04-19 19:44:06.440621 lindi-0.3.3/lindi/LindiStagingStore/__init__.py
+-rw-r--r--   0        0        0     2299 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LocalCache/LocalCache.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/LocalCache/__init__.py
+-rw-r--r--   0        0        0      388 2024-05-09 10:56:58.083955 lindi-0.3.3/lindi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.3/lindi/conversion/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.3.3/lindi/conversion/_util.py
+-rw-r--r--   0        0        0     5907 2024-04-24 16:16:12.091927 lindi-0.3.3/lindi/conversion/attr_conversion.py
+-rw-r--r--   0        0        0    10819 2024-04-24 16:16:12.091927 lindi-0.3.3/lindi/conversion/create_zarr_dataset_from_h5_data.py
+-rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.3.3/lindi/conversion/decode_references.py
+-rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.3.3/lindi/conversion/h5_filters_to_codecs.py
+-rw-r--r--   0        0        0     2041 2024-04-24 16:16:12.091927 lindi-0.3.3/lindi/conversion/h5_ref_to_zarr_attr.py
+-rw-r--r--   0        0        0      936 2024-04-18 21:52:00.325839 lindi-0.3.3/lindi/conversion/nan_inf_ninf.py
+-rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.3.3/lindi/conversion/reformat_json.py
+-rw-r--r--   0        0        0      729 2024-05-09 12:18:58.995992 lindi-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 lindi-0.3.3/PKG-INFO
```

### Comparing `lindi-0.3.2/LICENSE` & `lindi-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/README.md` & `lindi-0.3.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: lindi
+Version: 0.3.3
+Summary: 
+Author: Jeremy Magland
+Author-email: jmagland@flatironinstitute.org
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: h5py (>=3.10.0,<4.0.0)
+Requires-Dist: numcodecs (>=0.12.1,<0.13.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: zarr (>=2.16.1,<3.0.0)
+Description-Content-Type: text/markdown
+
 # LINDI - Linked Data Interface
 
 [![latest-release](https://img.shields.io/pypi/v/lindi.svg)](https://pypi.org/project/lindi)
 ![tests](https://github.com/neurodatawithoutborders/lindi/actions/workflows/integration_tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/neurodatawithoutborders/lindi/branch/main/graph/badge.svg?token=xxxx)](https://codecov.io/gh/neurodatawithoutborders/lindi)
 
 :warning: Please note, LINDI is currently under development and should not yet be used in practice.
@@ -90,15 +109,15 @@
 ### Read a local or remote .nwb.lindi.json file using pynwb or other tools
 
 ```python
 import pynwb
 import lindi
 
 # URL of the remote .nwb.lindi.json file
-url = 'https://kerchunk.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
+url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/56d875d6-a705-48d3-944c-53394a389c85/nwb.lindi.json'
 
 # Load the h5py-like client
 client = lindi.LindiH5pyFile.from_lindi_file(url)
 
 # Open using pynwb
 with pynwb.NWBHDF5IO(file=client, mode="r") as io:
     nwbfile = io.read()
@@ -108,36 +127,34 @@
 ### Edit a .nwb.lindi.json file using pynwb or other tools
 
 ```python
 import json
 import lindi
 
 # URL of the remote .nwb.lindi.json file
-url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
+url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/56d875d6-a705-48d3-944c-53394a389c85/nwb.lindi.json'
 
 # Load the h5py-like client for the reference file system
 # in read-write mode
 client = lindi.LindiH5pyFile.from_reference_file_system(url, mode="r+")
 
 # Edit an attribute
 client.attrs['new_attribute'] = 'new_value'
 
 # Save the changes to a new .nwb.lindi.json file
-rfs_new = client.to_reference_file_system()
-with open('new.nwb.lindi.json', 'w') as f:
-    f.write(json.dumps(rfs_new, indent=2, sort_keys=True))
+client.write_lindi_file('new.nwb.lindi.json')
 ```
 
 ### Add datasets to a .nwb.lindi.json file using a local staging area
 
 ```python
 import lindi
 
 # URL of the remote .nwb.lindi.json file
-url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
+url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/56d875d6-a705-48d3-944c-53394a389c85/nwb.lindi.json'
 
 # Load the h5py-like client for the reference file system
 # in read-write mode with a staging area
 with lindi.StagingArea.create(base_dir='lindi_staging') as staging_area:
     client = lindi.LindiH5pyFile.from_lindi_file(
         url,
         mode="r+",
@@ -154,7 +171,8 @@
 ## For developers
 
 [Special Zarr annotations used by LINDI](docs/special_zarr_annotations.md)
 
 ## License
 
 See [LICENSE](LICENSE).
+
```

### Comparing `lindi-0.3.2/lindi/File/File.py` & `lindi-0.3.3/lindi/File/File.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py` & `lindi-0.3.3/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py` & `lindi-0.3.3/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LindiH5ZarrStore/_util.py` & `lindi-0.3.3/lindi/LindiH5ZarrStore/_util.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyAttributes.py` & `lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyAttributes.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyDataset.py` & `lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyDataset.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyFile.py` & `lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyFile.py`

 * *Files 3% similar despite different names*

```diff
@@ -286,14 +286,18 @@
         """
         Write the reference file system to a .lindi.json file.
 
         Parameters
         ----------
         filename : str
             The filename to write to. It must end with '.lindi.json'.
+        generation_metadata : Union[dict, None], optional
+            The optional generation metadata to include in the reference file
+            system, by default None. This information dict is simply set to the
+            'generationMetadata' key in the reference file system.
         """
         if not filename.endswith(".lindi.json"):
             raise Exception("Filename must end with '.lindi.json'")
         rfs = self.to_reference_file_system()
         if generation_metadata is not None:
             rfs['generationMetadata'] = generation_metadata
         _write_rfs_to_file(rfs=rfs, output_file_name=filename)
@@ -513,19 +517,24 @@
                 if isinstance(src_zarr_store, LindiReferenceFileSystemStore) and isinstance(dst_zarr_store, LindiReferenceFileSystemStore):
                     src_rfs = src_zarr_store.rfs
                     dst_rfs = dst_zarr_store.rfs
                     src_ref_keys = list(src_rfs['refs'].keys())
                     for src_ref_key in src_ref_keys:
                         if src_ref_key.startswith(f'{src_item_name}/'):
                             dst_ref_key = f'{name}/{src_ref_key[len(src_item_name) + 1:]}'
-                            # Even though it's not expected to be a problem, we
-                            # do a deep copy here because a problem resulting
-                            # from one rfs being modified affecting another
-                            # would be very difficult to debug.
-                            dst_rfs['refs'][dst_ref_key] = _deep_copy(src_rfs['refs'][src_ref_key])
+                            # important to do a deep copy
+                            val = _deep_copy(src_rfs['refs'][src_ref_key])
+                            if isinstance(val, list) and len(val) > 0:
+                                # if it's a list then we need to resolve any
+                                # templates in the first element of the list.
+                                # This is very important because the destination
+                                # rfs will probably have different templates.
+                                url0 = _apply_templates(val[0], src_rfs.get('templates', {}))
+                                val[0] = url0
+                            dst_rfs['refs'][dst_ref_key] = val
                     return
 
         dst_item = dest.create_dataset(name, data=src_item[()], chunks=src_item.chunks)
         for k, v in src_item.attrs.items():
             dst_item.attrs[k] = v
     else:
         raise Exception(f"Unexpected type for src_item in _recursive_copy: {type(src_item)}")
```

### Comparing `lindi-0.3.2/lindi/LindiH5pyFile/LindiH5pyGroup.py` & `lindi-0.3.3/lindi/LindiH5pyFile/LindiH5pyGroup.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py` & `lindi-0.3.3/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,30 +45,32 @@
     it is, the string is assumed to be base64 encoded and is decoded before
     being returned. Otherwise, the string is utf-8 encoded and returned as is.
     Note that a file that actually begins with "base64:" should be represented
     by a base64 encoded string, to avoid ambiguity.
 
     We also support the use of templates as in fsspec, but do not support the
     full jinja2 templating. There may be an optional "templates" key in the
-    dictionary, which is a dictionary of template strings. For example,
-    {
+    dictionary, which is a dictionary of template strings. For example, {
         "templates": {"u1": "https://some/url", "u2": "https://some/other/url"},
         "refs": {
             ... "/some/key/0": [
                 "{{u1}}" 0, 100
             ],
             ...
         }
-    }
-    In this case, the "{{u1}}" will be replaced with the value of the "u1"
+    } In this case, the "{{u1}}" will be replaced with the value of the "u1"
     template string.
 
+    Optionally, the reference file system may contain a "generationMetadata"
+    key, which is a dictionary of metadata about the generation of the reference
+    file system. This metadata is not used by this class, but could be by other
+    software. See LindiH5pyFile.write_lindi_file(...)
+
     It is okay for rfs to be modified outside of this class, and the changes
-    will be reflected immediately in the store. This can be used by experimental
-    tools such as lindi-cloud.
+    will be reflected immediately in the store.
     """
     def __init__(self, rfs: dict, *, mode: Literal["r", "r+"] = "r+", local_cache: Union[LocalCache, None] = None):
         """
         Create a LindiReferenceFileSystemStore.
 
         Parameters
         ----------
```

### Comparing `lindi-0.3.2/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py` & `lindi-0.3.3/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py` & `lindi-0.3.3/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py` & `lindi-0.3.3/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LindiRemfile/LindiRemfile.py` & `lindi-0.3.3/lindi/LindiRemfile/LindiRemfile.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LindiStagingStore/LindiStagingStore.py` & `lindi-0.3.3/lindi/LindiStagingStore/LindiStagingStore.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LindiStagingStore/StagingArea.py` & `lindi-0.3.3/lindi/LindiStagingStore/StagingArea.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/LocalCache/LocalCache.py` & `lindi-0.3.3/lindi/LocalCache/LocalCache.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/conversion/attr_conversion.py` & `lindi-0.3.3/lindi/conversion/attr_conversion.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/conversion/create_zarr_dataset_from_h5_data.py` & `lindi-0.3.3/lindi/conversion/create_zarr_dataset_from_h5_data.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/conversion/decode_references.py` & `lindi-0.3.3/lindi/conversion/decode_references.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/conversion/h5_filters_to_codecs.py` & `lindi-0.3.3/lindi/conversion/h5_filters_to_codecs.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/conversion/h5_ref_to_zarr_attr.py` & `lindi-0.3.3/lindi/conversion/h5_ref_to_zarr_attr.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/lindi/conversion/nan_inf_ninf.py` & `lindi-0.3.3/lindi/conversion/nan_inf_ninf.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.2/pyproject.toml` & `lindi-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lindi"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = [
     "Jeremy Magland <jmagland@flatironinstitute.org>",
     "Ryan Ly <rly@lbl.gov>",
     "Oliver Ruebel <oruebel@lbl.gov>"
 ]
 readme = "README.md"
```

### Comparing `lindi-0.3.2/PKG-INFO` & `lindi-0.3.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: lindi
-Version: 0.3.2
-Summary: 
-Author: Jeremy Magland
-Author-email: jmagland@flatironinstitute.org
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: h5py (>=3.10.0,<4.0.0)
-Requires-Dist: numcodecs (>=0.12.1,<0.13.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: zarr (>=2.16.1,<3.0.0)
-Description-Content-Type: text/markdown
-
 # LINDI - Linked Data Interface
 
 [![latest-release](https://img.shields.io/pypi/v/lindi.svg)](https://pypi.org/project/lindi)
 ![tests](https://github.com/neurodatawithoutborders/lindi/actions/workflows/integration_tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/neurodatawithoutborders/lindi/branch/main/graph/badge.svg?token=xxxx)](https://codecov.io/gh/neurodatawithoutborders/lindi)
 
 :warning: Please note, LINDI is currently under development and should not yet be used in practice.
@@ -109,15 +90,15 @@
 ### Read a local or remote .nwb.lindi.json file using pynwb or other tools
 
 ```python
 import pynwb
 import lindi
 
 # URL of the remote .nwb.lindi.json file
-url = 'https://kerchunk.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
+url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/56d875d6-a705-48d3-944c-53394a389c85/nwb.lindi.json'
 
 # Load the h5py-like client
 client = lindi.LindiH5pyFile.from_lindi_file(url)
 
 # Open using pynwb
 with pynwb.NWBHDF5IO(file=client, mode="r") as io:
     nwbfile = io.read()
@@ -127,36 +108,34 @@
 ### Edit a .nwb.lindi.json file using pynwb or other tools
 
 ```python
 import json
 import lindi
 
 # URL of the remote .nwb.lindi.json file
-url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
+url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/56d875d6-a705-48d3-944c-53394a389c85/nwb.lindi.json'
 
 # Load the h5py-like client for the reference file system
 # in read-write mode
 client = lindi.LindiH5pyFile.from_reference_file_system(url, mode="r+")
 
 # Edit an attribute
 client.attrs['new_attribute'] = 'new_value'
 
 # Save the changes to a new .nwb.lindi.json file
-rfs_new = client.to_reference_file_system()
-with open('new.nwb.lindi.json', 'w') as f:
-    f.write(json.dumps(rfs_new, indent=2, sort_keys=True))
+client.write_lindi_file('new.nwb.lindi.json')
 ```
 
 ### Add datasets to a .nwb.lindi.json file using a local staging area
 
 ```python
 import lindi
 
 # URL of the remote .nwb.lindi.json file
-url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
+url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/56d875d6-a705-48d3-944c-53394a389c85/nwb.lindi.json'
 
 # Load the h5py-like client for the reference file system
 # in read-write mode with a staging area
 with lindi.StagingArea.create(base_dir='lindi_staging') as staging_area:
     client = lindi.LindiH5pyFile.from_lindi_file(
         url,
         mode="r+",
@@ -173,8 +152,7 @@
 ## For developers
 
 [Special Zarr annotations used by LINDI](docs/special_zarr_annotations.md)
 
 ## License
 
 See [LICENSE](LICENSE).
-
```

