# Comparing `tmp/scikit_build_core_conan-0.3.0.tar.gz` & `tmp/scikit_build_core_conan-0.3.1.tar.gz`

## Comparing `scikit_build_core_conan-0.3.0.tar` & `scikit_build_core_conan-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.0/src/scikit_build_core_conan/__init__.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.0/src/scikit_build_core_conan/build/__init__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.0/src/scikit_build_core_conan/build/settings.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.0/src/scikit_build_core_conan/build/wheel.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.0/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.0/LICENSE
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.0/README.md
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.1/src/scikit_build_core_conan/__init__.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.1/src/scikit_build_core_conan/build/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.1/src/scikit_build_core_conan/build/settings.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.1/src/scikit_build_core_conan/build/wheel.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.1/README.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.3.1/PKG-INFO
```

### Comparing `scikit_build_core_conan-0.3.0/.github/workflows/cd.yml` & `scikit_build_core_conan-0.3.1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core_conan-0.3.0/src/scikit_build_core_conan/build/__init__.py` & `scikit_build_core_conan-0.3.1/src/scikit_build_core_conan/build/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from scikit_build_core.build import (
     build_sdist,
     get_requires_for_build_editable,
     get_requires_for_build_sdist,
     get_requires_for_build_wheel,
     prepare_metadata_for_build_editable,
     prepare_metadata_for_build_wheel,
```

### Comparing `scikit_build_core_conan-0.3.0/src/scikit_build_core_conan/build/settings.py` & `scikit_build_core_conan-0.3.1/src/scikit_build_core_conan/build/settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core_conan-0.3.0/src/scikit_build_core_conan/build/wheel.py` & `scikit_build_core_conan-0.3.1/src/scikit_build_core_conan/build/wheel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core_conan-0.3.0/.gitignore` & `scikit_build_core_conan-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core_conan-0.3.0/LICENSE` & `scikit_build_core_conan-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core_conan-0.3.0/README.md` & `scikit_build_core_conan-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core_conan-0.3.0/pyproject.toml` & `scikit_build_core_conan-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scikit-build-core-conan"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     { name = "Zhengyu Wu", email = "zhengyu.wu21@imperial.ac.uk" },
 ]
 description = "A conan plugin for scikit-build-core"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scikit_build_core_conan-0.3.0/PKG-INFO` & `scikit_build_core_conan-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scikit-build-core-conan
-Version: 0.3.0
+Version: 0.3.1
 Summary: A conan plugin for scikit-build-core
 Project-URL: Homepage, https://github.com/wu-vincent/scikit-build-core-conan
 Project-URL: Issues, https://github.com/wu-vincent/scikit-build-core-conan/issues
 Author-email: Zhengyu Wu <zhengyu.wu21@imperial.ac.uk>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

