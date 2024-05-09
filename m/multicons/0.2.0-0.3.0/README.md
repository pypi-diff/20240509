# Comparing `tmp/multicons-0.2.0.tar.gz` & `tmp/multicons-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicons-0.2.0.tar", last modified: Tue Apr 11 12:51:51 2023, max compression
+gzip compressed data, was "multicons-0.3.0.tar", last modified: Thu May  9 17:36:04 2024, max compression
```

## Comparing `multicons-0.2.0.tar` & `multicons-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:51:51.783020 multicons-0.2.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1066 2023-04-11 12:51:51.000000 multicons-0.2.0/LICENSE.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1892 2023-04-11 12:51:51.783020 multicons-0.2.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1167 2023-04-11 12:51:51.000000 multicons-0.2.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1777 2023-04-11 12:51:51.787020 multicons-0.2.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-04-11 12:51:51.000000 multicons-0.2.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:51:51.783020 multicons-0.2.0/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:51:51.783020 multicons-0.2.0/src/multicons/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      394 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10315 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons/consensus.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16948 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons/core.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4867 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:51:51.783020 multicons-0.2.0/src/multicons.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1892 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      353 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      429 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 17:36:04.361042 multicons-0.3.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2024-05-09 17:36:03.000000 multicons-0.3.0/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2996 2024-05-09 17:36:04.361042 multicons-0.3.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1167 2024-05-09 17:36:03.000000 multicons-0.3.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1850 2024-05-09 17:36:04.365042 multicons-0.3.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-05-09 17:36:03.000000 multicons-0.3.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 17:36:04.357042 multicons-0.3.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 17:36:04.361042 multicons-0.3.0/src/multicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      394 2024-05-09 17:36:03.000000 multicons-0.3.0/src/multicons/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10352 2024-05-09 17:36:03.000000 multicons-0.3.0/src/multicons/consensus.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17057 2024-05-09 17:36:03.000000 multicons-0.3.0/src/multicons/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4867 2024-05-09 17:36:03.000000 multicons-0.3.0/src/multicons/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 17:36:04.361042 multicons-0.3.0/src/multicons.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2996 2024-05-09 17:36:04.000000 multicons-0.3.0/src/multicons.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-05-09 17:36:04.000000 multicons-0.3.0/src/multicons.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-09 17:36:04.000000 multicons-0.3.0/src/multicons.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2024-05-09 17:36:04.000000 multicons-0.3.0/src/multicons.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-05-09 17:36:04.000000 multicons-0.3.0/src/multicons.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-09 17:36:04.000000 multicons-0.3.0/src/multicons.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 17:36:04.361042 multicons-0.3.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4175 2024-05-09 17:36:03.000000 multicons-0.3.0/tests/test_consensus.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8174 2024-05-09 17:36:03.000000 multicons-0.3.0/tests/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6609 2024-05-09 17:36:03.000000 multicons-0.3.0/tests/test_utils.py
```

### Comparing `multicons-0.2.0/LICENSE.md` & `multicons-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `multicons-0.2.0/README.md` & `multicons-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `multicons-0.2.0/setup.cfg` & `multicons-0.3.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multicons
-version = 0.2.0
+version = 0.3.0
 description = MultiCons (Multiple Consensuses) algorithm
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = SergioSim
 author_email = sergio.simonian@etu.univ-cotedazur.fr
 url = https://github.com/SergioSim/multicons
 license = MIT
@@ -12,14 +12,17 @@
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options]
 include_package_data = True
 install_requires = 
 	graphviz>=0.20
 	numpy>=1.24.0
 	pandas>=2.0.0
@@ -29,33 +32,32 @@
 	=src
 packages = find:
 zip_safe = True
 python_requires = >= 3.9
 
 [options.extras_require]
 dev = 
-	bandit==1.7.5
-	black==23.3.0
-	flake8==6.0.0
-	fuzzy-c-means==1.7.0
-	isort==5.12.0
-	jupyterlab==3.6.3
-	jupyter_contrib_nbextensions==0.7.0
-	jupytext==1.14.5
-	matplotlib==3.7.1
-	mkdocs==1.4.2
-	mkdocs-jupyter==0.24.1
-	mkdocs-material==9.1.6
-	mkdocstrings[python]==0.21.2
-	pylint==2.17.2
-	pytest==7.3.0
-	pytest-cov==4.0.0
-	scikit-learn-extra==0.3.0
+	bandit==1.7.8
+	black==24.4.2
+	flake8==7.0.0
+	fuzzy-c-means==1.7.2
+	isort==5.13.2
+	jupyterlab==4.1.8
+	jupytext==1.16.2
+	kmedoids==0.5.1
+	matplotlib==3.8.4
+	mkdocs==1.6.0
+	mkdocs-jupyter==0.24.7
+	mkdocs-material==9.5.21
+	mkdocstrings[python]==0.25.1
+	pylint==3.1.0
+	pytest==8.2.0
+	pytest-cov==5.0.0
 ci = 
-	twine==4.0.2
+	twine==5.0.0
 
 [options.packages.find]
 where = src
 
 [wheel]
 universal = 1
