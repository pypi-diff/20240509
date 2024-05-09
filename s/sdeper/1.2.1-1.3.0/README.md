# Comparing `tmp/sdeper-1.2.1.tar.gz` & `tmp/sdeper-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdeper-1.2.1.tar", last modified: Fri May  3 02:57:10 2024, max compression
+gzip compressed data, was "sdeper-1.3.0.tar", last modified: Thu May  9 04:09:37 2024, max compression
```

## Comparing `sdeper-1.2.1.tar` & `sdeper-1.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:57:10.102728 sdeper-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 02:56:59.000000 sdeper-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 02:56:59.000000 sdeper-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-03 02:57:10.102728 sdeper-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-03 02:56:59.000000 sdeper-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-03 02:56:59.000000 sdeper-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-03 02:56:59.000000 sdeper-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:57:10.102728 sdeper-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-03 02:56:59.000000 sdeper-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:57:10.102728 sdeper-1.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/admm_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    45857 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/cvae.py
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/cvaeglrm.py
--rw-r--r--   0 runner    (1001) docker     (127)    30905 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/diagnosis_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    25987 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/hyper_parameter_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/imputation.py
--rw-r--r--   0 runner    (1001) docker     (127)    49987 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/local_fit_numba.py
--rw-r--r--   0 runner    (1001) docker     (127)    19609 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/model_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    55558 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/parse_opt.py
--rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/run_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:57:10.102728 sdeper-1.2.1/src/sdeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-03 02:57:09.000000 sdeper-1.2.1/src/sdeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-03 02:57:09.000000 sdeper-1.2.1/src/sdeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:57:09.000000 sdeper-1.2.1/src/sdeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 02:57:09.000000 sdeper-1.2.1/src/sdeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-03 02:57:09.000000 sdeper-1.2.1/src/sdeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-03 02:57:09.000000 sdeper-1.2.1/src/sdeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23397 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:09:37.206785 sdeper-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 04:09:30.000000 sdeper-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-09 04:09:30.000000 sdeper-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-09 04:09:37.206785 sdeper-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-09 04:09:30.000000 sdeper-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-09 04:09:30.000000 sdeper-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-09 04:09:30.000000 sdeper-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 04:09:37.206785 sdeper-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-09 04:09:30.000000 sdeper-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:09:37.206785 sdeper-1.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17314 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/admm_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52101 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/cvae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/cvaeglrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31469 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/diagnosis_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26645 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/hyper_parameter_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/imputation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49987 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/local_fit_numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21352 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/model_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55951 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/parse_opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/run_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:09:37.206785 sdeper-1.3.0/src/sdeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-09 04:09:37.000000 sdeper-1.3.0/src/sdeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-09 04:09:37.000000 sdeper-1.3.0/src/sdeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:09:37.000000 sdeper-1.3.0/src/sdeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-09 04:09:37.000000 sdeper-1.3.0/src/sdeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-09 04:09:37.000000 sdeper-1.3.0/src/sdeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-09 04:09:37.000000 sdeper-1.3.0/src/sdeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25297 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-09 04:09:30.000000 sdeper-1.3.0/src/version.py
```

### Comparing `sdeper-1.2.1/LICENSE` & `sdeper-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.1/PKG-INFO` & `sdeper-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: sdeper
-Version: 1.2.1
+Version: 1.3.0
 Summary: Spatial Deconvolution method with Platform Effect Removal
 Home-page: https://az7jh2.github.io/SDePER/
 Author: Ningshan Li
 Author-email: hill103.2@gmail.com
 Project-URL: Documentation, https://sdeper.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/az7jh2/SDePER
 Project-URL: Changelog, https://sdeper.readthedocs.io/en/latest/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9.12, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.22.4
 Requires-Dist: scipy==1.8.1
 Requires-Dist: pandas==1.4.3
 Requires-Dist: networkx==2.8.4
 Requires-Dist: matplotlib==3.5.2
```

### Comparing `sdeper-1.2.1/README.md` & `sdeper-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.1/setup.py` & `sdeper-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,16 @@
         ]
     },
     classifiers = [
         # Get strings from https://pypi.org/classifiers/
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
-        "Operating System :: OS Independent"],
+        "Programming Language :: Python :: 3.10",
+        "Operating System :: POSIX :: Linux"],
     url = "https://az7jh2.github.io/SDePER/",    # homepage
     project_urls={
         # additional relevant URLs
         'Documentation': 'https://sdeper.readthedocs.io/en/latest/',
         'Source': 'https://github.com/az7jh2/SDePER',
         'Changelog': 'https://sdeper.readthedocs.io/en/latest/changelog.html',
         }
```

### Comparing `sdeper-1.2.1/src/admm_fit.py` & `sdeper-1.3.0/src/admm_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,16 @@
             X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
             Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
             A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
             N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
             non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
             spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
             gene_names: a list of string of gene symbols. Only keep actually used marker genes.\n
-            celltype_names: a list of string of celltype names.
+            celltype_names: a list of string of celltype names.\n
+            initial_guess: initial guess of cell-type proportions of spatial spots.
     L : scipy sparse matrix (spots * spots)
         Laplacian matrix
     theta : 3-D numpy array (spots * celltypes * 1)
         initial guess of theta (celltype proportion).
     e_alpha : 1-D numpy array
         initial guess of e_alpha (spot-specific effect).
     gamma_g : 1-D numpy array
