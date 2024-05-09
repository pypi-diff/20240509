# Comparing `tmp/FlowVisor-0.1.3.tar.gz` & `tmp/FlowVisor-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.1.3.tar", last modified: Wed May  8 14:41:18 2024, max compression
+gzip compressed data, was "FlowVisor-0.1.4.tar", last modified: Thu May  9 19:18:06 2024, max compression
```

## Comparing `FlowVisor-0.1.3.tar` & `FlowVisor-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-08 14:41:18.814334 FlowVisor-0.1.3/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-08 14:41:18.810334 FlowVisor-0.1.3/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-08 14:41:18.000000 FlowVisor-0.1.3/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      497 2024-05-08 14:41:18.000000 FlowVisor-0.1.3/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-08 14:41:18.000000 FlowVisor-0.1.3/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-08 14:41:18.000000 FlowVisor-0.1.3/FlowVisor.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       52 2024-05-08 14:41:18.000000 FlowVisor-0.1.3/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-08 14:41:18.000000 FlowVisor-0.1.3/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.3/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-08 14:41:18.814334 FlowVisor-0.1.3/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.3/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-08 14:41:18.810334 FlowVisor-0.1.3/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)      180 2024-04-25 12:58:27.000000 FlowVisor-0.1.3/flowvisor/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-08 14:41:18.814334 FlowVisor-0.1.3/flowvisor/cli/
--rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.3/flowvisor/cli/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.3/flowvisor/cli/add_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.3/flowvisor/cli/remove_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.3/flowvisor/cli/vis_file.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    13238 2024-05-08 14:40:46.000000 FlowVisor-0.1.3/flowvisor/flowvisor.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     1571 2024-05-08 14:12:25.000000 FlowVisor-0.1.3/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8294 2024-05-08 14:29:44.000000 FlowVisor-0.1.3/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.3/flowvisor/time_tracker.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.3/flowvisor/timer.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2088 2024-04-25 12:36:32.000000 FlowVisor-0.1.3/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-08 14:41:18.814334 FlowVisor-0.1.3/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.3/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-09 19:18:06.511158 FlowVisor-0.1.4/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-09 19:18:06.507158 FlowVisor-0.1.4/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-09 19:18:06.000000 FlowVisor-0.1.4/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-09 19:18:06.000000 FlowVisor-0.1.4/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-09 19:18:06.000000 FlowVisor-0.1.4/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-09 19:18:06.000000 FlowVisor-0.1.4/FlowVisor.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       52 2024-05-09 19:18:06.000000 FlowVisor-0.1.4/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-09 19:18:06.000000 FlowVisor-0.1.4/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.4/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-09 19:18:06.511158 FlowVisor-0.1.4/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.4/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-09 19:18:06.511158 FlowVisor-0.1.4/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.1.4/flowvisor/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-09 19:18:06.511158 FlowVisor-0.1.4/flowvisor/cli/
+-rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.4/flowvisor/cli/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.4/flowvisor/cli/add_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.4/flowvisor/cli/remove_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.4/flowvisor/cli/vis_file.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)    15931 2024-05-09 09:31:09.000000 FlowVisor-0.1.4/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1751 2024-05-09 19:13:08.000000 FlowVisor-0.1.4/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     6185 2024-05-09 19:17:48.000000 FlowVisor-0.1.4/flowvisor/flowvisor_verifier.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8004 2024-05-09 07:05:50.000000 FlowVisor-0.1.4/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       98 2024-05-09 06:06:21.000000 FlowVisor-0.1.4/flowvisor/logger.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.1.4/flowvisor/sankey.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.4/flowvisor/time_tracker.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      292 2024-05-08 15:25:05.000000 FlowVisor-0.1.4/flowvisor/time_value.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.4/flowvisor/timer.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.1.4/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-09 19:18:06.511158 FlowVisor-0.1.4/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.4/setup.py
```

### Comparing `FlowVisor-0.1.3/FlowVisor.egg-info/PKG-INFO` & `FlowVisor-0.1.4/FlowVisor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.3
+Version: 0.1.4
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.1.3/LICENSE` & `FlowVisor-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.3/PKG-INFO` & `FlowVisor-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.3
+Version: 0.1.4
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.1.3/README.md` & `FlowVisor-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.3/flowvisor/cli/add_vis.py` & `FlowVisor-0.1.4/flowvisor/cli/add_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.3/flowvisor/cli/remove_vis.py` & `FlowVisor-0.1.4/flowvisor/cli/remove_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.3/flowvisor/cli/vis_file.py` & `FlowVisor-0.1.4/flowvisor/cli/vis_file.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.3/flowvisor/flowvisor.py` & `FlowVisor-0.1.4/flowvisor/flowvisor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 """
 The FlowVisor is a package that visualizes the flow of functions in a codebase.
 """
