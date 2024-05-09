# Comparing `tmp/pywgraph-1.0.1.tar.gz` & `tmp/pywgraph-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywgraph-1.0.1.tar", last modified: Tue May  7 19:46:34 2024, max compression
+gzip compressed data, was "pywgraph-1.0.2.tar", last modified: Thu May  9 21:29:25 2024, max compression
```

## Comparing `pywgraph-1.0.1.tar` & `pywgraph-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:34.808596 pywgraph-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-07 19:46:34.804595 pywgraph-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-05-07 19:46:28.000000 pywgraph-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:34.804595 pywgraph-1.0.1/pywgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 19:46:28.000000 pywgraph-1.0.1/pywgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-07 19:46:28.000000 pywgraph-1.0.1/pywgraph/_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-07 19:46:28.000000 pywgraph-1.0.1/pywgraph/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-07 19:46:28.000000 pywgraph-1.0.1/pywgraph/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-07 19:46:28.000000 pywgraph-1.0.1/pywgraph/_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-07 19:46:28.000000 pywgraph-1.0.1/pywgraph/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:34.804595 pywgraph-1.0.1/pywgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-07 19:46:34.000000 pywgraph-1.0.1/pywgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-07 19:46:34.000000 pywgraph-1.0.1/pywgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:46:34.000000 pywgraph-1.0.1/pywgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 19:46:34.000000 pywgraph-1.0.1/pywgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 19:46:34.000000 pywgraph-1.0.1/pywgraph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:46:34.808596 pywgraph-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-07 19:46:28.000000 pywgraph-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:34.804595 pywgraph-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:28.000000 pywgraph-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-07 19:46:28.000000 pywgraph-1.0.1/tests/test_directed_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-07 19:46:28.000000 pywgraph-1.0.1/tests/test_path_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-07 19:46:28.000000 pywgraph-1.0.1/tests/test_weighted_directed_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-07 19:46:28.000000 pywgraph-1.0.1/tests/test_weighted_directed_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-07 19:46:28.000000 pywgraph-1.0.1/tests/test_weighted_directed_graph_arrays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.170613 pywgraph-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-09 21:29:25.170613 pywgraph-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-09 21:29:21.000000 pywgraph-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.166613 pywgraph-1.0.2/pywgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.170613 pywgraph-1.0.2/pywgraph/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/exceptions/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.170613 pywgraph-1.0.2/pywgraph/graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/graphs/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/graphs/_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.170613 pywgraph-1.0.2/pywgraph/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-09 21:29:21.000000 pywgraph-1.0.2/pywgraph/groups/_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.170613 pywgraph-1.0.2/pywgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-09 21:29:25.000000 pywgraph-1.0.2/pywgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-09 21:29:25.000000 pywgraph-1.0.2/pywgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:29:25.000000 pywgraph-1.0.2/pywgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 21:29:25.000000 pywgraph-1.0.2/pywgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 21:29:25.000000 pywgraph-1.0.2/pywgraph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 21:29:25.170613 pywgraph-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-09 21:29:21.000000 pywgraph-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:25.170613 pywgraph-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:21.000000 pywgraph-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-09 21:29:21.000000 pywgraph-1.0.2/tests/test_directed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-09 21:29:21.000000 pywgraph-1.0.2/tests/test_path_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-09 21:29:21.000000 pywgraph-1.0.2/tests/test_weighted_directed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-05-09 21:29:21.000000 pywgraph-1.0.2/tests/test_weighted_directed_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-09 21:29:21.000000 pywgraph-1.0.2/tests/test_weighted_directed_graph_arrays.py
```

### Comparing `pywgraph-1.0.1/PKG-INFO` & `pywgraph-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pywgraph
-Version: 1.0.1
-Summary: A python implementation of weighted directed graphs where weights can be elements of a mathematical group
+Version: 1.0.2
+Summary: A python implementation of weighted directed graphs
 Home-page: https://github.com/josek98/pywgraph
 Author: josek98
 Author-email: josemmsscc98@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Requires-Dist: pytest>=7.0; extra == "dev"
@@ -263,7 +263,12 @@
 
 ## Release Notes
 
 ### Version 1.0.1 (2024-05-07)
 
 - Added a method to `WeightedDirectedGraph` to add a new node. 
 - Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights. 