```

### Comparing `sdeper-1.2.1/src/config.py` & `sdeper-1.3.0/src/config.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.1/src/cvae.py` & `sdeper-1.3.0/src/cvae.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 @author: hill103
 
 this script stores functions to build a CVAE for platform effect adjustment
 """
 
 
 
-from config import print
+import os
+from config import print, diagnosis_path
 import numpy as np
 import pandas as pd
 from utils import read_spatial_data, read_scRNA_data, run_DE
 from time import time
 import random
+from sklearn.decomposition import PCA
+from sklearn.neighbors import NearestNeighbors
 from sklearn.preprocessing import MinMaxScaler
 import scanpy as sc
 sc.settings.verbosity = 0  # verbosity: errors (0), warnings (1), info (2), hints (3)
 
 import tensorflow.keras.backend as K
 from tensorflow.keras.layers import Lambda, Input, Dense, Activation, concatenate
 from tensorflow.keras.layers import BatchNormalization
@@ -60,14 +63,69 @@
     # calculate cell-type proportions, divides each element in a row by the sum of that row
     celltype_prop = celltype_prop.div(celltype_prop.sum(axis=1), axis=0)
     
     return celltype_prop
 
 
 
+def transferProps(query, ref, ref_props, n_neighbors=10, sigma=1.0):
+    '''
+    transfer cell-type proportions by select K Nearest Neighbors in ref and take Gaussian weighted average of ref proportions
+
+    Parameters
+    ----------
+    query : 2-D numpy matrix
+        encoder embeddings of spatial spots (spots * latent layer neurons).
+    ref : 2-D numpy matrix
+        encoder embeddings of scRNA-seq cells and pseudo-spots in scRNA-seq condition (cells+pseudo-spots * latent layer neurons).
+    ref_props : 2-D numpy matrix
+        cell-type proportion matrix of scRNA-seq cells and pseudo-spots (cells+pseudo-spots * cell-types).
+    n_neighbors : int, optional
+        Number of neighbors to use. The default is 10.
+    sigma : float, optional
+        Standard deviation for the Gaussian weighting function. The default is 1.0.
+
+    Returns
+    -------
+    query_props : 2-D numpy matrix
+        cell-type proportion matrix for spatial spots.
+    '''
+    
+    # first take a PCA to avoid Curse of Dimensionality
+    # we perform PCA without any normalization and scaling, and reduce the dimensionality to one-third of the original dimensions
+    # orginal dimension: 3*#cell-types, reduced dimension: #cell-types
+    principal_components = PCA(n_components=int(query.shape[1]/3)).fit_transform(np.vstack((query, ref)))
+    # Split the principal components back into query and ref
+    query_pc = principal_components[:query.shape[0], :]
+    ref_pc = principal_components[query.shape[0]:, :]
+    
+    # perform KNN on query data on reduced dimension
+    nbrs = NearestNeighbors(n_neighbors=n_neighbors, algorithm='auto').fit(ref_pc)
+    # find nearest neighbors
+    distances, indices = nbrs.kneighbors(query_pc)
+    # Calculate Gaussian weighted averages
+    query_props = np.zeros((query.shape[0], ref_props.shape[1]))
+
+    for i, (dists, inds) in enumerate(zip(distances, indices)):
+        # Compute Gaussian weights
+        weights = np.exp(-dists**2 / (2 * sigma**2))
+        weights /= weights.sum()
+        # Multiply weights with corresponding rows in ref_props (element-wise multiplication)
+        # first inserts a new axis along the second dimension (column) of weights, changing the shape of weights from (K,) to (K, 1).
+        # then perform multiplication with shape (K, m) * (K, 1), numpy broadcasting expands weights along the column dimension (1 dimension), matching the column size of ref_props, and perform element-wise multiplication
+        weighted_props = ref_props[inds] * weights[:, np.newaxis]
+        # calculate weighted average for the current query row; axis=0 sum across columns
+        avg_props = np.sum(weighted_props, axis=0)
+        # normalize the proportions to sum to 1
+        query_props[i] = avg_props / np.sum(avg_props)
+        
+    return query_props
+
+
+
 def generate_pseudo_spots(exp_df, celltype_anno, n_spot, celltype_order, pseudo_spot_min_cell, pseudo_spot_max_cell):
     '''
     generate pseudo-spots for CVAE training by randomly combining scRNA-seq cells
     
     UPDATE:
     
     now we separate the pseudo-spots and all scRNA-seq cells, i.e. we DO NOT add all cells to the end of the dataframe as special pseudo-spots with only one cell
@@ -496,14 +554,16 @@
     -------
     spatial_transformed_numi : dataframe
         CVAE transformed (platform effect adjusted) spatial spot gene raw nUMI counts (spots * genes).
     scRNA_decode_avg_df : dataframe
         CVAE decodered average gene expression (normalized) of cell-types in scRNA-seq data (cell-types * genes).
     new_markers : list or None
         marker genes from re-run DE on CVAE transformed scRNA-seq data. It will be None if not re-run DE (rerun_DE=False).
+    cvae_pred : dataframe or None
+        cell-type proportions of spatial spots predicted or transferred by CVAE. It will be None if no way to got initial guess of cell-type proportions (spots * cell-types).
     '''
     
     assert((scRNA_df.index == scRNA_celltype.index).all())
     assert((spatial_df.columns == scRNA_df.columns).all())
     
     
     if diagnosis:
@@ -520,45 +580,47 @@
     depth_scaler = seq_depth_scaler
     # percentage of training pseudo spots
     training_pct = 0.8
     # max value when scaling the input gene expression of CVAE, while min is 0
     input_max = cvae_input_scaler
     # first log transform, then minmax scaling
     use_log_transform = True
+    # whether to get initial guess of cell-type proportions
+    do_initial_guess = True
     
     # the order of celltypes matters, unify the order throughout whole pipeline, which will be determined here
     celltype_order = sorted(list(scRNA_celltype.celltype.unique()))
     n_celltype = len(celltype_order)
     celltype_count_dict = scRNA_celltype.celltype.value_counts().to_dict()
     
     
     # Randomly select cells into pseudo-spots, at most X pseudo-spots
     # total number of generated pseudo-spots (including training and validation pseudo-spots, NOT include scRNA-seq cells)
-    n_spot_scrna = int(min(100 * spatial_df.shape[0] * n_celltype, n_max_pseudo_spots))
-    n_train_spot_scrna = int(np.floor(n_spot_scrna * training_pct))
-    n_valid_spot_scrna = int(n_spot_scrna - n_train_spot_scrna)
-    print(f'generate {n_spot_scrna} pseudo-spots containing {pseudo_spot_min_cell} to {pseudo_spot_max_cell} cells from scRNA-seq cells...')
+    n_pseudo_scrna = int(min(100 * spatial_df.shape[0] * n_celltype, n_max_pseudo_spots))
+    n_train_pseudo_scrna = int(np.floor(n_pseudo_scrna * training_pct))
+    n_valid_pseudo_scrna = int(n_pseudo_scrna - n_train_pseudo_scrna)
+    print(f'generate {n_pseudo_scrna} pseudo-spots containing {pseudo_spot_min_cell} to {pseudo_spot_max_cell} cells from scRNA-seq cells...')
     # pseudo-spot gene expression (pseudo-spots * genes; NO scRNA-seq cells at the end)
     # pseudo-spot cell-type proportions (pseudo-spots * cell-types; NO scRNA-seq cells at the end)
     # number of cells in pseudo-spots (NO scRNA-seq cells at the end)
-    pseudo_spots_df, pseudo_spots_celltype_prop, n_cell_in_spot = generate_pseudo_spots(scRNA_df, scRNA_celltype, n_spot_scrna, celltype_order, pseudo_spot_min_cell, pseudo_spot_max_cell)
+    pseudo_spots_df, pseudo_spots_celltype_prop, n_cell_in_spot = generate_pseudo_spots(scRNA_df, scRNA_celltype, n_pseudo_scrna, celltype_order, pseudo_spot_min_cell, pseudo_spot_max_cell)
     
     # convert scRNA-seq cell-type annotation to proportions
     scrna_cell_celltype_prop = celltype2props(scRNA_celltype, celltype_order)
     
     
     # generate pseudo-spots by combining spatial spots
     if use_spatial_pseudo:
-        n_spot_spatial = int(0.5 * n_spot_scrna)
+        n_pseudo_spatial = int(0.5 * n_pseudo_scrna)
     else:
-        n_spot_spatial = 0
-    n_train_spot_spatial = int(np.floor(n_spot_spatial * training_pct))
-    n_valid_spot_spatial = int(n_spot_spatial - n_train_spot_spatial)
-    print(f'generate {n_spot_spatial} pseudo-spots containing 2 to 6 spots from spatial spots...')
-    pseudo_spatial_df = combine_spatial_spots(spatial_df, n_spot_spatial, 2, 6)
+        n_pseudo_spatial = 0
+    n_train_pseudo_spatial = int(np.floor(n_pseudo_spatial * training_pct))
+    n_valid_pseudo_spatial = int(n_pseudo_spatial - n_train_pseudo_spatial)
+    print(f'generate {n_pseudo_spatial} pseudo-spots containing 2 to 6 spots from spatial spots...')
+    pseudo_spatial_df = combine_spatial_spots(spatial_df, n_pseudo_spatial, 2, 6)
     
     
     if use_log_transform:
         # since the input dataframe is extracted from AnnData object, and will not be used in downstream analysis (we can extract from AnnData again), it's safe to modify them directly here
         print('\nWARNING: first apply log transformation on sequencing depth normalized gene expressions, followed by Min-Max scaling')
         spatial_df = np.log1p(spatial_df)
         if pseudo_spots_df.shape[0] > 0:
@@ -569,28 +631,28 @@
         scRNA_df = np.log1p(scRNA_df)
     
     
     # Build training and validation data
     # first spots used for validation, rest spots used for training
     print(f'\n{"" : <24} | {"training": >9} | {"validation": >9}')
     print(f'{"spatial spots" : <24} | {spatial_df.shape[0]: >9} | {0: >9}')
-    print(f'{"spatial pseudo-spots" : <24} | {n_train_spot_spatial: >9} | {n_valid_spot_spatial: >9}')
+    print(f'{"spatial pseudo-spots" : <24} | {n_train_pseudo_spatial: >9} | {n_valid_pseudo_spatial: >9}')
     print(f'{"scRNA-seq cells" : <24} | {scRNA_df.shape[0]: >9} | {0: >9}')
-    print(f'{"scRNA-seq pseudo-spots" : <24} | {n_train_spot_scrna: >9} | {n_valid_spot_scrna: >9}\n')
+    print(f'{"scRNA-seq pseudo-spots" : <24} | {n_train_pseudo_scrna: >9} | {n_valid_pseudo_scrna: >9}\n')
     
-    train_scrna_df = pd.concat([pseudo_spots_df.iloc[n_valid_spot_scrna:,:], scRNA_df], ignore_index=False)
-    valid_scrna_df = pseudo_spots_df.iloc[:n_valid_spot_scrna,:]
+    train_scrna_df = pd.concat([pseudo_spots_df.iloc[n_valid_pseudo_scrna:,:], scRNA_df], ignore_index=False)
+    valid_scrna_df = pseudo_spots_df.iloc[:n_valid_pseudo_scrna,:]
     
-    train_spatial_df = pd.concat([pseudo_spatial_df.iloc[n_valid_spot_spatial:,:], spatial_df], ignore_index=False)
-    valid_spatial_df = pseudo_spatial_df.iloc[:n_valid_spot_spatial,:]
+    train_spatial_df = pd.concat([pseudo_spatial_df.iloc[n_valid_pseudo_spatial:,:], spatial_df], ignore_index=False)
+    valid_spatial_df = pseudo_spatial_df.iloc[:n_valid_pseudo_spatial,:]
     
-    assert train_scrna_df.shape[0] == (n_train_spot_scrna + scRNA_df.shape[0])
-    assert valid_scrna_df.shape[0] == n_valid_spot_scrna
-    assert train_spatial_df.shape[0] == (n_train_spot_spatial + spatial_df.shape[0])
-    assert valid_spatial_df.shape[0] == n_valid_spot_spatial
+    assert train_scrna_df.shape[0] == (n_train_pseudo_scrna + scRNA_df.shape[0])
+    assert valid_scrna_df.shape[0] == n_valid_pseudo_scrna
+    assert train_spatial_df.shape[0] == (n_train_pseudo_spatial + spatial_df.shape[0])
+    assert valid_spatial_df.shape[0] == n_valid_pseudo_spatial
     
     # scaling to [0,input_max] with each dataset separately
     # use only spatial spots + spatial pseudo-spots for spatial dataset scaling
     print(f'scaling inputs to range 0 to {input_max}')
     spatial_min_max_scaler = MinMaxScaler(feature_range=[0, input_max])
     train_spatial_data = spatial_min_max_scaler.fit_transform(train_spatial_df)
     if valid_spatial_df.shape[0] > 0:
@@ -605,31 +667,62 @@
         valid_scrna_data = scRNA_min_max_scaler.transform(valid_scrna_df)
     else:
         valid_scrna_data = valid_scrna_df.values
     
     
     # first spatial pseudo-spots then spatial spots then scRNA-seq pseudo-spots and scRNA-seq cells in data
     # we also consider whether to duplicate spatial data since they are few
-    oversample_scale = 1
-    data = np.vstack((np.tile(train_spatial_data, (oversample_scale, 1)), train_scrna_data))
-    labels = np.array([input_max]*train_spatial_data.shape[0]*oversample_scale + [0.]*train_scrna_data.shape[0])
+    # update: use training sample weights
+    data = np.vstack((train_spatial_data, train_scrna_data))
+    labels = np.array([input_max]*train_spatial_data.shape[0] + [0.]*train_scrna_data.shape[0])
     labels = labels.reshape((len(labels), 1))
     
     # validation data
     valid_data = np.vstack((valid_spatial_data, valid_scrna_data))
     valid_labels = np.array([input_max]*valid_spatial_data.shape[0] + [0.]*valid_scrna_data.shape[0])
     valid_labels = valid_labels.reshape((len(valid_labels), 1))
     
     
-    # re-weight spatial data to make sure the sample size equals spatial:scRNA = 1:10
-    sample_weight = np.ones((data.shape[0],))
-
-    if train_spatial_df.shape[0] < 0.1 * train_scrna_data.shape[0]:
-        # spatial data are located in first part
-        sample_weight[:train_spatial_df.shape[0]] *= 0.1 * train_scrna_data.shape[0] / train_spatial_df.shape[0]
+    # training sample weights
+    weight_pseudo_scrna = np.ones((n_train_pseudo_scrna,))
+    weight_cell_scrna = np.ones((scRNA_df.shape[0],))
+    weight_pseudo_spatial = np.ones((n_train_pseudo_spatial,))
+    weight_spot_spatial = np.ones((spatial_df.shape[0],))
+    
+    # weight sum of scRNA-seq cells : sum of scRNA pseudo spots = 1 : 1
+    # always decrease the weights for cohort with more samples
+    if n_train_pseudo_scrna > 0:
+        if n_train_pseudo_scrna > scRNA_df.shape[0]:
+            weight_pseudo_scrna *= scRNA_df.shape[0] / n_train_pseudo_scrna
+        elif n_train_pseudo_scrna < scRNA_df.shape[0]:
+            weight_cell_scrna *= n_train_pseudo_scrna / scRNA_df.shape[0]
+            
+    # weight sum of spatial spots : sum of spatial pseudo spots = 1 : 1
+    # always decrease the weights for cohort with more samples
+    if n_train_pseudo_spatial > 0:
+        if n_train_pseudo_spatial > spatial_df.shape[0]:
+            weight_pseudo_spatial *= spatial_df.shape[0] / n_train_pseudo_spatial
+        elif n_train_pseudo_spatial < spatial_df.shape[0]:
+            weight_spot_spatial *= n_train_pseudo_spatial / spatial_df.shape[0]
+    
+    # Final Balancing, re-weight spatial data to make sure the sum of spatial : sum of scRNA-seq = 1 : 1
+    # since we have already adjusted the weights, here we can not rely on sample size any more, use the sum of weight instead
+    # always decrease the weights for cohort with more samples
+    if (np.sum(weight_pseudo_scrna)+np.sum(weight_cell_scrna)) < (np.sum(weight_pseudo_spatial)+np.sum(weight_spot_spatial)):
+        # calculate factor beforehand to avoid update in weight causing factor change
+        tmp_factor = (np.sum(weight_pseudo_scrna)+np.sum(weight_cell_scrna)) / (np.sum(weight_pseudo_spatial)+np.sum(weight_spot_spatial))
+        weight_pseudo_spatial *= tmp_factor
+        weight_spot_spatial *= tmp_factor
+    elif (np.sum(weight_pseudo_scrna)+np.sum(weight_cell_scrna)) > (np.sum(weight_pseudo_spatial)+np.sum(weight_spot_spatial)):
+        tmp_factor = (np.sum(weight_pseudo_spatial)+np.sum(weight_spot_spatial)) / (np.sum(weight_pseudo_scrna)+np.sum(weight_cell_scrna))
+        weight_pseudo_scrna *= tmp_factor
+        weight_cell_scrna *= tmp_factor
+    
+    sample_weight = np.concatenate([weight_pseudo_spatial, weight_spot_spatial,
+                                    weight_pseudo_scrna, weight_cell_scrna])
     
     del train_spatial_data, valid_spatial_data, train_scrna_data, valid_scrna_data
     del train_spatial_df, valid_spatial_df, train_scrna_df, valid_scrna_df
     
     
     # Define CVAE
     # number of nodes in input layer (equals number of celltypes)
@@ -766,40 +859,55 @@
     scRNA_decode_avg_df['celltype'] = scRNA_celltype.celltype
     scRNA_decode_avg_df = scRNA_decode_avg_df.groupby(['celltype']).mean()
     
     # re-order the rows to match the previous defined cell-type order
     scRNA_decode_avg_df = scRNA_decode_avg_df.loc[celltype_order, :]
     
     
+    # transfer cell-type proportions as an initial guess
+    if n_pseudo_scrna == 0:
+        pseudo_spot_embed = np.empty((0, scRNA_embed.shape[1]))
+    else:
+        pseudo_spot_embed = encoder.predict([scRNA_min_max_scaler.transform(pseudo_spots_df), np.full((pseudo_spots_df.shape[0],1), 0)])[0]
+    
+    if do_initial_guess:
+        tmp_pred = transferProps(spatial_embed,
+                                 np.vstack((scRNA_embed, pseudo_spot_embed)),
+                                 pd.concat([scrna_cell_celltype_prop, pseudo_spots_celltype_prop]).values,
+                                 n_neighbors=10, sigma=1.0)
+        cvae_pred = pd.DataFrame(tmp_pred, index=spatial_df.index, columns=celltype_order)
+        
+        if diagnosis:
+            os.makedirs(os.path.join(diagnosis_path, 'initial_guess'), exist_ok=True)
+            cvae_pred.to_csv(os.path.join(diagnosis_path, 'initial_guess', 'celltype_props_by_transferring.csv'))
+            
+    else:
+        cvae_pred = None
+
+
     # whether to save models and transformed data
     if diagnosis:
-        
         # also embed pseudo-spots for diagnosis
-        if n_spot_spatial == 0:
+        if n_pseudo_spatial == 0:
             pseudo_spatial_embed = np.empty((0, spatial_embed.shape[1]))
         else:
             pseudo_spatial_embed = encoder.predict([spatial_min_max_scaler.transform(pseudo_spatial_df), np.full((pseudo_spatial_df.shape[0],1), input_max)])[0]
         
-        if n_spot_scrna == 0:
-            pseudo_spot_embed = np.empty((0, scRNA_embed.shape[1]))
-        else:
-            pseudo_spot_embed = encoder.predict([scRNA_min_max_scaler.transform(pseudo_spots_df), np.full((pseudo_spots_df.shape[0],1), 0)])[0]
-        
         
         from diagnosis_plots import diagnosisCVAE
         diagnosisCVAE(cvae, encoder, new_decoder,
                       spatial_embed, spatial_transformed_df, spatial_transformed_numi, pseudo_spatial_embed,
                       scRNA_celltype, celltype_order, celltype_count_dict, scrna_cell_celltype_prop, scRNA_embed,
                       pseudo_spots_celltype_prop, n_cell_in_spot, pseudo_spot_embed,
                       scRNA_decode_df, scRNA_decode_avg_df, new_markers, plot_colors)
 
 
     #print(f'before CVAE building function return RAM usage: {psutil.Process().memory_info().rss/1024**2:.2f} MB')
     
-    return spatial_transformed_numi, scRNA_decode_avg_df, new_markers
+    return spatial_transformed_numi, scRNA_decode_avg_df, new_markers, cvae_pred
 
 
 
 def build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_batch_norm, cvae_train_epoch, use_spatial_pseudo, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene):
     '''
     read related CSV files, build CVAE to adjust platform effect, return transformed spatial gene expression and scRNA-seq cell-type gene signature
 
@@ -862,20 +970,22 @@
     -------
     spatial_transformed_numi : dataframe
         CVAE transformed (platform effect adjusted) spatial spot gene raw nUMI counts (spots * genes).
     scRNA_decode_avg_df : dataframe
         CVAE decodered average gene expression (normalized) of cell-types in scRNA-seq data (cell-types * genes).
     new_markers : list or None
         marker genes from re-run DE on CVAE transformed scRNA-seq data. It will be None if not re-run DE.
+    cvae_pred : dataframe or None
+        cell-type proportions of spatial spots predicted or transferred by CVAE. It will be None if no way to got initial guess of cell-type proportions (spots * cell-types).
     '''
     
     start_time = time()
     
     # read spatial data
-    spatial_spot_obj = read_spatial_data(spatial_file, filter_gene)
+    spatial_spot_obj = read_spatial_data(spatial_file, filter_gene)[0]
     
     # read scRNA-seq data
     scrna_obj = read_scRNA_data(ref_file, ref_anno_file, filter_cell, filter_gene)
     
     # Overlap of genes between scRNA cell-level and spatial spot-level data
     overlap_genes = list(set(spatial_spot_obj.var_names).intersection(set(scrna_obj.var_names)))
     print(f'total {len(overlap_genes)} overlapped genes')
@@ -934,18 +1044,19 @@
     print('\nstart CVAE building...\n')
     scrna_celltype = sc.get.obs_df(scrna_obj, keys='celltype').to_frame()
     scrna_celltype['celltype'] = scrna_celltype['celltype'].astype(str)
     
     # build CVAE
     (spatial_transformed_numi,
      scRNA_decode_avg_df,
-     new_markers) = build_CVAE(sc.get.obs_df(spatial_spot_obj, keys=final_gene_list),
-                               sc.get.obs_df(scrna_obj, keys=final_gene_list),
-                               scrna_celltype,
-                               n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler,
-                               cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_batch_norm, cvae_train_epoch, use_spatial_pseudo,
-                               use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc,
-                               diagnosis, rerun_DE=redo_de, filter_gene=filter_gene)
+     new_markers,
+     cvae_pred) = build_CVAE(sc.get.obs_df(spatial_spot_obj, keys=final_gene_list),
+                             sc.get.obs_df(scrna_obj, keys=final_gene_list),
+                             scrna_celltype,
+                             n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler,
+                             cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_batch_norm, cvae_train_epoch, use_spatial_pseudo,
+                             use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc,
+                             diagnosis, rerun_DE=redo_de, filter_gene=filter_gene)
     
     print(f'\nplatform effect adjustment by CVAE finished. Elapsed time: {(time()-start_time)/60.0:.2f} minutes.\n\n')
     
-    return spatial_transformed_numi, scRNA_decode_avg_df, new_markers
+    return spatial_transformed_numi, scRNA_decode_avg_df, new_markers, cvae_pred
```

### Comparing `sdeper-1.2.1/src/cvaeglrm.py` & `sdeper-1.3.0/src/cvaeglrm.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.1/src/diagnosis_plots.py` & `sdeper-1.3.0/src/diagnosis_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         mu in latent space of spatial pseudo-spots (spatial pseudo-spots * latent neurons). It will have 0 rows if no spatial pseudo-spots generated
     scRNA_celltype : dataframe
         cell-type annotations for cells in scRNA-seq data. Only 1 column named <celltype>
     celltype_order : list
         already sorted unique cell-types. Its order matters, and will be the order in pseudo_spots_celltype (columns) and cell-type gene expression profile (rows)
     celltype_count_dict : dict
         number of cells in reference scRNA-seq data for each cell-type
-    scrna_cell_celltype_prop : dict
+    scrna_cell_celltype_prop : dataframe
         scRNA-seq cells cell-type proportions (cells * cell-types)
     scRNA_embed : 2-D numpy array
         mu in latent space of scRNA-seq cells (cells * latent neurons)
     pseudo_spots_celltype_prop : dataframe
         pseudo-spot cell-type proportions (pseudo-spots * cell-types; NO scRNA-seq cells included)
     n_cell_in_spot : list
         number of cells in pseudo-spots (no scRNA-seq cells included)
@@ -267,17 +267,26 @@
     # save model
     cvae.save(os.path.join(diagnosis_path, 'CVAE_model', 'CVAE_whole.h5'))
     encoder.save(os.path.join(diagnosis_path, 'CVAE_model', 'CVAE_encoder.h5'))
     decoder.save(os.path.join(diagnosis_path, 'CVAE_model', 'CVAE_decoder.h5'))
     
     
     # save transformed data, which are used in GLRM modeling
-    spatial_transformed_numi.to_csv(os.path.join(diagnosis_path, 'CVAE_transformed_data', 'spatial_spots_transformToscRNA_decoded.csv.gz'), compression='gzip')
-    scRNA_decode_avg_df.to_csv(os.path.join(diagnosis_path, 'CVAE_transformed_data', 'scRNA_decoded_avg_exp_bycelltypes.csv.gz'), compression='gzip')
-    
+    if new_markers is None:
+        spatial_transformed_numi.to_csv(os.path.join(diagnosis_path, 'CVAE_transformed_data', 'spatial_spots_transformToscRNA_decoded.csv.gz'), compression='gzip')
+    else:
+        # save only marker genes used in downstream anlaysis
+        spatial_transformed_numi[new_markers].to_csv(os.path.join(diagnosis_path, 'CVAE_transformed_data', 'spatial_spots_transformToscRNA_decoded.csv.gz'), compression='gzip')
+    
+    if new_markers is None:
+        scRNA_decode_avg_df.to_csv(os.path.join(diagnosis_path, 'CVAE_transformed_data', 'scRNA_decoded_avg_exp_bycelltypes.csv.gz'), compression='gzip')
+    else:
+        # save only marker genes used in downstream anlaysis
+        scRNA_decode_avg_df[new_markers].to_csv(os.path.join(diagnosis_path, 'CVAE_transformed_data', 'scRNA_decoded_avg_exp_bycelltypes.csv.gz'), compression='gzip')
+        
     
     # plot variance of mu of spatial spots and scRNA-seq cells
     latent_var = np.concatenate((spatial_embed, scRNA_embed), axis=0).var(axis=0)
     plt.figure()
     ax = sns.histplot(x=np.log10(latent_var))
     ax.set(xlabel='log10(var(mu))')
     plt.savefig(os.path.join(diagnosis_path, 'CVAE_latent_space', 'histogram_latent_neurons_variance_spatial_spots_and_scRNA-seq_cells.png'))
```

### Comparing `sdeper-1.2.1/src/hyper_parameter_optimization.py` & `sdeper-1.3.0/src/hyper_parameter_optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
             Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
             A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
             N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
             non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
             spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
             gene_names: a list of string of gene symbols. Only keep actually used marker genes.\n
             celltype_names: a list of string of celltype names.\n
+            initial_guess: initial guess of cell-type proportions of spatial spots.
     mle_theta : 3-D numpy array (spots * celltypes * 1)
         estimated theta (celltype proportion) by MLE.
     mle_e_alpha : 1-D numpy array
         estimated e_alpha (spot-specific effect) by MLE.
     gamma_g : 1-D numpy array
         gene-specific platform effect for all genes.
     sigma2 : float
@@ -318,15 +319,15 @@
         diagnosisParamsTuning(candidate_list, avg_rmse_list, optimal_idx, 'lambda_r', y_label)
         
 
     return candidate_list[optimal_idx]
     
     
     
-def cv_find_lambda_g(data, G, theta_mask, gamma_g, sigma2, candidate_list, hybrid_version=True, opt_method='L-BFGS-B', hv_x=None, hv_log_p=None, use_admm=True, use_likelihood=True, k=5, use_cache=True, diagnosis=False):
+def cv_find_lambda_g(data, G, stage1_theta, stage1_e_alpha, theta_mask, gamma_g, sigma2, candidate_list, hybrid_version=True, opt_method='L-BFGS-B', hv_x=None, hv_log_p=None, use_admm=True, use_likelihood=True, k=5, use_cache=True, diagnosis=False):
     '''
     find optimal value for hyper-parameter lambda_g by k fold cross-validation
     
     Parameters
     ----------
     data : Dict
         a Dict contains all info need for modeling:
@@ -334,14 +335,21 @@
             Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
             A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
             N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
             non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
             spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
             gene_names: a list of string of gene symbols. Only keep actually used marker genes.\n
             celltype_names: a list of string of celltype names.\n
+            initial_guess: initial guess of cell-type proportions of spatial spots.
+    G : built graph object from networks module
+        used for constructing Laplacian Matrix.
+    stage1_theta : 3-D numpy array (spots * celltypes * 1)
+        estimated theta (celltype proportion) in stage 1.
+    stage1_e_alpha : 1-D numpy array
+        estimated e_alpha (spot-specific effect) in stage 1.
     theta_mask : 3-D numpy array (spots * celltypes * 1)
         mask for cell-type proportions (1: present, 0: not present). Only used for stage 2 theta optmization.
     gamma_g : 1-D numpy array
         gene-specific platform effect for all genes.
     sigma2 : float
         variance paramter of the lognormal distribution of ln(lambda). All gene share the same variance.
     candidate_list : list
@@ -383,20 +391,26 @@
     
     # add 0 to candidate list
     candidate_list = [0] + candidate_list
     
     n_spot, n_gene = data['Y'].shape
     
     # re-initialize theta and e_alpha for only present cell-types
+    # update: reuse the result from stage 1
+    '''
     start_theta = np.zeros(theta_mask.shape)
     for i in range(n_spot):
         start_theta[i, theta_mask[i,:,:]==1] = 1.0/np.sum(theta_mask[i,:,:])
     
     start_e_alpha = np.full((n_spot,), 1.0)
-
+    '''
+    
+    start_theta = stage1_theta.copy()
+    start_e_alpha = stage1_e_alpha.copy()
+    
     # random permute the genes
     gene_idx = np.arange(n_gene)
     # set seed for reproducibility
     np.random.seed(420)
     np.random.shuffle(gene_idx)
     # divided into k folds
     fold_size = floor(n_gene / float(k))
```

### Comparing `sdeper-1.2.1/src/imputation.py` & `sdeper-1.3.0/src/imputation.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.1/src/local_fit_numba.py` & `sdeper-1.3.0/src/local_fit_numba.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.1/src/model_fit.py` & `sdeper-1.3.0/src/model_fit.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import scipy.sparse as sparse
 from utils import reparameterTheta
 from hyper_parameter_optimization import cv_find_lambda_r, cv_find_lambda_g
 from config import min_val, print, sigma2_digits
 
 
 
-def fit_base_model(data, gamma_g=None, global_optimize=False, hybrid_version=True, opt_method='L-BFGS-B', verbose=False, use_cache=True):
+def fit_base_model(data, gamma_g=None, global_optimize=False, hybrid_version=True, opt_method='L-BFGS-B', verbose=False, use_cache=True, use_initial_guess=False):
     '''
     fit local or base model without any Adaptive Lasso constrain or Graph Laplacian constrain
     
     this fitting is only used for gamma_g estimation and MLE theta estimation in GLRM stage 1
     
     when fitting the base model, we will perform fitting iteratively until the sigma^2 change <= 0.001
     
@@ -40,27 +40,30 @@
             X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
             Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
             A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
             N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
             non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
             spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
             gene_names: a list of string of gene symbols. Only keep actually used marker gene symbols.\n
-            celltype_names: a list of string of celltype names.
+            celltype_names: a list of string of celltype names.\n
+            initial_guess: initial guess of cell-type proportions of spatial spots.
     gamma_g : 1-D numpy array
         gene-specific platform effect for all genes.
     global_optimize : bool, optional
         if is True, use basin-hopping algorithm to find the global minimum. The default is False.
     hybrid_version : bool, optional
         if True, use the hybrid_version of GLRM, i.e. in ADMM local model loss function optimization for w but adaptive lasso constrain on theta. If False, local model loss function optimization and adaptive lasso will on the same w. The default is True.
     opt_method : string, optional
         specify method used in scipy.optimize.minimize for local model fitting. The default is 'L-BFGS-B', a default method in scipy for optimization with bounds. Another choice would be 'SLSQP', a default method in scipy for optimization with constrains and bounds.
     verbose : bool, optional
         if True, print more information in program running.
     use_cache : bool, optional
         if True, use the cached dict of calculated negative log-likelihood values.
+    use_initial_guess : bool, optional
+        if True, use initial guess instead of uniform distribution for theta initialization.
 
     Returns
     -------
     tuple
         a tuple of estimated theta, e_alpha and sigma2:
             theta : celltype proportions (3-D numpy array (spots * celltypes * 1))\n
             e_alpha : spot-specific effect (1-D array with length #spot)\n
@@ -72,15 +75,25 @@
     n_celltype, n_gene = data['X'].shape
     n_spot = data['Y'].shape[0]
     
     if verbose:
         print('\nGLRM model initialization...')
     
     # Initialization
-    theta = np.full((n_spot, n_celltype, 1), 1.0/n_celltype)
+    if use_initial_guess and (data['initial_guess'] is not None):
+        print('HIGHLIGHT: use initial guess derived from CVAE rather than uniform distribution for theta initialization')
+        assert data['initial_guess'].index.to_list() == data['spot_names']
+        assert data['initial_guess'].columns.to_list() == data['celltype_names']
+        theta = data['initial_guess'].values
+        # note the shape is (#spots, #cell-types, 1)
+        # use np.newaxis to add a new third dimension
+        theta = theta[:, :, np.newaxis]
+    else:
+        theta = np.full((n_spot, n_celltype, 1), 1.0/n_celltype)
+        
     e_alpha = np.full((n_spot,), 1.0)
     
     if use_cache:
         sigma2 = round(1.0, sigma2_digits)
     else:
         sigma2 = 1.0
    
@@ -156,15 +169,16 @@
             X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
             Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
             A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
             N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
             non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
             spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
             gene_names: a list of string of gene symbols. Only keep actually used marker gene symbols.\n
-            celltype_names: a list of string of celltype names.
+            celltype_names: a list of string of celltype names.\n
+            initial_guess: initial guess of cell-type proportions of spatial spots.
     hybrid_version : bool, optional
         if True, use the hybrid_version of GLRM, i.e. in ADMM local model loss function optimization for w but adaptive lasso constrain on theta. If False, local model loss function optimization and adaptive lasso will on the same w. The default is True.
     opt_method : string, optional
         specify method used in scipy.optimize.minimize for local model fitting. The default is 'L-BFGS-B', a default method in scipy for optimization with bounds. Another choice would be 'SLSQP', a default method in scipy for optimization with constrains and bounds.
     verbose : bool, optional
         if True, print more information in program running
     
@@ -187,15 +201,15 @@
     # genes with nUMI>0
     if data['non_zero_mtx'] is None:
         tmp_data['non_zero_mtx'] = None
     else:
         tmp_data['non_zero_mtx'] = np.sum(data['non_zero_mtx'], axis=0, keepdims=True) > 0
     
     # fit base model
-    theta, e_alpha, _ = fit_base_model(tmp_data, global_optimize=True, hybrid_version=hybrid_version, opt_method=opt_method, verbose=verbose, use_cache=False)
+    theta, e_alpha, _ = fit_base_model(tmp_data, global_optimize=True, hybrid_version=hybrid_version, opt_method=opt_method, verbose=verbose, use_cache=False, use_initial_guess=False)
     
     
     assert(len(e_alpha)==1)
     # calculate gamma_g
     # note theta is 3-Dimensional
     w = np.squeeze(theta) * e_alpha[0]
     
@@ -218,15 +232,16 @@
             X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
             Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
             A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
             N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
             non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
             spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
             gene_names: a list of string of gene symbols. Only keep actually used marker genes.\n
-            celltype_names: a list of string of celltype names.
+            celltype_names: a list of string of celltype names.\n
+            initial_guess: initial guess of cell-type proportions of spatial spots.
     G : built graph object from networks module
         used for constructing Laplacian Matrix
     gamma_g : 1-D numpy array
         gene-specific platform effect for all genes.
     lambda_r : float
         strength for Adaptive Lasso penalty. If None, use cross-validation to determine optimal lambda_r
     weight_threshold : float, optional
@@ -266,15 +281,15 @@
     n_spot = data['Y'].shape[0]
     
     
     print('first estimate MLE theta and corresponding e^alpha and sigma^2...')
     
     tmp_start_time = time()
     
-    theta, e_alpha, sigma2 = fit_base_model(data, gamma_g=gamma_g, global_optimize=global_optimize, hybrid_version=hybrid_version, opt_method=opt_method, verbose=True, use_cache=use_cache)
+    theta, e_alpha, sigma2 = fit_base_model(data, gamma_g=gamma_g, global_optimize=global_optimize, hybrid_version=hybrid_version, opt_method=opt_method, verbose=True, use_cache=use_cache, use_initial_guess=True)
     
     print(f'MLE theta estimation finished. Elapsed time: {(time()-tmp_start_time)/60.0:.2f} minutes.')
     
     # initialize x array for calculation of heavy-tail
     from local_fit_numba import z_hv, generate_log_heavytail_array
     # initialize density values of heavy-tail with initial sigma^2
     log_p_hv = generate_log_heavytail_array(z_hv, np.sqrt(sigma2))
@@ -331,19 +346,36 @@
     
     # stage 2
     tmp_start_time = time()
     
     print('\nStage 2: final theta estimation with Graph Laplacian Constrain using already estimated sigma^2 and gamma_g')
     
     # re-initialize theta and e_alpha for only present cell-types
+    # update: reuse the result from stage 1
+    '''
     theta = np.zeros(theta.shape)
     for i in range(n_spot):
         theta[i, theta_mask[i,:,:]==1] = 1.0/np.sum(theta_mask[i,:,:])
     
     e_alpha = np.full((n_spot,), 1.0)
+    '''
+    
+    # note theta shape is (#spots * #celltypes * 1)
+    theta[theta < weight_threshold] = 0
+    tmp_row_sums = theta.sum(axis=1)  # Sum along the second axis, got matrix (#spots * 1)
+    theta = theta / tmp_row_sums[:, np.newaxis] # broadcasting row sum to (#spots * 1 * 1) then performs element-wise division
+    assert theta.shape == theta_mask.shape
+    for i in range(theta.shape[0]):
+        assert abs(np.sum(theta[i,:,:]) - 1) < 1e-8
+    
+    # reuse e_alpha, as it related to spot not cell-types
+    e_alpha = stage1_result['e_alpha']
+    
+    print('HIGHLIGHT: reuse estimated theta and e^alpha in stage 1 as initial value')
+    
     
     if data['A'] is None:
         
         print('No Adjacency Matrix of spots specified! Ignore Graph Laplacian Constrain in stage 2')
         # Laplacian Matrix is all 0
         # transform it to a scipy sparse matrix to be consistent with Laplacian Matrix derived from graph object
         L = sparse.csr_matrix(np.zeros((n_spot, n_spot)))
@@ -357,15 +389,15 @@
     else:
         
         # considering Laplacian Constrain
         print(f'specified hyper-parameter for Graph Laplacian Constrain is: {lambda_g}')
     
         if isinstance(lambda_g, list):
             print(f'hyper-parameter for Graph Laplacian Constrain: use cross-validation to find the optimal value from {len(lambda_g)} candidates...')
-            lambda_g = cv_find_lambda_g(data, G, theta_mask, gamma_g, sigma2, lambda_g, hybrid_version=hybrid_version, opt_method=opt_method, hv_x=z_hv, hv_log_p=log_p_hv, use_admm=True, use_likelihood=True, use_cache=use_cache, diagnosis=diagnosis)
+            lambda_g = cv_find_lambda_g(data, G, theta, e_alpha, theta_mask, gamma_g, sigma2, lambda_g, hybrid_version=hybrid_version, opt_method=opt_method, hv_x=z_hv, hv_log_p=log_p_hv, use_admm=True, use_likelihood=True, use_cache=use_cache, diagnosis=diagnosis)
     
         # update edge weight in Graph, otherwise edge will have weight 1, then calculate the Laplacian Matrix
         for _, _, e in G.edges(data=True):
             e["weight"] = lambda_g
         # calculate Laplacian, result is a SciPy sparse matrix
         L = nx.laplacian_matrix(G)
```

### Comparing `sdeper-1.2.1/src/parse_opt.py` & `sdeper-1.3.0/src/parse_opt.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 checking on parameters will also be performed
 """
 
 
 
 from getopt import getopt
 import sys, os
