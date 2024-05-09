# Comparing `tmp/tools-jsyoo61-2024.5.9.0.tar.gz` & `tmp/tools-jsyoo61-2024.5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tools-jsyoo61-2024.5.9.0.tar", last modified: Thu May  9 20:56:59 2024, max compression
+gzip compressed data, was "tools-jsyoo61-2024.5.9.1.tar", last modified: Thu May  9 21:11:53 2024, max compression
```

## Comparing `tools-jsyoo61-2024.5.9.0.tar` & `tools-jsyoo61-2024.5.9.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.783680 tools-jsyoo61-2024.5.9.0/
--rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1338 2024-05-09 20:56:59.781680 tools-jsyoo61-2024.5.9.0/PKG-INFO
--rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-09 20:56:59.784679 tools-jsyoo61-2024.5.9.0/setup.cfg
--rw-rw-rw-   0        0        0      819 2024-05-09 20:56:32.000000 tools-jsyoo61-2024.5.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.658129 tools-jsyoo61-2024.5.9.0/tools/
--rw-rw-rw-   0        0        0      292 2024-05-09 20:56:46.000000 tools-jsyoo61-2024.5.9.0/tools/__init__.py
--rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/array.py
--rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/data.py
--rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/exp.py
-drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.661130 tools-jsyoo61-2024.5.9.0/tools/hydra/
--rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/hydra/__init__.py
--rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2024.5.9.0/tools/modules.py
-drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.670915 tools-jsyoo61-2024.5.9.0/tools/numpy/
--rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/numpy/__init__.py
--rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/numpy/_f.py
--rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/numpy/_utils.py
--rw-rw-rw-   0        0        0     2279 2024-05-03 02:04:50.000000 tools-jsyoo61-2024.5.9.0/tools/os.py
-drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.673923 tools-jsyoo61-2024.5.9.0/tools/pandas/
--rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.686451 tools-jsyoo61-2024.5.9.0/tools/plot/
--rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/plot/__init__.py
--rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/plot/sklearn.py
--rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/plot/utils.py
--rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/random.py
-drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.692450 tools-jsyoo61-2024.5.9.0/tools/sklearn/
--rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/sklearn/__init__.py
--rw-rw-rw-   0        0        0     6721 2024-01-22 14:45:14.000000 tools-jsyoo61-2024.5.9.0/tools/sklearn/model_selection.py
-drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.696994 tools-jsyoo61-2024.5.9.0/tools/stats/
--rw-rw-rw-   0        0        0     1241 2024-03-19 18:49:39.000000 tools-jsyoo61-2024.5.9.0/tools/stats/__init__.py
--rw-rw-rw-   0        0        0    15603 2024-05-03 18:32:59.000000 tools-jsyoo61-2024.5.9.0/tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.725321 tools-jsyoo61-2024.5.9.0/tools/torch/
--rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/__init__.py
--rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/_pandas.py
--rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/estimator.py
--rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/federated_learning.py
--rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/layers.py
--rw-rw-rw-   0        0        0    18008 2024-03-14 20:51:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/model.py
-drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.734099 tools-jsyoo61-2024.5.9.0/tools/torch/optim/
--rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/optim/__init__.py
--rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/optim/lr_scheduler.py
--rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/plot.py
--rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2024.5.9.0/tools/torch/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.778682 tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/
--rw-rw-rw-   0        0        0     1338 2024-05-09 20:56:58.000000 tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2024-05-09 20:56:59.000000 tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 20:56:58.000000 tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-09 20:56:58.000000 tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 21:11:53.099187 tools-jsyoo61-2024.5.9.1/
+-rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1338 2024-05-09 21:11:53.097147 tools-jsyoo61-2024.5.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-09 21:11:53.099187 tools-jsyoo61-2024.5.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      819 2024-05-09 20:56:32.000000 tools-jsyoo61-2024.5.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:11:53.009612 tools-jsyoo61-2024.5.9.1/tools/
+-rw-rw-rw-   0        0        0      292 2024-05-09 21:11:42.000000 tools-jsyoo61-2024.5.9.1/tools/__init__.py
+-rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/array.py
+-rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/data.py
+-rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/exp.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:11:53.012609 tools-jsyoo61-2024.5.9.1/tools/hydra/
+-rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/hydra/__init__.py
+-rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2024.5.9.1/tools/modules.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:11:53.018610 tools-jsyoo61-2024.5.9.1/tools/numpy/
+-rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/numpy/_f.py
+-rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/numpy/_utils.py
+-rw-rw-rw-   0        0        0     2279 2024-05-03 02:04:50.000000 tools-jsyoo61-2024.5.9.1/tools/os.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:11:53.020609 tools-jsyoo61-2024.5.9.1/tools/pandas/
+-rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:11:53.027609 tools-jsyoo61-2024.5.9.1/tools/plot/
+-rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/plot/__init__.py
+-rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/plot/sklearn.py
+-rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/plot/utils.py
+-rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/random.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:11:53.031608 tools-jsyoo61-2024.5.9.1/tools/sklearn/
+-rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/sklearn/__init__.py
+-rw-rw-rw-   0        0        0     6721 2024-01-22 14:45:14.000000 tools-jsyoo61-2024.5.9.1/tools/sklearn/model_selection.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:11:53.033609 tools-jsyoo61-2024.5.9.1/tools/stats/
+-rw-rw-rw-   0        0        0     1241 2024-03-19 18:49:39.000000 tools-jsyoo61-2024.5.9.1/tools/stats/__init__.py
+-rw-rw-rw-   0        0        0    15559 2024-05-09 21:11:38.000000 tools-jsyoo61-2024.5.9.1/tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:11:53.052609 tools-jsyoo61-2024.5.9.1/tools/torch/
+-rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/torch/__init__.py
+-rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/torch/_pandas.py
+-rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/torch/estimator.py
+-rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/torch/federated_learning.py
+-rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/torch/layers.py
+-rw-rw-rw-   0        0        0    18008 2024-03-14 20:51:33.000000 tools-jsyoo61-2024.5.9.1/tools/torch/model.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:11:53.057611 tools-jsyoo61-2024.5.9.1/tools/torch/optim/
+-rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/torch/optim/__init__.py
+-rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/torch/optim/lr_scheduler.py
+-rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.1/tools/torch/plot.py
+-rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2024.5.9.1/tools/torch/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:11:53.095150 tools-jsyoo61-2024.5.9.1/tools_jsyoo61.egg-info/
+-rw-rw-rw-   0        0        0     1338 2024-05-09 21:11:51.000000 tools-jsyoo61-2024.5.9.1/tools_jsyoo61.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2024-05-09 21:11:52.000000 tools-jsyoo61-2024.5.9.1/tools_jsyoo61.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 21:11:51.000000 tools-jsyoo61-2024.5.9.1/tools_jsyoo61.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-09 21:11:52.000000 tools-jsyoo61-2024.5.9.1/tools_jsyoo61.egg-info/top_level.txt
```

### Comparing `tools-jsyoo61-2024.5.9.0/LICENSE.txt` & `tools-jsyoo61-2024.5.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/PKG-INFO` & `tools-jsyoo61-2024.5.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2024.5.9.0
+Version: 2024.5.9.1
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
 Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tools-jsyoo61-2024.5.9.0/README.md` & `tools-jsyoo61-2024.5.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/setup.py` & `tools-jsyoo61-2024.5.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/array.py` & `tools-jsyoo61-2024.5.9.1/tools/array.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/data.py` & `tools-jsyoo61-2024.5.9.1/tools/data.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/exp.py` & `tools-jsyoo61-2024.5.9.1/tools/exp.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/modules.py` & `tools-jsyoo61-2024.5.9.1/tools/modules.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/numpy/_f.py` & `tools-jsyoo61-2024.5.9.1/tools/numpy/_f.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/numpy/_utils.py` & `tools-jsyoo61-2024.5.9.1/tools/numpy/_utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/os.py` & `tools-jsyoo61-2024.5.9.1/tools/os.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/plot/sklearn.py` & `tools-jsyoo61-2024.5.9.1/tools/plot/sklearn.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/plot/utils.py` & `tools-jsyoo61-2024.5.9.1/tools/plot/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/random.py` & `tools-jsyoo61-2024.5.9.1/tools/random.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/sklearn/model_selection.py` & `tools-jsyoo61-2024.5.9.1/tools/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/stats/__init__.py` & `tools-jsyoo61-2024.5.9.1/tools/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/tools.py` & `tools-jsyoo61-2024.5.9.1/tools/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from copy import deepcopy as dcopy
 import itertools as it
 import os
 import warnings
