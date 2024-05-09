# Comparing `tmp/cellmaps_sdk-0.0.15.tar.gz` & `tmp/cellmaps-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmaps_sdk-0.0.15.tar", last modified: Thu May  9 13:25:08 2024, max compression
+gzip compressed data, was "cellmaps-sdk-0.0.2.tar", last modified: Tue Mar 12 16:44:28 2024, max compression
```

## Comparing `cellmaps_sdk-0.0.15.tar` & `cellmaps-sdk-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-09 13:25:08.915569 cellmaps_sdk-0.0.15/
--rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.15/LICENSE.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1570 2024-05-09 13:25:08.915286 cellmaps_sdk-0.0.15/PKG-INFO
--rw-r--r--   0 colmbrandon   (501) staff       (20)      192 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.15/README.rst
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1562 2024-05-09 13:24:59.000000 cellmaps_sdk-0.0.15/pyproject.toml
--rw-r--r--   0 colmbrandon   (501) staff       (20)       38 2024-05-09 13:25:08.915627 cellmaps_sdk-0.0.15/setup.cfg
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-09 13:25:08.906586 cellmaps_sdk-0.0.15/src/
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-09 13:25:08.913002 cellmaps_sdk-0.0.15/src/cellmaps_sdk/
--rw-r--r--   0 colmbrandon   (501) staff       (20)      282 2024-02-06 12:12:31.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk/__init__.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     2871 2024-03-07 12:05:00.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk/__main__.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)    36830 2024-02-23 16:16:31.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk/_cli_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1636 2024-03-14 11:43:19.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk/_config.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     9718 2024-05-09 13:20:30.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk/_raw_data.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     2657 2024-02-12 17:14:01.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk/_test_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1820 2024-04-24 15:54:59.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk/_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)    35205 2024-04-18 12:00:14.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk/data.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     4461 2024-02-23 13:18:34.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk/data_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)    29788 2024-03-06 12:03:46.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk/process.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk/py.typed
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-09 13:25:08.914653 cellmaps_sdk-0.0.15/src/cellmaps_sdk.egg-info/
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1570 2024-05-09 13:25:08.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk.egg-info/PKG-INFO
--rw-r--r--   0 colmbrandon   (501) staff       (20)      595 2024-05-09 13:25:08.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)        1 2024-05-09 13:25:08.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)       55 2024-05-09 13:25:08.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk.egg-info/entry_points.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)      171 2024-05-09 13:25:08.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk.egg-info/requires.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)       13 2024-05-09 13:25:08.000000 cellmaps_sdk-0.0.15/src/cellmaps_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-03-12 16:44:28.194353 cellmaps-sdk-0.0.2/
+-rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps-sdk-0.0.2/LICENSE.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1519 2024-03-12 16:44:28.194080 cellmaps-sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      192 2024-01-26 12:59:01.000000 cellmaps-sdk-0.0.2/README.rst
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1516 2024-03-12 16:43:54.000000 cellmaps-sdk-0.0.2/pyproject.toml
+-rw-r--r--   0 colmbrandon   (501) staff       (20)       38 2024-03-12 16:44:28.194417 cellmaps-sdk-0.0.2/setup.cfg
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-03-12 16:44:28.185097 cellmaps-sdk-0.0.2/src/
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-03-12 16:44:28.192459 cellmaps-sdk-0.0.2/src/cellmaps_sdk/
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      282 2024-02-06 12:12:31.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk/__init__.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     2871 2024-03-07 12:05:00.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk/__main__.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)    36830 2024-02-23 16:16:31.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk/_cli_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1334 2024-03-06 14:29:02.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk/_config.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     2657 2024-02-12 17:14:01.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk/_test_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     4691 2024-03-12 16:43:03.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk/_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)    35174 2024-02-19 17:29:10.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk/data.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     4461 2024-02-23 13:18:34.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk/data_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)    29788 2024-03-06 12:03:46.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk/process.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk/py.typed
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-03-12 16:44:28.193524 cellmaps-sdk-0.0.2/src/cellmaps_sdk.egg-info/
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1519 2024-03-12 16:44:28.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      565 2024-03-12 16:44:28.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)        1 2024-03-12 16:44:28.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)       55 2024-03-12 16:44:28.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      171 2024-03-12 16:44:28.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk.egg-info/requires.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)       13 2024-03-12 16:44:28.000000 cellmaps-sdk-0.0.2/src/cellmaps_sdk.egg-info/top_level.txt
```

### Comparing `cellmaps_sdk-0.0.15/PKG-INFO` & `cellmaps-sdk-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: cellmaps-sdk
-Version: 0.0.15
+Version: 0.0.2
 Summary: The SDK for tool builders who wish to integrate their tool into the CellMaps Analysis Workflow IME
 Author-email: Colm Brandon <colm.brandon@ul.ie>
 Project-URL: Homepage, http://example.com
 Project-URL: Documentation, http://example.com
 Project-URL: Repository, http://example.com
 Project-URL: Bug Tracker, http://example.com
 Project-URL: Changelog, http://example.com
 Keywords: Highly-plexed Tissue Imaging,AI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: requests
