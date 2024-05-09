# Comparing `tmp/ft2bt-0.2.7.tar.gz` & `tmp/ft2bt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft2bt-0.2.7.tar", last modified: Thu May  9 07:43:10 2024, max compression
+gzip compressed data, was "ft2bt-0.3.1.tar", last modified: Thu May  9 17:30:02 2024, max compression
```

## Comparing `ft2bt-0.2.7.tar` & `ft2bt-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.166310 ft2bt-0.2.7/
--rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-06 09:05:53.000000 ft2bt-0.2.7/LICENSE
--rw-rw-r--   0 tda       (1000) tda       (1000)       55 2024-05-08 16:23:08.000000 ft2bt-0.2.7/MANIFEST.in
--rw-r--r--   0 tda       (1000) tda       (1000)     5644 2024-05-09 07:43:10.166310 ft2bt-0.2.7/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)     4670 2024-05-08 16:29:53.000000 ft2bt-0.2.7/README.md
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.162310 ft2bt-0.2.7/ft2bt/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.7/ft2bt/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.162310 ft2bt-0.2.7/ft2bt/scripts/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.7/ft2bt/scripts/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.162310 ft2bt-0.2.7/ft2bt/scripts/behavior_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.7/ft2bt/scripts/behavior_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)    21197 2024-04-25 13:52:26.000000 ft2bt-0.2.7/ft2bt/scripts/behavior_trees/behavior_tree.py
--rw-rw-r--   0 tda       (1000) tda       (1000)      418 2024-04-11 05:51:28.000000 ft2bt-0.2.7/ft2bt/scripts/behavior_trees/behavior_tree_node.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.162310 ft2bt-0.2.7/ft2bt/scripts/code_generator/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.7/ft2bt/scripts/code_generator/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-06 09:05:53.000000 ft2bt-0.2.7/ft2bt/scripts/code_generator/code_generator.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-06 09:05:53.000000 ft2bt-0.2.7/ft2bt/scripts/code_generator/header_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-06 09:05:53.000000 ft2bt-0.2.7/ft2bt/scripts/code_generator/main_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-06 09:05:53.000000 ft2bt-0.2.7/ft2bt/scripts/code_generator/source_file.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.162310 ft2bt-0.2.7/ft2bt/scripts/fault_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.7/ft2bt/scripts/fault_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)    10354 2024-04-09 06:16:12.000000 ft2bt-0.2.7/ft2bt/scripts/fault_trees/xml_fta_parser.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     3962 2024-04-25 13:51:47.000000 ft2bt-0.2.7/ft2bt/scripts/ft2bt.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.162310 ft2bt-0.2.7/ft2bt/scripts/hara/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-05-09 06:26:07.000000 ft2bt-0.2.7/ft2bt/scripts/hara/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     1524 2024-04-25 07:18:48.000000 ft2bt-0.2.7/ft2bt/scripts/hara/hara_parser.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.162310 ft2bt-0.2.7/ft2bt/test/
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.162310 ft2bt-0.2.7/ft2bt/test/behavior_trees/
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.166310 ft2bt-0.2.7/ft2bt/test/behavior_trees/render/
--rw-rw-r--   0 tda       (1000) tda       (1000)    72026 2024-04-06 09:05:53.000000 ft2bt-0.2.7/ft2bt/test/behavior_trees/render/BT_hz_01.svg
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.166310 ft2bt-0.2.7/ft2bt/test/fault_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)    16664 2024-05-08 09:29:47.000000 ft2bt-0.2.7/ft2bt/test/fault_trees/fta_example.png
--rw-rw-r--   0 tda       (1000) tda       (1000)    11443 2024-04-11 06:50:12.000000 ft2bt-0.2.7/ft2bt/test/fault_trees/fta_example.xml
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.166310 ft2bt-0.2.7/ft2bt/test/hara/
--rw-rw-r--   0 tda       (1000) tda       (1000)    22944 2024-05-08 10:07:58.000000 ft2bt-0.2.7/ft2bt/test/hara/hara_example.png
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 07:43:10.166310 ft2bt-0.2.7/ft2bt.egg-info/
--rw-r--r--   0 tda       (1000) tda       (1000)     5644 2024-05-09 07:43:10.000000 ft2bt-0.2.7/ft2bt.egg-info/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)      958 2024-05-09 07:43:10.000000 ft2bt-0.2.7/ft2bt.egg-info/SOURCES.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-05-09 07:43:10.000000 ft2bt-0.2.7/ft2bt.egg-info/dependency_links.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-05-09 07:43:10.000000 ft2bt-0.2.7/ft2bt.egg-info/entry_points.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)      239 2024-05-09 07:43:10.000000 ft2bt-0.2.7/ft2bt.egg-info/requires.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-05-09 07:43:10.000000 ft2bt-0.2.7/ft2bt.egg-info/top_level.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)      238 2024-05-09 07:41:28.000000 ft2bt-0.2.7/requirements.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-05-09 07:43:10.166310 ft2bt-0.2.7/setup.cfg
--rw-rw-r--   0 tda       (1000) tda       (1000)      980 2024-05-09 07:43:08.000000 ft2bt-0.2.7/setup.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.760787 ft2bt-0.3.1/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-06 09:05:53.000000 ft2bt-0.3.1/LICENSE
+-rw-rw-r--   0 tda       (1000) tda       (1000)       55 2024-05-08 16:23:08.000000 ft2bt-0.3.1/MANIFEST.in
+-rw-rw-r--   0 tda       (1000) tda       (1000)     5973 2024-05-09 17:30:02.760787 ft2bt-0.3.1/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)     4766 2024-05-09 17:28:15.000000 ft2bt-0.3.1/README.md
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/scripts/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/scripts/behavior_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/behavior_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)    22627 2024-05-09 17:25:26.000000 ft2bt-0.3.1/ft2bt/scripts/behavior_trees/behavior_tree.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)      418 2024-04-11 05:51:28.000000 ft2bt-0.3.1/ft2bt/scripts/behavior_trees/behavior_tree_node.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/scripts/code_generator/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/code_generator/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/code_generator/code_generator.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/code_generator/header_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/code_generator/main_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/code_generator/source_file.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/scripts/fault_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/fault_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)    10354 2024-04-09 06:16:12.000000 ft2bt-0.3.1/ft2bt/scripts/fault_trees/xml_fta_parser.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     4134 2024-05-09 17:28:33.000000 ft2bt-0.3.1/ft2bt/scripts/ft2bt.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.760787 ft2bt-0.3.1/ft2bt/scripts/hara/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-05-09 06:26:07.000000 ft2bt-0.3.1/ft2bt/scripts/hara/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     1524 2024-04-25 07:18:48.000000 ft2bt-0.3.1/ft2bt/scripts/hara/hara_parser.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/test/
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/test/behavior_trees/
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.760787 ft2bt-0.3.1/ft2bt/test/behavior_trees/render/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    72026 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/test/behavior_trees/render/BT_hz_01.svg
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.760787 ft2bt-0.3.1/ft2bt/test/fault_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    16664 2024-05-08 09:29:47.000000 ft2bt-0.3.1/ft2bt/test/fault_trees/fta_example.png
+-rw-rw-r--   0 tda       (1000) tda       (1000)    11443 2024-04-11 06:50:12.000000 ft2bt-0.3.1/ft2bt/test/fault_trees/fta_example.xml
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.760787 ft2bt-0.3.1/ft2bt/test/hara/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    22944 2024-05-08 10:07:58.000000 ft2bt-0.3.1/ft2bt/test/hara/hara_example.png
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt.egg-info/
+-rw-r--r--   0 tda       (1000) tda       (1000)     5973 2024-05-09 17:30:02.000000 ft2bt-0.3.1/ft2bt.egg-info/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)      958 2024-05-09 17:30:02.000000 ft2bt-0.3.1/ft2bt.egg-info/SOURCES.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-05-09 17:30:02.000000 ft2bt-0.3.1/ft2bt.egg-info/dependency_links.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       52 2024-05-09 17:30:02.000000 ft2bt-0.3.1/ft2bt.egg-info/entry_points.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)      239 2024-05-09 17:30:02.000000 ft2bt-0.3.1/ft2bt.egg-info/requires.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-05-09 17:30:02.000000 ft2bt-0.3.1/ft2bt.egg-info/top_level.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)      238 2024-05-09 07:41:28.000000 ft2bt-0.3.1/requirements.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-05-09 17:30:02.760787 ft2bt-0.3.1/setup.cfg
+-rw-rw-r--   0 tda       (1000) tda       (1000)      980 2024-05-09 17:29:42.000000 ft2bt-0.3.1/setup.py
```

### Comparing `ft2bt-0.2.7/LICENSE` & `ft2bt-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.7/README.md` & `ft2bt-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -49,26 +49,27 @@
 </p>
 
 ### Running the Conversion Tool
 
 Run the conversion command:
 
 ```bash
-ft2bt [-h] -f FTA_FILEPATH [-v] [-c] [-r] [-o OUTPUT_FOLDER] [-p] [-H HARA_FILEPATH]
+ft2bt [-h] -f FTA_FILEPATH [-v] [-c] [-r] [-o OUTPUT_FOLDER] [-p] [-H HARA_FILEPATH] [-os]
 ```
 
 Where:
 
 * **-f**: (Required) Specifies the XML global filepath name of the draw.io diagram.
 * **-v**: (Optional) Automatically shows and saves the renders. Defaults to false.
 * **-c**: (Optional) Generate a cpp ROS node template for the behavior tree. Defaults to false.
 * **-r**: (Optional) Replaces current code if previously generated and -c is set to True.
 * **-o**: (Optional) Specifies the global folder path, where the behavior tree XML diagram is saved.
 * **-p**: (Optional) Probabilities are considered to sort the behavior tree nodes.
 * **-H**: (Optional) Specifies the CSV global file name of the Hazard Analysis and Risk Assessment (HARA).
