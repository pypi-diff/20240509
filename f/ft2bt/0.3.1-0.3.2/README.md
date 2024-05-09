# Comparing `tmp/ft2bt-0.3.1.tar.gz` & `tmp/ft2bt-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft2bt-0.3.1.tar", last modified: Thu May  9 17:30:02 2024, max compression
+gzip compressed data, was "ft2bt-0.3.2.tar", last modified: Thu May  9 17:36:26 2024, max compression
```

## Comparing `ft2bt-0.3.1.tar` & `ft2bt-0.3.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.760787 ft2bt-0.3.1/
--rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-06 09:05:53.000000 ft2bt-0.3.1/LICENSE
--rw-rw-r--   0 tda       (1000) tda       (1000)       55 2024-05-08 16:23:08.000000 ft2bt-0.3.1/MANIFEST.in
--rw-rw-r--   0 tda       (1000) tda       (1000)     5973 2024-05-09 17:30:02.760787 ft2bt-0.3.1/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)     4766 2024-05-09 17:28:15.000000 ft2bt-0.3.1/README.md
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/scripts/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/scripts/behavior_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/behavior_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)    22627 2024-05-09 17:25:26.000000 ft2bt-0.3.1/ft2bt/scripts/behavior_trees/behavior_tree.py
--rw-rw-r--   0 tda       (1000) tda       (1000)      418 2024-04-11 05:51:28.000000 ft2bt-0.3.1/ft2bt/scripts/behavior_trees/behavior_tree_node.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/scripts/code_generator/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/code_generator/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/code_generator/code_generator.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/code_generator/header_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/code_generator/main_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/code_generator/source_file.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/scripts/fault_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/scripts/fault_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)    10354 2024-04-09 06:16:12.000000 ft2bt-0.3.1/ft2bt/scripts/fault_trees/xml_fta_parser.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     4134 2024-05-09 17:28:33.000000 ft2bt-0.3.1/ft2bt/scripts/ft2bt.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.760787 ft2bt-0.3.1/ft2bt/scripts/hara/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-05-09 06:26:07.000000 ft2bt-0.3.1/ft2bt/scripts/hara/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     1524 2024-04-25 07:18:48.000000 ft2bt-0.3.1/ft2bt/scripts/hara/hara_parser.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/test/
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt/test/behavior_trees/
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.760787 ft2bt-0.3.1/ft2bt/test/behavior_trees/render/
--rw-rw-r--   0 tda       (1000) tda       (1000)    72026 2024-04-06 09:05:53.000000 ft2bt-0.3.1/ft2bt/test/behavior_trees/render/BT_hz_01.svg
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.760787 ft2bt-0.3.1/ft2bt/test/fault_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)    16664 2024-05-08 09:29:47.000000 ft2bt-0.3.1/ft2bt/test/fault_trees/fta_example.png
--rw-rw-r--   0 tda       (1000) tda       (1000)    11443 2024-04-11 06:50:12.000000 ft2bt-0.3.1/ft2bt/test/fault_trees/fta_example.xml
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.760787 ft2bt-0.3.1/ft2bt/test/hara/
--rw-rw-r--   0 tda       (1000) tda       (1000)    22944 2024-05-08 10:07:58.000000 ft2bt-0.3.1/ft2bt/test/hara/hara_example.png
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:30:02.756787 ft2bt-0.3.1/ft2bt.egg-info/
--rw-r--r--   0 tda       (1000) tda       (1000)     5973 2024-05-09 17:30:02.000000 ft2bt-0.3.1/ft2bt.egg-info/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)      958 2024-05-09 17:30:02.000000 ft2bt-0.3.1/ft2bt.egg-info/SOURCES.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-05-09 17:30:02.000000 ft2bt-0.3.1/ft2bt.egg-info/dependency_links.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       52 2024-05-09 17:30:02.000000 ft2bt-0.3.1/ft2bt.egg-info/entry_points.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)      239 2024-05-09 17:30:02.000000 ft2bt-0.3.1/ft2bt.egg-info/requires.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-05-09 17:30:02.000000 ft2bt-0.3.1/ft2bt.egg-info/top_level.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)      238 2024-05-09 07:41:28.000000 ft2bt-0.3.1/requirements.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-05-09 17:30:02.760787 ft2bt-0.3.1/setup.cfg
--rw-rw-r--   0 tda       (1000) tda       (1000)      980 2024-05-09 17:29:42.000000 ft2bt-0.3.1/setup.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-06 09:05:53.000000 ft2bt-0.3.2/LICENSE
+-rw-rw-r--   0 tda       (1000) tda       (1000)       55 2024-05-08 16:23:08.000000 ft2bt-0.3.2/MANIFEST.in
+-rw-rw-r--   0 tda       (1000) tda       (1000)     6243 2024-05-09 17:36:26.478817 ft2bt-0.3.2/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)     5036 2024-05-09 17:35:27.000000 ft2bt-0.3.2/README.md
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/ft2bt/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.2/ft2bt/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/ft2bt/scripts/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.2/ft2bt/scripts/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/ft2bt/scripts/behavior_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.2/ft2bt/scripts/behavior_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)    22627 2024-05-09 17:25:26.000000 ft2bt-0.3.2/ft2bt/scripts/behavior_trees/behavior_tree.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)      418 2024-04-11 05:51:28.000000 ft2bt-0.3.2/ft2bt/scripts/behavior_trees/behavior_tree_node.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/ft2bt/scripts/code_generator/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.2/ft2bt/scripts/code_generator/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-06 09:05:53.000000 ft2bt-0.3.2/ft2bt/scripts/code_generator/code_generator.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-06 09:05:53.000000 ft2bt-0.3.2/ft2bt/scripts/code_generator/header_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-06 09:05:53.000000 ft2bt-0.3.2/ft2bt/scripts/code_generator/main_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-06 09:05:53.000000 ft2bt-0.3.2/ft2bt/scripts/code_generator/source_file.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/ft2bt/scripts/fault_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.3.2/ft2bt/scripts/fault_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)    10354 2024-04-09 06:16:12.000000 ft2bt-0.3.2/ft2bt/scripts/fault_trees/xml_fta_parser.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     4134 2024-05-09 17:28:33.000000 ft2bt-0.3.2/ft2bt/scripts/ft2bt.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/ft2bt/scripts/hara/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-05-09 06:26:07.000000 ft2bt-0.3.2/ft2bt/scripts/hara/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     1524 2024-04-25 07:18:48.000000 ft2bt-0.3.2/ft2bt/scripts/hara/hara_parser.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/ft2bt/test/
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/ft2bt/test/behavior_trees/
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/ft2bt/test/behavior_trees/render/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    72026 2024-04-06 09:05:53.000000 ft2bt-0.3.2/ft2bt/test/behavior_trees/render/BT_hz_01.svg
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/ft2bt/test/fault_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    16664 2024-05-08 09:29:47.000000 ft2bt-0.3.2/ft2bt/test/fault_trees/fta_example.png
+-rw-rw-r--   0 tda       (1000) tda       (1000)    11443 2024-04-11 06:50:12.000000 ft2bt-0.3.2/ft2bt/test/fault_trees/fta_example.xml
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/ft2bt/test/hara/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    22944 2024-05-08 10:07:58.000000 ft2bt-0.3.2/ft2bt/test/hara/hara_example.png
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-09 17:36:26.478817 ft2bt-0.3.2/ft2bt.egg-info/
+-rw-r--r--   0 tda       (1000) tda       (1000)     6243 2024-05-09 17:36:26.000000 ft2bt-0.3.2/ft2bt.egg-info/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)      958 2024-05-09 17:36:26.000000 ft2bt-0.3.2/ft2bt.egg-info/SOURCES.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-05-09 17:36:26.000000 ft2bt-0.3.2/ft2bt.egg-info/dependency_links.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       52 2024-05-09 17:36:26.000000 ft2bt-0.3.2/ft2bt.egg-info/entry_points.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)      239 2024-05-09 17:36:26.000000 ft2bt-0.3.2/ft2bt.egg-info/requires.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-05-09 17:36:26.000000 ft2bt-0.3.2/ft2bt.egg-info/top_level.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)      238 2024-05-09 07:41:28.000000 ft2bt-0.3.2/requirements.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-05-09 17:36:26.478817 ft2bt-0.3.2/setup.cfg
+-rw-rw-r--   0 tda       (1000) tda       (1000)      980 2024-05-09 17:36:20.000000 ft2bt-0.3.2/setup.py
```

### Comparing `ft2bt-0.3.1/LICENSE` & `ft2bt-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/PKG-INFO` & `ft2bt-0.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft2bt
-Version: 0.3.1
+Version: 0.3.2
 Summary: Automatic conversion from fault trees into behavior trees
 Home-page: https://github.com/cconejob/ft2bt_converter.git
 Author: Carlos Conejo
 Author-email: carlos.conejo@upc.edu
 License: GNU GPLv3
 Description: # Fault Tree to Behavior Tree Converter
         
