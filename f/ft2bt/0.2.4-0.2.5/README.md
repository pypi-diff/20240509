# Comparing `tmp/ft2bt-0.2.4.tar.gz` & `tmp/ft2bt-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft2bt-0.2.4.tar", last modified: Thu May  9 07:22:03 2024, max compression
+gzip compressed data, was "ft2bt-0.2.5.tar", last modified: Thu May  9 07:24:35 2024, max compression
```

## Comparing `ft2bt-0.2.4.tar` & `ft2bt-0.2.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/
--rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-06 09:05:53.000000 ft2bt-0.2.4/LICENSE
--rw-rw-r--   0 tda       (1000) tda       (1000)       55 2024-05-08 16:23:08.000000 ft2bt-0.2.4/MANIFEST.in
--rw-r--r--   0 tda       (1000) tda       (1000)     5276 2024-05-09 07:22:03.143424 ft2bt-0.2.4/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)     4670 2024-05-08 16:29:53.000000 ft2bt-0.2.4/README.md
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/ft2bt/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.4/ft2bt/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/ft2bt/scripts/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.4/ft2bt/scripts/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/ft2bt/scripts/behavior_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.4/ft2bt/scripts/behavior_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)    21197 2024-04-25 13:52:26.000000 ft2bt-0.2.4/ft2bt/scripts/behavior_trees/behavior_tree.py
--rw-rw-r--   0 tda       (1000) tda       (1000)      418 2024-04-11 05:51:28.000000 ft2bt-0.2.4/ft2bt/scripts/behavior_trees/behavior_tree_node.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/ft2bt/scripts/code_generator/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.4/ft2bt/scripts/code_generator/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-06 09:05:53.000000 ft2bt-0.2.4/ft2bt/scripts/code_generator/code_generator.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-06 09:05:53.000000 ft2bt-0.2.4/ft2bt/scripts/code_generator/header_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-06 09:05:53.000000 ft2bt-0.2.4/ft2bt/scripts/code_generator/main_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-06 09:05:53.000000 ft2bt-0.2.4/ft2bt/scripts/code_generator/source_file.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/ft2bt/scripts/fault_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.4/ft2bt/scripts/fault_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)    10354 2024-04-09 06:16:12.000000 ft2bt-0.2.4/ft2bt/scripts/fault_trees/xml_fta_parser.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     3962 2024-04-25 13:51:47.000000 ft2bt-0.2.4/ft2bt/scripts/ft2bt.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/ft2bt/scripts/hara/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-05-09 06:26:07.000000 ft2bt-0.2.4/ft2bt/scripts/hara/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     1524 2024-04-25 07:18:48.000000 ft2bt-0.2.4/ft2bt/scripts/hara/hara_parser.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/ft2bt/test/
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/ft2bt/test/behavior_trees/
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/ft2bt/test/behavior_trees/render/
--rw-rw-r--   0 tda       (1000) tda       (1000)    72026 2024-04-06 09:05:53.000000 ft2bt-0.2.4/ft2bt/test/behavior_trees/render/BT_hz_01.svg
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/ft2bt/test/fault_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)    16664 2024-05-08 09:29:47.000000 ft2bt-0.2.4/ft2bt/test/fault_trees/fta_example.png
--rw-rw-r--   0 tda       (1000) tda       (1000)    11443 2024-04-11 06:50:12.000000 ft2bt-0.2.4/ft2bt/test/fault_trees/fta_example.xml
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/ft2bt/test/hara/
--rw-rw-r--   0 tda       (1000) tda       (1000)    22944 2024-05-08 10:07:58.000000 ft2bt-0.2.4/ft2bt/test/hara/hara_example.png
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:22:03.143424 ft2bt-0.2.4/ft2bt.egg-info/
--rw-r--r--   0 tda       (1000) tda       (1000)     5276 2024-05-09 07:22:03.000000 ft2bt-0.2.4/ft2bt.egg-info/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)      958 2024-05-09 07:22:03.000000 ft2bt-0.2.4/ft2bt.egg-info/SOURCES.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-05-09 07:22:03.000000 ft2bt-0.2.4/ft2bt.egg-info/dependency_links.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-05-09 07:22:03.000000 ft2bt-0.2.4/ft2bt.egg-info/entry_points.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-05-09 07:22:03.000000 ft2bt-0.2.4/ft2bt.egg-info/requires.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-05-09 07:22:03.000000 ft2bt-0.2.4/ft2bt.egg-info/top_level.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       50 2024-05-09 07:21:13.000000 ft2bt-0.2.4/requirements.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-05-09 07:22:03.143424 ft2bt-0.2.4/setup.cfg
--rw-rw-r--   0 tda       (1000) tda       (1000)      980 2024-05-09 07:22:01.000000 ft2bt-0.2.4/setup.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.928211 ft2bt-0.2.5/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-06 09:05:53.000000 ft2bt-0.2.5/LICENSE
+-rw-rw-r--   0 tda       (1000) tda       (1000)       55 2024-05-08 16:23:08.000000 ft2bt-0.2.5/MANIFEST.in
+-rw-r--r--   0 tda       (1000) tda       (1000)     5579 2024-05-09 07:24:35.928211 ft2bt-0.2.5/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)     4670 2024-05-08 16:29:53.000000 ft2bt-0.2.5/README.md
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.924211 ft2bt-0.2.5/ft2bt/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.5/ft2bt/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.928211 ft2bt-0.2.5/ft2bt/scripts/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.5/ft2bt/scripts/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.928211 ft2bt-0.2.5/ft2bt/scripts/behavior_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.5/ft2bt/scripts/behavior_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)    21197 2024-04-25 13:52:26.000000 ft2bt-0.2.5/ft2bt/scripts/behavior_trees/behavior_tree.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)      418 2024-04-11 05:51:28.000000 ft2bt-0.2.5/ft2bt/scripts/behavior_trees/behavior_tree_node.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.928211 ft2bt-0.2.5/ft2bt/scripts/code_generator/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.5/ft2bt/scripts/code_generator/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-06 09:05:53.000000 ft2bt-0.2.5/ft2bt/scripts/code_generator/code_generator.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-06 09:05:53.000000 ft2bt-0.2.5/ft2bt/scripts/code_generator/header_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-06 09:05:53.000000 ft2bt-0.2.5/ft2bt/scripts/code_generator/main_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-06 09:05:53.000000 ft2bt-0.2.5/ft2bt/scripts/code_generator/source_file.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.928211 ft2bt-0.2.5/ft2bt/scripts/fault_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.5/ft2bt/scripts/fault_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)    10354 2024-04-09 06:16:12.000000 ft2bt-0.2.5/ft2bt/scripts/fault_trees/xml_fta_parser.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     3962 2024-04-25 13:51:47.000000 ft2bt-0.2.5/ft2bt/scripts/ft2bt.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.928211 ft2bt-0.2.5/ft2bt/scripts/hara/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-05-09 06:26:07.000000 ft2bt-0.2.5/ft2bt/scripts/hara/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     1524 2024-04-25 07:18:48.000000 ft2bt-0.2.5/ft2bt/scripts/hara/hara_parser.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.924211 ft2bt-0.2.5/ft2bt/test/
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.924211 ft2bt-0.2.5/ft2bt/test/behavior_trees/
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.928211 ft2bt-0.2.5/ft2bt/test/behavior_trees/render/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    72026 2024-04-06 09:05:53.000000 ft2bt-0.2.5/ft2bt/test/behavior_trees/render/BT_hz_01.svg
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.928211 ft2bt-0.2.5/ft2bt/test/fault_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    16664 2024-05-08 09:29:47.000000 ft2bt-0.2.5/ft2bt/test/fault_trees/fta_example.png
+-rw-rw-r--   0 tda       (1000) tda       (1000)    11443 2024-04-11 06:50:12.000000 ft2bt-0.2.5/ft2bt/test/fault_trees/fta_example.xml
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.928211 ft2bt-0.2.5/ft2bt/test/hara/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    22944 2024-05-08 10:07:58.000000 ft2bt-0.2.5/ft2bt/test/hara/hara_example.png
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:24:35.928211 ft2bt-0.2.5/ft2bt.egg-info/
+-rw-r--r--   0 tda       (1000) tda       (1000)     5579 2024-05-09 07:24:35.000000 ft2bt-0.2.5/ft2bt.egg-info/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)      958 2024-05-09 07:24:35.000000 ft2bt-0.2.5/ft2bt.egg-info/SOURCES.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-05-09 07:24:35.000000 ft2bt-0.2.5/ft2bt.egg-info/dependency_links.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-05-09 07:24:35.000000 ft2bt-0.2.5/ft2bt.egg-info/entry_points.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)      204 2024-05-09 07:24:35.000000 ft2bt-0.2.5/ft2bt.egg-info/requires.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-05-09 07:24:35.000000 ft2bt-0.2.5/ft2bt.egg-info/top_level.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)      203 2024-05-09 07:24:16.000000 ft2bt-0.2.5/requirements.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-05-09 07:24:35.928211 ft2bt-0.2.5/setup.cfg
+-rw-rw-r--   0 tda       (1000) tda       (1000)      980 2024-05-09 07:24:31.000000 ft2bt-0.2.5/setup.py
```

### Comparing `ft2bt-0.2.4/LICENSE` & `ft2bt-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/PKG-INFO` & `ft2bt-0.2.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: ft2bt
-Version: 0.2.4
-Summary: Automatic conversion from fault trees into behavior trees
-Home-page: https://github.com/cconejob/ft2bt_converter.git
-Author: Carlos Conejo
-Author-email: carlos.conejo@upc.edu
-License: GNU GPLv3
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: networkx>=2.8.8
-Requires-Dist: graphviz>=0.20.1
-Requires-Dist: matplotlib>=3.6.2
-
 # Fault Tree to Behavior Tree Converter
 
 ## Overview
 
 This project focuses on the conversion of fault trees, represented in draw.io diagram XML files, into behavior tree XML files compatible with the BehaviorTree.CPP library. It enables users to transform their fault tree diagrams into actionable behavior trees, facilitating integration with systems that utilize the BehaviorTree.CPP framework for managing complex behaviors.
 
 ## Installation
