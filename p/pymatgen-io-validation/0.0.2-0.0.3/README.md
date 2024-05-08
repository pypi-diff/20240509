# Comparing `tmp/pymatgen_io_validation-0.0.2.tar.gz` & `tmp/pymatgen_io_validation-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen_io_validation-0.0.2.tar", last modified: Fri May  3 19:07:40 2024, max compression
+gzip compressed data, was "pymatgen_io_validation-0.0.3.tar", last modified: Wed May  8 23:24:14 2024, max compression
```

## Comparing `pymatgen_io_validation-0.0.2.tar` & `pymatgen_io_validation-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.840586 pymatgen_io_validation-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-05-03 19:07:40.840586 pymatgen_io_validation-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13787 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.836586 pymatgen_io_validation-0.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/examples/MP_compliant_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.832586 pymatgen_io_validation-0.0.2/pymatgen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.832586 pymatgen_io_validation-0.0.2/pymatgen/io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.836586 pymatgen_io_validation-0.0.2/pymatgen/io/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_common_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_for_excess_empty_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    42367 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_incar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_kpoints_kspacing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_package_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_potcar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/compare_to_MP_ehull.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15892 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pymatgen/io/validation/vasp_defaults.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.840586 pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-05-03 19:07:40.000000 pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 19:07:40.000000 pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:07:40.000000 pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 19:07:40.000000 pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-03 19:07:40.000000 pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-03 19:07:40.840586 pymatgen_io_validation-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:07:40.840586 pymatgen_io_validation-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    27016 2024-05-03 19:07:35.000000 pymatgen_io_validation-0.0.2/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.050465 pymatgen_io_validation-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-05-08 23:24:14.050465 pymatgen_io_validation-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13787 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.046465 pymatgen_io_validation-0.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/examples/MP_compliant_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.046465 pymatgen_io_validation-0.0.3/pymatgen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.046465 pymatgen_io_validation-0.0.3/pymatgen/io/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.050465 pymatgen_io_validation-0.0.3/pymatgen/io/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_common_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_for_excess_empty_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42260 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_incar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_kpoints_kspacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_package_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_potcar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/compare_to_MP_ehull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15892 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/vasp_defaults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.050465 pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-05-08 23:24:14.000000 pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-08 23:24:14.000000 pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 23:24:14.000000 pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-08 23:24:14.000000 pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-08 23:24:14.000000 pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-08 23:24:14.054465 pymatgen_io_validation-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.050465 pymatgen_io_validation-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    27113 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/tests/test_validation.py
```

### Comparing `pymatgen_io_validation-0.0.2/LICENSE` & `pymatgen_io_validation-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/PKG-INFO` & `pymatgen_io_validation-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-io-validation
-Version: 0.0.2
+Version: 0.0.3
 Summary: A comprehensive I/O validator for electronic structure calculations
 Home-page: https://github.com/materialsproject/pymatgen-io-validation
 Author: Janosh Riebesell, Jason Munro, Aaron Kaplan
 Author-email: Matthew Kuner <matthewkuner@gmail.com>
 Maintainer: Matthew Kuner
 License: modified BSD
 Keywords: io,validation,dft,vasp
@@ -26,16 +26,16 @@
 License-File: LICENSE
 Requires-Dist: pymatgen
 Requires-Dist: numpy
 Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: pre-commit>=2.12.1; extra == "dev"
 Provides-Extra: tests
-Requires-Dist: pytest==8.0.2; extra == "tests"
-Requires-Dist: pytest-cov==4.1.0; extra == "tests"
+Requires-Dist: pytest==8.2.0; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0; extra == "tests"
 Requires-Dist: types-requests; extra == "tests"
 
 pymatgen-io-validation
 =====
 
 This package is an extension to `pymatgen` for performing I/O validation. Specifically, this package checks for discrepancies between a specific calculation and a provided input set; it also checks for known bugs when certain input parameters are used in combination, alongside several other small checks. The motivation for creating this package was to ensure VASP calculations performed by groups outside of the Materials Project (MP) are compliant with MP data, thus enabling their raw data to be included in the MP Database.
```

### Comparing `pymatgen_io_validation-0.0.2/README.md` & `pymatgen_io_validation-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/examples/MP_compliant_job.py` & `pymatgen_io_validation-0.0.3/examples/MP_compliant_job.py`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pymatgen/io/validation/__init__.py` & `pymatgen_io_validation-0.0.3/pymatgen/io/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_common_errors.py` & `pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_common_errors.py`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_for_excess_empty_space.py` & `pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_for_excess_empty_space.py`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_incar.py` & `pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_incar.py`

 * *Files 0% similar despite different names*

```diff
@@ -560,20 +560,18 @@
         else:
             self.defaults["SIGMA"]["operation"] = "<="
 
         # Also check if SIGMA is too large according to the VASP wiki,
         # which occurs when the entropy term in the energy is greater than 1 meV/atom.
         self.parameters["ELECTRONIC ENTROPY"] = -1e20
         for ionic_step in self._ionic_steps:
-            electronic_steps = ionic_step["electronic_steps"]
-            for elec_step in electronic_steps:
-                if elec_step.get("eentropy", None):
-                    self.parameters["ELECTRONIC ENTROPY"] = max(
-                        self.parameters["ELECTRONIC ENTROPY"], abs(elec_step["eentropy"] / self.structure.num_sites)
-                    )
+            if eentropy := ionic_step["electronic_steps"][-1].get("eentropy"):
+                self.parameters["ELECTRONIC ENTROPY"] = max(
+                    self.parameters["ELECTRONIC ENTROPY"], abs(eentropy / self.structure.num_sites)
+                )
 
         convert_eV_to_meV = 1000
         self.parameters["ELECTRONIC ENTROPY"] = round(self.parameters["ELECTRONIC ENTROPY"] * convert_eV_to_meV, 3)
         self.valid_values["ELECTRONIC ENTROPY"] = 0.001 * convert_eV_to_meV
 
         self.defaults["ELECTRONIC ENTROPY"] = {
             "value": 0.0,
```