@@ -33,15 +33,15 @@
             * **Events**: Depict events using circles. These are also required elements.
             * **AND/OR Gates**: Use the respective symbols for AND/OR gates in your diagram. These are required for depicting logical relationships in the fault tree.
             * **Probabilities**: Use text below the events to indicate the correspondent probability. Example: `p = 0.1`. These elements are not required.
         3. **Exporting the Diagram as XML**:
             * Once your fault tree diagram is ready, you need to export it in XML format. In draw.io, go to `File` > `Export as` > `XML` to save your diagram as an XML file.
         
         <p align="center">
-          <img src="ft2bt/test/fault_trees/fta_example.png" alt="Fault Tree Example">
+          <img src="https://github.com/cconejob/ft2bt_converter/blob/84847e3316d3363eb4e276729f382b198912925f/ft2bt/test/fault_trees/fta_example.png" alt="Fault Tree Example">
         </p>
         
         **Warning!**: All fault tree elements, with the exception of text probabilities, should be connected by directional arrows. Ensure that each arrow is physically attached to its corresponding elements to maintain clarity and accuracy in the diagram.
         
         ### Preparing Your Hazard Analysis and Risk Assessment (Opitonal)
         
         Create a *.csv file with some required column names:
@@ -49,15 +49,15 @@
         1. **Item_ID**: Identificator of the Item analyzed.
         2. **Hazard_ID**:  Identificator of the possible Hazard. The ID must match with the name of the correspondent Hazard in the Fault Tree.
         3. **Operating_Scenario_ID**: Identificator of the Operating Scenario.
         4. **ASIL**: Automotive Safety Integrity Level. Options: A, B, C, D
         5. **Safety_State_ID**: Identificator of the Safety State action.
         
         <p align="center">
