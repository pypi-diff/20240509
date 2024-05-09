# Comparing `tmp/toil_batch_system_tes-0.0.1.tar.gz` & `tmp/toil_batch_system_tes-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toil_batch_system_tes-0.0.1.tar", last modified: Thu Oct 26 18:53:35 2023, max compression
+gzip compressed data, was "toil_batch_system_tes-1.0.0.tar", last modified: Thu May  9 18:40:50 2024, max compression
```

## Comparing `toil_batch_system_tes-0.0.1.tar` & `toil_batch_system_tes-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 anovak     (503) staff       (20)        0 2023-10-26 18:53:35.574344 toil_batch_system_tes-0.0.1/
--rw-r--r--   0 anovak     (503) staff       (20)    11516 2023-10-26 18:12:24.000000 toil_batch_system_tes-0.0.1/LICENSE
--rw-r--r--   0 anovak     (503) staff       (20)     3131 2023-10-26 18:53:35.574266 toil_batch_system_tes-0.0.1/PKG-INFO
--rw-r--r--   0 anovak     (503) staff       (20)     2705 2023-10-26 18:49:52.000000 toil_batch_system_tes-0.0.1/README.md
--rw-r--r--   0 anovak     (503) staff       (20)      430 2023-10-26 18:51:50.000000 toil_batch_system_tes-0.0.1/pyproject.toml
--rw-r--r--   0 anovak     (503) staff       (20)      384 2023-10-26 18:53:35.574609 toil_batch_system_tes-0.0.1/setup.cfg
-drwxr-xr-x   0 anovak     (503) staff       (20)        0 2023-10-26 18:53:35.571470 toil_batch_system_tes-0.0.1/src/
-drwxr-xr-x   0 anovak     (503) staff       (20)        0 2023-10-26 18:53:35.572636 toil_batch_system_tes-0.0.1/src/toil_batch_system_tes/
--rw-r--r--   0 anovak     (503) staff       (20)      478 2023-10-26 18:23:38.000000 toil_batch_system_tes-0.0.1/src/toil_batch_system_tes/__init__.py
--rw-r--r--   0 anovak     (503) staff       (20)    20094 2023-10-26 17:28:45.000000 toil_batch_system_tes-0.0.1/src/toil_batch_system_tes/tes_batch_system.py
-drwxr-xr-x   0 anovak     (503) staff       (20)        0 2023-10-26 18:53:35.573911 toil_batch_system_tes-0.0.1/src/toil_batch_system_tes/test/
--rw-r--r--   0 anovak     (503) staff       (20)     1651 2023-10-26 18:32:06.000000 toil_batch_system_tes-0.0.1/src/toil_batch_system_tes/test/__init__.py
--rw-r--r--   0 anovak     (503) staff       (20)     1353 2023-10-26 18:00:13.000000 toil_batch_system_tes-0.0.1/src/toil_batch_system_tes/test/test.py
-drwxr-xr-x   0 anovak     (503) staff       (20)        0 2023-10-26 18:53:35.573557 toil_batch_system_tes-0.0.1/src/toil_batch_system_tes.egg-info/
--rw-r--r--   0 anovak     (503) staff       (20)     3131 2023-10-26 18:53:35.000000 toil_batch_system_tes-0.0.1/src/toil_batch_system_tes.egg-info/PKG-INFO
--rw-r--r--   0 anovak     (503) staff       (20)      452 2023-10-26 18:53:35.000000 toil_batch_system_tes-0.0.1/src/toil_batch_system_tes.egg-info/SOURCES.txt
--rw-r--r--   0 anovak     (503) staff       (20)        1 2023-10-26 18:53:35.000000 toil_batch_system_tes-0.0.1/src/toil_batch_system_tes.egg-info/dependency_links.txt
--rw-r--r--   0 anovak     (503) staff       (20)       32 2023-10-26 18:53:35.000000 toil_batch_system_tes-0.0.1/src/toil_batch_system_tes.egg-info/requires.txt
--rw-r--r--   0 anovak     (503) staff       (20)       22 2023-10-26 18:53:35.000000 toil_batch_system_tes-0.0.1/src/toil_batch_system_tes.egg-info/top_level.txt
+drwxr-xr-x   0 anovak     (503) staff       (20)        0 2024-05-09 18:40:50.865786 toil_batch_system_tes-1.0.0/
+-rw-r--r--   0 anovak     (503) staff       (20)    11516 2023-10-26 18:12:24.000000 toil_batch_system_tes-1.0.0/LICENSE
+-rw-r--r--   0 anovak     (503) staff       (20)     3204 2024-05-09 18:40:50.865697 toil_batch_system_tes-1.0.0/PKG-INFO
+-rw-r--r--   0 anovak     (503) staff       (20)     2773 2023-10-26 18:59:40.000000 toil_batch_system_tes-1.0.0/README.md
+-rw-r--r--   0 anovak     (503) staff       (20)      435 2024-05-09 18:24:12.000000 toil_batch_system_tes-1.0.0/pyproject.toml
+-rw-r--r--   0 anovak     (503) staff       (20)      384 2024-05-09 18:40:50.866120 toil_batch_system_tes-1.0.0/setup.cfg
+drwxr-xr-x   0 anovak     (503) staff       (20)        0 2024-05-09 18:40:50.860714 toil_batch_system_tes-1.0.0/src/
+drwxr-xr-x   0 anovak     (503) staff       (20)        0 2024-05-09 18:40:50.862897 toil_batch_system_tes-1.0.0/src/toil_batch_system_tes/
+-rw-r--r--   0 anovak     (503) staff       (20)      478 2024-05-09 18:24:12.000000 toil_batch_system_tes-1.0.0/src/toil_batch_system_tes/__init__.py
+-rw-r--r--   0 anovak     (503) staff       (20)    20094 2023-10-26 17:28:45.000000 toil_batch_system_tes-1.0.0/src/toil_batch_system_tes/tes_batch_system.py
+drwxr-xr-x   0 anovak     (503) staff       (20)        0 2024-05-09 18:40:50.865019 toil_batch_system_tes-1.0.0/src/toil_batch_system_tes/test/
+-rw-r--r--   0 anovak     (503) staff       (20)     1651 2023-10-26 18:32:06.000000 toil_batch_system_tes-1.0.0/src/toil_batch_system_tes/test/__init__.py
+-rw-r--r--   0 anovak     (503) staff       (20)     1353 2023-10-26 18:00:13.000000 toil_batch_system_tes-1.0.0/src/toil_batch_system_tes/test/test.py
+drwxr-xr-x   0 anovak     (503) staff       (20)        0 2024-05-09 18:40:50.865384 toil_batch_system_tes-1.0.0/src/toil_batch_system_tes.egg-info/
+-rw-r--r--   0 anovak     (503) staff       (20)     3204 2024-05-09 18:40:50.000000 toil_batch_system_tes-1.0.0/src/toil_batch_system_tes.egg-info/PKG-INFO
+-rw-r--r--   0 anovak     (503) staff       (20)      452 2024-05-09 18:40:50.000000 toil_batch_system_tes-1.0.0/src/toil_batch_system_tes.egg-info/SOURCES.txt
+-rw-r--r--   0 anovak     (503) staff       (20)        1 2024-05-09 18:40:50.000000 toil_batch_system_tes-1.0.0/src/toil_batch_system_tes.egg-info/dependency_links.txt
+-rw-r--r--   0 anovak     (503) staff       (20)       37 2024-05-09 18:40:50.000000 toil_batch_system_tes-1.0.0/src/toil_batch_system_tes.egg-info/requires.txt
+-rw-r--r--   0 anovak     (503) staff       (20)       22 2024-05-09 18:40:50.000000 toil_batch_system_tes-1.0.0/src/toil_batch_system_tes.egg-info/top_level.txt
```

### Comparing `toil_batch_system_tes-0.0.1/LICENSE` & `toil_batch_system_tes-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toil_batch_system_tes-0.0.1/PKG-INFO` & `toil_batch_system_tes-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: toil_batch_system_tes
-Version: 0.0.1
+Version: 1.0.0
 Summary: A TES batch system plugin for Toil
 Author-email: Adam Novak <anovak@soe.ucsc.edu>
 Project-URL: Homepage, https://github.com/adamnovak/toil_batch_system_tes
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: toil[aws]>5.12
+Requires-Dist: toil[aws]<6.2,>5.12
 Requires-Dist: py-tes<1,>=0.4.2
 
 # Toil TES Batch System
 
