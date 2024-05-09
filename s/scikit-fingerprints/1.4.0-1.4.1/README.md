# Comparing `tmp/scikit_fingerprints-1.4.0.tar.gz` & `tmp/scikit_fingerprints-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_fingerprints-1.4.0.tar", max compression
+gzip compressed data, was "scikit_fingerprints-1.4.1.tar", max compression
```

## Comparing `scikit_fingerprints-1.4.0.tar` & `scikit_fingerprints-1.4.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     1116 2024-05-04 20:40:05.660851 scikit_fingerprints-1.4.0/LICENSE.md
--rw-r--r--   0        0        0     3243 2024-05-04 20:40:05.660851 scikit_fingerprints-1.4.0/README.md
--rwxr-xr-x   0        0        0     1437 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/__init__.py
--rw-r--r--   0        0        0      170 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/bases/__init__.py
--rw-r--r--   0        0        0     6701 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/bases/base_fp_transformer.py
--rw-r--r--   0        0        0     1704 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/bases/base_preprocessor.py
--rw-r--r--   0        0        0     4439 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/bases/base_substructure_fp.py
--rw-r--r--   0        0        0     1268 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/__init__.py
--rw-r--r--   0        0        0     9801 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/atom_pair.py
--rw-r--r--   0        0        0     1535 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/autocorr.py
--rw-r--r--   0        0        0     4375 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/avalon.py
--rw-r--r--   0        0        0     8690 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/e3fp_fp.py
--rw-r--r--   0        0        0     3095 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/ecfp.py
--rw-r--r--   0        0        0     8229 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/erg.py
--rw-r--r--   0        0        0     1513 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/estate.py
--rw-r--r--   0        0        0     1439 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/getaway.py
--rw-r--r--   0        0        0     7279 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/ghose_crippen.py
--rw-r--r--   0        0        0   235066 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/klekota_roth.py
--rw-r--r--   0        0        0    28051 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/laggner.py
--rw-r--r--   0        0        0     2455 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/layered.py
--rw-r--r--   0        0        0     6344 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/lingo.py
--rw-r--r--   0        0        0     1091 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/maccs.py
--rw-r--r--   0        0        0     6806 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/map.py
--rw-r--r--   0        0        0     3115 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/mhfp.py
--rw-r--r--   0        0        0     1421 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/mordred_fp.py
--rw-r--r--   0        0        0     1069 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/morse.py
--rw-r--r--   0        0        0     1631 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/pattern.py
--rw-r--r--   0        0        0     2683 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/pharmacophore.py
--rw-r--r--   0        0        0     1785 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/physiochemical_properties.py
--rw-r--r--   0        0        0    41700 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/pubchem.py
--rw-r--r--   0        0        0     1061 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/rdf.py
--rw-r--r--   0        0        0     2898 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/rdk.py
--rw-r--r--   0        0        0     2751 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/secfp.py
--rw-r--r--   0        0        0     2194 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/topological_torsion.py
--rw-r--r--   0        0        0     7561 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/usr.py
--rw-r--r--   0        0        0     8145 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/usrcat.py
--rw-r--r--   0        0        0     1427 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/whim.py
--rw-r--r--   0        0        0     3787 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/parallel.py
--rw-r--r--   0        0        0      133 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/preprocessing/__init__.py
--rw-r--r--   0        0        0    14959 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/preprocessing/conformer_generator.py
--rw-r--r--   0        0        0     2494 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/preprocessing/mol_to_from_smiles.py
--rw-r--r--   0        0        0      243 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/rdkit_logging.py
--rw-r--r--   0        0        0     1118 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/validators.py
--rw-r--r--   0        0        0     4234 1970-01-01 00:00:00.000000 scikit_fingerprints-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1116 2024-05-09 17:44:16.016286 scikit_fingerprints-1.4.1/LICENSE.md
+-rw-r--r--   0        0        0     3243 2024-05-09 17:44:16.016286 scikit_fingerprints-1.4.1/README.md
+-rwxr-xr-x   0        0        0     1445 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/__init__.py
+-rw-r--r--   0        0        0      170 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/bases/__init__.py
+-rw-r--r--   0        0        0     6701 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/bases/base_fp_transformer.py
+-rw-r--r--   0        0        0     1704 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/bases/base_preprocessor.py
+-rw-r--r--   0        0        0     4439 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/bases/base_substructure_fp.py
+-rw-r--r--   0        0        0     1327 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/__init__.py
+-rw-r--r--   0        0        0     9788 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/atom_pair.py
+-rw-r--r--   0        0        0     1535 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/autocorr.py
+-rw-r--r--   0        0        0     4499 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/avalon.py
+-rw-r--r--   0        0        0     8677 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/e3fp_fp.py
+-rw-r--r--   0        0        0     3121 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/ecfp.py
+-rw-r--r--   0        0        0     8220 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/erg.py
+-rw-r--r--   0        0        0     1517 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/estate.py
+-rw-r--r--   0        0        0     7576 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/functional_groups.py
+-rw-r--r--   0        0        0     1457 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/getaway.py
+-rw-r--r--   0        0        0     7291 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/ghose_crippen.py
+-rw-r--r--   0        0        0   235078 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/klekota_roth.py
+-rw-r--r--   0        0        0    28063 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/laggner.py
+-rw-r--r--   0        0        0     2434 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/layered.py
+-rw-r--r--   0        0        0     6320 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/lingo.py
+-rw-r--r--   0        0        0     1095 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/maccs.py
+-rw-r--r--   0        0        0     6807 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/map.py
+-rw-r--r--   0        0        0     3092 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/mhfp.py
+-rw-r--r--   0        0        0     1425 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/mordred_fp.py
+-rw-r--r--   0        0        0     1069 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/morse.py
+-rw-r--r--   0        0        0     1653 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/pattern.py
+-rw-r--r--   0        0        0     2683 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/pharmacophore.py
+-rw-r--r--   0        0        0     1760 2024-05-09 17:44:16.020286 scikit_fingerprints-1.4.1/skfp/fingerprints/physiochemical_properties.py
+-rw-r--r--   0        0        0    41704 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/pubchem.py
+-rw-r--r--   0        0        0     1061 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/rdf.py
+-rw-r--r--   0        0        0     3002 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/rdk.py
+-rw-r--r--   0        0        0     2730 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/secfp.py
+-rw-r--r--   0        0        0     2341 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/topological_torsion.py
+-rw-r--r--   0        0        0     7561 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/usr.py
+-rw-r--r--   0        0        0     8145 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/usrcat.py
+-rw-r--r--   0        0        0     1445 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/fingerprints/whim.py
+-rw-r--r--   0        0        0     3787 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/parallel.py
+-rw-r--r--   0        0        0      133 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/preprocessing/__init__.py
+-rw-r--r--   0        0        0    15027 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/preprocessing/conformer_generator.py
+-rw-r--r--   0        0        0     2613 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/preprocessing/mol_to_from_smiles.py
+-rw-r--r--   0        0        0      243 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/rdkit_logging.py
+-rw-r--r--   0        0        0     1118 2024-05-09 17:44:16.024286 scikit_fingerprints-1.4.1/skfp/validators.py
+-rw-r--r--   0        0        0     4246 1970-01-01 00:00:00.000000 scikit_fingerprints-1.4.1/PKG-INFO
```

### Comparing `scikit_fingerprints-1.4.0/LICENSE.md` & `scikit_fingerprints-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/README.md` & `scikit_fingerprints-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/pyproject.toml` & `scikit_fingerprints-1.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scikit-fingerprints"
-version = "1.4.0"
+version = "1.4.1"
 description = "Library for effective molecular fingerprints calculation"
 authors = [
     "Scikit-Fingerprints Development Team <scikitfingerprints@gmail.com>",
     "Jakub Adamczyk <jakub.adamczyk10@gmail.com>",
     "Przemyslaw Kukla <przemek.kukla0703@gmail.com>",
     "Piotr Ludynia <piotrztych@gmail.com>",
     "Michal Szafarczyk <adammichal657@gmail.com>",
@@ -22,15 +22,15 @@
 
 datasketch = "*"
 e3fp = "*"
 joblib = "*"
 mordredcommunity = "*"
 numpy = "^1.20.0"
 pandas = "*"
-rdkit = "*"
+rdkit = "<2023.9.6"
 scikit-learn = "*"
 scipy = "*"
 tqdm = "*"
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `scikit_fingerprints-1.4.0/skfp/bases/base_fp_transformer.py` & `scikit_fingerprints-1.4.1/skfp/bases/base_fp_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/skfp/bases/base_preprocessor.py` & `scikit_fingerprints-1.4.1/skfp/bases/base_preprocessor.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/skfp/bases/base_substructure_fp.py` & `scikit_fingerprints-1.4.1/skfp/bases/base_substructure_fp.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/__init__.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .atom_pair import AtomPairFingerprint
 from .autocorr import AutocorrFingerprint
 from .avalon import AvalonFingerprint
 from .e3fp_fp import E3FPFingerprint
 from .ecfp import ECFPFingerprint
 from .erg import ERGFingerprint
 from .estate import EStateFingerprint
+from .functional_groups import FunctionalGroupsFingerprint
 from .getaway import GETAWAYFingerprint
 from .ghose_crippen import GhoseCrippenFingerprint
 from .klekota_roth import KlekotaRothFingerprint
 from .laggner import LaggnerFingerprint
 from .layered import LayeredFingerprint
 from .lingo import LingoFingerprint
 from .maccs import MACCSFingerprint
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/atom_pair.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/atom_pair.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from collections.abc import Sequence
 from numbers import Integral
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
-from sklearn.utils._param_validation import InvalidParameterError
+from sklearn.utils._param_validation import Interval, InvalidParameterError
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols, require_mols_with_conf_ids
 
 
 class AtomPairFingerprint(BaseFingerprintTransformer):
     """
@@ -132,17 +131,17 @@
     >>> smiles = ["O", "CC", "[C-]#N", "CC=O"]
     >>> fp = AtomPairFingerprint()
     >>> fp
     AtomPairFingerprint()
 
     >>> fp.transform(smiles)
     array([[0, 0, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0]], dtype=uint8)
+           [0, 0, 0, ..., 0, 0, 0],
+           [0, 0, 0, ..., 0, 0, 0],
+           [0, 0, 0, ..., 0, 0, 0]], dtype=uint8)
     """
 
     _parameter_constraints: dict = {
         **BaseFingerprintTransformer._parameter_constraints,
         "fp_size": [Interval(Integral, 1, None, closed="left")],
         "min_distance": [Interval(Integral, 1, None, closed="left")],
         "max_distance": [Interval(Integral, 1, None, closed="left")],
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/autocorr.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/autocorr.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/avalon.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/avalon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Sequence
 from numbers import Integral
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
+from sklearn.utils._param_validation import Interval
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
 class AvalonFingerprint(BaseFingerprintTransformer):
     """
@@ -18,15 +18,14 @@
     The implementation uses RDKit and Avalon Toolkit [1]_. This is a hashed fingerprint, where
     fragments are computed based on atom environments. The fingerprint is based on
     multiple features, including atom types, bond types, rings and paths. The detailed description
     can be found in the original paper [2]_.
 
     Parameters
     ----------
-
     fp_size : int, default=512
         Size of output vectors, i.e. number of bits for each fingerprint. Must be
         positive.
 
     count : bool, default=False
         Whether to return binary (bit) features, or their counts.
 
@@ -47,14 +46,17 @@
         Controls the verbosity when computing fingerprints.
 
     Attributes
     ----------
     n_features_out : int
         Number of output features. Equal to `fp_size`.
 
+    requires_conformers : bool = False
+        This fingerprint uses only 2D molecular graphs and does not require conformers.
+
     References
     ----------
     .. [1] Avalon toolkit
         https://sourceforge.net/projects/avalontoolkit/
     .. [2] `Gedeck, Peter, Bernhard Rohde, and Christian Bartels
         "QSAR − How Good Is It in Practice? Comparison of Descriptor Sets on an Unbiased
         Cross Section of Corporate Data Sets."
@@ -68,16 +70,14 @@
     >>> fp = AvalonFingerprint()
     >>> fp
     AvalonFingerprint()
     >>> X = fp.transform(smiles)
     >>> X
     array([[0, 0, 0, ..., 0, 0, 0],
            [0, 0, 0, ..., 0, 0, 0]])
-    >>> X.shape
-    (2, 512)
     """
 
     _parameter_constraints: dict = {
         **BaseFingerprintTransformer._parameter_constraints,
         "fp_size": [Interval(Integral, 1, None, closed="left")],
     }
 
@@ -125,17 +125,17 @@
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
         from rdkit.Avalon.pyAvalonTools import GetAvalonCountFP, GetAvalonFP
 
         X = ensure_mols(X)
 
         if self.count:
-            X = [GetAvalonCountFP(x, nBits=self.fp_size).ToList() for x in X]
+            X = [GetAvalonCountFP(mol, nBits=self.fp_size).ToList() for mol in X]
         else:
-            X = [GetAvalonFP(x, nBits=self.fp_size) for x in X]
+            X = [GetAvalonFP(mol, nBits=self.fp_size) for mol in X]
 
         dtype = np.uint32 if self.count else np.uint8
 
         if self.sparse:
             return csr_array(X, dtype=dtype)
         else:
             return np.array(X, dtype=dtype)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/e3fp_fp.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/e3fp_fp.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 import numpy as np
 import scipy.sparse
 from e3fp.conformer.generator import ConformerGenerator
 from e3fp.pipeline import fprints_from_mol
 from rdkit import RDLogger
 from rdkit.Chem import Mol, MolToSmiles
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
-from sklearn.utils._param_validation import InvalidParameterError
+from sklearn.utils._param_validation import Interval, InvalidParameterError
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import require_mols_with_conf_ids
 
 """
 Note: this file cannot have the "e3fp.py" name due to conflict with E3FP library.
 """
@@ -123,17 +122,17 @@
 
     >>> mol_from_smiles = MolFromSmilesTransformer()
     >>> mols = mol_from_smiles.transform(smiles)
     >>> conf_gen = ConformerGenerator()
     >>> mols = conf_gen.transform(mols)
     >>> fp.transform(mols)
     array([[0, 0, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0]], dtype=uint8)
+           [0, 0, 0, ..., 0, 0, 0],
+           [0, 0, 0, ..., 0, 0, 0],
+           [0, 0, 0, ..., 0, 0, 0]], dtype=uint8)
     """
 
     _parameter_constraints: dict = {
         **BaseFingerprintTransformer._parameter_constraints,
         "fp_size": [Interval(Integral, 1, None, closed="left")],
         "n_bits_before_folding": [Interval(Integral, 1, None, closed="left")],
         "level": [None, Interval(Integral, 1, None, closed="left")],
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/ecfp.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/ecfp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Sequence
 from numbers import Integral
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
+from sklearn.utils._param_validation import Interval
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
 class ECFPFingerprint(BaseFingerprintTransformer):
     """Extended Connectivity Fingerprint (ECFP) transformer."""
@@ -81,12 +81,12 @@
             includeRingMembership=self.include_ring_membership,
             countBounds=self.count_bounds,
             fpSize=self.fp_size,
             atomInvariantsGenerator=invgen,
         )
 
         if self.count:
-            X = [gen.GetCountFingerprintAsNumPy(x) for x in X]
+            X = [gen.GetCountFingerprintAsNumPy(mol) for mol in X]
         else:
-            X = [gen.GetFingerprintAsNumPy(x) for x in X]
+            X = [gen.GetFingerprintAsNumPy(mol) for mol in X]
 
         return csr_array(X) if self.sparse else np.array(X)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/erg.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/erg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from collections.abc import Sequence
 from numbers import Integral, Real
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
-from sklearn.utils._param_validation import InvalidParameterError, StrOptions
+from sklearn.utils._param_validation import Interval, InvalidParameterError, StrOptions
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
 class ERGFingerprint(BaseFingerprintTransformer):
     """
@@ -128,17 +127,17 @@
     >>> smiles = ["O", "CC", "[C-]#N", "CC=O"]
     >>> fp = ERGFingerprint()
     >>> fp
     ERGFingerprint()
 
     >>> fp.transform(smiles)
     array([[0., 0., 0., ..., 0., 0., 0.],
-       [0., 0., 0., ..., 0., 0., 0.],
-       [0., 0., 0., ..., 0., 0., 0.],
-       [0., 0., 0., ..., 0., 0., 0.]])
+           [0., 0., 0., ..., 0., 0., 0.],
+           [0., 0., 0., ..., 0., 0., 0.],
+           [0., 0., 0., ..., 0., 0., 0.]])
     """
 
     _parameter_constraints: dict = {
         **BaseFingerprintTransformer._parameter_constraints,
         "fuzz_increment": [Interval(Real, 0.0, None, closed="left")],
         "min_path": [Interval(Integral, 1, None, closed="left")],
         "max_path": [Interval(Integral, 1, None, closed="left")],
@@ -185,20 +184,20 @@
         X = ensure_mols(X)
 
         fuzz = self.fuzz_increment if self.variant == "fuzzy" else 0
 
         X = np.array(
             [
                 GetErGFingerprint(
-                    x,
+                    mol,
                     fuzzIncrement=fuzz,
                     minPath=self.min_path,
                     maxPath=self.max_path,
                 )
-                for x in X
+                for mol in X
             ]
         )
 
         if self.variant == "bit":
             X = X > 0
             dtype = np.uint8
         elif self.variant == "count":
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/estate.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/estate.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
         from rdkit.Chem.EState.Fingerprinter import FingerprintMol
 
         X = ensure_mols(X)
 
-        X = np.array([FingerprintMol(x) for x in X])
+        X = np.array([FingerprintMol(mol) for mol in X])
         if self.variant == "bit":
             X = (X[:, 0] > 0).astype(np.uint8)
         elif self.variant == "count":
             X = (X[:, 0]).astype(np.uint32)
         else:  # "sum" variant
             X = X[:, 1]
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/getaway.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/whim.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from collections.abc import Sequence
 from numbers import Real
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
+from sklearn.utils._param_validation import Interval
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import require_mols_with_conf_ids
 
 
-class GETAWAYFingerprint(BaseFingerprintTransformer):
-    """GETAWAY fingerprint."""
+class WHIMFingerprint(BaseFingerprintTransformer):
+    """WHIM fingerprint."""
 
     _parameter_constraints: dict = {
         **BaseFingerprintTransformer._parameter_constraints,
         "clip_val": [Interval(Real, 0, None, closed="left")],
     }
 
     def __init__(
@@ -24,23 +24,23 @@
         clip_val: int = np.iinfo(np.int32).max,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
         batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
         super().__init__(
-            n_features_out=273,
+            n_features_out=114,
             requires_conformers=True,
             sparse=sparse,
             n_jobs=n_jobs,
             batch_size=batch_size,
             verbose=verbose,
         )
         self.clip_val = clip_val
 
     def _calculate_fingerprint(self, X: Sequence[Mol]) -> Union[np.ndarray, csr_array]:
-        from rdkit.Chem.rdMolDescriptors import CalcGETAWAY
+        from rdkit.Chem.rdMolDescriptors import CalcWHIM
 
         X = require_mols_with_conf_ids(X)
-        X = [CalcGETAWAY(mol, confId=mol.GetIntProp("conf_id")) for mol in X]
+        X = [CalcWHIM(mol, confId=mol.GetIntProp("conf_id")) for mol in X]
         X = np.clip(X, -self.clip_val, self.clip_val)
         return csr_array(X) if self.sparse else np.array(X)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/ghose_crippen.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/ghose_crippen.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,17 +63,17 @@
     >>> smiles = ["O", "CC", "[C-]#N", "CC=O"]
     >>> fp = GhoseCrippenFingerprint()
     >>> fp
     GhoseCrippenFingerprint()
 
     >>> fp.transform(smiles)
     array([[0, 0, 0, ..., 0, 0, 0],
-       [0, 1, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0],
-       [0, 1, 0, ..., 0, 0, 0]], dtype=uint8)
+           [0, 1, 0, ..., 0, 0, 0],
+           [0, 0, 0, ..., 0, 0, 0],
+           [0, 1, 0, ..., 0, 0, 0]], dtype=uint8)
     """
 
     def __init__(
         self,
         count: bool = False,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/klekota_roth.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/klekota_roth.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,17 +52,17 @@
     >>> smiles = ["O", "CC", "[C-]#N", "CC=O"]
     >>> fp = KlekotaRothFingerprint()
     >>> fp
     KlekotaRothFingerprint()
 
     >>> fp.transform(smiles)
     array([[0, 0, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0]], dtype=uint8)
+           [0, 0, 0, ..., 0, 0, 0],
+           [0, 0, 0, ..., 0, 0, 0],
+           [0, 0, 0, ..., 0, 0, 0]], dtype=uint8)
     """
 
     def __init__(
         self,
         count: bool = False,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/laggner.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/laggner.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,17 +62,17 @@
     >>> smiles = ["O", "CC", "[C-]#N", "CC=O"]
     >>> fp = LaggnerFingerprint()
     >>> fp
     LaggnerFingerprint()
 
     >>> fp.transform(smiles)
     array([[0, 0, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0],
-       [0, 0, 0, ..., 0, 0, 0]], dtype=uint8)
+           [0, 0, 0, ..., 0, 0, 0],
+           [0, 0, 0, ..., 0, 0, 0],
+           [0, 0, 0, ..., 0, 0, 0]], dtype=uint8)
     """
 
     def __init__(
         self,
         count: bool = False,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/layered.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/layered.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from collections.abc import Sequence
 from numbers import Integral
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
-from sklearn.utils._param_validation import InvalidParameterError
+from sklearn.utils._param_validation import Interval, InvalidParameterError
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
 class LayeredFingerprint(BaseFingerprintTransformer):
     """Pattern fingerprint."""
@@ -59,20 +58,20 @@
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
         from rdkit.Chem.rdmolops import LayeredFingerprint as RDKitLayeredFingerprint
 
         X = ensure_mols(X)
         X = [
             RDKitLayeredFingerprint(
-                x,
+                mol,
                 fpSize=self.fp_size,
                 minPath=self.min_path,
                 maxPath=self.max_path,
                 branchedPaths=self.branched_paths,
             )
-            for x in X
+            for mol in X
         ]
 
         if self.sparse:
             return csr_array(X, dtype=np.uint8)
         else:
             return np.array(X, dtype=np.uint8)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/lingo.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/lingo.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections.abc import Sequence
 from numbers import Integral
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
+from sklearn.utils._param_validation import Interval
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_smiles
 
 
 class LingoFingerprint(BaseFingerprintTransformer):
     """