-          <img src="ft2bt/test/hara/hara_example.png" alt="HARA Example">
+          <img src="https://github.com/cconejob/ft2bt_converter/blob/84847e3316d3363eb4e276729f382b198912925f/ft2bt/test/hara/hara_example.png" alt="HARA Example">
         </p>
         
         ### Running the Conversion Tool
         
         Run the conversion command:
         
         ```bash
@@ -78,15 +78,15 @@
         ### Output Example: Behavior Tree Diagram
         
         Below is an example of the behavior tree diagrams generated from the fault tree. The XML file is loaded using [Groot](https://github.com/BehaviorTree/Groot):
         
         The order of the events is randomly selected in this version of the software. Future versions will sort the events by probability of occurrence.
         
         <p align="center">
-          <img src="ft2bt/test/behavior_trees/render/BT_hz_01.svg" alt="Behavior Tree Conversion Example" height="400"> <!-- or you can set the height instead -->
+          <img src="https://github.com/cconejob/ft2bt_converter/blob/84847e3316d3363eb4e276729f382b198912925f/ft2bt/test/behavior_trees/render/BT_hz_01.svg" alt="Behavior Tree Conversion Example" height="400"> <!-- or you can set the height instead -->
         </p>
         
         ## Contact Information and Acknowledgement
         
         For further information regarding this project, please feel free to reach out to Carlos Conejo.
         
         This project was developed at the [Institut de Robòtica i Informàtica Industrial (IRI)](https://www.iri.upc.edu/), a joint university research center of the Polytechnic University of Catalonia (UPC) and the Spanish National Research Council (CSIC).
```

### Comparing `ft2bt-0.3.1/README.md` & `ft2bt-0.3.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     * **Events**: Depict events using circles. These are also required elements.
     * **AND/OR Gates**: Use the respective symbols for AND/OR gates in your diagram. These are required for depicting logical relationships in the fault tree.
     * **Probabilities**: Use text below the events to indicate the correspondent probability. Example: `p = 0.1`. These elements are not required.
 3. **Exporting the Diagram as XML**:
     * Once your fault tree diagram is ready, you need to export it in XML format. In draw.io, go to `File` > `Export as` > `XML` to save your diagram as an XML file.
 
 <p align="center">
