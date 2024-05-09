# Comparing `tmp/pqam_rmsadtandoc2023-0.1.4.tar.gz` & `tmp/pqam_rmsadtandoc2023-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqam_rmsadtandoc2023-0.1.4.tar", last modified: Thu Feb 22 15:34:33 2024, max compression
+gzip compressed data, was "pqam_rmsadtandoc2023-0.1.5.tar", last modified: Thu May  9 14:44:14 2024, max compression
```

## Comparing `pqam_rmsadtandoc2023-0.1.4.tar` & `pqam_rmsadtandoc2023-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:34:33.687759 pqam_rmsadtandoc2023-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:34:33.683759 pqam_rmsadtandoc2023-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:34:33.683759 pqam_rmsadtandoc2023-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-22 15:34:22.000000 pqam_rmsadtandoc2023-0.1.4/.github/workflows/publishPyPI.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-22 15:34:22.000000 pqam_rmsadtandoc2023-0.1.4/.github/workflows/runtimeTesting.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-22 15:34:22.000000 pqam_rmsadtandoc2023-0.1.4/.github/workflows/weeklyRuntimeTesting.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-02-22 15:34:22.000000 pqam_rmsadtandoc2023-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-02-22 15:34:33.683759 pqam_rmsadtandoc2023-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-02-22 15:34:22.000000 pqam_rmsadtandoc2023-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:34:33.683759 pqam_rmsadtandoc2023-0.1.4/pqam_rmsadtandoc2023/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-22 15:34:22.000000 pqam_rmsadtandoc2023-0.1.4/pqam_rmsadtandoc2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-02-22 15:34:22.000000 pqam_rmsadtandoc2023-0.1.4/pqam_rmsadtandoc2023/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-22 15:34:22.000000 pqam_rmsadtandoc2023-0.1.4/pqam_rmsadtandoc2023/outputDefinition.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:34:33.683759 pqam_rmsadtandoc2023-0.1.4/pqam_rmsadtandoc2023.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-02-22 15:34:33.000000 pqam_rmsadtandoc2023-0.1.4/pqam_rmsadtandoc2023.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-22 15:34:33.000000 pqam_rmsadtandoc2023-0.1.4/pqam_rmsadtandoc2023.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 15:34:33.000000 pqam_rmsadtandoc2023-0.1.4/pqam_rmsadtandoc2023.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-22 15:34:33.000000 pqam_rmsadtandoc2023-0.1.4/pqam_rmsadtandoc2023.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-22 15:34:33.000000 pqam_rmsadtandoc2023-0.1.4/pqam_rmsadtandoc2023.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-02-22 15:34:22.000000 pqam_rmsadtandoc2023-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 15:34:33.687759 pqam_rmsadtandoc2023-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:44:14.366772 pqam_rmsadtandoc2023-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:44:14.362771 pqam_rmsadtandoc2023-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:44:14.366772 pqam_rmsadtandoc2023-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-09 14:44:06.000000 pqam_rmsadtandoc2023-0.1.5/.github/workflows/publishPyPI.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-09 14:44:06.000000 pqam_rmsadtandoc2023-0.1.5/.github/workflows/runtimeTesting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-09 14:44:06.000000 pqam_rmsadtandoc2023-0.1.5/.github/workflows/weeklyRuntimeTesting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-09 14:44:06.000000 pqam_rmsadtandoc2023-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-09 14:44:14.366772 pqam_rmsadtandoc2023-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-09 14:44:06.000000 pqam_rmsadtandoc2023-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:44:14.366772 pqam_rmsadtandoc2023-0.1.5/pqam_rmsadtandoc2023/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 14:44:06.000000 pqam_rmsadtandoc2023-0.1.5/pqam_rmsadtandoc2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-05-09 14:44:06.000000 pqam_rmsadtandoc2023-0.1.5/pqam_rmsadtandoc2023/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-09 14:44:06.000000 pqam_rmsadtandoc2023-0.1.5/pqam_rmsadtandoc2023/outputDefinition.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:44:14.366772 pqam_rmsadtandoc2023-0.1.5/pqam_rmsadtandoc2023.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-09 14:44:14.000000 pqam_rmsadtandoc2023-0.1.5/pqam_rmsadtandoc2023.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 14:44:14.000000 pqam_rmsadtandoc2023-0.1.5/pqam_rmsadtandoc2023.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:44:14.000000 pqam_rmsadtandoc2023-0.1.5/pqam_rmsadtandoc2023.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-09 14:44:14.000000 pqam_rmsadtandoc2023-0.1.5/pqam_rmsadtandoc2023.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-09 14:44:14.000000 pqam_rmsadtandoc2023-0.1.5/pqam_rmsadtandoc2023.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-09 14:44:06.000000 pqam_rmsadtandoc2023-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:44:14.366772 pqam_rmsadtandoc2023-0.1.5/setup.cfg
```

### Comparing `pqam_rmsadtandoc2023-0.1.4/.github/workflows/publishPyPI.yml` & `pqam_rmsadtandoc2023-0.1.5/.github/workflows/publishPyPI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
     tags:
       - '**'
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
         cache: 'pip'
         cache-dependency-path: 'pyproject.toml'
         
     - name: Install dependencies
       run: |
