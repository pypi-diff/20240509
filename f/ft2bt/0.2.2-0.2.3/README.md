# Comparing `tmp/ft2bt-0.2.2.tar.gz` & `tmp/ft2bt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft2bt-0.2.2.tar", last modified: Wed May  8 16:23:41 2024, max compression
+gzip compressed data, was "ft2bt-0.2.3.tar", last modified: Thu May  9 06:28:15 2024, max compression
```

## Comparing `ft2bt-0.2.2.tar` & `ft2bt-0.2.3.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 16:23:41.672784 ft2bt-0.2.2/
--rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-06 09:05:53.000000 ft2bt-0.2.2/LICENSE
--rw-rw-r--   0 tda       (1000) tda       (1000)       55 2024-05-08 16:23:08.000000 ft2bt-0.2.2/MANIFEST.in
--rw-r--r--   0 tda       (1000) tda       (1000)     5650 2024-05-08 16:23:41.672784 ft2bt-0.2.2/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)     4676 2024-05-08 12:26:20.000000 ft2bt-0.2.2/README.md
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 16:23:41.672784 ft2bt-0.2.2/ft2bt/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.2/ft2bt/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 16:23:41.672784 ft2bt-0.2.2/ft2bt/scripts/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.2/ft2bt/scripts/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 16:23:41.672784 ft2bt-0.2.2/ft2bt/scripts/behavior_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.2/ft2bt/scripts/behavior_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)    21197 2024-04-25 13:52:26.000000 ft2bt-0.2.2/ft2bt/scripts/behavior_trees/behavior_tree.py
--rw-rw-r--   0 tda       (1000) tda       (1000)      418 2024-04-11 05:51:28.000000 ft2bt-0.2.2/ft2bt/scripts/behavior_trees/behavior_tree_node.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 16:23:41.672784 ft2bt-0.2.2/ft2bt/scripts/code_generator/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.2/ft2bt/scripts/code_generator/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-06 09:05:53.000000 ft2bt-0.2.2/ft2bt/scripts/code_generator/code_generator.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-06 09:05:53.000000 ft2bt-0.2.2/ft2bt/scripts/code_generator/header_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-06 09:05:53.000000 ft2bt-0.2.2/ft2bt/scripts/code_generator/main_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-06 09:05:53.000000 ft2bt-0.2.2/ft2bt/scripts/code_generator/source_file.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 16:23:41.672784 ft2bt-0.2.2/ft2bt/scripts/fault_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.2/ft2bt/scripts/fault_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)    10354 2024-04-09 06:16:12.000000 ft2bt-0.2.2/ft2bt/scripts/fault_trees/xml_fta_parser.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     3962 2024-04-25 13:51:47.000000 ft2bt-0.2.2/ft2bt/scripts/ft2bt.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 16:23:41.668784 ft2bt-0.2.2/ft2bt/test/
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 16:23:41.668784 ft2bt-0.2.2/ft2bt/test/behavior_trees/
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 16:23:41.672784 ft2bt-0.2.2/ft2bt/test/behavior_trees/render/
--rw-rw-r--   0 tda       (1000) tda       (1000)    72026 2024-04-06 09:05:53.000000 ft2bt-0.2.2/ft2bt/test/behavior_trees/render/BT_hz_01.svg
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 16:23:41.672784 ft2bt-0.2.2/ft2bt/test/fault_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)    16664 2024-05-08 09:29:47.000000 ft2bt-0.2.2/ft2bt/test/fault_trees/fta_example.png
--rw-rw-r--   0 tda       (1000) tda       (1000)    11443 2024-04-11 06:50:12.000000 ft2bt-0.2.2/ft2bt/test/fault_trees/fta_example.xml
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 16:23:41.672784 ft2bt-0.2.2/ft2bt/test/hara/
--rw-rw-r--   0 tda       (1000) tda       (1000)    22944 2024-05-08 10:07:58.000000 ft2bt-0.2.2/ft2bt/test/hara/hara_example.png
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 16:23:41.672784 ft2bt-0.2.2/ft2bt.egg-info/
--rw-r--r--   0 tda       (1000) tda       (1000)     5650 2024-05-08 16:23:41.000000 ft2bt-0.2.2/ft2bt.egg-info/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)      893 2024-05-08 16:23:41.000000 ft2bt-0.2.2/ft2bt.egg-info/SOURCES.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-05-08 16:23:41.000000 ft2bt-0.2.2/ft2bt.egg-info/dependency_links.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-05-08 16:23:41.000000 ft2bt-0.2.2/ft2bt.egg-info/entry_points.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)      239 2024-05-08 16:23:41.000000 ft2bt-0.2.2/ft2bt.egg-info/requires.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-05-08 16:23:41.000000 ft2bt-0.2.2/ft2bt.egg-info/top_level.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)      238 2024-05-08 16:15:30.000000 ft2bt-0.2.2/requirements.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-05-08 16:23:41.672784 ft2bt-0.2.2/setup.cfg
--rw-rw-r--   0 tda       (1000) tda       (1000)      980 2024-05-08 16:23:29.000000 ft2bt-0.2.2/setup.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.013026 ft2bt-0.2.3/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-06 09:05:53.000000 ft2bt-0.2.3/LICENSE
+-rw-rw-r--   0 tda       (1000) tda       (1000)       55 2024-05-08 16:23:08.000000 ft2bt-0.2.3/MANIFEST.in
+-rw-r--r--   0 tda       (1000) tda       (1000)     5644 2024-05-09 06:28:15.013026 ft2bt-0.2.3/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)     4670 2024-05-08 16:29:53.000000 ft2bt-0.2.3/README.md
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.009026 ft2bt-0.2.3/ft2bt/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.3/ft2bt/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.009026 ft2bt-0.2.3/ft2bt/scripts/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.3/ft2bt/scripts/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.013026 ft2bt-0.2.3/ft2bt/scripts/behavior_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.3/ft2bt/scripts/behavior_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)    21197 2024-04-25 13:52:26.000000 ft2bt-0.2.3/ft2bt/scripts/behavior_trees/behavior_tree.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)      418 2024-04-11 05:51:28.000000 ft2bt-0.2.3/ft2bt/scripts/behavior_trees/behavior_tree_node.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.013026 ft2bt-0.2.3/ft2bt/scripts/code_generator/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.3/ft2bt/scripts/code_generator/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-06 09:05:53.000000 ft2bt-0.2.3/ft2bt/scripts/code_generator/code_generator.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-06 09:05:53.000000 ft2bt-0.2.3/ft2bt/scripts/code_generator/header_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-06 09:05:53.000000 ft2bt-0.2.3/ft2bt/scripts/code_generator/main_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-06 09:05:53.000000 ft2bt-0.2.3/ft2bt/scripts/code_generator/source_file.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.013026 ft2bt-0.2.3/ft2bt/scripts/fault_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.3/ft2bt/scripts/fault_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)    10354 2024-04-09 06:16:12.000000 ft2bt-0.2.3/ft2bt/scripts/fault_trees/xml_fta_parser.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     3962 2024-04-25 13:51:47.000000 ft2bt-0.2.3/ft2bt/scripts/ft2bt.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.013026 ft2bt-0.2.3/ft2bt/scripts/hara/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-05-09 06:26:07.000000 ft2bt-0.2.3/ft2bt/scripts/hara/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     1524 2024-04-25 07:18:48.000000 ft2bt-0.2.3/ft2bt/scripts/hara/hara_parser.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.009026 ft2bt-0.2.3/ft2bt/test/
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.009026 ft2bt-0.2.3/ft2bt/test/behavior_trees/
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.013026 ft2bt-0.2.3/ft2bt/test/behavior_trees/render/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    72026 2024-04-06 09:05:53.000000 ft2bt-0.2.3/ft2bt/test/behavior_trees/render/BT_hz_01.svg
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.013026 ft2bt-0.2.3/ft2bt/test/fault_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    16664 2024-05-08 09:29:47.000000 ft2bt-0.2.3/ft2bt/test/fault_trees/fta_example.png
+-rw-rw-r--   0 tda       (1000) tda       (1000)    11443 2024-04-11 06:50:12.000000 ft2bt-0.2.3/ft2bt/test/fault_trees/fta_example.xml
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.013026 ft2bt-0.2.3/ft2bt/test/hara/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    22944 2024-05-08 10:07:58.000000 ft2bt-0.2.3/ft2bt/test/hara/hara_example.png
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 06:28:15.013026 ft2bt-0.2.3/ft2bt.egg-info/
+-rw-r--r--   0 tda       (1000) tda       (1000)     5644 2024-05-09 06:28:14.000000 ft2bt-0.2.3/ft2bt.egg-info/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)      958 2024-05-09 06:28:14.000000 ft2bt-0.2.3/ft2bt.egg-info/SOURCES.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-05-09 06:28:14.000000 ft2bt-0.2.3/ft2bt.egg-info/dependency_links.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-05-09 06:28:14.000000 ft2bt-0.2.3/ft2bt.egg-info/entry_points.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)      239 2024-05-09 06:28:14.000000 ft2bt-0.2.3/ft2bt.egg-info/requires.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-05-09 06:28:14.000000 ft2bt-0.2.3/ft2bt.egg-info/top_level.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)      238 2024-05-08 16:15:30.000000 ft2bt-0.2.3/requirements.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-05-09 06:28:15.013026 ft2bt-0.2.3/setup.cfg
+-rw-rw-r--   0 tda       (1000) tda       (1000)      980 2024-05-09 06:28:13.000000 ft2bt-0.2.3/setup.py
```

### Comparing `ft2bt-0.2.2/LICENSE` & `ft2bt-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.2/PKG-INFO` & `ft2bt-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft2bt
-Version: 0.2.2
+Version: 0.2.3
 Summary: Automatic conversion from fault trees into behavior trees
 Home-page: https://github.com/cconejob/ft2bt_converter.git
 Author: Carlos Conejo
 Author-email: carlos.conejo@upc.edu
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -71,15 +71,15 @@
 1. **Item_ID**: Identificator of the Item analyzed.
 2. **Hazard_ID**:  Identificator of the possible Hazard. The ID must match with the name of the correspondent Hazard in the Fault Tree.
 3. **Operating_Scenario_ID**: Identificator of the Operating Scenario.
 4. **ASIL**: Automotive Safety Integrity Level. Options: A, B, C, D
 5. **Safety_State_ID**: Identificator of the Safety State action.
 
 <p align="center">