### Comparing `pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_kpoints_kspacing.py` & `pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_kpoints_kspacing.py`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_package_versions.py` & `pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_package_versions.py`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pymatgen/io/validation/check_potcar.py` & `pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_potcar.py`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pymatgen/io/validation/common.py` & `pymatgen_io_validation-0.0.3/pymatgen/io/validation/common.py`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pymatgen/io/validation/compare_to_MP_ehull.py` & `pymatgen_io_validation-0.0.3/pymatgen/io/validation/compare_to_MP_ehull.py`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pymatgen/io/validation/settings.py` & `pymatgen_io_validation-0.0.3/pymatgen/io/validation/settings.py`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pymatgen/io/validation/validation.py` & `pymatgen_io_validation-0.0.3/pymatgen/io/validation/validation.py`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pymatgen/io/validation/vasp_defaults.yaml` & `pymatgen_io_validation-0.0.3/pymatgen/io/validation/vasp_defaults.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/PKG-INFO` & `pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-io-validation
-Version: 0.0.2
+Version: 0.0.3
 Summary: A comprehensive I/O validator for electronic structure calculations
 Home-page: https://github.com/materialsproject/pymatgen-io-validation
 Author: Janosh Riebesell, Jason Munro, Aaron Kaplan
 Author-email: Matthew Kuner <matthewkuner@gmail.com>
 Maintainer: Matthew Kuner
 License: modified BSD
 Keywords: io,validation,dft,vasp
@@ -26,16 +26,16 @@
 License-File: LICENSE
 Requires-Dist: pymatgen
 Requires-Dist: numpy
 Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: pre-commit>=2.12.1; extra == "dev"
 Provides-Extra: tests
-Requires-Dist: pytest==8.0.2; extra == "tests"
-Requires-Dist: pytest-cov==4.1.0; extra == "tests"
+Requires-Dist: pytest==8.2.0; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0; extra == "tests"
 Requires-Dist: types-requests; extra == "tests"
 
 pymatgen-io-validation
 =====
 
 This package is an extension to `pymatgen` for performing I/O validation. Specifically, this package checks for discrepancies between a specific calculation and a provided input set; it also checks for known bugs when certain input parameters are used in combination, alongside several other small checks. The motivation for creating this package was to ensure VASP calculations performed by groups outside of the Materials Project (MP) are compliant with MP data, thus enabling their raw data to be included in the MP Database.
```

### Comparing `pymatgen_io_validation-0.0.2/pymatgen_io_validation.egg-info/SOURCES.txt` & `pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/pyproject.toml` & `pymatgen_io_validation-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 readme = "README.md"
 requires-python = '>=3.8'
 
 [project.optional-dependencies]
 dev = ["pre-commit>=2.12.1"]
 #docs = ["jupyter-book>=0.13.1",]
 
-tests = ["pytest==8.0.2", "pytest-cov==4.1.0", "types-requests"]
+tests = ["pytest==8.2.0", "pytest-cov==5.0.0", "types-requests"]
 
 
 [tool.setuptools.dynamic]
 readme = { file = ["README.md"] }
 
 #[project.urls]
 #repository = "https://github.com/materialsproject/pymatgen-io-validation"
```

### Comparing `pymatgen_io_validation-0.0.2/setup.cfg` & `pymatgen_io_validation-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.2/setup.py` & `pymatgen_io_validation-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with open(os.path.join(SETUP_PTH, "README.md")) as f:
     desc = f.read()
 
 
 setup(
     name="pymatgen-io-validation",
     packages=find_namespace_packages(include=["pymatgen.io.*"]),
-    version="0.0.2",
+    version="0.0.3",
     install_requires=["pymatgen>=2022.0.3", "emmet-core>=0.77.1", "pydantic>=2.4.2", "requests>=2.28.1"],
     extras_require={},
     package_data={"pymatgen.io.validation": ["*.yaml"]},
     author="Matthew Kuner, Janosh Riebesell, Jason Munro, Aaron Kaplan",
     author_email="matthewkuner@berkeley.edu",
     maintainer="Matthew Kuner",
     url="https://github.com/materialsproject/pymatgen-io-validation",
```

### Comparing `pymatgen_io_validation-0.0.2/tests/test_validation.py` & `pymatgen_io_validation-0.0.3/tests/test_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,14 +439,16 @@
 
 
 def _update_kpoints_for_test(task_doc: TaskDoc, kpoints_updates: dict):
     if isinstance(task_doc.calcs_reversed[0].input.kpoints, Kpoints):
         kpoints = task_doc.calcs_reversed[0].input.kpoints.as_dict()
     elif isinstance(task_doc.calcs_reversed[0].input.kpoints, dict):
         kpoints = task_doc.calcs_reversed[0].input.kpoints.copy()
+    if isinstance(kpoints_updates, Kpoints):
+        kpoints_updates = kpoints_updates.as_dict()
     kpoints.update(kpoints_updates)
     task_doc.calcs_reversed[0].input.kpoints = Kpoints.from_dict(kpoints)
 
 
 @pytest.mark.parametrize(
     "object_name",
     [
```

