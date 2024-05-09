# Comparing `tmp/rknntools-0.0.2.tar.gz` & `tmp/rknntools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rknntools-0.0.2.tar", last modified: Thu Nov 23 08:09:33 2023, max compression
+gzip compressed data, was "rknntools-0.0.3.tar", last modified: Thu May  9 07:40:37 2024, max compression
```

## Comparing `rknntools-0.0.2.tar` & `rknntools-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-11-23 08:09:33.425133 rknntools-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-11-23 07:22:32.000000 rknntools-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2442 2023-11-23 08:09:33.424136 rknntools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-11-22 10:30:59.000000 rknntools-0.0.2/README.md
--rw-rw-rw-   0        0        0      581 2023-11-23 08:09:24.000000 rknntools-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-11-23 08:09:33.417154 rknntools-0.0.2/rknntools/
--rw-rw-rw-   0        0        0       35 2023-11-23 08:07:39.000000 rknntools-0.0.2/rknntools/__init__.py
--rw-rw-rw-   0        0        0     3318 2023-11-22 10:25:53.000000 rknntools-0.0.2/rknntools/op_limit.py
-drwxrwxrwx   0        0        0        0 2023-11-23 08:09:33.423138 rknntools-0.0.2/rknntools.egg-info/
--rw-rw-rw-   0        0        0     2442 2023-11-23 08:09:33.000000 rknntools-0.0.2/rknntools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-11-23 08:09:33.000000 rknntools-0.0.2/rknntools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-23 08:09:33.000000 rknntools-0.0.2/rknntools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-11-23 08:09:33.000000 rknntools-0.0.2/rknntools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-11-23 08:09:33.000000 rknntools-0.0.2/rknntools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-23 08:09:33.425133 rknntools-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 07:40:37.631399 rknntools-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-11-23 07:22:32.000000 rknntools-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2442 2024-05-09 07:40:37.629404 rknntools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-11-22 10:30:59.000000 rknntools-0.0.3/README.md
+-rw-rw-rw-   0        0        0      581 2024-05-09 07:39:24.000000 rknntools-0.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-09 07:40:37.620794 rknntools-0.0.3/rknntools/
+-rw-rw-rw-   0        0        0       36 2023-12-04 06:10:34.000000 rknntools-0.0.3/rknntools/__init__.py
+-rw-rw-rw-   0        0        0     3539 2024-05-09 07:38:44.000000 rknntools-0.0.3/rknntools/op_limit.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:40:37.628407 rknntools-0.0.3/rknntools.egg-info/
+-rw-rw-rw-   0        0        0     2442 2024-05-09 07:40:37.000000 rknntools-0.0.3/rknntools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-09 07:40:37.000000 rknntools-0.0.3/rknntools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 07:40:37.000000 rknntools-0.0.3/rknntools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-09 07:40:37.000000 rknntools-0.0.3/rknntools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-09 07:40:37.000000 rknntools-0.0.3/rknntools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 07:40:37.631399 rknntools-0.0.3/setup.cfg
```

### Comparing `rknntools-0.0.2/LICENSE` & `rknntools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rknntools-0.0.2/PKG-INFO` & `rknntools-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rknntools
-Version: 0.0.2
+Version: 0.0.3
 Summary: A utility toolkit for converting RKNN2 models, potentially used during the model transformation process.
 Author-email: yuyun <15515722313@163.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rknntools-0.0.2/README.md` & `rknntools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rknntools-0.0.2/pyproject.toml` & `rknntools-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2272 6b6e 6e74 6f6f 6c73 220d 0a76  = "rknntools"..v
-00000020: 6572 7369 6f6e 203d 2022 302e 302e 3222  ersion = "0.0.2"
+00000020: 6572 7369 6f6e 203d 2022 302e 302e 3322  ersion = "0.0.3"
 00000030: 0d0a 6175 7468 6f72 7320 3d20 5b0d 0a20  ..authors = [.. 
 00000040: 207b 206e 616d 653d 2279 7579 756e 222c   { name="yuyun",
 00000050: 2065 6d61 696c 3d22 3135 3531 3537 3232   email="15515722
 00000060: 3331 3340 3136 332e 636f 6d22 7d2c 0d0a  313@163.com"},..
 00000070: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
 00000080: 2022 4120 7574 696c 6974 7920 746f 6f6c   "A utility tool
 00000090: 6b69 7420 666f 7220 636f 6e76 6572 7469  kit for converti
```

### Comparing `rknntools-0.0.2/rknntools/op_limit.py` & `rknntools-0.0.3/rknntools/op_limit.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,20 +45,23 @@
                           'InstanceNormalization', 'Less', 'LessOrEqual', 'LogSoftmax', 'LpNormalization', 'LRN',
                           'MaxRoiPool', 'MaxUnpool', 'Mish', 'Min',
                           'Pad', 'Pow', 'Proposal', 'ReduceMax', 'ReduceMin', 'Reorg', 'Reshape', 'Resize', 'RoiAlign',
                           'RMSNorm', 'ScatterND', 'Sin', 'Slice',
                           'SpaceToDetph', 'Split', 'Sqrt', 'Squeeze', 'Tile', 'Upsample', 'Not']  # 文档中的CPU算子
     RKNN_152_CPUOPLIST = [item.upper() for item in RKNN_152_CPUOPLIST]
 
+    RKNN_2_NEW_OP_LIST = ['And','GatherElements','Log']
+    RKNN_2_NEW_OP_LIST = [item.upper() for item in RKNN_2_NEW_OP_LIST] #RKNN 2.0.0版本号后支持的新的算子
+
     ONNX_OP = ['Constant', 'Unsqueeze', 'Conv', 'Identity', 'ConstantOfShape', 'Shape','Erf']  # 文档中没有或者名称不匹配，但实际支持的算子
     ONNX_OP = [item.upper() for item in ONNX_OP]
 
     NO_SUPPORT_LIST = []
     for item in operations:
-        if (item.upper() not in RK3566_152_NPUOPLIST) and (item.upper() not in RKNN_152_CPUOPLIST) and (
+        if (item.upper() not in RK3566_152_NPUOPLIST) and (item.upper() not in RKNN_152_CPUOPLIST) and (item.upper() not in RKNN_2_NEW_OP_LIST) and (
                 item.upper() not in ONNX_OP):
             NO_SUPPORT_LIST.append(item)
 
     if len(NO_SUPPORT_LIST) == 0:
         print("初步匹配该模型算子全部支持")
     else:
         print("不支持的操作列表：\n")
```

### Comparing `rknntools-0.0.2/rknntools.egg-info/PKG-INFO` & `rknntools-0.0.3/rknntools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rknntools
-Version: 0.0.2
+Version: 0.0.3
 Summary: A utility toolkit for converting RKNN2 models, potentially used during the model transformation process.
 Author-email: yuyun <15515722313@163.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