+
 import datetime
 import json
 import timeit
 from typing import List
-#from inspect import getmembers, isfunction, ismodule
 import pickle
 from diagrams import Diagram, Cluster
 from diagrams.custom import Custom
-from flowvisor import utils
+from flowvisor import logger, utils
 from flowvisor.flowvisor_config import FlowVisorConfig
+from flowvisor.flowvisor_verifier import FlowVisorVerifier, vis_verifier
 from flowvisor.function_node import FunctionNode
+from flowvisor.sankey import make_sankey_diagram
 from flowvisor.time_tracker import TimeTracker
+from flowvisor.time_value import TimeValue
 from flowvisor.utils import function_to_id
 
+
 def vis(func):
     """
+    The vis decorator
+    """
+
+    def wrapper(*args, **kwargs):
+        return FlowVisor.VIS_FUNCTION(func)(*args, **kwargs)
+
+    return wrapper
+
+
+def vis_impl(func):
+    """
     Decorator that visualizes the function.
     """
+
     def wrapper(*args, **kwargs):
         TimeTracker.stop()
 
         reduce_overhead = FlowVisor.CONFIG.reduce_overhead
         if reduce_overhead:
             TimeTracker.apply(advanced=FlowVisor.get_advanced_overhead_reduction())
             timer_id = TimeTracker.register_new_timer()
@@ -38,28 +54,33 @@
             TimeTracker.apply(advanced=FlowVisor.get_advanced_overhead_reduction())
             duration = TimeTracker.get_time_and_remove_timer(timer_id)
 
         FlowVisor.function_returned(func, duration)
 
         TimeTracker.start(reduce_overhead)
         return result
+
     return wrapper
 
+
 class FlowVisor:
     """
-    The FlowVisor class is responsible for managing the flow of the functions 
+    The FlowVisor class is responsible for managing the flow of the functions
     and generating the graph.
     """
 
+    VIS_FUNCTION = vis_impl
+
     NODES: List[FunctionNode] = []
     ROOTS: List[FunctionNode] = []
     STACK: List[FunctionNode] = []
     CONFIG = FlowVisorConfig()
 
     EXCLUDE_FUNCTIONS = []
+    VERIFIER_MODE = False
 
     @staticmethod
     def add_function_node(func):
         """
         Adds a function node to the list of nodes if it does not exist.
         """
         func_id = function_to_id(func)
@@ -107,46 +128,62 @@
             return
 
         if FlowVisor.is_function_excluded(func):
             return
 
         node = FlowVisor.STACK.pop()
 
-        if len(FlowVisor.STACK) > 0 and FlowVisor.CONFIG.exclusive_time_mode:
+        if len(FlowVisor.STACK) > 0:
             parent = FlowVisor.STACK[-1]
-            parent.time -= duration
+            parent.child_time += duration
 
         node.got_called(duration)
 
     @staticmethod
     def get_called_nodes_only():
         """
         Returns only the nodes that have been called.
         """
         return [node for node in FlowVisor.NODES if node.called > 0]
 
     @staticmethod
-    def graph():
+    def graph(verify=False, verify_file_name="flowvisor_verifier.json"):
         """
         Generates the graph.
         """
+        if FlowVisor.VERIFIER_MODE:
+            logger.log("Can not generate graph in verifier mode!")
+            return
+
+        verify_text = None
+        if verify:
+            if FlowVisor.verify(verify_file_name):
+                verify_text = "Verified ✅"
+            else:
+                verify_text = "Not Verified ❌"
+
         try:
-            with Diagram(FlowVisor.CONFIG.graph_title,
-                         show=FlowVisor.CONFIG.show_graph,
-                         filename=FlowVisor.CONFIG.output_file,
-                         direction="LR"):
+            with Diagram(
+                FlowVisor.CONFIG.graph_title,
+                show=FlowVisor.CONFIG.show_graph,
+                filename=FlowVisor.CONFIG.output_file,
+                direction="LR",
+            ):
 
                 blank_image = FunctionNode.make_node_image_cache()
 
-                FlowVisor.draw_meta_data(blank_image)
+                FlowVisor.draw_meta_data(blank_image, verify_text)
 
                 if FlowVisor.CONFIG.logo != "":
-                    Custom("", FlowVisor.CONFIG.logo,
-                           width=FlowVisor.CONFIG.get_node_scale(),
-                           height=FlowVisor.CONFIG.get_node_scale())
+                    Custom(
+                        "",
+                        FlowVisor.CONFIG.logo,
+                        width=FlowVisor.CONFIG.get_node_scale(),
+                        height=FlowVisor.CONFIG.get_node_scale(),
+                    )
 
                 called_nodes = FlowVisor.get_called_nodes_only()
 
                 # Draw nodes
                 if FlowVisor.CONFIG.group_nodes:
                     FlowVisor.draw_nodes_with_cluster(called_nodes)
                 else:
@@ -154,45 +191,66 @@
                         FlowVisor.draw_function_node(n)
 
         finally:
             # Make sure to clear the cache always
             FunctionNode.clear_node_image_cache()
 
     @staticmethod
+    def sankey_diagram():
+        """
+        Generates the sankey diagram.
+        """
+        make_sankey_diagram(FlowVisor.ROOTS, FlowVisor.NODES)
+
+    @staticmethod
     def get_highest_time():
         """
         Returns the highest time.
         """
         highest_time = -1
         for node in FlowVisor.NODES:
-            if node.time > highest_time:
-                highest_time = node.time
+            node_time = node.get_time(FlowVisor.CONFIG.exclusive_time_mode)
+            if node_time > highest_time:
+                highest_time = node_time
         return highest_time
 
     @staticmethod
     def get_total_time():
         """
         Returns the total time.
         """
         total_time = 0
         nodes = FlowVisor.NODES
         if not FlowVisor.CONFIG.exclusive_time_mode:
             nodes = FlowVisor.ROOTS
 
         for node in nodes:
-            total_time += node.time
+            total_time += node.get_time(FlowVisor.CONFIG.exclusive_time_mode)
 
         return total_time
 
     @staticmethod
-    def draw_meta_data(blank_image):
+    def get_mean_time():
+        """
+        Returns the mean time.
+        """
+        sum_time = 0
+        for node in FlowVisor.NODES:
+            sum_time += node.get_time(FlowVisor.CONFIG.exclusive_time_mode)
+
+        return sum_time / len(FlowVisor.NODES)
+
+    @staticmethod
+    def draw_meta_data(blank_image, verify_text):
         """
         Draws some metadata on the graph.
         """
         with Cluster("Metadata", graph_attr={"bgcolor": "#FFFFFF"}):
+            if verify_text is not None:
+                Custom(verify_text, blank_image, width="2", height="0.1")
             if FlowVisor.CONFIG.show_system_info:
                 sys_info = utils.get_sys_info()
                 text = ""
                 for key, value in sys_info.items():
                     text += f"{key}: {value}\n"
                 Custom(text, blank_image, width="6", height="1")
             if FlowVisor.CONFIG.show_timestamp:
@@ -204,25 +262,37 @@
 
     @staticmethod
     def draw_nodes_with_cluster(nodes: List[FunctionNode]):
         """
         Draws the nodes with cluster.
         """
         sorted_nodes = FlowVisor.get_node_sorted_by_filename(nodes)
-        total_times = [sum([n.get_time_without_children() for n in row]) for row in sorted_nodes]
+        total_times = [
+            sum([n.get_time_without_children() for n in row]) for row in sorted_nodes
+        ]
         highest_time_file_time = max(total_times)
         for index, row in enumerate(sorted_nodes):
