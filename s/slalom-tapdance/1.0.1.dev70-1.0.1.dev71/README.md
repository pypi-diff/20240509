# Comparing `tmp/slalom_tapdance-1.0.1.dev70.tar.gz` & `tmp/slalom_tapdance-1.0.1.dev71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-1.0.1.dev70.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.1.dev71.tar", max compression
```

## Comparing `slalom_tapdance-1.0.1.dev70.tar` & `slalom_tapdance-1.0.1.dev71.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-09 18:31:46.174534 slalom_tapdance-1.0.1.dev70/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-09 18:32:02.534739 slalom_tapdance-1.0.1.dev70/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/install_helper.py
--rw-r--r--   0        0        0    38026 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/states.py
--rw-r--r--   0        0        0    11998 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/syncs.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev70/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-09 18:34:32.896958 slalom_tapdance-1.0.1.dev71/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-09 18:34:50.136812 slalom_tapdance-1.0.1.dev71/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/install_helper.py
+-rw-r--r--   0        0        0    38026 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/states.py
+-rw-r--r--   0        0        0    11998 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/syncs.py
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev71/PKG-INFO
```

### Comparing `slalom_tapdance-1.0.1.dev70/LICENSE` & `slalom_tapdance-1.0.1.dev71/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev70/pyproject.toml` & `slalom_tapdance-1.0.1.dev71/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "1.0.1-dev.70"
+version = "1.0.1-dev.71"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-1.0.1.dev70/tapdance/cli.py` & `slalom_tapdance-1.0.1.dev71/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev70/tapdance/config.py` & `slalom_tapdance-1.0.1.dev71/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev70/tapdance/docker.py` & `slalom_tapdance-1.0.1.dev71/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev70/tapdance/install_helper.py` & `slalom_tapdance-1.0.1.dev71/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev70/tapdance/plans.py` & `slalom_tapdance-1.0.1.dev71/tapdance/plans.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev70/tapdance/states.py` & `slalom_tapdance-1.0.1.dev71/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev70/tapdance/syncs.py` & `slalom_tapdance-1.0.1.dev71/tapdance/syncs.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev70/PKG-INFO` & `slalom_tapdance-1.0.1.dev71/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 1.0.1.dev70
+Version: 1.0.1.dev71
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

