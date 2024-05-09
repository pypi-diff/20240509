# Comparing `tmp/connector2-0.2.0.tar.gz` & `tmp/connector2-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connector2-0.2.0.tar", last modified: Tue May  7 20:53:25 2024, max compression
+gzip compressed data, was "connector2-0.2.1.tar", last modified: Wed May  8 18:37:26 2024, max compression
```

## Comparing `connector2-0.2.0.tar` & `connector2-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 tsingh     (501) staff       (20)        0 2024-05-07 20:53:25.917965 connector2-0.2.0/
--rw-r--r--   0 tsingh     (501) staff       (20)     1074 2023-07-21 17:38:20.000000 connector2-0.2.0/LICENSE.md
--rw-r--r--   0 tsingh     (501) staff       (20)     7304 2024-05-07 20:53:25.917897 connector2-0.2.0/PKG-INFO
--rw-r--r--   0 tsingh     (501) staff       (20)     6874 2024-05-07 20:52:32.000000 connector2-0.2.0/README.md
-drwxr-xr-x   0 tsingh     (501) staff       (20)        0 2024-05-07 20:53:25.916745 connector2-0.2.0/connector/
--rw-r--r--   0 tsingh     (501) staff       (20)      981 2023-08-18 18:00:00.000000 connector2-0.2.0/connector/__init__.py
--rw-r--r--   0 tsingh     (501) staff       (20)      497 2024-05-07 20:53:25.918258 connector2-0.2.0/connector/_version.py
--rw-r--r--   0 tsingh     (501) staff       (20)     7726 2024-05-07 18:46:19.000000 connector2-0.2.0/connector/cli.py
--rw-r--r--   0 tsingh     (501) staff       (20)     1080 2023-10-11 15:52:29.000000 connector2-0.2.0/connector/googlecloud.py
--rw-r--r--   0 tsingh     (501) staff       (20)     1774 2024-05-07 18:46:19.000000 connector2-0.2.0/connector/googledrive.py
--rw-r--r--   0 tsingh     (501) staff       (20)     5059 2023-10-14 23:34:20.000000 connector2-0.2.0/connector/init_conda_env.py
--rw-r--r--   0 tsingh     (501) staff       (20)     1457 2023-08-25 18:26:17.000000 connector2-0.2.0/connector/remote.py
--rw-r--r--   0 tsingh     (501) staff       (20)     1896 2023-08-25 17:59:10.000000 connector2-0.2.0/connector/restricted.py
-drwxr-xr-x   0 tsingh     (501) staff       (20)        0 2024-05-07 20:53:25.917670 connector2-0.2.0/connector2.egg-info/
--rw-r--r--   0 tsingh     (501) staff       (20)     7304 2024-05-07 20:53:25.000000 connector2-0.2.0/connector2.egg-info/PKG-INFO
--rw-r--r--   0 tsingh     (501) staff       (20)      442 2024-05-07 20:53:25.000000 connector2-0.2.0/connector2.egg-info/SOURCES.txt
--rw-r--r--   0 tsingh     (501) staff       (20)        1 2024-05-07 20:53:25.000000 connector2-0.2.0/connector2.egg-info/dependency_links.txt
--rw-r--r--   0 tsingh     (501) staff       (20)       81 2024-05-07 20:53:25.000000 connector2-0.2.0/connector2.egg-info/entry_points.txt
--rw-r--r--   0 tsingh     (501) staff       (20)       47 2024-05-07 20:53:25.000000 connector2-0.2.0/connector2.egg-info/requires.txt
--rw-r--r--   0 tsingh     (501) staff       (20)       10 2024-05-07 20:53:25.000000 connector2-0.2.0/connector2.egg-info/top_level.txt
--rw-r--r--   0 tsingh     (501) staff       (20)      208 2024-05-07 20:53:25.918166 connector2-0.2.0/setup.cfg
--rw-r--r--   0 tsingh     (501) staff       (20)      984 2024-05-07 20:51:21.000000 connector2-0.2.0/setup.py
--rw-r--r--   0 tsingh     (501) staff       (20)    86677 2023-08-18 18:00:00.000000 connector2-0.2.0/versioneer.py
+drwxr-xr-x   0 tsingh     (501) staff       (20)        0 2024-05-08 18:37:26.912464 connector2-0.2.1/
+-rw-r--r--   0 tsingh     (501) staff       (20)     1074 2023-07-21 17:38:20.000000 connector2-0.2.1/LICENSE.md
+-rw-r--r--   0 tsingh     (501) staff       (20)     7354 2024-05-08 18:37:26.912401 connector2-0.2.1/PKG-INFO
+-rw-r--r--   0 tsingh     (501) staff       (20)     6925 2024-05-08 15:27:29.000000 connector2-0.2.1/README.md
+drwxr-xr-x   0 tsingh     (501) staff       (20)        0 2024-05-08 18:37:26.911267 connector2-0.2.1/connector/
+-rw-r--r--   0 tsingh     (501) staff       (20)      981 2023-08-18 18:00:00.000000 connector2-0.2.1/connector/__init__.py
+-rw-r--r--   0 tsingh     (501) staff       (20)      497 2024-05-08 18:37:26.912772 connector2-0.2.1/connector/_version.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     7726 2024-05-07 18:46:19.000000 connector2-0.2.1/connector/cli.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     1277 2024-05-08 18:36:41.000000 connector2-0.2.1/connector/googlecloud.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     2086 2024-05-08 18:36:41.000000 connector2-0.2.1/connector/googledrive.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     5371 2024-05-08 15:27:29.000000 connector2-0.2.1/connector/init_conda_env.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     1645 2024-05-08 18:36:41.000000 connector2-0.2.1/connector/remote.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     1896 2023-08-25 17:59:10.000000 connector2-0.2.1/connector/restricted.py
+-rw-r--r--   0 tsingh     (501) staff       (20)     1993 2024-05-08 18:36:41.000000 connector2-0.2.1/connector/utils.py
+drwxr-xr-x   0 tsingh     (501) staff       (20)        0 2024-05-08 18:37:26.912164 connector2-0.2.1/connector2.egg-info/
+-rw-r--r--   0 tsingh     (501) staff       (20)     7354 2024-05-08 18:37:26.000000 connector2-0.2.1/connector2.egg-info/PKG-INFO
+-rw-r--r--   0 tsingh     (501) staff       (20)      461 2024-05-08 18:37:26.000000 connector2-0.2.1/connector2.egg-info/SOURCES.txt
+-rw-r--r--   0 tsingh     (501) staff       (20)        1 2024-05-08 18:37:26.000000 connector2-0.2.1/connector2.egg-info/dependency_links.txt
+-rw-r--r--   0 tsingh     (501) staff       (20)       81 2024-05-08 18:37:26.000000 connector2-0.2.1/connector2.egg-info/entry_points.txt
+-rw-r--r--   0 tsingh     (501) staff       (20)       47 2024-05-08 18:37:26.000000 connector2-0.2.1/connector2.egg-info/requires.txt
+-rw-r--r--   0 tsingh     (501) staff       (20)       10 2024-05-08 18:37:26.000000 connector2-0.2.1/connector2.egg-info/top_level.txt
+-rw-r--r--   0 tsingh     (501) staff       (20)      208 2024-05-08 18:37:26.912670 connector2-0.2.1/setup.cfg
+-rw-r--r--   0 tsingh     (501) staff       (20)      984 2024-05-07 20:51:21.000000 connector2-0.2.1/setup.py
+-rw-r--r--   0 tsingh     (501) staff       (20)    86677 2023-08-18 18:00:00.000000 connector2-0.2.1/versioneer.py
```

### Comparing `connector2-0.2.0/LICENSE.md` & `connector2-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `connector2-0.2.0/PKG-INFO` & `connector2-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connector2
-Version: 0.2.0
+Version: 0.2.1
 Summary: Provides the default template for creating Python Package.
 Home-page: https://github.com/tjsinghlab/connector
 Author: Singh Lab
 Author-email: singhlab@nygenome.org
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -45,21 +45,22 @@
 
 However, I suggest you create an `.env` file in your root directory (`~`) with the following:
 
 ```
 HOME=/Users/[Your_Username]
 REMOTE_USER=[Your_Remote_Username]
 REMOTE_HOST=[Your_Remote_Host]
