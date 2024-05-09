# Comparing `tmp/cellxgene-schema-5.0.2rc1.tar.gz` & `tmp/cellxgene-schema-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene-schema-5.0.2rc1.tar", last modified: Tue Apr  2 16:52:52 2024, max compression
+gzip compressed data, was "cellxgene-schema-5.0.3.tar", last modified: Thu May  9 20:24:20 2024, max compression
```

## Comparing `cellxgene-schema-5.0.2rc1.tar` & `cellxgene-schema-5.0.3.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxr-xr-x   0 ngloria    (502) staff       (20)        0 2024-04-02 16:52:52.517512 cellxgene-schema-5.0.2rc1/
--rw-r--r--   0 ngloria    (502) staff       (20)     1098 2022-06-09 16:50:04.000000 cellxgene-schema-5.0.2rc1/LICENSE.txt
--rw-r--r--   0 ngloria    (502) staff       (20)      174 2022-09-27 19:46:36.000000 cellxgene-schema-5.0.2rc1/MANIFEST.in
--rw-r--r--   0 ngloria    (502) staff       (20)      723 2024-04-02 16:52:52.517617 cellxgene-schema-5.0.2rc1/PKG-INFO
-drwxr-xr-x   0 ngloria    (502) staff       (20)        0 2024-04-02 16:52:52.515313 cellxgene-schema-5.0.2rc1/cellxgene_schema/
--rw-r--r--   0 ngloria    (502) staff       (20)       27 2024-04-02 16:52:21.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/__init__.py
--rw-r--r--   0 ngloria    (502) staff       (20)     3902 2024-04-02 16:42:30.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/cli.py
--rw-r--r--   0 ngloria    (502) staff       (20)      493 2024-04-02 16:44:16.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/env.py
--rw-r--r--   0 ngloria    (502) staff       (20)     3304 2024-04-02 16:44:16.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/gencode.py
--rw-r--r--   0 ngloria    (502) staff       (20)    14201 2024-04-02 16:42:30.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/migrate.py
--rw-r--r--   0 ngloria    (502) staff       (20)     2774 2023-09-14 14:21:43.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/remove_labels.py
--rw-r--r--   0 ngloria    (502) staff       (20)      522 2023-09-14 14:21:43.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/schema.py
-drwxr-xr-x   0 ngloria    (502) staff       (20)        0 2024-04-02 16:52:52.516971 cellxgene-schema-5.0.2rc1/cellxgene_schema/schema_definitions/
--rw-r--r--   0 ngloria    (502) staff       (20)    28970 2024-04-02 16:44:21.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/schema_definitions/schema_definition.yaml
--rw-r--r--   0 ngloria    (502) staff       (20)     6738 2024-03-14 20:00:30.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/utils.py
--rw-r--r--   0 ngloria    (502) staff       (20)    63353 2024-04-02 16:44:21.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/validate.py
--rw-r--r--   0 ngloria    (502) staff       (20)    15528 2024-04-02 16:44:16.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/write_labels.py
-drwxr-xr-x   0 ngloria    (502) staff       (20)        0 2024-04-02 16:52:52.516772 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/
--rw-r--r--   0 ngloria    (502) staff       (20)      723 2024-04-02 16:52:52.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/PKG-INFO
--rw-r--r--   0 ngloria    (502) staff       (20)      681 2024-04-02 16:52:52.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/SOURCES.txt
--rw-r--r--   0 ngloria    (502) staff       (20)        1 2024-04-02 16:52:52.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/dependency_links.txt
--rw-r--r--   0 ngloria    (502) staff       (20)       70 2024-04-02 16:52:52.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/entry_points.txt
--rw-r--r--   0 ngloria    (502) staff       (20)        1 2023-12-13 19:01:56.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/not-zip-safe
--rw-r--r--   0 ngloria    (502) staff       (20)      176 2024-04-02 16:52:52.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/requires.txt
--rw-r--r--   0 ngloria    (502) staff       (20)       17 2024-04-02 16:52:52.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/top_level.txt
--rw-r--r--   0 ngloria    (502) staff       (20)      176 2024-04-02 16:44:16.000000 cellxgene-schema-5.0.2rc1/requirements.txt
--rw-r--r--   0 ngloria    (502) staff       (20)       70 2024-04-02 16:52:52.518251 cellxgene-schema-5.0.2rc1/setup.cfg
--rw-r--r--   0 ngloria    (502) staff       (20)     1229 2024-04-02 16:52:21.000000 cellxgene-schema-5.0.2rc1/setup.py
+drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-09 20:24:20.833459 cellxgene-schema-5.0.3/
+-rw-r--r--   0 trentsmith   (502) staff       (20)     1098 2022-06-01 19:47:22.000000 cellxgene-schema-5.0.3/LICENSE.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)      120 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/MANIFEST.in
+-rw-r--r--   0 trentsmith   (502) staff       (20)      701 2024-05-09 20:24:20.833561 cellxgene-schema-5.0.3/PKG-INFO
+drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-09 20:24:20.828253 cellxgene-schema-5.0.3/cellxgene_schema/
+-rw-r--r--   0 trentsmith   (502) staff       (20)       22 2024-05-09 20:23:37.000000 cellxgene-schema-5.0.3/cellxgene_schema/__init__.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)     3902 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/cli.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)      493 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/env.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)     3304 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/gencode.py
+drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-09 20:24:20.832880 cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/
+-rw-r--r--   0 trentsmith   (502) staff       (20)      714 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/genes_ercc.csv.gz
+-rw-r--r--   0 trentsmith   (502) staff       (20)   673926 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/genes_homo_sapiens.csv.gz
+-rw-r--r--   0 trentsmith   (502) staff       (20)   599259 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/genes_mus_musculus.csv.gz
+-rw-r--r--   0 trentsmith   (502) staff       (20)      171 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/gencode_files/genes_sars_cov_2.csv.gz
+-rw-r--r--   0 trentsmith   (502) staff       (20)    14201 2024-05-09 19:20:45.000000 cellxgene-schema-5.0.3/cellxgene_schema/migrate.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)     2774 2023-09-18 18:32:37.000000 cellxgene-schema-5.0.3/cellxgene_schema/remove_labels.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)      522 2023-09-18 18:32:37.000000 cellxgene-schema-5.0.3/cellxgene_schema/schema.py
+drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-09 20:24:20.833089 cellxgene-schema-5.0.3/cellxgene_schema/schema_definitions/
+-rw-r--r--   0 trentsmith   (502) staff       (20)    28970 2024-04-29 23:23:16.000000 cellxgene-schema-5.0.3/cellxgene_schema/schema_definitions/schema_definition.yaml
+-rw-r--r--   0 trentsmith   (502) staff       (20)     6738 2024-03-08 00:33:50.000000 cellxgene-schema-5.0.3/cellxgene_schema/utils.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)    90667 2024-05-09 20:23:37.000000 cellxgene-schema-5.0.3/cellxgene_schema/validate.py
+-rw-r--r--   0 trentsmith   (502) staff       (20)    15528 2024-04-25 22:44:06.000000 cellxgene-schema-5.0.3/cellxgene_schema/write_labels.py
+drwxr-xr-x   0 trentsmith   (502) staff       (20)        0 2024-05-09 20:24:20.829627 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/
+-rw-r--r--   0 trentsmith   (502) staff       (20)      701 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/PKG-INFO
+-rw-r--r--   0 trentsmith   (502) staff       (20)      899 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)        1 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)       69 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/entry_points.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)        1 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/not-zip-safe
+-rw-r--r--   0 trentsmith   (502) staff       (20)      189 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/requires.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)       17 2024-05-09 20:24:20.000000 cellxgene-schema-5.0.3/cellxgene_schema.egg-info/top_level.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)      276 2024-05-09 19:20:45.000000 cellxgene-schema-5.0.3/requirements.txt
+-rw-r--r--   0 trentsmith   (502) staff       (20)       70 2024-05-09 20:24:20.833822 cellxgene-schema-5.0.3/setup.cfg
+-rw-r--r--   0 trentsmith   (502) staff       (20)     1224 2024-05-09 20:23:37.000000 cellxgene-schema-5.0.3/setup.py
```

### Comparing `cellxgene-schema-5.0.2rc1/LICENSE.txt` & `cellxgene-schema-5.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc1/PKG-INFO` & `cellxgene-schema-5.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: cellxgene-schema
-Version: 5.0.2rc1
+Version: 5.0.3
 Summary: Tool for applying and validating cellxgene integration schema to single cell datasets
 Home-page: https://github.com/chanzuckerberg/single-cell-curation
 Author: Chan Zuckerberg Initiative
 Author-email: cellxgene@chanzuckerberg.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 License-File: LICENSE.txt
 
 Tool for applying and validating cellxgene integration schema to single cell datasets