-            cluster_title = f"{row[0].file_name} ({utils.get_time_as_string(total_times[index])})"
-            bg_color = utils.value_to_hex_color(total_times[index], highest_time_file_time,
-                                                light_color=[0xFF, 0xFF, 0xFF],
-                                                dark_color=[0xAA, 0xAA, 0xAA])
-            font_color = utils.value_to_hex_color(total_times[index], highest_time_file_time,
-                                                light_color=[0x00, 0x00, 0x00],
-                                                dark_color=[0xFF, 0xFF, 0xFF])
-            with Cluster(cluster_title, graph_attr={"bgcolor": bg_color, "fontcolor": font_color}):
+            cluster_title = (
+                f"{row[0].file_name} ({utils.get_time_as_string(total_times[index])})"
+            )
+            bg_color = utils.value_to_hex_color(
+                total_times[index],
+                highest_time_file_time,
+                light_color=[0xFF, 0xFF, 0xFF],
+                dark_color=[0xAA, 0xAA, 0xAA],
+            )
+            font_color = utils.value_to_hex_color(
+                total_times[index],
+                highest_time_file_time,
+                light_color=[0x00, 0x00, 0x00],
+                dark_color=[0xFF, 0xFF, 0xFF],
+            )
+            with Cluster(
+                cluster_title, graph_attr={"bgcolor": bg_color, "fontcolor": font_color}
+            ):
                 for n in row:
                     FlowVisor.draw_function_node(n)
 
     @staticmethod
     def get_node_sorted_by_filename(nodes: List[FunctionNode]):
         """
         Returns the nodes sorted by filename.
@@ -245,18 +315,22 @@
     def get_nodes_as_dict():
         """
         Returns the nodes as a dictionary.
         """
         return [node.to_dict() for node in FlowVisor.NODES]
 
     @staticmethod
-    def export(file: str, export_type = "pickle"):
+    def export(file: str, export_type="pickle"):
         """
         Saves the flow to a file.
         """
+        if FlowVisor.VERIFIER_MODE:
+            logger.log("Can not export in verifier mode!")
+            return
+
         nodes_dict = FlowVisor.get_nodes_as_dict()
         if export_type == "json":
             if not file.endswith(".json"):
                 file += ".json"
             with open(file, "w", encoding="utf-8") as f:
                 json.dump(nodes_dict, f, indent=4)
         if export_type == "pickle":
@@ -289,20 +363,22 @@
         FlowVisor.graph()
 
     @staticmethod
     def draw_function_node(func_node: FunctionNode):
         """
         Draws the function node.
         """
-        highest_time = FlowVisor.get_highest_time()
-        total_time = FlowVisor.get_total_time()
-        
-        node = func_node.get_as_diagram_node(highest_time,total_time, FlowVisor.CONFIG)
+        time_value = TimeValue()
+        time_value.max_time = FlowVisor.get_highest_time()
+        time_value.total_time = FlowVisor.get_total_time()
+        time_value.mean_time = FlowVisor.get_mean_time()
+
+        node = func_node.get_as_diagram_node(time_value, FlowVisor.CONFIG)
         for child in func_node.children:
-            _ = node >> child.get_as_diagram_node(highest_time, total_time, FlowVisor.CONFIG)
+            _ = node >> child.get_as_diagram_node(time_value, FlowVisor.CONFIG)
 
     @staticmethod
     def is_function_excluded(func):
         """
         Checks if a function is excluded.
         """
         func_id = function_to_id(func)
@@ -337,15 +413,15 @@
     def enable_advanced_overhead_reduction():
         """
         Enables advanced overhead reduction.
         """
         n = 50000
         t = timeit.timeit(setup="import time", stmt="time.time()", number=n)
         mean = t / n
-        print(f"Mean time for time.time() is: {utils.get_time_as_string(mean)}")
+        logger.log(f"Mean time for time.time() is: {utils.get_time_as_string(mean)}")
         FlowVisor.CONFIG.advanced_overhead_reduction = mean
 
     @staticmethod
     def disable_advanced_overhead_reduction():
         """
         Disables advanced overhead reduction.
         """
@@ -368,14 +444,45 @@
     @staticmethod
     def set_config(config: FlowVisorConfig):
         """
         Sets the configuration.
         """
         FlowVisor.CONFIG = config
 
+    @staticmethod
+    def enable_verifier_mode():
+        """
+        Enables the verifier mode.
+        """
+        FlowVisor.VERIFIER_MODE = True
+        FlowVisor.VIS_FUNCTION = vis_verifier
+        logger.log("*** Running FlowVisor in verify mode ***")
+
+    @staticmethod
+    def verify_export(file_name="flowvisor_verifier.json"):
+        """
+        Exports the verifier.
+        """
+        if not FlowVisor.VERIFIER_MODE:
+            logger.log("Can not export verify in non-verifier mode!")
+            return
+        FlowVisorVerifier.export(file_name)
+
+    @staticmethod
+    def verify(verify_file_name="flowvisor_verifier.json"):
+        """
+        Checks the result against the verifier.
+        """
+        if FlowVisor.VERIFIER_MODE:
+            logger.log("Can not verify in verifier mode!")
+            return False
+        return FlowVisorVerifier.verify(
+            FlowVisor.NODES, verify_file_name, FlowVisor.CONFIG.verify_threshold
+        )
+
     '''
     @staticmethod
     def visualize_all():
         """
         Visualizes all the functions in this project.
         """
         FlowVisor.visualize_module_by_name("__main__")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `FlowVisor-0.1.3/flowvisor/flowvisor_config.py` & `FlowVisor-0.1.4/flowvisor/flowvisor_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Configuration class for FlowVisor
 """