@@ -72,15 +72,15 @@
     >>> from skfp.fingerprints import LingoFingerprint
     >>> smiles = ["[C-]#N", "CC(=O)NC1=CC=C(C=C1)O"]
     >>> fp = LingoFingerprint()
     >>> fp
     LingoFingerprint()
     >>> fp.transform(smiles)
     array([[0, 0, 0, ..., 0, 0, 0],
-       [0, 1, 0, ..., 0, 0, 0]], dtype=uint8)
+           [0, 1, 0, ..., 0, 0, 0]], dtype=uint8)
     """
 
     _parameter_constraints: dict = {
         **BaseFingerprintTransformer._parameter_constraints,
         "fp_size": [Interval(Integral, 1, None, closed="left")],
         "substring_length": [Interval(Integral, 1, None, closed="left")],
         "count": ["boolean"],
@@ -139,26 +139,26 @@
 
         Returns
         -------
         result: list[dict[str, int]]
             List of dictionaries containing substring counts.
         """
         X = ensure_smiles(X)
-        # we are doing this according to the original paper
-        # which aimed for reducing the number of possible substrings
-        # and improving statistical sampling in the QSPR models.
-        X = [re.sub(r"[123456789]", "0", x) for x in X]
-        X = [re.sub(r"Cl", "L", x) for x in X]
-        X = [re.sub(r"Br", "R", x) for x in X]
+
+        # based on the original paper, we reduce the number of possible substrings
+        # to improve statistical sampling in the QSPR models
+        X = [re.sub(r"[123456789]", "0", smi) for smi in X]
+        X = [re.sub(r"Cl", "L", smi) for smi in X]
+        X = [re.sub(r"Br", "R", smi) for smi in X]
 
         result = []