+* **-os**: (Optional) Generate a BT that includes events to check the Operating Scenario.
 
 ### Output Example: Behavior Tree Diagram
 
 Below is an example of the behavior tree diagrams generated from the fault tree. The XML file is loaded using [Groot](https://github.com/BehaviorTree/Groot):
 
 The order of the events is randomly selected in this version of the software. Future versions will sort the events by probability of occurrence.
```

### Comparing `ft2bt-0.2.7/ft2bt/scripts/behavior_trees/behavior_tree.py` & `ft2bt-0.3.1/ft2bt/scripts/behavior_trees/behavior_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,21 @@
     Behavior tree class.
     Each behavior tree has a dictionary of nodes and a list of edges.
     
     Args:
         name (str, optional): Name of the behavior tree. Defaults to str().
         probabilistic (bool, optional): Whether the behavior tree is probabilistic. Defaults to False.
     """
-    def __init__(self, name=str(), probabilistic=False):
+    def __init__(self, name=str(), probabilistic=False, operating_scenario=False):
         self.nodes = dict()
         self.name = name
         self.event_number = int()
         self.action_number = int()
         self.probabilistic = probabilistic
+        self.operating_scenario = operating_scenario
         
         # Probabilistic behavior tree attributes
         if probabilistic:
             self.node_probabilities = dict()
             self.node_levels = dict()
             self.max_level = int()
             
@@ -282,47 +283,68 @@
         
         # Add a fallback node for the root node
         fallback_root_id = f'fallback_{self.name}'
         self.add_node(fallback_root_id, 'Fallback', label='Fallback')
         self.nodes[self.name].children.append(self.nodes[fallback_root_id])
         
         for operating_scenario_id, hazard_id_dict in hazard_dict.items():
-            # Add sequence node for each operating scenario
-            seq_operating_scenario_id = f'sequence_{operating_scenario_id}'
-            self.add_node(seq_operating_scenario_id, 'Sequence', label=seq_operating_scenario_id)
-            self.nodes[fallback_root_id].children.append(self.nodes[seq_operating_scenario_id])
-            
-            # Add operating scenario as a condition node
-            condition_operating_scenario_id = f'condition_{operating_scenario_id}'
-            self.add_node(condition_operating_scenario_id, 'Condition', label=condition_operating_scenario_id)
-            self.nodes[seq_operating_scenario_id].children.append(self.nodes[condition_operating_scenario_id])
-            
-            # Add operating scenario as a subtree node
-            self.add_node(operating_scenario_id, 'Subtree', label=operating_scenario_id)
-            self.nodes[seq_operating_scenario_id].children.append(self.nodes[operating_scenario_id])
-            hz_asil[seq_operating_scenario_id] = list()
-            
-            # Add FallBack node for each operating scenario
-            fallback_id = f'fallback_{operating_scenario_id}'
-            self.add_node(fallback_id, 'Fallback', label='Fallback')
-            self.nodes[operating_scenario_id].children.append(self.nodes[fallback_id])
+            if self.operating_scenario:
+                # Add sequence node for each operating scenario
+                seq_operating_scenario_id = f'sequence_{operating_scenario_id}'
+                self.add_node(seq_operating_scenario_id, 'Sequence', label=seq_operating_scenario_id)
+                self.nodes[fallback_root_id].children.append(self.nodes[seq_operating_scenario_id])
+                
+                # Add operating scenario as a condition node
+                condition_operating_scenario_id = f'condition_{operating_scenario_id}'
+                self.add_node(condition_operating_scenario_id, 'Condition', label=condition_operating_scenario_id)
+                self.nodes[seq_operating_scenario_id].children.append(self.nodes[condition_operating_scenario_id])
+                
+                # Add operating scenario as a subtree node
+                self.add_node(operating_scenario_id, 'Subtree', label=operating_scenario_id)
+                self.nodes[seq_operating_scenario_id].children.append(self.nodes[operating_scenario_id])
+                hz_asil[seq_operating_scenario_id] = list()
+                
+                # Add FallBack node for each operating scenario
+                fallback_id = f'fallback_{operating_scenario_id}'
+                self.add_node(fallback_id, 'Fallback', label='Fallback')
+                self.nodes[operating_scenario_id].children.append(self.nodes[fallback_id])
             
             for hazard_id, data in hazard_id_dict.items():
+                if not self.operating_scenario:
+                    seq_operating_scenario_id = f'sequence_{hazard_id}'
+                    fallback_id = fallback_root_id
+                    hz_asil[seq_operating_scenario_id] = list()
+                
                 # Get the ASIL and Safety State ID from the HARA data
                 asil = data['ASIL']
-                sequence_id = f'sequence_{hazard_id}_{operating_scenario_id}'
+                sequence_id = f'sequence_{hazard_id}_{operating_scenario_id}' if self.operating_scenario else f'sequence_{hazard_id}'
                 safety_state_id = data['Safety_State_ID']
                 hz_asil[seq_operating_scenario_id].append(asil)
                 
-                # Create a Sequence node for each operating scenario
-                self.add_node(sequence_id, 'Sequence', label='Sequence')
-                self.nodes[sequence_id].asil = asil
-                self.nodes[fallback_id].children.append(self.nodes[sequence_id])
+                if self.operating_scenario or sequence_id not in self.nodes.keys():
+                    # Create a Sequence node for each operating scenario and hazard
+                    self.add_node(sequence_id, 'Sequence', label='Sequence')
+                    self.nodes[sequence_id].asil = asil
+                    self.nodes[fallback_id].children.append(self.nodes[sequence_id])
+                    
+                elif asil > self.nodes[sequence_id].asil:
+                    # Update the ASIL level of the sequence node
+                    self.nodes[sequence_id].asil = asil
+                    
+                    # Remove the safety state node from the sequence node and add the new one
+                    self.nodes[sequence_id].children.remove(self.nodes[sequence_id].children[-1])
+                    safety_state_id = f'action_{safety_state_id}'
+                    self.add_node(safety_state_id, 'Action', label=safety_state_id)
+                    self.nodes[sequence_id].children.append(self.nodes[safety_state_id])
+                    continue
                 
-                # Add operating scenario as a condition node
+                else:
+                    continue
+                
+                # Add hazard and operating scenario as a condition node
                 hazard_id = f'{hazard_id}_{operating_scenario_id}'
                 self.add_node(hazard_id, 'Condition', label=hazard_id)
                 self.nodes[sequence_id].children.append(self.nodes[hazard_id])
                 
                 # Add safety state as an action node
                 safety_state_id = f'action_{safety_state_id}'
                 self.add_node(safety_state_id, 'Action', label=safety_state_id)
@@ -351,19 +373,18 @@
             # Get the HARA data for the root node
             if node.node_type == 'Root':
                 node.node_type = 'Subtree'
                 node.node_label = node_label + '_HARA'
                 for item in hara_dict.keys():
                     for operating_scenario in hara_dict[item].keys():
                         if node_label in hara_dict[item][operating_scenario].keys():
-                            id = f'sequence_{node_label}_{operating_scenario}'
+                            id = f'sequence_{node_label}_{operating_scenario}' if self.operating_scenario else f'sequence_{node_label}'
                             if id in self.nodes.keys():
                                 self.nodes[id].children.remove(self.nodes[id].children[0])
-                                self.nodes[id].children.insert(0, node)
-                                
+                                self.nodes[id].children.insert(0, node)                                
                                 
     def sort_nodes_asil(self, node_id):
         """
         Sort the nodes based on their ASIL
         
         Args:
             node_id (str): Node ID
```

### Comparing `ft2bt-0.2.7/ft2bt/scripts/code_generator/code_generator.py` & `ft2bt-0.3.1/ft2bt/scripts/code_generator/code_generator.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.7/ft2bt/scripts/code_generator/header_file.py` & `ft2bt-0.3.1/ft2bt/scripts/code_generator/header_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.7/ft2bt/scripts/code_generator/main_file.py` & `ft2bt-0.3.1/ft2bt/scripts/code_generator/main_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.7/ft2bt/scripts/code_generator/source_file.py` & `ft2bt-0.3.1/ft2bt/scripts/code_generator/source_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.7/ft2bt/scripts/fault_trees/xml_fta_parser.py` & `ft2bt-0.3.1/ft2bt/scripts/fault_trees/xml_fta_parser.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.7/ft2bt/scripts/ft2bt.py` & `ft2bt-0.3.1/ft2bt/scripts/ft2bt.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     parser.add_argument('-f', '--fta_filepath', type=str, help="*.xml fault tree global path", required=True)
     parser.add_argument('-v', '--view', action='store_true', help="View the behavior tree renders?")
     parser.add_argument('-c', '--generate_cpp', action='store_true', help="Generate C++ code template?")
     parser.add_argument('-r', '--replace', action='store_true', help="Replace existing files?")
     parser.add_argument('-o', '--output_folder', type=str, help="Output folder for the behavior trees.")
     parser.add_argument('-p', '--probabilistic', action='store_true', help="Generate probabilistic behavior trees.")
     parser.add_argument('-H', '--HARA_filepath', type=str, help="*.csv HARA file global path.", default=None, required=False)
+    parser.add_argument('-os', '--operating_scenario', action='store_true', help="Generate operating scenario behavior trees.")
     args = parser.parse_args()
     
     # Get the path to the package
     module_path = Path(__file__).resolve()
     package_path = module_path.parent.parent.parent
     hara_available = args.HARA_filepath is not None
     
@@ -46,15 +47,15 @@
     else:
         behavior_tree_folder = package_path / 'behavior_trees'
         
     # Read the HARA CSV file if it is provided
     if hara_available:
         hara_generator = HARAParser(hara_file=args.HARA_filepath)
         for item_id, hazard_dict in hara_generator.hara_dict.items():
-            bt_hara = BehaviorTree(name=item_id, probabilistic=args.probabilistic)
+            bt_hara = BehaviorTree(name=item_id, probabilistic=args.probabilistic, operating_scenario=args.operating_scenario)
             bt_hara.generate_from_hara(hazard_dict)
     
     for fta in fta_list:
         # Generate the behavior tree diagram from every fault tree diagram
         bt = BehaviorTree(name=fta.name, probabilistic=args.probabilistic)
         if prev_bt is None:
             prev_bt = bt
```

### Comparing `ft2bt-0.2.7/ft2bt/scripts/hara/hara_parser.py` & `ft2bt-0.3.1/ft2bt/scripts/hara/hara_parser.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.7/ft2bt/test/behavior_trees/render/BT_hz_01.svg` & `ft2bt-0.3.1/ft2bt/test/behavior_trees/render/BT_hz_01.svg`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.7/ft2bt/test/fault_trees/fta_example.png` & `ft2bt-0.3.1/ft2bt/test/fault_trees/fta_example.png`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.7/ft2bt/test/fault_trees/fta_example.xml` & `ft2bt-0.3.1/ft2bt/test/fault_trees/fta_example.xml`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.7/ft2bt/test/hara/hara_example.png` & `ft2bt-0.3.1/ft2bt/test/hara/hara_example.png`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.7/ft2bt.egg-info/SOURCES.txt` & `ft2bt-0.3.1/ft2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ft2bt-0.2.7/setup.py` & `ft2bt-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements.txt file
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='ft2bt',
-    version='0.2.7',
+    version='0.3.1',
     packages=find_packages(),
     install_requires=required,  # Use the list from requirements.txt
     entry_points={
         'console_scripts': [
             'ft2bt=ft2bt.scripts.ft2bt:main',
         ],
     },
```