-from pathlib import Path as P
+import pathlib
 import pickle
 import subprocess
 import time
-import yaml
 
 from . import os as _os
 
 __all__ = \
 [
 #  'Filename',
 'Printer',
@@ -314,15 +313,14 @@
 #     def __repr__(self):
 #         return '(Filename, name: "%s", suffix: "%s")'%(self.name, self.suffix)
 
 #     def __str__(self):
 #         return self.name
 
 # DEPRECATED: use pathlib.Path() instead
-import pathlib
 class Path(pathlib.Path):
     '''
     Joins paths by . syntax
     (Want to use pathlib.Path internally, but currently inherit from str)
 
     Parameters
     ----------
```

### Comparing `tools-jsyoo61-2024.5.9.0/tools/torch/estimator.py` & `tools-jsyoo61-2024.5.9.1/tools/torch/estimator.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/torch/federated_learning.py` & `tools-jsyoo61-2024.5.9.1/tools/torch/federated_learning.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/torch/model.py` & `tools-jsyoo61-2024.5.9.1/tools/torch/model.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/torch/optim/lr_scheduler.py` & `tools-jsyoo61-2024.5.9.1/tools/torch/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools/torch/utils.py` & `tools-jsyoo61-2024.5.9.1/tools/torch/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/PKG-INFO` & `tools-jsyoo61-2024.5.9.1/tools_jsyoo61.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2024.5.9.0
+Version: 2024.5.9.1
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
 Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/SOURCES.txt` & `tools-jsyoo61-2024.5.9.1/tools_jsyoo61.egg-info/SOURCES.txt`

 * *Files identical despite different names*