+
 from flowvisor import utils
 
 
 class FlowVisorConfig:
     """
     Configuration class for FlowVisor
     """
@@ -20,31 +21,39 @@
         self.show_function_time_percantage: bool = False
         self.show_node_avg_time: bool = True
         self.static_font_color: str = ""
         self.show_timestamp: bool = False
         self.show_system_info: bool = False
         self.show_flowvisor_settings: bool = False
         self.group_nodes: bool = False
+        self.outline_threshold: float = 0.1
 
         # File settings
         self.output_file: str = "function_flow"
 
         # Functional settings
         self.reduce_overhead: bool = True
-        self.exclusive_time_mode: bool = False
+        self.exclusive_time_mode: bool = True
         self.advanced_overhead_reduction = None
 
+        # Verifier settings
+        self.verify_threshold: float = 0.2
+
         # Other
         self.dev_mode: bool = False
 
     def get_node_scale(self):
         """
         Get the node scale as a string
         """
         return str(self.node_scale)
 
     def get_functional_settings_string(self):
         s = "Reduce Overhead: " + str(self.reduce_overhead) + "\n"
         if self.reduce_overhead and self.advanced_overhead_reduction is not None:
-            s += "Advanced Overhead reduction: " + utils.get_time_as_string(self.advanced_overhead_reduction) + "\n"
+            s += (
+                "Advanced Overhead reduction: "
+                + utils.get_time_as_string(self.advanced_overhead_reduction)
+                + "\n"
+            )
         s += "Exclusive Time Mode: " + str(self.exclusive_time_mode) + "\n"
         return s
