# Comparing `tmp/kfsmath-1.0.1.tar.gz` & `tmp/kfsmath-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsmath-1.0.1.tar", max compression
+gzip compressed data, was "kfsmath-1.0.2.tar", max compression
```

## Comparing `kfsmath-1.0.1.tar` & `kfsmath-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      690 2023-09-22 23:20:50.987294 kfsmath-1.0.1/KFSmath/KFSmath.py
--rw-r--r--   0        0        0        0 2023-09-22 23:20:50.987294 kfsmath-1.0.1/KFSmath/__init__.py
--rw-r--r--   0        0        0      416 2023-09-22 23:20:50.987294 kfsmath-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      647 2023-09-22 23:20:50.987294 kfsmath-1.0.1/readme.md
--rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 kfsmath-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      690 2024-05-09 21:53:43.013309 kfsmath-1.0.2/KFSmath/KFSmath.py
+-rw-r--r--   0        0        0      490 2024-05-09 21:53:43.013309 kfsmath-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      631 2024-05-09 21:53:43.013309 kfsmath-1.0.2/readme.md
+-rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 kfsmath-1.0.2/PKG-INFO
```

### Comparing `kfsmath-1.0.1/KFSmath/KFSmath.py` & `kfsmath-1.0.2/KFSmath/KFSmath.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023 구FS, all rights reserved. Subject to the MIT licence in `licence.md`.
+# Copyright (c) 2024 구FS, all rights reserved. Subject to the MIT licence in `licence.md`.
 import math
 
 
 def round_sig(x: float, significants: int) -> float:    
     """
     Round x to significant number. If significants is smaller 1, always returns 0.
```

### Comparing `kfsmath-1.0.1/readme.md` & `kfsmath-1.0.2/readme.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
-Topic: "KFSmath Library"
+Topic: "KFSmath"
 Author: "구FS"
 ---
 <link href="./doc_templates/md_style.css" rel="stylesheet"></link>
 <body>
 
-# <p style="text-align: center;">KFSmath Library</p>
+# <p style="text-align: center;">KFSmath</p>
 <br>
 <br>
 
 - [1. General](#1-general)
 - [2. Installation](#2-installation)
 
 ## 1. General
```

### Comparing `kfsmath-1.0.1/PKG-INFO` & `kfsmath-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: KFSmath
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
-Home-page: https://github.com/9-FS/2023-09-20-KFSmath-Library
+Home-page: https://github.com/9-FS/2023-09-20-KFSmath
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
-Requires-Python: >=3.11.0,<4.0.0
+Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSmath-Library
+Classifier: Programming Language :: Python :: 3.12
+Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSmath
 Description-Content-Type: text/markdown
 
 ---
-Topic: "KFSmath Library"
+Topic: "KFSmath"
 Author: "구FS"
 ---
 <link href="./doc_templates/md_style.css" rel="stylesheet"></link>
 <body>
 
-# <p style="text-align: center;">KFSmath Library</p>
+# <p style="text-align: center;">KFSmath</p>
 <br>
 <br>
 
 - [1. General](#1-general)
 - [2. Installation](#2-installation)
 
 ## 1. General
```