```

### Comparing `multicons-0.2.0/src/multicons/consensus.py` & `multicons-0.3.0/src/multicons/consensus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Consensus functions definitions."""
 
 # pylint: disable=unused-argument
 
+import numpy as np
 import pandas as pd
 import scipy.sparse as sp
 
 
 def consensus_function_10(bi_clust: list[set], merging_threshold=None):
     """Returns a modified bi_clust (set of unique instance sets)."""
 
@@ -185,15 +186,15 @@
 
     while True:
         _remove_subsets(bi_clust)
         bi_clust_size = len(bi_clust)
         if bi_clust_size == 1:
             return
         intersection_matrix = pd.DataFrame(
-            columns=range(bi_clust_size), index=range(bi_clust_size), dtype=int
+            columns=range(bi_clust_size), index=range(bi_clust_size), dtype=float
         )
 
         for i in range(bi_clust_size - 1):
             bi_clust_i = bi_clust[i]
             bi_clust_i_size = len(bi_clust_i)
             for j in range(i + 1, bi_clust_size):
                 bi_clust_j = bi_clust[j]
@@ -217,41 +218,41 @@
         pointer.sort_values(2, inplace=True, ascending=False)
         pointer = pointer[pointer.iloc[:, 2] > 0.0]
 
         for k in range(pointer.shape[0]):
             i = pointer.iloc[k, 0]
             j = pointer.iloc[k, 1]
             value = intersection_matrix.iloc[i, j]
-            if value is None:
+            if np.isnan(value):
                 continue
             if value >= merging_threshold:
                 bi_clust[i] = bi_clust[i].union(bi_clust[j])
                 bi_clust[j] = set()
-                intersection_matrix.iloc[i, :] = None
-                intersection_matrix.iloc[:, j] = None
+                intersection_matrix.iloc[i, :] = np.nan
+                intersection_matrix.iloc[:, j] = np.nan
                 continue
             if len(bi_clust[i]) <= len(bi_clust[j]):
                 bi_clust[j] = bi_clust[j] - bi_clust[i]
-                intersection_matrix.iloc[j, :] = None
-                intersection_matrix.iloc[:, j] = None
+                intersection_matrix.iloc[j, :] = np.nan
+                intersection_matrix.iloc[:, j] = np.nan
                 continue
             bi_clust[i] = bi_clust[i] - bi_clust[j]
-            intersection_matrix.iloc[i, :] = None
-            intersection_matrix.iloc[:, i] = None
+            intersection_matrix.iloc[i, :] = np.nan
+            intersection_matrix.iloc[:, i] = np.nan
 
 
 def consensus_function_15(bi_clust: list[set], merging_threshold: float = 0.5):
     """Returns a modified bi_clust (set of unique instance sets)."""
 
     _remove_subsets(bi_clust)
     bi_clust_size = len(bi_clust)
     if bi_clust_size == 1:
         return
     intersection_matrix = pd.DataFrame(
-        0, columns=range(bi_clust_size), index=range(bi_clust_size), dtype=int
+        0, columns=range(bi_clust_size), index=range(bi_clust_size), dtype=float
     )
     for i in range(bi_clust_size - 1):
         bi_clust_i = bi_clust[i]
         bi_clust_i_size = len(bi_clust_i)
         for j in range(i + 1, bi_clust_size):
             bi_clust_j = bi_clust[j]
             bi_clust_j_size = len(bi_clust_j)
```

### Comparing `multicons-0.2.0/src/multicons/core.py` & `multicons-0.3.0/src/multicons/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,16 +76,17 @@
 
             To use another similarity measure it is possible to pass a function instead
             of a string value. The function should accept two arguments - two numeric
             numpy arrays (representing the two clustering solutions) and should return a
             numeric score (indicating how similar the clustering solutions are).
         merging_threshold (float): Specifies the minimum required ratio (calculated from
             the intersection between two sets over the size of the smaller set) for
-            which the `consensus_function` should merge two sets. Only applies to
-            `consensus_function_12`.
+            which the `consensus_function` should merge two sets. Applies to
+            `consensus_function_12`, `consensus_function_13`, `consensus_function_14`
+            and `consensus_function_15`.
         optimize_label_names (bool): Indicates whether the label assignment of
             the clustering partitions should be optimized to maximize the similarity
             measure score (using the Hungarian algorithm). By default set to `False` as
             the default `similarity_measure` score ("JaccardSimilarity") does not depend
             on which labels are assigned to which cluster.
 
     Attributes:
@@ -171,20 +172,20 @@
         """Computes the MultiCons consensus.
 
         Args:
             X (list of numeric numpy arrays or a pandas Dataframe): Either a list of
                 arrays where each array represents one clustering solution
                 (base clusterings), or a Dataframe representing a binary membership
                 matrix.
-            y: Ignored. Not used, present here for API consistency by convention.
-            sample_weight: Ignored. Not used, present here for API consistency by
+            y (any): Ignored. Not used, present here for API consistency by convention.
+            sample_weight (any): Ignored. Not used, present here for API consistency by
                 convention.
 
         Returns:
-            self: Returns the (fitted) instance itself.
+            self (MultiCons): Returns the (fitted) instance itself.
         """
 
         if isinstance(X, pd.DataFrame):
             membership_matrix = pd.DataFrame(X, dtype=bool)
             X = build_base_clusterings(X)
         else:
             X = np.array(X, dtype=int)
```

### Comparing `multicons-0.2.0/src/multicons/utils.py` & `multicons-0.3.0/src/multicons/utils.py`

 * *Files identical despite different names*