```

### Comparing `ft2bt-0.2.4/ft2bt/scripts/behavior_trees/behavior_tree.py` & `ft2bt-0.2.5/ft2bt/scripts/behavior_trees/behavior_tree.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/ft2bt/scripts/code_generator/code_generator.py` & `ft2bt-0.2.5/ft2bt/scripts/code_generator/code_generator.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/ft2bt/scripts/code_generator/header_file.py` & `ft2bt-0.2.5/ft2bt/scripts/code_generator/header_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/ft2bt/scripts/code_generator/main_file.py` & `ft2bt-0.2.5/ft2bt/scripts/code_generator/main_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/ft2bt/scripts/code_generator/source_file.py` & `ft2bt-0.2.5/ft2bt/scripts/code_generator/source_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/ft2bt/scripts/fault_trees/xml_fta_parser.py` & `ft2bt-0.2.5/ft2bt/scripts/fault_trees/xml_fta_parser.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/ft2bt/scripts/ft2bt.py` & `ft2bt-0.2.5/ft2bt/scripts/ft2bt.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/ft2bt/scripts/hara/hara_parser.py` & `ft2bt-0.2.5/ft2bt/scripts/hara/hara_parser.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/ft2bt/test/behavior_trees/render/BT_hz_01.svg` & `ft2bt-0.2.5/ft2bt/test/behavior_trees/render/BT_hz_01.svg`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/ft2bt/test/fault_trees/fta_example.png` & `ft2bt-0.2.5/ft2bt/test/fault_trees/fta_example.png`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/ft2bt/test/fault_trees/fta_example.xml` & `ft2bt-0.2.5/ft2bt/test/fault_trees/fta_example.xml`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/ft2bt/test/hara/hara_example.png` & `ft2bt-0.2.5/ft2bt/test/hara/hara_example.png`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/ft2bt.egg-info/PKG-INFO` & `ft2bt-0.2.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 Metadata-Version: 2.1
 Name: ft2bt