```

### Comparing `cellmaps_sdk-0.0.15/pyproject.toml` & `cellmaps-sdk-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [project]
 name = "cellmaps-sdk"
 authors = [{name = "Colm Brandon", email = "colm.brandon@ul.ie"}]
-version = "0.0.15"
+version = "0.0.2"
 description = "The SDK for tool builders who wish to integrate their tool into the CellMaps Analysis Workflow IME"
 readme = "README.rst"
 license = {file = "LICENSE.txt"}
 keywords = ["Highly-plexed Tissue Imaging", "AI",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 requires-python = ">=3.7" # Can potentially expand on this
```

### Comparing `cellmaps_sdk-0.0.15/src/cellmaps_sdk/__main__.py` & `cellmaps-sdk-0.0.2/src/cellmaps_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.15/src/cellmaps_sdk/_cli_utils.py` & `cellmaps-sdk-0.0.2/src/cellmaps_sdk/_cli_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.15/src/cellmaps_sdk/_test_utils.py` & `cellmaps-sdk-0.0.2/src/cellmaps_sdk/_test_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.15/src/cellmaps_sdk/data.py` & `cellmaps-sdk-0.0.2/src/cellmaps_sdk/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 from PIL import Image as _Image, TiffImagePlugin as _TiffImagePlugin
 _Image.MAX_IMAGE_PIXELS = None #type: ignore
 
 from ._utils import get_minio_client as _get_minio_client
 from ._config import Config as _Config #type: ignore
 
 
-_NUM_PARALLEL_UPLOADS = _Config._MINIO_NUM_PARALLEL_UPLOADS
-
 # Need to include rpy stubs
 try: 
     import rpy2 as _rpy2 
     from rpy2 import robjects as _ro
     _RPY2_AVAILABLE = True
 except:
     _RPY2_AVAILABLE = False
@@ -197,22 +195,22 @@
             # write to buffer
             _tifffile.imwrite(b_out,_np.array(img),compression='zlib')
             # get bytes from buffer
             b_upload = _BytesIO(b_out.getvalue())
             
             # temporary
             bucket_name =_Config._MINIO_WORKFLOW_BUCKET
-            
+            NUM_PARALLEL_UPLOADS= ''
             
             client = _get_minio_client()
             client.put_object(
                 bucket_name=bucket_name, #perhaps use an environment variable?
                 object_name=prefix+image_name+cls.FILE_EXTENSION, #filename + sudopath 'x/core/filename.ome.tiff'
                 data=b_upload,
-                num_parallel_uploads=_NUM_PARALLEL_UPLOADS, #ENV Variable for setting the number of parallel uploads MINIO can use
+                num_parallel_uploads=NUM_PARALLEL_UPLOADS, #ENV Variable for setting the number of parallel uploads MINIO can use
                 length=b_upload.getbuffer().nbytes
             )
             
             del b_out, b_upload
             
             url = client.get_presigned_url('GET',bucket_name,prefix+image_name+cls.FILE_EXTENSION)
         
@@ -259,22 +257,22 @@
             # write to buffer
             df.to_csv(b_out)
             # get bytes from buffer - from here down could be abstracted
             b_upload = _BytesIO(b_out.getvalue())
 
             # temporary - 
             bucket_name = _Config._MINIO_WORKFLOW_BUCKET
-            
+            NUM_PARALLEL_UPLOADS= ''
             
             client = _get_minio_client()
             client.put_object(
                 bucket_name=bucket_name, #perhaps use an environment variable?
                 object_name=prefix+filename+cls.FILE_EXTENSION, #filename + sudopath 'x/core/filename.ome.tiff'
                 data=b_upload,
-                num_parallel_uploads=_NUM_PARALLEL_UPLOADS, #ENV Variable for setting the number of parallel uploads MINIO can use
+                num_parallel_uploads=NUM_PARALLEL_UPLOADS, #ENV Variable for setting the number of parallel uploads MINIO can use
                 length=b_upload.getbuffer().nbytes
             )
             
             del b_out, b_upload
             
             url = client.get_presigned_url('GET',bucket_name,prefix+filename+cls.FILE_EXTENSION)
         
@@ -343,22 +341,22 @@
             img.save(b_out,'PNG')
             # _tifffile.imwrite(b_out,np.array(img),compression='zlib')
             # get bytes from buffer
             b_upload = _BytesIO(b_out.getvalue())
             
             # temporary
             bucket_name =_Config._MINIO_WORKFLOW_BUCKET
-            
+            NUM_PARALLEL_UPLOADS= ''
             
             client = _get_minio_client()
             client.put_object(
                 bucket_name=bucket_name, #perhaps use an environment variable?
                 object_name=prefix+image_name+cls.FILE_EXTENSION, #filename + sudopath 'x/core/filename.ome.tiff'
                 data=b_upload,
-                num_parallel_uploads=_NUM_PARALLEL_UPLOADS, #ENV Variable for setting the number of parallel uploads MINIO can use
+                num_parallel_uploads=NUM_PARALLEL_UPLOADS, #ENV Variable for setting the number of parallel uploads MINIO can use
                 length=b_upload.getbuffer().nbytes
             )
             
             del b_out, b_upload
             
             url = client.get_presigned_url('GET',bucket_name,prefix+image_name+cls.FILE_EXTENSION)
         
@@ -373,15 +371,14 @@
     def read(self) -> _Union[_Image.Image, _TiffImagePlugin.TiffImageFile]:
         if _Config.DEBUG():
             return _Image.open(self.url)
         else:
             response = _requests.get(self.url)
             return _Image.open(_BytesIO(response.content))
         
-    # TO DO -> FIX THIS TO REFLECT K8S
     def get_external_url(self) -> str:
         target = _os.environ.get('REVERSE-PROXY-HOST')
         port = _os.environ.get('REVERSE-PROXY-PORT')
         parsed_url = _urlparse(self.url)
         return parsed_url._replace(netloc=f"{target}:{port}").geturl()
```

### Comparing `cellmaps_sdk-0.0.15/src/cellmaps_sdk/data_utils.py` & `cellmaps-sdk-0.0.2/src/cellmaps_sdk/data_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.15/src/cellmaps_sdk/process.py` & `cellmaps-sdk-0.0.2/src/cellmaps_sdk/process.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.15/src/cellmaps_sdk.egg-info/PKG-INFO` & `cellmaps-sdk-0.0.2/src/cellmaps_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: cellmaps-sdk
-Version: 0.0.15
+Version: 0.0.2
 Summary: The SDK for tool builders who wish to integrate their tool into the CellMaps Analysis Workflow IME
 Author-email: Colm Brandon <colm.brandon@ul.ie>
 Project-URL: Homepage, http://example.com
 Project-URL: Documentation, http://example.com
 Project-URL: Repository, http://example.com
 Project-URL: Bug Tracker, http://example.com
 Project-URL: Changelog, http://example.com
 Keywords: Highly-plexed Tissue Imaging,AI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: requests
```

### Comparing `cellmaps_sdk-0.0.15/src/cellmaps_sdk.egg-info/SOURCES.txt` & `cellmaps-sdk-0.0.2/src/cellmaps_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE.txt
 README.rst
 pyproject.toml
 src/cellmaps_sdk/__init__.py
 src/cellmaps_sdk/__main__.py
 src/cellmaps_sdk/_cli_utils.py
 src/cellmaps_sdk/_config.py
-src/cellmaps_sdk/_raw_data.py
 src/cellmaps_sdk/_test_utils.py
 src/cellmaps_sdk/_utils.py
 src/cellmaps_sdk/data.py
 src/cellmaps_sdk/data_utils.py
 src/cellmaps_sdk/process.py
 src/cellmaps_sdk/py.typed
 src/cellmaps_sdk.egg-info/PKG-INFO
```