-from config import print, input_path, cur_version
+from config import print, input_path, diagnosis_path, cur_version
 import numpy as np
 import pandas as pd
 import copy
 
 
 
 # default value for options
 default_paramdict = {'spatial_file': None, 'ref_file': None, 'ref_celltype_file': None, 'marker_file': None, 'loc_file': None, 'A_file': None,
                      'n_cores': 1, 'threshold': 0, 'use_cvae': True, 'use_imputation': False, 'diagnosis': False, 'verbose': True,
                      'use_fdr': True, 'p_val_cutoff': 0.05, 'fc_cutoff': 1.2, 'pct1_cutoff': 0.3, 'pct2_cutoff': 0.1, 'sortby_fc': True, 'n_marker_per_cmp': 20, 'filter_cell': True, 'filter_gene': True,
-                     'n_hv_gene': 200,  'n_pseudo_spot': 500000, 'pseudo_spot_min_cell': 2, 'pseudo_spot_max_cell':8, 'seq_depth_scaler': 10000, 'cvae_input_scaler': 10, 'cvae_init_lr':0.01, 'num_hidden_layer': 2, 'use_batch_norm': True, 'cvae_train_epoch': 500, 'use_spatial_pseudo': False, 'redo_de': True, 'seed': 383,
+                     'n_hv_gene': 200,  'n_pseudo_spot': 100000, 'pseudo_spot_min_cell': 2, 'pseudo_spot_max_cell':8, 'seq_depth_scaler': 10000, 'cvae_input_scaler': 10, 'cvae_init_lr':0.01, 'num_hidden_layer': 2, 'use_batch_norm': True, 'cvae_train_epoch': 500, 'use_spatial_pseudo': False, 'redo_de': True, 'seed': 383,
                      'lambda_r': None, 'lambda_r_range_min': 0.1, 'lambda_r_range_max': 100, 'lambda_r_range_k': 8,
                      'lambda_g': None, 'lambda_g_range_min': 0.1, 'lambda_g_range_max': 100, 'lambda_g_range_k': 8,
                      'diameter': 200, 'impute_diameter': [160, 114, 80]
                     }
 
 
 
