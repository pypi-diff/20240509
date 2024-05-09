# Comparing `tmp/qmatchatea-0.5.2.tar.gz` & `tmp/qmatchatea-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qmatchatea-0.5.2.tar", last modified: Tue Jan 16 18:26:15 2024, max compression
+gzip compressed data, was "qmatchatea-1.1.0.tar", last modified: Thu May  9 14:54:47 2024, max compression
```

## Comparing `qmatchatea-0.5.2.tar` & `qmatchatea-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-01-16 18:26:15.729473 qmatchatea-0.5.2/
--rw-r--r--   0 quantum    (128) quantum    (128)    10764 2022-12-06 17:46:42.000000 qmatchatea-0.5.2/LICENSE
--rw-r--r--   0 quantum    (128) quantum    (128)      891 2024-01-16 18:25:16.000000 qmatchatea-0.5.2/NOTICE
--rw-r--r--   0 quantum    (128) quantum    (128)     3246 2024-01-16 18:26:15.729473 qmatchatea-0.5.2/PKG-INFO
--rw-r--r--   0 quantum    (128) quantum    (128)     2549 2024-01-16 18:25:16.000000 qmatchatea-0.5.2/README.md
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-01-16 18:26:15.729473 qmatchatea-0.5.2/qmatchatea/
--rw-r--r--   0 quantum    (128) quantum    (128)      933 2022-12-06 17:46:42.000000 qmatchatea-0.5.2/qmatchatea/__init__.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-01-16 18:26:15.729473 qmatchatea-0.5.2/qmatchatea/circuit/
--rw-r--r--   0 quantum    (128) quantum    (128)      640 2022-12-06 17:46:42.000000 qmatchatea-0.5.2/qmatchatea/circuit/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    46551 2022-12-06 17:46:42.000000 qmatchatea-0.5.2/qmatchatea/circuit/circuit.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13174 2023-10-23 14:25:03.000000 qmatchatea-0.5.2/qmatchatea/circuit/observables.py
--rw-r--r--   0 quantum    (128) quantum    (128)    18735 2023-10-23 14:25:03.000000 qmatchatea-0.5.2/qmatchatea/circuit/operations.py
--rw-r--r--   0 quantum    (128) quantum    (128)    20306 2023-10-23 14:25:03.000000 qmatchatea-0.5.2/qmatchatea/interface.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5455 2023-04-03 09:52:51.000000 qmatchatea-0.5.2/qmatchatea/mpi_utils.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7508 2023-10-23 14:25:03.000000 qmatchatea-0.5.2/qmatchatea/par_simulations.py
--rw-r--r--   0 quantum    (128) quantum    (128)    20008 2023-10-23 14:25:03.000000 qmatchatea-0.5.2/qmatchatea/preprocessing.py
--rw-r--r--   0 quantum    (128) quantum    (128)    31836 2024-01-16 18:25:16.000000 qmatchatea-0.5.2/qmatchatea/py_emulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5853 2023-02-10 14:24:45.000000 qmatchatea-0.5.2/qmatchatea/qk_utils.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6496 2022-12-06 17:46:42.000000 qmatchatea-0.5.2/qmatchatea/sf_utils.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7945 2023-10-23 14:25:03.000000 qmatchatea-0.5.2/qmatchatea/tensor_compiler.py
--rw-r--r--   0 quantum    (128) quantum    (128)     8617 2023-04-03 09:52:51.000000 qmatchatea-0.5.2/qmatchatea/tn_utils.py
--rw-r--r--   0 quantum    (128) quantum    (128)    34554 2024-01-16 18:25:16.000000 qmatchatea-0.5.2/qmatchatea/utils.py
--rw-r--r--   0 quantum    (128) quantum    (128)      500 2024-01-16 18:25:16.000000 qmatchatea-0.5.2/qmatchatea/version.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-01-16 18:26:15.729473 qmatchatea-0.5.2/qmatchatea.egg-info/
--rw-r--r--   0 quantum    (128) quantum    (128)     3246 2024-01-16 18:26:15.000000 qmatchatea-0.5.2/qmatchatea.egg-info/PKG-INFO
--rw-r--r--   0 quantum    (128) quantum    (128)      829 2024-01-16 18:26:15.000000 qmatchatea-0.5.2/qmatchatea.egg-info/SOURCES.txt
--rw-r--r--   0 quantum    (128) quantum    (128)        1 2024-01-16 18:26:15.000000 qmatchatea-0.5.2/qmatchatea.egg-info/dependency_links.txt
--rw-r--r--   0 quantum    (128) quantum    (128)      100 2024-01-16 18:26:15.000000 qmatchatea-0.5.2/qmatchatea.egg-info/requires.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       11 2024-01-16 18:26:15.000000 qmatchatea-0.5.2/qmatchatea.egg-info/top_level.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       38 2024-01-16 18:26:15.729473 qmatchatea-0.5.2/setup.cfg
--rw-r--r--   0 quantum    (128) quantum    (128)     2425 2024-01-16 18:25:16.000000 qmatchatea-0.5.2/setup.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-01-16 18:26:15.729473 qmatchatea-0.5.2/tests/
--rw-r--r--   0 quantum    (128) quantum    (128)     2381 2023-10-23 14:25:03.000000 qmatchatea-0.5.2/tests/test_examples.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9821 2023-10-23 14:25:03.000000 qmatchatea-0.5.2/tests/test_qcircuit.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2512 2022-12-06 17:46:42.000000 qmatchatea-0.5.2/tests/test_tensor_compiler.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6564 2023-10-23 14:25:03.000000 qmatchatea-0.5.2/tests/tests_basic_circuits.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1379 2022-12-06 17:46:42.000000 qmatchatea-0.5.2/tests/tests_formatting.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9066 2023-10-23 14:25:03.000000 qmatchatea-0.5.2/tests/tests_linter.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1508 2022-12-06 17:46:42.000000 qmatchatea-0.5.2/tests/tests_mpi4py.py
--rw-r--r--   0 quantum    (128) quantum    (128)    10606 2023-10-23 14:25:03.000000 qmatchatea-0.5.2/tests/tests_observables.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 14:54:47.718386 qmatchatea-1.1.0/
+-rw-r--r--   0 quantum    (128) quantum    (128)    10764 2022-12-06 17:46:42.000000 qmatchatea-1.1.0/LICENSE
+-rw-r--r--   0 quantum    (128) quantum    (128)      891 2024-01-16 18:26:28.000000 qmatchatea-1.1.0/NOTICE
+-rw-r--r--   0 quantum    (128) quantum    (128)     3238 2024-05-09 14:54:47.714386 qmatchatea-1.1.0/PKG-INFO
+-rw-r--r--   0 quantum    (128) quantum    (128)     2549 2024-01-16 18:26:28.000000 qmatchatea-1.1.0/README.md
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 14:54:47.714386 qmatchatea-1.1.0/qmatchatea/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1084 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/__init__.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 14:54:47.714386 qmatchatea-1.1.0/qmatchatea/circuit/
+-rw-r--r--   0 quantum    (128) quantum    (128)      640 2022-12-06 17:46:42.000000 qmatchatea-1.1.0/qmatchatea/circuit/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    47446 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/circuit/circuit.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13179 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/circuit/observables.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    19048 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/circuit/operations.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    16545 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/interface.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7469 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/par_simulations.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    20020 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/preprocessing.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    33472 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/py_emulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7951 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/tensor_compiler.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 14:54:47.714386 qmatchatea-1.1.0/qmatchatea/utils/
+-rw-r--r--   0 quantum    (128) quantum    (128)      645 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     8166 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/mpi_utils.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7085 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/qk_utils.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6496 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/sf_utils.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    15538 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/simulation_results.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     8653 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/tn_utils.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    30231 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/utils.py
+-rw-r--r--   0 quantum    (128) quantum    (128)      500 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/version.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 14:54:47.714386 qmatchatea-1.1.0/qmatchatea.egg-info/
+-rw-r--r--   0 quantum    (128) quantum    (128)     3238 2024-05-09 14:54:47.000000 qmatchatea-1.1.0/qmatchatea.egg-info/PKG-INFO
+-rw-r--r--   0 quantum    (128) quantum    (128)      930 2024-05-09 14:54:47.000000 qmatchatea-1.1.0/qmatchatea.egg-info/SOURCES.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)        1 2024-05-09 14:54:47.000000 qmatchatea-1.1.0/qmatchatea.egg-info/dependency_links.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       92 2024-05-09 14:54:47.000000 qmatchatea-1.1.0/qmatchatea.egg-info/requires.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       11 2024-05-09 14:54:47.000000 qmatchatea-1.1.0/qmatchatea.egg-info/top_level.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       38 2024-05-09 14:54:47.718386 qmatchatea-1.1.0/setup.cfg
+-rw-r--r--   0 quantum    (128) quantum    (128)     2485 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/setup.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 14:54:47.714386 qmatchatea-1.1.0/tests/
+-rw-r--r--   0 quantum    (128) quantum    (128)     7191 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_basic_circuits.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    11887 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_examples.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1379 2022-12-06 17:46:42.000000 qmatchatea-1.1.0/tests/tests_formatting.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9540 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_linter.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     3297 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_mpi4py.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    10753 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_observables.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    10441 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_qcircuit.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2978 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_tensor_compiler.py
```

### Comparing `qmatchatea-0.5.2/LICENSE` & `qmatchatea-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qmatchatea-0.5.2/NOTICE` & `qmatchatea-1.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `qmatchatea-0.5.2/PKG-INFO` & `qmatchatea-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: qmatchatea
-Version: 0.5.2
+Version: 1.1.0
 Summary: Quantum matcha TEA python library for tensor network emulation of quantum circuits.
 Home-page: https://baltig.infn.it/quantum_matcha_tea/py_api_quantum_matcha_tea
 Author: Marco Ballarin
 Author-email: marco97.ballarin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: matplotlib>=3.1.3
-Requires-Dist: qtealeaves<0.5.0,>=0.4.54
+Requires-Dist: qtealeaves>=1.1.4
 Requires-Dist: qiskit==0.38.0
 Requires-Dist: mpi4py
 Requires-Dist: joblib
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
```

### Comparing `qmatchatea-0.5.2/README.md` & `qmatchatea-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `qmatchatea-0.5.2/qmatchatea/__init__.py` & `qmatchatea-1.1.0/qmatchatea/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,25 +10,33 @@
 
 """
 Module init
 """
 
 __all__ = [
     "utils",
-    "tn_utils",
     "preprocessing",
     "interface",
     "par_simulations",
     "circuit",
+    "utils",
     "tensor_compiler",
     "__version__",
 ]
-from qmatchatea.utils import *
-from qmatchatea.tn_utils import *
 from qmatchatea.preprocessing import *
 from qmatchatea.tensor_compiler import *
 from qmatchatea.interface import *
 from qmatchatea.par_simulations import *
+from qmatchatea.utils.simulation_results import SimulationResults
 
 from qmatchatea import circuit
+from qmatchatea import utils
+
+from qmatchatea.utils import (
+    QCBackend,
+    QCCheckpoints,
+    QCConvergenceParameters,
+    QCIO,
+    QCOperators,
+)
 
 from qmatchatea.version import __version__
```

### Comparing `qmatchatea-0.5.2/qmatchatea/circuit/__init__.py` & `qmatchatea-1.1.0/qmatchatea/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-0.5.2/qmatchatea/circuit/circuit.py` & `qmatchatea-1.1.0/qmatchatea/circuit/circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,26 +49,26 @@
 """
 
 from copy import deepcopy
 import numpy as np
 import scipy.sparse as sp
 from qiskit import QuantumCircuit
 
+from qmatchatea.utils.tn_utils import QCOperators
+
 # Operations
 from .operations import QCOperation, ClassicalCondition, QCRemoveSite, QCAddSite
 from .operations import QCRenormalize
 from .observables import QCObservableStep
 
 # Gates
 from .operations import QCMeasureProjective, QCZpauli, QCXpauli, QCYpauli, QCHadamard
 from .operations import QCSgate, QCTgate, QCSadggate, QCTadggate, QCPgate
 from .operations import QCSwap, QCCnot, QCCz, QCCp
 
-from ..tn_utils import QCOperators
-
 __all__ = ["Qcircuit"]
 
 
 class Qcircuit:
     """
     Class used to represent a quantum circuit in
     the qmatchatea library.
@@ -178,14 +178,19 @@
 
     @property
     def num_sites(self):
         """Number of sites property"""
         return self._num_sites
 
     @property
+    def num_qubits(self):
+        """Number of sites property, with another name for simplicity of interfaces"""
+        return self._num_sites
+
+    @property
     def local_dim(self):
         """Local dimension property"""
         return self._local_dim
 
     @property
     def num_layers(self):
         """Number of layers in the circuit"""
@@ -417,14 +422,15 @@
         num_reps = len(self._qregisters[register])
         for _ in range(num_reps):
             self.remove_site(register, 0)
 
         # Remove the key from the dictionary
         del self._qregisters[register]
 
+    # pylint: disable-next=too-many-branches
     def add(self, operation, sites, register="default"):
         """
         Add an operation to the circuit
 
         Parameters
         ----------
         operation : :class:`QCOperation`
@@ -437,14 +443,17 @@
         """
         if not issubclass(type(operation), QCOperation):
             raise TypeError(
                 f"operation must be of type QCOperation, not {type(operation)}"
             )
         if isinstance(sites, int):  # Trasnsfor integer in array-like list
             sites = [sites]
+            self._num_one_site_operations += 1
+        else:
+            self._num_two_site_operations += 1
         if isinstance(register, str):
             register = [register] * len(sites)
 
         if register is not None:
             for idx, site in enumerate(sites):
                 sites[idx] = self._qregisters[register[idx]][site]
 
@@ -732,14 +741,15 @@
                 if max(sites) < self.num_sites - 1:
                     op_mat = kron(op_mat, iden(2 ** (self.num_sites - max(sites) - 1)))
 
                 matrix = op_mat @ matrix
 
         return matrix
 
+    # pylint: disable-next=too-many-locals
     def str_repr(self):
         """
         Get the string representation of the circuit
         """
 
         # Initialization
         str_repr = []
@@ -748,24 +758,35 @@
             str_idx = f"q_{idx} "
             str_idx += " " * (biggest_idx_len - len(str_idx))
             void = " " * biggest_idx_len
 
             str_repr.append([void, str_idx, void])
 
         for layer in self._data:
+            used_sites = []
+            max_len = 0
             for instruction in layer:
                 op_str = instruction[0].string_rep.split("\n")
                 sites = instruction[1]
+                used_sites += list(sites)
 
                 for idx, site in enumerate(sites):
                     current_str = op_str[idx * 3 : (idx + 1) * 3]
+                    if len(current_str) == 0:
+                        current_str = op_str[:3]
 
                     for idx_str, str1 in enumerate(current_str):
                         str_repr[site][idx_str] += str1
+                        max_len = max(max_len, len(str1))
 
+            empty_idxs = np.setdiff1d(np.arange(self.num_sites), np.array(used_sites))
+            for site in empty_idxs:
+                str_repr[site][0] += " " * max_len
+                str_repr[site][1] += "─" * max_len
+                str_repr[site][2] += " " * max_len
         circ_rep = ""
         for site in str_repr:
             circ_rep += "\n".join(site)
 
         return circ_rep
 
     ################################################################
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qmatchatea-0.5.2/qmatchatea/circuit/observables.py` & `qmatchatea-1.1.0/qmatchatea/circuit/observables.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 It also handles the indexing of quantum registers and observables.
 """
 from copy import deepcopy
 import numpy as np
 from qtealeaves.observables import TNObservables
 
-from qmatchatea.tn_utils import QCOperators
+from qmatchatea.utils.tn_utils import QCOperators
 from .operations import QCOperation, ClassicalCondition
 
 
 class QCObservableStep(QCOperation):
     """
     Perform a measurement of the observables TNObservables.
     The observables are applied on the **WHOLE** circuit,
@@ -274,15 +274,14 @@
                 key = np.array2string(key[indexing].astype(int), separator=sep)
                 key = key.replace("[", "").replace("]", "")
 
                 if key in new_measures[qreg_key]:
                     new_measures[qreg_key][key] += value
                 else:
                     new_measures[qreg_key][key] = value
-
         projective.results_buffer["projective_measurements"] = new_measures
 
         return projective
 
     def _postprocess_probabilities(self, probabilities):
         """
         Postprocess probability measurements. In input,
```

### Comparing `qmatchatea-0.5.2/qmatchatea/circuit/operations.py` & `qmatchatea-1.1.0/qmatchatea/circuit/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,14 +394,24 @@
     def operator(self):
         """
         Overwriting operator with cz
         """
         cz_op = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, -1]])
         return cz_op
 
+    @property
+    def string_rep(self):
+        """Return the string representation for printing"""
+        str_rep = f"─ {self.name} ─"
+        void = " " * len(str_rep)
+        string = void + "\n" + str_rep + "\n" + void + "\n"
+        string += void + "\n" + str_rep + "\n" + void
+
+        return string
+
 
 class QCHadamard(QCOperation):
     """
     Hadamard operation.
      Its matrix representation is as follows:
 
     .. math::
```

### Comparing `qmatchatea-0.5.2/qmatchatea/interface.py` & `qmatchatea-1.1.0/qmatchatea/interface.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,19 +35,14 @@
 - Using the Fortran backend (``mpi_approach='SR'``). It is the faster implementation, but requires
   the presence of the executable ``main_qmatchatea.exe``.
 - Using the Python backend (``backend='PY'``). The backend is entirely built with numpy, it
   is optimized but slightly slower than the fortran backend.
 - Using the Python GPU backend (``backend='PY'``, ``device='gpu'``).
   The backend is entirely built with cupy,
   and runs the simulation on a GPU, giving back the results on the CPU.
-- Using the Python Fortran backend (``approach='PF'``). This backend uses the Python backend
-  but simulates the same I/O files of the fortran one. It can be used as an initial debugging
-  backend in the case the I/O fortran files are used in a more general setting. Furthermore,
-  the strawberry-fields interface is not available for the ``'PY'`` approach, but is available
-  here. Finally, it is very useful for developers.
 
 Parallel program
 ~~~~~~~~~~~~~~~~
 
 There are three possible algorithm provided to run the program on multiple cores:
 
 - a Master/Worker approach (``mpi_approach='MW'``), where you store the state in the master
@@ -64,30 +59,14 @@
 number of processes you will use. It should be given as input to the :class:`IO_INFO`.
 For further details on the input class see :doc:`utils`.
 
 Remember that there are communications involved in the MPI parallel program.
 You should use it only if your system is large enough or if the bond
 dimension used is big enough.
 
-Changing the approach at runtime with command line arguments
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-When you write a python script with a specific approach, it is possible to change that
-approach at runtime, using optional arguments. The following optional arguments are
-available:
-
-- ``--approach``: it should be a ``str``, and if it is present, it overwrites the script approach.
-  This means that, if in your ``my_script.py`` you selected the approach ``PF`` but you run on the
-  command line ``python my_script.py --approach='SR'``, the :func:`run_simulation` will use the
-  approach ``'SR'``.
-- ``--mpi``: it should be an ``int``. It represent the number of cores that should be used in the
-  simulation. If ``--approach`` is absent, it overwrites the script approach to ``'CT'``, and then
-  sets the number of cores to the numeric value passed. It automatically changes the PATH of the
-  executable to the parallel path.
-
 Checking the convergence: Singular values cut
 ---------------------------------------------
 
 The singular values cut are an indication of the approximation taking place during the
 simulation. Indeed, at each application of two-qubit there is an approximation going on,
 subject to the *bond_dim* :math:`\\chi` and the *cut_ratio* :math:`\\epsilon` parameters.
 Based on the *trunc_tracking_mode* the singular values are reported:
@@ -114,52 +93,59 @@
 # Numpy
 import os
 import os.path
 from typing import OrderedDict
 import subprocess
 import sys
 import pickle
-import argparse
 
 import numpy as np
 from qtealeaves import write_nml
 from qtealeaves.observables import TNObservables
 
-from qmatchatea.py_emulator import mock_fortran, run_py_simulation
+from qmatchatea.py_emulator import run_py_simulation
+from qmatchatea.circuit import Qcircuit
 from .preprocessing import pre_parser, preprocess
-from .tn_utils import QCOperators, read_nml
-from .mpi_utils import to_layered_circ
-from .qk_utils import qk_transpilation_params
-from .utils import QCCheckpoints, QCIO, QCConvergenceParameters, merge_ordered_dicts
-from .utils import simulation_results, EXE_PATH, QCBackend
+from .utils.tn_utils import QCOperators, read_nml
+from .utils.mpi_utils import to_layered_circ
+from .utils.qk_utils import qk_transpilation_params
+from .utils.utils import (
+    QCCheckpoints,
+    QCIO,
+    QCConvergenceParameters,
+    merge_ordered_dicts,
+    QCBackend,
+)
+from .utils.simulation_results import SimulationResults
 
-__all__ = ["run_simulation", "simulation_results", "restart_from_checkpoint"]
+__all__ = ["run_simulation", "SimulationResults", "restart_from_checkpoint"]
 
 
 def run_simulation(
     circ,
     local_dim=2,
     convergence_parameters=QCConvergenceParameters(),
     operators=QCOperators(),
     io_info=QCIO(),
     observables=TNObservables(),
     transpilation_parameters=qk_transpilation_params(),
     checkpoints=QCCheckpoints(),
     where_barriers=-1,
     backend=QCBackend(),
-    cmd_args=None,
 ):
     """
     Transpile the circuit to adapt it to the linear structure of the MPS and run the circuit,
     obtaining in output the measurements.
 
     Parameters
     ----------
-    circ: QuantumCircuit or strawberryfields.Program
-        qiskit quantum circuit object to simulate
+    circ: QuantumCircuit | strawberryfields.Program | Qcircuit
+        Quantum circuit object to simulate.
+        Be careful, if one passes a Qcircuit **no check** is done on the quantum circuit, i.e.
+        it is not linearized and no barriers are added automatically.
     local_dim: int, optional
         Local dimension of the single degree of freedom. Default is 2, for qubits
     convergence_parameters: :py:class:`QCConvergenceParameters`, optional
         Maximum bond dimension and cut ratio. Default to max_bond_dim=10, cut_ratio=1e-9.
     operators: :py:class:`QCOperators`, optional
         Operator class with the observables operators ALREADY THERE. If None, then it is
         initialized empty. Default to None.
@@ -175,21 +161,18 @@
     where_barriers: int, optional
         This parameter is important only if you want to use MPI parallelization.
         If where_barriers > 0 then the circuit gets ordered in layers and a barrier is applyed
         each where_barriers layers. We recall that a barrier is equivalent to a canonization in
         the MPS simulation. Default to -1.
     backend: :py:class:`QCBackend`, optional
         Backend containing all the information for where to run the simulation
-    cmd_args: list of strings, optional
-        Allows controlling the arguments parsed by argparse within qmatchatea.
-        Default to `None` which retrieves arguments from sys.argv
 
     Returns
     -------
-    result: qmatchatea.simulation_results
+    result: qmatchatea.SimulationResults
         Results of the simulation, containing the following data:
         - Measures
         - Statevector
         - Computational time
         - Singular values cut
         - Entanglement
         - Measure probabilities
@@ -197,99 +180,88 @@
         - Observables measurements
     """
     # Checks on input parameters
     if not isinstance(convergence_parameters, QCConvergenceParameters):
         raise TypeError(
             "convergence_parameters must be of type QCConvergenceParameters"
         )
-    elif not isinstance(operators, QCOperators):
+    if not isinstance(operators, QCOperators):
         raise TypeError("operators must be of type QCOperators")
-    elif not isinstance(io_info, QCIO):
+    if not isinstance(io_info, QCIO):
         raise TypeError("io_info must be of type QCIO")
-    elif not isinstance(observables, TNObservables):
+    if not isinstance(observables, TNObservables):
         raise TypeError("observables must be of type TNObservables")
-    elif not isinstance(transpilation_parameters, qk_transpilation_params):
+    if not isinstance(transpilation_parameters, qk_transpilation_params):
         raise TypeError(
             "transpilation_parameters must be of type qk_transpilation_params"
         )
-    elif not isinstance(checkpoints, QCCheckpoints):
+    if not isinstance(checkpoints, QCCheckpoints):
         raise TypeError("checkpoints must be of type QCCheckpoints")
-    elif not isinstance(backend, QCBackend):
+    if not isinstance(backend, QCBackend):
         raise TypeError("backend must be of type QCBackend")
 
-    # Checks on command line arguments that MIGHT modify the script
-    io_info, backend, where_barriers = _parse_and_modify(
-        cmd_args, io_info, backend, where_barriers
-    )
-
-    # If the approach is pure python, do not go through all the steps for
-    # the usual simulation setting
-    if backend.backend == "PY":
-        return run_py_simulation(
-            circ,
-            local_dim,
-            convergence_parameters,
-            operators,
-            observables,
-            transpilation_parameters=transpilation_parameters,
-            backend=backend,
-            initial_state=io_info.initial_state,
-        )
-
     # Ensure observables output folders is present and set IO
-    io_info.setup()
+    io_info.setup(backend.backend == "FR")
+
     if backend.num_procs > 1:
-        new_exe = ["mpiexec", "-n", str(backend.num_procs), *io_info.exe_file]
+        new_exe = backend.mpi_command + [
+            "-n",
+            str(backend.num_procs),
+            *io_info.exe_file,
+        ]
         io_info.set_exe_file(new_exe)
-    if not os.path.isdir(os.path.join(io_info.outPATH, observables.folder_observables)):
-        os.makedirs(os.path.join(io_info.outPATH, observables.folder_observables))
 
     # Set the PATH to the saved files into the output folder
     for ii in range(len(observables.obs_list["TNState2File"])):
         if "/" not in observables.obs_list["TNState2File"].name[ii]:
             observables.obs_list["TNState2File"].name[ii] = os.path.join(
                 io_info.outPATH, observables.obs_list["TNState2File"].name[ii]
             )
 
     # Checks for parallel implementation
     if backend.mpi_approach not in ("SR", "PF"):
-        if io_info.exe_cmd[0] == EXE_PATH:
-            raise RuntimeError("Selected parallel approach using serial executable")
         if where_barriers <= 0:
             raise ValueError(
                 "To obtain a correct result in a parallel approach the \
                 where_barriers parameters must be greater then 0"
             )
         if backend.mpi_approach == "MW":
             if where_barriers != 1:
                 raise ValueError(
                     "To obtain a correct result with the MW approach \
                     where_barrier must be 1."
                 )
+    if isinstance(circ, Qcircuit):
+        preprocessed_circ = circ
+        if backend.backend == "FR":
+            raise ValueError("Qcircuit simulations not implemented in fortran")
+    else:
+        # Preprocess the circuit to adapt it to the MPS constraints (linearity)
+        preprocessed_circ = preprocess(circ, qk_params=transpilation_parameters)
 
-    # Preprocess the circuit to adapt it to the MPS constraints (linearity)
-    preprocessed_circ = preprocess(circ, qk_params=transpilation_parameters)
+        # If required order the circuit in a layered way and apply barriers
+        if where_barriers > 0:
+            preprocessed_circ = to_layered_circ(
+                preprocessed_circ, where_barriers=where_barriers
+            )
 