-Version: 0.2.4
+Version: 0.2.5
 Summary: Automatic conversion from fault trees into behavior trees
 Home-page: https://github.com/cconejob/ft2bt_converter.git
 Author: Carlos Conejo
 Author-email: carlos.conejo@upc.edu
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx>=2.8.8
 Requires-Dist: graphviz>=0.20.1
 Requires-Dist: matplotlib>=3.6.2
+Requires-Dist: cloudpickle>=1.3.0
+Requires-Dist: future>=0.18.2
+Requires-Dist: omegaconf>=2
+Requires-Dist: pycocotools>=2.0.2
+Requires-Dist: pydot>=1.4.1
+Requires-Dist: tabulate>=0.8.9
+Requires-Dist: tensorboard>=2.1.1
+Requires-Dist: termcolor>=1.1
+Requires-Dist: tqdm>4.29.0
+Requires-Dist: yacs>=0.1.6
 
 # Fault Tree to Behavior Tree Converter
 
 ## Overview
 
 This project focuses on the conversion of fault trees, represented in draw.io diagram XML files, into behavior tree XML files compatible with the BehaviorTree.CPP library. It enables users to transform their fault tree diagrams into actionable behavior trees, facilitating integration with systems that utilize the BehaviorTree.CPP framework for managing complex behaviors.
```

### Comparing `ft2bt-0.2.4/ft2bt.egg-info/SOURCES.txt` & `ft2bt-0.2.5/ft2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.4/setup.py` & `ft2bt-0.2.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements.txt file
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='ft2bt',
-    version='0.2.4',
+    version='0.2.5',
     packages=find_packages(),
     install_requires=required,  # Use the list from requirements.txt
     entry_points={
         'console_scripts': [
             'ft2bt=ft2bt.scripts.ft2bt:main',
         ],
     },
```