@@ -814,8 +814,18 @@
                     paramdict['use_imputation'] = False
     
     
     print('\nrunning options:')
     for k,v in paramdict.items():
         print(f'{k}: {v}')
         
+    if paramdict['diagnosis']:
+        # need to create subfolders first, otherwise got FileNotFoundError
+        os.makedirs(diagnosis_path, exist_ok=True)
+        
+        # save options to file
+        with open(os.path.join(diagnosis_path, 'SDePER_settings.txt'), "w") as file:
+            for k, v in paramdict.items():
+                file.write(f"{k}: {v}\n")
+
+        
     return paramdict
```

### Comparing `sdeper-1.2.1/src/preprocess.py` & `sdeper-1.3.0/src/preprocess.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,18 +18,17 @@
     4. filter genes and spots before GLRM modeling
     
     5. check datasets to avoid some mistakes
 """
 
 
 
-import numpy as np
 import pandas as pd
 from cvae import build_CVAE_whole
-from utils import run_DE_only
+from utils import read_spatial_data, run_DE_only
 from config import print
 
 
 
 def preprocess(spatial_file, ref_file, ref_anno_file, marker_file, A_file, use_cvae, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_batch_norm, cvae_train_epoch, use_spatial_pseudo, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, filter_cell, filter_gene, diagnosis):
     '''
     preprocess files
@@ -100,58 +99,39 @@
             X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
             Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
             A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
             N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
             non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
             spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
             gene_names: a list of string of gene symbols. Only keep actually used marker gene symbols.\n
-            celltype_names: a list of string of celltype names.
+            celltype_names: a list of string of cell-type names.\n
+            initial_guess: initial guess of cell-type proportions of spatial spots.
     '''
     
     # first determine whether to build CVAE
     if use_cvae:
         if ref_file is None or ref_anno_file is None:
             raise Exception('ERROR: building CVAE requires both reference scRNA-seq data and corresponding cell-type annotation specified! But at least one of them is not specified!')
             
         print('first build CVAE...\n')
         # build CVAE, and return the data dict including transformed spatial data and reference gene expression
-        spatial_df, cvae_marker_df, new_markers = build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_batch_norm, cvae_train_epoch, use_spatial_pseudo, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene)
+        spatial_df, cvae_marker_df, new_markers, cvae_pred = build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_batch_norm, cvae_train_epoch, use_spatial_pseudo, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene)
         
         # calculate squencing depth, sum also works on sparse dataframe
         N = spatial_df.sum(axis=1)
     
     else:
         
         print('building CVAE skipped...\n')
         
-        # to_dense has been depreated
-        # read spatial dataframe into a sparse dataframe
-        # the default mangle_dupe_cols=True will handle the duplicated columns
-        spatial_df = pd.concat(chunk.astype('Sparse[int]') for chunk in pd.read_csv(spatial_file, index_col=0, chunksize=1e4))
-        print(f'read spatial data from file {spatial_file}')
-        print(f'total {spatial_df.shape[0]} spots; {spatial_df.shape[1]} genes\n')
-        
-        # check whether cell name are unique
-        if len(set(spatial_df.index.to_list())) < spatial_df.shape[0]:
-            raise Exception('spot barcodes in spatial data are not unique!')
-            
-        # filtering genes
-        if filter_gene:
-            # Remove genes present in <3 cells
-            pre_n_gene = spatial_df.shape[1]
-            spatial_df = spatial_df.loc[:, spatial_df.apply(lambda x: np.count_nonzero(x), axis=0) >= 3].copy()
-            if pre_n_gene > spatial_df.shape[1]:
-                print(f'filtering genes present in <3 spots: {pre_n_gene-spatial_df.shape[1]} genes removed\n')
-            else:
-                print('filtering genes present in <3 spots: No genes removed\n')
-    
-        # calculate squencing depth, sum also works on sparse dataframe
-        N = spatial_df.sum(axis=1)
+        # read spatial data
+        spatial_obj, spatial_df, N = read_spatial_data(spatial_file, filter_gene)
         
         new_markers = None
+        cvae_pred = None
     
         
     # use marker genes from original scRNA-seq or CVAE transformed data
     if new_markers is None:
         
         # whether to perform DE
         if marker_file is not None:
@@ -203,14 +183,19 @@
     else:
         print('all genes passed filtering')
     
     # subset genes
     spatial_df = spatial_df[marker_genes]
     marker_df = marker_df[marker_genes]
     
+    # reorder cell-type orders in marker gene profile for consistency
+    celltype_order = sorted(marker_df.index.to_list())
+    if cvae_pred is not None:
+        assert celltype_order == cvae_pred.columns.to_list()
+    marker_df = marker_df.loc[celltype_order, :]
     
     if A_file is None:
         A_df = None
     else:
         A_df = pd.read_csv(A_file, index_col=0)
         
     # filter spots based on sum of nUMI
@@ -226,18 +211,27 @@
         print('all spots passed filtering')
         
         
     if diagnosis and not use_cvae:
         # plot UMAP for raw input gene expressions here
         import scanpy as sc
         from diagnosis_plots import defineColor, rawInputUMAP
-        tmp_scrna_celltype = sc.get.obs_df(tmp_scrna_obj, keys='celltype').to_frame()
-        tmp_scrna_celltype['celltype'] = tmp_scrna_celltype['celltype'].astype(str)
-        plot_colors = defineColor(spatial_df.shape[0], tmp_scrna_celltype)
-        rawInputUMAP(spatial_df, sc.get.obs_df(tmp_scrna_obj, keys=marker_genes), tmp_scrna_celltype, plot_colors)
+        # get raw input of scRNA-seq cells
+        if 'tmp_scrna_obj' not in locals():
+            if ref_file is not None and ref_anno_file is not None:
+                from utils import read_scRNA_data
+                tmp_scrna_obj = read_scRNA_data(ref_file, ref_anno_file, filter_cell, filter_gene)
+            else:
+                tmp_scrna_obj = None
+        
+        if tmp_scrna_obj is not None:
+            tmp_scrna_celltype = sc.get.obs_df(tmp_scrna_obj, keys='celltype').to_frame()
+            tmp_scrna_celltype['celltype'] = tmp_scrna_celltype['celltype'].astype(str)
+            plot_colors = defineColor(spatial_df.shape[0], tmp_scrna_celltype)
+            rawInputUMAP(spatial_df, sc.get.obs_df(tmp_scrna_obj, keys=marker_genes), tmp_scrna_celltype, plot_colors)
 
     
     # record the zeros in spatial data if filtering zeros is turned on
     filter_zero_gene = False
     use_original_nUMI = True
     
     if filter_zero_gene:
@@ -276,8 +270,9 @@
     return {'X': marker_df.values,
             'Y': spatial_df.values,
             'A': A,
             'N': N.values,
             'non_zero_mtx': non_zero_mtx,
             'spot_names': spatial_df.index.to_list(),
             'gene_names': spatial_df.columns.to_list(),
-            'celltype_names': marker_df.index.to_list()}
+            'celltype_names': marker_df.index.to_list(),
+            'initial_guess': cvae_pred}
```

### Comparing `sdeper-1.2.1/src/run_model.py` & `sdeper-1.3.0/src/run_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,16 @@
             X: a 2-D numpy matrix of celltype specific marker gene expression (celltypes * genes).\n
             Y: a 2-D numpy matrix of spatial gene expression (spots * genes).\n
             A: a 2-D numpy matrix of Adjacency matrix (spots * spots), or is None. Adjacency matrix of spatial sptots (1: connected / 0: disconnected). All 0 in diagonal.\n
             N: a 1-D numpy array of sequencing depth of all spots (length #spots). If it's None, use sum of observed marker gene expressions as sequencing depth.\n
             non_zero_mtx: If it's None, then do not filter zeros during regression. If it's a bool 2-D numpy matrix (spots * genes) as False means genes whose nUMI=0 while True means genes whose nUMI>0 in corresponding spots. The bool indicators can be calculated based on either observerd raw nUMI counts in spatial data, or CVAE transformed nUMI counts.\n
             spot_names: a list of string of spot barcodes. Only keep spots passed filtering.\n
             gene_names: a list of string of gene symbols. Only keep actually used marker genes.\n
-            celltype_names: a list of string of celltype names.
+            celltype_names: a list of string of celltype names.\n
+            initial_guess: initial guess of cell-type proportions of spatial spots.
     lambda_r : float, optional
         strength for Adaptive Lasso penalty. The default is None, i.e. use cross-validation to determine optimal value
     weight_threshold : float, optional
         threshold for Adaptive Lasso weight. Theta values smaller than threshold value will be re-set. The default is 1e-3.
     lambda_g : float, optional
         edge weight for graph, and will affect the strength of Graph Laplacian constrain. The default is None, i.e. use cross-validation to determine optimal value
     estimate_gamma_g : bool, optional
@@ -101,15 +102,15 @@
     print('use weight threshold for Adaptive Lasso: ', weight_threshold)
     
     from local_fit_numba import update_unique_nUMI
     update_unique_nUMI(data['Y'])
     
     use_cache = False
     if use_cache:
-        print('use dict to cache likelihoods in regression')
+        print('HIGHLIGHT: use dict to cache likelihoods in regression for quick calculation')
     
     # define graph from adjacency matrix
     if data['A'] is None:
         # empty graph
         G = nx.empty_graph(n_spot)
     else:
         np.fill_diagonal(data['A'], 0)
```

### Comparing `sdeper-1.2.1/src/sdeper.egg-info/PKG-INFO` & `sdeper-1.3.0/src/sdeper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: sdeper
-Version: 1.2.1
+Version: 1.3.0
 Summary: Spatial Deconvolution method with Platform Effect Removal
 Home-page: https://az7jh2.github.io/SDePER/
 Author: Ningshan Li
 Author-email: hill103.2@gmail.com
 Project-URL: Documentation, https://sdeper.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/az7jh2/SDePER
 Project-URL: Changelog, https://sdeper.readthedocs.io/en/latest/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9.12, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.22.4
 Requires-Dist: scipy==1.8.1
 Requires-Dist: pandas==1.4.3
 Requires-Dist: networkx==2.8.4
 Requires-Dist: matplotlib==3.5.2
```

### Comparing `sdeper-1.2.1/src/sdeper.egg-info/SOURCES.txt` & `sdeper-1.3.0/src/sdeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.1/src/utils.py` & `sdeper-1.3.0/src/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,28 +80,35 @@
         re-parametrization w = e^alpha * theta.
     '''
     
     return e_alpha[:, None, None] * theta
 
 
 
-def read_spatial_data(spatial_file, filter_gene):
+def read_spatial_data(spatial_file, filter_gene, n_hv_gene=0):
     '''
     read spatial data saved as a CSV file by Scanpy
 
     Parameters
     ----------
     spatial_file : string
         full path of input csv file of raw nUMI counts in spatial transcriptomic data (spots * genes).
     filter_gene : bool
         whether to filter genes before DE.
+    n_hv_gene : int
+        number of highly variable genes to be kept in spatial data. If equals 0, all genes are kept.
         
     Returns
     -------
-    a AnnData object
+    spatial_spot_obj : a AnnData object
+        AnnData object of spatial spot data.
+    tmp_df : dataframe
+        dataframe of raw nUMI of spatial data (spots * genes).
+    N : series
+        sequencing depth per spot.
     '''
     
     # Read spatial spot-level data
     spatial_spot_obj = sc.read_csv(spatial_file)
     print(f'read spatial data from file {spatial_file}')
     print(f'total {spatial_spot_obj.n_obs} spots; {spatial_spot_obj.n_vars} genes\n')
     
@@ -120,18 +127,38 @@
         if pre_n_gene > spatial_spot_obj.n_vars:
             print(f'filtering genes present in <3 spots: {pre_n_gene-spatial_spot_obj.n_vars} genes removed\n')
         else:
             print('filtering genes present in <3 spots: No genes removed\n')
             
     # make a DEEP COPY of raw nUMI count
     spatial_spot_obj.layers['raw_nUMI'] = spatial_spot_obj.X.copy()
+    
+    # calculate sequencing depth per cell, note currently X is nUMI, we make a deep copy to avoid dataframe change
+    tmp_df = spatial_spot_obj.to_df().copy()
+    N = tmp_df.sum(axis=1) # sum also works on sparse dataframe
+    
     # Normalize each cell by total counts over ALL genes
     sc.pp.normalize_total(spatial_spot_obj, target_sum=1, inplace=True)
     
-    return spatial_spot_obj
+    # identify highly variable genes in spatial data, select TOP X HV genes
+    # no need to consider highly variable genes in spatial data, as for cell-type deconvolution, we work on each spot independently
+    if n_hv_gene >= spatial_spot_obj.n_vars:
+        print(f'\nWARNING: use all {spatial_spot_obj.n_vars} genes for downstream analysis as available genes in spatial data <= specified highly varabile gene number {n_hv_gene}')
+    
+    elif n_hv_gene > 0:
+        print(f'\nWARNING: identify {n_hv_gene} highly variable genes from spatial data and keep those genes only...')
+        spatial_hv_genes = sc.pp.highly_variable_genes(spatial_spot_obj, layer='raw_nUMI', flavor='seurat_v3', n_top_genes=n_hv_gene, inplace=False)
+        spatial_hv_genes = spatial_hv_genes.loc[spatial_hv_genes['highly_variable']==True].index.to_list()
+        spatial_spot_obj = spatial_spot_obj[:, spatial_hv_genes].copy()
+        
+        tmp_df = tmp_df[spatial_hv_genes]
+    
+    print(f'remain {spatial_spot_obj.n_obs} spots; {spatial_spot_obj.n_vars} genes for downstream analysis\n')
+    
+    return spatial_spot_obj, tmp_df, N
 
 
 
 def read_scRNA_data(ref_file, ref_anno_file, filter_cell, filter_gene):
     '''
     read scRNA-seq data saved as a CSV file by Scanpy, also read cell-type annotation, then subset cells with cell-type annotation
 
@@ -205,14 +232,16 @@
             print('filtering genes present in <10 cells: No genes removed\n')
     
     # make a DEEP COPY of raw nUMI count
     scrna_obj.layers['raw_nUMI'] = scrna_obj.X.copy()
     # Normalize each cell by total counts over ALL genes
     sc.pp.normalize_total(scrna_obj, target_sum=1, inplace=True)
     
+    print(f'remain {scrna_obj.n_obs} cells; {scrna_obj.n_vars} genes for downstream analysis\n')
+    
     return scrna_obj
 
 
 
 def run_DE(sc_obj, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, save_result=False, save_file_name=None):
     '''
     differential on cell-types in scRNA-seq data.
@@ -324,15 +353,15 @@
             # add cell-types
             tmp_df['celltype1'] = this_celltype
             tmp_df['celltype2'] = other_celltype
             
             if tmp_df.shape[0] <= n_marker_per_cmp:
                 
                 if tmp_df.shape[0] < n_marker_per_cmp:
-                    print(f'WARNING: only {tmp_df.shape[0]} genes passing filtering (<{n_marker_per_cmp}) for {this_celltype} vs {other_celltype}')
+                    print(f'\nWARNING: only {tmp_df.shape[0]} genes passing filtering (<{n_marker_per_cmp}) for {this_celltype} vs {other_celltype}')
                 
                 # no need to further rank, directly select all available genes
                 scrna_marker_genes += tmp_df['names'].to_list()
                 
                 # combine DE result
                 tmp_df['selected'] = 1
             
@@ -361,15 +390,17 @@
                 scrna_marker_genes += tmp_df['names'].to_list()[:n_marker_per_cmp]
                 # combine DE result
                 tmp_df['selected'] = 0
                 tmp_df.loc[tmp_df.index.to_list()[:n_marker_per_cmp], 'selected'] = 1
             
             tmp_df.rename(columns={'names': 'gene'}, inplace=True)
             de_result_list.append(tmp_df.loc[:, ['gene', 'logfoldchanges', 'pvals', 'pvals_adj', 'pct1', 'pct2', 'celltype1', 'celltype2', 'selected']].copy())
-
+    
+    print('100%')
+    
     scrna_marker_genes = sorted(list(set(scrna_marker_genes)))
     print(f'finally selected {len(scrna_marker_genes)} cell-type marker genes\n')
     
     if save_result:
         os.makedirs(os.path.join(diagnosis_path, 'celltype_markers'), exist_ok=True)
         pd.concat(de_result_list).to_csv(os.path.join(diagnosis_path, 'celltype_markers', save_file_name)+'.gz', index=False, compression='gzip')
     
@@ -420,14 +451,15 @@
         average gene expressions of identified cell-type specific marker genes from refer scRNA-seq data
     '''
     
     scrna_obj = read_scRNA_data(ref_file, ref_anno_file, filter_cell, filter_gene)
     
     # subset genes
     overlap_genes = list(set(spatial_genes).intersection(set(scrna_obj.var_names)))
+    print(f'get {len(overlap_genes)} overlapped genes between spatial data and reference scRNA-seq data\n')
     #if len(overlap_genes) < len(spatial_genes):
         #print(f'{len(spatial_genes)-len(overlap_genes)} genes in spatial data but not found in scRNA-seq data: {", ".join(set(spatial_genes).difference(set(overlap_genes)))}\n')
     
     scrna_obj = scrna_obj[:, overlap_genes].copy()
     
     # DE
     marker_genes = run_DE(scrna_obj, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, save_result, 'DE_celltype_markers.csv')
```