-  <img src="ft2bt/test/hara/hara_example.png" alt="Fault Tree Example">
+  <img src="ft2bt/test/hara/hara_example.png" alt="HARA Example">
 </p>
 
 ### Running the Conversion Tool
 
 Run the conversion command:
 
 ```bash
```

### Comparing `ft2bt-0.2.2/README.md` & `ft2bt-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 1. **Item_ID**: Identificator of the Item analyzed.
 2. **Hazard_ID**:  Identificator of the possible Hazard. The ID must match with the name of the correspondent Hazard in the Fault Tree.
 3. **Operating_Scenario_ID**: Identificator of the Operating Scenario.
 4. **ASIL**: Automotive Safety Integrity Level. Options: A, B, C, D
 5. **Safety_State_ID**: Identificator of the Safety State action.
 
 <p align="center">
-  <img src="ft2bt/test/hara/hara_example.png" alt="Fault Tree Example">
+  <img src="ft2bt/test/hara/hara_example.png" alt="HARA Example">
 </p>
 
 ### Running the Conversion Tool
 
 Run the conversion command:
 
 ```bash
```

### Comparing `ft2bt-0.2.2/ft2bt/scripts/behavior_trees/behavior_tree.py` & `ft2bt-0.2.3/ft2bt/scripts/behavior_trees/behavior_tree.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.2/ft2bt/scripts/code_generator/code_generator.py` & `ft2bt-0.2.3/ft2bt/scripts/code_generator/code_generator.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.2/ft2bt/scripts/code_generator/header_file.py` & `ft2bt-0.2.3/ft2bt/scripts/code_generator/header_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.2/ft2bt/scripts/code_generator/main_file.py` & `ft2bt-0.2.3/ft2bt/scripts/code_generator/main_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.2/ft2bt/scripts/code_generator/source_file.py` & `ft2bt-0.2.3/ft2bt/scripts/code_generator/source_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.2/ft2bt/scripts/fault_trees/xml_fta_parser.py` & `ft2bt-0.2.3/ft2bt/scripts/fault_trees/xml_fta_parser.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.2/ft2bt/scripts/ft2bt.py` & `ft2bt-0.2.3/ft2bt/scripts/ft2bt.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.2/ft2bt/test/behavior_trees/render/BT_hz_01.svg` & `ft2bt-0.2.3/ft2bt/test/behavior_trees/render/BT_hz_01.svg`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.2/ft2bt/test/fault_trees/fta_example.png` & `ft2bt-0.2.3/ft2bt/test/fault_trees/fta_example.png`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.2/ft2bt/test/fault_trees/fta_example.xml` & `ft2bt-0.2.3/ft2bt/test/fault_trees/fta_example.xml`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.2/ft2bt/test/hara/hara_example.png` & `ft2bt-0.2.3/ft2bt/test/hara/hara_example.png`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.2/ft2bt.egg-info/PKG-INFO` & `ft2bt-0.2.3/ft2bt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft2bt
-Version: 0.2.2
+Version: 0.2.3
 Summary: Automatic conversion from fault trees into behavior trees
 Home-page: https://github.com/cconejob/ft2bt_converter.git
 Author: Carlos Conejo
 Author-email: carlos.conejo@upc.edu
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -71,15 +71,15 @@
 1. **Item_ID**: Identificator of the Item analyzed.
 2. **Hazard_ID**:  Identificator of the possible Hazard. The ID must match with the name of the correspondent Hazard in the Fault Tree.
 3. **Operating_Scenario_ID**: Identificator of the Operating Scenario.
 4. **ASIL**: Automotive Safety Integrity Level. Options: A, B, C, D
 5. **Safety_State_ID**: Identificator of the Safety State action.
 
 <p align="center">