-
```

### Comparing `cellxgene-schema-5.0.2rc1/cellxgene_schema/cli.py` & `cellxgene-schema-5.0.3/cellxgene_schema/cli.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc1/cellxgene_schema/gencode.py` & `cellxgene-schema-5.0.3/cellxgene_schema/gencode.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc1/cellxgene_schema/migrate.py` & `cellxgene-schema-5.0.3/cellxgene_schema/migrate.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc1/cellxgene_schema/remove_labels.py` & `cellxgene-schema-5.0.3/cellxgene_schema/remove_labels.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc1/cellxgene_schema/schema.py` & `cellxgene-schema-5.0.3/cellxgene_schema/schema.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc1/cellxgene_schema/schema_definitions/schema_definition.yaml` & `cellxgene-schema-5.0.3/cellxgene_schema/schema_definitions/schema_definition.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-title: Corpora schema version 4.X.X
+title: Corpora schema version 5.X.X
 type: anndata
 # If sparsity of any expression matrix is greater than this and not csr sparse matrix, then there will be warning.
 sparsity: 0.5
 # If the R array will exceed this number in size, then Seurat conversion will fail
 max_size_for_seurat: 2147483647  # 2^31 - 1 (max value for 4-byte signed int)
 # Perform the checks for "raw" requirements IF:
 raw:
```

### Comparing `cellxgene-schema-5.0.2rc1/cellxgene_schema/utils.py` & `cellxgene-schema-5.0.3/cellxgene_schema/utils.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc1/cellxgene_schema/validate.py` & `cellxgene-schema-5.0.3/cellxgene_schema/validate.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,47 +18,106 @@
 from . import gencode, schema
 from .utils import SPARSE_MATRIX_TYPES, get_matrix_format, getattr_anndata, read_h5ad
 
 logger = logging.getLogger(__name__)
 
 ONTOLOGY_PARSER = OntologyParser(schema_version=f"v{schema.get_current_schema_version()}")
 
+ASSAY_VISIUM = "EFO:0010961"
+ASSAY_SLIDE_SEQV2 = "EFO:0030062"
+
+VISIUM_AND_IS_SINGLE_TRUE_MATRIX_SIZE = 4992
+SPATIAL_HIRES_IMAGE_MAX_DIMENSION_SIZE = 2000
+
+ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE = "obs['assay_ontology_term_id'] 'EFO:0010961' (Visium Spatial Gene Expression) and uns['spatial']['is_single'] is True"
+ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE_FORBIDDEN = f"is only allowed for {ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE}"
+ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE_REQUIRED = f"is required for {ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE}"
+ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE_IN_TISSUE_0 = f"{ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE} and in_tissue is 0"
+
 
 class Validator:
     """Handles validation of AnnData"""
 
     def __init__(self, ignore_labels=False):
         self.schema_def = dict()
         self.schema_version: str = None
         self.ignore_labels = ignore_labels
