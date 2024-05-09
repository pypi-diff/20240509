# Comparing `tmp/viewai-0.1.1.tar.gz` & `tmp/viewai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viewai-0.1.1.tar", last modified: Thu May  9 03:52:08 2024, max compression
+gzip compressed data, was "viewai-0.1.2.tar", last modified: Thu May  9 04:02:39 2024, max compression
```

## Comparing `viewai-0.1.1.tar` & `viewai-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 shivamarora   (501) staff       (20)        0 2024-05-09 03:52:08.261739 viewai-0.1.1/
--rw-r--r--   0 shivamarora   (501) staff       (20)     1080 2024-05-08 22:00:52.000000 viewai-0.1.1/LICENCE.md
--rw-r--r--   0 shivamarora   (501) staff       (20)     9439 2024-05-09 03:52:08.261633 viewai-0.1.1/PKG-INFO
--rw-r--r--   0 shivamarora   (501) staff       (20)     8165 2024-05-09 02:39:04.000000 viewai-0.1.1/README.md
--rw-r--r--   0 shivamarora   (501) staff       (20)       38 2024-05-09 03:52:08.262031 viewai-0.1.1/setup.cfg
--rw-r--r--   0 shivamarora   (501) staff       (20)      989 2024-05-09 03:50:41.000000 viewai-0.1.1/setup.py
-drwxr-xr-x   0 shivamarora   (501) staff       (20)        0 2024-05-09 03:52:08.252175 viewai-0.1.1/tests/
--rw-r--r--   0 shivamarora   (501) staff       (20)        0 2024-05-09 01:37:17.000000 viewai-0.1.1/tests/__init__.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     2047 2024-05-09 01:55:46.000000 viewai-0.1.1/tests/test.py
-drwxr-xr-x   0 shivamarora   (501) staff       (20)        0 2024-05-09 03:52:08.254487 viewai-0.1.1/viewai/
--rw-r--r--   0 shivamarora   (501) staff       (20)       20 2024-05-09 01:38:09.000000 viewai-0.1.1/viewai/__init__.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     4312 2024-05-09 01:17:40.000000 viewai-0.1.1/viewai/config.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     5618 2024-05-08 22:01:23.000000 viewai-0.1.1/viewai/explanations.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     1368 2024-05-09 01:18:10.000000 viewai-0.1.1/viewai/imports.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     4798 2024-05-09 01:18:21.000000 viewai-0.1.1/viewai/inputs.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     2016 2024-05-08 22:27:48.000000 viewai-0.1.1/viewai/logger.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     7736 2024-05-09 01:18:27.000000 viewai-0.1.1/viewai/modules.py
--rw-r--r--   0 shivamarora   (501) staff       (20)    15240 2024-05-08 22:01:38.000000 viewai-0.1.1/viewai/plots.py
-drwxr-xr-x   0 shivamarora   (501) staff       (20)        0 2024-05-09 03:52:08.261256 viewai-0.1.1/viewai/utils/
--rw-r--r--   0 shivamarora   (501) staff       (20)     2900 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_SPOTgreedy.py
--rw-r--r--   0 shivamarora   (501) staff       (20)      358 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/__init__.py
--rw-r--r--   0 shivamarora   (501) staff       (20)    13459 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_clean_simple.py
--rw-r--r--   0 shivamarora   (501) staff       (20)    82780 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_clean_x.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     5212 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_compressed_dataset.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     6217 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_explanation.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     2369 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_histogram.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     7675 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_link.py
--rw-r--r--   0 shivamarora   (501) staff       (20)    11074 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_measure_interactions.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     3318 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_misc.py
--rw-r--r--   0 shivamarora   (501) staff       (20)    67125 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_native.py
--rw-r--r--   0 shivamarora   (501) staff       (20)    24834 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_preprocessor.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     6145 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_privacy.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     2038 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_rank_interactions.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     2603 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_seed.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     3962 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_shap_common.py
--rw-r--r--   0 shivamarora   (501) staff       (20)    16230 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_synthetic.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     3274 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_unify_data.py
--rw-r--r--   0 shivamarora   (501) staff       (20)     5091 2024-05-06 18:43:36.000000 viewai-0.1.1/viewai/utils/_unify_predict.py
--rw-r--r--   0 shivamarora   (501) staff       (20)    11396 2024-05-09 01:21:40.000000 viewai-0.1.1/viewai/xai.py
-drwxr-xr-x   0 shivamarora   (501) staff       (20)        0 2024-05-09 03:52:08.255254 viewai-0.1.1/viewai.egg-info/
--rw-r--r--   0 shivamarora   (501) staff       (20)     9439 2024-05-09 03:52:08.000000 viewai-0.1.1/viewai.egg-info/PKG-INFO
--rw-r--r--   0 shivamarora   (501) staff       (20)      912 2024-05-09 03:52:08.000000 viewai-0.1.1/viewai.egg-info/SOURCES.txt
--rw-r--r--   0 shivamarora   (501) staff       (20)        1 2024-05-09 03:52:08.000000 viewai-0.1.1/viewai.egg-info/dependency_links.txt
--rw-r--r--   0 shivamarora   (501) staff       (20)      309 2024-05-09 03:52:08.000000 viewai-0.1.1/viewai.egg-info/requires.txt
--rw-r--r--   0 shivamarora   (501) staff       (20)       13 2024-05-09 03:52:08.000000 viewai-0.1.1/viewai.egg-info/top_level.txt
+drwxr-xr-x   0 shivamarora   (501) staff       (20)        0 2024-05-09 04:02:39.294807 viewai-0.1.2/
+-rw-r--r--   0 shivamarora   (501) staff       (20)     1080 2024-05-08 22:00:52.000000 viewai-0.1.2/LICENCE.md
+-rw-r--r--   0 shivamarora   (501) staff       (20)     9272 2024-05-09 04:02:39.294721 viewai-0.1.2/PKG-INFO
+-rw-r--r--   0 shivamarora   (501) staff       (20)     8165 2024-05-09 02:39:04.000000 viewai-0.1.2/README.md
+-rw-r--r--   0 shivamarora   (501) staff       (20)       38 2024-05-09 04:02:39.295022 viewai-0.1.2/setup.cfg
+-rw-r--r--   0 shivamarora   (501) staff       (20)      989 2024-05-09 04:02:35.000000 viewai-0.1.2/setup.py
+drwxr-xr-x   0 shivamarora   (501) staff       (20)        0 2024-05-09 04:02:39.285475 viewai-0.1.2/tests/
+-rw-r--r--   0 shivamarora   (501) staff       (20)        0 2024-05-09 01:37:17.000000 viewai-0.1.2/tests/__init__.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     2047 2024-05-09 01:55:46.000000 viewai-0.1.2/tests/test.py
+drwxr-xr-x   0 shivamarora   (501) staff       (20)        0 2024-05-09 04:02:39.287966 viewai-0.1.2/viewai/
+-rw-r--r--   0 shivamarora   (501) staff       (20)       20 2024-05-09 01:38:09.000000 viewai-0.1.2/viewai/__init__.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     4312 2024-05-09 01:17:40.000000 viewai-0.1.2/viewai/config.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     5618 2024-05-08 22:01:23.000000 viewai-0.1.2/viewai/explanations.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     1310 2024-05-09 04:02:22.000000 viewai-0.1.2/viewai/imports.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     4798 2024-05-09 01:18:21.000000 viewai-0.1.2/viewai/inputs.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     2016 2024-05-08 22:27:48.000000 viewai-0.1.2/viewai/logger.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     7736 2024-05-09 01:18:27.000000 viewai-0.1.2/viewai/modules.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)    15240 2024-05-08 22:01:38.000000 viewai-0.1.2/viewai/plots.py
+drwxr-xr-x   0 shivamarora   (501) staff       (20)        0 2024-05-09 04:02:39.294299 viewai-0.1.2/viewai/utils/
+-rw-r--r--   0 shivamarora   (501) staff       (20)     2900 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_SPOTgreedy.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)      358 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/__init__.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)    13459 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_clean_simple.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)    82780 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_clean_x.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     5212 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_compressed_dataset.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     6217 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_explanation.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     2369 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_histogram.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     7675 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_link.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)    11074 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_measure_interactions.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     3318 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_misc.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)    67125 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_native.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)    24834 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_preprocessor.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     6145 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_privacy.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     2038 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_rank_interactions.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     2603 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_seed.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     3962 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_shap_common.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)    16230 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_synthetic.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     3274 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_unify_data.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)     5091 2024-05-06 18:43:36.000000 viewai-0.1.2/viewai/utils/_unify_predict.py
+-rw-r--r--   0 shivamarora   (501) staff       (20)    11396 2024-05-09 01:21:40.000000 viewai-0.1.2/viewai/xai.py
+drwxr-xr-x   0 shivamarora   (501) staff       (20)        0 2024-05-09 04:02:39.294478 viewai-0.1.2/viewai.egg-info/
+-rw-r--r--   0 shivamarora   (501) staff       (20)     9272 2024-05-09 04:02:39.000000 viewai-0.1.2/viewai.egg-info/PKG-INFO
+-rw-r--r--   0 shivamarora   (501) staff       (20)      912 2024-05-09 04:02:39.000000 viewai-0.1.2/viewai.egg-info/SOURCES.txt
+-rw-r--r--   0 shivamarora   (501) staff       (20)        1 2024-05-09 04:02:39.000000 viewai-0.1.2/viewai.egg-info/dependency_links.txt
+-rw-r--r--   0 shivamarora   (501) staff       (20)      172 2024-05-09 04:02:39.000000 viewai-0.1.2/viewai.egg-info/requires.txt
+-rw-r--r--   0 shivamarora   (501) staff       (20)       13 2024-05-09 04:02:39.000000 viewai-0.1.2/viewai.egg-info/top_level.txt
```

### Comparing `viewai-0.1.1/LICENCE.md` & `viewai-0.1.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/PKG-INFO` & `viewai-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viewai
-Version: 0.1.1
+Version: 0.1.2
 Summary: xAI is an open-source package to explain blackbox systems.
 Home-page: https://github.com/View-AI/xAI
 Author: View AI Team
 Author-email: arorashivam@viewai.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -15,30 +15,28 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: plotly