-  <img src="ft2bt/test/hara/hara_example.png" alt="Fault Tree Example">
+  <img src="ft2bt/test/hara/hara_example.png" alt="HARA Example">
 </p>
 
 ### Running the Conversion Tool
 
 Run the conversion command:
 
 ```bash
```

### Comparing `ft2bt-0.2.2/ft2bt.egg-info/SOURCES.txt` & `ft2bt-0.2.3/ft2bt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,11 +18,13 @@
 ft2bt/scripts/code_generator/__init__.py
 ft2bt/scripts/code_generator/code_generator.py
 ft2bt/scripts/code_generator/header_file.py
 ft2bt/scripts/code_generator/main_file.py
 ft2bt/scripts/code_generator/source_file.py
 ft2bt/scripts/fault_trees/__init__.py
 ft2bt/scripts/fault_trees/xml_fta_parser.py
+ft2bt/scripts/hara/__init__.py
+ft2bt/scripts/hara/hara_parser.py
 ft2bt/test/behavior_trees/render/BT_hz_01.svg
 ft2bt/test/fault_trees/fta_example.png
 ft2bt/test/fault_trees/fta_example.xml
 ft2bt/test/hara/hara_example.png
```

### Comparing `ft2bt-0.2.2/setup.py` & `ft2bt-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements.txt file
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='ft2bt',
-    version='0.2.2',
+    version='0.2.3',
     packages=find_packages(),
     install_requires=required,  # Use the list from requirements.txt
     entry_points={
         'console_scripts': [
             'ft2bt=ft2bt.scripts.ft2bt:main',
         ],
     },
```