+        self.visium_and_is_single_true_matrix_size = VISIUM_AND_IS_SINGLE_TRUE_MATRIX_SIZE
 
         # Values will be instances of gencode.GeneChecker,
         # keys will be one of gencode.SupportedOrganisms
         self.gene_checkers = dict()
 
     def reset(self):
         self.errors = []
         self.warnings = []
         self.is_valid = False
         self.h5ad_path = ""
         self._raw_layer_exists = None
         self.is_seurat_convertible: bool = True
+        self.is_spatial = None
+        self.is_visium = None
+        self.is_visium_and_is_single_true = None
 
         # Matrix (e.g., X, raw.X, ...) number non-zero cache
         self.number_non_zero = dict()
 
     @property
     def adata(self) -> anndata.AnnData:
         return self._adata
 
     @adata.setter
     def adata(self, adata: anndata.AnnData):
         self.reset()
         self._adata = adata
 
+    def _is_single(self) -> bool | None:
+        """
+        Determine value of uns.spatial.is_single. None if non-spatial.
+
+        :return Value of uns.spatial.is_single if specified, None otherwise.
+        :rtype bool | None
+        """
+        return (
+            self.adata.uns["spatial"]["is_single"]
+            if hasattr(self.adata, "uns")
+            and "spatial" in self.adata.uns
+            and isinstance(self.adata.uns["spatial"], dict)
+            and "is_single" in self.adata.uns["spatial"]
+            else None
+        )
+
+    def _is_supported_spatial_assay(self) -> bool:
+        """
+        Determine if the assay_ontology_term_id is either Visium (EFO:0010961) or Slide-seqV2 (EFO:0030062).
+
+        :return True if assay_ontology_term_id is Visium or Slide-seqV2, False otherwise.
+        :rtype bool
+        """
+        if self.is_spatial is None:
+            try:
+                self.is_spatial = False
+                if self.adata.obs.assay_ontology_term_id.isin([ASSAY_VISIUM, ASSAY_SLIDE_SEQV2]).any():
+                    self.is_spatial = True
+            except AttributeError:
+                # specific error reporting will occur downstream in the validation
+                self.is_spatial = False
+        return self.is_spatial
+
+    def _is_visium_and_is_single_true(self) -> bool:
+        """
+        Determine if the assay_ontology_term_id is Visium (EFO:0010961) and uns.spatial.is_single is True.
+
+        :return True if assay_ontology_term_id is Visium and is_single_cell is True, False otherwise.
+        :rtype bool
+        """
+        if self.is_visium_and_is_single_true is None:
+            self.is_visium_and_is_single_true = bool(self._is_visium() and self._is_single())
+        return self.is_visium_and_is_single_true
+
     def _validate_encoding_version(self):
         import h5py
 
         with h5py.File(self.h5ad_path, "r") as f:
             encoding_dict = dict(f.attrs)
             encoding_version = encoding_dict.get("encoding-version")
             if encoding_version != "0.1.0":
@@ -875,14 +934,22 @@
     def _validate_seurat_convertibility(self):
         """
         Use length of component matrices to determine if the anndata object will be unable to be converted to Seurat by
         virtue of the R language's array size limit (4-byte signed int length). Add warning for each matrix which is
         too large.
         rtype: None
         """
+        # Seurat conversion is not supported for Visium datasets.
+        if self._is_visium():
+            self.warnings.append(
+                "Datasets with assay_ontology_term_id 'EFO:0010961' (Visium Spatial Gene Expression) are not compatible with Seurat."
+            )
+            self.is_seurat_convertible = False
+            return
+
         to_validate = [(self.adata.X, "X")]
         # check if there's raw data
         if self.adata.raw:
             to_validate.append((self.adata.raw.X, "raw.X"))
         # Check length of component arrays
         for matrix, matrix_name in to_validate:
             matrix_format = get_matrix_format(self.adata, matrix)
@@ -939,57 +1006,88 @@
 
         obsm_with_x_prefix = 0
         for key, value in self.adata.obsm.items():
             issue_list = self.errors
 
             regex_pattern = r"^[a-zA-Z][a-zA-Z0-9_.-]*$"
 
+            unknown_key = False  # an unknown key does not match 'spatial' or 'X_{suffix}'
             if key.startswith("X_"):
                 obsm_with_x_prefix += 1
+                # if key.lower() == "x_spatial":  # TODO undo after 5.0 patch release
+                #     self.errors.append(f"Embedding key in 'adata.obsm' {key} cannot be used.")
                 if not re.match(regex_pattern, key[2:]):
                     self.errors.append(
                         f"Suffix for embedding key in 'adata.obsm' {key} does not match the regex pattern {regex_pattern}."
                     )
-            else:
+            elif key.lower() != "spatial":
                 if not re.match(regex_pattern, key):
                     self.errors.append(
                         f"Embedding key in 'adata.obsm' {key} does not match the regex pattern {regex_pattern}."
                     )
                 self.warnings.append(
-                    f"Embedding key in 'adata.obsm' {key} does not start with X_ and thus will not be available in Explorer"
+                    f"Embedding key in 'adata.obsm' {key} is not 'spatial' nor does it start with 'X_'. Thus, it will "
+                    f"not be available in Explorer"
                 )
                 issue_list = self.warnings
+                unknown_key = True
 
             if not isinstance(value, np.ndarray):