+Requires-Dist: numpy
 Requires-Dist: matplotlib
-Requires-Dist: fuzzywuzzy==0.18.0
-Requires-Dist: textblob==0.15.3
-Requires-Dist: missingpy==0.2.0
-Requires-Dist: interpret==0.2.4
-Requires-Dist: interpret-core==0.3.2
-Requires-Dist: tabulate==0.8.9
-Requires-Dist: MarkupSafe==2.0.1
-Requires-Dist: Jinja2==2.11.3
-Requires-Dist: itsdangerous==2.0.1
-Requires-Dist: orjson==3.6.4
-Requires-Dist: cchardet==2.1.7
-Requires-Dist: category-encoders==2.2.2
-Requires-Dist: numpy==1.20.3
-Requires-Dist: requests==2.31.0
-Requires-Dist: imbalanced-learn==0.7.0
+Requires-Dist: fuzzywuzzy
+Requires-Dist: textblob
+Requires-Dist: missingpy
+Requires-Dist: interpret
+Requires-Dist: interpret-core
+Requires-Dist: tabulate
+Requires-Dist: MarkupSafe
+Requires-Dist: Jinja2
+Requires-Dist: itsdangerous
+Requires-Dist: orjson
+Requires-Dist: requests
+Requires-Dist: imbalanced-learn
 
 <div align="center">
     <img src="https://www.viewai.ca/_next/image?url=%2Fcompany-images%2Flogo-no-background.png&w=128&q=75" alt="Lenster Logo" height="100" width="100">
     <h1>xAI</h1>
     <strong>Understand Models. Build Responsibly.</strong>
 </div>
 <br>
