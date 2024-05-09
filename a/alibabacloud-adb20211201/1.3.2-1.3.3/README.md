# Comparing `tmp/alibabacloud_adb20211201-1.3.2.tar.gz` & `tmp/alibabacloud_adb20211201-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_adb20211201-1.3.2.tar", last modified: Tue Apr  9 17:13:38 2024, max compression
+gzip compressed data, was "dist/alibabacloud_adb20211201-1.3.3.tar", last modified: Wed Apr 10 17:11:51 2024, max compression
```

## Comparing `alibabacloud_adb20211201-1.3.2.tar` & `alibabacloud_adb20211201-1.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/
--rw-r--r--   0 root         (0) root         (0)     2068 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2401 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201/__init__.py
--rw-r--r--   0 root         (0) root         (0)   432546 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201/client.py
--rw-r--r--   0 root         (0) root         (0)   920205 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2401 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2024-04-09 17:13:38.000000 alibabacloud_adb20211201-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/
+-rw-r--r--   0 root         (0) root         (0)     2134 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   432974 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201/client.py
+-rw-r--r--   0 root         (0) root         (0)   920707 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/setup.py
```

### Comparing `alibabacloud_adb20211201-1.3.2/ChangeLog.md` & `alibabacloud_adb20211201-1.3.3/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-04-09 Version: 1.3.2
+- Generated python 2021-12-01 for adb.
+
 2024-03-25 Version: 1.3.1
 - Update API CreateDBResourceGroup: add param Rules.
 - Update API DescribeDBResourceGroup: update response param.
 - Update API ModifyDBResourceGroup: add param Rules.
 
 
 2024-03-23 Version: 1.3.0
```

### Comparing `alibabacloud_adb20211201-1.3.2/LICENSE` & `alibabacloud_adb20211201-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201-1.3.2/PKG-INFO` & `alibabacloud_adb20211201-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_adb20211201
-Version: 1.3.2
+Version: 1.3.3
 Summary: Alibaba Cloud adb (20211201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adb20211201-1.3.2/README-CN.md` & `alibabacloud_adb20211201-1.3.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201-1.3.2/README.md` & `alibabacloud_adb20211201-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201/client.py` & `alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2506,14 +2506,18 @@
         request: adb_20211201_models.DescribeApsResourceGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> adb_20211201_models.DescribeApsResourceGroupsResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             body['DBClusterId'] = request.dbcluster_id
+        if not UtilClient.is_unset(request.region_id):
+            body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.workload_id):
+            body['WorkloadId'] = request.workload_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeApsResourceGroups',
             version='2021-12-01',
             protocol='HTTPS',
@@ -2534,14 +2538,18 @@
         request: adb_20211201_models.DescribeApsResourceGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> adb_20211201_models.DescribeApsResourceGroupsResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             body['DBClusterId'] = request.dbcluster_id
+        if not UtilClient.is_unset(request.region_id):
+            body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.workload_id):
+            body['WorkloadId'] = request.workload_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DescribeApsResourceGroups',
             version='2021-12-01',
             protocol='HTTPS',
```

### Comparing `alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201/models.py` & `alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7105,37 +7105,49 @@
         return self
 
 
 class DescribeApsResourceGroupsRequest(TeaModel):
     def __init__(
         self,
         dbcluster_id: str = None,
+        region_id: str = None,
+        workload_id: str = None,
     ):
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         # 
         # >  You can call the [DescribeDBClusters](~~612397~~) operation to query the IDs of all AnalyticDB for MySQL Data Lakehouse Edition (V3.0) clusters within a region.
         self.dbcluster_id = dbcluster_id
+        self.region_id = region_id
+        self.workload_id = workload_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.dbcluster_id is not None:
             result['DBClusterId'] = self.dbcluster_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.workload_id is not None:
+            result['WorkloadId'] = self.workload_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('DBClusterId') is not None:
             self.dbcluster_id = m.get('DBClusterId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('WorkloadId') is not None:
+            self.workload_id = m.get('WorkloadId')
         return self
 
 
 class DescribeApsResourceGroupsResponseBodyDataResourceGroups(TeaModel):
     def __init__(
         self,
         available: bool = None,
```

### Comparing `alibabacloud_adb20211201-1.3.2/alibabacloud_adb20211201.egg-info/PKG-INFO` & `alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-adb20211201
-Version: 1.3.2
+Version: 1.3.3
 Summary: Alibaba Cloud adb (20211201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adb20211201-1.3.2/setup.py` & `alibabacloud_adb20211201-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_adb20211201.
 
-Created on 09/04/2024
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_adb20211201"
 NAME = "alibabacloud_adb20211201" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud adb (20211201) SDK Library for Python"
```