-        for smiles in X:
+        for smi in X:
             result_dict: defaultdict[str, int] = defaultdict(int)
-            for i in range(len(smiles) - self.substring_length + 1):
-                result_dict[smiles[i : i + self.substring_length]] += 1
+            for i in range(len(smi) - self.substring_length + 1):
+                result_dict[smi[i : i + self.substring_length]] += 1
             result.append(dict(result_dict))
 
         return result
 
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/maccs.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/maccs.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,13 +29,13 @@
 
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
         from rdkit.Chem.rdMolDescriptors import GetMACCSKeysFingerprint
 
         X = ensure_mols(X)
-        X = [GetMACCSKeysFingerprint(x) for x in X]
+        X = [GetMACCSKeysFingerprint(mol) for mol in X]
 
         if self.sparse:
             return csr_array(X, dtype=np.uint8)
         else:
             return np.array(X, dtype=np.uint8)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/map.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 
 import numpy as np
 from datasketch import MinHash
 from rdkit.Chem import MolToSmiles, PathToSubmol
 from rdkit.Chem.rdchem import Mol
 from rdkit.Chem.rdmolops import FindAtomEnvironmentOfRadiusN, GetDistanceMatrix
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
-from sklearn.utils._param_validation import StrOptions
+from sklearn.utils._param_validation import Interval, StrOptions
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 """
 Code inspired by the original work of the authors of the MAP4 Fingerprint:
 https://github.com/reymond-group/map4
@@ -59,15 +58,17 @@
         self.radius = radius
         self.variant = variant
 
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
         X = ensure_mols(X)
-        X = np.stack([self._calculate_single_mol_fingerprint(x) for x in X], dtype=int)
+        X = np.stack(
+            [self._calculate_single_mol_fingerprint(mol) for mol in X], dtype=int
+        )
 
         if self.variant == "bit":
             X = (X > 0).astype(np.uint8)
         elif self.variant == "count":
             X = X.astype(np.uint32)
 
         return csr_array(X) if self.sparse else np.array(X)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/mhfp.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/mhfp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from collections.abc import Sequence
 from numbers import Integral
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
-from sklearn.utils._param_validation import InvalidParameterError, StrOptions
+from sklearn.utils._param_validation import Interval, InvalidParameterError, StrOptions
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
 class MHFPFingerprint(BaseFingerprintTransformer):
     """MinHashed FingerPrint (MHFP) transformer."""
@@ -82,14 +81,14 @@
             isomeric=self.isomeric,
             kekulize=self.kekulize,
         )
         X = np.array(X, dtype=np.uint32)
 
         if self.variant in {"bit", "count"}:
             X = np.mod(X, self.fp_size)
-            X = np.stack([np.bincount(x, minlength=self.fp_size) for x in X])
+            X = np.stack([np.bincount(fp, minlength=self.fp_size) for fp in X])
             if self.variant == "bit":
                 X = (X > 0).astype(np.uint8)
             else:
                 X = X.astype(np.uint32)
 
         return csr_array(X) if self.sparse else np.array(X)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/mordred_fp.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/mordred_fp.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,14 @@
 
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
         X = ensure_mols(X)
 
         calc = Calculator(descriptors, ignore_3D=not self.use_3D)
-        X = [calc(x) for x in X]
+        X = [calc(mol) for mol in X]
 
         return (
             csr_array(X, dtype=np.float32)
             if self.sparse
             else np.array(X, dtype=np.float32)
         )
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/morse.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/morse.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/pattern.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/pattern.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Sequence
 from numbers import Integral
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
+from sklearn.utils._param_validation import Interval
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
 class PatternFingerprint(BaseFingerprintTransformer):
     """Pattern fingerprint."""
@@ -43,16 +43,16 @@
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
         from rdkit.Chem.rdmolops import PatternFingerprint as RDKitPatternFingerprint
 
         X = ensure_mols(X)
         X = [
             RDKitPatternFingerprint(
-                x, fpSize=self.fp_size, tautomerFingerprints=self.tautomers
+                mol, fpSize=self.fp_size, tautomerFingerprints=self.tautomers
             )
-            for x in X
+            for mol in X
         ]
 
         if self.sparse:
             return csr_array(X, dtype=np.uint8)
         else:
             return np.array(X, dtype=np.uint8)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/pharmacophore.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/pharmacophore.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/physiochemical_properties.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/physiochemical_properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from collections.abc import Sequence
 from numbers import Integral
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
-from sklearn.utils._param_validation import StrOptions
+from sklearn.utils._param_validation import Interval, StrOptions
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
 class PhysiochemicalPropertiesFingerprint(BaseFingerprintTransformer):
     """Physiochemical properties fingerprint."""
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/pubchem.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/pubchem.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         )
 
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
         X = ensure_mols(X)
 
-        X = [self._get_pubchem_fingerprint(x) for x in X]
+        X = [self._get_pubchem_fingerprint(mol) for mol in X]
         return csr_array(X) if self.sparse else np.vstack(X)
 
     def _get_pubchem_fingerprint(self, mol: Mol) -> Union[np.ndarray, csr_array]:
         # PubChem's definition requires hydrogens to be present
         mol = AddHs(mol)
 
         atom_counts = self._get_atom_counts(mol)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/rdf.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/rdf.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/rdk.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/rdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from collections.abc import Sequence
 from numbers import Integral
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
-from sklearn.utils._param_validation import InvalidParameterError
+from sklearn.utils._param_validation import Interval, InvalidParameterError
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
 class RDKitFingerprint(BaseFingerprintTransformer):
     """RDKit fingerprint."""
@@ -77,12 +76,16 @@
             useBondOrder=self.use_bond_order,
             countSimulation=self.count,
             fpSize=self.fp_size,
             numBitsPerFeature=self.num_bits_per_feature,
         )
 
         if self.count:
-            X = [gen.GetCountFingerprintAsNumPy(x) for x in X]
+            X = [gen.GetCountFingerprintAsNumPy(mol) for mol in X]
         else:
-            X = [gen.GetFingerprintAsNumPy(x) for x in X]
+            X = [gen.GetFingerprintAsNumPy(mol) for mol in X]
 
-        return csr_array(X) if self.sparse else np.array(X)
+        dtype = np.uint32 if self.count else np.uint8
+        if self.sparse:
+            return csr_array(X, dtype=dtype)
+        else:
+            return np.array(X, dtype=dtype)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/secfp.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/secfp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from collections.abc import Sequence
 from numbers import Integral
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
-from sklearn.utils._param_validation import InvalidParameterError
+from sklearn.utils._param_validation import Interval, InvalidParameterError
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
 class SECFPFingerprint(BaseFingerprintTransformer):
     """SECFP fingerprint."""
@@ -68,22 +67,22 @@
 
         X = ensure_mols(X)
 
         # bulk function does not work
         encoder = MHFPEncoder(self.fp_size, self.random_state)
         X = [
             encoder.EncodeSECFPMol(
-                x,
+                mol,
                 length=self.fp_size,
                 radius=self.radius,
                 min_radius=self.min_radius,
                 rings=self.rings,
                 isomeric=self.isomeric,
                 kekulize=self.kekulize,
             )
-            for x in X
+            for mol in X
         ]
 
         if self.sparse:
             return csr_array(X, dtype=np.uint8)
         else:
             return np.array(X, dtype=np.uint8)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/topological_torsion.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/topological_torsion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Sequence
 from numbers import Integral
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
+from sklearn.utils._param_validation import Interval
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
 class TopologicalTorsionFingerprint(BaseFingerprintTransformer):
     """Topological torsion fingerprint."""
@@ -58,12 +58,16 @@
             includeChirality=self.include_chirality,
             torsionAtomCount=self.torsion_atom_count,
             countSimulation=self.count_simulation,
             fpSize=self.fp_size,
         )
 
         if self.count:
-            X = [gen.GetCountFingerprintAsNumPy(x) for x in X]
+            X = [gen.GetCountFingerprintAsNumPy(mol) for mol in X]
         else:
-            X = [gen.GetFingerprintAsNumPy(x) for x in X]
+            X = [gen.GetFingerprintAsNumPy(mol) for mol in X]
 
-        return csr_array(X) if self.sparse else np.array(X)
+        dtype = np.uint32 if self.count else np.uint8
+        if self.sparse:
+            return csr_array(X, dtype=dtype)
+        else:
+            return np.array(X, dtype=dtype)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/usr.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/usr.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/usrcat.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/usrcat.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/skfp/fingerprints/whim.py` & `scikit_fingerprints-1.4.1/skfp/fingerprints/getaway.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from collections.abc import Sequence
 from numbers import Real
 from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
-from sklearn.utils import Interval
+from sklearn.utils._param_validation import Interval
 
 from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import require_mols_with_conf_ids
 
 
-class WHIMFingerprint(BaseFingerprintTransformer):
-    """WHIM fingerprint."""
+class GETAWAYFingerprint(BaseFingerprintTransformer):
+    """GETAWAY fingerprint."""
 
     _parameter_constraints: dict = {
         **BaseFingerprintTransformer._parameter_constraints,
         "clip_val": [Interval(Real, 0, None, closed="left")],
     }
 
     def __init__(
@@ -24,23 +24,23 @@
         clip_val: int = np.iinfo(np.int32).max,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
         batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
         super().__init__(
-            n_features_out=114,
+            n_features_out=273,
             requires_conformers=True,
             sparse=sparse,
             n_jobs=n_jobs,
             batch_size=batch_size,
             verbose=verbose,
         )
         self.clip_val = clip_val
 
     def _calculate_fingerprint(self, X: Sequence[Mol]) -> Union[np.ndarray, csr_array]:
-        from rdkit.Chem.rdMolDescriptors import CalcWHIM
+        from rdkit.Chem.rdMolDescriptors import CalcGETAWAY
 
         X = require_mols_with_conf_ids(X)
-        X = [CalcWHIM(mol, confId=mol.GetIntProp("conf_id")) for mol in X]
+        X = [CalcGETAWAY(mol, confId=mol.GetIntProp("conf_id")) for mol in X]
         X = np.clip(X, -self.clip_val, self.clip_val)
         return csr_array(X) if self.sparse else np.array(X)
```

### Comparing `scikit_fingerprints-1.4.0/skfp/parallel.py` & `scikit_fingerprints-1.4.1/skfp/parallel.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/skfp/preprocessing/conformer_generator.py` & `scikit_fingerprints-1.4.1/skfp/preprocessing/conformer_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 )
 from rdkit.ForceField import ForceField
 from sklearn.utils import Interval
 from sklearn.utils._param_validation import InvalidParameterError, StrOptions
 
 from skfp.bases import BasePreprocessor
 from skfp.parallel import run_in_parallel
+from skfp.validators import ensure_mols
 
 
 class ConformerGenerator(BasePreprocessor):
     """
     Generate molecule conformer.
 
     The implementation uses RDKit and distance geometry (DG) approach [1], with
