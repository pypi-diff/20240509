# Comparing `tmp/perceval_opnfv-1.0.0rc2.tar.gz` & `tmp/perceval_opnfv-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_opnfv-1.0.0rc2.tar", max compression
+gzip compressed data, was "perceval_opnfv-1.0.1rc1.tar", max compression
```

## Comparing `perceval_opnfv-1.0.0rc2.tar` & `perceval_opnfv-1.0.1rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      329 2024-04-11 10:49:46.827883 perceval_opnfv-1.0.0rc2/AUTHORS
--rw-r--r--   0        0        0    35147 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0     2481 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/NEWS
--rw-r--r--   0        0        0     2250 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/README.md
--rw-r--r--   0        0        0        0 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/perceval/backends/opnfv/__init__.py
--rw-r--r--   0        0        0       91 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/perceval/backends/opnfv/_version.py
--rw-r--r--   0        0        0     7996 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/perceval/backends/opnfv/functest.py
--rw-r--r--   0        0        0     1405 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/tests/__init__.py
--rw-r--r--   0        0        0     1887 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/tests/base.py
--rw-r--r--   0        0        0    46769 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/tests/data/functest/functest_results.json
--rw-r--r--   0        0        0      101 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/tests/data/functest/functest_results_empty.json
--rw-r--r--   0        0        0    41641 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/tests/data/functest/functest_results_page_1.json
--rw-r--r--   0        0        0     5312 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/tests/data/functest/functest_results_page_2.json
--rwxr-xr-x   0        0        0     1017 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/tests/run_tests.py
--rw-r--r--   0        0        0    13686 2024-04-11 10:49:46.831883 perceval_opnfv-1.0.0rc2/tests/test_functest.py
--rw-r--r--   0        0        0     3381 1970-01-01 00:00:00.000000 perceval_opnfv-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      329 2024-05-09 08:00:56.597866 perceval_opnfv-1.0.1rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-05-09 08:00:56.597866 perceval_opnfv-1.0.1rc1/LICENSE
+-rw-r--r--   0        0        0     2639 2024-05-09 08:00:56.597866 perceval_opnfv-1.0.1rc1/NEWS
+-rw-r--r--   0        0        0     2250 2024-05-09 08:00:56.597866 perceval_opnfv-1.0.1rc1/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 08:00:56.601866 perceval_opnfv-1.0.1rc1/perceval/backends/opnfv/__init__.py
+-rw-r--r--   0        0        0       91 2024-05-09 08:00:56.601866 perceval_opnfv-1.0.1rc1/perceval/backends/opnfv/_version.py
+-rw-r--r--   0        0        0     7996 2024-05-09 08:00:56.601866 perceval_opnfv-1.0.1rc1/perceval/backends/opnfv/functest.py
+-rw-r--r--   0        0        0     1405 2024-05-09 08:00:56.601866 perceval_opnfv-1.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-09 08:00:56.601866 perceval_opnfv-1.0.1rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1887 2024-05-09 08:00:56.601866 perceval_opnfv-1.0.1rc1/tests/base.py
+-rw-r--r--   0        0        0    46769 2024-05-09 08:00:56.601866 perceval_opnfv-1.0.1rc1/tests/data/functest/functest_results.json
+-rw-r--r--   0        0        0      101 2024-05-09 08:00:56.601866 perceval_opnfv-1.0.1rc1/tests/data/functest/functest_results_empty.json
+-rw-r--r--   0        0        0    41641 2024-05-09 08:00:56.601866 perceval_opnfv-1.0.1rc1/tests/data/functest/functest_results_page_1.json
+-rw-r--r--   0        0        0     5312 2024-05-09 08:00:56.601866 perceval_opnfv-1.0.1rc1/tests/data/functest/functest_results_page_2.json
+-rwxr-xr-x   0        0        0     1017 2024-05-09 08:00:56.601866 perceval_opnfv-1.0.1rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    13686 2024-05-09 08:00:56.601866 perceval_opnfv-1.0.1rc1/tests/test_functest.py
+-rw-r--r--   0        0        0     3381 1970-01-01 00:00:00.000000 perceval_opnfv-1.0.1rc1/PKG-INFO
```

### Comparing `perceval_opnfv-1.0.0rc2/LICENSE` & `perceval_opnfv-1.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-1.0.0rc2/NEWS` & `perceval_opnfv-1.0.1rc1/NEWS`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Releases
 
+## perceval-opnfv 1.0.0 - (2024-04-13)
+
+**New features:**
+
+ * First major release\
+   GrimoireLab reached a stable status. This is our first major release.
+
+
   ## perceval-opnfv 0.2.25 - (2024-03-27)
   
   * Update Poetry's package dependencies
 
   ## perceval-opnfv 0.2.24 - (2024-03-12)
   
   * Update Poetry's package dependencies
```

### Comparing `perceval_opnfv-1.0.0rc2/README.md` & `perceval_opnfv-1.0.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-1.0.0rc2/perceval/backends/opnfv/functest.py` & `perceval_opnfv-1.0.1rc1/perceval/backends/opnfv/functest.py`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-1.0.0rc2/pyproject.toml` & `perceval_opnfv-1.0.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-opnfv"
-version = "1.0.0-rc.2"
+version = "1.0.1-rc.1"
 description = "Bundle of Perceval backends for OPNFV ecosystem."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `perceval_opnfv-1.0.0rc2/tests/base.py` & `perceval_opnfv-1.0.1rc1/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-1.0.0rc2/tests/data/functest/functest_results.json` & `perceval_opnfv-1.0.1rc1/tests/data/functest/functest_results.json`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-1.0.0rc2/tests/data/functest/functest_results_page_1.json` & `perceval_opnfv-1.0.1rc1/tests/data/functest/functest_results_page_1.json`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-1.0.0rc2/tests/data/functest/functest_results_page_2.json` & `perceval_opnfv-1.0.1rc1/tests/data/functest/functest_results_page_2.json`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-1.0.0rc2/tests/run_tests.py` & `perceval_opnfv-1.0.1rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-1.0.0rc2/tests/test_functest.py` & `perceval_opnfv-1.0.1rc1/tests/test_functest.py`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-1.0.0rc2/PKG-INFO` & `perceval_opnfv-1.0.1rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-opnfv
-Version: 1.0.0rc2
+Version: 1.0.1rc1
 Summary: Bundle of Perceval backends for OPNFV ecosystem.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