-GOOGLE_ROOT="/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]"
-MY_DRIVE="/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]/My Drive"
-SHARED_DRIVE="/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]/Shared Drives"
+GOOGLE_ROOT=/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]
+MY_DRIVE=/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]/My Drive
+SHARED_DRIVE=/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]/Shared Drives
 ONE_DRIVE="/Users/[Your_Username]/Library/CloudStorage/[Your_OneDrive_Account]"
 SLACK_USER_ID=[Your_Slack_User_ID]
 SLACK_BOT_TOKEN=[Your_Slack_Bot_Token]
 ```
+*Do not use quotes when specifying variables in `.env`*
 
 Within your conda environment, run `tcinit ~/.env` to load all the parameters into your conda environment.
 
 ### Project-specific parameters
 To configure your Conda environment, you'll need to set a few environment variables:
 
 1. `CLOUD_ROOT`: This is the base name of your Google bucket. For example, if your Google bucket URL is `gs://gpc_array`, then `CLOUD_ROOT` should be set to `gs://gpc_array`.
```

### Comparing `connector2-0.2.0/README.md` & `connector2-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,21 +30,22 @@
 
 However, I suggest you create an `.env` file in your root directory (`~`) with the following:
 
 ```
 HOME=/Users/[Your_Username]
 REMOTE_USER=[Your_Remote_Username]
 REMOTE_HOST=[Your_Remote_Host]
-GOOGLE_ROOT="/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]"
-MY_DRIVE="/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]/My Drive"
-SHARED_DRIVE="/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]/Shared Drives"
+GOOGLE_ROOT=/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]
+MY_DRIVE=/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]/My Drive
+SHARED_DRIVE=/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]/Shared Drives
 ONE_DRIVE="/Users/[Your_Username]/Library/CloudStorage/[Your_OneDrive_Account]"
 SLACK_USER_ID=[Your_Slack_User_ID]
 SLACK_BOT_TOKEN=[Your_Slack_Bot_Token]
 ```