-  <img src="ft2bt/test/fault_trees/fta_example.png" alt="Fault Tree Example">
+  <img src="https://github.com/cconejob/ft2bt_converter/blob/84847e3316d3363eb4e276729f382b198912925f/ft2bt/test/fault_trees/fta_example.png" alt="Fault Tree Example">
 </p>
 
 **Warning!**: All fault tree elements, with the exception of text probabilities, should be connected by directional arrows. Ensure that each arrow is physically attached to its corresponding elements to maintain clarity and accuracy in the diagram.
 
 ### Preparing Your Hazard Analysis and Risk Assessment (Opitonal)
 
 Create a *.csv file with some required column names:
@@ -41,15 +41,15 @@
 1. **Item_ID**: Identificator of the Item analyzed.
 2. **Hazard_ID**:  Identificator of the possible Hazard. The ID must match with the name of the correspondent Hazard in the Fault Tree.
 3. **Operating_Scenario_ID**: Identificator of the Operating Scenario.
 4. **ASIL**: Automotive Safety Integrity Level. Options: A, B, C, D
 5. **Safety_State_ID**: Identificator of the Safety State action.
 
 <p align="center">
-  <img src="ft2bt/test/hara/hara_example.png" alt="HARA Example">
+  <img src="https://github.com/cconejob/ft2bt_converter/blob/84847e3316d3363eb4e276729f382b198912925f/ft2bt/test/hara/hara_example.png" alt="HARA Example">
 </p>
 
 ### Running the Conversion Tool
 
 Run the conversion command:
 
 ```bash
@@ -70,15 +70,15 @@
 ### Output Example: Behavior Tree Diagram
 
 Below is an example of the behavior tree diagrams generated from the fault tree. The XML file is loaded using [Groot](https://github.com/BehaviorTree/Groot):
 
 The order of the events is randomly selected in this version of the software. Future versions will sort the events by probability of occurrence.
 
 <p align="center">
-  <img src="ft2bt/test/behavior_trees/render/BT_hz_01.svg" alt="Behavior Tree Conversion Example" height="400"> <!-- or you can set the height instead -->
+  <img src="https://github.com/cconejob/ft2bt_converter/blob/84847e3316d3363eb4e276729f382b198912925f/ft2bt/test/behavior_trees/render/BT_hz_01.svg" alt="Behavior Tree Conversion Example" height="400"> <!-- or you can set the height instead -->
 </p>
 
 ## Contact Information and Acknowledgement
 
 For further information regarding this project, please feel free to reach out to Carlos Conejo.
 
 This project was developed at the [Institut de Robòtica i Informàtica Industrial (IRI)](https://www.iri.upc.edu/), a joint university research center of the Polytechnic University of Catalonia (UPC) and the Spanish National Research Council (CSIC).
```

### Comparing `ft2bt-0.3.1/ft2bt/scripts/behavior_trees/behavior_tree.py` & `ft2bt-0.3.2/ft2bt/scripts/behavior_trees/behavior_tree.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/ft2bt/scripts/code_generator/code_generator.py` & `ft2bt-0.3.2/ft2bt/scripts/code_generator/code_generator.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/ft2bt/scripts/code_generator/header_file.py` & `ft2bt-0.3.2/ft2bt/scripts/code_generator/header_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/ft2bt/scripts/code_generator/main_file.py` & `ft2bt-0.3.2/ft2bt/scripts/code_generator/main_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/ft2bt/scripts/code_generator/source_file.py` & `ft2bt-0.3.2/ft2bt/scripts/code_generator/source_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/ft2bt/scripts/fault_trees/xml_fta_parser.py` & `ft2bt-0.3.2/ft2bt/scripts/fault_trees/xml_fta_parser.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/ft2bt/scripts/ft2bt.py` & `ft2bt-0.3.2/ft2bt/scripts/ft2bt.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/ft2bt/scripts/hara/hara_parser.py` & `ft2bt-0.3.2/ft2bt/scripts/hara/hara_parser.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/ft2bt/test/behavior_trees/render/BT_hz_01.svg` & `ft2bt-0.3.2/ft2bt/test/behavior_trees/render/BT_hz_01.svg`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/ft2bt/test/fault_trees/fta_example.png` & `ft2bt-0.3.2/ft2bt/test/fault_trees/fta_example.png`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/ft2bt/test/fault_trees/fta_example.xml` & `ft2bt-0.3.2/ft2bt/test/fault_trees/fta_example.xml`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/ft2bt/test/hara/hara_example.png` & `ft2bt-0.3.2/ft2bt/test/hara/hara_example.png`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/ft2bt.egg-info/PKG-INFO` & `ft2bt-0.3.2/ft2bt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft2bt
-Version: 0.3.1
+Version: 0.3.2
 Summary: Automatic conversion from fault trees into behavior trees
 Home-page: https://github.com/cconejob/ft2bt_converter.git
 Author: Carlos Conejo
 Author-email: carlos.conejo@upc.edu
 License: GNU GPLv3
 Description: # Fault Tree to Behavior Tree Converter
         