-                issue_list.append(
+                self.errors.append(
                     f"All embeddings have to be of 'numpy.ndarray' type, " f"'adata.obsm['{key}']' is {type(value)}')."
                 )
                 # Skip over the subsequent checks that require the value to be an array
                 continue
 
-            if len(value.shape) < 2 or value.shape[0] != self.adata.n_obs or value.shape[1] < 2:
-                issue_list.append(
-                    f"All embeddings must have as many rows as cells, and at least two columns."
-                    f" 'adata.obsm['{key}']' has shape of '{value.shape}'."
+            if len(value.shape) < 2:
+                self.errors.append(
+                    f"All embeddings must at least two dimensions. 'adata.obsm['{key}']' has a shape length of '{len(value.shape)}'."
                 )
+            else:
+                if value.shape[0] != self.adata.n_obs:
+                    self.errors.append(
+                        f"All embeddings must have as many rows as cells. 'adata.obsm['{key}']' has rows='{value.shape[0]}'."
+                    )
+
+                if unknown_key and value.shape[1] < 1:
+                    self.errors.append(
+                        f"All unspecified embeddings must have at least one column. 'adata.obsm['{key}']' has columns='{value.shape[1]}'."
+                    )
+
+                if not unknown_key and value.shape[1] < 2:
+                    self.errors.append(
+                        f"All 'X_' and 'spatial' embeddings must have at least two columns. 'adata.obsm['{key}']' has columns='{value.shape[1]}'."
+                    )
+
             if not (np.issubdtype(value.dtype, np.integer) or np.issubdtype(value.dtype, np.floating)):
                 issue_list.append(
                     f"adata.obsm['{key}'] has an invalid data type. It should be "
                     "float, integer, or unsigned integer of any precision (8, 16, 32, or 64 bits)."
                 )
             else:
                 # Check for inf/NaN values only if the dtype is numeric
                 if np.isinf(value).any():
                     issue_list.append(f"adata.obsm['{key}'] contains positive infinity or negative infinity values.")
                 if np.all(np.isnan(value)):
                     issue_list.append(f"adata.obsm['{key}'] contains all NaN values.")
 
-        if obsm_with_x_prefix == 0:
+        if self._is_supported_spatial_assay() is False and obsm_with_x_prefix == 0:
             self.errors.append("At least one embedding in 'obsm' has to have a key with an 'X_' prefix.")
 
+        is_single = self._is_single()
+        has_spatial_embedding = "spatial" in self.adata.obsm
+        if is_single and not has_spatial_embedding:
+            self.errors.append(
+                "'spatial' embedding is required in 'adata.obsm' if " "adata.uns['spatial']['is_single'] is True."
+            )
+        elif is_single is None and has_spatial_embedding:
+            self.errors.append(
+                "'spatial' embedding is forbidden in 'adata.obsm' if " "adata.uns['spatial']['is_single'] is not set."
+            )
+
     def _validate_annotation_mapping(self, component_name: str, component: Mapping):
         for key, value in component.items():
             # Check for empty ndarrays
             if isinstance(value, np.ndarray) and not value.size:
                 self.errors.append(
                     f"The size of the ndarray stored for a 'adata.{component_name}['{key}']' MUST NOT be zero."
                 )
@@ -1064,45 +1162,122 @@
                 self._raw_layer_exists = False
                 self.errors.append("Raw matrix values must have type numpy.float32.")
                 return self._raw_layer_exists
 
             matrix_format = get_matrix_format(self.adata, x)
             assert matrix_format != "unknown"
             self._raw_layer_exists = True
-            has_row_of_zeros = False
-            has_invalid_nonzero_value = False
             is_sparse_matrix = matrix_format in SPARSE_MATRIX_TYPES
-            for matrix_chunk, _, _ in self._chunk_matrix(x):
-                if not has_row_of_zeros:
-                    if is_sparse_matrix:
-                        row_indices, _ = matrix_chunk.nonzero()
-                        if len(set(row_indices)) != matrix_chunk.shape[0]:
-                            has_row_of_zeros = True
-                    # else, must be dense matrix, confirm that all rows have at least 1 nonzero value
-                    elif not all(np.apply_along_axis(np.any, axis=1, arr=matrix_chunk)):
-                        has_row_of_zeros = True
 
-                if not has_invalid_nonzero_value:
-                    data = matrix_chunk if isinstance(matrix_chunk, np.ndarray) else matrix_chunk.data
-                    if np.any((data % 1 > 0) | (data < 0)):
-                        has_invalid_nonzero_value = True
-
-                if has_row_of_zeros and has_invalid_nonzero_value:
-                    # Fail fast, exit loop and report
-                    break
-
-            if has_row_of_zeros:
-                self._raw_layer_exists = False
-                self.errors.append("Each cell must have at least one non-zero value in its row in the raw matrix.")
-            if has_invalid_nonzero_value:
+            is_visium_and_is_single_true = self._is_visium_and_is_single_true()
+            if is_visium_and_is_single_true and x.shape[0] != self.visium_and_is_single_true_matrix_size:
                 self._raw_layer_exists = False
-                self.errors.append("All non-zero values in raw matrix must be positive integers of type numpy.float32.")
+                self.errors.append(
+                    f"When {ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE}, the raw matrix must be the "
+                    f"unfiltered feature-barcode matrix 'raw_feature_bc_matrix'. It must have exactly "
+                    f"{self.visium_and_is_single_true_matrix_size} rows. Raw matrix row count is "
+                    f"{x.shape[0]}."
+                )
+
+            if (
+                is_visium_and_is_single_true
+                and "in_tissue" in self.adata.obs
+                and 0 in self.adata.obs["in_tissue"].values
+            ):
+                self._validate_raw_data_with_in_tissue_0(x, is_sparse_matrix)
+            else:
+                self._validate_raw_data(x, is_sparse_matrix)
 
         return self._raw_layer_exists
 
+    def _validate_raw_data(self, x: Union[np.ndarray, sparse.spmatrix], is_sparse_matrix: bool):
+        """
+        Validates the data values in the raw matrix. Matrix size is chunked for large matrices.
+
+        :param x: raw matrix
+        :param is_sparse_matrix: bool indicating if the matrix is sparse {csc, csr, coo}
+        """
+        has_row_of_zeros = False
+        has_invalid_nonzero_value = False
+        for matrix_chunk, _, _ in self._chunk_matrix(x):
+            if not has_row_of_zeros:
+                if is_sparse_matrix:
+                    row_indices, _ = matrix_chunk.nonzero()
+                    if len(set(row_indices)) != matrix_chunk.shape[0]:
+                        has_row_of_zeros = True
+                # else, must be dense matrix, confirm that all rows have at least 1 nonzero value
+                elif not all(np.apply_along_axis(np.any, axis=1, arr=matrix_chunk)):
+                    has_row_of_zeros = True
+
+            if not has_invalid_nonzero_value and self._matrix_has_invalid_nonzero_values(matrix_chunk):
+                has_invalid_nonzero_value = True
+
+            if has_row_of_zeros and has_invalid_nonzero_value:
+                # Fail fast, exit loop and report
+                break
+
+        if has_row_of_zeros:
+            self._raw_layer_exists = False
+            self.errors.append("Each cell must have at least one non-zero value in its row in the raw matrix.")
+        if has_invalid_nonzero_value:
+            self._raw_layer_exists = False
+            self.errors.append("All non-zero values in raw matrix must be positive integers of type numpy.float32.")
+
+    def _validate_raw_data_with_in_tissue_0(self, x: Union[np.ndarray, sparse.spmatrix], is_sparse_matrix: bool):
+        """
+        Special case validation checks for Visium data with is_single = True and in_tissue column in obs where in_tissue
+        has at least one value 0. Static matrix size of 4992 rows, so chunking is not required.
+
+        :param x: raw matrix
+        :param is_sparse_matrix: bool indicating if the matrix is sparse {csc, csr, coo}
+        """
+        has_tissue_0_non_zero_row = False
+        has_tissue_1_zero_row = False
+        if is_sparse_matrix:
+            nonzero_row_indices, _ = x.nonzero()
+        else:  # must be dense matrix
+            nonzero_row_indices = np.where(np.any(x != 0, axis=1))[0]
+        for i in range(x.shape[0]):
+            if not has_tissue_0_non_zero_row and i in nonzero_row_indices and self.adata.obs["in_tissue"][i] == 0:
+                has_tissue_0_non_zero_row = True
+            elif not has_tissue_1_zero_row and i not in nonzero_row_indices and self.adata.obs["in_tissue"][i] == 1:
+                has_tissue_1_zero_row = True
+            if has_tissue_0_non_zero_row and has_tissue_1_zero_row:
+                # exit early and report
+                break
+
+        if not has_tissue_0_non_zero_row:
+            self._raw_layer_exists = False
+            self.errors.append(
+                "If obs['in_tissue'] contains at least one value 0, then there must be at least "
+                "one row with obs['in_tissue'] == 0 that has a non-zero value in the raw matrix."
+            )
+        if has_tissue_1_zero_row:
+            self._raw_layer_exists = False
+            self.errors.append(
+                "Each observation with obs['in_tissue'] == 1 must have at least one "
+                "non-zero value in its row in the raw matrix."
+            )
+        if self._matrix_has_invalid_nonzero_values(x):
+            self._raw_layer_exists = False
+            self.errors.append("All non-zero values in raw matrix must be positive integers of type numpy.float32.")
+
+    def _matrix_has_invalid_nonzero_values(self, x: Union[np.ndarray, sparse.spmatrix]) -> bool:
+        """
+        Checks whether the matrix has invalid non-zero values. The matrix must have all non-zero values as positive
+        integers (type is numpy.float32).
+
+        :param x: The matrix to validate
+
+        :rtype bool
+        :return True if any non-zero values are invalid given validation rules, False otherwise
+        """
+        data = x if isinstance(x, np.ndarray) else x.data
+        return np.any((data % 1 > 0) | (data < 0))
+
     def _validate_x_raw_x_dimensions(self):
         """
         Validates that X and raw.X have the same shape, if raw.X exists. Adds errors to self.errors if any.
         """
 
         if self._get_raw_x_loc() == "raw.X":
             if self.adata.n_vars != self.adata.raw.n_vars:
@@ -1278,14 +1453,418 @@
 
             # Do it for index that map to columns
             if "index" in component_def:
                 index_def = component_def["index"]
                 if "add_labels" in index_def:
                     self._check_single_column_availability(component, index_def["add_labels"])
 
+    def _check_spatial(self):
+        """
+        Sequence validation of spatial-related values of the AnnData object.
+
+        :rtype none
+        """
+        self._check_spatial_uns()
+        self._check_spatial_obs()
+
+    def _check_spatial_obs(self):
+        """
+        Validate obs spatial-related values of the AnnData object. Validation is not defined in schema definition yaml.
+        Errors are added to self.errors.
+
+        :rtype none
+        """
+
+        # Exit if obs is not specified. Error is reported in core validate functionality.
+        obs_component = getattr_anndata(self.adata, "obs")
+        if obs_component is None:
+            return
+
+        # Validate assay ontology term id.
+        self._validate_spatial_assay_ontology_term_id()
+
+        # Validate tissue positions.
+        self._validate_spatial_tissue_positions()
+
+        # Validate cell type.
+        self._validate_spatial_cell_type_ontology_term_id()
+
+        self._validate_spatial_is_primary_data()
+
+    def _validate_spatial_is_primary_data(self):
+        """
+        Validate is_primary_data for spatial datasets.
+        """
+        obs = getattr_anndata(self.adata, "obs")
+        if obs is None or "is_primary_data" not in obs:
+            return
+        if self._is_single() is False and obs["is_primary_data"].any():
+            self.errors.append(
+                "When uns['spatial']['is_single'] is False, obs['is_primary_data'] must be False for all rows."
+            )
+
+    def _validate_spatial_assay_ontology_term_id(self):
+        """
+        If assay is spatial, all assay ontology term ids should be identical.
+
+        :rtype none
+        """
+        # Identical check requires assay_ontology_term_id.
+        obs = getattr_anndata(self.adata, "obs")
+        if obs is None or "assay_ontology_term_id" not in obs:
+            return
+
+        # Identical check is only applicable to spatial datasets.
+        if not self._is_supported_spatial_assay():
+            return
+
+        # Validate assay ontology term ids are identical.
+        term_count = obs["assay_ontology_term_id"].nunique()
+        if term_count > 1:
+            self.errors.append(
+                "When obs['assay_ontology_term_id'] is either 'EFO:0010961' (Visium Spatial Gene Expression) or "
+                "'EFO:0030062' (Slide-seqV2), all observations must contain the same value."
+            )
+
+    def _validate_spatial_cell_type_ontology_term_id(self):
+        """
+        Validate cell type ontology term id is "unknown" if Visium, is_single is True and in_tissue is 0.
+
+        :rtype none
+        """
+        # Exit if:
+        # - not Visium and is_single is True as no further checks are necessary
+        # - in_tissue is not specified as checks are dependent on this value
+        if not self._is_visium_and_is_single_true() or "in_tissue" not in self.adata.obs:
+            return
+
+        # Validate cell type: must be "unknown" if Visium and is_single is True and in_tissue is 0.
+        if (
+            (self.adata.obs["assay_ontology_term_id"] == ASSAY_VISIUM)
+            & (self.adata.obs["in_tissue"] == 0)
+            & (self.adata.obs["cell_type_ontology_term_id"] != "unknown")
+        ).any():
+            self.errors.append(
+                f"obs['cell_type_ontology_term_id'] must be 'unknown' when {ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE_IN_TISSUE_0}."
+            )
+
+    def _validate_spatial_tissue_position(self, tissue_position_name: str, min: int, max: int):
+        """
+        Validate tissue position is allowed and required, and are integers within the given range. Validation is not defined in
+        schema definition yaml.
+
+        :rtype none
+        """
+        # Tissue position is foribidden if assay is not Visium and is_single is True.
+        if tissue_position_name in self.adata.obs and (
+            not self._is_visium_and_is_single_true()
+            or (
+                ~(self.adata.obs["assay_ontology_term_id"] == ASSAY_VISIUM)
+                & (self.adata.obs[tissue_position_name].notnull())
+            ).any()
+        ):
+            self.errors.append(f"obs['{tissue_position_name}'] {ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE_FORBIDDEN}.")
+            return
+
+        # Exit if we're not dealing with Visium and _is_single True as no further checks are necessary.
+        if not self._is_visium_and_is_single_true():
+            return
+
+        # At this point, is_single is True and:
+        # - there's at least one row with Visum, tissue position column is required
+        # - for any Visium row, tissue position is required.
+        if (
+            tissue_position_name not in self.adata.obs
+            or (
+                (self.adata.obs["assay_ontology_term_id"] == ASSAY_VISIUM)
+                & (self.adata.obs[tissue_position_name].isnull())
+            ).any()
+        ):
+            self.errors.append(f"obs['{tissue_position_name}'] {ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE_REQUIRED}.")
+            return
+
+        # Tissue position must be an int.
+        obs_tissue_position = self.adata.obs.get(tissue_position_name)
+        if not np.issubdtype(obs_tissue_position.dtype, np.integer):
+            self.errors.append(f"obs['{tissue_position_name}'] must be of int type, it is {obs_tissue_position.dtype}.")
+            return
+
+        # Tissue position must be within the given range.
+        if not ((obs_tissue_position >= min) & (obs_tissue_position <= max)).all():
+            if tissue_position_name == "in_tissue":
+                error_message_token = f"{min} or {max}"
+            else:
+                error_message_token = f"between {min} and {max}"
+            self.errors.append(
+                f"obs['{tissue_position_name}'] must be {error_message_token}, the min and max are {obs_tissue_position.min()} and {obs_tissue_position.max()}. "
+                f"This must be the value of the column tissue_positions_in_tissue from the tissue_positions_list.csv or tissue_positions.csv."
+            )
+
+    def _validate_spatial_tissue_positions(self):
+        """
+        Validate tissue positions of spatial datasets.
+
+        :rtype none
+        """
+        self._validate_spatial_tissue_position("array_col", 0, 127)
+        self._validate_spatial_tissue_position("array_row", 0, 77)
+        self._validate_spatial_tissue_position("in_tissue", 0, 1)
+
+    def _check_spatial_uns(self):
+        """
+        Validate uns spatial-related values of the AnnData object. Validation is not defined in schema definition yaml.
+        Errors are added to self.errors.
+
+        :rtype none
+        """
+
+        # Exit if uns is not specified. Error is reported in core validate functionality.
+        uns_component = getattr_anndata(self.adata, "uns")
+        if uns_component is None:
+            return
+
+        # uns spatial validation is dependent on obs.assay_ontology_term_id; exit if not specified. Error is
+        # reported in core validate functionality.
+        obs_component = getattr_anndata(self.adata, "obs")
+        if obs_component is None or "assay_ontology_term_id" not in obs_component:
+            return
+
+        # spatial is forbidden if assay it not a supported spatial assay.
+        uns_spatial = self.adata.uns.get("spatial")
+        is_supported_spatial_assay = self._is_supported_spatial_assay()
+        if uns_spatial is not None and not is_supported_spatial_assay:
+            self.errors.append(
+                "uns['spatial'] is only allowed for obs['assay_ontology_term_id'] values "
+                "'EFO:0010961' (Visium Spatial Gene Expression) and 'EFO:0030062' (Slide-seqV2)."
+            )
+            return
+
+        # Exit if we aren't dealing with a supported spatial assay as no further checks are necessary.
+        if not is_supported_spatial_assay:
+            return
+
+        # spatial is required for supported spatial assays.
+        if not isinstance(uns_spatial, dict):
+            self.errors.append(
+                "A dict in uns['spatial'] is required for obs['assay_ontology_term_id'] values "
+                "'EFO:0010961' (Visium Spatial Gene Expression) and 'EFO:0030062' (Slide-seqV2)."
+            )
+            return
+
+        # is_single is required.
+        if "is_single" not in uns_spatial:
+            self.errors.append("uns['spatial'] must contain the key 'is_single'.")
+            # Exit if is_single is missing as all further checks are dependent on its value.
+            return
+
+        # is_single must be a boolean.
+        uns_is_single = uns_spatial["is_single"]
+        if not isinstance(uns_is_single, (np.bool_, np.bool)):
+            self.errors.append(f"uns['spatial']['is_single'] must be of boolean type, it is {type(uns_is_single)}.")
+            # Exit if is_single is not valid as all further checks are dependent on its value.
+            return
+
+        # Check there is at most one library_id.
+        uns_spatial_keys = list(uns_spatial.keys())
+        library_ids = list(filter(lambda x: x != "is_single", uns_spatial_keys))
+        if len(library_ids) > 1:
+            self.errors.append(
+                "uns['spatial'] must contain only two top-level keys: 'is_single' and a library_id. "
+                f"More than two top-level keys detected: {library_ids}."
+            )
+            # Exit if there is more than one library_id as we don't know which library_id to validate.
+            return
+
+        # library_id is forbidden if assay is not Visium or is_single is false.
+        is_visium_and_uns_is_single = self._is_visium_and_is_single_true()
+        if len(library_ids) > 0 and not is_visium_and_uns_is_single:
+            self.errors.append(f"uns['spatial'][library_id] {ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE_FORBIDDEN}.")
+            # Exit as library_id is not allowed.
+            return
+
+        # Exit if we're not dealing with Visium and _is_single True as no further checks are necessary.
+        if not is_visium_and_uns_is_single:
+            return
+
+        # library_id is required if assay is Visium and is_single is True.
+        if len(library_ids) == 0:
+            self.errors.append(
+                f"uns['spatial'] must contain at least one key representing the library_id when {ERROR_SUFFIX_VISIUM_AND_IS_SINGLE_TRUE}."
+            )
+            # Exit as library_id is missing.
+            return
+
+        # Confirm shape of library_id is valid: allowed keys are images and scalefactors.
+        library_id_key = library_ids[0]
+        uns_library_id = uns_spatial[library_id_key]
+        if not isinstance(uns_library_id, dict):
+            self.errors.append("uns['spatial'][library_id] must be a dictionary.")
+            return
+        elif not self._has_no_extra_keys(uns_library_id, ["images", "scalefactors"]):
+            self.errors.append(
+                "uns['spatial'][library_id] can only contain the keys 'images' and 'scalefactors'."
+                f"Detected keys: {list(uns_library_id.keys())}."
+            )
+
+        # images is required.
+        if "images" not in uns_library_id:
+            self.errors.append("uns['spatial'][library_id] must contain the key 'images'.")
+        # images is specified: proceed with validation of images.
+        elif not isinstance(uns_library_id["images"], dict):
+            self.errors.append("uns['spatial'][library_id]['images'] must be a dictionary.")
+        else:
+            # Confirm shape of images is valid: allowed keys are fullres and hires.
+            uns_images = uns_library_id["images"]
+
+            if not self._has_no_extra_keys(uns_images, ["fullres", "hires"]):
+                self.errors.append(
+                    "uns['spatial'][library_id]['images'] can only contain the keys 'fullres' and 'hires'."
+                    f"Detected keys: {list(uns_images.keys())}."
+                )
+
+            # hires is required.
+            if "hires" not in uns_images:
+                self.errors.append("uns['spatial'][library_id]['images'] must contain the key 'hires'.")
+            # hires is specified: proceed with validation of hires.
+            else:
+                self._validate_spatial_image_shape("hires", uns_images["hires"], SPATIAL_HIRES_IMAGE_MAX_DIMENSION_SIZE)
+
+            # fullres is optional.
+            uns_fullres = uns_images.get("fullres")
+            if uns_fullres is None:
+                # Warn if no fullres is specified as it is strongly recommended.
+                self.warnings.append(
+                    "No uns['spatial'][library_id]['images']['fullres'] was found. "
+                    "It is STRONGLY RECOMMENDED that uns['spatial'][library_id]['images']['fullres'] is provided."
+                )
+            else:
+                self._validate_spatial_image_shape("fullres", uns_fullres)
+
+        # scalefactors is required.
+        if "scalefactors" not in uns_library_id:
+            self.errors.append("uns['spatial'][library_id] must contain the key 'scalefactors'.")
+        # scalefactors is specified: proceed with validation of scalefactors.
+        elif not isinstance(uns_library_id["scalefactors"], dict):
+            self.errors.append("uns['spatial'][library_id]['scalefactors'] must be a dictionary.")
+        else:
+            # Confirm shape of scalefactors is valid: allowed keys are spot_diameter_fullres and tissue_hires_scalef.
+            uns_scalefactors = uns_library_id["scalefactors"]
+            if not self._has_no_extra_keys(uns_scalefactors, ["spot_diameter_fullres", "tissue_hires_scalef"]):
+                self.errors.append(
+                    "uns['spatial'][library_id]['scalefactors'] can only contain the keys "
+                    "'spot_diameter_fullres' and 'tissue_hires_scalef'."
+                    f"Detected keys: {list(uns_scalefactors.keys())}."
+                )
+
+            # spot_diameter_fullres is required.
+            if "spot_diameter_fullres" not in uns_scalefactors:
+                self.errors.append(
+                    "uns['spatial'][library_id]['scalefactors'] must contain the key 'spot_diameter_fullres'."
+                )
+            # spot_diameter_fullres is specified: proceed with validation.
+            else:
+                spot_diameter_fullres = uns_scalefactors["spot_diameter_fullres"]
+                if not isinstance(spot_diameter_fullres, float):
+                    self.errors.append(
+                        "uns['spatial'][library_id]['scalefactors']['spot_diameter_fullres'] must be of type float, it is "
+                        f"{type(spot_diameter_fullres)}. This must be the value of the spot_diameter_fullres field from scalefactors_json.json"
+                    )
+
+            # tissue_hires_scalef is required.
+            if "tissue_hires_scalef" not in uns_scalefactors:
+                self.errors.append(
+                    "uns['spatial'][library_id]['scalefactors'] must contain the key 'tissue_hires_scalef'."
+                )
+            # tissue_hires_scalef is specified: proceed with validation.
+            else:
+                tissue_hires_scalef = uns_scalefactors["tissue_hires_scalef"]
+                if not isinstance(tissue_hires_scalef, float):
+                    self.errors.append(
+                        "uns['spatial'][library_id]['scalefactors']['tissue_hires_scalef'] must be of type float, it is "
+                        f"{type(tissue_hires_scalef)}. This must be the value of the tissue_hires_scalef field from scalefactors_json.json"
+                    )
+
+    def _has_no_extra_keys(self, dictionary: dict, allowed_keys: List[str]) -> bool:
+        """
+        Determine if the dictionary has only the given allowed keys. Keys can be missing (required
+        checks are executed separately) but no additional keys are allowed.
+
+        :param dict dictionary: the dictionary to check.
+        :param List[str] allowed_keys: the list of allowed keys.
+
+        :rtype bool
+        """
+        return set(dictionary.keys()).issubset(allowed_keys)
+
+    def _is_valid_visium_image_shape(self, image: np.ndarray) -> bool:
+        """
+        Determine if the image has shape (,,3 or 4); image is expected to be a 3D numpy array
+        with the size of the last dimension being three or four.
+
+        :param np.ndarray image: the image to check the shape of.
+
+        :return True if image has shape (,,3 or 4), False otherwise.
+        :rtype bool
+        """
+        return len(image.shape) == 3 and image.shape[2] in [3, 4]
+
+    def _is_visium(self) -> bool:
+        """
+        Determine if the assay_ontology_term_id is Visium (EFO:0010961).
+
+        :return True if assay_ontology_term_id is Visium, False otherwise.
+        :rtype bool
+        """
+        if self.is_visium is None:
+            assay_ontology_term_id = self.adata.obs.get("assay_ontology_term_id")
+            self.is_visium = assay_ontology_term_id is not None and (assay_ontology_term_id == ASSAY_VISIUM).any()
+        return self.is_visium
+
+    def _validate_spatial_image_shape(self, image_name: str, image: np.ndarray, max_dimension: int = None):
+        """
+        Validate the spatial image is of shape (,,3 or 4) and has a max dimension, if specified. A spatial image
+        is either spatial[library_id]['images']['hires'] or spatial[library_id]['images']['fullres']. Errors
+        are added to self.errors if any.
+
+        :param str image_name: the name of the image, either "hires" or "fullres".
+        :param np.ndarray image: the image to validate.
+        :param int max_dimension: the largest allowed dimension of the image, optional.
+
+        :rtype None
+        """
+        # Image must be an ndarray.
+        if not isinstance(image, np.ndarray):
+            self.errors.append(
+                f"uns['spatial'][library_id]['images']['{image_name}'] must be of numpy.ndarray type, "
+                f"it is {type(image)}."
+            )
+            return
+
+        # Confirm type of ndarray is uint8.
+        if image.dtype != np.uint8:
+            self.errors.append(
+                f"uns['spatial'][library_id]['images']['{image_name}'] must be of type numpy.uint8, "
+                f"it is {image.dtype}."
+            )
+
+        # Confirm shape of image is valid: allowed shape is (,,3 or 4).
+        if not self._is_valid_visium_image_shape(image):
+            self.errors.append(
+                f"uns['spatial'][library_id]['images']['{image_name}'] must have a length of 3 and "
+                "either 3 (RGB color model for example) or 4 (RGBA color model for example) for its last dimension, "
+                f"it has shape {image.shape}."
+            )
+
+        # Confirm max dimension of image, if specified, is valid.
+        if max_dimension is not None and max(image.shape) != max_dimension:
+            self.errors.append(
+                f"The largest dimension of uns['spatial'][library_id]['images']['{image_name}'] must be "
+                f"{max_dimension} pixels, it has a largest dimension of {max(image.shape)} pixels."
+            )
+
     def _deep_check(self):
         """
         Perform a "deep" check of the AnnData object using the schema definition. Adds errors to self.errors if any
 
         :rtype None
         """
         # Checks DataFrame column name uniqueness
@@ -1300,14 +1879,17 @@
         # Checks that reserved columns are not used
         self._check_column_availability()
 
         # Checks sparsity
         logger.debug("Validating sparsity...")
         self._validate_sparsity()
 
+        # Checks spatial
+        self._check_spatial()
+
         # Checks Seurat convertibility
         logger.debug("Validating Seurat convertibility...")
         self._validate_seurat_convertibility()
 
         # Checks each component
         for component_name, component_def in self.schema_def["components"].items():
             logger.debug(f"Validating component: {component_name}")
```

### Comparing `cellxgene-schema-5.0.2rc1/cellxgene_schema/write_labels.py` & `cellxgene-schema-5.0.3/cellxgene_schema/write_labels.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/PKG-INFO` & `cellxgene-schema-5.0.3/cellxgene_schema.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: cellxgene-schema
-Version: 5.0.2rc1
+Version: 5.0.3
 Summary: Tool for applying and validating cellxgene integration schema to single cell datasets
 Home-page: https://github.com/chanzuckerberg/single-cell-curation
 Author: Chan Zuckerberg Initiative
 Author-email: cellxgene@chanzuckerberg.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 License-File: LICENSE.txt
 
 Tool for applying and validating cellxgene integration schema to single cell datasets
-
```

### Comparing `cellxgene-schema-5.0.2rc1/setup.py` & `cellxgene-schema-5.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("requirements.txt") as fh:
     requirements = fh.read().splitlines()
 
 setup(
     name="cellxgene-schema",
-    version="5.0.2-rc.1",
+    version="5.0.3",
     url="https://github.com/chanzuckerberg/single-cell-curation",
     license="MIT",
     author="Chan Zuckerberg Initiative",
     author_email="cellxgene@chanzuckerberg.com",
     description="Tool for applying and validating cellxgene integration schema to single cell datasets",
     long_description="Tool for applying and validating cellxgene integration schema to single cell datasets",
     install_requires=requirements,
```

