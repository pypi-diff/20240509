# Comparing `tmp/dna_se-0.0.6.tar.gz` & `tmp/dna_se-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dna_se-0.0.6.tar", last modified: Thu May  9 06:50:37 2024, max compression
+gzip compressed data, was "dna_se-0.0.7.tar", last modified: Thu May  9 07:03:07 2024, max compression
```

## Comparing `dna_se-0.0.6.tar` & `dna_se-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 06:50:37.000000 dna_se-0.0.6/
-drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 06:50:37.000000 dna_se-0.0.6/DNA_SE/
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     5069 2024-05-09 06:50:16.000000 dna_se-0.0.6/DNA_SE/DNA_SE.py
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)       25 2024-05-08 12:46:34.000000 dna_se-0.0.6/DNA_SE/__init__.py
-drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 06:50:37.000000 dna_se-0.0.6/DNA_SE.egg-info/
--rw-r--r--   0 r12user2  (1003) r12user2  (1003)     2202 2024-05-09 06:50:37.000000 dna_se-0.0.6/DNA_SE.egg-info/PKG-INFO
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)      186 2024-05-09 06:50:37.000000 dna_se-0.0.6/DNA_SE.egg-info/SOURCES.txt
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)        1 2024-05-09 06:50:37.000000 dna_se-0.0.6/DNA_SE.egg-info/dependency_links.txt
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)        7 2024-05-09 06:50:37.000000 dna_se-0.0.6/DNA_SE.egg-info/top_level.txt
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     1091 2024-05-08 12:46:34.000000 dna_se-0.0.6/LICENSE.txt
--rw-r--r--   0 r12user2  (1003) r12user2  (1003)     2202 2024-05-09 06:50:37.000000 dna_se-0.0.6/PKG-INFO
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     1783 2024-05-08 12:46:34.000000 dna_se-0.0.6/README.md
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)       38 2024-05-09 06:50:37.000000 dna_se-0.0.6/setup.cfg
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)      686 2024-05-09 06:50:32.000000 dna_se-0.0.6/setup.py
+drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 07:03:07.000000 dna_se-0.0.7/
+drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 07:03:07.000000 dna_se-0.0.7/DNA_SE/
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     5069 2024-05-09 07:01:44.000000 dna_se-0.0.7/DNA_SE/DNA_SE.py
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)       25 2024-05-08 12:46:34.000000 dna_se-0.0.7/DNA_SE/__init__.py
+drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 07:03:07.000000 dna_se-0.0.7/DNA_SE.egg-info/
+-rw-r--r--   0 r12user2  (1003) r12user2  (1003)     2202 2024-05-09 07:03:07.000000 dna_se-0.0.7/DNA_SE.egg-info/PKG-INFO
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)      186 2024-05-09 07:03:07.000000 dna_se-0.0.7/DNA_SE.egg-info/SOURCES.txt
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)        1 2024-05-09 07:03:07.000000 dna_se-0.0.7/DNA_SE.egg-info/dependency_links.txt
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)        7 2024-05-09 07:03:07.000000 dna_se-0.0.7/DNA_SE.egg-info/top_level.txt
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     1091 2024-05-08 12:46:34.000000 dna_se-0.0.7/LICENSE.txt
+-rw-r--r--   0 r12user2  (1003) r12user2  (1003)     2202 2024-05-09 07:03:07.000000 dna_se-0.0.7/PKG-INFO
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     1783 2024-05-08 12:46:34.000000 dna_se-0.0.7/README.md
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)       38 2024-05-09 07:03:07.000000 dna_se-0.0.7/setup.cfg
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)      686 2024-05-09 07:03:01.000000 dna_se-0.0.7/setup.py
```

### Comparing `dna_se-0.0.6/DNA_SE/DNA_SE.py` & `dna_se-0.0.7/DNA_SE/DNA_SE.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 from torch import nn
 from torch.optim import Adam
 import torch.utils.data as Data
 import numpy as np
 import torch.nn.functional as F     
 
-def dnase(p, Oi, BATCHSIZE, EPOCH, M, B, input_dim, hidden_dim, output_dim, K_func, C, psi_func, depth, activation = 'relu', device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
+def dnase(p, Oi, BATCHSIZE, EPOCH, M, B, input_dim, hidden_dim, output_dim, K_func, C, psi_func, depth, activation = 'tanh', device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
     
     '''
     p: int, the number of features X
     Oi: np.array, the observed data
     BATCHSIZE: int, the batch size
     EPOCH: int, the number of epochs
     M: int, the Monte Carlo number of data points for t
```

### Comparing `dna_se-0.0.6/DNA_SE.egg-info/PKG-INFO` & `dna_se-0.0.7/DNA_SE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DNA_SE
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Home-page: https://github.com/liuqs111/DNA-SE
 Author: Qinshuo
 Author-email: u3008680@connect.hku.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dna_se-0.0.6/LICENSE.txt` & `dna_se-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dna_se-0.0.6/PKG-INFO` & `dna_se-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DNA_SE
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Home-page: https://github.com/liuqs111/DNA-SE
 Author: Qinshuo
 Author-email: u3008680@connect.hku.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dna_se-0.0.6/README.md` & `dna_se-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dna_se-0.0.6/setup.py` & `dna_se-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="DNA_SE", # Replace with your own username
-    version="0.0.6",
+    version="0.0.7",
     author="Qinshuo",
     author_email="u3008680@connect.hku.hk",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liuqs111/DNA-SE",
     packages=setuptools.find_packages(),
```