+
+### Version 1.0.2 (2024-05-09)
+
+- Added a method to `WeightedDirectedGraph` to remove a node. 
+- Added a method to `WeightedDirectedGraph` to remove an edge.
```

### Comparing `pywgraph-1.0.1/README.md` & `pywgraph-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -249,8 +249,13 @@
 Notice that this graph is not conmutative since the weight of the path `["A", "C"]` is different from the weight of the path `["A", "B", "C]`.
 
 ## Release Notes
 
 ### Version 1.0.1 (2024-05-07)
 
 - Added a method to `WeightedDirectedGraph` to add a new node. 
-- Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights. 
+- Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights. 
+
+### Version 1.0.2 (2024-05-09)
+
+- Added a method to `WeightedDirectedGraph` to remove a node. 
+- Added a method to `WeightedDirectedGraph` to remove an edge.
```

### Comparing `pywgraph-1.0.1/pywgraph/_edge.py` & `pywgraph-1.0.2/pywgraph/graphs/_edge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import TypeVar
-from ._groups import Group
+from ..groups import Group
 
 T = TypeVar("T")
 _default_group = Group(
     "Real numbers with multiplication", 1.0, lambda x, y: x * y, lambda x: 1 / x
 )
```

### Comparing `pywgraph-1.0.1/pywgraph/_exceptions.py` & `pywgraph-1.0.2/pywgraph/exceptions/_exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 class NodeNotFound(Exception):
     """Exception raised when a node is not found in a graph."""
 
     def __init__(self, nodes: str | set[str]) -> None:
-        self.nodes = nodes
         super().__init__(f"Nodes {nodes} not found in the graph.")
 
 class NodeAlreadyExists(Exception):
     """Exception raised when a node already exists in a graph."""
 
     def __init__(self, node: str) -> None:
-        self.node = node
         super().__init__(f"Node {node} already exists in the graph.")
 
 class EdgeAlreadyExists(Exception):
     """Exception raised when an edge already exists in a graph."""
 
     def __init__(self, start: str, end: str) -> None:
-        self.start = start
-        self.end = end
-        super().__init__(f"Edge {start} -> {end} already exists in the graph.")
+        super().__init__(f"Edge {start} -> {end} already exists in the graph.")
+
+class EdgeNotFound(Exception):
+    """Exception raised when an edge is not found in a graph."""
+    def __init__(self, start: str, end: str) -> None:
+        super().__init__(f"Edge {start} -> {end} not found in the graph.")
```

### Comparing `pywgraph-1.0.1/pywgraph/_graph.py` & `pywgraph-1.0.2/pywgraph/graphs/_graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import reduce  # type: ignore
-from ._groups import Group
+from ..groups import Group
 from ._edge import WeightedDirectedEdge  # type: ignore