```

### Comparing `FlowVisor-0.1.3/flowvisor/function_node.py` & `FlowVisor-0.1.4/flowvisor/function_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 A node in the function call graph.
 """
+
 import os
 from typing import List
 import uuid
 from PIL import Image, ImageDraw
 from diagrams.custom import Custom
 
 from flowvisor import utils
 from flowvisor.flowvisor_config import FlowVisorConfig
+from flowvisor.time_value import TimeValue
 
 
 class FunctionNode:
     """
     A node in the function call graph
     """
 
@@ -24,118 +26,118 @@
             self.id: str = utils.function_to_id(func)
             self.uuid = str(uuid.uuid4())
             self.name: str = func.__name__
             self.file_path: str = func.__code__.co_filename
             self.file_name: str = os.path.basename(self.file_path)
         self.children: List[FunctionNode] = []
         self.children_ids: List[str] = []
-        self.time: float = 0
+        self.__time: float = 0
         self.diagram_node = None
         self.called: int = 0
+        self.child_time: float = 0
 
-    def export_node_image(self, highest_time):
+    def export_node_image(self, time_value: TimeValue, config: FlowVisorConfig):
         """
         Generates the node image background.
         """
         dim = FunctionNode.NODE_IMAGE_SCALE
-        image = Image.new('RGB', (dim, dim), 'white')
+        image = Image.new("RGB", (dim, dim), "white")
         draw = ImageDraw.Draw(image)
 
-        color = utils.value_to_hex_color(self.time, highest_time)
+        t = self.get_time(config.exclusive_time_mode)
+
+        color = utils.value_to_hex_color_using_mean(t, time_value.mean_time)
 
-        if self.time >= highest_time * 0.9:
+        if t >= time_value.max_time * (1 - config.outline_threshold):
             # draw outline
             draw.rectangle((0, 0, dim, dim), fill="#ff0000")
             ## draw inner
             draw.rectangle((10, 10, dim - 10, dim - 10), fill=color)
         else:
             draw.rectangle((0, 0, dim, dim), fill=color)
 
         os.makedirs(FunctionNode.NODE_IMAGE_CACHE, exist_ok=True)
         file_name = f"{FunctionNode.NODE_IMAGE_CACHE}/{self.uuid}.png"
         image.save(file_name)
 
         return file_name
 
-    def get_as_diagram_node(self,highest_time: float, total_time: float, config: FlowVisorConfig):
+    def get_as_diagram_node(self, time_value: TimeValue, config: FlowVisorConfig):
         """
         Gets the node as a diagram node.
         """
         if self.diagram_node is None:
-            self.generate_diagram_node(highest_time, total_time, config)
+            self.generate_diagram_node(time_value, config)
         return self.diagram_node
 
-    def generate_diagram_node(self, highest_time: float, total_time: float, config: FlowVisorConfig):
+    def generate_diagram_node(self, time_value: TimeValue, config: FlowVisorConfig):
         """
         Generates the diagram node.
         """
-        node_image = self.export_node_image(highest_time)
-
-        size = self.time / highest_time
-        if size < 0.1:
-            size = 0.1
+        node_image = self.export_node_image(time_value, config)
 
-        size = 1
-        size = size * config.node_scale
+        size = config.node_scale
 
-        title = self.get_node_title(total_time, config)
+        title = self.get_node_title(time_value, config)
 
         font_color = config.static_font_color
         if font_color == "":
-            font_color = utils.value_to_hex_color(self.time, highest_time,
-                                                  dark_color=[0xFF, 0xC0, 0x82],
-                                                  light_color=[0x00, 0x00, 0x00])
-
-        self.diagram_node = Custom(title, node_image,
-                                   width=str(size),
-                                   height=str(size),
-                                   fontcolor=font_color)
+            font_color = utils.value_to_hex_color_using_mean(
+                self.get_time(config.exclusive_time_mode),
+                time_value.mean_time,
+                dark_color=[0xFF, 0xC0, 0x82],
+                light_color=[0x00, 0x00, 0x00],
+            )
+
+        self.diagram_node = Custom(
+            title, node_image, width=str(size), height=str(size), fontcolor=font_color
+        )
 
-    def get_node_title(self, total_time: float, config: FlowVisorConfig):
+    def get_node_title(self, time_value: TimeValue, config: FlowVisorConfig):
         """
         Returns the title of the node, that is displayed in the diagram.
         """
         title = self.name + "\n"
 
         if config.show_node_file:
             title += self.file_name + "\n"
-
-        title += utils.get_time_as_string(self.time)
+        t = self.get_time(config.exclusive_time_mode)
+        title += utils.get_time_as_string(t)
 
         if config.show_node_call_count:
             title += f" ({self.called})"
 
         title += "\n"
 
         if config.show_node_avg_time:
-            title += f"avg {utils.get_time_as_string(self.time / self.called)}"
+            title += f"avg {utils.get_time_as_string(t / self.called)}"
 
         title += "\n"
 
         if config.show_function_time_percantage:
-            percentage = (self.time / total_time) * 100
+            percentage = (t / time_value.total_time) * 100
             title += f"{round(percentage, 2)}%"
 
         title += "\n"
 
-        for _ in range(int(config.node_scale) - 1 ):
+        for _ in range(int(config.node_scale) - 1):
             title += "\n\n"
         return title
 
-    def got_called(self,duration: float):
+    def got_called(self, duration: float):
         """
         The function got called.
