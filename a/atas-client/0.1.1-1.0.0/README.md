# Comparing `tmp/atas_client-0.1.1.tar.gz` & `tmp/atas_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atas_client-0.1.1.tar", last modified: Tue Apr 23 03:54:17 2024, max compression
+gzip compressed data, was "atas_client-1.0.0.tar", last modified: Thu May  9 02:08:28 2024, max compression
```

## Comparing `atas_client-0.1.1.tar` & `atas_client-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-04-23 03:54:17.298861 atas_client-0.1.1/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1073 2022-12-05 06:04:48.000000 atas_client-0.1.1/LICENSE
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2024-04-23 03:54:17.298573 atas_client-0.1.1/PKG-INFO
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       23 2022-12-05 06:50:55.000000 atas_client-0.1.1/README.md
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      551 2024-04-23 03:54:11.000000 atas_client-0.1.1/pyproject.toml
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       38 2024-04-23 03:54:17.298901 atas_client-0.1.1/setup.cfg
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-04-23 03:54:17.295044 atas_client-0.1.1/src/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:17.000000 atas_client-0.1.1/src/__init__.py
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-04-23 03:54:17.296558 atas_client-0.1.1/src/atas_client/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     2823 2024-04-23 03:53:07.000000 atas_client-0.1.1/src/atas_client/CoreATASApi.py
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1353 2024-03-29 01:25:29.000000 atas_client-0.1.1/src/atas_client/HttpUtil.py
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:10.000000 atas_client-0.1.1/src/atas_client/__init__.py
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1194 2024-04-23 03:53:07.000000 atas_client-0.1.1/src/atas_client/atas_client.py
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-04-23 03:54:17.298250 atas_client-0.1.1/src/atas_client.egg-info/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2024-04-23 03:54:17.000000 atas_client-0.1.1/src/atas_client.egg-info/PKG-INFO
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      322 2024-04-23 03:54:17.000000 atas_client-0.1.1/src/atas_client.egg-info/SOURCES.txt
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        1 2024-04-23 03:54:17.000000 atas_client-0.1.1/src/atas_client.egg-info/dependency_links.txt
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       21 2024-04-23 03:54:17.000000 atas_client-0.1.1/src/atas_client.egg-info/top_level.txt
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-05-09 02:08:28.185802 atas_client-1.0.0/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1073 2022-12-05 06:04:48.000000 atas_client-1.0.0/LICENSE
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2024-05-09 02:08:28.185487 atas_client-1.0.0/PKG-INFO
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       23 2022-12-05 06:50:55.000000 atas_client-1.0.0/README.md
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      551 2024-05-09 02:07:32.000000 atas_client-1.0.0/pyproject.toml
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       38 2024-05-09 02:08:28.185861 atas_client-1.0.0/setup.cfg
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-05-09 02:08:28.181288 atas_client-1.0.0/src/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:17.000000 atas_client-1.0.0/src/__init__.py
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-05-09 02:08:28.182739 atas_client-1.0.0/src/atas_client/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     3846 2024-05-09 02:05:51.000000 atas_client-1.0.0/src/atas_client/CoreATASApi.py
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1353 2024-03-29 01:25:29.000000 atas_client-1.0.0/src/atas_client/HttpUtil.py
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:10.000000 atas_client-1.0.0/src/atas_client/__init__.py
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1741 2024-05-09 02:07:32.000000 atas_client-1.0.0/src/atas_client/atas_client.py
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-05-09 02:08:28.185012 atas_client-1.0.0/src/atas_client.egg-info/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2024-05-09 02:08:28.000000 atas_client-1.0.0/src/atas_client.egg-info/PKG-INFO
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      322 2024-05-09 02:08:28.000000 atas_client-1.0.0/src/atas_client.egg-info/SOURCES.txt
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        1 2024-05-09 02:08:28.000000 atas_client-1.0.0/src/atas_client.egg-info/dependency_links.txt
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       21 2024-05-09 02:08:28.000000 atas_client-1.0.0/src/atas_client.egg-info/top_level.txt
```

### Comparing `atas_client-0.1.1/LICENSE` & `atas_client-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atas_client-0.1.1/PKG-INFO` & `atas_client-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atas_client
-Version: 0.1.1
+Version: 1.0.0
 Summary: ATAS Automation API
 Author-email: "tao.ding" <tao.ding@rakuten.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `atas_client-0.1.1/pyproject.toml` & `atas_client-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atas_client"
-version = "0.1.1"
+version = "1.0.0"
 authors = [
   { name="tao.ding", email="tao.ding@rakuten.com" },
 ]
 description = "ATAS Automation API"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `atas_client-0.1.1/src/atas_client/CoreATASApi.py` & `atas_client-1.0.0/src/atas_client/CoreATASApi.py`

 * *Files 16% similar despite different names*

```diff
@@ -67,7 +67,37 @@
         body = "{\"executionId\":\"" + id + "\"}"
         method = "post"
         try:
             res = HttpUtil.http_request(url, method, None, None, json.loads(body), headers=eval(headers))
         except Exception:
             raise
         return res
+
+    @staticmethod
+    def bulk_save_result(uri, token, data):
+        headers = "{\"Content-Type\": \"application/json;charset=UTF-8\",\"auth-key\": \"" + token + "\"}"
+        url = uri + "/automation/v2/launch/execute"
+        body = data
+        method = "post"
+        try:
+            res = HttpUtil.http_request(url, method, None, None, body, headers=eval(headers))
+        except Exception:
+            raise
+        return res
+
+    @staticmethod
+    def upload_attachment(uri, token, file_path):
+        url = uri + "/automation/v2/launch/upload"
+        if file_path is None:
+            attachment = ('file', (
+                '', '',
+                'image/png'))
+        else:
+            attachment = ('file', (
+                file_path[file_path.rindex("/") + 1:], open(file_path, 'rb'),
+                'image/png'))
+        files = [attachment]
+        try:
+            res = HttpUtil.http_multipart_request(url, None, files, auth_key=token)
+        except Exception:
+            raise
+        return res
```

### Comparing `atas_client-0.1.1/src/atas_client/HttpUtil.py` & `atas_client-1.0.0/src/atas_client/HttpUtil.py`

 * *Files identical despite different names*

### Comparing `atas_client-0.1.1/src/atas_client.egg-info/PKG-INFO` & `atas_client-1.0.0/src/atas_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atas_client
-Version: 0.1.1
+Version: 1.0.0
 Summary: ATAS Automation API
 Author-email: "tao.ding" <tao.ding@rakuten.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

