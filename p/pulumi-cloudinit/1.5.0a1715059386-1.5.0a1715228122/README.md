# Comparing `tmp/pulumi_cloudinit-1.5.0a1715059386.tar.gz` & `tmp/pulumi_cloudinit-1.5.0a1715228122.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_cloudinit-1.5.0a1715059386.tar", last modified: Tue May  7 05:26:01 2024, max compression
+gzip compressed data, was "pulumi_cloudinit-1.5.0a1715228122.tar", last modified: Thu May  9 04:19:03 2024, max compression
```

## Comparing `pulumi_cloudinit-1.5.0a1715059386.tar` & `pulumi_cloudinit-1.5.0a1715228122.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:26:01.278317 pulumi_cloudinit-1.5.0a1715059386/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-07 05:26:01.278317 pulumi_cloudinit-1.5.0a1715059386/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-07 05:25:52.000000 pulumi_cloudinit-1.5.0a1715059386/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:26:01.278317 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-07 05:25:52.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-07 05:25:52.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-07 05:25:52.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-05-07 05:25:52.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-07 05:25:52.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-07 05:25:52.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-07 05:25:52.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 05:25:52.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:25:52.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:26:01.278317 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-07 05:26:01.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-07 05:26:01.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 05:26:01.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 05:26:01.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 05:26:01.000000 pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-07 05:25:52.000000 pulumi_cloudinit-1.5.0a1715059386/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 05:26:01.278317 pulumi_cloudinit-1.5.0a1715059386/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:19:03.712431 pulumi_cloudinit-1.5.0a1715228122/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-09 04:19:03.712431 pulumi_cloudinit-1.5.0a1715228122/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-09 04:18:54.000000 pulumi_cloudinit-1.5.0a1715228122/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:19:03.712431 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-09 04:18:54.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-09 04:18:54.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 04:18:54.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-05-09 04:18:54.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-09 04:18:54.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-09 04:18:54.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-09 04:18:54.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 04:18:54.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:18:54.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:19:03.712431 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-09 04:19:03.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 04:19:03.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:19:03.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 04:19:03.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 04:19:03.000000 pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-09 04:18:54.000000 pulumi_cloudinit-1.5.0a1715228122/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 04:19:03.712431 pulumi_cloudinit-1.5.0a1715228122/setup.cfg
```

### Comparing `pulumi_cloudinit-1.5.0a1715059386/PKG-INFO` & `pulumi_cloudinit-1.5.0a1715228122/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudinit
-Version: 1.5.0a1715059386
+Version: 1.5.0a1715228122
 Summary: A Pulumi package for creating and managing cloudinit cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudinit
 Keywords: pulumi,cloudinit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudinit-1.5.0a1715059386/README.md` & `pulumi_cloudinit-1.5.0a1715228122/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/__init__.py` & `pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/_inputs.py` & `pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/_utilities.py` & `pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/config.py` & `pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/get_config.py` & `pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/outputs.py` & `pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit/provider.py` & `pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715059386/pulumi_cloudinit.egg-info/PKG-INFO` & `pulumi_cloudinit-1.5.0a1715228122/pulumi_cloudinit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudinit
-Version: 1.5.0a1715059386
+Version: 1.5.0a1715228122
 Summary: A Pulumi package for creating and managing cloudinit cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudinit
 Keywords: pulumi,cloudinit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudinit-1.5.0a1715059386/pyproject.toml` & `pulumi_cloudinit-1.5.0a1715228122/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_cloudinit"
   description = "A Pulumi package for creating and managing cloudinit cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "cloudinit"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.5.0a1715059386"
+  version = "1.5.0a1715228122"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-cloudinit"
 
 [build-system]
```