+Find us on [PyPI](https://pypi.org/project/toil-batch-system-tes)!
+
 This package contains the TES batch system implementation that was removed from
 Toil after version 5.12. It allows the [Toil workflow engine](https://toil.readthedocs.io/en/latest/)
 to run workflows on servers that implement [the GA4GH Task Execution Schemas API](https://github.com/ga4gh/task-execution-schemas).
 
 If you intall it, newer versions of Toil will pick up that it is installed, import it, and allow you to use it with `--batchSystem tes`.
 
 ## Installation
```

### Comparing `toil_batch_system_tes-0.0.1/README.md` & `toil_batch_system_tes-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Toil TES Batch System
 
+Find us on [PyPI](https://pypi.org/project/toil-batch-system-tes)!
+
 This package contains the TES batch system implementation that was removed from
 Toil after version 5.12. It allows the [Toil workflow engine](https://toil.readthedocs.io/en/latest/)
 to run workflows on servers that implement [the GA4GH Task Execution Schemas API](https://github.com/ga4gh/task-execution-schemas).
 
 If you intall it, newer versions of Toil will pick up that it is installed, import it, and allow you to use it with `--batchSystem tes`.
 
 ## Installation
```

### Comparing `toil_batch_system_tes-0.0.1/src/toil_batch_system_tes/tes_batch_system.py` & `toil_batch_system_tes-1.0.0/src/toil_batch_system_tes/tes_batch_system.py`

 * *Files identical despite different names*

### Comparing `toil_batch_system_tes-0.0.1/src/toil_batch_system_tes/test/__init__.py` & `toil_batch_system_tes-1.0.0/src/toil_batch_system_tes/test/__init__.py`

 * *Files identical despite different names*

### Comparing `toil_batch_system_tes-0.0.1/src/toil_batch_system_tes/test/test.py` & `toil_batch_system_tes-1.0.0/src/toil_batch_system_tes/test/test.py`

 * *Files identical despite different names*

### Comparing `toil_batch_system_tes-0.0.1/src/toil_batch_system_tes.egg-info/PKG-INFO` & `toil_batch_system_tes-1.0.0/src/toil_batch_system_tes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
-Name: toil-batch-system-tes
-Version: 0.0.1
+Name: toil_batch_system_tes
+Version: 1.0.0
 Summary: A TES batch system plugin for Toil
 Author-email: Adam Novak <anovak@soe.ucsc.edu>
 Project-URL: Homepage, https://github.com/adamnovak/toil_batch_system_tes
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: toil[aws]>5.12
+Requires-Dist: toil[aws]<6.2,>5.12
 Requires-Dist: py-tes<1,>=0.4.2
 
 # Toil TES Batch System
 
+Find us on [PyPI](https://pypi.org/project/toil-batch-system-tes)!
+
 This package contains the TES batch system implementation that was removed from
 Toil after version 5.12. It allows the [Toil workflow engine](https://toil.readthedocs.io/en/latest/)
 to run workflows on servers that implement [the GA4GH Task Execution Schemas API](https://github.com/ga4gh/task-execution-schemas).
 
 If you intall it, newer versions of Toil will pick up that it is installed, import it, and allow you to use it with `--batchSystem tes`.
 
 ## Installation
```