+*Do not use quotes when specifying variables in `.env`*
 
 Within your conda environment, run `tcinit ~/.env` to load all the parameters into your conda environment.
 
 ### Project-specific parameters
 To configure your Conda environment, you'll need to set a few environment variables:
 
 1. `CLOUD_ROOT`: This is the base name of your Google bucket. For example, if your Google bucket URL is `gs://gpc_array`, then `CLOUD_ROOT` should be set to `gs://gpc_array`.
@@ -147,8 +148,8 @@
 
 ## Maintainer
 
 [Tarjinder Singh @ ts3475@cumc.columbia.edu](ts3475@cumc.columbia.edu)
 
 ## Acknowledgements
 
-## Release Notes
+## Release Notes
```

### Comparing `connector2-0.2.0/connector/__init__.py` & `connector2-0.2.1/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `connector2-0.2.0/connector/cli.py` & `connector2-0.2.1/connector/cli.py`

 * *Files identical despite different names*

### Comparing `connector2-0.2.0/connector/googlecloud.py` & `connector2-0.2.1/connector/googlecloud.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import re
 import os
 import subprocess
+from .utils import create_directory_for_path
 
 
 def sync_bucket(args):
     """Sync a local directory to a Google Cloud Storage bucket using gsutil."""
     try:
         drive_dir = f"{os.environ['CLOUD_ROOT']}"
         drive_dir = re.sub('^gs://', '', drive_dir)
     except KeyError:
         print('CLOUD_ROOT environment variable is not defined. Error...')
         exit()
+    if args.subdir.startswith('data/'):
+        raise ValueError('subdir argument cannot start with "data/".')
     local_dir = f"{args.folder}/{args.subdir}/"
     drive_dir = f"{drive_dir}/{args.folder}/{args.subdir}/"
     if args.open:
         subprocess.call(
             ['open', 'https://console.cloud.google.com/storage/browser/' + drive_dir])
         return
     if args.list:
         cmd = ["gsutil", "ls", f"gs://{drive_dir}"]
         subprocess.run(cmd, check=True)
         return
+    create_directory_for_path(local_dir)
     cmd = ["gsutil", "-m", "rsync", "-x",
            ".*\.ht|.*\.mt|.*\.vcf|.*\.log", "-r"]
     if args.debug:
         cmd.append("-n")
     if args.dir == 'up':
         cmd.extend([local_dir, f"gs://{drive_dir}"])
     else:
```

### Comparing `connector2-0.2.0/connector/init_conda_env.py` & `connector2-0.2.1/connector/init_conda_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 """
 
 import argparse
 import subprocess
 import os
 from loguru import logger
 
+_keys = ["REMOTE_USER", "REMOTE_HOST", "GOOGLE_ROOT", "MY_DRIVE",
+         "SHARED_DRIVE", "ONE_DRIVE", "SLACK_USER_ID", "SLACK_BOT_TOKEN"]
 
 def set_conda_env_vars(env_file_path='.'):
     """
     Set environment variables for the active conda environment based on a file.
 
     Parameters
     ----------
@@ -76,17 +78,20 @@
         line = line.strip()
 
         # Skip comments and empty lines
         if line.startswith('#') or not line:
             continue
 
         try:
-            # Set environment variable for the active conda environment
-            subprocess.run(['conda', 'env', 'config',
-                            'vars', 'set', line], check=True)
+            # Set environment variable for the active conda environmen
+            key, value = line.split('=')[0], line.split('=')[1]
+            if key in _keys:
+                subprocess.run(['conda', 'env', 'config',
+                                'vars', 'set', f'{key}={value}'], check=True)
+                logger.info(f'Set variable: {key}={value}')
         except subprocess.CalledProcessError as e:
             print(f"Error setting variable: {line}")
             print(f"Error message: {e}")
             continue
 
     print("Remember to deactivate and reactivate your conda environment to apply changes.")
```

### Comparing `connector2-0.2.0/connector/remote.py` & `connector2-0.2.1/connector/remote.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os
 import subprocess
+from .utils import create_directory_for_path
 
 def sync_remote(args):
     """Sync a local directory to a remote cluster filesystem using rsync."""
     try:
         remote_dir = f"{os.environ['REMOTE_DIR']}" if args.remote_dir is None else args.remote_dir
     except KeyError:
         print('REMOTE_DIR environment variable is not defined. Error...')
-        exit()
-        
+        exit()   
     try:
         user = f"{os.environ['REMOTE_USER']}" if args.user is None else args.user
         host = f"{os.environ['REMOTE_HOST']}" if args.host is None else args.host
-    except:
+    except KeyError:
         print('REMOTE_USER or REMOTE_HOST environment variable is not defined. Error...')
-        exit()
-        
+        exit()       
     if args.list:
         ssh_cmd = ["ssh", f"{user}@{host}", f"ls -l {remote_dir}"]
         subprocess.run(ssh_cmd, check=True)
         return
-    
+    if args.subdir.startswith('data/'):
+        raise ValueError('subdir argument cannot start with "data/".')
     local_dir = f"{args.folder}/{args.subdir}/"
     remote_dir = f"{user}@{host}:{remote_dir}/{args.folder}/{args.subdir}/"
-    
+    create_directory_for_path(local_dir)
     cmd = ["rsync", "-avhW"]
     includes = ["--include=*.tsv", "--include=*.csv",
                 "--include=*.txt", "--include=*.xlsx", "--include=*/"]
     excludes = ["--exclude=*"]
     
     max_size = f"--max-size={args.max_size_mb}mb"
     if args.debug:
```

### Comparing `connector2-0.2.0/connector/restricted.py` & `connector2-0.2.1/connector/restricted.py`

 * *Files identical despite different names*

### Comparing `connector2-0.2.0/connector2.egg-info/PKG-INFO` & `connector2-0.2.1/connector2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connector2
-Version: 0.2.0
+Version: 0.2.1
 Summary: Provides the default template for creating Python Package.
 Home-page: https://github.com/tjsinghlab/connector
 Author: Singh Lab
 Author-email: singhlab@nygenome.org
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -45,21 +45,22 @@
 
 However, I suggest you create an `.env` file in your root directory (`~`) with the following:
 
 ```
 HOME=/Users/[Your_Username]
 REMOTE_USER=[Your_Remote_Username]
 REMOTE_HOST=[Your_Remote_Host]
-GOOGLE_ROOT="/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]"
-MY_DRIVE="/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]/My Drive"
-SHARED_DRIVE="/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]/Shared Drives"
+GOOGLE_ROOT=/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]
+MY_DRIVE=/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]/My Drive
+SHARED_DRIVE=/Users/[Your_Username]/Library/CloudStorage/[Your_GoogleDrive_Account]/Shared Drives
 ONE_DRIVE="/Users/[Your_Username]/Library/CloudStorage/[Your_OneDrive_Account]"
 SLACK_USER_ID=[Your_Slack_User_ID]
 SLACK_BOT_TOKEN=[Your_Slack_Bot_Token]
 ```
+*Do not use quotes when specifying variables in `.env`*
 
 Within your conda environment, run `tcinit ~/.env` to load all the parameters into your conda environment.
 
 ### Project-specific parameters
 To configure your Conda environment, you'll need to set a few environment variables:
 
 1. `CLOUD_ROOT`: This is the base name of your Google bucket. For example, if your Google bucket URL is `gs://gpc_array`, then `CLOUD_ROOT` should be set to `gs://gpc_array`.
```

### Comparing `connector2-0.2.0/setup.py` & `connector2-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `connector2-0.2.0/versioneer.py` & `connector2-0.2.1/versioneer.py`

 * *Files identical despite different names*

