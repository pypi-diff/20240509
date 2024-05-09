# Comparing `tmp/pathologyfoundation-0.2.3.tar.gz` & `tmp/pathologyfoundation-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathologyfoundation-0.2.3.tar", last modified: Fri May  3 00:08:28 2024, max compression
+gzip compressed data, was "pathologyfoundation-0.2.4.tar", last modified: Thu May  9 01:26:13 2024, max compression
```

## Comparing `pathologyfoundation-0.2.3.tar` & `pathologyfoundation-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-03 00:08:28.520907 pathologyfoundation-0.2.3/
--rw-r--r--   0 zhihuang   (501) staff       (20)     1048 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.3/LICENSE
--rw-r--r--   0 zhihuang   (501) staff       (20)      542 2024-05-03 00:08:28.519816 pathologyfoundation-0.2.3/PKG-INFO
--rw-r--r--   0 zhihuang   (501) staff       (20)     2730 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.3/README.md
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-03 00:08:28.514752 pathologyfoundation-0.2.3/pathologyfoundation/
--rw-r--r--   0 zhihuang   (501) staff       (20)      112 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.3/pathologyfoundation/__init__.py
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-03 00:08:28.517813 pathologyfoundation-0.2.3/pathologyfoundation/dataset/
--rw-r--r--   0 zhihuang   (501) staff       (20)       25 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.3/pathologyfoundation/dataset/__init__.py
--rw-r--r--   0 zhihuang   (501) staff       (20)     2813 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.3/pathologyfoundation/dataset/load_data.py
--rw-r--r--   0 zhihuang   (501) staff       (20)      461 2024-04-26 22:13:48.000000 pathologyfoundation-0.2.3/pathologyfoundation/model_zoo.py
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-03 00:08:28.519274 pathologyfoundation-0.2.3/pathologyfoundation/models/
--rw-r--r--   0 zhihuang   (501) staff       (20)       64 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.3/pathologyfoundation/models/__init__.py
--rw-r--r--   0 zhihuang   (501) staff       (20)    11127 2024-05-03 00:07:31.000000 pathologyfoundation-0.2.3/pathologyfoundation/models/finetuner.py
--rw-r--r--   0 zhihuang   (501) staff       (20)     6619 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.3/pathologyfoundation/models/plip_vit.py
--rw-r--r--   0 zhihuang   (501) staff       (20)      700 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.3/pathologyfoundation/utils.py
-drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-03 00:08:28.516850 pathologyfoundation-0.2.3/pathologyfoundation.egg-info/
--rw-r--r--   0 zhihuang   (501) staff       (20)      542 2024-05-03 00:08:28.000000 pathologyfoundation-0.2.3/pathologyfoundation.egg-info/PKG-INFO
--rw-r--r--   0 zhihuang   (501) staff       (20)      533 2024-05-03 00:08:28.000000 pathologyfoundation-0.2.3/pathologyfoundation.egg-info/SOURCES.txt
--rw-r--r--   0 zhihuang   (501) staff       (20)        1 2024-05-03 00:08:28.000000 pathologyfoundation-0.2.3/pathologyfoundation.egg-info/dependency_links.txt
--rw-r--r--   0 zhihuang   (501) staff       (20)       92 2024-05-03 00:08:28.000000 pathologyfoundation-0.2.3/pathologyfoundation.egg-info/requires.txt
--rw-r--r--   0 zhihuang   (501) staff       (20)       20 2024-05-03 00:08:28.000000 pathologyfoundation-0.2.3/pathologyfoundation.egg-info/top_level.txt
--rw-r--r--   0 zhihuang   (501) staff       (20)       38 2024-05-03 00:08:28.521088 pathologyfoundation-0.2.3/setup.cfg
--rw-r--r--   0 zhihuang   (501) staff       (20)      981 2024-05-03 00:07:49.000000 pathologyfoundation-0.2.3/setup.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-09 01:26:13.465820 pathologyfoundation-0.2.4/
+-rw-r--r--   0 zhihuang   (501) staff       (20)     1048 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.4/LICENSE
+-rw-r--r--   0 zhihuang   (501) staff       (20)      542 2024-05-09 01:26:13.464808 pathologyfoundation-0.2.4/PKG-INFO
+-rw-r--r--   0 zhihuang   (501) staff       (20)     2730 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.4/README.md
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-09 01:26:13.450374 pathologyfoundation-0.2.4/pathologyfoundation/
+-rw-r--r--   0 zhihuang   (501) staff       (20)      112 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.4/pathologyfoundation/__init__.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-09 01:26:13.462340 pathologyfoundation-0.2.4/pathologyfoundation/dataset/
+-rw-r--r--   0 zhihuang   (501) staff       (20)       25 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.4/pathologyfoundation/dataset/__init__.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)     2813 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.4/pathologyfoundation/dataset/load_data.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)      461 2024-04-26 22:13:48.000000 pathologyfoundation-0.2.4/pathologyfoundation/model_zoo.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-09 01:26:13.463989 pathologyfoundation-0.2.4/pathologyfoundation/models/
+-rw-r--r--   0 zhihuang   (501) staff       (20)       64 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.4/pathologyfoundation/models/__init__.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)    11163 2024-05-09 01:25:24.000000 pathologyfoundation-0.2.4/pathologyfoundation/models/finetuner.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)     6619 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.4/pathologyfoundation/models/plip_vit.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)      700 2024-04-26 21:38:18.000000 pathologyfoundation-0.2.4/pathologyfoundation/utils.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-05-09 01:26:13.457533 pathologyfoundation-0.2.4/pathologyfoundation.egg-info/
+-rw-r--r--   0 zhihuang   (501) staff       (20)      542 2024-05-09 01:26:13.000000 pathologyfoundation-0.2.4/pathologyfoundation.egg-info/PKG-INFO
+-rw-r--r--   0 zhihuang   (501) staff       (20)      533 2024-05-09 01:26:13.000000 pathologyfoundation-0.2.4/pathologyfoundation.egg-info/SOURCES.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)        1 2024-05-09 01:26:13.000000 pathologyfoundation-0.2.4/pathologyfoundation.egg-info/dependency_links.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)       92 2024-05-09 01:26:13.000000 pathologyfoundation-0.2.4/pathologyfoundation.egg-info/requires.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)       20 2024-05-09 01:26:13.000000 pathologyfoundation-0.2.4/pathologyfoundation.egg-info/top_level.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)       38 2024-05-09 01:26:13.465965 pathologyfoundation-0.2.4/setup.cfg
+-rw-r--r--   0 zhihuang   (501) staff       (20)      981 2024-05-09 01:26:06.000000 pathologyfoundation-0.2.4/setup.py
```

### Comparing `pathologyfoundation-0.2.3/LICENSE` & `pathologyfoundation-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2.3/PKG-INFO` & `pathologyfoundation-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathologyfoundation
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package of pathology foundation models.
 Home-page: https://github.com/PathologyFoundation/pathologyfoundation
 Author: Zhi Huang
 Author-email: hz9423@gmail.com
 Keywords: Pathology,Foundation model,PLIP,OpenPath
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pathologyfoundation-0.2.3/README.md` & `pathologyfoundation-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2.3/pathologyfoundation/dataset/load_data.py` & `pathologyfoundation-0.2.4/pathologyfoundation/dataset/load_data.py`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2.3/pathologyfoundation/models/finetuner.py` & `pathologyfoundation-0.2.4/pathologyfoundation/models/finetuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from PIL import Image
 from tqdm import tqdm
 import pandas as pd
 from sklearn.metrics import *
 from PIL import Image
 import random
+from collections import OrderedDict
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils.data import DataLoader
 import os
 opj = os.path.join
```