@@ -33,15 +33,15 @@
             * **Events**: Depict events using circles. These are also required elements.
             * **AND/OR Gates**: Use the respective symbols for AND/OR gates in your diagram. These are required for depicting logical relationships in the fault tree.
             * **Probabilities**: Use text below the events to indicate the correspondent probability. Example: `p = 0.1`. These elements are not required.
         3. **Exporting the Diagram as XML**:
             * Once your fault tree diagram is ready, you need to export it in XML format. In draw.io, go to `File` > `Export as` > `XML` to save your diagram as an XML file.
         
         <p align="center">
-          <img src="ft2bt/test/fault_trees/fta_example.png" alt="Fault Tree Example">
+          <img src="https://github.com/cconejob/ft2bt_converter/blob/84847e3316d3363eb4e276729f382b198912925f/ft2bt/test/fault_trees/fta_example.png" alt="Fault Tree Example">
         </p>
         
         **Warning!**: All fault tree elements, with the exception of text probabilities, should be connected by directional arrows. Ensure that each arrow is physically attached to its corresponding elements to maintain clarity and accuracy in the diagram.
         
         ### Preparing Your Hazard Analysis and Risk Assessment (Opitonal)
         
         Create a *.csv file with some required column names:
@@ -49,15 +49,15 @@
         1. **Item_ID**: Identificator of the Item analyzed.
         2. **Hazard_ID**:  Identificator of the possible Hazard. The ID must match with the name of the correspondent Hazard in the Fault Tree.
         3. **Operating_Scenario_ID**: Identificator of the Operating Scenario.
         4. **ASIL**: Automotive Safety Integrity Level. Options: A, B, C, D
         5. **Safety_State_ID**: Identificator of the Safety State action.
         
         <p align="center">
-          <img src="ft2bt/test/hara/hara_example.png" alt="HARA Example">
+          <img src="https://github.com/cconejob/ft2bt_converter/blob/84847e3316d3363eb4e276729f382b198912925f/ft2bt/test/hara/hara_example.png" alt="HARA Example">
         </p>
         
         ### Running the Conversion Tool
         
         Run the conversion command:
         
         ```bash
@@ -78,15 +78,15 @@
         ### Output Example: Behavior Tree Diagram
         
         Below is an example of the behavior tree diagrams generated from the fault tree. The XML file is loaded using [Groot](https://github.com/BehaviorTree/Groot):
         
         The order of the events is randomly selected in this version of the software. Future versions will sort the events by probability of occurrence.
         
         <p align="center">
-          <img src="ft2bt/test/behavior_trees/render/BT_hz_01.svg" alt="Behavior Tree Conversion Example" height="400"> <!-- or you can set the height instead -->
+          <img src="https://github.com/cconejob/ft2bt_converter/blob/84847e3316d3363eb4e276729f382b198912925f/ft2bt/test/behavior_trees/render/BT_hz_01.svg" alt="Behavior Tree Conversion Example" height="400"> <!-- or you can set the height instead -->
         </p>
         
         ## Contact Information and Acknowledgement
         
         For further information regarding this project, please feel free to reach out to Carlos Conejo.
         
         This project was developed at the [Institut de Robòtica i Informàtica Industrial (IRI)](https://www.iri.upc.edu/), a joint university research center of the Polytechnic University of Catalonia (UPC) and the Spanish National Research Council (CSIC).
```

### Comparing `ft2bt-0.3.1/ft2bt.egg-info/SOURCES.txt` & `ft2bt-0.3.2/ft2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ft2bt-0.3.1/setup.py` & `ft2bt-0.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements.txt file
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='ft2bt',
-    version='0.3.1',
+    version='0.3.2',
     packages=find_packages(),
     install_requires=required,  # Use the list from requirements.txt
     entry_points={
         'console_scripts': [
             'ft2bt=ft2bt.scripts.ft2bt:main',
         ],
     },
```