-        
+
         Args:
             duration: The time it took to execute the function.
         """
         self.called += 1
         self.set_time(duration)
 
-    def add_child(self, child): # type: ignore
+    def add_child(self, child):  # type: ignore
         """
         Adds a child node to the current node.
 
         Args:
             child (FunctionNode): The child node to add.
         """
         if self.id == child.id:
@@ -148,49 +150,29 @@
     def set_time(self, time: float):
         """
         Sets the time of the function.
 
         Args:
             time (float): The time it took to execute the function.
         """
-        self.time += time
-
-    def to_json(self, inline = 0):
-        """
-        Returns the node as a json string.
-        
-        Args:
-            inline: The number of spaces to indent.
-        """
-        inline_str = "  " * inline
-        result = f'"{self.file_function_name()}({self.time})"'
-        if len(self.children) == 0:
-            return inline_str + result
-        result += ":["
-        for index,child in enumerate(self.children):
-            if index > 0:
-                result += ","
-            result += f"\n{child.to_json(inline + 1)}"
-        result += f"\n{inline_str}]"
-        result = inline_str + "{"+ result + "}"
-        return result
+        self.__time += time
 
     def file_function_name(self):
         """
         Returns the file name and function name.
         """
         return f"{self.file_name}::{self.name}"
 
     def __str__(self):
         return self.file_function_name()
 
-    def to_dict(self, short = False):
+    def to_dict(self, short=False):
         """
         Gets the node as a dictionary.
-        
+
         Args:
             short: If the dictionary should be short.
         """
 
         if short:
             return {
                 "id": self.id,
@@ -202,54 +184,66 @@
         return {
             "id": self.id,
             "uuid": self.uuid,
             "name": self.name,
             "file_path": self.file_path,
             "file_name": self.file_name,
             "children": [child.to_dict(True) for child in self.children],
-            "time": self.time,
-            "called": self.called
+            "exclusive_time": self.get_time(True),
+            "inclusive_time": self.get_time(False),
+            "called": self.called,
         }
 
     def resolve_children_ids(self, all_nodes):
         """
         Resolves the children ids.
-        
+
         Args:
             all_nodes: All nodes in the graph.
         """
         self.children = []
         for child_id in self.children_ids:
             for node in all_nodes:
                 if node.uuid == child_id:
                     self.add_child(node)
 
     def get_time_without_children(self):
         """
         Gets the time without the children.
         """
-        time = self.time
+        time = self.get_time()
         for child in self.children:
             time -= child.time
         return time
 
+    def get_time(self, exclusive=True):
+        """
+        Gets the time of the node.
+
+        Args:
+            exclusive: If the time should be exclusive.
+        """
+        if exclusive:
+            return self.__time - self.child_time
+        return self.__time
+
     @staticmethod
     def make_node_image_cache():
         """
         Makes the node image cache.
-        
+
         Returns:
             The file name of the blank image.
         """
         os.makedirs(FunctionNode.NODE_IMAGE_CACHE, exist_ok=True)
 
         FunctionNode.NODE_IMAGE_CACHE = os.path.abspath(FunctionNode.NODE_IMAGE_CACHE)
 
         dim = FunctionNode.NODE_IMAGE_SCALE
-        image = Image.new('RGB', (dim, dim), 'white')
+        image = Image.new("RGB", (dim, dim), "white")
 
         file_name = f"{FunctionNode.NODE_IMAGE_CACHE}/_blank.png"
         image.save(file_name)
         return file_name
 
     @staticmethod
     def clear_node_image_cache():
@@ -260,15 +254,15 @@
             os.remove(f"{FunctionNode.NODE_IMAGE_CACHE}/{file}")
         os.rmdir(FunctionNode.NODE_IMAGE_CACHE)
 
     @staticmethod
     def from_dict(d):
         """
         Creates a FunctionNode from a dictionary.
-        
+
         Args:
             dict: The dictionary to create the FunctionNode from.
         """
         node = FunctionNode(None)
         node.id = d["id"]
         node.uuid = d["uuid"]
         node.name = d["name"]
```

### Comparing `FlowVisor-0.1.3/flowvisor/time_tracker.py` & `FlowVisor-0.1.4/flowvisor/time_tracker.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.3/setup.py` & `FlowVisor-0.1.4/setup.py`

 * *Files identical despite different names*