@@ -244,14 +245,16 @@
     ) -> tuple[list[PropertyMol], np.ndarray]:
         self._validate_params()
 
         if copy:
             X = deepcopy(X)
             y = deepcopy(y)
 
+        X = ensure_mols(X)
+
         n_jobs = effective_n_jobs(self.n_jobs)
         if n_jobs == 1:
             mols = self._embed_molecules(X)
         else:
             mols = run_in_parallel(
                 self._embed_molecules,
                 data=X,
```

### Comparing `scikit_fingerprints-1.4.0/skfp/preprocessing/mol_to_from_smiles.py` & `scikit_fingerprints-1.4.1/skfp/preprocessing/mol_to_from_smiles.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections.abc import Sequence
 from numbers import Integral
 from typing import Optional
 
 from rdkit.Chem import Mol, MolFromSmiles, MolToSmiles
 
 from skfp.bases import BasePreprocessor
+from skfp.validators import ensure_mols, ensure_smiles
 
 
 class MolFromSmilesTransformer(BasePreprocessor):
     _parameter_constraints: dict = {
         "sanitize": ["boolean"],
         "replacements": [dict, None],
     }
@@ -20,18 +21,19 @@
     ):
         self.sanitize = sanitize
         self.replacements = replacements
 
     def transform(self, X: Sequence[str], copy: bool = False) -> list[Mol]:
         # no parallelization, too fast to benefit from it
         self._validate_params()