```

### Comparing `pqam_rmsadtandoc2023-0.1.4/.github/workflows/runtimeTesting.yml` & `pqam_rmsadtandoc2023-0.1.5/.github/workflows/runtimeTesting.yml`

 * *Files identical despite different names*

### Comparing `pqam_rmsadtandoc2023-0.1.4/.github/workflows/weeklyRuntimeTesting.yml` & `pqam_rmsadtandoc2023-0.1.5/.github/workflows/weeklyRuntimeTesting.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 name: (weekly) periodic verification everything works
 
 on: 
   schedule:
     - cron: '30 17 * * 1'
+  workflow_dispatch:
 
 jobs:
   tests:
     strategy:
       matrix:
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
         platform: [ubuntu-latest, macos-latest, windows-latest]
     runs-on: ${{ matrix.platform }}
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         cache: 'pip'
         cache-dependency-path: 'pyproject.toml'
 
     - name: Install dependencies
       run: |
```

### Comparing `pqam_rmsadtandoc2023-0.1.4/LICENSE` & `pqam_rmsadtandoc2023-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pqam_rmsadtandoc2023-0.1.4/PKG-INFO` & `pqam_rmsadtandoc2023-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqam_rmsadtandoc2023
-Version: 0.1.4
+Version: 0.1.5
 Summary: PyQAlloy-compatible Model for RMSAD prediction based on Tandoc 2023 (https://doi.org/10.1038/s41524-023-00993-x)
 Author-email: Adam Krajewski <ak@psu.edu>
 Project-URL: Documentation, https://github.com/tandocca/Lattice-Distortion
 Project-URL: Homepage, https://github.com/amkrajewski/pqam_RMSADTandoc2023
 Project-URL: Bug Tracker, https://github.com/amkrajewski/pqam_RMSADTandoc2023/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -32,15 +32,17 @@
 
 Tests: [![small runtime test](https://github.com/amkrajewski/pqam_RMSADTandoc2023/actions/workflows/runtimeTesting.yml/badge.svg)](https://github.com/amkrajewski/pqam_RMSADTandoc2023/actions/workflows/runtimeTesting.yml)
 
 License: [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 
 ## This Fork
 
-This small repository is a lightweight fork version of the original one by Tandoc. It is only slightly modified to fit automated pipelines of the [ULTERA Database (ultera.org)](https://ultera.org) infrastrcutre, which expects `model.py` script with `predict(comp: pymatgen.Composition)` and `predict(comp: str)` function returning an ordered array of output numbers or a labeled dictionary of them.
+This small repository is a lightweight fork (with extra checks) version of the original one by Tandoc. It is only slightly modified to fit automated pipelines of the [ULTERA Database (ultera.org)](https://ultera.org) infrastrcutre, which expects `model.py` script with `predict(comp: pymatgen.Composition)` and `predict(comp: str)` function returning an ordered array of output numbers or a labeled dictionary of them corresponding to the machine-readible definition under `outputDefinition.json`.
+
+Chemical Space: `["Ti", "Zr", "Hf", "V", "Nb", "Ta", "Mo", "W", "Re", "Ru"]`
 
 Output Order: [`rmsad_Tandoc2023`]
 
 Output Meaning (all based on [10.1038/s41524-023-00993-x](https://doi.org/10.1038/s41524-023-00993-x)):
 - `rmsad_Tandoc2023` - Root Mean Squared Atomic Displacement in the units of Angstrom
 
 ## Install and Use
```

### Comparing `pqam_rmsadtandoc2023-0.1.4/README.md` & `pqam_rmsadtandoc2023-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 Tests: [![small runtime test](https://github.com/amkrajewski/pqam_RMSADTandoc2023/actions/workflows/runtimeTesting.yml/badge.svg)](https://github.com/amkrajewski/pqam_RMSADTandoc2023/actions/workflows/runtimeTesting.yml)
 
 License: [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 
 ## This Fork
 
-This small repository is a lightweight fork version of the original one by Tandoc. It is only slightly modified to fit automated pipelines of the [ULTERA Database (ultera.org)](https://ultera.org) infrastrcutre, which expects `model.py` script with `predict(comp: pymatgen.Composition)` and `predict(comp: str)` function returning an ordered array of output numbers or a labeled dictionary of them.
+This small repository is a lightweight fork (with extra checks) version of the original one by Tandoc. It is only slightly modified to fit automated pipelines of the [ULTERA Database (ultera.org)](https://ultera.org) infrastrcutre, which expects `model.py` script with `predict(comp: pymatgen.Composition)` and `predict(comp: str)` function returning an ordered array of output numbers or a labeled dictionary of them corresponding to the machine-readible definition under `outputDefinition.json`.
+
+Chemical Space: `["Ti", "Zr", "Hf", "V", "Nb", "Ta", "Mo", "W", "Re", "Ru"]`
 
 Output Order: [`rmsad_Tandoc2023`]
 
 Output Meaning (all based on [10.1038/s41524-023-00993-x](https://doi.org/10.1038/s41524-023-00993-x)):
 - `rmsad_Tandoc2023` - Root Mean Squared Atomic Displacement in the units of Angstrom
 
 ## Install and Use
```

### Comparing `pqam_rmsadtandoc2023-0.1.4/pqam_rmsadtandoc2023/model.py` & `pqam_rmsadtandoc2023-0.1.5/pqam_rmsadtandoc2023/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,19 @@
     assert isinstance(comp, (str, Composition)), "comp must be a string or a pymatgen Composition object."
 
     if isinstance(comp, str):
         comp = Composition(comp)
     
     elements = {}
     for element in comp:
-        elements[str(element)] = comp.get_atomic_fraction(element)
+        elStr = str(element)
+        if elStr not in ["Ti", "Zr", "Hf", "V", "Nb", "Ta", "Mo", "W", "Re", "Ru"]:
+            raise NotImplementedError(
+                f"Element {elStr} passed as an input has not been implemented within Tandoc 2023 model covering Ti, Zr, Hf, V, Nb, Ta, Mo, W, Re, Ru")
+        elements[elStr] = comp.get_atomic_fraction(element)
     pairs = {}
     for element1 in elements:
         for element2 in elements:
             pair = element1 + element2
             concentration = elements[element1] * elements[element2]
             pairs[pair] = concentration
```

### Comparing `pqam_rmsadtandoc2023-0.1.4/pqam_rmsadtandoc2023.egg-info/PKG-INFO` & `pqam_rmsadtandoc2023-0.1.5/pqam_rmsadtandoc2023.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqam_rmsadtandoc2023
-Version: 0.1.4
+Version: 0.1.5
 Summary: PyQAlloy-compatible Model for RMSAD prediction based on Tandoc 2023 (https://doi.org/10.1038/s41524-023-00993-x)
 Author-email: Adam Krajewski <ak@psu.edu>
 Project-URL: Documentation, https://github.com/tandocca/Lattice-Distortion
 Project-URL: Homepage, https://github.com/amkrajewski/pqam_RMSADTandoc2023
 Project-URL: Bug Tracker, https://github.com/amkrajewski/pqam_RMSADTandoc2023/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -32,15 +32,17 @@
 
 Tests: [![small runtime test](https://github.com/amkrajewski/pqam_RMSADTandoc2023/actions/workflows/runtimeTesting.yml/badge.svg)](https://github.com/amkrajewski/pqam_RMSADTandoc2023/actions/workflows/runtimeTesting.yml)
 
 License: [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 
 ## This Fork
 
-This small repository is a lightweight fork version of the original one by Tandoc. It is only slightly modified to fit automated pipelines of the [ULTERA Database (ultera.org)](https://ultera.org) infrastrcutre, which expects `model.py` script with `predict(comp: pymatgen.Composition)` and `predict(comp: str)` function returning an ordered array of output numbers or a labeled dictionary of them.
+This small repository is a lightweight fork (with extra checks) version of the original one by Tandoc. It is only slightly modified to fit automated pipelines of the [ULTERA Database (ultera.org)](https://ultera.org) infrastrcutre, which expects `model.py` script with `predict(comp: pymatgen.Composition)` and `predict(comp: str)` function returning an ordered array of output numbers or a labeled dictionary of them corresponding to the machine-readible definition under `outputDefinition.json`.
+
+Chemical Space: `["Ti", "Zr", "Hf", "V", "Nb", "Ta", "Mo", "W", "Re", "Ru"]`
 
 Output Order: [`rmsad_Tandoc2023`]
 
 Output Meaning (all based on [10.1038/s41524-023-00993-x](https://doi.org/10.1038/s41524-023-00993-x)):
 - `rmsad_Tandoc2023` - Root Mean Squared Atomic Displacement in the units of Angstrom
 
 ## Install and Use
```

### Comparing `pqam_rmsadtandoc2023-0.1.4/pyproject.toml` & `pqam_rmsadtandoc2023-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pqam_rmsadtandoc2023"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Adam Krajewski", email="ak@psu.edu" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