-    # If required order the circuit in a layered way and apply barriers
-    if where_barriers > 0:
-        preprocessed_circ = to_layered_circ(
-            preprocessed_circ, where_barriers=where_barriers
+    if backend.backend == "PY":
+        circ_str = preprocessed_circ
+        n_sites = preprocessed_circ.num_qubits
+    else:
+        # Write the circuit on file
+        n_sites, operator_mapping, circ_str = pre_parser(
+            preprocessed_circ,
+            operators,
+            io_info.inPATH,
+            fock_cutoff=local_dim,
+            sparse=io_info.sparse,
         )
-
-    # Write the circuit on file
-    n_sites, operator_mapping, circ_str = pre_parser(
-        preprocessed_circ,
-        operators,
-        io_info.inPATH,
-        fock_cutoff=local_dim,
-        sparse=io_info.sparse,
-    )
-
-    # Write the observables on file
-    observables.write(io_info.inPATH, {}, operator_mapping)
+        # Write the observables on file
+        observables.write(io_info.inPATH, {}, operator_mapping)
 
     # Prepare input dictionary
     input_dict = OrderedDict()
     input_dict["num_sites"] = n_sites
     input_dict["local_dim"] = local_dim
     input_dict["observables_filename"] = os.path.join(observables.filename_observables)
 
@@ -310,29 +282,44 @@
     # Save input parameters on namelist file
     write_nml("INPUT", input_dict, os.path.join(io_info.inPATH, io_info.input_namelist))
 
     # Setting checkpoints if required
     if checkpoints.frequency > 0:
         checkpoints.set_up(input_dict, operators, observables, circ_str)
 
-    # Run the fortran program with the namelist name as argument
-    if backend.mpi_approach == "PF":
-        res = mock_fortran(io_info.exe_cmd, observables, operator_mapping)
+    # If the approach is pure python, do not go through all the steps for
+    # the usual simulation setting
+    if backend.backend == "PY":
+        # Write all the information of the simulation as json
+        to_write = [convergence_parameters, backend, io_info, checkpoints]
+        for cls_to_write in to_write:
+            cls_to_write.to_json(io_info.inPATH)
+        result = run_py_simulation(
+            preprocessed_circ,
+            local_dim,
+            convergence_parameters,
+            operators,
+            observables,
+            backend=backend,
+            initial_state=io_info.initial_state,
+            checkpoints=checkpoints,
+        )
     else:
+        # Run the fortran program with the namelist name as argument
         res = subprocess.run(io_info.exe_file, capture_output=True)
         if res.stderr:
             print("--------------------------------------------")
             print("Program terminated with the following error:")
             print(res.stderr.decode())
             print("--------------------------------------------")
             sys.exit(1)
-    result = simulation_results(input_dict, observables)
+        result = SimulationResults(input_dict, observables)
 
-    # Retrieve results
-    result._get_results()
+        # Retrieve results
+        result._get_results()
 
     return result
 
 
 def restart_from_checkpoint(io_info, checkpoint_number=-1):
     """
     Restart a simulation starting from a checkpoint. Remember not to move checkpoints around,
@@ -354,15 +341,15 @@
         of the simulation, starting from that checkpoint, will be saved.
     checkpoint_number: int
         Number of the directory you want to restart from. If `-1` restart from the last one.
         Default to -1.
 
     Returns
     -------
-    result: qmatchatea.simulation_results
+    result: qmatchatea.SimulationResults
         Results of the simulation
     """
     if not isinstance(io_info, QCIO):
         raise TypeError("io_info must be of type QCIO")
 
     PATH = io_info.inPATH
     if not os.path.isdir(PATH):
@@ -414,83 +401,13 @@
     res = subprocess.run(io_info.exe_file, capture_output=True)
     if res.stderr:
         print("--------------------------------------------")
         print("Program terminated with the following error:")
         print(res.stderr.decode())
         print("--------------------------------------------")
         sys.exit(1)
-    result = simulation_results(input_dict, observables)
+    result = SimulationResults(input_dict, observables)
 
     # Retrieve results
     result._get_results()
 
     return result
-
-
-def _parse_and_modify(cmd_args, io_info, backend, where_barriers):
-    """
-    Parse command line input and modify at runtime the change of approach.
-    If the --approach command line argument is present, it overwrites the script approach.
-    If --approach is absent, but --mpi is present, the script approach is overwritten to 'CT'
-
-    Parameters
-    ----------
-    cmd_args: list of strings or `None`
-        Allows controlling the arguments parsed by argparse within qmatchatea.
-        Passing `None` retrieves arguments from sys.argv
-    io_info : :class: QCIO
-        Input information. The executable path might be modified
-    approach : QCBackend
-        Approach of the simulation. If command lines are present might be modified
-    where_barriers : int
-        Where to put barriers in the parallel approach. If it is -1 and the command
-        line arguments are present, it is modified to 1.
-
-    Returns
-    -------
-    :class: QCIO
-        New io information
-    str
-        New approach
-    where_barriers
-        New number of barriers
-    """
-    parser = argparse.ArgumentParser(
-        prog="qmatchatea parser",
-        description="Change the behavior of your script at runtime",
-    )
-    parser.add_argument(
-        "--mpi",
-        help="Number of cores to be used. Set the approach to"
-        + "'CT' if not otherwise stated",
-    )
-    parser.add_argument(
-        "--approach", help="Modify at runtime the approach used in the simulation"
-    )
-
-    # Dummy argument for running in jupyter
-    parser.add_argument("-f")
-    args, _ = parser.parse_known_args(cmd_args)
-
-    # If approach is present, overwrite the script approach
-    if args.approach:
-        approach = args.approach
-        backend._mpi_approach = approach
-        # Set the correct file if approach is serial
-        if approach == "SR":
-            new_exe = [EXE_PATH]
-            io_info.set_exe_file(new_exe)
-    # If approach is absent and mpi is present, approach becomes 'CT'
-    elif args.mpi:
-        backend._mpi_approach = "CT"
-
-    # If mpi is present we modify the io info to add the parallel run
-    if args.mpi:
-        backend._num_procs = int(args.mpi)
-        new_exe = "mpirun -np " + str(args.mpi) + " " + EXE_PATH
-        io_info.set_exe_file(new_exe.split())
-
-    # Modify where_barriers if any argument is present and where_barriers is -1
-    if (args.approach or args.mpi) and where_barriers == -1:
-        where_barriers = 1
-
-    return io_info, backend, where_barriers
```

### Comparing `qmatchatea-0.5.2/qmatchatea/mpi_utils.py` & `qmatchatea-1.1.0/qmatchatea/utils/mpi_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,15 +32,85 @@
     # This try except makes the code compatible also with the latest version of
     # qiskit, where the _get_layered_instructions changed path
     from qiskit.visualization.circuit._utils import _get_layered_instructions
 from qiskit import QuantumCircuit
 import numpy as np
 from .sf_utils import Barrier
 
-__all__ = ["to_layered_circ"]
+__all__ = ["MPISettings", "to_layered_circ"]
+
+
+class MPISettings:
+    """
+    Settings for using the library on multiple processes using MPI.
+    The default settings use no MPI, i.e. a serial execution of the algorithm.
+
+    Parameters
+    ----------
+    mpi_approach: str, optional
+        Approach for the MPI simulation.
+        Available:
+        - "SR": serial, the algorithm is run serially on the TN ansatz
+        - "CT": cartesian, the MPS is divided between different processes,
+                and the algorithm is done in parallel. MPS ONLY.
+        - "MW": master-worker. The MPS is stored ona single process (the master)
+                but the operations are done on the worker processes. It requires
+                a lot of communications. FORTRAN ONLY, MPS ONLY.
+        Default to "SR".
+    isometrization: int | List[int], optional
+        How to perform the isometrization.
+        - `-1` is a serial isometrization step
+        - A `int` is a parallel isometrization step with that number of layers
+        - A `List[int]` is a parallel isometrization step where each entry is
+          the number of layers for the `i`-th isometrization. If the number of
+          isometrization steps is greater than the length of the array, the array
+          is repeated.
+        Default to `-1`
+    num_procs: int, optional, FORTRAN ONLY
+        Number of processes for the MPI simulation. Default to 1.
+    mpi_command : List[str], optional, FORTRAN ONLY
+        MPI command that should be called when launching MPI from fortran.
+        The "-n" for the number of processes is already taken into account.
+        Default to ["mpi_exec"].
+    """
+
+    def __init__(
+        self, mpi_approach="SR", isometrization=-1, num_procs=1, mpi_command=None
+    ):
+        self.num_procs = num_procs
+        self.mpi_approach = mpi_approach.upper()
+        self.isometrization = isometrization
+        if mpi_command is None:
+            mpi_command = ["mpiexec"]
+        self.mpi_command = list(mpi_command)
+
+    def __getitem__(self, idx):
+        """
+        Get the settings of the isometrization for the idx-th isometrization
+        """
+        if np.isscalar(self.isometrization):
+            return self.isometrization
+
+        return self.isometrization[idx % len(self.isometrization)]
+
+    def print_isometrization_type(self, idx):
+        """
+        print which type of isometrization we have at index idx
+
+        Parameters
+        ----------
+        idx : int
+            Index of the isometrization
+        """
+
+        iso_type = self[idx]
+        if iso_type < 0:
+            print(f"At step {idx} serial isometrization")
+        else:
+            print(f"At step {idx} parallel isometrization with {iso_type} layers")
 
 
 def _to_layered_circ_qk(qc, where_barriers=1):
     """
     Transform a quantum circuit in another, where the instruction are ordered by layers.
     Apply a barrier every where_barriers layers.
```

### Comparing `qmatchatea-0.5.2/qmatchatea/par_simulations.py` & `qmatchatea-1.1.0/qmatchatea/par_simulations.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 import os
 import os.path
 from typing import OrderedDict
 import inspect
 from shutil import rmtree
 
 from qmatchatea.utils import QCIO
-from .interface import run_simulation, simulation_results
+from .interface import run_simulation, SimulationResults
 
 __all__ = ["run_parallel_simulations", "MASTER"]
 
 FREETAG = 0  # Tag to say that the workers are free
 WORKTAG = 1  # Tag to send the working parameters to the workers
 DIETAG = 2  # Tag to break the MW communications
 
@@ -61,15 +61,15 @@
     MPI: MPI module
         MPI module to perform the MPI calls
 
     Returns
     -------
     results : OrderedDict
         Ordered dict where the key is the simulation ID and the value the corresponding
-        :py:class:`simulation_results`
+        :py:class:`SimulationResults`
 
     Raises
     ------
     TypeError
         If the input parameters are not an ordered dict
     """
     if not isinstance(params, OrderedDict):
@@ -95,15 +95,15 @@
 def _master(params, MPI):
     comm = MPI.COMM_WORLD
     results = OrderedDict()
     requests = []
     for ID, sim_param in zip(params.keys(), params.values()):
         print(f"**** Done ID={ID} *****")
         # Initialize results
-        # results[ID] = simulation_results()
+        # results[ID] = SimulationResults()
 
         # Check which process is free
         free_process = comm.recv(buf=None, source=MPI.ANY_SOURCE, tag=FREETAG)
 
         # Send the data to the worker
         comm.send(obj=sim_param, dest=free_process, tag=WORKTAG)
         comm.send(obj=ID, dest=free_process, tag=WORKTAG)
@@ -112,16 +112,15 @@
         req = comm.irecv(buf=None, source=free_process, tag=WORKTAG)
         requests.append(req)
     print("----- Finished circuits -----")
 
     # When you finished wait for all the results
     for simID, req in zip(params.keys(), requests):
         path = req.wait()
-        results[simID] = simulation_results()
-        results[simID].load_results(path)
+        results[simID] = SimulationResults.read_pickle(path)
 
     # Send the DIETAG to the workers
     for ii in range(comm.Get_size()):
         if ii == MASTER:
             continue
         comm.send(obj=None, dest=ii, tag=DIETAG)
 
@@ -142,17 +141,17 @@
             break
 
         # Perform the simulation
         simID = comm.recv(buf=None, source=MASTER, tag=WORKTAG)
         simulation_parameters = _check_parameters(simulation_parameters, rank)
         results = run_simulation(*simulation_parameters)
 
-        results.save_results("TMP_MPI", name=simID)
-
-        path = os.path.join("TMP_MPI", simID + "_" + results.date_time)
+        # Save the results
+        path = os.path.join("TMP_MPI", f"{simID}.pkl")
+        results.save_pickle(path)
         # Send back the results
         comm.send(obj=path, dest=MASTER, tag=WORKTAG)
 
         # Send the I'm FREE message to the MASTER
         comm.send(obj=rank, dest=MASTER, tag=FREETAG)
 
     return
```

### Comparing `qmatchatea-0.5.2/qmatchatea/preprocessing.py` & `qmatchatea-1.1.0/qmatchatea/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 
 import os
 import os.path
 import warnings
 from qiskit import QuantumCircuit, transpile, transpiler
 import numpy as np
 from qtealeaves import StrBuffer
-from .sf_utils import optical_gates
-from .qk_utils import get_index, qk_transpilation_params
+from .utils.sf_utils import optical_gates
+from .utils.qk_utils import get_index, qk_transpilation_params
 from .tensor_compiler import tensor_compiler
 
 try:
     from strawberryfields import Program
 
     SF_IS_IMPORTED = True
 except ModuleNotFoundError:
```

### Comparing `qmatchatea-0.5.2/qmatchatea/py_emulator.py` & `qmatchatea-1.1.0/qmatchatea/py_emulator.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,91 +17,92 @@
 by using the :py:class:`QCEmulator` class.
 
 Functions and classes
 ~~~~~~~~~~~~~~~~~~~~~
 
 """
 
-import os
+# pylint: disable=protected-access
+
 import time
-from warnings import warn
 from copy import deepcopy
+import warnings
+import os
 
+import psutil
 import numpy as np
 from qiskit import QuantumCircuit
-from qtealeaves import read_tensor
 from qtealeaves.convergence_parameters import TNConvergenceParameters
-from qtealeaves.emulator import MPS, TTN, _AbstractTN
+from qtealeaves.emulator import MPS, TTN, MPIMPS, _AbstractTN
+from qtealeaves.mpos import DenseMPO
 from qtealeaves.observables import TNObservables
-
-# Try to import cupy
-try:
-    import cupy as cp
-    from cupy_backends.cuda.api.runtime import CUDARuntimeError
-
-    try:
-        _ = cp.cuda.Device()
-        GPU_AVAILABLE = True
-    except CUDARuntimeError:
-        GPU_AVAILABLE = False
-except ImportError:
-    cp = None
-    GPU_AVAILABLE = False
+from qtealeaves.tensors import TensorBackend
+from qtealeaves.emulator.tn_simulation import run_tn_measurements, AVAIL_DTYPES
 
 from .circuit import Qcircuit
 from .circuit.observables import QCObservableStep
-from .preprocessing import preprocess
-from .tn_utils import read_nml, QCOperators, write_tensor
-from .qk_utils import qk_transpilation_params
-from .utils import QCIO, QCConvergenceParameters, simulation_results
-from .utils import QCBackend
+from .utils.tn_utils import QCOperators
+from .utils.utils import QCConvergenceParameters, QCBackend, QCCheckpoints
+from .utils.simulation_results import SimulationResults
 
-__all__ = ["QcMps", "QCEmulator", "mock_fortran", "run_py_simulation"]
+__all__ = ["QCEmulator", "run_py_simulation"]
 
 
 class QCEmulator:
     """
     Emulator class to run quantum circuits, powered by either
     TTNs or MPS.
 
 
     Parameters
     ----------
 
     num_sites: int
         Number of sites
-    num_clbits: int
-        Number of classical bits
     convergence_parameters: :py:class:`QCConvergenceParameters`
         Class for handling convergence parameters. In particular, in the MPS simulator we are
         interested in:
         - the *maximum bond dimension* :math:`\\chi`;
         - the *cut ratio* :math:`\\epsilon` after which the singular values are neglected, i.e.
           if :math:`\\lambda_1` is the bigger singular values then after an SVD we neglect all the
           singular values such that :math:`\\frac{\\lambda_i}{\\lambda_1}\\leq\\epsilon`
     local_dim: int, optional
         Local dimension of the degrees of freedom. Default to 2.
+    tensor_backend: TensorBackend, optional
+        Contains all the information on the tensors, such as dtype and device.
+        Default to TensorBackend() (dtype=np.complex128, device="cpu").
+    qc_backend: QCBackend, optional
+        Backend for the qmatchatea emulation, containing the backend and other important infos.
+        Default to QCBackend() (ansatz="MPS", precision="A", device="cpu")
+    initialize: str, optional
+        Initialization procedure.
+        Default to "vacuum", the 0000...0 state.
+        Available: "random", "vacuum", path_to_file
     """
 
+    ansatzes = {"MPS": MPS, "TTN": TTN, "MPIMPS": MPIMPS}
+
     def __init__(
         self,
         num_sites,
         convergence_parameters=QCConvergenceParameters(),
         local_dim=2,
-        dtype=np.complex128,
-        device="cpu",
-        ansatz="MPS",
+        tensor_backend=TensorBackend(),
+        qc_backend=QCBackend(),
+        initialize="vacuum",
     ):
         if not isinstance(convergence_parameters, TNConvergenceParameters):
             raise TypeError(
                 "convergence_parameters must be of the QCConvergenceParameters class"
             )
+        if qc_backend.device != tensor_backend.device:
+            raise ValueError("Tensor backend and QCBackend have different devices")
 
         self._trunc_tracking_mode = convergence_parameters.trunc_tracking_mode
-        self.ansatz = ansatz
+        self._qc_backend = qc_backend
 
         # Classical registers to hold qiskit informations
         self.cl_regs = {}
 
         # Observables measured
         self.is_measured = [
             True,
@@ -113,33 +114,60 @@
             True,
             True,
             True,
             False,
             False,
         ]
 
-        if ansatz.upper() == "MPS":
-            self.emulator = MPS(
+        # If a TTN, pad with empty sites until you get to a power of 2 sites
+        if self.ansatz == "TTN":
+            if num_sites & (num_sites - 1) == 0:
+                exponent = np.ceil(np.log2(num_sites))
+                num_sites = int(2**exponent)
+
+        # Initialize based on the intialized keyword
+        if os.path.isfile(initialize):
+            if initialize.endswith(
+                "pkl" + self.ansatzes[qc_backend.ansatz.upper()].extension
+            ):
+                self.emulator = self.ansatzes[qc_backend.ansatz.upper()].read_pickle(
+                    filename=initialize
+                )
+            elif initialize.endswith(
+                self.ansatzes[qc_backend.ansatz.upper()].extension
+            ):
+                self.emulator = self.ansatzes[qc_backend.ansatz.upper()].read(
+                    filename=initialize,
+                    tensor_backend=tensor_backend,
+                    cmplx=np.iscomplex(np.empty(1, dtype=tensor_backend.dtype))[0],
+                    order="F",
+                )
+            else:
+                raise IOError(f"Extension {initialize} not supported by QCEmulator")
+
+            self.emulator._tensor_backend = tensor_backend
+            self.emulator._convergence_parameters = convergence_parameters
+        else:
+            self.emulator = self.ansatzes[qc_backend.ansatz.upper()](
                 num_sites=num_sites,
                 convergence_parameters=convergence_parameters,
                 local_dim=local_dim,
-                dtype=dtype,
-                device=device,
+                initialize=initialize,
+                tensor_backend=tensor_backend,
             )
-        elif ansatz.upper() == "TTN":
-            zero_state = np.zeros((num_sites, local_dim), dtype=dtype)
-            zero_state[:, 0] = 1
-            self.emulator = TTN.product_state_from_local_states(
-                zero_state,
-                convergence_parameters=convergence_parameters,
-                dtype=dtype,
-                device=device,
-            )
-        else:
-            raise ValueError(f"Ansatz {ansatz} is not available for QCEmulator")
+
+    @property
+    def tensor_backend(self):
+        """Tensor backend of the simulation"""
+        return self.emulator._tensor_backend
+
+    @property
+    def ansatz(self):
+        """Ansatz of the emulator"""
+        return self._qc_backend.ansatz
 
     def __getattr__(self, __name: str):
         """
         Check for the attribute in emulator, i.e. the QCEmulator inherits all
         the emulator calls.
         This call is for convenience and for retrocompatibility
 
@@ -147,78 +175,98 @@
             The method `__getattr__` is called when `__getattribute__` fails,
             so it already covers the possibility of the attribute being in the
             base class
         """
         return self.emulator.__getattribute__(__name)
 
     @classmethod
-    def from_emulator(cls, emulator, conv_params=None, dtype=None):
+    def from_emulator(
+        cls, emulator, conv_params=None, tensor_backend=None, qc_backend=QCBackend()
+    ):
         """
         Initialize the QCEmulator class starting from an emulator class, i.e. either
         MPS or TTN
 
         Parameters
         ----------
         emulator : :class:`_AbstractTN`
             Either an MPS or TTN emulator
         conv_params : :class:`TNConvergenceParameters`, optional
             Convergence parameters. If None, the convergence parameters of the emulator
             are used
-        dtype : type, optional
-            Type to be used, If None, the dtype of the emulator is used
+        tensor_backend: TensorBackend, optional
+            Contains all the information on the tensors, such as dtype and device.
+            Default to TensorBackend() (dtype=np.complex128, device="cpu").
+        qc_backend : QCBackend(), optional
+            Backend of the qmatchatea simulation
 
         Return
         ------
         QCEmulator
             The quantum circuit emulator class
         """
         if not isinstance(emulator, _AbstractTN):
             raise TypeError("The emulator should be a TN emulator class")
         if conv_params is None:
-            conv_params = emulator.convergence_parameters
-        if dtype is None:
-            dtype = emulator.dtype
+            conv_params = emulator._convergence_parameters
+        if tensor_backend is None:
+            tensor_backend = emulator._tensor_backend
 
         simulator = cls(
-            emulator.num_sites, conv_params, emulator.local_dim, dtype=dtype
+            emulator.num_sites,
+            conv_params,
+            emulator.local_dim,
+            tensor_backend=tensor_backend,
+            qc_backend=qc_backend,
         )
+        emulator._convergence_parameters = conv_params
+        emulator._tensor_backend = tensor_backend
         simulator.emulator = emulator
-        simulator.ansatz = str(emulator)
+        simulator.emulator.convert(
+            device=tensor_backend.device, dtype=tensor_backend.dtype
+        )
 
         return simulator
 
     @classmethod
-    def from_tensor_list(cls, tensor_list, conv_params=None, dtype=None):
+    def from_tensor_list(
+        cls, tensor_list, conv_params=None, tensor_backend=None, qc_backend=QCBackend()
+    ):
         """
         Initialize the QCEmulator class starting from a tensor list, i.e. either
         MPS or TTN
 
         Parameters
         ----------
         tensor_list : list of tensors
             Either an MPS or TTN list of tensors
         conv_params : :class:`TNConvergenceParameters`, optional
             Convergence parameters. If None, the convergence parameters of the emulator
             are used
-        dtype : type, optional
-            Type to be used, If None, the dtype of the emulator is used
+        tensor_backend: TensorBackend, optional
+            Contains all the information on the tensors, such as dtype and device.
+            Default to TensorBackend() (dtype=np.complex128, device="cpu").
+        qc_backend : QCBackend(), optional
+            Backend of the qmatchatea simulation
 
         Return
         ------
         QCEmulator
             The quantum circuit emulator class
         """
         # A list of lists is a TTN, while a list of tensors is an MPS
-        if isinstance(tensor_list[0], list):
-            initial_state = TTN.from_tensor_list(tensor_list)
-        else:
-            initial_state = MPS.from_tensor_list(tensor_list)
+        initial_state = cls.ansatzes[qc_backend.ansatz].from_tensor_list(
+            tensor_list, conv_params=conv_params, tensor_backend=tensor_backend
+        )
 
         simulator = cls.from_emulator(
-            initial_state, conv_params=conv_params, dtype=dtype
+            initial_state,
+            conv_params=conv_params,
+            tensor_backend=tensor_backend,
+            qc_backend=qc_backend,
         )
 
         return simulator
 
     def meas_projective(
         self, nmeas=1024, qiskit_convention=True, seed=None, unitary_setup=None
     ):
@@ -235,165 +283,155 @@
         return self.emulator.to_statevector(qiskit_order, max_qubit_equivalent)
 
     def apply_two_site_gate(self, operator, control, target):
         """Apply a two-site gate, regardless of the position on the chain
 
         Parameters
         ----------
-        operator : np.ndarray
+        operator : QTeaTensor
             Gate to be applied
         control : int
             control qubit index
         target : int
             target qubit index
 
         Returns
         -------
         singvals_cut
             singular values cut in the process
         """
-        xp = self._device_checks()
-        if operator.shape == (4, 4):
-            operator = operator.reshape(2, 2, 2, 2)
+        local_dim = self.local_dim[0]
+        if operator.shape == (local_dim**2, local_dim**2):
+            operator = operator.reshape([local_dim] * 4)
         # Reorder for qiskit convention on the two-qubits gates
         if control < target or self.ansatz == "TTN":
-            operator = xp.transpose(operator, [1, 0, 3, 2])
+            operator = operator.transpose([1, 0, 3, 2])
 
         singvals_cut = self.apply_two_site_operator(operator, [control, target])
 
         # Avoid errors due to no singv cut
         singvals_cut = np.append(singvals_cut, 0)
         if self._trunc_tracking_mode == "M":
-            singvals_cut = max(0, xp.max(singvals_cut))
+            singvals_cut = max(0, singvals_cut.max())
         elif self._trunc_tracking_mode == "C":
-            singvals_cut = xp.sum(singvals_cut**2)
+            singvals_cut = (singvals_cut**2).sum()
+
+        if hasattr(singvals_cut, "get"):
+            singvals_cut = singvals_cut.get()
 
         return [singvals_cut]
 
-    def meas_observables(self, observables, op_list, op_mapping=None, approach="PF"):
+    def apply_multi_site_gate(self, operator, sites):
+        """
+        Apply a n-sites gate, regardless of the position on the chain
+
+        Parameters
+        ----------
+        operator : QTeaTensor | List[QTeaTensor]
+            If a single QTeaTensor, it is the unitary matrix of the
+            n-qubits gate. If a List[QTeaTensor] it is already
+            written in the MPO form
+        sites : List[int]
+            Sites to which the operator should be applied
+
+        Returns
+        -------
+        singvals_cut
+            singular values cut in the process
+        """
+        # This site order could be reversed for the qiskit convention
+        site_order = np.argsort(sites)
+        local_dim = self.local_dim[sites[0]]
+        if isinstance(operator, self.tensor_backend.tensor_cls):
+            operator = operator.reshape([local_dim] * len(sites) * 2)
+            transpose_idxs = np.arange(operator.ndim).reshape(2, -1)
+            transpose_idxs[0, :] = transpose_idxs[0, site_order]
+            transpose_idxs[1, :] = transpose_idxs[1, site_order]
+            operator.transpose_update(transpose_idxs.reshape(-1))
+            operator = DenseMPO.from_matrix(
+                operator, sites, local_dim, self._convergence_parameters
+            )
+
+        singvals_cut = self.apply_mpo(operator)
+
+        # Avoid errors due to no singv cut
+        singvals_cut = np.append(singvals_cut, 0)
+        if self._trunc_tracking_mode == "M":
+            singvals_cut = max(0, singvals_cut.max())
+        elif self._trunc_tracking_mode == "C":
+            singvals_cut = (singvals_cut**2).sum()
+
+        if hasattr(singvals_cut, "get"):
+            singvals_cut = singvals_cut.get()
+
+        return [singvals_cut]
+
+    def meas_observables(self, observables, operators):
         """Measure all the observables
 
         Parameters
         ----------
         observables : :py:class:`TNObservables`
             All the observables to be measured
-        op_list : list of tensors
+        oeprators : :py:class:`TNOperators`
             List of operators that form the circuit stored in THE CORRECT DEVICE.
             If you are running on GPU the operators should be on the GPU.
-        op_mapping : dict
-            Mapping between the operators name and the operators idx
-        approach : string, optional
-            Approach of the simulation, if 'PY', 'PF'
 
         Returns
         -------
         TNObservables
             Observables with the results in results_buffer
         """
         if not isinstance(observables, TNObservables):
             raise TypeError("observables must be TNObservables")
 
-        keys = np.array(list(observables.obs_list.keys()))[self.is_measured]
-        ii = 0
-        ## LOCAL OBSERVABLES ##
-        local = observables.obs_list[keys[ii]]
-        for name, idx in zip(local.name, local.operator):
-            if approach == "PF":
-                idx = op_mapping[idx] - 1
-            local.results_buffer[name] = self.meas_local(op_list[idx])
-        ii += 1
-
-        ## SAVE STATE ##
-        state_obs = observables.obs_list[keys[ii]]
-        if len(state_obs.name) > 0:
-            if approach == "PY":
-                observables.results_buffer["tn_state"] = self.emulator.to_tensor_list()
-            else:
-                name = state_obs.name[0]
-                state_obs.results_buffer[name] = name
-                self.emulator.write(name)
-        ii += 1
-
-        ## TENSOR PRODUCT OBSERVABLES ##
-        tensor_prod = observables.obs_list[keys[ii]]
-        for name, ops, sites in zip(
-            tensor_prod.name, tensor_prod.operators, tensor_prod.sites
-        ):
-            sites = [site[0] for site in sites]
-            if approach == "PF":
-                operators = [op_list[op_mapping[ii] - 1] for ii in ops]
-            else:
-                operators = [op_list[ii] for ii in ops]
-            tensor_prod.results_buffer[name] = np.complex128(
-                self.emulator.meas_tensor_product(operators, sites)
+        with warnings.catch_warnings():
+            # We use a function that raises a warning for a specific thing we are not interested in.
+            # So we filter it out.
+            warnings.filterwarnings(
+                "ignore",
+                message="Tried to compute energy with no effective operators. Returning nan",
             )
-        ii += 1
-
-        ## WEIGHTED SUM OBSERVABLES ##
-        wsum = observables.obs_list[keys[ii]]
-        for name, coef, tp_ops in zip(wsum.name, wsum.coeffs, wsum.tp_operators):
-            op_string = []
-            idxs_string = []
-            if isinstance(tp_ops, list):
-                tp_op = tp_ops[0]
-            else:
-                tp_op = tp_ops
-            for ops, sites in zip(tp_op.operators, tp_op.sites):
-                sites = [site[0] for site in sites]
-                if approach == "PF":
-                    operators = [op_list[op_mapping[ii] - 1] for ii in ops]
+            # At the moment, observables are only measured serially
+            if self.ansatz == "MPIMPS":
+                if self._qc_backend.mpi_settings[-1] < 0:
+                    self.emulator.reinstall_isometry_serial()
                 else:
-                    operators = [op_list[ii] for ii in ops]
-                idxs_string.append(sites)
-                op_string.append(operators)
-
-            wsum.results_buffer[name] = np.complex128(
-                self.emulator.meas_weighted_sum(op_string, idxs_string, coef)
-            )
-        ii += 1
-
-        ## FINAL PROJECTIVE MEASUREMENT OBSERVABLES ##
-        proj_obs = observables.obs_list[keys[ii]]
-        proj_obs.results_buffer[proj_obs.name[0]] = self.meas_projective(
-            nmeas=proj_obs.num_shots
-        )
-        ii += 1
-
-        ## PROBABILITY MEASURE ##
-        prob_obs = observables.obs_list[keys[ii]]
-        for name, prob_type, prob_param in zip(
-            prob_obs.name, prob_obs.prob_type, prob_obs.prob_param
-        ):
-            if isinstance(name, list):
-                name = name[0]
-            if prob_type == "U":
-                prob_obs.results_buffer[
-                    name
-                ] = self.emulator.meas_unbiased_probabilities(prob_param, True)
-            elif prob_type == "E":
-                prob_obs.results_buffer[name] = self.emulator.meas_even_probabilities(
-                    prob_param, True
+                    self.emulator.reinstall_isometry_parallel(
+                        self._qc_backend.mpi_settings[-1]
+                    )
+                rank = self.emulator.rank
+                tensor_list = self.emulator.mpi_gather_tn()
+                if rank != 0:
+                    return observables
+                emulator = MPS.from_tensor_list(
+                    tensor_list,
+                    self.emulator._convergence_parameters,
+                    self.tensor_backend,
                 )
-            elif prob_type == "G":
-                prob_obs.results_buffer[name] = self.emulator.meas_greedy_probabilities(
-                    prob_param, True
-                )
-        ii += 1
+            else:
+                rank = 0
+                emulator = self.emulator
 
-        ## ENTANGLEMENT MEASURE ##
-        ent_obs = observables.obs_list[keys[ii]]
-        if len(ent_obs.name) == 1:
-            bond_entropy = self.emulator.meas_bond_entropy()
-            ent_obs.results_buffer[ent_obs.name[0]] = bond_entropy
-        ii += 1
+            if rank == 0:
+                emulator.normalize()
+                observables = run_tn_measurements(
+                    state=emulator,
+                    observables=observables,
+                    operators=operators,
+                    params={},
+                    tensor_backend=self.tensor_backend,
+                    tn_type=6 if self.ansatz in ("MPS", "MPSMPI") else 5,
+                )
 
         return observables
 
     def run_circuit_from_instruction(self, op_list, instr_list):
-        """Run a circuit
+        """
+        Run a circuit from the istructions similar to those of fortran
 
         Parameters
         ----------
         op_list : list of tensors
             List of operators that form the circuit
         instr_list : list of instructions
             Instruction for the circuit, i.e. [op_name, op_idx, [sites] ]
@@ -424,111 +462,185 @@
                 elif self._trunc_tracking_mode == "C":
                     singvals_cut.append(np.sum(singv_cut**2))
 
             else:
                 raise ValueError("Only one and two-site operations are implemented")
         return singvals_cut
 
-    def run_from_qk(self, circuit):
+    def run_from_qk(self, circuit, operators=None, checkpoints=QCCheckpoints()):
         """
         Run a qiskit quantum circuit on the simulator
 
         Parameters
         ----------
         circuit : :py:class:`QuantumCircuit`
             qiskit quantum circuit
+        operators : TNOperators
+            Operators class
+        checkpoints : QCCheckpoints
+            Checkpoints class
 
         Returns
         -------
-        list of floats
+        List[float]
             singular values cutted in the simulation
-        """
-        xp = self._device_checks()
-        data = circuit.data  # data structure of the quantum circuit
+        Dictionary[TNObservables]
+            The dictionary with the observables measured mid circuit
+        List[float]
+            Memory used in the simulation in bytes
+        """
+        # data structure of the quantum circuit
+        data = circuit.data[checkpoints._initial_line :]
+        process = psutil.Process()
+        memory = np.zeros(len(data))
+        obs_dict = {}
         singvals_cut = []
         for creg in circuit.cregs:
             self.cl_regs[creg.name] = np.zeros(creg.size)
 
+        start_time = time.time()
+        barrier_cnt = 0
         # Run over instances
-        for instance in data:
-            gate_name = instance[0].name
-            num_qubits = len(instance[1])
-            qubits = [circuit.find_bit(qub).index for qub in instance[1]]
+        for idx, instance in enumerate(data):
+            try:
+                operation = instance[0]
+                qubits = instance[1]
+                clbits = instance[2]
+            except AttributeError:
+                operation = instance.operation
+                qubits = instance.qubits
+                clbits = instance.clbits
+            gate_name = operation.name
+            num_qubits = len(qubits)
+            qubits = [circuit.find_bit(qub).index for qub in qubits]
 
             if gate_name == "barrier":
+                if self._qc_backend.mpi_settings[barrier_cnt] < 0:
+                    self.emulator.reinstall_isometry_serial()
+                else:
+                    self.emulator.reinstall_isometry_parallel(
+                        self._qc_backend.mpi_settings[barrier_cnt]
+                    )
+                barrier_cnt += 1
                 continue
             elif gate_name == "measure":
                 meas_state, _ = self.apply_projective_operator(*qubits)
-                self.cl_regs[instance[2][0].register.name][0] = meas_state
+                self.cl_regs[clbits[0].register.name][0] = meas_state
                 continue
             elif gate_name == "reset":
                 self.reset(qubits)
                 continue
+            elif gate_name == "MeasureObservables":
+                tic = time.time()
+                obs = self.meas_observables(instance[0].observables, operators)
+                toc = time.time()
+                obs.results_buffer["time"] = tic - start_time
+                obs.results_buffer["energy"] = None
+                obs.results_buffer["norm"] = self.norm()
+                obs.results_buffer["measurement_time"] = toc - tic
+                obs_dict[instance[0].label] = obs
+                continue
             else:
-                gate_mat = instance[0].to_matrix()
+                gate_mat = operation.to_matrix()
 
-            if instance[0].condition is None:
+            if operation.condition is None:
                 apply_gate = True
             else:
-                bit_idx = [clbit.index for clbit in instance[0].condition[0]]
-                bit_value = self.cl_regs[instance[0].condition[0].name][bit_idx[0]]
-                apply_gate = bit_value == instance[0].condition[1]
+                bit_idx = [clbit.index for clbit in operation.condition[0]]
+                bit_value = self.cl_regs[operation.condition[0].name][bit_idx[0]]
+                apply_gate = bit_value == operation.condition[1]
 
             if apply_gate:
-                # Move the operator to the GPU
-                if xp == cp:
-                    gate_mat = cp.asarray(gate_mat)
+                # Move the operator to the correct device
+                gate = self.tensor_backend.tensor_cls.from_elem_array(
+                    gate_mat, self.tensor_backend.dtype, self.tensor_backend.device
+                )
                 if num_qubits == 1:
-                    self.emulator.apply_one_site_operator(gate_mat, *qubits)
+                    self.emulator.apply_one_site_operator(gate, *qubits)
                 elif num_qubits == 2:
-                    singv_cut = self.apply_two_site_gate(gate_mat, *qubits)
+                    singv_cut = self.apply_two_site_gate(gate, *qubits)
                     singvals_cut += singv_cut
                 else:
-                    raise ValueError("Only one and two-site operations are implemented")
-        return singvals_cut
+                    singv_cut = self.apply_multi_site_gate(gate, qubits)
+                    singvals_cut += singv_cut
+
+            memory[idx] = process.memory_info().rss
+            # Check if you can change settings every n iterations
+            self._runtime_checks_updates(idx, self.num_sites, singvals_cut)
+            # Save checkpoints if needed
+            checkpoints.save_checkpoint(idx, self.emulator)
 
-    def run_from_qcirc(self, qcirc, starting_idx=0):
+        return singvals_cut, obs_dict, memory
+
+    def run_from_qcirc(self, qcirc, starting_idx=0, checkpoints=QCCheckpoints()):
         """
-        Run a simulation starting from a Qcircuit on a portion of the MPS state
+        Run a simulation starting from a Qcircuit on a portion of the TN state
 
         Parameters
         ----------
         qcirc : :class:`Qcircuit`
             Quantum circuit
         starting_idx : int, optional
             MPS index that correspond to the index 0 of the Qcircuit. Default to 0.
+        checkpoints : QCCheckpoints, optional
+            Checkpoints in the simulation
+
+        Returns
+        -------
+        List[float]
+            singular values cutted in the simulation
+        Dictionary[TNObservables]
+            The dictionary with the observables measured mid circuit
+        List[float]
+            Memory used in the simulation in bytes
         """
         if not isinstance(qcirc, Qcircuit):
             raise TypeError(f"qcirc must be of type Qcircuit, not {type(qcirc)}")
-        xp = self._device_checks()
-        results = {}
-        svd_cuts = []
+
+        process = psutil.Process()
+        memory = np.zeros(len(qcirc))
+        obs_dict = {}
+        singvals_cut = []
         start_time = time.time()
+        cnt = -1
         for layer in qcirc:
             for instruction in layer:
+                cnt += 1
+                if cnt < checkpoints._initial_line:
+                    continue
                 sites = [ss + starting_idx for ss in instruction[1]]
                 operation = instruction[0]
 
                 # Check for classical conditioning
                 appy_operation = operation.c_if.is_satisfied(qcirc)
                 if appy_operation:
                     # First, check for particular keywords
                     if isinstance(operation, QCObservableStep):
+                        operators = (
+                            self.tensor_backend.base_tensor_cls.convert_operator_dict(
+                                operation.operators,
+                                params={},
+                                symmetries=[],
+                                generators=[],
+                                base_tensor_cls=self.tensor_backend.base_tensor_cls,
+                                dtype=self.tensor_backend.dtype,
+                                device=self.tensor_backend.device,
+                            )
+                        )
                         obs = self.meas_observables(
                             operation.observables,
-                            operation.operators.ops,
-                            approach="PY",
+                            operators,
                         )
                         obs.results_buffer["time"] = time.time() - start_time
                         obs.results_buffer["norm"] = self.norm()
                         operation.observables = obs
                         operation.postprocess_obs_indexing()  # Postprocess for qregisters
                         for elem in obs.obs_list:
                             obs.results_buffer.update(obs.obs_list[elem].results_buffer)
-                        results[operation.name] = deepcopy(
+                        obs_dict[operation.name] = deepcopy(
                             operation.observables.results_buffer
                         )
                         del obs
 
                     # Check for particular keywords
                     elif operation.name == "renormalize":
                         self.normalize()
@@ -543,237 +655,79 @@
                     elif operation.name == "add_site":
                         self.emulator.add_site(operation.position)
                     elif operation.name == "remove_site":
                         self.apply_projective_operator(operation.position, remove=True)
 
                     # Apply gates
                     elif len(sites) == 1:
-                        if xp == cp:
-                            gate_mat = cp.asarray(gate_mat)
+                        gate = self.tensor_backend.tensor_cls.from_elem_array(
+                            operation.operator,
+                            self.tensor_backend.dtype,
+                            self.tensor_backend.device,
+                        )
                         self.site_canonize(*sites, keep_singvals=True)
-                        self.apply_one_site_operator(operation.operator, *sites)
+                        self.apply_one_site_operator(gate, *sites)
+                    elif len(sites) == 2:
+                        gate = self.tensor_backend.tensor_cls.from_elem_array(
+                            operation.operator,
+                            self.tensor_backend.dtype,
+                            self.tensor_backend.device,
+                        )
+                        svd_cut = self.apply_two_site_gate(gate, *sites)
+                        singvals_cut += svd_cut
                     else:
-                        if xp == cp:
-                            gate_mat = cp.asarray(gate_mat)
-                        svd_cut = self.apply_two_site_gate(operation.operator, *sites)
-                        svd_cuts += svd_cut
-
-        # Truncation
-        results["singular_values_cut"] = svd_cuts
-        return results
-
-
-class QcMps(QCEmulator):
-    """
-    Class for retrocompatibility with QCEmulator
-    """
-
-    def __init__(self, *args, **kwargs):
-        warn("Using deprecated QcMps, please switch to QCEmulator")
-        super().__init__(*args, **kwargs)
-
-
-def mock_fortran(command_line, observables, op_mapping):
-    """
-    Mock the execution of the Fortran program, by doing the exact same things Fortran would do
-
-    Parameters
-    ----------
-    command_line : list of str
-        List of commands that should be run on terminal for the compiled fortran simulator
-    """
-    input_dict_path = command_line[-1]
-    if not os.path.isfile(input_dict_path):
-        raise ValueError(
-            'The given PATH "%s" for the input file is not a file.'
-            % (str(input_dict_path))
-        )
-
-    _, input_dict = read_nml(command_line[-1])
-
-    # Checks and retrieval on input parameters
-    if input_dict["checkpoint_frequency"] > 0:
-        raise NotImplementedError(
-            "Checkpoints are not implemented in the python simulator"
-        )
-    io_info = QCIO(
-        inPATH=input_dict["inPATH"],
-        outPATH=input_dict["outPATH"],
-        sparse=input_dict["sparse"],
-    )
-    conv_params = QCConvergenceParameters(
-        max_bond_dimension=input_dict["max_bond_dimension"],
-        cut_ratio=input_dict["cut_ratio"],
-        trunc_tracking_mode=input_dict["trunc_tracking_mode"],
-    )
-
-    # Retrieve input information on operators and circuit
-    op_list, instruction_list, num_sites, num_cl_bits = _mock_fortran_input(io_info)
-
-    # Initialize the state
-    emulator = QCEmulator(
-        num_sites,
-        num_cl_bits,
-        conv_params,
-        input_dict["local_dim"],
-        ansatz=input_dict["ansatz"],
-    )
-
-    # Retrieve initial state if present
-    if input_dict["initial_state"] != "Vacuum":
-        initial_state_path = os.path.join(io_info.inPATH, input_dict["initial_state"])
-        emulator.read(initial_state_path)
-
-    # Run the circuit
-    start = time.time()
-    singvals_cut = emulator.run_circuit_from_instruction(op_list, instruction_list)
-    simulation_time = time.time() - start
-
-    # Perform measurements and final operations
-    observables = _mock_fortran_measurements(emulator, observables, op_list, op_mapping)
-    observables.results_buffer["time"] = simulation_time
-
-    # Write everithing in the output directory
-    _mock_fortran_output(emulator, io_info, input_dict, singvals_cut, observables)
-
-    return True
-
-
-def _mock_fortran_input(io_info):
-    """
-    Perform the reading necessary for the python emulator
-
-    Parameters
-    ----------
-    io_info : :py:class:`QCIO`
-        IO informations
-
-    Returns
-    -------
-    op_list: list of ndarray
-        List of operators
-    instruction_list: list
-        list of instruction for the circuit
-    num_sites: int
-        Number of sites in the MPS
-    num_cl_bits : int
-        Number of classical bits in the MPS
-    """
-    if not isinstance(io_info, QCIO):
-        raise TypeError("io_info must be of type QCIO")
-
-    # Retrieve operators
-    op_path = os.path.join(io_info.inPATH, "TENSORS/operators.dat")
-    op_list = []
-    with open(op_path, "r") as fh:
-        op_num = int(fh.readline().replace("\n", ""))
-        for _ in range(op_num):
-            tens = read_tensor(fh)
-            op_list.append(tens)
-
-    # Retrieve circuit
-    instruction_path = os.path.join(io_info.inPATH, "circuit.dat")
-    instruction_list = []
-    with open(instruction_path, "r") as fh:
-        num_sites = int(fh.readline().replace("\n", ""))
-        num_cl_bits = int(fh.readline().replace("\n", ""))
-        num_lines = int(fh.readline().replace("\n", ""))
-        for _ in range(num_lines):
-            line_1 = fh.readline().replace("\n", "").split(" ")
-            line_2 = fh.readline().replace("\n", "").split(" ")
-            line_2.remove("")
-            # [ name, op_idx, [qubits] ]
-            instruction = [
-                line_1[0],
-                int(line_1[1]) - 1,
-                [int(site) - 1 for site in line_2],
-            ]
-
-            instruction_list.append(instruction)
-
-    return op_list, instruction_list, num_sites, num_cl_bits
-
-
-def _mock_fortran_measurements(emulator, observables, op_list, op_mapping):
-    """
-    Perform the different measurements to mock with python a fortran simulation
-
-    Parameters
-    ----------
-    emulator : :py:class:`QCEmulator`
-        Matrix product state class
-    observables : :py:class:`TNObservables`
-        Observables class
-    op_list : list of ndarray
-        List of operators
-
-    Return
-    ------
-    measurements : OrderedDict
-        Ordered dictionary with as keys:
-            - proj_meas, the projective measurements dictionary
-            - statevector, the statevector
-            - entanglement, the entanglement
-            - obs_results, the observables results
-
-    """
-    if not isinstance(emulator, QCEmulator):
-        raise TypeError("mps_state must be of type emulator")
-    elif not isinstance(observables, TNObservables):
-        raise TypeError("observables must be of type TNObservables")
-
-    # Observables with measured quantities
-    observables = emulator.meas_observables(observables, op_list, op_mapping)
-    observables.results_buffer["energy"] = 999e300
-    observables.results_buffer["norm"] = emulator.norm()
-
-    return observables
+                        gate = self.tensor_backend.tensor_cls.from_elem_array(
+                            operation.operator,
+                            self.tensor_backend.dtype,
+                            self.tensor_backend.device,
+                        )
+                        svd_cut = self.apply_multi_site_gate(gate, sites)
+                        singvals_cut += svd_cut
 
+                # Check if you can change settings every n iterations
+                self._runtime_checks_updates(cnt, self.num_sites, singvals_cut)
+                # Save checkpoints if needed
+                checkpoints.save_checkpoint(cnt, self.emulator)
+                memory[cnt] = process.memory_info().rss
 
-def _mock_fortran_output(emulator, io_info, input_dict, singval_cut, observables):
-    """
-    Mock the fortran simulator by writing the same output files it would
-    write
+        return singvals_cut, obs_dict, memory
 
-    Parameters
-    ----------
-    emulator : :py:class:`QCEmulator`
-        QCEmulator state class
-    io_info : :py:class:`QCIO`
-        Info about the output file path
-    input_dict : OrderedDict
-        Ordered dictionary with the input parameters
-    singval_cut : array-like
-        Singular values cut in the simulation
-    observables : :py:class:`TNObservables`
-        Observables
-    """
-    if not isinstance(emulator, QCEmulator):
-        raise TypeError("mps_state must be of type QCEmulator")
-    elif not isinstance(io_info, QCIO):
-        raise TypeError("io_info must be of type QCIO")
-
-    # Observables
-    obs_path = os.path.normpath(input_dict["observables_filename"])
-    obs_path = os.path.join(io_info.outPATH, obs_path)
-    observables.write_results(obs_path, emulator.is_measured, {})
+    def _runtime_checks_updates(self, idx, frequency, norm_cut):
+        """
+        Perform the checks to change the device and the precision if
+        idx%frequency is 0.
 
-    with open(os.path.join(io_info.outPATH, "singular_values_cut.txt"), "w") as fh:
-        _write_value(singval_cut, fh)
+        Parameters
+        ----------
+        idx : int
+            Index of the current operation of the quantum circuit
+        frequency: int
+            The checks are done every frequency operations
+        norm_cut: float
+            The norm cut in the last simulation
+        """
+        if idx % frequency == 0:
+            device = self._qc_backend.resolve_device(
+                self.emulator.current_max_bond_dim, self.tensor_backend.device
+            )
+            precision = self._qc_backend.resolve_precision(
+                (1 - np.array(norm_cut)).prod()
+            )
+            self.emulator.convert(device=device, dtype=precision)
 
 
 def run_py_simulation(
     circ,
     local_dim=2,
     convergence_parameters=QCConvergenceParameters(),
     operators=QCOperators(),
     observables=TNObservables(),
     initial_state=None,
-    transpilation_parameters=qk_transpilation_params(),
     backend=QCBackend(),
+    checkpoints=QCCheckpoints(),
 ):
     """
     Transpile the circuit to adapt it to the linear structure of the MPS and run the circuit,
     obtaining in output the measurements.
 
     Parameters
     ----------
@@ -787,116 +741,141 @@
         Operator class with the observables operators ALREADY THERE. If None, then it is
         initialized empty. Default to None.
     observables: :py:class:`TNObservables`, optional
         The observables to be measured at the end of the simulation. Default to TNObservables(),
         which contains no observables to measure.
     initial_state : list on ndarray, optional
         Initial state of the simulation. If None, ``|00...0>`` is considered. Default to None.
-    transpilation_parameters: :py:class:`qk_transpilation_params`, optional
-        Parameters used in the qiskit transpilation phase. Default to qk_transpilation_params().
     backend: :py:class:`QCBackend`, optional
         Backend containing all the information for where to run the simulation
+    checkpoints: :py:class:`QCCheckpoints`, optional
+        Class to handle checkpoints in the simulation
 
     Returns
     -------
-    result: qmatchatea.simulation_results
+    result: qmatchatea.SimulationResults
         Results of the simulation, containing the following data:
         - Measures
         - Statevector
         - Computational time
         - Singular values cut
         - Entanglement
         - Measure probabilities
         - MPS state
         - MPS file size
         - Observables measurements
     """
-    # Preprocess the circuit to adapt it to the MPS constraints (linearity)
-    preprocessed_circ = preprocess(circ, qk_params=transpilation_parameters)
-
-    if isinstance(circ, QuantumCircuit):
+    if isinstance(circ, (QuantumCircuit, Qcircuit)):
         num_qubits = circ.num_qubits
-        # num_clbits = circ.num_clbits
     else:
         raise TypeError(
-            "Only qiskit Quantum Circuits are implemented for pure python"
+            "Only qiskit Quantum Circuits and Qcircuit are implemented for pure python"
             + f" simulation, not {type(circ)}"
         )
-    tn_type = np.complex128 if backend.precision == "Z" else np.complex64
+    tn_type = AVAIL_DTYPES[backend.resolve_precision(1)]
     start = time.time()
-    if initial_state is None or initial_state == "Vacuum":
+    tensor_backend = TensorBackend(
+        device=backend.resolve_device(1, "cpu"), dtype=tn_type
+    )
+    if backend.mpi_approach != "SR" and backend.ansatz == "MPS":
+        backend._ansatz = "MPIMPS"
+
+    operators = tensor_backend.base_tensor_cls.convert_operator_dict(
+        operators,
+        params={},
+        symmetries=[],
+        generators=[],
+        base_tensor_cls=tensor_backend.base_tensor_cls,
+        dtype=tensor_backend.dtype,
+        device=tensor_backend.device,
+    )
+    # Check if you selected restart from a checkpoint
+    initial_state = checkpoints.restart_from_checkpoint(initial_state)
+
+    # The scalar check is to avoid a warning
+    if np.isscalar(initial_state):
+        if initial_state is None:
+            initial_state = "vacuum"
         simulator = QCEmulator(
             num_qubits,
             convergence_parameters,
             local_dim=local_dim,
-            dtype=tn_type,
-            ansatz=backend.ansatz,
+            tensor_backend=tensor_backend,
+            qc_backend=backend,
+            initialize=initial_state.lower(),
         )
     elif isinstance(initial_state, _AbstractTN):
         simulator = QCEmulator.from_emulator(
-            initial_state, conv_params=convergence_parameters, dtype=tn_type
+            initial_state,
+            conv_params=convergence_parameters,
+            tensor_backend=tensor_backend,
+            qc_backend=backend,
         )
     else:
         simulator = QCEmulator.from_tensor_list(
-            initial_state, conv_params=convergence_parameters, dtype=tn_type
+            initial_state,
+            conv_params=convergence_parameters,
+            tensor_backend=tensor_backend,
+            qc_backend=backend,
+        )
+    if isinstance(circ, QuantumCircuit):
+        singvals_cut, obs_dict, memory = simulator.run_from_qk(
+            circ, operators, checkpoints
+        )
+    elif isinstance(circ, Qcircuit):
+        singvals_cut, obs_dict, memory = simulator.run_from_qcirc(
+            circ, checkpoints=checkpoints
         )
 
-    simulator.to_device(backend.device)
-    singvals_cut = simulator.run_from_qk(preprocessed_circ)
     end = time.time()
 
-    observables = simulator.meas_observables(observables, operators.ops, approach="PY")
+    tic = time.time()
+    observables = simulator.meas_observables(observables, operators)
+    toc = time.time()
+
     observables.results_buffer["time"] = end - start
     observables.results_buffer["energy"] = None
     observables.results_buffer["norm"] = simulator.norm()
+    observables.results_buffer["measurement_time"] = toc - tic
+    observables.results_buffer["memory"] = memory / (1024**3)
 
     result_dict = observables.results_buffer
-    for elem in observables.obs_list:
-        result_dict.update(observables.obs_list[elem].results_buffer)
 
-    results = simulation_results()
-    results.set_results(result_dict, singvals_cut)
-
-    return results
+    # Observables postprocessing
+    postprocess = False
+    if simulator.ansatz == "MPIMPS":
+        if simulator.rank == 0:
+            postprocess = True
+    else:
+        postprocess = True
 
+    if postprocess:
+        for elem in observables.obs_list:
+            result_dict.update(observables.obs_list[elem].results_buffer)
+            # Special treatment for TNState2file
+            if str(elem) == "TNState2File":
+                for value in observables.obs_list[elem].name:
+                    result_dict["tn_state_path"] = observables.obs_list[
+                        elem
+                    ].results_buffer[value]
+
+        # Storing the results of measurement happened mid-circuit
+        # under their label
+        # pylint: disable-next=consider-using-dict-items
+        for label in obs_dict:
+            obs_values = obs_dict[label]
+            tmp = obs_values.results_buffer
+            for elem in obs_values.obs_list:
+                tmp.update(obs_values.obs_list[elem].results_buffer)
+                # Special treatment for TNState2file
+                if str(elem) == "TNState2File":
+                    for value in obs_values.obs_list[elem].name:
+                        tmp["tn_state_path"] = observables.obs_list[
+                            elem
+                        ].results_buffer[value]
 
-def _write_value(value, fh):
-    """
-    Print a value for the mock fortran output
-    based on its type
+            result_dict[label] = tmp
 
-    Parameters
-    ----------
-    value : scalar, dict or array-like
-        value to be saved
-    fh : file handler
-        Where to write the values
-    """
-
-    # None case
-    if value is not None:
-        # Writing scalar results
-        if np.isscalar(value):
-            if np.iscomplexobj(value):
-                fh.write(f"{np.real(value) }, {np.imag(value) } \n")
-            else:
-                fh.write(f"{value} \n")
+    results = SimulationResults()
+    results.set_results(result_dict, singvals_cut)
 
-        # Writing dictionary results
-        elif isinstance(value, dict):
-            fh.write(f"{len(value)} \n")
-            for subkey, subvalue in value.items():
-                fh.write(f"{subkey} | {subvalue} \n")
-
-        # Writing vector results
-        elif len(np.array(value[0]).shape) < 2:
-            fh.write(f"{len(value)} \n")
-            if np.iscomplexobj(value):
-                for subvalue in value:
-                    fh.write(f"{np.real(subvalue) }, {np.imag(subvalue) } \n")
-            else:
-                for subvalue in value:
-                    fh.write(f"{subvalue} \n")
-        else:
-            fh.write(f"{len(value)} \n")
-            for subvalue in value:
-                write_tensor(subvalue, fh, np.iscomplexobj(subvalue))
+    return results
```

### Comparing `qmatchatea-0.5.2/qmatchatea/qk_utils.py` & `qmatchatea-1.1.0/qmatchatea/utils/qk_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,20 +10,62 @@
 
 """
 Utility functions to generate common quantum circuits and have
 a convenient visualization of the quantum state
 """
 from copy import deepcopy
 from qiskit import execute
+from qiskit.circuit import Barrier
 from qiskit_aer.aerprovider import AerSimulator
 import numpy as np
 
 __all__ = ["qiskit_get_statevect", "W_qiskit", "GHZ_qiskit", "QFT_qiskit", "get_index"]
 
 
+class MeasureObservables(Barrier):
+    """
+    Class to apply mid-circuit observables measurements with qmatchatea.
+
+    Parameters
+    ----------
+
+    label: str
+        Name of the observable. It will be used to recover the information
+        at the end of the simulation.
+    num_qubits: int
+        Number of qubits on which the observable is defined. It should be
+        the number of qubits in the quantum circuit.
+    observables: TNObservables
+        The observable class with the information about what you want to
+        measure. The input observables will be copied, and it is thus NOT
+        modified in place.
+    """
+
+    def __init__(self, label, num_qubits, observables):
+        self._obs = deepcopy(observables)
+        # pylint: disable-next=unexpected-keyword-arg
+        super().__init__(num_qubits)
+        self._name = "MeasureObservables"
+        self._label = label
+
+    @property
+    def observables(self):
+        """Observables property"""
+        return self._obs
+
+    @property
+    def label(self):
+        """Return the label of the observable"""
+        return self._label
+
+    def inverse(self):
+        """Special case. Return self."""
+        return self
+
+
 class qk_transpilation_params:
     """Class to contain the
     transpilation parameters used to map
     a qiskit circuit
 
     Parameters
     ----------
```

### Comparing `qmatchatea-0.5.2/qmatchatea/sf_utils.py` & `qmatchatea-1.1.0/qmatchatea/utils/sf_utils.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-0.5.2/qmatchatea/tensor_compiler.py` & `qmatchatea-1.1.0/qmatchatea/tensor_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ---------------------
 
 """
 
 import numpy as np
 from qiskit.extensions import UnitaryGate
 from qiskit.converters import circuit_to_dag, dag_to_circuit
-from .qk_utils import get_index
+from .utils.qk_utils import get_index
 
 __all__ = ["tensor_compiler"]
 
 
 def are_contractable(this, other):
     """
     Check if this DagNode ant the other DagNode
```

### Comparing `qmatchatea-0.5.2/qmatchatea/tn_utils.py` & `qmatchatea-1.1.0/qmatchatea/utils/tn_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,25 +20,18 @@
 import os
 import os.path
 from ast import literal_eval
 from typing import OrderedDict
 import numpy as np
 from qtealeaves import read_tensor
 from qtealeaves.operators import TNOperators
-from qtealeaves.fortran_interfaces import StrBuffer
+from qtealeaves.tooling import StrBuffer
 
 __all__ = ["write_tensor", "write_mps", "read_mps", "QCOperators"]
 
-pauli_matrices = {
-    "Z": np.array([[1, 0], [0, -1]]),
-    "X": np.array([[0, 1], [1, 0]]),
-    "Y": np.array([[0, -1j], [1j, 0]]),
-    "I": np.array([[1, 0], [0, 1]]),
-}
-
 
 def read_nml(namelist_file):
     """
     Read a fortran namelist file
 
     Parameters
     ----------
@@ -190,14 +183,20 @@
     self.ops['op_name'] = op_tensor.
 
     It starts with the pauli operators already defined, with keywords "X","Y","Z"
     """
 
     def __init__(self, folder_operators="TENSORS"):
         TNOperators.__init__(self, folder_operators=folder_operators)
+        pauli_matrices = {
+            "Z": np.array([[1, 0], [0, -1]]),
+            "X": np.array([[0, 1], [1, 0]]),
+            "Y": np.array([[0, -1j], [1j, 0]]),
+            "I": np.array([[1, 0], [0, 1]]),
+        }
         for key, val in pauli_matrices.items():
             self.ops[key] = val
 
     def write_operator(self, folder_dst, operator_name, params, sparse=False):
         """
         Write operator to file.
```

### Comparing `qmatchatea-0.5.2/qmatchatea/utils.py` & `qmatchatea-1.1.0/qmatchatea/utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,31 +12,34 @@
 General utility functions and classes for the simulation
 """
 
 # Import necessary packages
 import os
 import pickle
 import shutil
+import json
+import time
 from warnings import warn
-from datetime import datetime
 from typing import OrderedDict
 import numpy as np
+from qiskit.circuit import QuantumCircuit
+import qiskit.qpy as qpy_serialization
 from qtealeaves import write_nml
 from qtealeaves.convergence_parameters import TNConvergenceParameters
-from qtealeaves.emulator import MPS, TTN
-
+from qtealeaves.emulator import _AbstractTN
 from qtealeaves.observables import TNObservables
+from qtealeaves.tensors.tensor import GPU_AVAILABLE
 
-from .tn_utils import QCOperators, read_mps
+from .tn_utils import QCOperators
+from .mpi_utils import MPISettings
 
 EXE_PATH_DIR = os.path.dirname(__file__)
 EXE_PATH = os.path.join(EXE_PATH_DIR, "bin/qmatchatea.exe")
 
 __all__ = [
-    "simulation_results",
     "print_state",
     "fidelity",
     "QCCheckpoints",
     "QCIO",
     "QCConvergenceParameters",
     "QCBackend",
     "SimpleHamiltonian",
@@ -114,509 +117,67 @@
 
             pauli_dict["paulis"].append(
                 {"label": key, "coeff": {"real": np.real(val), "imag": np.imag(val)}}
             )
         return pauli_dict
 
 
-class simulation_results:
-    """
-    This class is used to handle the results of a simulation with qmatchatea.
-    You can use it to:
-
-    - Retrieve the results of a FORTRAN simulation;
-    - Save the results of a simulation (see the `save_results()` method);
-    - Load the results of a simulation (see the `load_results()` method);
-
-    The results can be then accessed in python through the following properties.
-
-    Input Properties
-    ----------------
-    date_time: str
-        The date-time when the simulation started as ``Year-month-day-Hour:Minute:Second``
-    input_params : dict
-        Dictionary containing all the input informations
-    initial_state : List[np.ndarray] or str
-        The initial state of the simulation
-
-    Output Properties
-    -----------------
-    fidelity: float
-        Lower bound on the fidelity of the final state
-    singular_values_cut : np.ndarray
-        Singular values cut during the simulation
-    measures: dict
-        Projective measures of the simulation, in the format `{"000":15, "011":24}`
-    measure_probabilities: List[dict or None]
-        The 0th element is the result of the unbiased (OPES) sampling, with a format
-        `{"000" : (0, 1)}` where the values are the left and right boundaries of the
-        probability interval.
-        The 1st element is even probability and the 2nd element greedy probabilities,
-        with the format `{"000": 1}`, where the value is the probability of the state
-    tens_net : List[np.ndarray]
-        The tensor network state
-    statevector: np.ndarray or None
-        The statevector of the final state. Returned only if `num_sites<30`
-    entanglement: dict or None
-        Entanglement across bipartition, where the key is the bipartition. An example
-        for a 2-site MPS system in a product state is `{(0,1) : 0}`
-    observables : dict
-        The dictionary containing ALL the observables of the simulation
-    computational_time: float or None
-        Time of the simulation
-    """
-
-    def __init__(self, input_params=None, observables=None):
-        """
-        Initialization. Provide a input params dictionary only if you want to retrieve
-        the result directly from the Fortran working folder.
-        Otherwise, if you want to load previous results, just initialize the class
-        without parameters.
-
-        Parameters
-        ----------
-        input_params: dict, optional
-            If provided contains all the input parameters of the simulation.
-            If it is empty than you should use this class to upload a previous experiment
-        observables: TNObservables, optional
-            observables used in the simulation
-        """
-        # Name of the input parameters in a simulation
-        self._input_params_names = [
-            "num_sites",
-            "local_dim",
-            "approach",
-            "observables_filename",
-            "max_bond_dimension",
-            "cut_ratio",
-            "trunc_tracking_mode",
-            "inPATH",
-            "outPATH",
-            "sparse",
-            "initial_state",
-            "checkpoint_PATH",
-            "checkpoint_frequency",
-            "initial_line",
-        ]
-
-        self._input_params = {} if input_params is None else input_params
-        self._from_simulation = (
-            False  # flag set to True if you have to obtain data from Fortran,
-        )
-        # i.e. if you provide a suitable input parameter dictionary
-
-        if all("settings%" + k in self._input_params for k in self._input_params_names):
-            self.inPATH = input_params["settings%inPATH"]
-            self.outPATH = input_params["settings%outPATH"]
-            assert os.path.isdir(self.inPATH), "Input PATH is not a folder"
-            assert os.path.isdir(self.outPATH), "Output PATH is not a folder"
-            self._from_simulation = True
-
-        self._datetime = datetime.today().strftime("%Y-%m-%d-%H:%M:%S")
-
-        # Set to None all the variables
-        self._initial_state = "Vacuum"
-        if "settings%initial_state" in self._input_params:
-            if self._input_params["settings%initial_state"] == "Vacuum":
-                pass
-            elif int(self._input_params["settings%initial_line"]) == 1:
-                self._initial_state = read_mps(
-                    os.path.join(
-                        self.inPATH, self._input_params["settings%initial_state"]
-                    )
-                )
-            else:
-                self._initial_state = read_mps(
-                    os.path.join(
-                        self._input_params["settings%checkpoint_PATH"],
-                        self._input_params["settings%initial_state"],
-                    )
-                )
-
-        self._observables = {} if observables is None else observables
-        self._singular_values_cut = None
-        self._statevector = None
-
-    def _get_results(self):
-        """
-        Load the results on python from the output files
-        """
-
-        assert (
-            self._from_simulation
-        ), "Cannot retrieve results if no input parameters are provided"
-
-        if self._observables is not None:
-            self._observables = self._observables.read(
-                self._input_params["settings%observables_filename"],
-                self.outPATH,
-                {},
-            )
-
-            tensorlist = None
-            for key in self._observables.keys():
-                # The only key with the '/' is the MPS state
-                if "/" in key:
-                    tensorlist = read_mps(self._observables[key])
-            if tensorlist is not None:
-                self._observables["tn_state"] = tensorlist
-
-        self._singular_values_cut = np.loadtxt(
-            os.path.join(self.outPATH, "singular_values_cut.txt")
-        )
-
-    # ----------------------------
-    # Methods to save/load results
-    # ----------------------------
-    def save_results(self, PATH, name, README=""):
-        """Save the results in the folder PATH, creating a new subfolder named name
-
-        Parameters
-        ----------
-        PATH: str
-            path to the folder where to save the results
-        README: str, optional
-            String to save as additional README file inside the result folder.
-            Default to empty string.
-        name: str, optional
-            Name to add before the date_time information in the folder name
-
-        Returns
-        -------
-        _PATH: str
-            The PATH to the new subfolder
-        """
-        if not os.path.isdir(PATH):
-            os.makedirs(PATH)
-
-        # Create result folder
-        _PATH = os.path.join(PATH, name)
-        os.makedirs(_PATH)
-
-        # Save results
-        # Input parameters
-        np.save(os.path.join(_PATH, "input_params.npy"), self.input_params)
-        # Singular values
-        np.save(
-            os.path.join(_PATH, "singular_values_cut.npy"), self.singular_values_cut
-        )
-        # Initial state
-        np.save(os.path.join(_PATH, "initial_state.npy"), self.initial_state)
-        # Observables expectation values
-        np.save(os.path.join(_PATH, "observables.npy"), self.observables)
-        # README
-        README = self.date_time + "\n" + README
-        with open(os.path.join(_PATH, "README.txt"), "w") as RM:
-            RM.write(README)
-
-        return _PATH
-
-    def load_results(self, PATH):
-        """Load the results of a previous simulation
-
-        Parameters
-        ----------
-        PATH: str
-            PATH to the folder from which we want to load the results
-
-        Returns
-        -------
-        README: str
-            The text contained in the README file inside the folder
-        """
-        assert os.path.isdir(PATH), f"{PATH} is not an existing folder"
-
-        # Act on protected variables
-        # Input parameters
-        self._input_params = np.load(
-            os.path.join(PATH, "input_params.npy"), allow_pickle="TRUE"
-        ).item()
-        # Singular values
-        self._singular_values_cut = np.load(
-            os.path.join(PATH, "singular_values_cut.npy"), allow_pickle="TRUE"
-        )
-        # Initial state
-        self._initial_state = np.load(
-            os.path.join(PATH, "initial_state.npy"), allow_pickle="TRUE"
-        )
-        # Probabilities
-        self._observables = np.load(
-            os.path.join(PATH, "observables.npy"), allow_pickle="TRUE"
-        ).item()
-        # README
-        with open(os.path.join(PATH, "README.txt"), "r") as RM:
-            README = RM.read()
-        self._datetime = README.split("\n")[0]
-
-        return README
-
-    def set_results(self, result_dict, singvals_cut):
-        """Set the results of a simulation
-
-        Parameters
-        ----------
-        result_dict: dict
-            Dictionary of the attribute to be set
-        singvals_cut: array-like
-            Array of singular values cut through the simulation
-        """
-        self._observables = result_dict
-        self._singular_values_cut = singvals_cut
-
-        tensorlist = None
-        for key in result_dict.keys():
-            # The only key with the '/' is the MPS state
-            if "/" in key:
-                tensorlist = read_mps(result_dict[key])
-        if tensorlist is not None:
-            self._observables["tn_state"] = tensorlist
-
-    # -----------------------------
-    # Methods to access the results
-    # -----------------------------
-    @property
-    def fidelity(self):
-        """
-        Return the lower bound for the fidelity of the simulation,
-        using the method described in
-        If you are interested in the evolution of the fidelity through
-        the simulation compute it yourself using `np.cumprod(1-self.singular_values_cut)`.
-
-        Returns
-        -------
-        float
-            fidelity of the final state
-        """
-
-        fid = np.prod(1 - np.array(self.singular_values_cut))
-        return fid
-
-    @property
-    def measures(self):
-        """Obtain the measures of the simulation as a dictionary.
-        The keys are the measured states, the values the number of occurrencies
-
-        Returns
-        -------
-        measures: dict
-            Measures of the simulation
-        """
-        if "projective_measurements" in self.observables.keys():
-            measures = self.observables["projective_measurements"]
-        else:
-            measures = None
-        return measures
-
-    @property
-    def statevector(self):
-        """Obtain the statevector as a complex numpy array
-
-        Returns
-        -------
-        statevector: np.array or None
-            The statevector of the simulation
-        """
-        if self._statevector is None:
-            if "tn_state" in self.observables.keys():
-                tensor_list = self.observables["tn_state"]
-                if isinstance(tensor_list[0], list):
-                    tn_state = TTN.from_tensor_list(tensor_list)
-                else:
-                    tn_state = MPS.from_tensor_list(tensor_list)
-                if tn_state.num_sites < 30:
-                    self._statevector = tn_state.to_statevector(qiskit_order=True)
-        return self._statevector
-
-    @property
-    def singular_values_cut(self):
-        """Obtain the singular values cutted through the simulation, depending on the mode
-        chosen. If 'M' for maximum (default), 'C' for cumulated.
-
-        Returns
-        -------
-        singular_values_cut: np.array
-            Singular values cut during the simulation
-        """
-        return self._singular_values_cut
-
-    @property
-    def computational_time(self):
-        """Obtain the computational time of the simulation
-
-        Returns
-        -------
-        computational_time: double
-            computational time of the simulation
-        """
-        if "time" in self.observables.keys():
-            time = self.observables["time"]
-        else:
-            time = None
-        return time
-
-    @property
-    def entanglement(self):
-        """Obtain the bond entanglement entropy measured along each bond of the MPS at
-        the end of the simulation
-
-        Returns
-        -------
-        entanglement: dict or None
-            Bond entanglement entropy
-        """
-        if "bond_entropy" in self.observables.keys():
-            entanglement = self.observables["bond_entropy"]
-        elif "bond_entropy0" in self.observables.keys():
-            entanglement = self.observables["bond_entropy0"]
-        else:
-            entanglement = None
-        return entanglement
-
-    @property
-    def measure_probabilities(self):
-        """Return the probability of measuring a given state, which is computed using a
-        binary tree by eliminating all the branches with probability under a certain threshold.
-
-        Returns
-        -------
-        measure_probabilities: dict or None
-            probability of measuring a certain state if it is greater than a threshold
-        """
-        keys = ["unbiased_probability", "even_probability", "greedy_probability"]
-        probs = []
-        for key in keys:
-            if key in self.observables.keys():
-                probs += [self.observables[key]]
-            else:
-                probs += [None]
-        return probs
-
-    @property
-    def date_time(self):
-        """Obtain the starting date and time of the simulation, in the format
-        ``Year-month-day-Hour:Minute:Second``
-
-        Returns
-        -------
-        datetime: string
-            The date-time when the simulation started
-        """
-        return self._datetime
-
-    @property
-    def input_params(self):
-        """Obtain the input parameters used in the simulation, which are the following:
-            - 'num_sites',              number of sites of the mps
-            - 'local_dim',              local dimension of the single site
-            - 'max_bond_dim',           maximum bond dimension of the mps
-            - 'cut_ratio',              cut ration used in the SVD truncation
-            - 'in_name',                path to the fortran input folder
-            - 'out_name',               path to the Fortran output folder
-            - 'trunc_tracking_mode',           mode to save the singular values cut
-            - 'sparse',                 if the input gate tensors are saved as sparse
-            - 'par_approach',           parallel approach of the simulation. Can be
-                'SR' (serial), 'MW' (master/workers) or 'CT' (cartesian)
-            - 'initial_state',          initial state of the simulation. 'Vacuum' or
-                the PATH to the initial state
-            - 'do_observables',         True if there are some observables to compute at
-                the end
-
-        Returns
-        -------
-        input_params: dict or None
-            Input parameters
-        """
-        return self._input_params
-
-    @property
-    def tens_net(self):
-        """
-        Returns the tensor list in row-major format.
-        The indexing of the single tensor is as follows:
-
-        .. code-block::
-
-            1-o-3
-             2|
-
-        Returns
-        -------
-        mps: list
-            list of np.array tensors
-        """
-        if "tn_state" in self.observables.keys():
-            tn_state = self.observables["tn_state"]
-        else:
-            tn_state = None
-        return tn_state
-
-    @property
-    def initial_state(self):
-        """Returns the initial state of the simulation, as an MPS in row-major format or as
-        a string if starting from the Vacuum state
-
-        Returns
-        -------
-        initial_state: list or str
-            list of np.array tensors or Vacuum
-        """
-        return self._initial_state
-
-    @property
-    def observables(self):
-        """Returns the expectation values of the observables as a dict with the format
-            observable_name : observable_expectation_value
-
-        Returns
-        -------
-        observables: dict or None
-            Expectation values of the observables
-        """
-        return self._observables
-
-
 class QCCheckpoints:
     """
     Class to handle checkpoint parameters
 
     Parameters
     ----------
     PATH: str, optional
         PATH to the checkpoint directory. Default `data/checkpoints/`.
     frequency: float, optional
         Decide the frequency, in **hours**, of the checkpoints.
         If negative no checkpoints are present. Default to -1.
     input_nml: str, optional
         Name of the input namelist. Default 'input.nml'
+    restart: int, optional
+        If an int is provided, it is the checkpoint counter from which the user wants to restart.
+        Default to None.
     """
 
-    def __init__(self, PATH="data/checkoints/", frequency=-1, input_nml="input.nml"):
+    def __init__(
+        self,
+        PATH="data/checkpoints/",
+        frequency=-1,
+        input_nml="input.nml",
+        restart=None,
+    ):
         self._PATH = PATH if (PATH.endswith("/")) else PATH + "/"
         self._frequency = frequency
         self._input_nml = input_nml
+        self.restart = restart
+        self._checkpoint_cnt = 0
+        self._initial_line = 0
+        self._initial_time = -1
 
     def set_up(
         self,
         input_dict,
         operators=QCOperators(),
         observables=TNObservables(),
-        circ_str="",
+        circ="",
     ):
         """Set up the checkpoints directory
 
         Parameters
         ----------
         input_dict : dict
             Input parameter dictionary
         operators : :py:class:`QCOperators`, optional
             Tensor operators
         obervables : :py:class: `TNObservables`, optional
             Tensor observables
-        circ_str: str
-            circuit string
+        circ_str: str or QuantumCircuit
+            String representing the quantum circuit (fortran) or
+            the qiskit quantum circuit (python)
         """
         if not isinstance(operators, QCOperators):
             raise TypeError("Operators must be QCOperators type")
         elif not isinstance(observables, TNObservables):
             raise TypeError("observables must be TNObservables type")
 
         if not os.path.isdir(self.PATH):
@@ -627,16 +188,26 @@
 
         # Write files that can be already written
         with open(os.path.join(self.PATH, "observables.pk"), "wb") as fh:
             pickle.dump(observables, fh)
         _, operator_mapping = operators.write_input_3(self.PATH)
         observables.write(self.PATH, {}, operator_mapping)
         write_nml("INPUT", input_dict, os.path.join(self.PATH, self.input_nml))
-        with open(os.path.join(self.PATH, "circuit.dat"), "w") as fh:
-            fh.write(circ_str)
+
+        # We save extra infos for checkpoints, i.e. the quantum circuit
+        if isinstance(circ, str):
+            with open(os.path.join(self.PATH, "circuit.dat"), "w") as fh:
+                fh.write(circ)
+        elif isinstance(circ, QuantumCircuit):
+            with open(os.path.join(self.PATH, "circuit.qpy"), "wb") as fd:
+                qpy_serialization.dump(circ, fd)
+        else:
+            raise ValueError(f"Impossible to handle circuit of type {type(circ)}")
+
+        self._initial_time = time.time()
 
     @property
     def PATH(self):
         """PATH property"""
         return self._PATH
 
     @property
@@ -645,31 +216,130 @@
         return self._frequency
 
     @property
     def input_nml(self):
         """Input namelist property"""
         return self._input_nml
 
+    def save_checkpoint(self, operation_idx, emulator):
+        """
+        Save the state for the checkpoint if the
+        `operation_idx` exceeded the frequency of the
+        checkpoints
+
+        Parameters
+        ----------
+        operation_idx : int
+            Index of the current operation in the quantum circuit
+        emulator: _AbstractTN
+            Tensor network class
+
+        Returns
+        -------
+        None
+        """
+        elapsed_time = (time.time() - self._initial_time) / 3600
+        if elapsed_time > self.frequency > 0:
+            dir_path = os.path.join(self.PATH, str(self._checkpoint_cnt))
+
+            # Create directory if not accessible
+            if not os.path.isdir(dir_path):
+                os.makedirs(dir_path)
+
+            # Save the TN state on file.
+            file_path = os.path.join(dir_path, "tn_state.npy")
+            tensor_list = emulator.to_tensor_list()
+            np.save(file_path, np.array(tensor_list, dtype=object), allow_pickle=True)
+
+            # Save the index of the line on file
+            # The +1 is because that operation has already been applied
+            with open(os.path.join(dir_path, "index.txt"), "w") as fh:
+                fh.write(str(operation_idx + 1))
+
+            # Update the counter
+            self._checkpoint_cnt += 1
+
+            # Restart the countdown to the next checkpoint
+            self._initial_time = time.time()
+
+    def restart_from_checkpoint(self, initial_state):
+        """
+        Restart from the checkpoint passed in the initialization. Python only.
+
+        Parameters
+        ----------
+        initial_state: str | List[Tensors] | _AbstractTN
+            The initial state of the simulation. Might be overwritten on exit.
+
+        Returns
+        -------
+        str | List[Tensors] | _AbstractTN
+            The new initial state. If `self.restart` is None, it is the old
+            initial state.
+        """
+        # Default value, no restart was requested
+        if self.restart is None:
+            return initial_state
+
+        # If the value is -1, restart from the last one
+        if self.restart == -1:
+            self.restart = 0
+            while os.path.isdir(os.path.join(self.PATH, str(self.restart))):
+                self.restart += 1
+            self.restart -= 1
+
+        dir_path = os.path.join(self.PATH, str(self.restart))
+
+        # Save the index of the line on file
+        with open(os.path.join(dir_path, "index.txt"), "r") as fh:
+            self._initial_line = int(fh.read())
+
+        # Read the TN state
+        initial_state = np.load(
+            os.path.join(dir_path, "tn_state.npy"), allow_pickle=True
+        )
+
+        return initial_state
+
     def to_dict(self):
         """Return the ordered dictionary of the properties of
-        the class
+        the class for fortran
 
         Returns
         -------
         dictionary: OrderedDict
             Ordered dictionary of the class properties
         """
         dictionary = OrderedDict()
 
         dictionary["checkpoint_PATH"] = self.PATH
         dictionary["checkpoint_frequency"] = self.frequency
         dictionary["initial_line"] = 1
 
         return dictionary
 
+    def to_json(self, path):
+        """
+        Write the class as a json on file
+        """
+        path = os.path.join(path, "checkpoints.json")
+        with open(path, "w") as fp:
+            json.dump(self.to_dict(), fp, indent=4)
+
+    @classmethod
+    def from_json(cls, path):
+        """
+        Initialize the class from a json file
+        """
+        path = os.path.join(path, "checkpoints.json")
+        with open(path, "r") as fp:
+            dictionary = json.load(fp)[0]
+
+        return cls(**dictionary)
+
 
 class QCIO:
     """
     Class to handle Input/Output parameters
 
     Parameters
     ----------
@@ -691,14 +361,16 @@
         inPATH/initial_state.dat. If 'Vacuum' start from |000...0>. Default to 'Vacuum'.
         If a PATH it is a PATH to a saved MPS.
     sparse: bool, optional
         Weather to write operators in a semi-sparse format or not.
         Default to False
     """
 
+    initial_states_keywords = ("vacuum", "random")
+
     def __init__(
         self,
         inPATH="data/in/",
         outPATH="data/out/",
         input_namelist="input.nml",
         exe_file=None,
         initial_state="Vacuum",
@@ -715,43 +387,67 @@
         elif isinstance(exe_file, str):
             self._exe_file = [exe_file]
         else:
             self._exe_file = exe_file
         self._sparse = sparse
         self._initial_state = initial_state
 
-    def setup(self):
-        """Setup the io files"""
+    def setup(self, fortran=False):
+        """
+        Setup the io files
+
+        Parameters
+        ----------
+        fortran: bool, optional
+            If True, the simulation will be run by fortran.
+            Default to False.
+        """
 
         # Directories
         if not os.path.isdir(self.inPATH):
             os.makedirs(self.inPATH)
         if not os.path.isdir(self.outPATH):
             os.makedirs(self.outPATH)
 
-        # Executable
+        # Executable. Not used for python simulations
         if self.exe_file[-1] != os.path.join(self.inPATH, self.input_namelist):
             self._exe_file += [os.path.join(self.inPATH, self.input_namelist)]
 
         # Initial state
-        if self.initial_state != "Vacuum":
-            if isinstance(self.initial_state, str):
+
+        # First, check if it is a string.
+        if isinstance(self.initial_state, str):
+            if self.initial_state.lower() not in self.initial_states_keywords:
                 # Handle the string case assuming it is a path
                 if not os.path.isfile(self.initial_state):
                     raise Exception("Path to input file does not exist.")
-                else:
+
+                # Move it to the input folder if fortran is involved
+                if fortran:
                     new_path = os.path.join(
                         self.inPATH, os.path.basename(self.initial_state)
                     )
-                    if not os.path.samefile(self._initial_state, new_path):
-                        shutil.move(self.initial_state, new_path)
-                        self._initial_state = os.path.basename(self.initial_state)
+                    shutil.copy(self.initial_state, new_path)
+                    self._initial_state = os.path.basename(self.initial_state)
+        else:
+            # Assume it is an _AbstractTN that we can write in a formatted way
+            if hasattr(self.initial_state, "write"):
+                self.initial_state.write(os.path.join(self.inPATH, "initial_state"))
+            elif hasattr(self.initial_state, "save_pickle"):
+                self.initial_state.save_pickle(
+                    os.path.join(self.inPATH, "initial_state")
+                )
+            # Assume it is a list and use numpy save
             else:
-                # Assume it is an MPS that we can write
-                self.initial_state.write(os.path.join(self.inPATH, "initial_state.dat"))
+                np.save(
+                    os.path.join(self.inPATH, "initial_state"),
+                    np.array(self.initial_state, dtype=object),
+                    allow_pickle=True,
+                )
+            if fortran:
                 self._initial_state = "initial_state.dat"
 
     @property
     def inPATH(self):
         """Input PATH property"""
         return self._inPATH
 
@@ -785,44 +481,65 @@
         """Initial state property"""
         return self._initial_state
 
     # @initial_state.setter
     def set_initial_state(self, initial_state):
         """Modify the initial state property"""
         if not isinstance(initial_state, str):
-            if not isinstance(initial_state, MPS):
+            if not isinstance(initial_state, _AbstractTN):
                 raise TypeError(
-                    "A non-str initial state must be initialized as MPS class"
+                    "A non-str initial state must be initialized as an _AbstractTN class"
                 )
         self._initial_state = initial_state
 
     # @exe_file setter
     def set_exe_file(self, exe_file):
         """Modify exe file"""
         if not isinstance(exe_file, list):
             raise TypeError(f"exe_file must be a list of strings, not {type(exe_file)}")
         self._exe_file = exe_file
 
     def to_dict(self):
         """Return the ordered dictionary of the properties of
-        the class
+        the class for fortran
 
         Returns
         -------
         dictionary: OrderedDict
             Ordered dictionary of the class properties
         """
         dictionary = OrderedDict()
         for prop, value in vars(self).items():
             if prop in ("_exe_file", "_input_namelist"):
                 continue
+            if prop == "_initial_state" and not isinstance(value, str):
+                value = "initial_state.dat"
             dictionary[prop[1:]] = value
 
         return dictionary
 
+    def to_json(self, path):
+        """
+        Write the class as a json on file
+        """
+        path = os.path.join(path, "io_info.json")
+        with open(path, "w") as fp:
+            json.dump(self.to_dict(), fp, indent=4)
+
+    @classmethod
+    def from_json(cls, path):
+        """
+        Initialize the class from a json file
+        """
+        path = os.path.join(path, "io_info.json")
+        with open(path, "r") as fp:
+            dictionary = json.load(fp)[0]
+
+        return cls(**dictionary)
+
 
 class QCConvergenceParameters(TNConvergenceParameters):
     """Convergence parameter class, inhereting from the
     more general Tensor Network type. Here the convergence
     parameters are only the bond dimension and the cut ratio.
 
     Parameters
@@ -831,34 +548,49 @@
         Maximum bond dimension of the problem. Default to 10.
     cut_ratio : float, optional
         Cut ratio for singular values. If :math:`\\lambda_n/\\lambda_1 <` cut_ratio then
         :math:`\\lambda_n` is neglected. Default to 1e-9.
     trunc_tracking_mode : str, optional
         Modus for storing truncation, 'M' for maximum, 'C' for
         cumulated (default).
+    svd_ctrl : character, optional
+        Control for the SVD algorithm. Available:
+        - "A" : automatic. Some heuristic is run to choose the best mode for the algorithm.
+                The heuristic can be seen in qtealeaves/tensors/tensors.py
+                in the function _process_svd_ctrl.
+        - "V" : gesvd. Safe but slow method. Recommended in Fortran simulation
+        - "D" : gesdd. Fast iterative method. It might fail. Resort to gesvd if it fails
+        - "E" : eigenvalue decomposition method. Faster on GPU. Available only when
+                contracting the singular value to left or right
+        - "X" : sparse eigenvalue decomposition method. Used when you reach the maximum
+                bond dimension. Only python.
+        - "R" : random svd method. Used when you reach the maximum bond dimension.
+                Only python.
+        Default to 'A'.
+    ini_bond_dimension: int, optional
+        Initial bond dimension of the simulation. It is used if the initial state is random.
+        Default to 1.
 
     """
 
     def __init__(
         self,
         max_bond_dimension=10,
         cut_ratio=1e-9,
         trunc_tracking_mode="C",
-        singval_mode=None,
+        svd_ctrl="A",
+        ini_bond_dimension=1,
     ):
-        if singval_mode is not None:
-            warn(
-                "singval_mode parameter is deprecated. Please use trunc_tracking_mode instead"
-            )
-            trunc_tracking_mode = singval_mode
         TNConvergenceParameters.__init__(
             self,
             max_bond_dimension=max_bond_dimension,
             cut_ratio=cut_ratio,
             trunc_tracking_mode=trunc_tracking_mode,
+            svd_ctrl=svd_ctrl,
+            ini_bond_dimension=ini_bond_dimension,
         )
 
     def to_dict(self):
         """Return the ordered dictionary of the properties of
         the class
 
         Returns
@@ -869,129 +601,288 @@
         dictionary = OrderedDict()
         dictionary["max_bond_dimension"] = self.max_bond_dimension
         dictionary["cut_ratio"] = self.cut_ratio
         dictionary["trunc_tracking_mode"] = self.trunc_tracking_mode
 
         return dictionary
 
+    def pretty_print(self):
+        """
+        Print the convergence parameters.
+        (Implemented to avoid too few public methods)
+        """
+        print("-" * 50)
+        print(
+            "-" * 10 + f" Maximum bond dimension: {self.max_bond_dimension} " + "-" * 10
+        )
+        print("-" * 10 + f" Cut ratio: {self.cut_ratio} " + "-" * 10)
+        print(
+            "-" * 10
+            + f" Truncation tracking mode: {self.trunc_tracking_mode} "
+            + "-" * 10
+        )
+        print("-" * 50)
+
+    def to_json(self, path):
+        """
+        Write the class as a json on file
+        """
+        path = os.path.join(path, "convergence_parameters.json")
+        with open(path, "w") as fp:
+            dictionary = self.to_dict()
+            dictionary["svd_ctrl"] = self.svd_ctrl
+            json.dump(dictionary, fp, indent=4)
+
+    @classmethod
+    def from_json(cls, path):
+        """
+        Initialize the class from a json file
+        """
+        path = os.path.join(path, "convergence_parameters.json")
+        with open(path, "r") as fp:
+            dictionary = json.load(fp)[0]
+
+        return cls(**dictionary)
+
 
 class QCBackend:
     """
     Backend for the simulation. Contains all the informations about
     which executable you want to run
 
     Parameters
     ----------
     backend : str, optional
         First backend definition. Either "PY" (python) or "FR" (fortran).
         Default to "PY".
     precision: str, optional
-        Precision of the simulation. Either "Z" (double complex) or "C"
-        (single complex). Default to "Z".
+        Precision of the simulation.
+        Select a real precision ONLY if you use ONLY real gates.
+        Available:
+        - "A": automatic. For the heuristic see `self.resolve_precision`.
+        - "Z": double precision complex;
+        - "C": single precision complex;
+        - "D": double precision real;
+        - "S": single precision real.
+        Default to "A".
     device: str, optional
-        Device of the simulation. Either "cpu" or "gpu". Default to "cpu".
-    num_procs: int, optional
-        Number of processes for the MPI simulation. Default to 1.
-    mpi_approach: str, optional
-        Approach for the MPI simulation. Either "MW", "CT" or "SR".
-        Default to "SR".
+        Device of the simulation.
+        Available:
+        - "A" : automatic. For the heuristic see `self.resolve_device`
+        - "cpu": use the cpu
+        - "gpu": use the gpu if it is available
+        Defailt to "A"
     ansatz : str, optional
         Weather to run the circuit with MPS or TTN tensor network ansatz.
         Default to "MPS".
+    mpi_settings : MPISettings | None, optional
+        Settings for running the simulation multi-node.
+        Default to None, i.e. no MPI.
     """
 
     def __init__(
         self,
         backend="PY",
-        precision="Z",
+        precision="A",
         device="cpu",
-        num_procs=1,
-        mpi_approach="SR",
         ansatz="MPS",
+        mpi_settings=None,
     ):
-        if backend == "PY" and mpi_approach != "SR":
-            raise ValueError("Only serial simulation available in python")
         if backend == "FR" and device == "gpu" and precision == "C":
             raise ValueError(
                 "Only double precision complex available "
                 + "in fortran with the GPU device"
             )
-        if num_procs == 1:
-            mpi_approach = "SR"
 
         self._backend = backend.upper()
         self._precision = precision.upper()
         self._device = device
-        self._num_procs = num_procs
-        self._mpi_approach = mpi_approach.upper()
         if backend == "FR" and ansatz.upper() != "MPS":
             warn(
                 f"Only MPS ansatz available on fortran simulation, not {ansatz}."
                 + "The ansatz is set back to MPS."
             )
             ansatz = "MPS"
         self._ansatz = ansatz.upper()
+        self.mpi_settings = MPISettings() if mpi_settings is None else mpi_settings
 
     def to_dict(self):
         """
         Map the backend to a dictionary for fortran
         """
         dictionary = OrderedDict({})
-        mpi = "T" if self._num_procs > 1 else "F"
+        mpi = "T" if self.num_procs > 1 else "F"
         gpu = "T" if self.device == "gpu" else "F"
         dictionary["simulation_mode"] = self.precision + mpi + gpu
         dictionary["approach"] = self.mpi_approach
         # dictionary["ansatz"] = self.ansatz
 
         return dictionary
 
+    def resolve_precision(self, min_fidelity, tol=1e-7):
+        """
+        Resolve the precision of the simulation.
+        Heuristic if `self._precision=`"A"`.
+
+        Parameters
+        ----------
+        min_fidelity: float
+            Lower bound of the fidelity of the simulation at the moment
+        tol: float, optional
+            Tolerance after which you switch to single precision.
+            Default to 1e-7
+
+        Returns
+        -------
+        str
+            The selected precision
+        """
+        if self._precision != "A":
+            return self.precision
+
+        # For fortran, automatic means Z
+        if self.backend == "FR":
+            return "Z"
+
+        # The lower bound of the fidelity of our state is
+        # below the number of digits of a single
+        # precision
+        if 1 - min_fidelity > tol:
+            return "C"
+
+        return "Z"
+
+    def resolve_device(self, bond_dimension, previous_device, exp_gpu=7):
+        """
+        Resolve the device if it set on automatic.
+
+        Parameters
+        ----------
+        bond_dimension : int
+            Maximum bond dimension of the system
+        previous_device : str
+            Device where the system is currently. This is used
+            to ensure we do not keep exchanging data back and
+            forth.
+        exp_gpu : int, optional
+            Exponent of the bond dimension after which you switch
+            to the gpu, i.e:
+            - if chi >= 2**exp_gpu -> use gpu
+            - if chi <= 2**(exp_gpu-1) -> use cpu
+            Default to 7. (switch at 128)
+
+        Returns
+        -------
+        str
+            Device where to move (or keep) the system
+        """
+        if self._device != "A":
+            if self._device == "cgpu":
+                return "cpu"
+            return self._device
+
+        # For fortran, automatic means cpu
+        if self.backend == "FR":
+            return "cpu"
+
+        if bond_dimension >= 2**exp_gpu and GPU_AVAILABLE:
+            return "gpu"
+        # The condition on the CPU is here because we want
+        # to avoid keep exchanging informations if the bond
+        # dimension oscillates between 129 and 120
+        if bond_dimension <= 2 ** (exp_gpu - 1):
+            return "cpu"
+
+        return previous_device
+
     @property
     def backend(self):
         """Backend property"""
         return self._backend
 
     @property
     def precision(self):
         """Precision property"""
+        # For fortran, automatic means Z
+        if self.backend == "FR":
+            return "Z"
         return self._precision
 
     @property
     def device(self):
         """Device property"""
+        # For fortran, automatic means cpu
+        if self.backend == "FR":
+            return "cpu"
         return self._device
 
     @property
     def num_procs(self):
         """Number of processes property"""
-        return self._num_procs
+        return self.mpi_settings.num_procs
 
     @property
     def mpi_approach(self):
         """mpi_approach property"""
-        return self._mpi_approach
+        return self.mpi_settings.mpi_approach.upper()
 
     @property
     def ansatz(self):
         """ansatz property"""
         return self._ansatz
 
     @property
+    def mpi_command(self):
+        """mpi_command property"""
+        return self.mpi_settings.mpi_command
+
+    @property
     def identifier(self):
         """Identifier combining all properties."""
         return ":".join(
             [
                 self.backend,
-                self.precision,
-                self.device,
+                self.resolve_precision(1),
+                self.resolve_device(1, "cpu"),
                 str(self.num_procs),
                 self.mpi_approach,
                 self.ansatz,
             ]
         )
 
+    def to_json(self, path):
+        """
+        Write the class as a json on file as
+        backend.json in the flder path
+        """
+        path = os.path.join(path, "backend.json")
+        dictionary = OrderedDict()
+        dictionary["backend"] = self.backend
+        dictionary["device"] = self.device
+        dictionary["precision"] = self.precision
+        dictionary["num_procs"] = self.num_procs
+        dictionary["ansatz"] = self.ansatz
+        dictionary["mpi_approach"] = self.mpi_approach
+        dictionary["mpi_command"] = self.mpi_command
+
+        with open(path, "w") as fp:
+            json.dump(dictionary, fp, indent=4)
+
+    @classmethod
+    def from_json(cls, path):
+        """
+        Initialize the class from a json file called
+        "backend.json" in the folder path
+        """
+        path = os.path.join(path, "backend.json")
+        with open(path, "r") as fp:
+            dictionary = json.load(fp)[0]
+
+        return cls(**dictionary)
+
 
 def merge_ordered_dicts(dicts):
     """Merge ordered dicts together, concatenating them in the order provided in the list
 
     Parameters
     ----------
     dicts : list of OrderedDict
```

### Comparing `qmatchatea-0.5.2/qmatchatea.egg-info/PKG-INFO` & `qmatchatea-1.1.0/qmatchatea.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: qmatchatea
-Version: 0.5.2
+Version: 1.1.0
 Summary: Quantum matcha TEA python library for tensor network emulation of quantum circuits.
 Home-page: https://baltig.infn.it/quantum_matcha_tea/py_api_quantum_matcha_tea
 Author: Marco Ballarin
 Author-email: marco97.ballarin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: matplotlib>=3.1.3
-Requires-Dist: qtealeaves<0.5.0,>=0.4.54
+Requires-Dist: qtealeaves>=1.1.4
 Requires-Dist: qiskit==0.38.0
 Requires-Dist: mpi4py
 Requires-Dist: joblib
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
```

### Comparing `qmatchatea-0.5.2/qmatchatea.egg-info/SOURCES.txt` & `qmatchatea-1.1.0/qmatchatea.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 LICENSE
 NOTICE
 README.md
 setup.py
 qmatchatea/__init__.py
 qmatchatea/interface.py
-qmatchatea/mpi_utils.py
 qmatchatea/par_simulations.py
 qmatchatea/preprocessing.py
 qmatchatea/py_emulator.py
-qmatchatea/qk_utils.py
-qmatchatea/sf_utils.py
 qmatchatea/tensor_compiler.py
-qmatchatea/tn_utils.py
-qmatchatea/utils.py
 qmatchatea/version.py
 qmatchatea.egg-info/PKG-INFO
 qmatchatea.egg-info/SOURCES.txt
 qmatchatea.egg-info/dependency_links.txt
 qmatchatea.egg-info/requires.txt
 qmatchatea.egg-info/top_level.txt
 qmatchatea/circuit/__init__.py
 qmatchatea/circuit/circuit.py
 qmatchatea/circuit/observables.py
 qmatchatea/circuit/operations.py
-tests/test_examples.py
-tests/test_qcircuit.py
-tests/test_tensor_compiler.py
+qmatchatea/utils/__init__.py
+qmatchatea/utils/mpi_utils.py
+qmatchatea/utils/qk_utils.py
+qmatchatea/utils/sf_utils.py
+qmatchatea/utils/simulation_results.py
+qmatchatea/utils/tn_utils.py
+qmatchatea/utils/utils.py
 tests/tests_basic_circuits.py
+tests/tests_examples.py
 tests/tests_formatting.py
 tests/tests_linter.py
 tests/tests_mpi4py.py
-tests/tests_observables.py
+tests/tests_observables.py
+tests/tests_qcircuit.py
+tests/tests_tensor_compiler.py
```

### Comparing `qmatchatea-0.5.2/setup.py` & `qmatchatea-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 else:
     install_requires = []
 
 install_requires = [
     "numpy>=1.18.1",
     "scipy>=1.4.1",
     "matplotlib>=3.1.3",
-    "qtealeaves>=0.4.54,<0.5.0",
+    "qtealeaves>=1.1.4",
     "qiskit==0.38.0",
     "mpi4py",
     "joblib",
 ]
 
 # Get the readme file
 if os.path.isfile("README.md"):
@@ -57,16 +57,17 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     package_dir={
         "qmatchatea": "qmatchatea",
         "qmatchatea.circuit": "qmatchatea/circuit",
+        "qmatchatea.utils": "qmatchatea/utils",
     },
-    packages=["qmatchatea", "qmatchatea.circuit"],
+    packages=["qmatchatea", "qmatchatea.circuit", "qmatchatea.utils"],
     python_requires=">=3.8",
     install_requires=install_requires,
     # entry_points = { 'console_scripts': ['build_exec = qmatchatea.bin.compiler:main', ], },
     # These packages are not mandatory for a pip installation. If they are not there
     # they will simply be ignored.
     package_data={"qmatchatea": ["bin/qmatchatea.exe", "bin/par_qmatchatea.exe"]},
 )
```

### Comparing `qmatchatea-0.5.2/tests/test_qcircuit.py` & `qmatchatea-1.1.0/tests/tests_qcircuit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,30 @@
+# This code is part of qmatchatea.
+#
+# This code is licensed under the Apache License, Version 2.0. You may
+# obtain a copy of this license in the LICENSE.txt file in the root directory
+# of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
+#
+# Any modifications or derivative works of this code must retain this
+# copyright notice, and modified files need to carry a notice indicating
+# that they have been altered from the originals.
+
 import unittest
 from qmatchatea.circuit import Qcircuit
 from qmatchatea.circuit import observables
 from qmatchatea.circuit.observables import QCObservableStep
 from qiskit import QuantumCircuit, execute
 from qiskit_aer.aerprovider import AerSimulator
 import numpy as np
 
 import qtealeaves.observables as obs
 from qmatchatea.circuit.operations import QCZpauli
 from qmatchatea.py_emulator import QCEmulator
-from qmatchatea.tn_utils import QCOperators
+from qmatchatea.utils.tn_utils import QCOperators
+from qmatchatea import run_simulation
 
 
 class TestQcircuit(unittest.TestCase):
     """Test basic feature of Qcircuit without simulations"""
 
     def setUp(self):
         """Define 'global' variables"""
@@ -151,15 +162,15 @@
 
         qc.measure_observables("step1", obsv, ops, "default")
 
         qc.add_qregister("new", [0])
         qc.x(0, qreg="new")
         qc.measure_observables("step2", obsv, ops)
 
-        results = sim.run_from_qcirc(qc)
+        _, results, _ = sim.run_from_qcirc(qc)
 
         step1_res = results["step1"]["sz"]["default"]
         step2_res = results["step2"]
 
         expected = np.zeros(4)
 
         self.assertTrue(
@@ -172,23 +183,23 @@
         self.assertTrue(conds, "Local measurement on multiple" + " registers correct")
 
     def test_projective(self):
         """test projective observables"""
         qc, obsv, ops = self._make_ghz()
         sim = QCEmulator(self.num_sites)
 
-        obsv += obs.TNObsProjective(1024)
+        obsv += obs.TNObsProjective(1024, True)
 
         qc.measure_observables("step1", obsv, ops, "default")
 
         qc.add_qregister("new", [0])
         qc.x(0, qreg="new")
         qc.measure_observables("step2", obsv, ops)
 
-        results = sim.run_from_qcirc(qc)
+        _, results, _ = sim.run_from_qcirc(qc)
 
         step1_res = results["step1"]["projective_measurements"]["default"]
         step2_res = results["step2"]["projective_measurements"]["new"]
 
         self.assertIn(
             "1111", step1_res, "Projective measurement on single" + " register correct"
         )
@@ -214,22 +225,24 @@
 
             qc.measure_observables("step1", obsv, ops, "default")
 
             qc.add_qregister("new", [0])
             qc.x(0, qreg="new")
             qc.measure_observables("step2", obsv, ops)
 
-            results = sim.run_from_qcirc(qc)
+            _, results, _ = sim.run_from_qcirc(qc)
 
             step1_res = results["step1"][pn]["default"]
-            step2_res = results["step2"][pn]["new"]["1"]
+            step2_res = results["step2"][pn]["new"]
 
             if pn == "unbiased_probability":
-                temp = step2_res[1] - step2_res[0]
-                step2_res = temp + step2_res[3] - step2_res[2]
+                step2_res["1"] = step2_res["1"][1] - step2_res["1"][0]
+                step2_res["0"] = step2_res["0"][1] - step2_res["0"][0]
+
+            step2_res = np.sum(list(step2_res.values()))
 
             self.assertIn(
                 "1111",
                 step1_res,
                 pb + " probability measurement on single" + " register correct",
             )
 
@@ -247,16 +260,15 @@
         obsv += obs.TNObsBondEntropy()
 
         qc.add_qregister("new", [0])
         qc.x(0, qreg="new")
         qc.cx([0, 0], qreg=["new", "default"])
         qc.measure_observables("step1", obsv, ops)
 
-        results = sim.run_from_qcirc(qc)
-
+        _, results, _ = sim.run_from_qcirc(qc)
         bd = results["step1"]["bond_entropy"]
 
         res = np.array(list(bd.values()))[1:]
 
         self.assertAlmostEqual(bd[(0, 1)], 0, msg="No entanglement in tensor product")
         self.assertTrue(
             (res == 0.6931471805599454).all(),
@@ -270,15 +282,15 @@
         obsv += obs.TNObsTensorProduct("sz", "sz", 1)
         ops.ops["sz"] = self.sz
 
         qc.add_qregister("new", [0])
         qc.x(0, qreg="new")
         qc.measure_observables("step1", obsv, ops, qreg="new")
 
-        results = sim.run_from_qcirc(qc)
+        _, results, _ = sim.run_from_qcirc(qc)
 
         step2_res = np.real(results["step1"]["sz"])
 
         self.assertAlmostEqual(
             step2_res, -1, msg="Tensor product operator correctly broadcasted"
         )
 
@@ -293,14 +305,14 @@
         ops.ops["sz"] = self.sz
         ops.ops["id"] = np.eye(2)
 
         qc.add_qregister("new", [0, 0])
         qc.x(0, qreg="new")
         qc.measure_observables("step1", obsv, ops, qreg="new")
 
-        results = sim.run_from_qcirc(qc)
+        _, results, _ = sim.run_from_qcirc(qc)
 
         res = np.real(results["step1"]["szz"])
 
         self.assertAlmostEqual(
             res, 5, msg="Weighted sum operator correctly broadcasted"
         )
```

### Comparing `qmatchatea-0.5.2/tests/test_tensor_compiler.py` & `qmatchatea-1.1.0/tests/tests_tensor_compiler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,23 @@
+# This code is part of qmatchatea.
+#
+# This code is licensed under the Apache License, Version 2.0. You may
+# obtain a copy of this license in the LICENSE.txt file in the root directory
+# of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
+#
+# Any modifications or derivative works of this code must retain this
+# copyright notice, and modified files need to carry a notice indicating
+# that they have been altered from the originals.
+
 import unittest
 import sys
 import numpy as np
 
-from qmatchatea.utils import fidelity
-from qmatchatea.qk_utils import GHZ_qiskit, W_qiskit, qiskit_get_statevect
+from qmatchatea.utils.utils import fidelity
+from qmatchatea.utils.qk_utils import GHZ_qiskit, W_qiskit, qiskit_get_statevect
 from qmatchatea import tensor_compiler
 from qiskit import QuantumCircuit, transpiler, transpile
 from qiskit.circuit.library import QuantumVolume
 
 sys.argv = [""]
 avail_gates = [
     "x",
```

### Comparing `qmatchatea-0.5.2/tests/tests_basic_circuits.py` & `qmatchatea-1.1.0/tests/tests_basic_circuits.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+# This code is part of qmatchatea.
+#
+# This code is licensed under the Apache License, Version 2.0. You may
+# obtain a copy of this license in the LICENSE.txt file in the root directory
+# of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
+#
+# Any modifications or derivative works of this code must retain this
+# copyright notice, and modified files need to carry a notice indicating
+# that they have been altered from the originals.
+
 import os
 import os.path
 import unittest
 import sys
 from shutil import rmtree
 import numpy as np
 
@@ -17,21 +27,22 @@
         GPU_AVAILABLE = False
 except ImportError:
     cp = None
     GPU_AVAILABLE = False
 
 from qmatchatea import run_simulation, QCBackend
 from qmatchatea.utils import QCConvergenceParameters, fidelity, QCIO
-from qmatchatea.qk_utils import (
+from qmatchatea.utils.qk_utils import (
     GHZ_qiskit,
     W_qiskit,
     qiskit_get_statevect,
     qk_transpilation_params,
 )
-from qmatchatea.mpi_utils import to_layered_circ
+from qmatchatea.circuit import Qcircuit
+from qmatchatea.utils.mpi_utils import to_layered_circ
 from qiskit import QuantumCircuit, transpiler, transpile, ClassicalRegister
 from qiskit.circuit.library import QuantumVolume
 from qtealeaves.observables import TNObsProjective, TNObservables, TNState2File
 
 sys.argv = [""]
 avail_gates = [
     "x",
@@ -87,68 +98,56 @@
 class TestBasicCircuits(unittest.TestCase):
     def setUp(self):
         if not os.path.isdir("TMP_TEST"):
             os.makedirs("TMP_TEST")
         self.qcio = QCIO("TMP_TEST/data/in", "TMP_TEST/data/out")
         self.backends = self.get_python_backends()
         self.obs = TNObservables()
-        self.obs += TNObsProjective(1024)
+        self.obs += TNObsProjective(16)
         self.obs += TNState2File("TMP_TEST/data/out/statevector.txt", "F")
         np.random.seed(123)
 
     @staticmethod
     def get_python_backends():
         """
         Generate all possible backends for python.
         """
         backends = (
             {
                 "backend": "PY",
-                "mpi_approach": "SR",
-                "num_procs": 1,
                 "precision": "C",
                 "device": "cpu",
                 "ansatz": "MPS",
             },
             {
                 "backend": "PY",
-                "mpi_approach": "SR",
-                "num_procs": 1,
                 "precision": "Z",
                 "device": "cpu",
                 "ansatz": "MPS",
             },
             {
                 "backend": "PY",
-                "mpi_approach": "SR",
-                "num_procs": 1,
                 "precision": "C",
                 "device": "cpu",
                 "ansatz": "TTN",
             },
             {
                 "backend": "PY",
-                "mpi_approach": "SR",
-                "num_procs": 1,
                 "precision": "Z",
                 "device": "cpu",
                 "ansatz": "TTN",
             },
             {
                 "backend": "PY",
-                "mpi_approach": "SR",
-                "num_procs": 1,
                 "precision": "C",
                 "device": "gpu",
                 "ansatz": "MPS",
             },
             {
                 "backend": "PY",
-                "mpi_approach": "SR",
-                "num_procs": 1,
                 "precision": "Z",
                 "device": "gpu",
                 "ansatz": "MPS",
             },
         )
 
         if GPU_AVAILABLE:
@@ -159,52 +158,72 @@
         backends = [QCBackend(**elem) for elem in backends]
 
         return backends
 
     def tearDown(self):
         if os.path.isdir("TMP_TEST"):
             rmtree("TMP_TEST")
+        return
 
     def test_GHZ(self):
         """
         Check that the GHZ circuit is reproduced correctly
         """
         for backend in self.backends:
             num_qubits = 8
             qc = QuantumCircuit(num_qubits)
             GHZ_qiskit(qc)
             true_state = qiskit_get_statevect(qc)
             res = run_simulation(
                 qc, io_info=self.qcio, backend=backend, observables=self.obs
             )
             statevect = res.statevector
-            if backend.device == "gpu":
-                statevect = statevect.get()
             fid = fidelity(statevect, true_state)
             self.assertAlmostEqual(
                 fid, 1, places=12, msg="GHZ state not described correctly"
             )
 
         return
 
+    def test_GHZ_qcircuit(self):
+        """
+        Check that the GHZ circuit is reproduced correctly
+        """
+        num_qubits = 8
+        true_state = np.zeros(2**num_qubits)
+        true_state[[0, -1]] = 1 / np.sqrt(2)
+        for backend in self.backends:
+            qc = Qcircuit(num_qubits)
+            qc.h(0)
+            for ii in range(0, num_qubits - 1):
+                qc.cx([ii, ii + 1])
+            res = run_simulation(
+                qc, io_info=self.qcio, backend=backend, observables=self.obs
+            )
+            statevect = res.statevector
+            fid = fidelity(statevect, true_state)
+            self.assertAlmostEqual(
+                fid, 1, places=12, msg="GHZ state not described correctly with Qcircuit"
+            )
+
+        return
+
     def test_W(self):
         """
         Check that the W circuit is reproduced correctly
         """
         for backend in self.backends:
             num_qubits = 8
             qc = QuantumCircuit(num_qubits)
             W_qiskit(qc)
             true_state = qiskit_get_statevect(qc)
             res = run_simulation(
                 qc, io_info=self.qcio, backend=backend, observables=self.obs
             )
             statevect = res.statevector
-            if backend.device == "gpu":
-                statevect = statevect.get()
             fid = fidelity(statevect, true_state)
             self.assertAlmostEqual(
                 fid, 1, places=12, msg="W state not described correctly"
             )
 
         return
 
@@ -225,18 +244,16 @@
                 convergence_parameters=convergence_params,
                 io_info=self.qcio,
                 transpilation_parameters=transpilation_params,
                 backend=backend,
                 observables=self.obs,
             )
             statevect = res.statevector
-            if backend.device == "gpu":
-                statevect = statevect.get()
             fid = fidelity(statevect, true_state)
-            tol_places = 12 if (backend.precision == "Z") else 6
+            tol_places = 12 if (backend.precision == "Z") else 5
             self.assertAlmostEqual(
                 fid,
                 1,
                 places=tol_places,
                 msg=f"QVOLUME state not described correctly with {approach}.",
             )
```

### Comparing `qmatchatea-0.5.2/tests/tests_formatting.py` & `qmatchatea-1.1.0/tests/tests_formatting.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-0.5.2/tests/tests_linter.py` & `qmatchatea-1.1.0/tests/tests_linter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+# This code is part of qmatchatea.
+#
+# This code is licensed under the Apache License, Version 2.0. You may
+# obtain a copy of this license in the LICENSE.txt file in the root directory
+# of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
+#
+# Any modifications or derivative works of this code must retain this
+# copyright notice, and modified files need to carry a notice indicating
+# that they have been altered from the originals.
+
 import os
 import os.path
 import unittest
 from io import StringIO
 import pylint.lint
 from pylint.reporters.text import ParseableTextReporter
 
@@ -33,15 +43,15 @@
             "[E0611(no-name-in-module), ] No name '_TNObsBase' in module"
             + " 'qtealeaves'"
         )
         pattern_2 = "[E0401(import-error), ] Unable to import 'strawberryfields'"
         pattern_3 = "[E0401(import-error), ] Unable to import 'strawberryfields.backends.fockbackend'"
         self.default_patterns = [pattern_1, pattern_2, pattern_3]
         self.pylint_args = {
-            "good-names": "ii,jj,kk,nn,mm,fh,dx,dy,dz,dt,hh,qc,dl,gh,xp",
+            "good-names": "ii,jj,kk,nn,mm,fh,dx,dy,dz,dt,hh,qc,dl,gh,xp,PATH,inPATH,outPATH",
             "disable": "C0325,C0209,W1514,R1711,R1732"
             #'ignore_in_line' : pattern_1
         }
 
     def run_pylint(self, filename, local_settings={}):
         """
         Run linter test with our unit test settings for one specific
```

### Comparing `qmatchatea-0.5.2/tests/tests_observables.py` & `qmatchatea-1.1.0/tests/tests_observables.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+# This code is part of qmatchatea.
+#
+# This code is licensed under the Apache License, Version 2.0. You may
+# obtain a copy of this license in the LICENSE.txt file in the root directory
+# of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
+#
+# Any modifications or derivative works of this code must retain this
+# copyright notice, and modified files need to carry a notice indicating
+# that they have been altered from the originals.
+
 import os
 import os.path
 import unittest
 import sys
 from shutil import rmtree
 
 # Try to import cupy
@@ -15,19 +25,18 @@
     except CUDARuntimeError:
         GPU_AVAILABLE = False
 except ImportError:
     cp = None
     GPU_AVAILABLE = False
 
 from qmatchatea import run_simulation, QCOperators, QCBackend
-from qmatchatea.qk_utils import GHZ_qiskit, W_qiskit
+from qmatchatea.utils.qk_utils import GHZ_qiskit, W_qiskit
 from qmatchatea.utils import QCIO
 from qiskit import QuantumCircuit
 from qtealeaves.observables import TNObservables, TNObsWeightedSum, TNObsTensorProduct
-from qmatchatea.tn_utils import pauli_matrices
 
 sys.argv = [""]
 
 
 class TestObservables(unittest.TestCase):
     def setUp(self):
         if not os.path.isdir("TMP_TEST"):
@@ -39,56 +48,44 @@
     def get_python_backends():
         """
         Generate all possible backends for python.
         """
         backends = (
             {
                 "backend": "PY",
-                "mpi_approach": "SR",
-                "num_procs": 1,
                 "precision": "C",
                 "device": "cpu",
                 "ansatz": "MPS",
             },
             {
                 "backend": "PY",
-                "mpi_approach": "SR",
-                "num_procs": 1,
                 "precision": "Z",
                 "device": "cpu",
                 "ansatz": "MPS",
             },
             {
                 "backend": "PY",
-                "mpi_approach": "SR",
-                "num_procs": 1,
                 "precision": "C",
                 "device": "cpu",
                 "ansatz": "TTN",
             },
             {
                 "backend": "PY",
-                "mpi_approach": "SR",
-                "num_procs": 1,
                 "precision": "Z",
                 "device": "cpu",
                 "ansatz": "TTN",
             },
             {
                 "backend": "PY",
-                "mpi_approach": "SR",
-                "num_procs": 1,
                 "precision": "C",
                 "device": "gpu",
                 "ansatz": "MPS",
             },
             {
                 "backend": "PY",
-                "mpi_approach": "SR",
-                "num_procs": 1,
                 "precision": "Z",
                 "device": "gpu",
                 "ansatz": "MPS",
             },
         )
 
         if GPU_AVAILABLE:
@@ -129,43 +126,42 @@
             zsingle = TNObsTensorProduct("Zsingle", ["Z"], [[1]])
 
             obs += xtp
             obs += ztp
             obs += zsingle
 
             operators = QCOperators()
-            operators.ops["Z"] = pauli_matrices["Z"]
-            operators.ops["X"] = pauli_matrices["X"]
 
             res = run_simulation(
                 qc,
                 io_info=self.qcio,
                 observables=obs,
                 operators=operators,
                 backend=backend,
             )
 
             obs_res = res.observables
+            places = 12 if backend.precision in ("Z", "D") else 5
 
             self.assertAlmostEqual(
                 obs_res["Ztp"],
                 1,
-                places=12,
+                places=places,
                 msg=f"Tensor product of ZZ...Z has value 1 on even number of qubits",
             )
             self.assertAlmostEqual(
                 obs_res["Xtp"],
                 1,
-                places=12,
+                places=places,
                 msg=f"Tensor product of XX...X has value 1",
             )
             self.assertAlmostEqual(
                 obs_res["Zsingle"],
                 0,
-                places=12,
+                places=places,
                 msg=f"Single Z on second site has value 0",
             )
 
         return
 
     def test_TensorProductOnW(self):
         """
@@ -190,35 +186,37 @@
             zsingle = TNObsTensorProduct("Zsingle", ["Z"], [[1]])
 
             obs += xtp
             obs += ztp
             obs += zsingle
 
             operators = QCOperators()
-            operators.ops["Z"] = pauli_matrices["Z"]
-            operators.ops["X"] = pauli_matrices["X"]
 
             res = run_simulation(
                 qc,
                 io_info=self.qcio,
                 observables=obs,
                 operators=operators,
                 backend=backend,
             )
 
             obs_res = res.observables
 
+            places = 12 if backend.precision in ("Z", "D") else 5
             self.assertAlmostEqual(
                 obs_res["Ztp"],
                 -1,
-                places=12,
+                places=places,
                 msg="Tensor product of ZZ...Z has value 0 on even number of qubits",
             )
             self.assertAlmostEqual(
-                obs_res["Xtp"], 0, places=12, msg="Tensor product of XX...X has value 1"
+                obs_res["Xtp"],
+                0,
+                places=places,
+                msg="Tensor product of XX...X has value 1",
             )
 
         return
 
     def test_WeightedSumOnGHZ(self):
         """
         Test the evaluation of WS observables on GHZ state
@@ -236,85 +234,89 @@
             )
             xtp = TNObsTensorProduct(
                 "Xtp",
                 ["X" for i in range(num_qubits)],
                 [[i] for i in range(num_qubits)],
             )
 
-            xx = TNObsWeightedSum("X", xtp, [2])
-            zz = TNObsWeightedSum("Z", ztp, [3])
+            xx = TNObsWeightedSum("X", xtp, [2], use_itpo=False)
+            zz = TNObsWeightedSum("Z", ztp, [3], use_itpo=False)
 
             obs += xx
             obs += zz
 
             operators = QCOperators()
-            operators.ops["Z"] = pauli_matrices["Z"]
-            operators.ops["X"] = pauli_matrices["X"]
 
             res = run_simulation(
                 qc,
                 io_info=self.qcio,
                 observables=obs,
                 operators=operators,
                 backend=backend,
             )
 
             obs_res = res.observables
 
+            places = 12 if backend.precision in ("Z", "D") else 4
             self.assertAlmostEqual(
                 obs_res["Z"],
                 0,
-                places=12,
+                places=places,
                 msg="Tensor product of ZZ...Z has value 0 on odd number of qubits",
             )
             self.assertAlmostEqual(
-                obs_res["X"], 2, places=12, msg="Tensor product of XX...X is correct"
+                obs_res["X"],
+                2,
+                places=places,
+                msg="Tensor product of XX...X is correct",
             )
 
         return
 
     def test_WeightedFromPauli(self):
         """
         Test the evaluation of WS observables on GHZ state
         """
         for backend in self.backends:
+            if backend.ansatz == "MPS":
+                continue
             num_qubits = 16
             qc = QuantumCircuit(num_qubits)
             GHZ_qiskit(qc)
 
             obs = TNObservables("observables.dat")
             pauli_dict = {
                 "paulis": [
                     {"label": "X" * num_qubits, "coeff": {"real": 1, "imag": 0}},
                     {"label": "Z" * (num_qubits - 1), "coeff": {"real": 1, "imag": 0}},
                 ]
             }
 
-            obsw = TNObsWeightedSum.empty()
-            obsw.from_pauli_string("test", pauli_dict)
+            obsw = TNObsWeightedSum.from_pauli_string(
+                "test", pauli_dict, use_itpo=False
+            )
             obs += obsw
 
             operators = QCOperators()
-            operators.ops["Z"] = pauli_matrices["Z"]
-            operators.ops["X"] = pauli_matrices["X"]
 
             res = run_simulation(
                 qc,
                 io_info=self.qcio,
                 observables=obs,
                 operators=operators,
                 backend=backend,
             )
 
             obs_res = res.observables
 
+            places = 12 if backend.precision in ("Z", "D") else 5
             self.assertAlmostEqual(
                 obs_res["test"],
                 1,
-                places=12,
+                places=places,
                 msg="Tensor product of ZZ...Z + XX...X has value 0 on odd number of qubits",
             )
 
         return
 
     def test_WeightedSumOnW(self):
         """
@@ -339,28 +341,33 @@
 
             xx = TNObsWeightedSum("X", xtp, [2])
             zz = TNObsWeightedSum("Z", ztp, [3])
             obs += xx
             obs += zz
 
             operators = QCOperators()
-            operators.ops["Z"] = pauli_matrices["Z"]
-            operators.ops["X"] = pauli_matrices["X"]
 
             res = run_simulation(
                 qc,
                 io_info=self.qcio,
                 observables=obs,
                 operators=operators,
                 backend=backend,
             )
 
             obs_res = res.observables
 
+            places = 12 if backend.precision in ("Z", "D") else 5
             self.assertAlmostEqual(
-                obs_res["Z"], -3, places=12, msg="Tensor product of ZZ...Z is correct"
+                obs_res["Z"],
+                -3,
+                places=places,
+                msg="Tensor product of ZZ...Z is correct",
             )
             self.assertAlmostEqual(
-                obs_res["X"], 0, places=12, msg="Tensor product of XX...X is correct"
+                obs_res["X"],
+                0,
+                places=places,
+                msg="Tensor product of XX...X is correct",
             )
 
         return
```

