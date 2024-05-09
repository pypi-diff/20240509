# Comparing `tmp/shipyard_s3-0.1.5a0.tar.gz` & `tmp/shipyard_s3-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_s3-0.1.5a0.tar", max compression
+gzip compressed data, was "shipyard_s3-0.2.0a0.tar", max compression
```

## Comparing `shipyard_s3-0.1.5a0.tar` & `shipyard_s3-0.2.0a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.839785 shipyard_s3-0.1.5a0/README.md
--rw-r--r--   0        0        0      629 2024-05-02 20:31:07.798494 shipyard_s3-0.1.5a0/pyproject.toml
--rw-r--r--   0        0        0       25 2023-05-12 18:48:21.840305 shipyard_s3-0.1.5a0/shipyard_s3/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.447197 shipyard_s3-0.1.5a0/shipyard_s3/cli/__init__.py
--rw-r--r--   0        0        0      433 2024-05-02 20:30:30.260693 shipyard_s3-0.1.5a0/shipyard_s3/cli/authtest.py
--rw-r--r--   0        0        0     4894 2024-03-08 15:17:28.225079 shipyard_s3-0.1.5a0/shipyard_s3/cli/download.py
--rw-r--r--   0        0        0     5197 2024-02-27 15:08:25.023699 shipyard_s3-0.1.5a0/shipyard_s3/cli/move.py
--rw-r--r--   0        0        0     3308 2024-03-06 13:42:18.655104 shipyard_s3-0.1.5a0/shipyard_s3/cli/remove.py
--rw-r--r--   0        0        0     5792 2024-03-08 15:17:28.225579 shipyard_s3-0.1.5a0/shipyard_s3/cli/upload.py
--rw-r--r--   0        0        0     9351 2024-05-02 20:30:30.316826 shipyard_s3-0.1.5a0/shipyard_s3/s3.py
--rw-r--r--   0        0        0     2386 2024-03-08 15:17:28.226639 shipyard_s3-0.1.5a0/shipyard_s3/utils/exceptions.py
--rw-r--r--   0        0        0      781 2024-02-27 15:08:25.119517 shipyard_s3-0.1.5a0/shipyard_s3/utils/utils.py
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 shipyard_s3-0.1.5a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-14 16:50:02.445112 shipyard_s3-0.2.0a0/README.md
+-rw-r--r--   0        0        0      630 2024-05-09 15:12:30.135177 shipyard_s3-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0       25 2024-02-22 17:47:27.269473 shipyard_s3-0.2.0a0/shipyard_s3/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-08 19:26:38.974929 shipyard_s3-0.2.0a0/shipyard_s3/cli/__init__.py
+-rw-r--r--   0        0        0      433 2024-05-03 15:58:02.915963 shipyard_s3-0.2.0a0/shipyard_s3/cli/authtest.py
+-rw-r--r--   0        0        0     4672 2024-05-09 18:22:19.249046 shipyard_s3-0.2.0a0/shipyard_s3/cli/download.py
+-rw-r--r--   0        0        0     5197 2024-03-08 19:26:38.976765 shipyard_s3-0.2.0a0/shipyard_s3/cli/move.py
+-rw-r--r--   0        0        0     3308 2024-03-08 19:26:38.977450 shipyard_s3-0.2.0a0/shipyard_s3/cli/remove.py
+-rw-r--r--   0        0        0     5792 2024-04-18 03:07:13.734426 shipyard_s3-0.2.0a0/shipyard_s3/cli/upload.py
+-rw-r--r--   0        0        0     9351 2024-05-03 15:58:02.916608 shipyard_s3-0.2.0a0/shipyard_s3/s3.py
+-rw-r--r--   0        0        0     2386 2024-04-18 03:07:13.735477 shipyard_s3-0.2.0a0/shipyard_s3/utils/exceptions.py
+-rw-r--r--   0        0        0      781 2024-03-08 19:26:38.978780 shipyard_s3-0.2.0a0/shipyard_s3/utils/utils.py
+-rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 shipyard_s3-0.2.0a0/PKG-INFO
```

### Comparing `shipyard_s3-0.1.5a0/pyproject.toml` & `shipyard_s3-0.2.0a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "shipyard-s3"
-version = "0.1.5a0"
+version = "0.2.0a0"
 description = "A local client for connecting and working with AWS S3"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_s3"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "1.34.44"