+        X = ensure_smiles(X)
         replacements = self.replacements if self.replacements else {}
         return [
-            MolFromSmiles(x, sanitize=self.sanitize, replacements=replacements)
-            for x in X
+            MolFromSmiles(smi, sanitize=self.sanitize, replacements=replacements)
+            for smi in X
         ]
 
 
 class MolToSmilesTransformer(BasePreprocessor):
     _parameter_constraints: dict = {
         "isomeric_smiles": ["boolean"],
         "kekule_smiles": ["boolean"],
@@ -59,20 +61,21 @@
         self.all_bonds_explicit = all_bonds_explicit
         self.all_hs_explicit = all_hs_explicit
         self.do_random = do_random
 
     def transform(self, X: Sequence[Mol], copy: bool = False) -> list[str]:
         # no parallelization, too fast to benefit from it
         self._validate_params()
+        X = ensure_mols(X)
         return [
             MolToSmiles(
-                x,
+                mol,
                 isomericSmiles=self.isomeric_smiles,
                 kekuleSmiles=self.kekule_smiles,
                 rootedAtAtom=self.rooted_at_atom,
                 canonical=self.canonical,
                 allBondsExplicit=self.all_bonds_explicit,
                 allHsExplicit=self.all_hs_explicit,
                 doRandom=self.do_random,
             )
-            for x in X
+            for mol in X
         ]
```

### Comparing `scikit_fingerprints-1.4.0/skfp/validators.py` & `scikit_fingerprints-1.4.1/skfp/validators.py`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.4.0/PKG-INFO` & `scikit_fingerprints-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-fingerprints
-Version: 1.4.0
+Version: 1.4.1
 Summary: Library for effective molecular fingerprints calculation
 Home-page: https://github.com/Arch4ngel21/scikit-fingerprints
 License: MIT
 Author: Scikit-Fingerprints Development Team
 Author-email: scikitfingerprints@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: datasketch
 Requires-Dist: e3fp
 Requires-Dist: joblib
 Requires-Dist: mordredcommunity
 Requires-Dist: numpy (>=1.20.0,<2.0.0)
 Requires-Dist: pandas
-Requires-Dist: rdkit
+Requires-Dist: rdkit (<2023.9.6)
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Project-URL: Repository, https://github.com/Arch4ngel21/scikit-fingerprints
 Description-Content-Type: text/markdown
 
 # scikit-fingerprints
```