```

### Comparing `viewai-0.1.1/README.md` & `viewai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/setup.py` & `viewai-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='viewai',
-    version='0.1.1',
+    version='0.1.2',
     description='xAI is an open-source package to explain blackbox systems.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='View AI Team',
     author_email='arorashivam@viewai.ca',
     url='https://github.com/View-AI/xAI',
     packages=find_packages(),
```

### Comparing `viewai-0.1.1/tests/test.py` & `viewai-0.1.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/config.py` & `viewai-0.1.2/viewai/config.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/explanations.py` & `viewai-0.1.2/viewai/explanations.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/imports.py` & `viewai-0.1.2/viewai/imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # Copyright (c) 2024 The View AI Contributors
 # Distributed under the MIT software license
 
 import warnings
 warnings.filterwarnings("ignore")
 
 import sys
-import sklearn.neighbors._base
 import requests
 from enum import Enum
 
 # BASE
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import random
 from time import time
 
 import os
 import orjson
 import argparse
 import logging
-import cchardet as chardet
 
 # PREPROCESSING
 from sklearn.model_selection import (
     train_test_split,
     cross_val_score,
     StratifiedKFold,
     KFold,
```

### Comparing `viewai-0.1.1/viewai/inputs.py` & `viewai-0.1.2/viewai/inputs.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/logger.py` & `viewai-0.1.2/viewai/logger.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/modules.py` & `viewai-0.1.2/viewai/modules.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/plots.py` & `viewai-0.1.2/viewai/plots.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_SPOTgreedy.py` & `viewai-0.1.2/viewai/utils/_SPOTgreedy.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_clean_simple.py` & `viewai-0.1.2/viewai/utils/_clean_simple.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_clean_x.py` & `viewai-0.1.2/viewai/utils/_clean_x.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_compressed_dataset.py` & `viewai-0.1.2/viewai/utils/_compressed_dataset.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_explanation.py` & `viewai-0.1.2/viewai/utils/_explanation.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_histogram.py` & `viewai-0.1.2/viewai/utils/_histogram.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_link.py` & `viewai-0.1.2/viewai/utils/_link.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_measure_interactions.py` & `viewai-0.1.2/viewai/utils/_measure_interactions.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_misc.py` & `viewai-0.1.2/viewai/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_native.py` & `viewai-0.1.2/viewai/utils/_native.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_preprocessor.py` & `viewai-0.1.2/viewai/utils/_preprocessor.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_privacy.py` & `viewai-0.1.2/viewai/utils/_privacy.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_rank_interactions.py` & `viewai-0.1.2/viewai/utils/_rank_interactions.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_seed.py` & `viewai-0.1.2/viewai/utils/_seed.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_shap_common.py` & `viewai-0.1.2/viewai/utils/_shap_common.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_synthetic.py` & `viewai-0.1.2/viewai/utils/_synthetic.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_unify_data.py` & `viewai-0.1.2/viewai/utils/_unify_data.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/utils/_unify_predict.py` & `viewai-0.1.2/viewai/utils/_unify_predict.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai/xai.py` & `viewai-0.1.2/viewai/xai.py`

 * *Files identical despite different names*

### Comparing `viewai-0.1.1/viewai.egg-info/PKG-INFO` & `viewai-0.1.2/viewai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viewai
-Version: 0.1.1
+Version: 0.1.2
 Summary: xAI is an open-source package to explain blackbox systems.
 Home-page: https://github.com/View-AI/xAI
 Author: View AI Team
 Author-email: arorashivam@viewai.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -15,30 +15,28 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: plotly
+Requires-Dist: numpy
 Requires-Dist: matplotlib
-Requires-Dist: fuzzywuzzy==0.18.0
-Requires-Dist: textblob==0.15.3
-Requires-Dist: missingpy==0.2.0
-Requires-Dist: interpret==0.2.4
-Requires-Dist: interpret-core==0.3.2
-Requires-Dist: tabulate==0.8.9
-Requires-Dist: MarkupSafe==2.0.1
-Requires-Dist: Jinja2==2.11.3
-Requires-Dist: itsdangerous==2.0.1
-Requires-Dist: orjson==3.6.4
-Requires-Dist: cchardet==2.1.7
-Requires-Dist: category-encoders==2.2.2
-Requires-Dist: numpy==1.20.3
-Requires-Dist: requests==2.31.0
-Requires-Dist: imbalanced-learn==0.7.0
+Requires-Dist: fuzzywuzzy
+Requires-Dist: textblob
+Requires-Dist: missingpy
+Requires-Dist: interpret
+Requires-Dist: interpret-core
+Requires-Dist: tabulate
+Requires-Dist: MarkupSafe
+Requires-Dist: Jinja2
+Requires-Dist: itsdangerous
+Requires-Dist: orjson
+Requires-Dist: requests
+Requires-Dist: imbalanced-learn
 
 <div align="center">
     <img src="https://www.viewai.ca/_next/image?url=%2Fcompany-images%2Flogo-no-background.png&w=128&q=75" alt="Lenster Logo" height="100" width="100">
     <h1>xAI</h1>
     <strong>Understand Models. Build Responsibly.</strong>
 </div>
 <br>
```

### Comparing `viewai-0.1.1/viewai.egg-info/SOURCES.txt` & `viewai-0.1.2/viewai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

