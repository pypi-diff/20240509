# Comparing `tmp/pbc_distance_calculator-1.2.1.tar.gz` & `tmp/pbc_distance_calculator-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbc_distance_calculator-1.2.1.tar", last modified: Tue Apr 23 15:51:57 2024, max compression
+gzip compressed data, was "pbc_distance_calculator-1.3.0.tar", last modified: Thu May  9 19:27:34 2024, max compression
```

## Comparing `pbc_distance_calculator-1.2.1.tar` & `pbc_distance_calculator-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:51:57.081689 pbc_distance_calculator-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 15:51:52.000000 pbc_distance_calculator-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-23 15:51:57.081689 pbc_distance_calculator-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-23 15:51:52.000000 pbc_distance_calculator-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:51:57.077690 pbc_distance_calculator-1.2.1/pbc_distance_calculator/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 15:51:52.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-23 15:51:52.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator/calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:51:57.081689 pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-23 15:51:57.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-23 15:51:57.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:51:57.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 15:51:57.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 15:51:57.000000 pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-23 15:51:57.081689 pbc_distance_calculator-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 15:51:52.000000 pbc_distance_calculator-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:27:34.003362 pbc_distance_calculator-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-09 19:27:29.000000 pbc_distance_calculator-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-09 19:27:34.003362 pbc_distance_calculator-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-09 19:27:29.000000 pbc_distance_calculator-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:27:34.003362 pbc_distance_calculator-1.3.0/pbc_distance_calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-09 19:27:29.000000 pbc_distance_calculator-1.3.0/pbc_distance_calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-09 19:27:29.000000 pbc_distance_calculator-1.3.0/pbc_distance_calculator/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-09 19:27:29.000000 pbc_distance_calculator-1.3.0/pbc_distance_calculator/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:27:34.003362 pbc_distance_calculator-1.3.0/pbc_distance_calculator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-09 19:27:29.000000 pbc_distance_calculator-1.3.0/pbc_distance_calculator/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:27:34.003362 pbc_distance_calculator-1.3.0/pbc_distance_calculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-09 19:27:33.000000 pbc_distance_calculator-1.3.0/pbc_distance_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-09 19:27:33.000000 pbc_distance_calculator-1.3.0/pbc_distance_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 19:27:33.000000 pbc_distance_calculator-1.3.0/pbc_distance_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 19:27:33.000000 pbc_distance_calculator-1.3.0/pbc_distance_calculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 19:27:33.000000 pbc_distance_calculator-1.3.0/pbc_distance_calculator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-09 19:27:34.003362 pbc_distance_calculator-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-09 19:27:29.000000 pbc_distance_calculator-1.3.0/setup.py
```

### Comparing `pbc_distance_calculator-1.2.1/LICENSE` & `pbc_distance_calculator-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pbc_distance_calculator-1.2.1/PKG-INFO` & `pbc_distance_calculator-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbc_distance_calculator
-Version: 1.2.1
+Version: 1.3.0
 Summary: A package for computing distances accounting for periodic boundary conditions
 Home-page: https://github.com/muexly/pbc_distance_calculator
 Author: Jacob Jeffries
 Author-email: jwjeffr@clemson.edu
 License: MIT
 Keywords: periodic-boundary-conditions,distance-computation,simulation,molecular-dynamics,lattice-systems,neighbor-lists,periodic-images
 Requires-Python: <=3.12,>=3.8
```

### Comparing `pbc_distance_calculator-1.2.1/README.md` & `pbc_distance_calculator-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pbc_distance_calculator-1.2.1/pbc_distance_calculator.egg-info/PKG-INFO` & `pbc_distance_calculator-1.3.0/pbc_distance_calculator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbc_distance_calculator
-Version: 1.2.1
+Version: 1.3.0
 Summary: A package for computing distances accounting for periodic boundary conditions
 Home-page: https://github.com/muexly/pbc_distance_calculator
 Author: Jacob Jeffries
 Author-email: jwjeffr@clemson.edu
 License: MIT
 Keywords: periodic-boundary-conditions,distance-computation,simulation,molecular-dynamics,lattice-systems,neighbor-lists,periodic-images
 Requires-Python: <=3.12,>=3.8
```

### Comparing `pbc_distance_calculator-1.2.1/setup.cfg` & `pbc_distance_calculator-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = pbc_distance_calculator
 author = Jacob Jeffries
 author_email = jwjeffr@clemson.edu
 url = https://github.com/muexly/pbc_distance_calculator
 long_description_content_type = text/markdown
 long_description = file: README.md
 description = A package for computing distances accounting for periodic boundary conditions
-version = 1.2.1
+version = 1.3.0
 license = MIT
 license_files = LICENSE
 keywords = 
 	periodic-boundary-conditions
 	distance-computation
 	simulation
 	molecular-dynamics
```
