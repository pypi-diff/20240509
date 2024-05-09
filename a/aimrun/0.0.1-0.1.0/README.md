# Comparing `tmp/aimrun-0.0.1.tar.gz` & `tmp/aimrun-0.1.0.tar.gz`

## Comparing `aimrun-0.0.1.tar` & `aimrun-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 aimrun-0.0.1/aimrun/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 aimrun-0.0.1/LICENSE
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aimrun-0.0.1/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 aimrun-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 aimrun-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 aimrun-0.1.0/aimrun/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 aimrun-0.1.0/LICENSE
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aimrun-0.1.0/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 aimrun-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 aimrun-0.1.0/PKG-INFO
```

### Comparing `aimrun-0.0.1/aimrun/__init__.py` & `aimrun-0.1.0/aimrun/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,17 @@
         _init(experiment=project, args=config, **kwargs)
     @staticmethod
     def log(*args, **kwargs):
         _track(*args, **kwargs)
     @staticmethod
     def finish():
         _close()
+    @staticmethod
+    def set_default_repo(repo):
+        set_default_repo(repo)
 
 # aim interface
 
 class Run:
     def __init__(self, *args, **kwargs):
         _init(*args, **kwargs)
     def track(self, *args, **kwargs):
```

### Comparing `aimrun-0.0.1/LICENSE` & `aimrun-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aimrun-0.0.1/pyproject.toml` & `aimrun-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aimrun"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name = "Peter Schneider-Kamp" },
   { name = "Jacob Nielsen" },
 ]
 
 description = "A simple way of integrating aim into MLOps frameworks."
 readme = "README.md"
```

### Comparing `aimrun-0.0.1/PKG-INFO` & `aimrun-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aimrun
-Version: 0.0.1
+Version: 0.1.0
 Summary: A simple way of integrating aim into MLOps frameworks.
 Project-URL: Homepage, https://github.com/schneiderkamplab/aimrun
 Project-URL: Bug Tracker, https://github.com/schneiderkamplab/aimrun/issues
 Author: Peter Schneider-Kamp, Jacob Nielsen
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