### Comparing `pathologyfoundation-0.2.3/pathologyfoundation/models/plip_vit.py` & `pathologyfoundation-0.2.4/pathologyfoundation/models/plip_vit.py`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2.3/pathologyfoundation/utils.py` & `pathologyfoundation-0.2.4/pathologyfoundation/utils.py`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2.3/pathologyfoundation.egg-info/PKG-INFO` & `pathologyfoundation-0.2.4/pathologyfoundation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathologyfoundation
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package of pathology foundation models.
 Home-page: https://github.com/PathologyFoundation/pathologyfoundation
 Author: Zhi Huang
 Author-email: hz9423@gmail.com
 Keywords: Pathology,Foundation model,PLIP,OpenPath
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pathologyfoundation-0.2.3/pathologyfoundation.egg-info/SOURCES.txt` & `pathologyfoundation-0.2.4/pathologyfoundation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.2.3/setup.py` & `pathologyfoundation-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         "appdirs",
         "pandas",
         "numpy",
         "tqdm",
         "gdown",
         "scikit-learn",
     ],
-    version = '0.2.3',  # Ideally should be same as the GitHub release tag varsion
+    version = '0.2.4',  # Ideally should be same as the GitHub release tag varsion
     description="A package of pathology foundation models.",
     long_description="Please check our github page: https://github.com/PathologyFoundation/pathologyfoundation",
     author = 'Zhi Huang',
     author_email = 'hz9423@gmail.com',
     url = 'https://github.com/PathologyFoundation/pathologyfoundation',
     keywords = ['Pathology', 'Foundation model', "PLIP", "OpenPath"],
     classifiers=[
```

