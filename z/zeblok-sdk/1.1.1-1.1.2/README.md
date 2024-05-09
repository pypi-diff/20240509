# Comparing `tmp/zeblok_sdk-1.1.1.tar.gz` & `tmp/zeblok_sdk-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeblok_sdk-1.1.1.tar", last modified: Wed May  8 04:11:47 2024, max compression
+gzip compressed data, was "zeblok_sdk-1.1.2.tar", last modified: Thu May  9 17:19:00 2024, max compression
```

## Comparing `zeblok_sdk-1.1.1.tar` & `zeblok_sdk-1.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:47.966150 zeblok_sdk-1.1.1/
--rw-rw-rw-   0        0        0      158 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.1/LICENSE.md
--rw-rw-rw-   0        0        0     3730 2024-05-08 04:11:47.965147 zeblok_sdk-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3302 2024-05-04 04:55:41.000000 zeblok_sdk-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 04:11:47.966150 zeblok_sdk-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      876 2024-05-04 04:40:25.000000 zeblok_sdk-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:47.917597 zeblok_sdk-1.1.1/tests/
--rw-rw-rw-   0        0        0     3913 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.1/tests/test_auth.py
--rw-rw-rw-   0        0        0     3107 2024-04-05 01:26:57.000000 zeblok_sdk-1.1.1/tests/test_namespace.py
--rw-rw-rw-   0        0        0     7198 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.1/tests/test_orchestration.py
--rw-rw-rw-   0        0        0    13891 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.1/tests/test_plan.py
--rw-rw-rw-   0        0        0     9559 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.1/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:47.933167 zeblok_sdk-1.1.1/zeblok/
--rw-rw-rw-   0        0        0      406 2024-05-07 09:16:30.000000 zeblok_sdk-1.1.1/zeblok/__init__.py
--rw-rw-rw-   0        0        0     9679 2024-05-02 05:12:43.000000 zeblok_sdk-1.1.1/zeblok/api.py
--rw-rw-rw-   0        0        0     2490 2023-12-20 09:11:18.000000 zeblok_sdk-1.1.1/zeblok/auth.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:47.942945 zeblok_sdk-1.1.1/zeblok/base/
--rw-rw-rw-   0        0        0        0 2023-11-21 08:39:11.000000 zeblok_sdk-1.1.1/zeblok/base/__init__.py
--rw-rw-rw-   0        0        0     3493 2024-04-10 10:49:32.000000 zeblok_sdk-1.1.1/zeblok/base/base_airuns.py
--rw-rw-rw-   0        0        0     1057 2023-12-20 15:23:23.000000 zeblok_sdk-1.1.1/zeblok/base/base_auth.py
--rw-rw-rw-   0        0        0     5250 2024-05-01 05:23:24.000000 zeblok_sdk-1.1.1/zeblok/base/base_dataset.py
--rw-rw-rw-   0        0        0     1535 2024-04-05 00:33:45.000000 zeblok_sdk-1.1.1/zeblok/base/base_service.py
--rw-rw-rw-   0        0        0      292 2023-11-23 06:00:40.000000 zeblok_sdk-1.1.1/zeblok/base/base_zbl.py
--rw-rw-rw-   0        0        0    10366 2024-05-07 09:04:39.000000 zeblok_sdk-1.1.1/zeblok/dataset.py
--rw-rw-rw-   0        0        0     8945 2024-04-05 00:33:45.000000 zeblok_sdk-1.1.1/zeblok/microservice.py
--rw-rw-rw-   0        0        0     4720 2023-12-20 09:11:18.000000 zeblok_sdk-1.1.1/zeblok/namespace.py
--rw-rw-rw-   0        0        0     8274 2024-05-03 08:09:55.000000 zeblok_sdk-1.1.1/zeblok/orchestration.py
--rw-rw-rw-   0        0        0    14379 2024-05-03 07:28:33.000000 zeblok_sdk-1.1.1/zeblok/pipeline.py
--rw-rw-rw-   0        0        0     6569 2024-05-03 10:47:22.000000 zeblok_sdk-1.1.1/zeblok/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:47.953529 zeblok_sdk-1.1.1/zeblok/utils/
--rw-rw-rw-   0        0        0        0 2023-11-15 02:39:00.000000 zeblok_sdk-1.1.1/zeblok/utils/__init__.py
--rw-rw-rw-   0        0        0     3261 2024-03-30 04:04:56.000000 zeblok_sdk-1.1.1/zeblok/utils/error_message.py
--rw-rw-rw-   0        0        0     3045 2024-05-07 08:40:36.000000 zeblok_sdk-1.1.1/zeblok/utils/errors.py
--rw-rw-rw-   0        0        0      727 2023-11-02 04:35:55.000000 zeblok_sdk-1.1.1/zeblok/utils/misc.py
--rw-rw-rw-   0        0        0     5347 2023-11-15 02:39:40.000000 zeblok_sdk-1.1.1/zeblok/utils/progressbar.py
--rw-rw-rw-   0        0        0    13599 2024-04-28 03:10:00.000000 zeblok_sdk-1.1.1/zeblok/utils/validations.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:47.964137 zeblok_sdk-1.1.1/zeblok_sdk.egg-info/
--rw-rw-rw-   0        0        0     3730 2024-05-08 04:11:47.000000 zeblok_sdk-1.1.1/zeblok_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      786 2024-05-08 04:11:47.000000 zeblok_sdk-1.1.1/zeblok_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 04:11:47.000000 zeblok_sdk-1.1.1/zeblok_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-08 04:11:47.000000 zeblok_sdk-1.1.1/zeblok_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-08 04:11:47.000000 zeblok_sdk-1.1.1/zeblok_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 17:19:00.534355 zeblok_sdk-1.1.2/
+-rw-rw-rw-   0        0        0      158 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0     3730 2024-05-09 17:19:00.533351 zeblok_sdk-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3302 2024-05-04 04:55:41.000000 zeblok_sdk-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-09 17:19:00.534355 zeblok_sdk-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      799 2024-05-08 04:30:06.000000 zeblok_sdk-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:19:00.487514 zeblok_sdk-1.1.2/tests/
+-rw-rw-rw-   0        0        0     3913 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.2/tests/test_auth.py
+-rw-rw-rw-   0        0        0     3107 2024-04-05 01:26:57.000000 zeblok_sdk-1.1.2/tests/test_namespace.py
+-rw-rw-rw-   0        0        0     7198 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.2/tests/test_orchestration.py
+-rw-rw-rw-   0        0        0    13891 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.2/tests/test_plan.py
+-rw-rw-rw-   0        0        0     9559 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:19:00.503513 zeblok_sdk-1.1.2/zeblok/
+-rw-rw-rw-   0        0        0      406 2024-05-09 17:14:24.000000 zeblok_sdk-1.1.2/zeblok/__init__.py
+-rw-rw-rw-   0        0        0     9679 2024-05-02 05:12:43.000000 zeblok_sdk-1.1.2/zeblok/api.py
+-rw-rw-rw-   0        0        0     2490 2023-12-20 09:11:18.000000 zeblok_sdk-1.1.2/zeblok/auth.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:19:00.512458 zeblok_sdk-1.1.2/zeblok/base/
+-rw-rw-rw-   0        0        0        0 2023-11-21 08:39:11.000000 zeblok_sdk-1.1.2/zeblok/base/__init__.py
+-rw-rw-rw-   0        0        0     3493 2024-04-10 10:49:32.000000 zeblok_sdk-1.1.2/zeblok/base/base_airuns.py
+-rw-rw-rw-   0        0        0     1057 2023-12-20 15:23:23.000000 zeblok_sdk-1.1.2/zeblok/base/base_auth.py
+-rw-rw-rw-   0        0        0     5250 2024-05-01 05:23:24.000000 zeblok_sdk-1.1.2/zeblok/base/base_dataset.py
+-rw-rw-rw-   0        0        0     1535 2024-04-05 00:33:45.000000 zeblok_sdk-1.1.2/zeblok/base/base_service.py
+-rw-rw-rw-   0        0        0      292 2023-11-23 06:00:40.000000 zeblok_sdk-1.1.2/zeblok/base/base_zbl.py
+-rw-rw-rw-   0        0        0    10470 2024-05-09 17:17:28.000000 zeblok_sdk-1.1.2/zeblok/dataset.py
+-rw-rw-rw-   0        0        0     8945 2024-04-05 00:33:45.000000 zeblok_sdk-1.1.2/zeblok/microservice.py
+-rw-rw-rw-   0        0        0     4720 2023-12-20 09:11:18.000000 zeblok_sdk-1.1.2/zeblok/namespace.py
+-rw-rw-rw-   0        0        0     8274 2024-05-03 08:09:55.000000 zeblok_sdk-1.1.2/zeblok/orchestration.py
+-rw-rw-rw-   0        0        0    14379 2024-05-03 07:28:33.000000 zeblok_sdk-1.1.2/zeblok/pipeline.py
+-rw-rw-rw-   0        0        0     6569 2024-05-03 10:47:22.000000 zeblok_sdk-1.1.2/zeblok/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:19:00.521601 zeblok_sdk-1.1.2/zeblok/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-15 02:39:00.000000 zeblok_sdk-1.1.2/zeblok/utils/__init__.py
+-rw-rw-rw-   0        0        0     3261 2024-03-30 04:04:56.000000 zeblok_sdk-1.1.2/zeblok/utils/error_message.py
+-rw-rw-rw-   0        0        0     3045 2024-05-07 08:40:36.000000 zeblok_sdk-1.1.2/zeblok/utils/errors.py
+-rw-rw-rw-   0        0        0      727 2023-11-02 04:35:55.000000 zeblok_sdk-1.1.2/zeblok/utils/misc.py
+-rw-rw-rw-   0        0        0     5347 2023-11-15 02:39:40.000000 zeblok_sdk-1.1.2/zeblok/utils/progressbar.py
+-rw-rw-rw-   0        0        0    13599 2024-04-28 03:10:00.000000 zeblok_sdk-1.1.2/zeblok/utils/validations.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:19:00.532226 zeblok_sdk-1.1.2/zeblok_sdk.egg-info/
+-rw-rw-rw-   0        0        0     3730 2024-05-09 17:19:00.000000 zeblok_sdk-1.1.2/zeblok_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      786 2024-05-09 17:19:00.000000 zeblok_sdk-1.1.2/zeblok_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 17:19:00.000000 zeblok_sdk-1.1.2/zeblok_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-09 17:19:00.000000 zeblok_sdk-1.1.2/zeblok_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-09 17:19:00.000000 zeblok_sdk-1.1.2/zeblok_sdk.egg-info/top_level.txt
```

### Comparing `zeblok_sdk-1.1.1/PKG-INFO` & `zeblok_sdk-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeblok-sdk
-Version: 1.1.1
+Version: 1.1.2
 Summary: Zeblok Python SDK
 Home-page: 
 Author: Karan Pathak
 Author-email: karan@dataturtles.com
 Keywords: python,zeblok
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `zeblok_sdk-1.1.1/README.md` & `zeblok_sdk-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/setup.py` & `zeblok_sdk-1.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pip._internal.req import parse_requirements
 from setuptools import setup, find_packages
 from pathlib import Path
 import zeblok
 
 DESCRIPTION = 'Zeblok Python SDK'
-# LONG_DESCRIPTION = 'Zeblok Python SDK to interact the Zeblok Ai-MicroCloud'
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+
 setup(
     name="zeblok-sdk",
     version=zeblok.__version__,
     author="Karan Pathak",
     author_email="karan@dataturtles.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

### Comparing `zeblok_sdk-1.1.1/tests/test_auth.py` & `zeblok_sdk-1.1.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/tests/test_namespace.py` & `zeblok_sdk-1.1.2/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/tests/test_orchestration.py` & `zeblok_sdk-1.1.2/tests/test_orchestration.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/tests/test_plan.py` & `zeblok_sdk-1.1.2/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/tests/test_utils.py` & `zeblok_sdk-1.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/api.py` & `zeblok_sdk-1.1.2/zeblok/api.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/auth.py` & `zeblok_sdk-1.1.2/zeblok/auth.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/base/base_airuns.py` & `zeblok_sdk-1.1.2/zeblok/base/base_airuns.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/base/base_auth.py` & `zeblok_sdk-1.1.2/zeblok/base/base_auth.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/base/base_dataset.py` & `zeblok_sdk-1.1.2/zeblok/base/base_dataset.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/base/base_service.py` & `zeblok_sdk-1.1.2/zeblok/base/base_service.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/dataset.py` & `zeblok_sdk-1.1.2/zeblok/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from datetime import datetime, timedelta
 
 
 class AwsS3(DataSetBase):
     def __init__(self, access_key: str, secret_key: str, bucket_name: str):
         init_params = {
             'aws_access_key_id': access_key, 'aws_secret_access_key': secret_key,
+            'config': boto3.session.Config(signature_version='s3v4', s3={'addressing_style': 'path'}),
         }
         self.__s3_client = boto3.client('s3', **init_params)
         super().__init__(access_key=access_key, access_secret=secret_key, bucket_name=bucket_name)
 
         self.__update_client_with_region(init_params=init_params)
 
     def __update_client_with_region(self, init_params: Dict) -> None:
```

### Comparing `zeblok_sdk-1.1.1/zeblok/microservice.py` & `zeblok_sdk-1.1.2/zeblok/microservice.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/namespace.py` & `zeblok_sdk-1.1.2/zeblok/namespace.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/orchestration.py` & `zeblok_sdk-1.1.2/zeblok/orchestration.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/pipeline.py` & `zeblok_sdk-1.1.2/zeblok/pipeline.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/plan.py` & `zeblok_sdk-1.1.2/zeblok/plan.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/utils/error_message.py` & `zeblok_sdk-1.1.2/zeblok/utils/error_message.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/utils/errors.py` & `zeblok_sdk-1.1.2/zeblok/utils/errors.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/utils/misc.py` & `zeblok_sdk-1.1.2/zeblok/utils/misc.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/utils/progressbar.py` & `zeblok_sdk-1.1.2/zeblok/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok/utils/validations.py` & `zeblok_sdk-1.1.2/zeblok/utils/validations.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.1/zeblok_sdk.egg-info/PKG-INFO` & `zeblok_sdk-1.1.2/zeblok_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeblok-sdk
-Version: 1.1.1
+Version: 1.1.2
 Summary: Zeblok Python SDK
 Home-page: 
 Author: Karan Pathak
 Author-email: karan@dataturtles.com
 Keywords: python,zeblok
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `zeblok_sdk-1.1.1/zeblok_sdk.egg-info/SOURCES.txt` & `zeblok_sdk-1.1.2/zeblok_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