-from ._exceptions import NodeNotFound, NodeAlreadyExists, EdgeAlreadyExists  # type: ignore
-from ._utils import _find_path
+from ..exceptions import NodeNotFound, NodeAlreadyExists, EdgeAlreadyExists, EdgeNotFound  # type: ignore
+from .._utils import _find_path
 
 _default_group = Group(
     "Real numbers under multiplication", 1.0, lambda x, y: x * y, lambda x: 1 / x
 )
 
 
 def _check_nodes_in_edges(
@@ -65,78 +65,116 @@
             return
 
         return_graph = WeightedDirectedGraph(
             nodes=self._nodes | {node}, edges=self._edges, group=self.group
         )
         return return_graph
 
+    def delete_node(self, node: str, inplace: bool = False):
+        """Deletes a node from the graph. Also removes all edges connected to this node."""
+        if node not in self._nodes:
+            raise NodeNotFound(node)
+
+        node_edges = {
+            edge for edge in self._edges if edge.start == node or edge.end == node
+        }
+        good_edges = self.edges - node_edges
+
+        if inplace:
+            self._nodes.remove(node)
+            self._edges = good_edges
+            return
+
+        return_graph = WeightedDirectedGraph(
+            nodes=self._nodes - {node}, edges=good_edges, group=self.group
+        )
+        return return_graph
+
     def add_edge(
         self,
         start: str,
         end: str,
         weight: "Group.element" = None,
         path: list[str] | None = None,
         allow_inverse: bool = True,
-        inplace: bool = False
+        inplace: bool = False,
     ):
         """Adds an edge connectingh two existing nodes.
-        
+
         Parameter
         --------
         start: str
-            The start node of the edge. Must be an existing node from the graph. 
+            The start node of the edge. Must be an existing node from the graph.
         end: str
-            The end node of the edge. Must be an existing node from the graph. 
+            The end node of the edge. Must be an existing node from the graph.
         weight: Optional[Group.element]
-            The weight of the edge. If no weight and not path is provided, the weight will be try 
-            to be calculated finding a path connecting the edges. 
+            The weight of the edge. If no weight and not path is provided, the weight will be try
+            to be calculated finding a path connecting the edges.
         path: Optional[list[str]]
-            If this is provided and no weight is given the weight will be calculated using this path. 
-            If this path is not possible and exception will be raised. It is possible to use 
-            a path that exists but does not connect start and end node, this might be removed 
+            If this is provided and no weight is given the weight will be calculated using this path.
+            If this path is not possible and exception will be raised. It is possible to use
+            a path that exists but does not connect start and end node, this might be removed
             in future versions.
         allow_inverse: bool
-            If True, allows the creation of the inverse edge to find a path between edges. 
+            If True, allows the creation of the inverse edge to find a path between edges.
         """
 
         bad_nodes = {start, end} - self._nodes
         if bad_nodes:
             raise NodeNotFound(bad_nodes)
         if (start, end) in {(edge.start, edge.end) for edge in self._edges}:
             raise EdgeAlreadyExists(start, end)
-        
-        if weight is None: # Find weight in another way
-            if allow_inverse: 
+
+        if weight is None:  # Find weight in another way
+            if allow_inverse:
                 search_graph = self.add_reverse_edges(inplace=False)
-            else: 
+            else:
                 search_graph = self
 
-            if path is not None: # Apply weight of the given path
+            if path is not None:  # Apply weight of the given path
                 weight = search_graph.path_weight(path)
-            else: # Find path to get a weight
+            else:  # Find path to get a weight
                 path = search_graph.find_path(start, end)
                 if not path:
                     print(f"Unable to find a weight to connect edge {start} -> {end}")
                     if inplace:
-                        return 
+                        return
                     return self
-                else: 
+                else:
                     weight = search_graph.path_weight(path)
 
         if inplace:
             self._edges.add(WeightedDirectedEdge(start, end, weight, self.group))
             return
 
         return_graph = WeightedDirectedGraph(
             nodes=self._nodes,
             edges=self._edges | {WeightedDirectedEdge(start, end, weight)},
             group=self.group,
         )
         return return_graph
 
+    def delete_edge(self, start: str, end: str, inplace: bool = False):
+        """Deletes an edge connecting two existing nodes."""
+
+        bad_nodes = {start, end} - self._nodes
+        if bad_nodes:
+            raise NodeNotFound(bad_nodes)
+
+        good_edges = {
+            edge for edge in self._edges if (edge.start, edge.end) != (start, end)
+        }
+        if good_edges == self._edges:
+            raise EdgeNotFound(start, end)
+        if inplace:
+            self._edges = good_edges
+            return
+
+        return WeightedDirectedGraph(self._nodes, good_edges, self.group)
+
     def add_reverse_edges(self, inplace: bool = False):
         """Adds the missing inverse direction edges"""
 
         all_inverse_edges = {edge.inverse for edge in self._edges}
         inverse_edges = {
             edge
             for edge in all_inverse_edges
```

### Comparing `pywgraph-1.0.1/pywgraph/_groups.py` & `pywgraph-1.0.2/pywgraph/groups/_groups.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.1/pywgraph/_utils.py` & `pywgraph-1.0.2/pywgraph/_utils.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.1/pywgraph.egg-info/PKG-INFO` & `pywgraph-1.0.2/pywgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pywgraph
-Version: 1.0.1
-Summary: A python implementation of weighted directed graphs where weights can be elements of a mathematical group
+Version: 1.0.2
+Summary: A python implementation of weighted directed graphs
 Home-page: https://github.com/josek98/pywgraph
 Author: josek98
 Author-email: josemmsscc98@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Requires-Dist: pytest>=7.0; extra == "dev"
@@ -263,7 +263,12 @@
 
 ## Release Notes
 
 ### Version 1.0.1 (2024-05-07)
 
 - Added a method to `WeightedDirectedGraph` to add a new node. 
 - Added a method to `WeightedDirectedGraph` to add a new edge. This can be doned given the desire weight, given a path between the nodes to connect and use the product of the weights or just let the graph find a path between nodes and use the product of the weights. 
+
+### Version 1.0.2 (2024-05-09)
+
+- Added a method to `WeightedDirectedGraph` to remove a node. 
+- Added a method to `WeightedDirectedGraph` to remove an edge.
```

### Comparing `pywgraph-1.0.1/tests/test_directed_edge.py` & `pywgraph-1.0.2/tests/test_directed_edge.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.1/tests/test_path_finding.py` & `pywgraph-1.0.2/tests/test_path_finding.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.1/tests/test_weighted_directed_edge.py` & `pywgraph-1.0.2/tests/test_weighted_directed_edge.py`

 * *Files identical despite different names*

### Comparing `pywgraph-1.0.1/tests/test_weighted_directed_graph.py` & `pywgraph-1.0.2/tests/test_weighted_directed_graph.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pytest
 from pywgraph import (
     WeightedDirectedGraph, 
     WeightedDirectedEdge, 
     NodeAlreadyExists, 
     NodeNotFound,
-    EdgeAlreadyExists
+    EdgeAlreadyExists,
+    EdgeNotFound
 )
 
 
 def graph() -> WeightedDirectedGraph:
     nodes = {"A", "B", "C"}
     edges = {
         WeightedDirectedEdge("A", "B", 7),
@@ -112,14 +113,33 @@
         update_dict["D"] = {}
         assert WeightedDirectedGraph.from_dict(update_dict) == graph_copy
 
     def test_add_node_exception(self):
         with pytest.raises(NodeAlreadyExists):
             graph().add_node("A")
 
+    def test_delete_node(self): 
+        graph_copy = graph()
+        new_dict = _dict_graph.copy()
+        del new_dict["A"]
+        new_graph = WeightedDirectedGraph.from_dict(new_dict)
+        assert graph_copy.delete_node("A", inplace=False) == new_graph
+
+    def test_delete_node_inplace(self):
+        graph_copy = graph()
+        new_dict = _dict_graph.copy()
+        del new_dict["A"]
+        new_graph = WeightedDirectedGraph.from_dict(new_dict)
+        graph_copy.delete_node("A", inplace=True)
+        assert graph_copy == new_graph
+
+    def test_delete_node_exception(self):
+        with pytest.raises(NodeNotFound):
+            graph().delete_node("D")
+
     # region Testing adding edges
     def test_add_edge_naive(self):
         graph_copy = graph()
         new_graph = graph_copy.add_edge("C", "A", 10, inplace=False)
         update_dict = _dict_graph.copy()
         update_dict["C"] = update_dict["C"] | {"A": 10}
         assert WeightedDirectedGraph.from_dict(update_dict) == new_graph
@@ -220,7 +240,32 @@
 
     def test_add_edge_existing_edge(self): 
         graph_copy = graph()
         with pytest.raises(EdgeAlreadyExists):
             graph_copy.add_edge(start="A", end="B", weight=2, inplace=True)
 
         assert graph_copy == graph()
+
+    def test_delete_edge(self): 
+        graph_copy = graph()
+        new_dict = _dict_graph.copy()
+        new_dict["B"] = {}
+        new_graph = WeightedDirectedGraph.from_dict(new_dict)
+        assert new_graph == graph_copy.delete_edge(start="B", end="C", inplace=False)
+
+    def test_delete_edge_inplace(self):
+        graph_copy = graph()
+        new_dict = _dict_graph.copy()
+        new_dict["B"] = {}
+        new_graph = WeightedDirectedGraph.from_dict(new_dict)
+        graph_copy.delete_edge(start="B", end="C", inplace=True)
+        assert graph_copy == new_graph
+
+    def test_delete_edge_bad_nodes(self):
+        graph_copy = graph()
+        with pytest.raises(NodeNotFound):
+            graph_copy.delete_edge(start="S", end="A")
+
+    def test_delete_edge_bad_edges(self):
+        graph_copy = graph()
+        with pytest.raises(EdgeNotFound):
+            graph_copy.delete_edge(start="C", end="B")
```

### Comparing `pywgraph-1.0.1/tests/test_weighted_directed_graph_arrays.py` & `pywgraph-1.0.2/tests/test_weighted_directed_graph_arrays.py`

 * *Files identical despite different names*