-shipyard-templates = "0.6.2"
-shipyard-bp-utils = "^1.0.3"
+shipyard-templates = "^0.8.2"
+shipyard-bp-utils = "^1.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0"
 python-dotenv = "^1.0.1"
 black = "^24.2.0"
 
 [tool.pytest.ini_options]
```

### Comparing `shipyard_s3-0.1.5a0/shipyard_s3/cli/download.py` & `shipyard_s3-0.2.0a0/shipyard_s3/cli/download.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,23 +47,23 @@
 
 
 def main():
     try:
         args = get_args()
         bucket_name = args.bucket_name
         src_file = args.source_file_name
-        src_folder = (
-            shipyard.files.clean_folder_name(args.source_folder_name)
-            if args.source_folder_name
-            else None
-        )
+        src_folder = args.source_folder_name
+
+        src_path = shipyard.files.combine_folder_and_file_name(src_folder, src_file)
+
         match_type = args.source_file_name_match_type
         target_dir = shipyard.files.clean_folder_name(args.destination_folder_name)
 
-        shipyard.files.create_folder_if_dne(target_dir)
+        if args.destination_folder_name:
+            shipyard.files.create_folder_if_dne(target_dir)
 
         client = S3Client(
             aws_access_key=args.aws_access_key_id,
             aws_secret_access_key=args.aws_secret_access_key,
             region=args.aws_default_region,
         )
         client.connect()
@@ -102,21 +102,14 @@
                     s3_path=key_name,
                     dest_path=dest_path,
                 )
                 logger.info(
                     f"Successfully downloaded s3://{bucket_name}/{key_name} to {dest_path}"
                 )
         else:
-            if src_folder:
-                src_path = shipyard.files.combine_folder_and_file_name(
-                    folder_name=src_folder, file_name=src_file
-                )
-            else:
-                src_path = src_file
-
             dest_path = shipyard.files.determine_destination_full_path(
                 destination_folder_name=target_dir,
                 destination_file_name=args.destination_file_name,
                 source_full_path=src_path,
             )
             client.download(
                 bucket_name=bucket_name,
```

### Comparing `shipyard_s3-0.1.5a0/shipyard_s3/cli/move.py` & `shipyard_s3-0.2.0a0/shipyard_s3/cli/move.py`

 * *Files identical despite different names*

### Comparing `shipyard_s3-0.1.5a0/shipyard_s3/cli/remove.py` & `shipyard_s3-0.2.0a0/shipyard_s3/cli/remove.py`

 * *Files identical despite different names*

### Comparing `shipyard_s3-0.1.5a0/shipyard_s3/cli/upload.py` & `shipyard_s3-0.2.0a0/shipyard_s3/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_s3-0.1.5a0/shipyard_s3/s3.py` & `shipyard_s3-0.2.0a0/shipyard_s3/s3.py`

 * *Files identical despite different names*

### Comparing `shipyard_s3-0.1.5a0/shipyard_s3/utils/exceptions.py` & `shipyard_s3-0.2.0a0/shipyard_s3/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_s3-0.1.5a0/shipyard_s3/utils/utils.py` & `shipyard_s3-0.2.0a0/shipyard_s3/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_s3-0.1.5a0/PKG-INFO` & `shipyard_s3-0.2.0a0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: shipyard-s3
-Version: 0.1.5a0
+Version: 0.2.0a0
 Summary: A local client for connecting and working with AWS S3
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (==1.34.44)
-Requires-Dist: shipyard-bp-utils (>=1.0.3,<2.0.0)
-Requires-Dist: shipyard-templates (==0.6.2)
+Requires-Dist: shipyard-bp-utils (>=1.2.1,<2.0.0)
+Requires-Dist: shipyard-templates (>=0.8.2,<0.9.0)
 Description-Content-Type: text/markdown
```

