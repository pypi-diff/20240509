# Comparing `tmp/ucxdsa-2024.4.23.tar.gz` & `tmp/ucxdsa-2024.5.9.tar.gz`

## Comparing `ucxdsa-2024.4.23.tar` & `ucxdsa-2024.5.9.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0    26445 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa.zip
--rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/test.ipynb
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/todo.md
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/__init__.py
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/array.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/doublylinkedlist.py
--rw-r--r--   0        0        0    18828 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/graph.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/hashtable.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/heap.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/huffman.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/pretty_print.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/queue.py
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/singlylinkedlist.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/sorttools.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/stack.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/tree.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/trie.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa.egg-info/PKG-INFO
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa.egg-info/top_level.txt
--rw-r--r--   0        0        0    35587 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/array.html
--rw-r--r--   0        0        0    22386 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/doublylinkedlist.html
--rw-r--r--   0        0        0    57112 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/graph.html
--rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/hashtable.html
--rw-r--r--   0        0        0    20103 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/heap.html
--rw-r--r--   0        0        0    15512 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/huffman.html
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/index.html
--rw-r--r--   0        0        0    12664 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/pretty_print.html
--rw-r--r--   0        0        0    22281 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/queue.html
--rw-r--r--   0        0        0    19253 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/singlylinkedlist.html
--rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/sorttools.html
--rw-r--r--   0        0        0    24822 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/stack.html
--rw-r--r--   0        0        0    18397 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/tree.html
--rw-r--r--   0        0        0    19308 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/trie.html
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/ucxdsa.egg-info/PKG-INFO
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/ucxdsa.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/ucxdsa.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/ucxdsa.egg-info/top_level.txt
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_array.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_doublylinkedlist.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_graph_list.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_graph_matrix.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_hash.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_heap.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_huffman.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_linkedlist.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_pretty_print.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_queue.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_stack.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_tree.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_trie.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/LICENSE
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/README.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/pyproject.toml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/PKG-INFO
+-rw-r--r--   0        0        0    67247 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa.zip
+-rw-r--r--   0        0        0    71345 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsadocs.zip
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/test.ipynb
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/todo.md
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/__init__.py
+-rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/array.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/doublylinkedlist.py
+-rw-r--r--   0        0        0    19119 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/graph.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/hashtable.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/heap.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/huffman.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/pretty_print.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/queue.py
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/singlylinkedlist.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/sorttools.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/stack.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/tree.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa/trie.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/dsa.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35804 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/array.html
+-rw-r--r--   0        0        0    28944 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/doublylinkedlist.html
+-rw-r--r--   0        0        0    78508 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/graph.html
+-rw-r--r--   0        0        0    18855 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/hashtable.html
+-rw-r--r--   0        0        0    33611 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/heap.html
+-rw-r--r--   0        0        0    15963 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/huffman.html
+-rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/index.html
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/pretty_print.html
+-rw-r--r--   0        0        0    22281 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/queue.html
+-rw-r--r--   0        0        0    25660 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/singlylinkedlist.html
+-rw-r--r--   0        0        0    11095 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/sorttools.html
+-rw-r--r--   0        0        0    24822 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/stack.html
+-rw-r--r--   0        0        0    23960 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/tree.html
+-rw-r--r--   0        0        0    27861 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/html/dsa/trie.html
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/ucxdsa.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/ucxdsa.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/ucxdsa.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/src/ucxdsa.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_array.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_doublylinkedlist.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_graph_list.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_graph_matrix.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_hash.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_heap.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_huffman.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_linkedlist.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_pretty_print.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_queue.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_stack.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_tree.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/tests/test_trie.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/LICENSE
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/README.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/pyproject.toml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 ucxdsa-2024.5.9/PKG-INFO
```

### Comparing `ucxdsa-2024.4.23/src/test.ipynb` & `ucxdsa-2024.5.9/src/test.ipynb`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa/array.py` & `ucxdsa-2024.5.9/src/dsa/array.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa/doublylinkedlist.py` & `ucxdsa-2024.5.9/src/dsa/doublylinkedlist.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa/graph.py` & `ucxdsa-2024.5.9/src/dsa/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,21 +564,22 @@
         return self.value
 
     def __lt__(self, vertex):
         return self.value < vertex.value
 
     
 #### Dijkstra's Algorithm Functions
-def shortest_path(start, end):
+def shortest_path(start, end, debug=False):
     """ 
     Helper function that returns a weight table and a previous vertex table using Dijkstra's Algorithm.
 
     Args:
         start: starting vertex
         end: ending vertex
+        debug: if True, display weight table as it is being built
     
     Returns:
     a tuple of a weight table dictionary and a previous path dictionary
     """
     weight_table = {}
     previous = {}
     visited = {}
@@ -586,55 +587,60 @@
     
     current = start
     queue.append(current)
     weight_table[current.value] = 0
     previous[current.value] = current
     
     while len(queue) > 0:
-        current_weight = weight_table.get(current.value, None)
+        current_weight = weight_table.get(current.value, float('inf'))
         visited[current.value] = True
 
-# for non-weighted version, use:
-# for adjacent in current.adjacents:
-#   weight = 1
-
+        # for non-weighted version, use:
+        # for adjacent in current.adjacents:
+        #   weight = 1
         for adjacent, weight in current.adjacents.items():
             if not visited.get(adjacent.value, False):
                 queue.append(adjacent)
 
-            wt = weight_table.get(adjacent.value, None)
-            if not wt or wt > weight + current_weight:
-                print(weight_table)
+            wt = weight_table.get(adjacent.value, float('inf'))
+            if wt > weight + current_weight:
                 weight_table[adjacent.value] = weight + current_weight
                 previous[adjacent.value] = current
+                if debug:
+                    print(weight_table)
 
         current = queue[0]
         del queue[0]
             
     return weight_table, previous
 
-def find_path(start, end):
+def find_path(start, end, debug=False):
     """ 
     Return the shortest path of two vertices using Dijkstra's Algorithm.
 
     Args:
         start: starting vertex
         end: ending vertex
+        debug: if True, display the weight table 
 
     Returns:
     A list of vertices that form a shortest path
     """
-    weight_table, previous = shortest_path(start, end)
+    weight_table, previous = shortest_path(start, end, debug)
     path = []
 
     current = end
     path.append(current.value)
     while current != start:
         current = previous[current.value]
         path.append(current.value)
         
     path.reverse()
-    print("weight table")
-    print(weight_table)
-    print("price ", weight_table[end.value])
+    if debug:
+        print("previous table")
+        print(previous)
+
+        print("weight table")
+        print(weight_table)
+        print("price ", weight_table[end.value])
     return path
```

### Comparing `ucxdsa-2024.4.23/src/dsa/hashtable.py` & `ucxdsa-2024.5.9/src/dsa/hashtable.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa/heap.py` & `ucxdsa-2024.5.9/src/dsa/heap.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa/huffman.py` & `ucxdsa-2024.5.9/src/dsa/huffman.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa/pretty_print.py` & `ucxdsa-2024.5.9/src/dsa/pretty_print.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa/queue.py` & `ucxdsa-2024.5.9/src/dsa/queue.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa/singlylinkedlist.py` & `ucxdsa-2024.5.9/src/dsa/singlylinkedlist.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa/sorttools.py` & `ucxdsa-2024.5.9/src/dsa/sorttools.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa/stack.py` & `ucxdsa-2024.5.9/src/dsa/stack.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa/tree.py` & `ucxdsa-2024.5.9/src/dsa/tree.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa/trie.py` & `ucxdsa-2024.5.9/src/dsa/trie.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/dsa.egg-info/PKG-INFO` & `ucxdsa-2024.5.9/src/dsa.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/html/dsa/array.html` & `ucxdsa-2024.5.9/src/html/dsa/array.html`

 * *Files 1% similar despite different names*

```diff
@@ -70,76 +70,76 @@
         
         Args:
             array: contains elements to be appended
         &#34;&#34;&#34;
         for e in array:
             self.append(e)
 
-    def insert(self, index, element):
+    def insert(self, index: int, element):
         &#34;&#34;&#34; 
         Insert an element at a specified index.  Raise IndexError if index is out of range.
         
         Args:
             index: index to insert an element
             element: the element to insert
         &#34;&#34;&#34;
         if index &lt; 0 or index &gt;= self.count:
             raise IndexError
 
         self.shift_right(self.count, index)
         self._array[index] = element
         self.count += 1
         
-    def shift_right(self, start, end):
+    def shift_right(self, start: int, end: int):
         &#34;&#34;&#34;
         a helper method to shift elements to the right
 
         Args:
             start: starting index of shift
             end: ending index of shift
         &#34;&#34;&#34;
         for i in range(start, end, -1):
             self._array[i] = self._array[i - 1]
 
-    def delete(self, index):
+    def delete(self, index: int):
         &#34;&#34;&#34;  
         Delete an element at a specified index. Raise IndexError if index is out of range.
 
         Args:
             index: index of the element to be deleted
         
         &#34;&#34;&#34;
         if index &gt;= self.count or index &lt; 0:
             raise IndexError
 
         self.shift_left(index, self.count)
         self.count -= 1
 
-    def shift_left(self, start, end):
+    def shift_left(self, start: int, end: int):
         &#34;&#34;&#34;
         a helper method to shift elements to the right
 
         Args:
             start: starting index of shift
             end: ending index of shift
         &#34;&#34;&#34;
         for i in range(start, end):
             self._array[i] = self._array[i + 1]
 
     ### special methods for handling index operator
-    def __getitem__(self, index):
+    def __getitem__(self, index: int):
         &#34;&#34;&#34;
         Returns: 
             the element at the specified index of an array
         &#34;&#34;&#34;
         if index &lt; 0 or index &gt;= self.count: 
             raise IndexError
         return self._array[index]
             
-    def __setitem__(self, index, value):
+    def __setitem__(self, index: int, value):
         &#34;&#34;&#34;
         set a new value at the specified index of an array
         &#34;&#34;&#34;
         if index &lt; 0 or index &gt;= self.count: 
             raise IndexError
         self._array[index] = value
         
@@ -147,15 +147,15 @@
     def __len__(self):
         &#34;&#34;&#34; 
         Returns: 
             the count of an array
         &#34;&#34;&#34;
         return self.count
 
-    def capacity(self):
+    def capacity(self) -&gt; int:
         &#34;&#34;&#34; 
         Returns:
             the capacity of an array
         &#34;&#34;&#34;
         return len(self._array)
 
     ### override the representation value with the Python interpreter
@@ -234,15 +234,15 @@
         
         Args:
             array: contains elements to be appended
         &#34;&#34;&#34;
         for e in array:
             self.append(e)
 
-    def insert(self, index, element):
+    def insert(self, index: int, element):
         &#34;&#34;&#34;  
         Insert an element at a specified index. Raise IndexError if index is out of range.
 
         Args:
             index: index to insert an element
             element: the element to insert
 
@@ -252,15 +252,15 @@
 
         self.check_capacity()
 
         self.shift_right(self.count, index)
         self._array[index] = element
         self.count += 1
         
-    def delete(self, index):
+    def delete(self, index: int):
         &#34;&#34;&#34;  
         Delete an element at a specified index. Raise IndexError if index is out of range.
 
         Args:
             index: index of the element to be deleted
         
         &#34;&#34;&#34;
@@ -352,76 +352,76 @@
         
         Args:
             array: contains elements to be appended
         &#34;&#34;&#34;
         for e in array:
             self.append(e)
 
-    def insert(self, index, element):
+    def insert(self, index: int, element):
         &#34;&#34;&#34; 
         Insert an element at a specified index.  Raise IndexError if index is out of range.
         
         Args:
             index: index to insert an element
             element: the element to insert
         &#34;&#34;&#34;
         if index &lt; 0 or index &gt;= self.count:
             raise IndexError
 
         self.shift_right(self.count, index)
         self._array[index] = element
         self.count += 1
         
-    def shift_right(self, start, end):
+    def shift_right(self, start: int, end: int):
         &#34;&#34;&#34;
         a helper method to shift elements to the right
 
         Args:
             start: starting index of shift
             end: ending index of shift
         &#34;&#34;&#34;
         for i in range(start, end, -1):
             self._array[i] = self._array[i - 1]
 
-    def delete(self, index):
+    def delete(self, index: int):
         &#34;&#34;&#34;  
         Delete an element at a specified index. Raise IndexError if index is out of range.
 
         Args:
             index: index of the element to be deleted
         
         &#34;&#34;&#34;
         if index &gt;= self.count or index &lt; 0:
             raise IndexError
 
         self.shift_left(index, self.count)
         self.count -= 1
 
-    def shift_left(self, start, end):
+    def shift_left(self, start: int, end: int):
         &#34;&#34;&#34;
         a helper method to shift elements to the right
 
         Args:
             start: starting index of shift
             end: ending index of shift
         &#34;&#34;&#34;
         for i in range(start, end):
             self._array[i] = self._array[i + 1]
 
     ### special methods for handling index operator
-    def __getitem__(self, index):
+    def __getitem__(self, index: int):
         &#34;&#34;&#34;
         Returns: 
             the element at the specified index of an array
         &#34;&#34;&#34;
         if index &lt; 0 or index &gt;= self.count: 
             raise IndexError
         return self._array[index]
             
-    def __setitem__(self, index, value):
+    def __setitem__(self, index: int, value):
         &#34;&#34;&#34;
         set a new value at the specified index of an array
         &#34;&#34;&#34;
         if index &lt; 0 or index &gt;= self.count: 
             raise IndexError
         self._array[index] = value
         
@@ -429,15 +429,15 @@
     def __len__(self):
         &#34;&#34;&#34; 
         Returns: 
             the count of an array
         &#34;&#34;&#34;
         return self.count
 
-    def capacity(self):
+    def capacity(self) -&gt; int:
         &#34;&#34;&#34; 
         Returns:
             the capacity of an array
         &#34;&#34;&#34;
         return len(self._array)
 
     ### override the representation value with the Python interpreter
@@ -486,46 +486,46 @@
         raise Exception(f&#34;Capacity Error: {len(self)} maximum&#34;)
 
     self._array[self.count] = element
     self.count += 1</code></pre>
 </details>
 </dd>
 <dt id="dsa.array.Array.capacity"><code class="name flex">
-<span>def <span class="ident">capacity</span></span>(<span>self)</span>
+<span>def <span class="ident">capacity</span></span>(<span>self) ‑> int</span>
 </code></dt>
 <dd>
 <div class="desc"><h2 id="returns">Returns</h2>
 <p>the capacity of an array</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def capacity(self):
+<pre><code class="python">def capacity(self) -&gt; int:
     &#34;&#34;&#34; 
     Returns:
         the capacity of an array
     &#34;&#34;&#34;
     return len(self._array)</code></pre>
 </details>
 </dd>
 <dt id="dsa.array.Array.delete"><code class="name flex">
-<span>def <span class="ident">delete</span></span>(<span>self, index)</span>
+<span>def <span class="ident">delete</span></span>(<span>self, index: int)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Delete an element at a specified index. Raise IndexError if index is out of range.</p>
 <h2 id="args">Args</h2>
 <dl>
 <dt><strong><code>index</code></strong></dt>
 <dd>index of the element to be deleted</dd>
 </dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def delete(self, index):
+<pre><code class="python">def delete(self, index: int):
     &#34;&#34;&#34;  
     Delete an element at a specified index. Raise IndexError if index is out of range.
 
     Args:
         index: index of the element to be deleted
     
     &#34;&#34;&#34;
@@ -558,15 +558,15 @@
         array: contains elements to be appended
     &#34;&#34;&#34;
     for e in array:
         self.append(e)</code></pre>
 </details>
 </dd>
 <dt id="dsa.array.Array.insert"><code class="name flex">
-<span>def <span class="ident">insert</span></span>(<span>self, index, element)</span>
+<span>def <span class="ident">insert</span></span>(<span>self, index: int, element)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Insert an element at a specified index.
 Raise IndexError if index is out of range.</p>
 <h2 id="args">Args</h2>
 <dl>
 <dt><strong><code>index</code></strong></dt>
@@ -574,15 +574,15 @@
 <dt><strong><code>element</code></strong></dt>
 <dd>the element to insert</dd>
 </dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def insert(self, index, element):
+<pre><code class="python">def insert(self, index: int, element):
     &#34;&#34;&#34; 
     Insert an element at a specified index.  Raise IndexError if index is out of range.
     
     Args:
         index: index to insert an element
         element: the element to insert
     &#34;&#34;&#34;
@@ -591,58 +591,58 @@
 
     self.shift_right(self.count, index)
     self._array[index] = element
     self.count += 1</code></pre>
 </details>
 </dd>
 <dt id="dsa.array.Array.shift_left"><code class="name flex">
-<span>def <span class="ident">shift_left</span></span>(<span>self, start, end)</span>
+<span>def <span class="ident">shift_left</span></span>(<span>self, start: int, end: int)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>a helper method to shift elements to the right</p>
 <h2 id="args">Args</h2>
 <dl>
 <dt><strong><code>start</code></strong></dt>
 <dd>starting index of shift</dd>
 <dt><strong><code>end</code></strong></dt>
 <dd>ending index of shift</dd>
 </dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def shift_left(self, start, end):
+<pre><code class="python">def shift_left(self, start: int, end: int):
     &#34;&#34;&#34;
     a helper method to shift elements to the right
 
     Args:
         start: starting index of shift
         end: ending index of shift
     &#34;&#34;&#34;
     for i in range(start, end):
         self._array[i] = self._array[i + 1]</code></pre>
 </details>
 </dd>
 <dt id="dsa.array.Array.shift_right"><code class="name flex">
-<span>def <span class="ident">shift_right</span></span>(<span>self, start, end)</span>
+<span>def <span class="ident">shift_right</span></span>(<span>self, start: int, end: int)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>a helper method to shift elements to the right</p>
 <h2 id="args">Args</h2>
 <dl>
 <dt><strong><code>start</code></strong></dt>
 <dd>starting index of shift</dd>
 <dt><strong><code>end</code></strong></dt>
 <dd>ending index of shift</dd>
 </dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def shift_right(self, start, end):
+<pre><code class="python">def shift_right(self, start: int, end: int):
     &#34;&#34;&#34;
     a helper method to shift elements to the right
 
     Args:
         start: starting index of shift
         end: ending index of shift
     &#34;&#34;&#34;
@@ -744,15 +744,15 @@
         
         Args:
             array: contains elements to be appended
         &#34;&#34;&#34;
         for e in array:
             self.append(e)
 
-    def insert(self, index, element):
+    def insert(self, index: int, element):
         &#34;&#34;&#34;  
         Insert an element at a specified index. Raise IndexError if index is out of range.
 
         Args:
             index: index to insert an element
             element: the element to insert
 
@@ -762,15 +762,15 @@
 
         self.check_capacity()
 
         self.shift_right(self.count, index)
         self._array[index] = element
         self.count += 1
         
-    def delete(self, index):
+    def delete(self, index: int):
         &#34;&#34;&#34;  
         Delete an element at a specified index. Raise IndexError if index is out of range.
 
         Args:
             index: index of the element to be deleted
         
         &#34;&#34;&#34;
@@ -882,30 +882,30 @@
     for i in range(len(self._array)):
         new_array[i] = self._array[i]
 
     self._array = new_array</code></pre>
 </details>
 </dd>
 <dt id="dsa.array.DynamicArray.insert"><code class="name flex">
-<span>def <span class="ident">insert</span></span>(<span>self, index, element)</span>
+<span>def <span class="ident">insert</span></span>(<span>self, index: int, element)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Insert an element at a specified index. Raise IndexError if index is out of range.</p>
 <h2 id="args">Args</h2>
 <dl>
 <dt><strong><code>index</code></strong></dt>
 <dd>index to insert an element</dd>
 <dt><strong><code>element</code></strong></dt>
 <dd>the element to insert</dd>
 </dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def insert(self, index, element):
+<pre><code class="python">def insert(self, index: int, element):
     &#34;&#34;&#34;  
     Insert an element at a specified index. Raise IndexError if index is out of range.
 
     Args:
         index: index to insert an element
         element: the element to insert
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -46,15 +46,15 @@
 
         Args:
             array: contains elements to be appended
         """
         for e in array:
             self.append(e)
 
-    def insert(self, index, element):
+    def insert(self, index: int, element):
         """
         Insert an element at a specified index.  Raise IndexError if index is
 out of range.
 
         Args:
             index: index to insert an element
             element: the element to insert
@@ -62,62 +62,62 @@
         if index < 0 or index >= self.count:
             raise IndexError
 
         self.shift_right(self.count, index)
         self._array[index] = element
         self.count += 1
 
-    def shift_right(self, start, end):
+    def shift_right(self, start: int, end: int):
         """
         a helper method to shift elements to the right
 
         Args:
             start: starting index of shift
             end: ending index of shift
         """
         for i in range(start, end, -1):
             self._array[i] = self._array[i - 1]
 
-    def delete(self, index):
+    def delete(self, index: int):
         """
         Delete an element at a specified index. Raise IndexError if index is
 out of range.
 
         Args:
             index: index of the element to be deleted
 
         """
         if index >= self.count or index < 0:
             raise IndexError
 
         self.shift_left(index, self.count)
         self.count -= 1
 
-    def shift_left(self, start, end):
+    def shift_left(self, start: int, end: int):
         """
         a helper method to shift elements to the right
 
         Args:
             start: starting index of shift
             end: ending index of shift
         """
         for i in range(start, end):
             self._array[i] = self._array[i + 1]
 
     ### special methods for handling index operator
-    def __getitem__(self, index):
+    def __getitem__(self, index: int):
         """
         Returns:
             the element at the specified index of an array
         """
         if index < 0 or index >= self.count:
             raise IndexError
         return self._array[index]
 
-    def __setitem__(self, index, value):
+    def __setitem__(self, index: int, value):
         """
         set a new value at the specified index of an array
         """
         if index < 0 or index >= self.count:
             raise IndexError
         self._array[index] = value
 
@@ -125,15 +125,15 @@
     def __len__(self):
         """
         Returns:
             the count of an array
         """
         return self.count
 
-    def capacity(self):
+    def capacity(self) -> int:
         """
         Returns:
             the capacity of an array
         """
         return len(self._array)
 
     ### override the representation value with the Python interpreter
@@ -214,15 +214,15 @@
 
         Args:
             array: contains elements to be appended
         """
         for e in array:
             self.append(e)
 
-    def insert(self, index, element):
+    def insert(self, index: int, element):
         """
         Insert an element at a specified index. Raise IndexError if index is
 out of range.
 
         Args:
             index: index to insert an element
             element: the element to insert
@@ -233,15 +233,15 @@
 
         self.check_capacity()
 
         self.shift_right(self.count, index)
         self._array[index] = element
         self.count += 1
 
-    def delete(self, index):
+    def delete(self, index: int):
         """
         Delete an element at a specified index. Raise IndexError if index is
 out of range.
 
         Args:
             index: index of the element to be deleted
 
@@ -317,15 +317,15 @@
 
               Args:
                   array: contains elements to be appended
               """
               for e in array:
                   self.append(e)
 
-          def insert(self, index, element):
+          def insert(self, index: int, element):
               """
               Insert an element at a specified index.  Raise IndexError if
       index is out of range.
 
               Args:
                   index: index to insert an element
                   element: the element to insert
@@ -333,62 +333,62 @@
               if index < 0 or index >= self.count:
                   raise IndexError
 
               self.shift_right(self.count, index)
               self._array[index] = element
               self.count += 1
 
-          def shift_right(self, start, end):
+          def shift_right(self, start: int, end: int):
               """
               a helper method to shift elements to the right
 
               Args:
                   start: starting index of shift
                   end: ending index of shift
               """
               for i in range(start, end, -1):
                   self._array[i] = self._array[i - 1]
 
-          def delete(self, index):
+          def delete(self, index: int):
               """
               Delete an element at a specified index. Raise IndexError if index
       is out of range.
 
               Args:
                   index: index of the element to be deleted
 
               """
               if index >= self.count or index < 0:
                   raise IndexError
 
               self.shift_left(index, self.count)
               self.count -= 1
 
-          def shift_left(self, start, end):
+          def shift_left(self, start: int, end: int):
               """
               a helper method to shift elements to the right
 
               Args:
                   start: starting index of shift
                   end: ending index of shift
               """
               for i in range(start, end):
                   self._array[i] = self._array[i + 1]
 
           ### special methods for handling index operator
-          def __getitem__(self, index):
+          def __getitem__(self, index: int):
               """
               Returns:
                   the element at the specified index of an array
               """
               if index < 0 or index >= self.count:
                   raise IndexError
               return self._array[index]
 
-          def __setitem__(self, index, value):
+          def __setitem__(self, index: int, value):
               """
               set a new value at the specified index of an array
               """
               if index < 0 or index >= self.count:
                   raise IndexError
               self._array[index] = value
 
@@ -396,15 +396,15 @@
           def __len__(self):
               """
               Returns:
                   the count of an array
               """
               return self.count
 
-          def capacity(self):
+          def capacity(self) -> int:
               """
               Returns:
                   the capacity of an array
               """
               return len(self._array)
 
           ### override the representation value with the Python interpreter
@@ -437,32 +437,32 @@
                     element: the element to append
                 """
                 if self.count >= self.capacity():
                     raise Exception(f"Capacity Error: {len(self)} maximum")
 
                 self._array[self.count] = element
                 self.count += 1
-        def capacity(self)
+        def capacity(self) ‑> int
             ********** RReettuurrnnss **********
             the capacity of an array
             Expand source code
-            def capacity(self):
+            def capacity(self) -> int:
                 """
                 Returns:
                     the capacity of an array
                 """
                 return len(self._array)
-        def delete(self, index)
+        def delete(self, index: int)
             Delete an element at a specified index. Raise IndexError if index
             is out of range.
             ********** AArrggss **********
               iinnddeexx
                   index of the element to be deleted
             Expand source code
-            def delete(self, index):
+            def delete(self, index: int):
                 """
                 Delete an element at a specified index. Raise IndexError if
             index is out of range.
 
                 Args:
                     index: index of the element to be deleted
 
@@ -485,65 +485,65 @@
             trying to add more elements than the capacity.
 
                 Args:
                     array: contains elements to be appended
                 """
                 for e in array:
                     self.append(e)
-        def insert(self, index, element)
+        def insert(self, index: int, element)
             Insert an element at a specified index. Raise IndexError if index
             is out of range.
             ********** AArrggss **********
               iinnddeexx
                   index to insert an element
               eelleemmeenntt
                   the element to insert
             Expand source code
-            def insert(self, index, element):
+            def insert(self, index: int, element):
                 """
                 Insert an element at a specified index.  Raise IndexError if
             index is out of range.
 
                 Args:
                     index: index to insert an element
                     element: the element to insert
                 """
                 if index < 0 or index >= self.count:
                     raise IndexError
 
                 self.shift_right(self.count, index)
                 self._array[index] = element
                 self.count += 1
-        def shift_left(self, start, end)
+        def shift_left(self, start: int, end: int)
             a helper method to shift elements to the right
             ********** AArrggss **********
               ssttaarrtt
                   starting index of shift
               eenndd
                   ending index of shift
             Expand source code
-            def shift_left(self, start, end):
+            def shift_left(self, start: int, end: int):
                 """
                 a helper method to shift elements to the right
 
                 Args:
                     start: starting index of shift
                     end: ending index of shift
                 """
                 for i in range(start, end):
                     self._array[i] = self._array[i + 1]
-        def shift_right(self, start, end)
+        def shift_right(self, start: int, end: int)
             a helper method to shift elements to the right
             ********** AArrggss **********
               ssttaarrtt
                   starting index of shift
               eenndd
                   ending index of shift
             Expand source code
-            def shift_right(self, start, end):
+            def shift_right(self, start: int, end: int):
                 """
                 a helper method to shift elements to the right
 
                 Args:
                     start: starting index of shift
                     end: ending index of shift
                 """
@@ -633,15 +633,15 @@
 
               Args:
                   array: contains elements to be appended
               """
               for e in array:
                   self.append(e)
 
-          def insert(self, index, element):
+          def insert(self, index: int, element):
               """
               Insert an element at a specified index. Raise IndexError if index
       is out of range.
 
               Args:
                   index: index to insert an element
                   element: the element to insert
@@ -652,15 +652,15 @@
 
               self.check_capacity()
 
               self.shift_right(self.count, index)
               self._array[index] = element
               self.count += 1
 
-          def delete(self, index):
+          def delete(self, index: int):
               """
               Delete an element at a specified index. Raise IndexError if index
       is out of range.
 
               Args:
                   index: index of the element to be deleted
 
@@ -736,24 +736,24 @@
                 new_array = [ None ] * new_size
 
                 # copy elements
                 for i in range(len(self._array)):
                     new_array[i] = self._array[i]
 
                 self._array = new_array
-        def insert(self, index, element)
+        def insert(self, index: int, element)
             Insert an element at a specified index. Raise IndexError if index
             is out of range.
             ********** AArrggss **********
               iinnddeexx
                   index to insert an element
               eelleemmeenntt
                   the element to insert
             Expand source code
-            def insert(self, index, element):
+            def insert(self, index: int, element):
                 """
                 Insert an element at a specified index. Raise IndexError if
             index is out of range.
 
                 Args:
                     index: index to insert an element
                     element: the element to insert
```

### Comparing `ucxdsa-2024.4.23/src/html/dsa/doublylinkedlist.html` & `ucxdsa-2024.5.9/src/html/dsa/singlylinkedlist.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,533 +1,677 @@
 <!doctype html>
 <html lang="en">
 <head>
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
 <meta name="generator" content="pdoc 0.10.0" />
-<title>dsa.doublylinkedlist API documentation</title>
+<title>dsa.singlylinkedlist API documentation</title>
 <meta name="description" content="" />
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
 <link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
 <style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
 <style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
 <style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
 <script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
 <script>window.addEventListener('DOMContentLoaded', () => hljs.initHighlighting())</script>
 </head>
 <body>
 <main>
 <article id="content">
 <header>
-<h1 class="title">Module <code>dsa.doublylinkedlist</code></h1>
+<h1 class="title">Module <code>dsa.singlylinkedlist</code></h1>
 </header>
 <section id="section-intro">
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">class Node:
+    &#34;&#34;&#34; 
+    A singly linked list node implementation in Python
+    &#34;&#34;&#34;
     def __init__(self, value):
+        &#34;&#34;&#34; 
+        Args:
+            value: the value of the node
+        &#34;&#34;&#34;
+        #: value of the node
         self.value = value
+        #: reference to the next node
         self.next = None
-        self.prev = None
-    
-class DoublyLinkedList:
-    def __init__(self, head=None, tail=None, count=0):
-        &#39;&#39;&#39; initialize a doubly linked list
-            accepts an optional head node, tail node and count
-            if only the head node is specified, tail is set to the head node and count is automatically set to 0
-            if both head and tail nodes are specified, count should be specified as well
-        &#39;&#39;&#39;
+
+class LinkedList:
+    &#34;&#34;&#34; 
+    A singly linked list implementation in Python
+    &#34;&#34;&#34;
+    def __init__(self, head: Node=None, tail: Node=None, count: int=0):
+        &#34;&#34;&#34; 
+        Initialize a singly linked list.
+        
+        if only the head node is specified, tail is set to the head node and count is automatically set to 0
+        if both head and tail nodes are specified, count should be specified as well
+        
+        Args:
+            head: reference to the head node
+            tail: reference to the tail node
+            count: the number of nodes in the linked list
+
+        &#34;&#34;&#34;        
         self.head = head
         if head is not None and tail is None:
             self.tail = head
             self.count = 1
         else:
             self.tail = tail
             self.count = count
 
     @classmethod
     def from_array(cls, mylist=None):
-        &#39;&#39;&#39; create a linked list from an array &#39;&#39;&#39;
+        &#34;&#34;&#34;
+        Create a linked list from an array.
+
+        Args:
+            mylist: an array or container to conver from
+        
+        Returns:
+            Linked List
+        &#34;&#34;&#34;
+        &#39;&#39;&#39;  &#39;&#39;&#39;
         ll = cls()
         for value in mylist:
             ll.append(value)
 
         return ll
-        
+    
+    def print(self):
+        &#34;&#34;&#34;
+        Print the contents of the linked list.
+        &#34;&#34;&#34;
+        current = self.head
+        while current is not None:
+            print(current.value, end=&#34; &#34;)
+            current = current.next
+        print()
+
+            
     def __repr__(self):
         s = &#34;&#34;
         current = self.head
         while current is not None:
             s += str(current.value) + &#34; &#34;
             current = current.next
 
         return f&#34;[{s}] Count: {self.count}&#34;
     
-    def print_reverse(self):
-        current = self.tail
-        while current is not None:
-            print(current.value, end=&#34; &#34;)
-            current = current.prev
-        print()
-
-    def search(self, value):
-        &#39;&#39;&#39; return index of specified value &#39;&#39;&#39;
+    def search(self, value) -&gt; int:
+        &#34;&#34;&#34;
+        Search for a value in the linked list.
+
+        Args:
+            value: value to search for
+
+        Returns:
+            return index of found value
+        &#34;&#34;&#34;
         i = 0
         current = self.head
         while current is not None:
             if current.value == value:
                 return i
             i += 1
             current = current.next
         raise Exception(&#34;Value not found&#34;)
     
-    def insert(self, index, value):
-        &#39;&#39;&#39; insert value at a specified index &#39;&#39;&#39;
+    def insert(self, index: int, value):
+        &#34;&#34;&#34;
+        Insert a value at a specified index.
+
+        Args:
+            index: the index to insert a value
+            value: a value to append
+        &#34;&#34;&#34;
+        i = 0
         
         # insert front
         if index == 0:
-            self.prepend(value)
+            new_node = Node(value)
+            new_node.next = self.head
+            self.head = new_node
+            self.count += 1
             return
             
-        i = 0
         current = self.head
         while index &lt; i or current is not None:
+            i += 1
             if i == index:
                 break
             current = current.next
-            i += 1
-
+        
         if index &gt; i:
             raise Exception(&#34;Index Out of Bounds&#34;)
         new_node = Node(value)
-        
-        new_node.next = current
-        new_node.prev = current.prev
-        current.prev = new_node
-        new_node.prev.next = new_node
-
+        tmp = current.next
+        current.next = new_node
+        new_node.next = tmp
         self.count += 1
 
         
-    def prepend(self, value):
-        &#39;&#39;&#39; prepend value at the beginning of the list &#39;&#39;&#39;
-        new_node = Node(value)
-        new_node.next = self.head
-        self.head.prev = new_node
-        self.head = new_node
-        self.count += 1
-
     def append(self, value):
-        &#39;&#39;&#39; append value to the end of the list &#39;&#39;&#39;
-        
+        &#34;&#34;&#34;
+        Place a value at the end of the linked list.
+
+        Args:
+            value: a value to append
+        &#34;&#34;&#34;
         if self.head is None:
             self.head = Node(value)
             if self.count == 0:
                 self.tail = self.head
             self.count += 1
             return
-        
+
         # go to the end of the list
         new_node = Node(value)
-        new_node.prev = self.tail
         self.tail.next = new_node
         self.tail = new_node
         
         self.count += 1
-        
-
-    def delete(self, index):
-        &#39;&#39;&#39; delete node at a specified index &#39;&#39;&#39;
-        if self.head is None:
-            raise Exception(&#34;DoublyLinkedList is Empty&#34;)
 
-        i = 0
+    def delete(self, index: int):
+        &#34;&#34;&#34;
+        Delete a node at a specified index. Raise Exception if linked list is empty or if index is not found.
+
+        Args:
+            index: index of element to be deleted
+        &#34;&#34;&#34;
         if index == 0:
+            if self.head is None:
+                raise Exception(&#34;LinkedList is Empty&#34;)
             self.head = self.head.next
-            if self.head is not None:
-                self.head.prev = None
             self.count -= 1
             return
         
+        i = 0
         current = self.head
+        prev = current
         while current is not None:
             if index == i:
-                current.prev.next = current.next
-                if current.next is not None:
-                    current.next.prev = current.prev
-                else:
-                    self.tail = current.prev
-
+                prev.next = current.next
                 self.count -= 1
                 return
-            current = current.next
             i += 1
-        raise Exception(&#34;Index not found&#34;)</code></pre>
+            prev = current
+            current = current.next
+        raise Exception(&#34;Index not found&#34;)
+        
+    </code></pre>
 </details>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
 <h2 class="section-title" id="header-classes">Classes</h2>
 <dl>
-<dt id="dsa.doublylinkedlist.DoublyLinkedList"><code class="flex name class">
-<span>class <span class="ident">DoublyLinkedList</span></span>
-<span>(</span><span>head=None, tail=None, count=0)</span>
+<dt id="dsa.singlylinkedlist.LinkedList"><code class="flex name class">
+<span>class <span class="ident">LinkedList</span></span>
+<span>(</span><span>head: <a title="dsa.singlylinkedlist.Node" href="#dsa.singlylinkedlist.Node">Node</a> = None, tail: <a title="dsa.singlylinkedlist.Node" href="#dsa.singlylinkedlist.Node">Node</a> = None, count: int = 0)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>initialize a doubly linked list
-accepts an optional head node, tail node and count
-if only the head node is specified, tail is set to the head node and count is automatically set to 0
-if both head and tail nodes are specified, count should be specified as well</p></div>
+<div class="desc"><p>A singly linked list implementation in Python</p>
+<p>Initialize a singly linked list.</p>
+<p>if only the head node is specified, tail is set to the head node and count is automatically set to 0
+if both head and tail nodes are specified, count should be specified as well</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>head</code></strong></dt>
+<dd>reference to the head node</dd>
+<dt><strong><code>tail</code></strong></dt>
+<dd>reference to the tail node</dd>
+<dt><strong><code>count</code></strong></dt>
+<dd>the number of nodes in the linked list</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">class DoublyLinkedList:
-    def __init__(self, head=None, tail=None, count=0):
-        &#39;&#39;&#39; initialize a doubly linked list
-            accepts an optional head node, tail node and count
-            if only the head node is specified, tail is set to the head node and count is automatically set to 0
-            if both head and tail nodes are specified, count should be specified as well
-        &#39;&#39;&#39;
+<pre><code class="python">class LinkedList:
+    &#34;&#34;&#34; 
+    A singly linked list implementation in Python
+    &#34;&#34;&#34;
+    def __init__(self, head: Node=None, tail: Node=None, count: int=0):
+        &#34;&#34;&#34; 
+        Initialize a singly linked list.
+        
+        if only the head node is specified, tail is set to the head node and count is automatically set to 0
+        if both head and tail nodes are specified, count should be specified as well
+        
+        Args:
+            head: reference to the head node
+            tail: reference to the tail node
+            count: the number of nodes in the linked list
+
+        &#34;&#34;&#34;        
         self.head = head
         if head is not None and tail is None:
             self.tail = head
             self.count = 1
         else:
             self.tail = tail
             self.count = count
 
     @classmethod
     def from_array(cls, mylist=None):
-        &#39;&#39;&#39; create a linked list from an array &#39;&#39;&#39;
+        &#34;&#34;&#34;
+        Create a linked list from an array.
+
+        Args:
+            mylist: an array or container to conver from
+        
+        Returns:
+            Linked List
+        &#34;&#34;&#34;
+        &#39;&#39;&#39;  &#39;&#39;&#39;
         ll = cls()
         for value in mylist:
             ll.append(value)
 
         return ll
-        
+    
+    def print(self):
+        &#34;&#34;&#34;
+        Print the contents of the linked list.
+        &#34;&#34;&#34;
+        current = self.head
+        while current is not None:
+            print(current.value, end=&#34; &#34;)
+            current = current.next
+        print()
+
+            
     def __repr__(self):
         s = &#34;&#34;
         current = self.head
         while current is not None:
             s += str(current.value) + &#34; &#34;
             current = current.next
 
         return f&#34;[{s}] Count: {self.count}&#34;
     
-    def print_reverse(self):
-        current = self.tail
-        while current is not None:
-            print(current.value, end=&#34; &#34;)
-            current = current.prev
-        print()
-
-    def search(self, value):
-        &#39;&#39;&#39; return index of specified value &#39;&#39;&#39;
+    def search(self, value) -&gt; int:
+        &#34;&#34;&#34;
+        Search for a value in the linked list.
+
+        Args:
+            value: value to search for
+
+        Returns:
+            return index of found value
+        &#34;&#34;&#34;
         i = 0
         current = self.head
         while current is not None:
             if current.value == value:
                 return i
             i += 1
             current = current.next
         raise Exception(&#34;Value not found&#34;)
     
-    def insert(self, index, value):
-        &#39;&#39;&#39; insert value at a specified index &#39;&#39;&#39;
+    def insert(self, index: int, value):
+        &#34;&#34;&#34;
+        Insert a value at a specified index.
+
+        Args:
+            index: the index to insert a value
+            value: a value to append
+        &#34;&#34;&#34;
+        i = 0
         
         # insert front
         if index == 0:
-            self.prepend(value)
+            new_node = Node(value)
+            new_node.next = self.head
+            self.head = new_node
+            self.count += 1
             return
             
-        i = 0
         current = self.head
         while index &lt; i or current is not None:
+            i += 1
             if i == index:
                 break
             current = current.next
-            i += 1
-
+        
         if index &gt; i:
             raise Exception(&#34;Index Out of Bounds&#34;)
         new_node = Node(value)
-        
-        new_node.next = current
-        new_node.prev = current.prev
-        current.prev = new_node
-        new_node.prev.next = new_node
-
+        tmp = current.next
+        current.next = new_node
+        new_node.next = tmp
         self.count += 1
 
         
-    def prepend(self, value):
-        &#39;&#39;&#39; prepend value at the beginning of the list &#39;&#39;&#39;
-        new_node = Node(value)
-        new_node.next = self.head
-        self.head.prev = new_node
-        self.head = new_node
-        self.count += 1
-
     def append(self, value):
-        &#39;&#39;&#39; append value to the end of the list &#39;&#39;&#39;
-        
+        &#34;&#34;&#34;
+        Place a value at the end of the linked list.
+
+        Args:
+            value: a value to append
+        &#34;&#34;&#34;
         if self.head is None:
             self.head = Node(value)
             if self.count == 0:
                 self.tail = self.head
             self.count += 1
             return
-        
+
         # go to the end of the list
         new_node = Node(value)
-        new_node.prev = self.tail
         self.tail.next = new_node
         self.tail = new_node
         
         self.count += 1
-        
-
-    def delete(self, index):
-        &#39;&#39;&#39; delete node at a specified index &#39;&#39;&#39;
-        if self.head is None:
-            raise Exception(&#34;DoublyLinkedList is Empty&#34;)
 
-        i = 0
+    def delete(self, index: int):
+        &#34;&#34;&#34;
+        Delete a node at a specified index. Raise Exception if linked list is empty or if index is not found.
+
+        Args:
+            index: index of element to be deleted
+        &#34;&#34;&#34;
         if index == 0:
+            if self.head is None:
+                raise Exception(&#34;LinkedList is Empty&#34;)
             self.head = self.head.next
-            if self.head is not None:
-                self.head.prev = None
             self.count -= 1
             return
         
+        i = 0
         current = self.head
+        prev = current
         while current is not None:
             if index == i:
-                current.prev.next = current.next
-                if current.next is not None:
-                    current.next.prev = current.prev
-                else:
-                    self.tail = current.prev
-
+                prev.next = current.next
                 self.count -= 1
                 return
-            current = current.next
             i += 1
+            prev = current
+            current = current.next
         raise Exception(&#34;Index not found&#34;)</code></pre>
 </details>
 <h3>Static methods</h3>
 <dl>
-<dt id="dsa.doublylinkedlist.DoublyLinkedList.from_array"><code class="name flex">
+<dt id="dsa.singlylinkedlist.LinkedList.from_array"><code class="name flex">
 <span>def <span class="ident">from_array</span></span>(<span>mylist=None)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>create a linked list from an array</p></div>
+<div class="desc"><p>Create a linked list from an array.</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>mylist</code></strong></dt>
+<dd>an array or container to conver from</dd>
+</dl>
+<h2 id="returns">Returns</h2>
+<p>Linked List</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">@classmethod
 def from_array(cls, mylist=None):
-    &#39;&#39;&#39; create a linked list from an array &#39;&#39;&#39;
+    &#34;&#34;&#34;
+    Create a linked list from an array.
+
+    Args:
+        mylist: an array or container to conver from
+    
+    Returns:
+        Linked List
+    &#34;&#34;&#34;
+    &#39;&#39;&#39;  &#39;&#39;&#39;
     ll = cls()
     for value in mylist:
         ll.append(value)
 
     return ll</code></pre>
 </details>
 </dd>
 </dl>
 <h3>Methods</h3>
 <dl>
-<dt id="dsa.doublylinkedlist.DoublyLinkedList.append"><code class="name flex">
+<dt id="dsa.singlylinkedlist.LinkedList.append"><code class="name flex">
 <span>def <span class="ident">append</span></span>(<span>self, value)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>append value to the end of the list</p></div>
+<div class="desc"><p>Place a value at the end of the linked list.</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>value</code></strong></dt>
+<dd>a value to append</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def append(self, value):
-    &#39;&#39;&#39; append value to the end of the list &#39;&#39;&#39;
-    
+    &#34;&#34;&#34;
+    Place a value at the end of the linked list.
+
+    Args:
+        value: a value to append
+    &#34;&#34;&#34;
     if self.head is None:
         self.head = Node(value)
         if self.count == 0:
             self.tail = self.head
         self.count += 1
         return
-    
+
     # go to the end of the list
     new_node = Node(value)
-    new_node.prev = self.tail
     self.tail.next = new_node
     self.tail = new_node
     
     self.count += 1</code></pre>
 </details>
 </dd>
-<dt id="dsa.doublylinkedlist.DoublyLinkedList.delete"><code class="name flex">
-<span>def <span class="ident">delete</span></span>(<span>self, index)</span>
+<dt id="dsa.singlylinkedlist.LinkedList.delete"><code class="name flex">
+<span>def <span class="ident">delete</span></span>(<span>self, index: int)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>delete node at a specified index</p></div>
+<div class="desc"><p>Delete a node at a specified index. Raise Exception if linked list is empty or if index is not found.</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>index</code></strong></dt>
+<dd>index of element to be deleted</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def delete(self, index):
-    &#39;&#39;&#39; delete node at a specified index &#39;&#39;&#39;
-    if self.head is None:
-        raise Exception(&#34;DoublyLinkedList is Empty&#34;)
-
-    i = 0
+<pre><code class="python">def delete(self, index: int):
+    &#34;&#34;&#34;
+    Delete a node at a specified index. Raise Exception if linked list is empty or if index is not found.
+
+    Args:
+        index: index of element to be deleted
+    &#34;&#34;&#34;
     if index == 0:
+        if self.head is None:
+            raise Exception(&#34;LinkedList is Empty&#34;)
         self.head = self.head.next
-        if self.head is not None:
-            self.head.prev = None
         self.count -= 1
         return
     
+    i = 0
     current = self.head
+    prev = current
     while current is not None:
         if index == i:
-            current.prev.next = current.next
-            if current.next is not None:
-                current.next.prev = current.prev
-            else:
-                self.tail = current.prev
-
+            prev.next = current.next
             self.count -= 1
             return
-        current = current.next
         i += 1
+        prev = current
+        current = current.next
     raise Exception(&#34;Index not found&#34;)</code></pre>
 </details>
 </dd>
-<dt id="dsa.doublylinkedlist.DoublyLinkedList.insert"><code class="name flex">
-<span>def <span class="ident">insert</span></span>(<span>self, index, value)</span>
+<dt id="dsa.singlylinkedlist.LinkedList.insert"><code class="name flex">
+<span>def <span class="ident">insert</span></span>(<span>self, index: int, value)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>insert value at a specified index</p></div>
+<div class="desc"><p>Insert a value at a specified index.</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>index</code></strong></dt>
+<dd>the index to insert a value</dd>
+<dt><strong><code>value</code></strong></dt>
+<dd>a value to append</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def insert(self, index, value):
-    &#39;&#39;&#39; insert value at a specified index &#39;&#39;&#39;
+<pre><code class="python">def insert(self, index: int, value):
+    &#34;&#34;&#34;
+    Insert a value at a specified index.
+
+    Args:
+        index: the index to insert a value
+        value: a value to append
+    &#34;&#34;&#34;
+    i = 0
     
     # insert front
     if index == 0:
-        self.prepend(value)
+        new_node = Node(value)
+        new_node.next = self.head
+        self.head = new_node
+        self.count += 1
         return
         
-    i = 0
     current = self.head
     while index &lt; i or current is not None:
+        i += 1
         if i == index:
             break
         current = current.next
-        i += 1
-
+    
     if index &gt; i:
         raise Exception(&#34;Index Out of Bounds&#34;)
     new_node = Node(value)
-    
-    new_node.next = current
-    new_node.prev = current.prev
-    current.prev = new_node
-    new_node.prev.next = new_node
-
+    tmp = current.next
+    current.next = new_node
+    new_node.next = tmp
     self.count += 1</code></pre>
 </details>
 </dd>
-<dt id="dsa.doublylinkedlist.DoublyLinkedList.prepend"><code class="name flex">
-<span>def <span class="ident">prepend</span></span>(<span>self, value)</span>
+<dt id="dsa.singlylinkedlist.LinkedList.print"><code class="name flex">
+<span>def <span class="ident">print</span></span>(<span>self)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>prepend value at the beginning of the list</p></div>
+<div class="desc"><p>Print the contents of the linked list.</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def prepend(self, value):
-    &#39;&#39;&#39; prepend value at the beginning of the list &#39;&#39;&#39;
-    new_node = Node(value)
-    new_node.next = self.head
-    self.head.prev = new_node
-    self.head = new_node
-    self.count += 1</code></pre>
-</details>
-</dd>
-<dt id="dsa.doublylinkedlist.DoublyLinkedList.print_reverse"><code class="name flex">
-<span>def <span class="ident">print_reverse</span></span>(<span>self)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def print_reverse(self):
-    current = self.tail
+<pre><code class="python">def print(self):
+    &#34;&#34;&#34;
+    Print the contents of the linked list.
+    &#34;&#34;&#34;
+    current = self.head
     while current is not None:
         print(current.value, end=&#34; &#34;)
-        current = current.prev
+        current = current.next
     print()</code></pre>
 </details>
 </dd>
-<dt id="dsa.doublylinkedlist.DoublyLinkedList.search"><code class="name flex">
-<span>def <span class="ident">search</span></span>(<span>self, value)</span>
+<dt id="dsa.singlylinkedlist.LinkedList.search"><code class="name flex">
+<span>def <span class="ident">search</span></span>(<span>self, value) ‑> int</span>
 </code></dt>
 <dd>
-<div class="desc"><p>return index of specified value</p></div>
+<div class="desc"><p>Search for a value in the linked list.</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>value</code></strong></dt>
+<dd>value to search for</dd>
+</dl>
+<h2 id="returns">Returns</h2>
+<p>return index of found value</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def search(self, value):
-    &#39;&#39;&#39; return index of specified value &#39;&#39;&#39;
+<pre><code class="python">def search(self, value) -&gt; int:
+    &#34;&#34;&#34;
+    Search for a value in the linked list.
+
+    Args:
+        value: value to search for
+
+    Returns:
+        return index of found value
+    &#34;&#34;&#34;
     i = 0
     current = self.head
     while current is not None:
         if current.value == value:
             return i
         i += 1
         current = current.next
     raise Exception(&#34;Value not found&#34;)</code></pre>
 </details>
 </dd>
 </dl>
 </dd>
-<dt id="dsa.doublylinkedlist.Node"><code class="flex name class">
+<dt id="dsa.singlylinkedlist.Node"><code class="flex name class">
 <span>class <span class="ident">Node</span></span>
 <span>(</span><span>value)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>A singly linked list node implementation in Python</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>value</code></strong></dt>
+<dd>the value of the node</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">class Node:
+    &#34;&#34;&#34; 
+    A singly linked list node implementation in Python
+    &#34;&#34;&#34;
     def __init__(self, value):
+        &#34;&#34;&#34; 
+        Args:
+            value: the value of the node
+        &#34;&#34;&#34;
+        #: value of the node
         self.value = value
-        self.next = None
-        self.prev = None</code></pre>
+        #: reference to the next node
+        self.next = None</code></pre>
 </details>
+<h3>Instance variables</h3>
+<dl>
+<dt id="dsa.singlylinkedlist.Node.next"><code class="name">var <span class="ident">next</span></code></dt>
+<dd>
+<div class="desc"><p>reference to the next node</p></div>
+</dd>
+<dt id="dsa.singlylinkedlist.Node.value"><code class="name">var <span class="ident">value</span></code></dt>
+<dd>
+<div class="desc"><p>value of the node</p></div>
+</dd>
+</dl>
 </dd>
 </dl>
 </section>
 </article>
 <nav id="sidebar">
 <h1>Index</h1>
 <div class="toc">
@@ -538,27 +682,30 @@
 <ul>
 <li><code><a title="dsa" href="index.html">dsa</a></code></li>
 </ul>
 </li>
 <li><h3><a href="#header-classes">Classes</a></h3>
 <ul>
 <li>
-<h4><code><a title="dsa.doublylinkedlist.DoublyLinkedList" href="#dsa.doublylinkedlist.DoublyLinkedList">DoublyLinkedList</a></code></h4>
+<h4><code><a title="dsa.singlylinkedlist.LinkedList" href="#dsa.singlylinkedlist.LinkedList">LinkedList</a></code></h4>
 <ul class="two-column">
-<li><code><a title="dsa.doublylinkedlist.DoublyLinkedList.append" href="#dsa.doublylinkedlist.DoublyLinkedList.append">append</a></code></li>
-<li><code><a title="dsa.doublylinkedlist.DoublyLinkedList.delete" href="#dsa.doublylinkedlist.DoublyLinkedList.delete">delete</a></code></li>
-<li><code><a title="dsa.doublylinkedlist.DoublyLinkedList.from_array" href="#dsa.doublylinkedlist.DoublyLinkedList.from_array">from_array</a></code></li>
-<li><code><a title="dsa.doublylinkedlist.DoublyLinkedList.insert" href="#dsa.doublylinkedlist.DoublyLinkedList.insert">insert</a></code></li>
-<li><code><a title="dsa.doublylinkedlist.DoublyLinkedList.prepend" href="#dsa.doublylinkedlist.DoublyLinkedList.prepend">prepend</a></code></li>
-<li><code><a title="dsa.doublylinkedlist.DoublyLinkedList.print_reverse" href="#dsa.doublylinkedlist.DoublyLinkedList.print_reverse">print_reverse</a></code></li>
-<li><code><a title="dsa.doublylinkedlist.DoublyLinkedList.search" href="#dsa.doublylinkedlist.DoublyLinkedList.search">search</a></code></li>
+<li><code><a title="dsa.singlylinkedlist.LinkedList.append" href="#dsa.singlylinkedlist.LinkedList.append">append</a></code></li>
+<li><code><a title="dsa.singlylinkedlist.LinkedList.delete" href="#dsa.singlylinkedlist.LinkedList.delete">delete</a></code></li>
+<li><code><a title="dsa.singlylinkedlist.LinkedList.from_array" href="#dsa.singlylinkedlist.LinkedList.from_array">from_array</a></code></li>
+<li><code><a title="dsa.singlylinkedlist.LinkedList.insert" href="#dsa.singlylinkedlist.LinkedList.insert">insert</a></code></li>
+<li><code><a title="dsa.singlylinkedlist.LinkedList.print" href="#dsa.singlylinkedlist.LinkedList.print">print</a></code></li>
+<li><code><a title="dsa.singlylinkedlist.LinkedList.search" href="#dsa.singlylinkedlist.LinkedList.search">search</a></code></li>
 </ul>
 </li>
 <li>
-<h4><code><a title="dsa.doublylinkedlist.Node" href="#dsa.doublylinkedlist.Node">Node</a></code></h4>
+<h4><code><a title="dsa.singlylinkedlist.Node" href="#dsa.singlylinkedlist.Node">Node</a></code></h4>
+<ul class="">
+<li><code><a title="dsa.singlylinkedlist.Node.next" href="#dsa.singlylinkedlist.Node.next">next</a></code></li>
+<li><code><a title="dsa.singlylinkedlist.Node.value" href="#dsa.singlylinkedlist.Node.value">value</a></code></li>
+</ul>
 </li>
 </ul>
 </li>
 </ul>
 </nav>
 </main>
 <footer id="footer">
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,429 +1,569 @@
-************ MMoodduullee ddssaa..ddoouubbllyylliinnkkeeddlliisstt ************
+************ MMoodduullee ddssaa..ssiinnggllyylliinnkkeeddlliisstt ************
 Expand source code
 class Node:
+    """
+    A singly linked list node implementation in Python
+    """
     def __init__(self, value):
+        """
+        Args:
+            value: the value of the node
+        """
+        #: value of the node
         self.value = value
+        #: reference to the next node
         self.next = None
-        self.prev = None
 
-class DoublyLinkedList:
-    def __init__(self, head=None, tail=None, count=0):
-        ''' initialize a doubly linked list
-            accepts an optional head node, tail node and count
-            if only the head node is specified, tail is set to the head node
-and count is automatically set to 0
-            if both head and tail nodes are specified, count should be
-specified as well
-        '''
+class LinkedList:
+    """
+    A singly linked list implementation in Python
+    """
+    def __init__(self, head: Node=None, tail: Node=None, count: int=0):
+        """
+        Initialize a singly linked list.
+
+        if only the head node is specified, tail is set to the head node and
+count is automatically set to 0
+        if both head and tail nodes are specified, count should be specified as
+well
+
+        Args:
+            head: reference to the head node
+            tail: reference to the tail node
+            count: the number of nodes in the linked list
+
+        """
         self.head = head
         if head is not None and tail is None:
             self.tail = head
             self.count = 1
         else:
             self.tail = tail
             self.count = count
 
     @classmethod
     def from_array(cls, mylist=None):
-        ''' create a linked list from an array '''
+        """
+        Create a linked list from an array.
+
+        Args:
+            mylist: an array or container to conver from
+
+        Returns:
+            Linked List
+        """
+        '''  '''
         ll = cls()
         for value in mylist:
             ll.append(value)
 
         return ll
 
+    def print(self):
+        """
+        Print the contents of the linked list.
+        """
+        current = self.head
+        while current is not None:
+            print(current.value, end=" ")
+            current = current.next
+        print()
+
+
     def __repr__(self):
         s = ""
         current = self.head
         while current is not None:
             s += str(current.value) + " "
             current = current.next
 
         return f"[{s}] Count: {self.count}"
 
-    def print_reverse(self):
-        current = self.tail
-        while current is not None:
-            print(current.value, end=" ")
-            current = current.prev
-        print()
-
-    def search(self, value):
-        ''' return index of specified value '''
+    def search(self, value) -> int:
+        """
+        Search for a value in the linked list.
+
+        Args:
+            value: value to search for
+
+        Returns:
+            return index of found value
+        """
         i = 0
         current = self.head
         while current is not None:
             if current.value == value:
                 return i
             i += 1
             current = current.next
         raise Exception("Value not found")
 
-    def insert(self, index, value):
-        ''' insert value at a specified index '''
+    def insert(self, index: int, value):
+        """
+        Insert a value at a specified index.
+
+        Args:
+            index: the index to insert a value
+            value: a value to append
+        """
+        i = 0
 
         # insert front
         if index == 0:
-            self.prepend(value)
+            new_node = Node(value)
+            new_node.next = self.head
+            self.head = new_node
+            self.count += 1
             return
 
-        i = 0
         current = self.head
         while index < i or current is not None:
+            i += 1
             if i == index:
                 break
             current = current.next
-            i += 1
 
         if index > i:
             raise Exception("Index Out of Bounds")
         new_node = Node(value)
-
-        new_node.next = current
-        new_node.prev = current.prev
-        current.prev = new_node
-        new_node.prev.next = new_node
-
+        tmp = current.next
+        current.next = new_node
+        new_node.next = tmp
         self.count += 1
 
 
-    def prepend(self, value):
-        ''' prepend value at the beginning of the list '''
-        new_node = Node(value)
-        new_node.next = self.head
-        self.head.prev = new_node
-        self.head = new_node
-        self.count += 1
-
     def append(self, value):
-        ''' append value to the end of the list '''
+        """
+        Place a value at the end of the linked list.
 
+        Args:
+            value: a value to append
+        """
         if self.head is None:
             self.head = Node(value)
             if self.count == 0:
                 self.tail = self.head
             self.count += 1
             return
 
         # go to the end of the list
         new_node = Node(value)
-        new_node.prev = self.tail
         self.tail.next = new_node
         self.tail = new_node
 
         self.count += 1
 
-
-    def delete(self, index):
-        ''' delete node at a specified index '''
-        if self.head is None:
-            raise Exception("DoublyLinkedList is Empty")
-
-        i = 0
+    def delete(self, index: int):
+        """
+        Delete a node at a specified index. Raise Exception if linked list is
+empty or if index is not found.
+
+        Args:
+            index: index of element to be deleted
+        """
         if index == 0:
+            if self.head is None:
+                raise Exception("LinkedList is Empty")
             self.head = self.head.next
-            if self.head is not None:
-                self.head.prev = None
             self.count -= 1
             return
 
+        i = 0
         current = self.head
+        prev = current
         while current is not None:
             if index == i:
-                current.prev.next = current.next
-                if current.next is not None:
-                    current.next.prev = current.prev
-                else:
-                    self.tail = current.prev
-
+                prev.next = current.next
                 self.count -= 1
                 return
-            current = current.next
             i += 1
+            prev = current
+            current = current.next
         raise Exception("Index not found")
+
+
 ********** CCllaasssseess **********
-  class DoublyLinkedList (head=None, tail=None, count=0)
-      initialize a doubly linked list accepts an optional head node, tail node
-      and count if only the head node is specified, tail is set to the head
-      node and count is automatically set to 0 if both head and tail nodes are
+  class LinkedList (head: _N_o_d_e = None, tail: _N_o_d_e = None, count: int = 0)
+      A singly linked list implementation in Python
+      Initialize a singly linked list.
+      if only the head node is specified, tail is set to the head node and
+      count is automatically set to 0 if both head and tail nodes are
       specified, count should be specified as well
+      ********** AArrggss **********
+        hheeaadd
+            reference to the head node
+        ttaaiill
+            reference to the tail node
+        ccoouunntt
+            the number of nodes in the linked list
       Expand source code
-      class DoublyLinkedList:
-          def __init__(self, head=None, tail=None, count=0):
-              ''' initialize a doubly linked list
-                  accepts an optional head node, tail node and count
-                  if only the head node is specified, tail is set to the head
-      node and count is automatically set to 0
-                  if both head and tail nodes are specified, count should be
+      class LinkedList:
+          """
+          A singly linked list implementation in Python
+          """
+          def __init__(self, head: Node=None, tail: Node=None, count: int=0):
+              """
+              Initialize a singly linked list.
+
+              if only the head node is specified, tail is set to the head node
+      and count is automatically set to 0
+              if both head and tail nodes are specified, count should be
       specified as well
-              '''
+
+              Args:
+                  head: reference to the head node
+                  tail: reference to the tail node
+                  count: the number of nodes in the linked list
+
+              """
               self.head = head
               if head is not None and tail is None:
                   self.tail = head
                   self.count = 1
               else:
                   self.tail = tail
                   self.count = count
 
           @classmethod
           def from_array(cls, mylist=None):
-              ''' create a linked list from an array '''
+              """
+              Create a linked list from an array.
+
+              Args:
+                  mylist: an array or container to conver from
+
+              Returns:
+                  Linked List
+              """
+              '''  '''
               ll = cls()
               for value in mylist:
                   ll.append(value)
 
               return ll
 
+          def print(self):
+              """
+              Print the contents of the linked list.
+              """
+              current = self.head
+              while current is not None:
+                  print(current.value, end=" ")
+                  current = current.next
+              print()
+
+
           def __repr__(self):
               s = ""
               current = self.head
               while current is not None:
                   s += str(current.value) + " "
                   current = current.next
 
               return f"[{s}] Count: {self.count}"
 
-          def print_reverse(self):
-              current = self.tail
-              while current is not None:
-                  print(current.value, end=" ")
-                  current = current.prev
-              print()
-
-          def search(self, value):
-              ''' return index of specified value '''
+          def search(self, value) -> int:
+              """
+              Search for a value in the linked list.
+
+              Args:
+                  value: value to search for
+
+              Returns:
+                  return index of found value
+              """
               i = 0
               current = self.head
               while current is not None:
                   if current.value == value:
                       return i
                   i += 1
                   current = current.next
               raise Exception("Value not found")
 
-          def insert(self, index, value):
-              ''' insert value at a specified index '''
+          def insert(self, index: int, value):
+              """
+              Insert a value at a specified index.
+
+              Args:
+                  index: the index to insert a value
+                  value: a value to append
+              """
+              i = 0
 
               # insert front
               if index == 0:
-                  self.prepend(value)
+                  new_node = Node(value)
+                  new_node.next = self.head
+                  self.head = new_node
+                  self.count += 1
                   return
 
-              i = 0
               current = self.head
               while index < i or current is not None:
+                  i += 1
                   if i == index:
                       break
                   current = current.next
-                  i += 1
 
               if index > i:
                   raise Exception("Index Out of Bounds")
               new_node = Node(value)
-
-              new_node.next = current
-              new_node.prev = current.prev
-              current.prev = new_node
-              new_node.prev.next = new_node
-
+              tmp = current.next
+              current.next = new_node
+              new_node.next = tmp
               self.count += 1
 
 
-          def prepend(self, value):
-              ''' prepend value at the beginning of the list '''
-              new_node = Node(value)
-              new_node.next = self.head
-              self.head.prev = new_node
-              self.head = new_node
-              self.count += 1
-
           def append(self, value):
-              ''' append value to the end of the list '''
+              """
+              Place a value at the end of the linked list.
 
+              Args:
+                  value: a value to append
+              """
               if self.head is None:
                   self.head = Node(value)
                   if self.count == 0:
                       self.tail = self.head
                   self.count += 1
                   return
 
               # go to the end of the list
               new_node = Node(value)
-              new_node.prev = self.tail
               self.tail.next = new_node
               self.tail = new_node
 
               self.count += 1
 
-
-          def delete(self, index):
-              ''' delete node at a specified index '''
-              if self.head is None:
-                  raise Exception("DoublyLinkedList is Empty")
-
-              i = 0
+          def delete(self, index: int):
+              """
+              Delete a node at a specified index. Raise Exception if linked
+      list is empty or if index is not found.
+
+              Args:
+                  index: index of element to be deleted
+              """
               if index == 0:
+                  if self.head is None:
+                      raise Exception("LinkedList is Empty")
                   self.head = self.head.next
-                  if self.head is not None:
-                      self.head.prev = None
                   self.count -= 1
                   return
 
+              i = 0
               current = self.head
+              prev = current
               while current is not None:
                   if index == i:
-                      current.prev.next = current.next
-                      if current.next is not None:
-                          current.next.prev = current.prev
-                      else:
-                          self.tail = current.prev
-
+                      prev.next = current.next
                       self.count -= 1
                       return
-                  current = current.next
                   i += 1
+                  prev = current
+                  current = current.next
               raise Exception("Index not found")
       ******** SSttaattiicc mmeetthhooddss ********
         def from_array(mylist=None)
-            create a linked list from an array
+            Create a linked list from an array.
+            ********** AArrggss **********
+              mmyylliisstt
+                  an array or container to conver from
+            ********** RReettuurrnnss **********
+            Linked List
             Expand source code
             @classmethod
             def from_array(cls, mylist=None):
-                ''' create a linked list from an array '''
+                """
+                Create a linked list from an array.
+
+                Args:
+                    mylist: an array or container to conver from
+
+                Returns:
+                    Linked List
+                """
+                '''  '''
                 ll = cls()
                 for value in mylist:
                     ll.append(value)
 
                 return ll
       ******** MMeetthhooddss ********
         def append(self, value)
-            append value to the end of the list
+            Place a value at the end of the linked list.
+            ********** AArrggss **********
+              vvaalluuee
+                  a value to append
             Expand source code
             def append(self, value):
-                ''' append value to the end of the list '''
+                """
+                Place a value at the end of the linked list.
 
+                Args:
+                    value: a value to append
+                """
                 if self.head is None:
                     self.head = Node(value)
                     if self.count == 0:
                         self.tail = self.head
                     self.count += 1
                     return
 
                 # go to the end of the list
                 new_node = Node(value)
-                new_node.prev = self.tail
                 self.tail.next = new_node
                 self.tail = new_node
 
                 self.count += 1
-        def delete(self, index)
-            delete node at a specified index
+        def delete(self, index: int)
+            Delete a node at a specified index. Raise Exception if linked list
+            is empty or if index is not found.
+            ********** AArrggss **********
+              iinnddeexx
+                  index of element to be deleted
             Expand source code
-            def delete(self, index):
-                ''' delete node at a specified index '''
-                if self.head is None:
-                    raise Exception("DoublyLinkedList is Empty")
-
-                i = 0
+            def delete(self, index: int):
+                """
+                Delete a node at a specified index. Raise Exception if linked
+            list is empty or if index is not found.
+
+                Args:
+                    index: index of element to be deleted
+                """
                 if index == 0:
+                    if self.head is None:
+                        raise Exception("LinkedList is Empty")
                     self.head = self.head.next
-                    if self.head is not None:
-                        self.head.prev = None
                     self.count -= 1
                     return
 
+                i = 0
                 current = self.head
+                prev = current
                 while current is not None:
                     if index == i:
-                        current.prev.next = current.next
-                        if current.next is not None:
-                            current.next.prev = current.prev
-                        else:
-                            self.tail = current.prev
-
+                        prev.next = current.next
                         self.count -= 1
                         return
-                    current = current.next
                     i += 1
+                    prev = current
+                    current = current.next
                 raise Exception("Index not found")
-        def insert(self, index, value)
-            insert value at a specified index
+        def insert(self, index: int, value)
+            Insert a value at a specified index.
+            ********** AArrggss **********
+              iinnddeexx
+                  the index to insert a value
+              vvaalluuee
+                  a value to append
             Expand source code
-            def insert(self, index, value):
-                ''' insert value at a specified index '''
+            def insert(self, index: int, value):
+                """
+                Insert a value at a specified index.
+
+                Args:
+                    index: the index to insert a value
+                    value: a value to append
+                """
+                i = 0
 
                 # insert front
                 if index == 0:
-                    self.prepend(value)
+                    new_node = Node(value)
+                    new_node.next = self.head
+                    self.head = new_node
+                    self.count += 1
                     return
 
-                i = 0
                 current = self.head
                 while index < i or current is not None:
+                    i += 1
                     if i == index:
                         break
                     current = current.next
-                    i += 1
 
                 if index > i:
                     raise Exception("Index Out of Bounds")
                 new_node = Node(value)
-
-                new_node.next = current
-                new_node.prev = current.prev
-                current.prev = new_node
-                new_node.prev.next = new_node
-
+                tmp = current.next
+                current.next = new_node
+                new_node.next = tmp
                 self.count += 1
-        def prepend(self, value)
-            prepend value at the beginning of the list
+        def print(self)
+            Print the contents of the linked list.
             Expand source code
-            def prepend(self, value):
-                ''' prepend value at the beginning of the list '''
-                new_node = Node(value)
-                new_node.next = self.head
-                self.head.prev = new_node
-                self.head = new_node
-                self.count += 1
-        def print_reverse(self)
-            Expand source code
-            def print_reverse(self):
-                current = self.tail
+            def print(self):
+                """
+                Print the contents of the linked list.
+                """
+                current = self.head
                 while current is not None:
                     print(current.value, end=" ")
-                    current = current.prev
+                    current = current.next
                 print()
-        def search(self, value)
-            return index of specified value
+        def search(self, value) ‑> int
+            Search for a value in the linked list.
+            ********** AArrggss **********
+              vvaalluuee
+                  value to search for
+            ********** RReettuurrnnss **********
+            return index of found value
             Expand source code
-            def search(self, value):
-                ''' return index of specified value '''
+            def search(self, value) -> int:
+                """
+                Search for a value in the linked list.
+
+                Args:
+                    value: value to search for
+
+                Returns:
+                    return index of found value
+                """
                 i = 0
                 current = self.head
                 while current is not None:
                     if current.value == value:
                         return i
                     i += 1
                     current = current.next
                 raise Exception("Value not found")
   class Node (value)
+      A singly linked list node implementation in Python
+      ********** AArrggss **********
+        vvaalluuee
+            the value of the node
       Expand source code
       class Node:
+          """
+          A singly linked list node implementation in Python
+          """
           def __init__(self, value):
+              """
+              Args:
+                  value: the value of the node
+              """
+              #: value of the node
               self.value = value
+              #: reference to the next node
               self.next = None
-              self.prev = None
+      ******** IInnssttaannccee vvaarriiaabblleess ********
+        var next
+            reference to the next node
+        var value
+            value of the node
 ************ IInnddeexx ************
     * ******** SSuuppeerr--mmoodduullee ********
           o _d_s_a
     * ******** _CC_ll_aa_ss_ss_ee_ss ********
-          o ****** _DD_oo_uu_bb_ll_yy_LL_ii_nn_kk_ee_dd_LL_ii_ss_tt ******
+          o ****** _LL_ii_nn_kk_ee_dd_LL_ii_ss_tt ******
                 # _a_p_p_e_n_d
                 # _d_e_l_e_t_e
                 # _f_r_o_m___a_r_r_a_y
                 # _i_n_s_e_r_t
-                # _p_r_e_p_e_n_d
-                # _p_r_i_n_t___r_e_v_e_r_s_e
+                # _p_r_i_n_t
                 # _s_e_a_r_c_h
           o ****** _NN_oo_dd_ee ******
+                # _n_e_x_t
+                # _v_a_l_u_e
 Generated by_p_d_o_c_0_._1_0_._0.
```

### Comparing `ucxdsa-2024.4.23/src/html/dsa/hashtable.html` & `ucxdsa-2024.5.9/src/html/dsa/hashtable.html`

 * *Files 26% similar despite different names*

```diff
@@ -23,67 +23,107 @@
 </header>
 <section id="section-intro">
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">class HashTable:
+    &#34;&#34;&#34; 
+    A hashtable implementation in Python
+    &#34;&#34;&#34;
     def __init__(self, capacity=20):
+        &#34;&#34;&#34;
+        Args:
+            capacity: the capacity of the hashtable
+        &#34;&#34;&#34;
         self.capacity = capacity
 
         self.array = []
         for _ in range(self.capacity):
             self.array.append([])
+
+        #: the number of items in the hashtable
         self.count = 0
         
-    def hash_function(self, key):
+    def hash_function(self, key) -&gt; int:
+        &#34;&#34;&#34; 
+        Return a hash value based on a given key. 
+
+        Args:
+            key: the key to convert to a hashvalue
+        Returns:
+        hash value modded to the hashtable capacity
+        &#34;&#34;&#34;
         charsum = sum(ord(c) * i for i, c in enumerate(key, 1))
         return charsum % self.capacity      
         
-    def key_exists(self, key):
-        &#39;&#39;&#39; returns a Boolean on whether a key exists in the hashtable or not &#39;&#39;&#39;
+    def key_exists(self, key) -&gt; bool:
+        &#34;&#34;&#34; 
+        Returns a Boolean on whether a key exists in the hashtable or not 
+
+        Args:
+            key: the key to check for in the hashtable
+        Returns:
+        Boolean of key existence
+        &#34;&#34;&#34;
         bucket = self.hash_function(key)
         if self.array[bucket] is None:
             return False
         
         for e in self.array[bucket]:
             if e[0] == key:
                 return True
         return False
 
     def set(self, key, value):
-        &#39;&#39;&#39; if key exists, replace the value 
-            otherwise, create a new key-pair
-        &#39;&#39;&#39;
+        &#34;&#34;&#34; 
+        if key exists, replace the value 
+        otherwise, create a new key-pair
+        Args:
+            key: the key to check for
+            value: the value to set or create
+        &#34;&#34;&#34;
 
         bucket = self.hash_function(key)
 
         # linear searh for key 
         for e in self.array[bucket]:
             if e[0] == key:
                 e[1] = value
                 break
         else:
             self.array[bucket].append([ key, value ])
             self.count += 1
 
     def get(self, key):
-        &#39;&#39;&#39; get corresponding value of key
-            return None if key is not found
-        &#39;&#39;&#39;
+        &#34;&#34;&#34; 
+        get corresponding value of key
+
+        Args:
+            key: the key to check for
+            value: the value to set or create
+        Returns:
+        corresponding value of key
+        None if key is not found
+        &#34;&#34;&#34;
         bucket = self.hash_function(key)
 
         for e in self.array[bucket]:
             if e[0] == key:
                 return e[1]
 
         return None
 
     def delete(self, key):
-        &#39;&#39;&#39; delete key-value pair if specified key is found &#39;&#39;&#39;
+        &#34;&#34;&#34; 
+        Delete key-value pair if specified key is found 
+
+        Args:
+            key: the key to check for
+        &#34;&#34;&#34;
         bucket = self.hash_function(key)
 
         for i in range(len(self.array[bucket])):
             kvpair = self.array[bucket][i]
             if kvpair and kvpair[0] == key:
                 del self.array[bucket][i]
                 self.count -= 1
@@ -106,73 +146,118 @@
 <h2 class="section-title" id="header-classes">Classes</h2>
 <dl>
 <dt id="dsa.hashtable.HashTable"><code class="flex name class">
 <span>class <span class="ident">HashTable</span></span>
 <span>(</span><span>capacity=20)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>A hashtable implementation in Python</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>capacity</code></strong></dt>
+<dd>the capacity of the hashtable</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">class HashTable:
+    &#34;&#34;&#34; 
+    A hashtable implementation in Python
+    &#34;&#34;&#34;
     def __init__(self, capacity=20):
+        &#34;&#34;&#34;
+        Args:
+            capacity: the capacity of the hashtable
+        &#34;&#34;&#34;
         self.capacity = capacity
 
         self.array = []
         for _ in range(self.capacity):
             self.array.append([])
+
+        #: the number of items in the hashtable
         self.count = 0
         
-    def hash_function(self, key):
+    def hash_function(self, key) -&gt; int:
+        &#34;&#34;&#34; 
+        Return a hash value based on a given key. 
+
+        Args:
+            key: the key to convert to a hashvalue
+        Returns:
+        hash value modded to the hashtable capacity
+        &#34;&#34;&#34;
         charsum = sum(ord(c) * i for i, c in enumerate(key, 1))
         return charsum % self.capacity      
         
-    def key_exists(self, key):
-        &#39;&#39;&#39; returns a Boolean on whether a key exists in the hashtable or not &#39;&#39;&#39;
+    def key_exists(self, key) -&gt; bool:
+        &#34;&#34;&#34; 
+        Returns a Boolean on whether a key exists in the hashtable or not 
+
+        Args:
+            key: the key to check for in the hashtable
+        Returns:
+        Boolean of key existence
+        &#34;&#34;&#34;
         bucket = self.hash_function(key)
         if self.array[bucket] is None:
             return False
         
         for e in self.array[bucket]:
             if e[0] == key:
                 return True
         return False
 
     def set(self, key, value):
-        &#39;&#39;&#39; if key exists, replace the value 
-            otherwise, create a new key-pair
-        &#39;&#39;&#39;
+        &#34;&#34;&#34; 
+        if key exists, replace the value 
+        otherwise, create a new key-pair
+        Args:
+            key: the key to check for
+            value: the value to set or create
+        &#34;&#34;&#34;
 
         bucket = self.hash_function(key)
 
         # linear searh for key 
         for e in self.array[bucket]:
             if e[0] == key:
                 e[1] = value
                 break
         else:
             self.array[bucket].append([ key, value ])
             self.count += 1
 
     def get(self, key):
-        &#39;&#39;&#39; get corresponding value of key
-            return None if key is not found
-        &#39;&#39;&#39;
+        &#34;&#34;&#34; 
+        get corresponding value of key
+
+        Args:
+            key: the key to check for
+            value: the value to set or create
+        Returns:
+        corresponding value of key
+        None if key is not found
+        &#34;&#34;&#34;
         bucket = self.hash_function(key)
 
         for e in self.array[bucket]:
             if e[0] == key:
                 return e[1]
 
         return None
 
     def delete(self, key):
-        &#39;&#39;&#39; delete key-value pair if specified key is found &#39;&#39;&#39;
+        &#34;&#34;&#34; 
+        Delete key-value pair if specified key is found 
+
+        Args:
+            key: the key to check for
+        &#34;&#34;&#34;
         bucket = self.hash_function(key)
 
         for i in range(len(self.array[bucket])):
             kvpair = self.array[bucket][i]
             if kvpair and kvpair[0] == key:
                 del self.array[bucket][i]
                 self.count -= 1
@@ -180,85 +265,147 @@
     
     def __repr__(self):
         s = &#34;&#34;
         for i, bucket in enumerate(self.array):
             s += f&#34;Bucket {i}: {bucket}\n&#34;
         return s</code></pre>
 </details>
+<h3>Instance variables</h3>
+<dl>
+<dt id="dsa.hashtable.HashTable.count"><code class="name">var <span class="ident">count</span></code></dt>
+<dd>
+<div class="desc"><p>the number of items in the hashtable</p></div>
+</dd>
+</dl>
 <h3>Methods</h3>
 <dl>
 <dt id="dsa.hashtable.HashTable.delete"><code class="name flex">
 <span>def <span class="ident">delete</span></span>(<span>self, key)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>delete key-value pair if specified key is found</p></div>
+<div class="desc"><p>Delete key-value pair if specified key is found </p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>key</code></strong></dt>
+<dd>the key to check for</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def delete(self, key):
-    &#39;&#39;&#39; delete key-value pair if specified key is found &#39;&#39;&#39;
+    &#34;&#34;&#34; 
+    Delete key-value pair if specified key is found 
+
+    Args:
+        key: the key to check for
+    &#34;&#34;&#34;
     bucket = self.hash_function(key)
 
     for i in range(len(self.array[bucket])):
         kvpair = self.array[bucket][i]
         if kvpair and kvpair[0] == key:
             del self.array[bucket][i]
             self.count -= 1
             break</code></pre>
 </details>
 </dd>
 <dt id="dsa.hashtable.HashTable.get"><code class="name flex">
 <span>def <span class="ident">get</span></span>(<span>self, key)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>get corresponding value of key
-return None if key is not found</p></div>
+<div class="desc"><p>get corresponding value of key</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>key</code></strong></dt>
+<dd>the key to check for</dd>
+<dt><strong><code>value</code></strong></dt>
+<dd>the value to set or create</dd>
+</dl>
+<p>Returns:
+corresponding value of key
+None if key is not found</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def get(self, key):
-    &#39;&#39;&#39; get corresponding value of key
-        return None if key is not found
-    &#39;&#39;&#39;
+    &#34;&#34;&#34; 
+    get corresponding value of key
+
+    Args:
+        key: the key to check for
+        value: the value to set or create
+    Returns:
+    corresponding value of key
+    None if key is not found
+    &#34;&#34;&#34;
     bucket = self.hash_function(key)
 
     for e in self.array[bucket]:
         if e[0] == key:
             return e[1]
 
     return None</code></pre>
 </details>
 </dd>
 <dt id="dsa.hashtable.HashTable.hash_function"><code class="name flex">
-<span>def <span class="ident">hash_function</span></span>(<span>self, key)</span>
+<span>def <span class="ident">hash_function</span></span>(<span>self, key) ‑> int</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>Return a hash value based on a given key. </p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>key</code></strong></dt>
+<dd>the key to convert to a hashvalue</dd>
+</dl>
+<p>Returns:
+hash value modded to the hashtable capacity</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def hash_function(self, key):
+<pre><code class="python">def hash_function(self, key) -&gt; int:
+    &#34;&#34;&#34; 
+    Return a hash value based on a given key. 
+
+    Args:
+        key: the key to convert to a hashvalue
+    Returns:
+    hash value modded to the hashtable capacity
+    &#34;&#34;&#34;
     charsum = sum(ord(c) * i for i, c in enumerate(key, 1))
     return charsum % self.capacity      </code></pre>
 </details>
 </dd>
 <dt id="dsa.hashtable.HashTable.key_exists"><code class="name flex">
-<span>def <span class="ident">key_exists</span></span>(<span>self, key)</span>
+<span>def <span class="ident">key_exists</span></span>(<span>self, key) ‑> bool</span>
 </code></dt>
 <dd>
-<div class="desc"><p>returns a Boolean on whether a key exists in the hashtable or not</p></div>
+<div class="desc"><p>Returns a Boolean on whether a key exists in the hashtable or not </p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>key</code></strong></dt>
+<dd>the key to check for in the hashtable</dd>
+</dl>
+<p>Returns:
+Boolean of key existence</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def key_exists(self, key):
-    &#39;&#39;&#39; returns a Boolean on whether a key exists in the hashtable or not &#39;&#39;&#39;
+<pre><code class="python">def key_exists(self, key) -&gt; bool:
+    &#34;&#34;&#34; 
+    Returns a Boolean on whether a key exists in the hashtable or not 
+
+    Args:
+        key: the key to check for in the hashtable
+    Returns:
+    Boolean of key existence
+    &#34;&#34;&#34;
     bucket = self.hash_function(key)
     if self.array[bucket] is None:
         return False
     
     for e in self.array[bucket]:
         if e[0] == key:
             return True
@@ -266,23 +413,34 @@
 </details>
 </dd>
 <dt id="dsa.hashtable.HashTable.set"><code class="name flex">
 <span>def <span class="ident">set</span></span>(<span>self, key, value)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>if key exists, replace the value
-otherwise, create a new key-pair</p></div>
+otherwise, create a new key-pair</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>key</code></strong></dt>
+<dd>the key to check for</dd>
+<dt><strong><code>value</code></strong></dt>
+<dd>the value to set or create</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def set(self, key, value):
-    &#39;&#39;&#39; if key exists, replace the value 
-        otherwise, create a new key-pair
-    &#39;&#39;&#39;
+    &#34;&#34;&#34; 
+    if key exists, replace the value 
+    otherwise, create a new key-pair
+    Args:
+        key: the key to check for
+        value: the value to set or create
+    &#34;&#34;&#34;
 
     bucket = self.hash_function(key)
 
     # linear searh for key 
     for e in self.array[bucket]:
         if e[0] == key:
             e[1] = value
@@ -308,15 +466,16 @@
 <li><code><a title="dsa" href="index.html">dsa</a></code></li>
 </ul>
 </li>
 <li><h3><a href="#header-classes">Classes</a></h3>
 <ul>
 <li>
 <h4><code><a title="dsa.hashtable.HashTable" href="#dsa.hashtable.HashTable">HashTable</a></code></h4>
-<ul class="">
+<ul class="two-column">
+<li><code><a title="dsa.hashtable.HashTable.count" href="#dsa.hashtable.HashTable.count">count</a></code></li>
 <li><code><a title="dsa.hashtable.HashTable.delete" href="#dsa.hashtable.HashTable.delete">delete</a></code></li>
 <li><code><a title="dsa.hashtable.HashTable.get" href="#dsa.hashtable.HashTable.get">get</a></code></li>
 <li><code><a title="dsa.hashtable.HashTable.hash_function" href="#dsa.hashtable.HashTable.hash_function">hash_function</a></code></li>
 <li><code><a title="dsa.hashtable.HashTable.key_exists" href="#dsa.hashtable.HashTable.key_exists">key_exists</a></code></li>
 <li><code><a title="dsa.hashtable.HashTable.set" href="#dsa.hashtable.HashTable.set">set</a></code></li>
 </ul>
 </li>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,64 +1,103 @@
 ************ MMoodduullee ddssaa..hhaasshhttaabbllee ************
 Expand source code
 class HashTable:
+    """
+    A hashtable implementation in Python
+    """
     def __init__(self, capacity=20):
+        """
+        Args:
+            capacity: the capacity of the hashtable
+        """
         self.capacity = capacity
 
         self.array = []
         for _ in range(self.capacity):
             self.array.append([])
+
+        #: the number of items in the hashtable
         self.count = 0
 
-    def hash_function(self, key):
+    def hash_function(self, key) -> int:
+        """
+        Return a hash value based on a given key.
+
+        Args:
+            key: the key to convert to a hashvalue
+        Returns:
+        hash value modded to the hashtable capacity
+        """
         charsum = sum(ord(c) * i for i, c in enumerate(key, 1))
         return charsum % self.capacity
 
-    def key_exists(self, key):
-        ''' returns a Boolean on whether a key exists in the hashtable or not
-'''
+    def key_exists(self, key) -> bool:
+        """
+        Returns a Boolean on whether a key exists in the hashtable or not
+
+        Args:
+            key: the key to check for in the hashtable
+        Returns:
+        Boolean of key existence
+        """
         bucket = self.hash_function(key)
         if self.array[bucket] is None:
             return False
 
         for e in self.array[bucket]:
             if e[0] == key:
                 return True
         return False
 
     def set(self, key, value):
-        ''' if key exists, replace the value
-            otherwise, create a new key-pair
-        '''
+        """
+        if key exists, replace the value
+        otherwise, create a new key-pair
+        Args:
+            key: the key to check for
+            value: the value to set or create
+        """
 
         bucket = self.hash_function(key)
 
         # linear searh for key
         for e in self.array[bucket]:
             if e[0] == key:
                 e[1] = value
                 break
         else:
             self.array[bucket].append([ key, value ])
             self.count += 1
 
     def get(self, key):
-        ''' get corresponding value of key
-            return None if key is not found
-        '''
+        """
+        get corresponding value of key
+
+        Args:
+            key: the key to check for
+            value: the value to set or create
+        Returns:
+        corresponding value of key
+        None if key is not found
+        """
         bucket = self.hash_function(key)
 
         for e in self.array[bucket]:
             if e[0] == key:
                 return e[1]
 
         return None
 
     def delete(self, key):
-        ''' delete key-value pair if specified key is found '''
+        """
+        Delete key-value pair if specified key is found
+
+        Args:
+            key: the key to check for
+        """
         bucket = self.hash_function(key)
 
         for i in range(len(self.array[bucket])):
             kvpair = self.array[bucket][i]
             if kvpair and kvpair[0] == key:
                 del self.array[bucket][i]
                 self.count -= 1
@@ -67,138 +106,239 @@
     def __repr__(self):
         s = ""
         for i, bucket in enumerate(self.array):
             s += f"Bucket {i}: {bucket}\n"
         return s
 ********** CCllaasssseess **********
   class HashTable (capacity=20)
+      A hashtable implementation in Python
+      ********** AArrggss **********
+        ccaappaacciittyy
+            the capacity of the hashtable
       Expand source code
       class HashTable:
+          """
+          A hashtable implementation in Python
+          """
           def __init__(self, capacity=20):
+              """
+              Args:
+                  capacity: the capacity of the hashtable
+              """
               self.capacity = capacity
 
               self.array = []
               for _ in range(self.capacity):
                   self.array.append([])
+
+              #: the number of items in the hashtable
               self.count = 0
 
-          def hash_function(self, key):
+          def hash_function(self, key) -> int:
+              """
+              Return a hash value based on a given key.
+
+              Args:
+                  key: the key to convert to a hashvalue
+              Returns:
+              hash value modded to the hashtable capacity
+              """
               charsum = sum(ord(c) * i for i, c in enumerate(key, 1))
               return charsum % self.capacity
 
-          def key_exists(self, key):
-              ''' returns a Boolean on whether a key exists in the hashtable or
-      not '''
+          def key_exists(self, key) -> bool:
+              """
+              Returns a Boolean on whether a key exists in the hashtable or not
+
+
+              Args:
+                  key: the key to check for in the hashtable
+              Returns:
+              Boolean of key existence
+              """
               bucket = self.hash_function(key)
               if self.array[bucket] is None:
                   return False
 
               for e in self.array[bucket]:
                   if e[0] == key:
                       return True
               return False
 
           def set(self, key, value):
-              ''' if key exists, replace the value
-                  otherwise, create a new key-pair
-              '''
+              """
+              if key exists, replace the value
+              otherwise, create a new key-pair
+              Args:
+                  key: the key to check for
+                  value: the value to set or create
+              """
 
               bucket = self.hash_function(key)
 
               # linear searh for key
               for e in self.array[bucket]:
                   if e[0] == key:
                       e[1] = value
                       break
               else:
                   self.array[bucket].append([ key, value ])
                   self.count += 1
 
           def get(self, key):
-              ''' get corresponding value of key
-                  return None if key is not found
-              '''
+              """
+              get corresponding value of key
+
+              Args:
+                  key: the key to check for
+                  value: the value to set or create
+              Returns:
+              corresponding value of key
+              None if key is not found
+              """
               bucket = self.hash_function(key)
 
               for e in self.array[bucket]:
                   if e[0] == key:
                       return e[1]
 
               return None
 
           def delete(self, key):
-              ''' delete key-value pair if specified key is found '''
+              """
+              Delete key-value pair if specified key is found
+
+              Args:
+                  key: the key to check for
+              """
               bucket = self.hash_function(key)
 
               for i in range(len(self.array[bucket])):
                   kvpair = self.array[bucket][i]
                   if kvpair and kvpair[0] == key:
                       del self.array[bucket][i]
                       self.count -= 1
                       break
 
           def __repr__(self):
               s = ""
               for i, bucket in enumerate(self.array):
                   s += f"Bucket {i}: {bucket}\n"
               return s
+      ******** IInnssttaannccee vvaarriiaabblleess ********
+        var count
+            the number of items in the hashtable
       ******** MMeetthhooddss ********
         def delete(self, key)
-            delete key-value pair if specified key is found
+            Delete key-value pair if specified key is found
+            ********** AArrggss **********
+              kkeeyy
+                  the key to check for
             Expand source code
             def delete(self, key):
-                ''' delete key-value pair if specified key is found '''
+                """
+                Delete key-value pair if specified key is found
+
+                Args:
+                    key: the key to check for
+                """
                 bucket = self.hash_function(key)
 
                 for i in range(len(self.array[bucket])):
                     kvpair = self.array[bucket][i]
                     if kvpair and kvpair[0] == key:
                         del self.array[bucket][i]
                         self.count -= 1
                         break
         def get(self, key)
-            get corresponding value of key return None if key is not found
+            get corresponding value of key
+            ********** AArrggss **********
+              kkeeyy
+                  the key to check for
+              vvaalluuee
+                  the value to set or create
+            Returns: corresponding value of key None if key is not found
             Expand source code
             def get(self, key):
-                ''' get corresponding value of key
-                    return None if key is not found
-                '''
+                """
+                get corresponding value of key
+
+                Args:
+                    key: the key to check for
+                    value: the value to set or create
+                Returns:
+                corresponding value of key
+                None if key is not found
+                """
                 bucket = self.hash_function(key)
 
                 for e in self.array[bucket]:
                     if e[0] == key:
                         return e[1]
 
                 return None
-        def hash_function(self, key)
+        def hash_function(self, key) ‑> int
+            Return a hash value based on a given key.
+            ********** AArrggss **********
+              kkeeyy
+                  the key to convert to a hashvalue
+            Returns: hash value modded to the hashtable capacity
             Expand source code
-            def hash_function(self, key):
+            def hash_function(self, key) -> int:
+                """
+                Return a hash value based on a given key.
+
+                Args:
+                    key: the key to convert to a hashvalue
+                Returns:
+                hash value modded to the hashtable capacity
+                """
                 charsum = sum(ord(c) * i for i, c in enumerate(key, 1))
                 return charsum % self.capacity
-        def key_exists(self, key)
-            returns a Boolean on whether a key exists in the hashtable or not
+        def key_exists(self, key) ‑> bool
+            Returns a Boolean on whether a key exists in the hashtable or not
+            ********** AArrggss **********
+              kkeeyy
+                  the key to check for in the hashtable
+            Returns: Boolean of key existence
             Expand source code
-            def key_exists(self, key):
-                ''' returns a Boolean on whether a key exists in the hashtable
-            or not '''
+            def key_exists(self, key) -> bool:
+                """
+                Returns a Boolean on whether a key exists in the hashtable or
+            not
+
+                Args:
+                    key: the key to check for in the hashtable
+                Returns:
+                Boolean of key existence
+                """
                 bucket = self.hash_function(key)
                 if self.array[bucket] is None:
                     return False
 
                 for e in self.array[bucket]:
                     if e[0] == key:
                         return True
                 return False
         def set(self, key, value)
             if key exists, replace the value otherwise, create a new key-pair
+            ********** AArrggss **********
+              kkeeyy
+                  the key to check for
+              vvaalluuee
+                  the value to set or create
             Expand source code
             def set(self, key, value):
-                ''' if key exists, replace the value
-                    otherwise, create a new key-pair
-                '''
+                """
+                if key exists, replace the value
+                otherwise, create a new key-pair
+                Args:
+                    key: the key to check for
+                    value: the value to set or create
+                """
 
                 bucket = self.hash_function(key)
 
                 # linear searh for key
                 for e in self.array[bucket]:
                     if e[0] == key:
                         e[1] = value
@@ -207,13 +347,14 @@
                     self.array[bucket].append([ key, value ])
                     self.count += 1
 ************ IInnddeexx ************
     * ******** SSuuppeerr--mmoodduullee ********
           o _d_s_a
     * ******** _CC_ll_aa_ss_ss_ee_ss ********
           o ****** _HH_aa_ss_hh_TT_aa_bb_ll_ee ******
+                # _c_o_u_n_t
                 # _d_e_l_e_t_e
                 # _g_e_t
                 # _h_a_s_h___f_u_n_c_t_i_o_n
                 # _k_e_y___e_x_i_s_t_s
                 # _s_e_t
 Generated by_p_d_o_c_0_._1_0_._0.
```

### Comparing `ucxdsa-2024.4.23/src/html/dsa/heap.html` & `ucxdsa-2024.5.9/src/html/dsa/queue.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,467 +1,510 @@
 <!doctype html>
 <html lang="en">
 <head>
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
 <meta name="generator" content="pdoc 0.10.0" />
-<title>dsa.heap API documentation</title>
+<title>dsa.queue API documentation</title>
 <meta name="description" content="" />
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
 <link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
 <style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
 <style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
 <style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
 <script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
 <script>window.addEventListener('DOMContentLoaded', () => hljs.initHighlighting())</script>
 </head>
 <body>
 <main>
 <article id="content">
 <header>
-<h1 class="title">Module <code>dsa.heap</code></h1>
+<h1 class="title">Module <code>dsa.queue</code></h1>
 </header>
 <section id="section-intro">
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">class Heap:
-    def __init__(self):
-        self.array = []
-    
-    def root(self):
-        if self.count() == 0:
-            return None
-
-        return self.array[0]
-    
-    def last(self):
-        if self.count() == 0:
-            return None
-
-        return self.array[-1] 
-    
-    def left_index(self, index):
-        return (index * 2) + 1
-
-    def right_index(self, index):
-        return (index * 2) + 2
-
-    def parent_index(self, index):
-        return (index - 1) // 2
-    
-    def has_left(self, index):
-        return self.left_index(index) &lt; self.count()
-    
-    def has_right(self, index):
-        return self.right_index(index) &lt; self.count()
-
-    def has_parent(self, index):
-        return self.parent_index(index) &gt;= 0
-    
-    def insert(self, value):
-        self.array.append(value)
+<pre><code class="python">class Queue:
+    &#34;&#34;&#34; 
+    A static queue implementation in Python
+    &#34;&#34;&#34;
+    def __init__(self, capacity=10):
+        &#34;&#34;&#34; 
+        Args:
+            capacity: the initial size of the stack (defaults to 10)
+        &#34;&#34;&#34;
+        self._array = [None] * capacity
+        self._front = 0
+        #: number of elements in queue
+        self.count = 0
+    
+    def enqueue(self, element):
+        &#34;&#34;&#34;
+        Enqueue an element into the queue. Raise Exception when trying to enqueue more elements than the capacity.
+
+        Args:
+            element: the element to enqueue
+        &#34;&#34;&#34;
+        if self.count &gt;= len(self._array):
+            raise Exception(&#34;Capacity Reached&#34;)
+
+        index = (self._front + self.count) % len(self._array)
+        self._array[index] = element
+        self.count += 1
         
-        start_index = self.count() - 1
-        self.heapify_up(start_index)
-    
-    def heapify_up(self, index):
-        parent_index = self.parent_index(index)
-        while self.has_parent(index) and self.array[index] &gt; self.array[parent_index]:
-            self.array[index], self.array[parent_index] = self.array[parent_index], self.array[index]
-            index = parent_index
-            parent_index = self.parent_index(index)
+    def dequeue(self):
+        &#34;&#34;&#34;
+        Dequeue an element from the queue. Raise Exception when there are no elements to dequeue.
+
+        Returns:
+            the from element in the queue
+        &#34;&#34;&#34;
+        if self.is_empty():
+            raise Exception(&#34;Empty Queue&#34;)
+
+        element = self._array[self._front]
+        self._front += 1
+        if self._front &gt;= len(self._array):
+            self._front = 0
+        self.count -= 1
+
+        return element
+    
+    def peek(self):
+        &#34;&#34;&#34;
+        Return the element in front of the queue. Raise Exception if queue is empty.
+        &#34;&#34;&#34;
+        if self.is_empty():
+            raise Exception(&#34;Empty Queue&#34;)
 
-    def pop(self):
-        root_value = self.root()
-        
-        # start at root node
-        start_index = 0
-        if self.count() == 1:
-            self.array.pop()
-        else:
-            self.array[start_index] = self.array.pop()
-        
-        self.heapify_down(start_index)
-        return root_value
-        
-    def heapify_down(self, index):
-        while self.has_left(index):
-            higher_index = self.left_index(index)
-
-            right_index = self.right_index(index)
-            if self.has_right(index) and self.array[right_index] &gt; self.array[higher_index]:
-                higher_index = right_index
-            
-            if self.array[index] &gt; self.array[higher_index]:
-                break
-            else:
-                self.array[index], self.array[higher_index] = self.array[higher_index], self.array[index]
-                
-            index = higher_index
-    
-    def count(self):
-        return len(self.array)
-    
-    def is_empty(self):
-        return self.count() == 0
+        return self._array[self._front]
 
-    def print(self):
-        node_count = 1
-        for i in range(self.count()):
-            if i + 1 &gt;= node_count:
-                print()
-                node_count *= 2
-            print(self.array[i], end=&#34; &#34;)</code></pre>
+    def is_empty(self):
+        &#34;&#34;&#34;
+        Return a Boolean on whether the stack is empty or not.
+        &#34;&#34;&#34;
+        return self.count == 0
+    
+    def capacity(self):
+        &#34;&#34;&#34;
+        Return the capacity of the queue.
+        &#34;&#34;&#34;
+        return len(self._array)
+
+    def __repr__(self):
+        arr = []
+        for i in range(self.count):
+            index = (i + self._front) % len(self._array)
+            arr.append(str(self._array[index]))
+        arrstr = &#34;, &#34;.join(arr)
+        return f&#34;[{arrstr}] Front: {self._front} count: {self.count} Capacity: {self.capacity()}&#34;
+    
+
+# shrink not implemented
+class DynamicQueue(Queue):
+    &#34;&#34;&#34; 
+    A dynamic queue implementation in Python
+    &#34;&#34;&#34;
+    def __init__(self, capacity=10):
+        super().__init__(capacity)
+    
+    def grow(self):
+        &#34;&#34;&#34; 
+        double the capacity of the current array 
+        &#34;&#34;&#34;
+        new_array = [ None ] * len(self._array) * 2
+        
+        # copy elements
+        for i in range(self.count):
+            new_array[i] = self._array[i + self._front]
+        self._front = 0
+        self._array = new_array
+
+    def check_capacity(self):
+        &#34;&#34;&#34; 
+        if count &gt;= capacity, grow the array
+        &#34;&#34;&#34;
+        if self._front + self.count &gt;= len(self._array):
+            self.grow()
+
+    def enqueue(self, element):
+        &#34;&#34;&#34;
+        Enqueue an element into the queue. Increae capacity if count is greater than the capacity.
+
+        Args:
+            element: the element to enqueue
+        &#34;&#34;&#34;
+        self.check_capacity()
+        index = self._front + self.count
+        self._array[index] = element
+        self.count += 1</code></pre>
 </details>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
 <h2 class="section-title" id="header-classes">Classes</h2>
 <dl>
-<dt id="dsa.heap.Heap"><code class="flex name class">
-<span>class <span class="ident">Heap</span></span>
+<dt id="dsa.queue.DynamicQueue"><code class="flex name class">
+<span>class <span class="ident">DynamicQueue</span></span>
+<span>(</span><span>capacity=10)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>A dynamic queue implementation in Python</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>capacity</code></strong></dt>
+<dd>the initial size of the stack (defaults to 10)</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">class Heap:
-    def __init__(self):
-        self.array = []
-    
-    def root(self):
-        if self.count() == 0:
-            return None
-
-        return self.array[0]
-    
-    def last(self):
-        if self.count() == 0:
-            return None
-
-        return self.array[-1] 
-    
-    def left_index(self, index):
-        return (index * 2) + 1
-
-    def right_index(self, index):
-        return (index * 2) + 2
-
-    def parent_index(self, index):
-        return (index - 1) // 2
-    
-    def has_left(self, index):
-        return self.left_index(index) &lt; self.count()
-    
-    def has_right(self, index):
-        return self.right_index(index) &lt; self.count()
-
-    def has_parent(self, index):
-        return self.parent_index(index) &gt;= 0
-    
-    def insert(self, value):
-        self.array.append(value)
-        
-        start_index = self.count() - 1
-        self.heapify_up(start_index)
+<pre><code class="python">class DynamicQueue(Queue):
+    &#34;&#34;&#34; 
+    A dynamic queue implementation in Python
+    &#34;&#34;&#34;
+    def __init__(self, capacity=10):
+        super().__init__(capacity)
     
-    def heapify_up(self, index):
-        parent_index = self.parent_index(index)
-        while self.has_parent(index) and self.array[index] &gt; self.array[parent_index]:
-            self.array[index], self.array[parent_index] = self.array[parent_index], self.array[index]
-            index = parent_index
-            parent_index = self.parent_index(index)
-
-    def pop(self):
-        root_value = self.root()
+    def grow(self):
+        &#34;&#34;&#34; 
+        double the capacity of the current array 
+        &#34;&#34;&#34;
+        new_array = [ None ] * len(self._array) * 2
         
-        # start at root node
-        start_index = 0
-        if self.count() == 1:
-            self.array.pop()
-        else:
-            self.array[start_index] = self.array.pop()
-        
-        self.heapify_down(start_index)
-        return root_value
-        
-    def heapify_down(self, index):
-        while self.has_left(index):
-            higher_index = self.left_index(index)
-
-            right_index = self.right_index(index)
-            if self.has_right(index) and self.array[right_index] &gt; self.array[higher_index]:
-                higher_index = right_index
-            
-            if self.array[index] &gt; self.array[higher_index]:
-                break
-            else:
-                self.array[index], self.array[higher_index] = self.array[higher_index], self.array[index]
-                
-            index = higher_index
-    
-    def count(self):
-        return len(self.array)
-    
-    def is_empty(self):
-        return self.count() == 0
-
-    def print(self):
-        node_count = 1
-        for i in range(self.count()):
-            if i + 1 &gt;= node_count:
-                print()
-                node_count *= 2
-            print(self.array[i], end=&#34; &#34;)</code></pre>
-</details>
+        # copy elements
+        for i in range(self.count):
+            new_array[i] = self._array[i + self._front]
+        self._front = 0
+        self._array = new_array
+
+    def check_capacity(self):
+        &#34;&#34;&#34; 
+        if count &gt;= capacity, grow the array
+        &#34;&#34;&#34;
+        if self._front + self.count &gt;= len(self._array):
+            self.grow()
+
+    def enqueue(self, element):
+        &#34;&#34;&#34;
+        Enqueue an element into the queue. Increae capacity if count is greater than the capacity.
+
+        Args:
+            element: the element to enqueue
+        &#34;&#34;&#34;
+        self.check_capacity()
+        index = self._front + self.count
+        self._array[index] = element
+        self.count += 1</code></pre>
+</details>
+<h3>Ancestors</h3>
+<ul class="hlist">
+<li><a title="dsa.queue.Queue" href="#dsa.queue.Queue">Queue</a></li>
+</ul>
 <h3>Methods</h3>
 <dl>
-<dt id="dsa.heap.Heap.count"><code class="name flex">
-<span>def <span class="ident">count</span></span>(<span>self)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def count(self):
-    return len(self.array)</code></pre>
-</details>
-</dd>
-<dt id="dsa.heap.Heap.has_left"><code class="name flex">
-<span>def <span class="ident">has_left</span></span>(<span>self, index)</span>
+<dt id="dsa.queue.DynamicQueue.check_capacity"><code class="name flex">
+<span>def <span class="ident">check_capacity</span></span>(<span>self)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>if count &gt;= capacity, grow the array</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def has_left(self, index):
-    return self.left_index(index) &lt; self.count()</code></pre>
+<pre><code class="python">def check_capacity(self):
+    &#34;&#34;&#34; 
+    if count &gt;= capacity, grow the array
+    &#34;&#34;&#34;
+    if self._front + self.count &gt;= len(self._array):
+        self.grow()</code></pre>
 </details>
 </dd>
-<dt id="dsa.heap.Heap.has_parent"><code class="name flex">
-<span>def <span class="ident">has_parent</span></span>(<span>self, index)</span>
+<dt id="dsa.queue.DynamicQueue.enqueue"><code class="name flex">
+<span>def <span class="ident">enqueue</span></span>(<span>self, element)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def has_parent(self, index):
-    return self.parent_index(index) &gt;= 0</code></pre>
-</details>
-</dd>
-<dt id="dsa.heap.Heap.has_right"><code class="name flex">
-<span>def <span class="ident">has_right</span></span>(<span>self, index)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def has_right(self, index):
-    return self.right_index(index) &lt; self.count()</code></pre>
-</details>
-</dd>
-<dt id="dsa.heap.Heap.heapify_down"><code class="name flex">
-<span>def <span class="ident">heapify_down</span></span>(<span>self, index)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
+<div class="desc"><p>Enqueue an element into the queue. Increae capacity if count is greater than the capacity.</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>element</code></strong></dt>
+<dd>the element to enqueue</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def heapify_down(self, index):
-    while self.has_left(index):
-        higher_index = self.left_index(index)
+<pre><code class="python">def enqueue(self, element):
+    &#34;&#34;&#34;
+    Enqueue an element into the queue. Increae capacity if count is greater than the capacity.
 
-        right_index = self.right_index(index)
-        if self.has_right(index) and self.array[right_index] &gt; self.array[higher_index]:
-            higher_index = right_index
-        
-        if self.array[index] &gt; self.array[higher_index]:
-            break
-        else:
-            self.array[index], self.array[higher_index] = self.array[higher_index], self.array[index]
-            
-        index = higher_index</code></pre>
-</details>
-</dd>
-<dt id="dsa.heap.Heap.heapify_up"><code class="name flex">
-<span>def <span class="ident">heapify_up</span></span>(<span>self, index)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def heapify_up(self, index):
-    parent_index = self.parent_index(index)
-    while self.has_parent(index) and self.array[index] &gt; self.array[parent_index]:
-        self.array[index], self.array[parent_index] = self.array[parent_index], self.array[index]
-        index = parent_index
-        parent_index = self.parent_index(index)</code></pre>
+    Args:
+        element: the element to enqueue
+    &#34;&#34;&#34;
+    self.check_capacity()
+    index = self._front + self.count
+    self._array[index] = element
+    self.count += 1</code></pre>
 </details>
 </dd>
-<dt id="dsa.heap.Heap.insert"><code class="name flex">
-<span>def <span class="ident">insert</span></span>(<span>self, value)</span>
+<dt id="dsa.queue.DynamicQueue.grow"><code class="name flex">
+<span>def <span class="ident">grow</span></span>(<span>self)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>double the capacity of the current array</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def insert(self, value):
-    self.array.append(value)
+<pre><code class="python">def grow(self):
+    &#34;&#34;&#34; 
+    double the capacity of the current array 
+    &#34;&#34;&#34;
+    new_array = [ None ] * len(self._array) * 2
     
-    start_index = self.count() - 1
-    self.heapify_up(start_index)</code></pre>
+    # copy elements
+    for i in range(self.count):
+        new_array[i] = self._array[i + self._front]
+    self._front = 0
+    self._array = new_array</code></pre>
 </details>
 </dd>
-<dt id="dsa.heap.Heap.is_empty"><code class="name flex">
-<span>def <span class="ident">is_empty</span></span>(<span>self)</span>
-</code></dt>
-<dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def is_empty(self):
-    return self.count() == 0</code></pre>
-</details>
+</dl>
+<h3>Inherited members</h3>
+<ul class="hlist">
+<li><code><b><a title="dsa.queue.Queue" href="#dsa.queue.Queue">Queue</a></b></code>:
+<ul class="hlist">
+<li><code><a title="dsa.queue.Queue.capacity" href="#dsa.queue.Queue.capacity">capacity</a></code></li>
+<li><code><a title="dsa.queue.Queue.count" href="#dsa.queue.Queue.count">count</a></code></li>
+<li><code><a title="dsa.queue.Queue.dequeue" href="#dsa.queue.Queue.dequeue">dequeue</a></code></li>
+<li><code><a title="dsa.queue.Queue.is_empty" href="#dsa.queue.Queue.is_empty">is_empty</a></code></li>
+<li><code><a title="dsa.queue.Queue.peek" href="#dsa.queue.Queue.peek">peek</a></code></li>
+</ul>
+</li>
+</ul>
 </dd>
-<dt id="dsa.heap.Heap.last"><code class="name flex">
-<span>def <span class="ident">last</span></span>(<span>self)</span>
+<dt id="dsa.queue.Queue"><code class="flex name class">
+<span>class <span class="ident">Queue</span></span>
+<span>(</span><span>capacity=10)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>A static queue implementation in Python</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>capacity</code></strong></dt>
+<dd>the initial size of the stack (defaults to 10)</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def last(self):
-    if self.count() == 0:
-        return None
+<pre><code class="python">class Queue:
+    &#34;&#34;&#34; 
+    A static queue implementation in Python
+    &#34;&#34;&#34;
+    def __init__(self, capacity=10):
+        &#34;&#34;&#34; 
+        Args:
+            capacity: the initial size of the stack (defaults to 10)
+        &#34;&#34;&#34;
+        self._array = [None] * capacity
+        self._front = 0
+        #: number of elements in queue
+        self.count = 0
+    
+    def enqueue(self, element):
+        &#34;&#34;&#34;
+        Enqueue an element into the queue. Raise Exception when trying to enqueue more elements than the capacity.
+
+        Args:
+            element: the element to enqueue
+        &#34;&#34;&#34;
+        if self.count &gt;= len(self._array):
+            raise Exception(&#34;Capacity Reached&#34;)
+
+        index = (self._front + self.count) % len(self._array)
+        self._array[index] = element
+        self.count += 1
+        
+    def dequeue(self):
+        &#34;&#34;&#34;
+        Dequeue an element from the queue. Raise Exception when there are no elements to dequeue.
+
+        Returns:
+            the from element in the queue
+        &#34;&#34;&#34;
+        if self.is_empty():
+            raise Exception(&#34;Empty Queue&#34;)
+
+        element = self._array[self._front]
+        self._front += 1
+        if self._front &gt;= len(self._array):
+            self._front = 0
+        self.count -= 1
+
+        return element
+    
+    def peek(self):
+        &#34;&#34;&#34;
+        Return the element in front of the queue. Raise Exception if queue is empty.
+        &#34;&#34;&#34;
+        if self.is_empty():
+            raise Exception(&#34;Empty Queue&#34;)
 
-    return self.array[-1] </code></pre>
-</details>
-</dd>
-<dt id="dsa.heap.Heap.left_index"><code class="name flex">
-<span>def <span class="ident">left_index</span></span>(<span>self, index)</span>
-</code></dt>
+        return self._array[self._front]
+
+    def is_empty(self):
+        &#34;&#34;&#34;
+        Return a Boolean on whether the stack is empty or not.
+        &#34;&#34;&#34;
+        return self.count == 0
+    
+    def capacity(self):
+        &#34;&#34;&#34;
+        Return the capacity of the queue.
+        &#34;&#34;&#34;
+        return len(self._array)
+
+    def __repr__(self):
+        arr = []
+        for i in range(self.count):
+            index = (i + self._front) % len(self._array)
+            arr.append(str(self._array[index]))
+        arrstr = &#34;, &#34;.join(arr)
+        return f&#34;[{arrstr}] Front: {self._front} count: {self.count} Capacity: {self.capacity()}&#34;</code></pre>
+</details>
+<h3>Subclasses</h3>
+<ul class="hlist">
+<li><a title="dsa.queue.DynamicQueue" href="#dsa.queue.DynamicQueue">DynamicQueue</a></li>
+</ul>
+<h3>Instance variables</h3>
+<dl>
+<dt id="dsa.queue.Queue.count"><code class="name">var <span class="ident">count</span></code></dt>
 <dd>
-<div class="desc"></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def left_index(self, index):
-    return (index * 2) + 1</code></pre>
-</details>
+<div class="desc"><p>number of elements in queue</p></div>
 </dd>
-<dt id="dsa.heap.Heap.parent_index"><code class="name flex">
-<span>def <span class="ident">parent_index</span></span>(<span>self, index)</span>
+</dl>
+<h3>Methods</h3>
+<dl>
+<dt id="dsa.queue.Queue.capacity"><code class="name flex">
+<span>def <span class="ident">capacity</span></span>(<span>self)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>Return the capacity of the queue.</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def parent_index(self, index):
-    return (index - 1) // 2</code></pre>
+<pre><code class="python">def capacity(self):
+    &#34;&#34;&#34;
+    Return the capacity of the queue.
+    &#34;&#34;&#34;
+    return len(self._array)</code></pre>
 </details>
 </dd>
-<dt id="dsa.heap.Heap.pop"><code class="name flex">
-<span>def <span class="ident">pop</span></span>(<span>self)</span>
+<dt id="dsa.queue.Queue.dequeue"><code class="name flex">
+<span>def <span class="ident">dequeue</span></span>(<span>self)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>Dequeue an element from the queue. Raise Exception when there are no elements to dequeue.</p>
+<h2 id="returns">Returns</h2>
+<p>the from element in the queue</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def pop(self):
-    root_value = self.root()
-    
-    # start at root node
-    start_index = 0
-    if self.count() == 1:
-        self.array.pop()
-    else:
-        self.array[start_index] = self.array.pop()
-    
-    self.heapify_down(start_index)
-    return root_value</code></pre>
+<pre><code class="python">def dequeue(self):
+    &#34;&#34;&#34;
+    Dequeue an element from the queue. Raise Exception when there are no elements to dequeue.
+
+    Returns:
+        the from element in the queue
+    &#34;&#34;&#34;
+    if self.is_empty():
+        raise Exception(&#34;Empty Queue&#34;)
+
+    element = self._array[self._front]
+    self._front += 1
+    if self._front &gt;= len(self._array):
+        self._front = 0
+    self.count -= 1
+
+    return element</code></pre>
 </details>
 </dd>
-<dt id="dsa.heap.Heap.print"><code class="name flex">
-<span>def <span class="ident">print</span></span>(<span>self)</span>
+<dt id="dsa.queue.Queue.enqueue"><code class="name flex">
+<span>def <span class="ident">enqueue</span></span>(<span>self, element)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>Enqueue an element into the queue. Raise Exception when trying to enqueue more elements than the capacity.</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>element</code></strong></dt>
+<dd>the element to enqueue</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def print(self):
-    node_count = 1
-    for i in range(self.count()):
-        if i + 1 &gt;= node_count:
-            print()
-            node_count *= 2
-        print(self.array[i], end=&#34; &#34;)</code></pre>
+<pre><code class="python">def enqueue(self, element):
+    &#34;&#34;&#34;
+    Enqueue an element into the queue. Raise Exception when trying to enqueue more elements than the capacity.
+
+    Args:
+        element: the element to enqueue
+    &#34;&#34;&#34;
+    if self.count &gt;= len(self._array):
+        raise Exception(&#34;Capacity Reached&#34;)
+
+    index = (self._front + self.count) % len(self._array)
+    self._array[index] = element
+    self.count += 1</code></pre>
 </details>
 </dd>
-<dt id="dsa.heap.Heap.right_index"><code class="name flex">
-<span>def <span class="ident">right_index</span></span>(<span>self, index)</span>
+<dt id="dsa.queue.Queue.is_empty"><code class="name flex">
+<span>def <span class="ident">is_empty</span></span>(<span>self)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>Return a Boolean on whether the stack is empty or not.</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def right_index(self, index):
-    return (index * 2) + 2</code></pre>
+<pre><code class="python">def is_empty(self):
+    &#34;&#34;&#34;
+    Return a Boolean on whether the stack is empty or not.
+    &#34;&#34;&#34;
+    return self.count == 0</code></pre>
 </details>
 </dd>
-<dt id="dsa.heap.Heap.root"><code class="name flex">
-<span>def <span class="ident">root</span></span>(<span>self)</span>
+<dt id="dsa.queue.Queue.peek"><code class="name flex">
+<span>def <span class="ident">peek</span></span>(<span>self)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>Return the element in front of the queue. Raise Exception if queue is empty.</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def root(self):
-    if self.count() == 0:
-        return None
+<pre><code class="python">def peek(self):
+    &#34;&#34;&#34;
+    Return the element in front of the queue. Raise Exception if queue is empty.
+    &#34;&#34;&#34;
+    if self.is_empty():
+        raise Exception(&#34;Empty Queue&#34;)
 
-    return self.array[0]</code></pre>
+    return self._array[self._front]</code></pre>
 </details>
 </dd>
 </dl>
 </dd>
 </dl>
 </section>
 </article>
@@ -475,31 +518,30 @@
 <ul>
 <li><code><a title="dsa" href="index.html">dsa</a></code></li>
 </ul>
 </li>
 <li><h3><a href="#header-classes">Classes</a></h3>
 <ul>
 <li>
-<h4><code><a title="dsa.heap.Heap" href="#dsa.heap.Heap">Heap</a></code></h4>
+<h4><code><a title="dsa.queue.DynamicQueue" href="#dsa.queue.DynamicQueue">DynamicQueue</a></code></h4>
+<ul class="">
+<li><code><a title="dsa.queue.DynamicQueue.check_capacity" href="#dsa.queue.DynamicQueue.check_capacity">check_capacity</a></code></li>
+<li><code><a title="dsa.queue.DynamicQueue.enqueue" href="#dsa.queue.DynamicQueue.enqueue">enqueue</a></code></li>
+<li><code><a title="dsa.queue.DynamicQueue.grow" href="#dsa.queue.DynamicQueue.grow">grow</a></code></li>
+</ul>
+</li>
+<li>
+<h4><code><a title="dsa.queue.Queue" href="#dsa.queue.Queue">Queue</a></code></h4>
 <ul class="two-column">
-<li><code><a title="dsa.heap.Heap.count" href="#dsa.heap.Heap.count">count</a></code></li>
-<li><code><a title="dsa.heap.Heap.has_left" href="#dsa.heap.Heap.has_left">has_left</a></code></li>
-<li><code><a title="dsa.heap.Heap.has_parent" href="#dsa.heap.Heap.has_parent">has_parent</a></code></li>
-<li><code><a title="dsa.heap.Heap.has_right" href="#dsa.heap.Heap.has_right">has_right</a></code></li>
-<li><code><a title="dsa.heap.Heap.heapify_down" href="#dsa.heap.Heap.heapify_down">heapify_down</a></code></li>
-<li><code><a title="dsa.heap.Heap.heapify_up" href="#dsa.heap.Heap.heapify_up">heapify_up</a></code></li>
-<li><code><a title="dsa.heap.Heap.insert" href="#dsa.heap.Heap.insert">insert</a></code></li>
-<li><code><a title="dsa.heap.Heap.is_empty" href="#dsa.heap.Heap.is_empty">is_empty</a></code></li>
-<li><code><a title="dsa.heap.Heap.last" href="#dsa.heap.Heap.last">last</a></code></li>
-<li><code><a title="dsa.heap.Heap.left_index" href="#dsa.heap.Heap.left_index">left_index</a></code></li>
-<li><code><a title="dsa.heap.Heap.parent_index" href="#dsa.heap.Heap.parent_index">parent_index</a></code></li>
-<li><code><a title="dsa.heap.Heap.pop" href="#dsa.heap.Heap.pop">pop</a></code></li>
-<li><code><a title="dsa.heap.Heap.print" href="#dsa.heap.Heap.print">print</a></code></li>
-<li><code><a title="dsa.heap.Heap.right_index" href="#dsa.heap.Heap.right_index">right_index</a></code></li>
-<li><code><a title="dsa.heap.Heap.root" href="#dsa.heap.Heap.root">root</a></code></li>
+<li><code><a title="dsa.queue.Queue.capacity" href="#dsa.queue.Queue.capacity">capacity</a></code></li>
+<li><code><a title="dsa.queue.Queue.count" href="#dsa.queue.Queue.count">count</a></code></li>
+<li><code><a title="dsa.queue.Queue.dequeue" href="#dsa.queue.Queue.dequeue">dequeue</a></code></li>
+<li><code><a title="dsa.queue.Queue.enqueue" href="#dsa.queue.Queue.enqueue">enqueue</a></code></li>
+<li><code><a title="dsa.queue.Queue.is_empty" href="#dsa.queue.Queue.is_empty">is_empty</a></code></li>
+<li><code><a title="dsa.queue.Queue.peek" href="#dsa.queue.Queue.peek">peek</a></code></li>
 </ul>
 </li>
 </ul>
 </li>
 </ul>
 </nav>
 </main>
```

#### html2text {}

```diff
@@ -1,315 +1,398 @@
-************ MMoodduullee ddssaa..hheeaapp ************
+************ MMoodduullee ddssaa..qquueeuuee ************
 Expand source code
-class Heap:
-    def __init__(self):
-        self.array = []
+class Queue:
+    """
+    A static queue implementation in Python
+    """
+    def __init__(self, capacity=10):
+        """
+        Args:
+            capacity: the initial size of the stack (defaults to 10)
+        """
+        self._array = [None] * capacity
+        self._front = 0
+        #: number of elements in queue
+        self.count = 0
+
+    def enqueue(self, element):
+        """
+        Enqueue an element into the queue. Raise Exception when trying to
+enqueue more elements than the capacity.
+
+        Args:
+            element: the element to enqueue
+        """
+        if self.count >= len(self._array):
+            raise Exception("Capacity Reached")
+
+        index = (self._front + self.count) % len(self._array)
+        self._array[index] = element
+        self.count += 1
+
+    def dequeue(self):
+        """
+        Dequeue an element from the queue. Raise Exception when there are no
+elements to dequeue.
+
+        Returns:
+            the from element in the queue
+        """
+        if self.is_empty():
+            raise Exception("Empty Queue")
+
+        element = self._array[self._front]
+        self._front += 1
+        if self._front >= len(self._array):
+            self._front = 0
+        self.count -= 1
+
+        return element
+
+    def peek(self):
+        """
+        Return the element in front of the queue. Raise Exception if queue is
+empty.
+        """
+        if self.is_empty():
+            raise Exception("Empty Queue")
 
-    def root(self):
-        if self.count() == 0:
-            return None
-
-        return self.array[0]
-
-    def last(self):
-        if self.count() == 0:
-            return None
-
-        return self.array[-1]
-
-    def left_index(self, index):
-        return (index * 2) + 1
-
-    def right_index(self, index):
-        return (index * 2) + 2
-
-    def parent_index(self, index):
-        return (index - 1) // 2
-
-    def has_left(self, index):
-        return self.left_index(index) < self.count()
-
-    def has_right(self, index):
-        return self.right_index(index) < self.count()
-
-    def has_parent(self, index):
-        return self.parent_index(index) >= 0
-
-    def insert(self, value):
-        self.array.append(value)
-
-        start_index = self.count() - 1
-        self.heapify_up(start_index)
-
-    def heapify_up(self, index):
-        parent_index = self.parent_index(index)
-        while self.has_parent(index) and self.array[index] > self.array
-[parent_index]:
-            self.array[index], self.array[parent_index] = self.array
-[parent_index], self.array[index]
-            index = parent_index
-            parent_index = self.parent_index(index)
-
-    def pop(self):
-        root_value = self.root()
-
-        # start at root node
-        start_index = 0
-        if self.count() == 1:
-            self.array.pop()
-        else:
-            self.array[start_index] = self.array.pop()
-
-        self.heapify_down(start_index)
-        return root_value
-
-    def heapify_down(self, index):
-        while self.has_left(index):
-            higher_index = self.left_index(index)
-
-            right_index = self.right_index(index)
-            if self.has_right(index) and self.array[right_index] > self.array
-[higher_index]:
-                higher_index = right_index
-
-            if self.array[index] > self.array[higher_index]:
-                break
-            else:
-                self.array[index], self.array[higher_index] = self.array
-[higher_index], self.array[index]
-
-            index = higher_index
-
-    def count(self):
-        return len(self.array)
+        return self._array[self._front]
 
     def is_empty(self):
-        return self.count() == 0
-
-    def print(self):
-        node_count = 1
-        for i in range(self.count()):
-            if i + 1 >= node_count:
-                print()
-                node_count *= 2
-            print(self.array[i], end=" ")
+        """
+        Return a Boolean on whether the stack is empty or not.
+        """
+        return self.count == 0
+
+    def capacity(self):
+        """
+        Return the capacity of the queue.
+        """
+        return len(self._array)
+
+    def __repr__(self):
+        arr = []
+        for i in range(self.count):
+            index = (i + self._front) % len(self._array)
+            arr.append(str(self._array[index]))
+        arrstr = ", ".join(arr)
+        return f"[{arrstr}] Front: {self._front} count: {self.count} Capacity:
+{self.capacity()}"
+
+
+# shrink not implemented
+class DynamicQueue(Queue):
+    """
+    A dynamic queue implementation in Python
+    """
+    def __init__(self, capacity=10):
+        super().__init__(capacity)
+
+    def grow(self):
+        """
+        double the capacity of the current array
+        """
+        new_array = [ None ] * len(self._array) * 2
+
+        # copy elements
+        for i in range(self.count):
+            new_array[i] = self._array[i + self._front]
+        self._front = 0
+        self._array = new_array
+
+    def check_capacity(self):
+        """
+        if count >= capacity, grow the array
+        """
+        if self._front + self.count >= len(self._array):
+            self.grow()
+
+    def enqueue(self, element):
+        """
+        Enqueue an element into the queue. Increae capacity if count is greater
+than the capacity.
+
+        Args:
+            element: the element to enqueue
+        """
+        self.check_capacity()
+        index = self._front + self.count
+        self._array[index] = element
+        self.count += 1
 ********** CCllaasssseess **********
-  class Heap
+  class DynamicQueue (capacity=10)
+      A dynamic queue implementation in Python
+      ********** AArrggss **********
+        ccaappaacciittyy
+            the initial size of the stack (defaults to 10)
       Expand source code
-      class Heap:
-          def __init__(self):
-              self.array = []
-
-          def root(self):
-              if self.count() == 0:
-                  return None
-
-              return self.array[0]
-
-          def last(self):
-              if self.count() == 0:
-                  return None
-
-              return self.array[-1]
-
-          def left_index(self, index):
-              return (index * 2) + 1
-
-          def right_index(self, index):
-              return (index * 2) + 2
-
-          def parent_index(self, index):
-              return (index - 1) // 2
-
-          def has_left(self, index):
-              return self.left_index(index) < self.count()
-
-          def has_right(self, index):
-              return self.right_index(index) < self.count()
-
-          def has_parent(self, index):
-              return self.parent_index(index) >= 0
-
-          def insert(self, value):
-              self.array.append(value)
-
-              start_index = self.count() - 1
-              self.heapify_up(start_index)
-
-          def heapify_up(self, index):
-              parent_index = self.parent_index(index)
-              while self.has_parent(index) and self.array[index] > self.array
-      [parent_index]:
-                  self.array[index], self.array[parent_index] = self.array
-      [parent_index], self.array[index]
-                  index = parent_index
-                  parent_index = self.parent_index(index)
-
-          def pop(self):
-              root_value = self.root()
-
-              # start at root node
-              start_index = 0
-              if self.count() == 1:
-                  self.array.pop()
-              else:
-                  self.array[start_index] = self.array.pop()
-
-              self.heapify_down(start_index)
-              return root_value
-
-          def heapify_down(self, index):
-              while self.has_left(index):
-                  higher_index = self.left_index(index)
-
-                  right_index = self.right_index(index)
-                  if self.has_right(index) and self.array[right_index] >
-      self.array[higher_index]:
-                      higher_index = right_index
-
-                  if self.array[index] > self.array[higher_index]:
-                      break
-                  else:
-                      self.array[index], self.array[higher_index] = self.array
-      [higher_index], self.array[index]
-
-                  index = higher_index
+      class DynamicQueue(Queue):
+          """
+          A dynamic queue implementation in Python
+          """
+          def __init__(self, capacity=10):
+              super().__init__(capacity)
+
+          def grow(self):
+              """
+              double the capacity of the current array
+              """
+              new_array = [ None ] * len(self._array) * 2
+
+              # copy elements
+              for i in range(self.count):
+                  new_array[i] = self._array[i + self._front]
+              self._front = 0
+              self._array = new_array
+
+          def check_capacity(self):
+              """
+              if count >= capacity, grow the array
+              """
+              if self._front + self.count >= len(self._array):
+                  self.grow()
+
+          def enqueue(self, element):
+              """
+              Enqueue an element into the queue. Increae capacity if count is
+      greater than the capacity.
+
+              Args:
+                  element: the element to enqueue
+              """
+              self.check_capacity()
+              index = self._front + self.count
+              self._array[index] = element
+              self.count += 1
+      ******** AAnncceessttoorrss ********
+          * _Q_u_e_u_e
+      ******** MMeetthhooddss ********
+        def check_capacity(self)
+            if count >= capacity, grow the array
+            Expand source code
+            def check_capacity(self):
+                """
+                if count >= capacity, grow the array
+                """
+                if self._front + self.count >= len(self._array):
+                    self.grow()
+        def enqueue(self, element)
+            Enqueue an element into the queue. Increae capacity if count is
+            greater than the capacity.
+            ********** AArrggss **********
+              eelleemmeenntt
+                  the element to enqueue
+            Expand source code
+            def enqueue(self, element):
+                """
+                Enqueue an element into the queue. Increae capacity if count is
+            greater than the capacity.
+
+                Args:
+                    element: the element to enqueue
+                """
+                self.check_capacity()
+                index = self._front + self.count
+                self._array[index] = element
+                self.count += 1
+        def grow(self)
+            double the capacity of the current array
+            Expand source code
+            def grow(self):
+                """
+                double the capacity of the current array
+                """
+                new_array = [ None ] * len(self._array) * 2
+
+                # copy elements
+                for i in range(self.count):
+                    new_array[i] = self._array[i + self._front]
+                self._front = 0
+                self._array = new_array
+      ******** IInnhheerriitteedd mmeemmbbeerrss ********
+          * _QQ_uu_ee_uu_ee:
+                o _c_a_p_a_c_i_t_y
+                o _c_o_u_n_t
+                o _d_e_q_u_e_u_e
+                o _i_s___e_m_p_t_y
+                o _p_e_e_k
+  class Queue (capacity=10)
+      A static queue implementation in Python
+      ********** AArrggss **********
+        ccaappaacciittyy
+            the initial size of the stack (defaults to 10)
+      Expand source code
+      class Queue:
+          """
+          A static queue implementation in Python
+          """
+          def __init__(self, capacity=10):
+              """
+              Args:
+                  capacity: the initial size of the stack (defaults to 10)
+              """
+              self._array = [None] * capacity
+              self._front = 0
+              #: number of elements in queue
+              self.count = 0
+
+          def enqueue(self, element):
+              """
+              Enqueue an element into the queue. Raise Exception when trying to
+      enqueue more elements than the capacity.
+
+              Args:
+                  element: the element to enqueue
+              """
+              if self.count >= len(self._array):
+                  raise Exception("Capacity Reached")
+
+              index = (self._front + self.count) % len(self._array)
+              self._array[index] = element
+              self.count += 1
+
+          def dequeue(self):
+              """
+              Dequeue an element from the queue. Raise Exception when there are
+      no elements to dequeue.
+
+              Returns:
+                  the from element in the queue
+              """
+              if self.is_empty():
+                  raise Exception("Empty Queue")
+
+              element = self._array[self._front]
+              self._front += 1
+              if self._front >= len(self._array):
+                  self._front = 0
+              self.count -= 1
+
+              return element
+
+          def peek(self):
+              """
+              Return the element in front of the queue. Raise Exception if
+      queue is empty.
+              """
+              if self.is_empty():
+                  raise Exception("Empty Queue")
 
-          def count(self):
-              return len(self.array)
+              return self._array[self._front]
 
           def is_empty(self):
-              return self.count() == 0
-
-          def print(self):
-              node_count = 1
-              for i in range(self.count()):
-                  if i + 1 >= node_count:
-                      print()
-                      node_count *= 2
-                  print(self.array[i], end=" ")
+              """
+              Return a Boolean on whether the stack is empty or not.
+              """
+              return self.count == 0
+
+          def capacity(self):
+              """
+              Return the capacity of the queue.
+              """
+              return len(self._array)
+
+          def __repr__(self):
+              arr = []
+              for i in range(self.count):
+                  index = (i + self._front) % len(self._array)
+                  arr.append(str(self._array[index]))
+              arrstr = ", ".join(arr)
+              return f"[{arrstr}] Front: {self._front} count: {self.count}
+      Capacity: {self.capacity()}"
+      ******** SSuubbccllaasssseess ********
+          * _D_y_n_a_m_i_c_Q_u_e_u_e
+      ******** IInnssttaannccee vvaarriiaabblleess ********
+        var count
+            number of elements in queue
       ******** MMeetthhooddss ********
-        def count(self)
-            Expand source code
-            def count(self):
-                return len(self.array)
-        def has_left(self, index)
-            Expand source code
-            def has_left(self, index):
-                return self.left_index(index) < self.count()
-        def has_parent(self, index)
+        def capacity(self)
+            Return the capacity of the queue.
             Expand source code
-            def has_parent(self, index):
-                return self.parent_index(index) >= 0
-        def has_right(self, index)
-            Expand source code
-            def has_right(self, index):
-                return self.right_index(index) < self.count()
-        def heapify_down(self, index)
-            Expand source code
-            def heapify_down(self, index):
-                while self.has_left(index):
-                    higher_index = self.left_index(index)
-
-                    right_index = self.right_index(index)
-                    if self.has_right(index) and self.array[right_index] >
-            self.array[higher_index]:
-                        higher_index = right_index
-
-                    if self.array[index] > self.array[higher_index]:
-                        break
-                    else:
-                        self.array[index], self.array[higher_index] =
-            self.array[higher_index], self.array[index]
-
-                    index = higher_index
-        def heapify_up(self, index)
-            Expand source code
-            def heapify_up(self, index):
-                parent_index = self.parent_index(index)
-                while self.has_parent(index) and self.array[index] > self.array
-            [parent_index]:
-                    self.array[index], self.array[parent_index] = self.array
-            [parent_index], self.array[index]
-                    index = parent_index
-                    parent_index = self.parent_index(index)
-        def insert(self, value)
-            Expand source code
-            def insert(self, value):
-                self.array.append(value)
-
-                start_index = self.count() - 1
-                self.heapify_up(start_index)
+            def capacity(self):
+                """
+                Return the capacity of the queue.
+                """
+                return len(self._array)
+        def dequeue(self)
+            Dequeue an element from the queue. Raise Exception when there are
+            no elements to dequeue.
+            ********** RReettuurrnnss **********
+            the from element in the queue
+            Expand source code
+            def dequeue(self):
+                """
+                Dequeue an element from the queue. Raise Exception when there
+            are no elements to dequeue.
+
+                Returns:
+                    the from element in the queue
+                """
+                if self.is_empty():
+                    raise Exception("Empty Queue")
+
+                element = self._array[self._front]
+                self._front += 1
+                if self._front >= len(self._array):
+                    self._front = 0
+                self.count -= 1
+
+                return element
+        def enqueue(self, element)
+            Enqueue an element into the queue. Raise Exception when trying to
+            enqueue more elements than the capacity.
+            ********** AArrggss **********
+              eelleemmeenntt
+                  the element to enqueue
+            Expand source code
+            def enqueue(self, element):
+                """
+                Enqueue an element into the queue. Raise Exception when trying
+            to enqueue more elements than the capacity.
+
+                Args:
+                    element: the element to enqueue
+                """
+                if self.count >= len(self._array):
+                    raise Exception("Capacity Reached")
+
+                index = (self._front + self.count) % len(self._array)
+                self._array[index] = element
+                self.count += 1
         def is_empty(self)
+            Return a Boolean on whether the stack is empty or not.
             Expand source code
             def is_empty(self):
-                return self.count() == 0
-        def last(self)
-            Expand source code
-            def last(self):
-                if self.count() == 0:
-                    return None
-
-                return self.array[-1]
-        def left_index(self, index)
-            Expand source code
-            def left_index(self, index):
-                return (index * 2) + 1
-        def parent_index(self, index)
-            Expand source code
-            def parent_index(self, index):
-                return (index - 1) // 2
-        def pop(self)
-            Expand source code
-            def pop(self):
-                root_value = self.root()
-
-                # start at root node
-                start_index = 0
-                if self.count() == 1:
-                    self.array.pop()
-                else:
-                    self.array[start_index] = self.array.pop()
-
-                self.heapify_down(start_index)
-                return root_value
-        def print(self)
-            Expand source code
-            def print(self):
-                node_count = 1
-                for i in range(self.count()):
-                    if i + 1 >= node_count:
-                        print()
-                        node_count *= 2
-                    print(self.array[i], end=" ")
-        def right_index(self, index)
-            Expand source code
-            def right_index(self, index):
-                return (index * 2) + 2
-        def root(self)
-            Expand source code
-            def root(self):
-                if self.count() == 0:
-                    return None
+                """
+                Return a Boolean on whether the stack is empty or not.
+                """
+                return self.count == 0
+        def peek(self)
+            Return the element in front of the queue. Raise Exception if queue
+            is empty.
+            Expand source code
+            def peek(self):
+                """
+                Return the element in front of the queue. Raise Exception if
+            queue is empty.
+                """
+                if self.is_empty():
+                    raise Exception("Empty Queue")
 
-                return self.array[0]
+                return self._array[self._front]
 ************ IInnddeexx ************
     * ******** SSuuppeerr--mmoodduullee ********
           o _d_s_a
     * ******** _CC_ll_aa_ss_ss_ee_ss ********
-          o ****** _HH_ee_aa_pp ******
+          o ****** _DD_yy_nn_aa_mm_ii_cc_QQ_uu_ee_uu_ee ******
+                # _c_h_e_c_k___c_a_p_a_c_i_t_y
+                # _e_n_q_u_e_u_e
+                # _g_r_o_w
+          o ****** _QQ_uu_ee_uu_ee ******
+                # _c_a_p_a_c_i_t_y
                 # _c_o_u_n_t
-                # _h_a_s___l_e_f_t
-                # _h_a_s___p_a_r_e_n_t
-                # _h_a_s___r_i_g_h_t
-                # _h_e_a_p_i_f_y___d_o_w_n
-                # _h_e_a_p_i_f_y___u_p
-                # _i_n_s_e_r_t
+                # _d_e_q_u_e_u_e
+                # _e_n_q_u_e_u_e
                 # _i_s___e_m_p_t_y
-                # _l_a_s_t
-                # _l_e_f_t___i_n_d_e_x
-                # _p_a_r_e_n_t___i_n_d_e_x
-                # _p_o_p
-                # _p_r_i_n_t
-                # _r_i_g_h_t___i_n_d_e_x
-                # _r_o_o_t
+                # _p_e_e_k
 Generated by_p_d_o_c_0_._1_0_._0.
```

### Comparing `ucxdsa-2024.4.23/src/html/dsa/huffman.html` & `ucxdsa-2024.5.9/src/html/dsa/huffman.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html lang="en">
 <head>
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
 <meta name="generator" content="pdoc 0.10.0" />
 <title>dsa.huffman API documentation</title>
-<meta name="description" content="" />
+<meta name="description" content="a collection of Huffman functions" />
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
 <link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
 <style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
 <style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
 <style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
 <script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
@@ -18,87 +18,95 @@
 <body>
 <main>
 <article id="content">
 <header>
 <h1 class="title">Module <code>dsa.huffman</code></h1>
 </header>
 <section id="section-intro">
+<p>a collection of Huffman functions</p>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">import heapq
+<pre><code class="python">&#34;&#34;&#34; a collection of Huffman functions &#34;&#34;&#34;
+import heapq
 
 class Node:
+    &#34;&#34;&#34; binary node implementation &#34;&#34;&#34;
     def __init__(self, left, right, value=None):
-        self.child = [left, right]
+        self.left = left
+        self.right = right
         self.value = value
     
     def __lt__(self, other):
         return False
     
     def __repr__(self):
         if self.value is None:
             return &#34;none&#34;
         else:
             return self.value
 
-def character_frequency(s):
-    &#39;&#39;&#39; takes a string a returns a dictionary on character frequency &#39;&#39;&#39;
+def character_frequency(s: str):
+    &#34;&#34;&#34; takes a string a returns a dictionary on character frequency &#34;&#34;&#34;
     d = {}
     for c in s:
         if c not in d:
             d[c] = 1
         else:
             d[c] += 1
     return d
 
-def build_frequency_table(s):
-    &#39;&#39;&#39; accepts a string to encode and returns a heap of the characters &#39;&#39;&#39;
+def build_frequency_table(s: str):
+    &#34;&#34;&#34; accepts a string to encode and returns a heap of the characters &#34;&#34;&#34;
     frequency_dictionary = character_frequency(s)
     
     # add to priority queue
     h = []
     for item in frequency_dictionary.items():
         heapq.heappush(h, (item[1], Node(None, None, item[0])))
 
     return h
 
 def build_huffman_tree(heap):
-    &#39;&#39;&#39; accepts a heap and returns a Huffman Tree &#39;&#39;&#39;
+    &#34;&#34;&#34; accepts a heap and returns a Huffman Tree &#34;&#34;&#34;
     while len(heap) &gt; 1:
         n1 = heapq.heappop(heap)
         n2 = heapq.heappop(heap)
         node = Node(n1[1], n2[1])
         heapq.heappush(heap, (n1[0] + n2[0], node))
     return heap[0][1]
 
-def build_huffman_dictionary(node, bit_string=&#34;&#34;):
-    &#39;&#39;&#39; given a Huffman Node, build a Huffman Dictionary &#39;&#39;&#39;
+def build_huffman_dictionary(node, bit_string: str=&#34;&#34;):
+    &#34;&#34;&#34; given a Huffman Node, build a Huffman Dictionary &#34;&#34;&#34;
     d = {}
-    if node.child[0] is None and node.child[1] is None:
+    if node.left is None and node.right is None:
         return {node.value: bit_string}
 
-    d.update(build_huffman_dictionary(node.child[0], bit_string + &#39;0&#39;))
-    d.update(build_huffman_dictionary(node.child[1], bit_string + &#39;1&#39;))
+    d.update(build_huffman_dictionary(node.left, bit_string + &#39;0&#39;))
+    d.update(build_huffman_dictionary(node.right, bit_string + &#39;1&#39;))
 
     return d
 
-def huffman_encode(string, hd):
+def huffman_encode(st, hd):
     s = &#34;&#34;
-    for c in string:
+    for c in st:
         s += hd[c]
     return s
 
 def huffman_decode(encoded_data, tree):
     root = tree
     s = &#34;&#34;
     for bit in encoded_data:
-        tree = tree.child[int(bit)]
-        if tree.child[0] is None and tree.child[1] is None: 
+        if int(bit) == 0:
+            tree = tree.left
+        else:
+            tree = tree.right
+
+        if tree.left is None and tree.right is None: 
             s += tree.value
             tree = root
     return s
 
 def bitstring_to_bytes(s):
     return bytes(int(s[i : i + 8], 2) for i in range(0, len(s), 8))
 
@@ -131,66 +139,66 @@
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def bitstring_to_bytes(s):
     return bytes(int(s[i : i + 8], 2) for i in range(0, len(s), 8))</code></pre>
 </details>
 </dd>
 <dt id="dsa.huffman.build_frequency_table"><code class="name flex">
-<span>def <span class="ident">build_frequency_table</span></span>(<span>s)</span>
+<span>def <span class="ident">build_frequency_table</span></span>(<span>s: str)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>accepts a string to encode and returns a heap of the characters</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def build_frequency_table(s):
-    &#39;&#39;&#39; accepts a string to encode and returns a heap of the characters &#39;&#39;&#39;
+<pre><code class="python">def build_frequency_table(s: str):
+    &#34;&#34;&#34; accepts a string to encode and returns a heap of the characters &#34;&#34;&#34;
     frequency_dictionary = character_frequency(s)
     
     # add to priority queue
     h = []
     for item in frequency_dictionary.items():
         heapq.heappush(h, (item[1], Node(None, None, item[0])))
 
     return h</code></pre>
 </details>
 </dd>
 <dt id="dsa.huffman.build_huffman_dictionary"><code class="name flex">
-<span>def <span class="ident">build_huffman_dictionary</span></span>(<span>node, bit_string='')</span>
+<span>def <span class="ident">build_huffman_dictionary</span></span>(<span>node, bit_string: str = '')</span>
 </code></dt>
 <dd>
 <div class="desc"><p>given a Huffman Node, build a Huffman Dictionary</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def build_huffman_dictionary(node, bit_string=&#34;&#34;):
-    &#39;&#39;&#39; given a Huffman Node, build a Huffman Dictionary &#39;&#39;&#39;
+<pre><code class="python">def build_huffman_dictionary(node, bit_string: str=&#34;&#34;):
+    &#34;&#34;&#34; given a Huffman Node, build a Huffman Dictionary &#34;&#34;&#34;
     d = {}
-    if node.child[0] is None and node.child[1] is None:
+    if node.left is None and node.right is None:
         return {node.value: bit_string}
 
-    d.update(build_huffman_dictionary(node.child[0], bit_string + &#39;0&#39;))
-    d.update(build_huffman_dictionary(node.child[1], bit_string + &#39;1&#39;))
+    d.update(build_huffman_dictionary(node.left, bit_string + &#39;0&#39;))
+    d.update(build_huffman_dictionary(node.right, bit_string + &#39;1&#39;))
 
     return d</code></pre>
 </details>
 </dd>
 <dt id="dsa.huffman.build_huffman_tree"><code class="name flex">
 <span>def <span class="ident">build_huffman_tree</span></span>(<span>heap)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>accepts a heap and returns a Huffman Tree</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def build_huffman_tree(heap):
-    &#39;&#39;&#39; accepts a heap and returns a Huffman Tree &#39;&#39;&#39;
+    &#34;&#34;&#34; accepts a heap and returns a Huffman Tree &#34;&#34;&#34;
     while len(heap) &gt; 1:
         n1 = heapq.heappop(heap)
         n2 = heapq.heappop(heap)
         node = Node(n1[1], n2[1])
         heapq.heappush(heap, (n1[0] + n2[0], node))
     return heap[0][1]</code></pre>
 </details>
@@ -213,24 +221,24 @@
     byte = f&#34;{ba[-1]:b}&#34;.zfill(bitlength) 
     s += byte
 
     return s</code></pre>
 </details>
 </dd>
 <dt id="dsa.huffman.character_frequency"><code class="name flex">
-<span>def <span class="ident">character_frequency</span></span>(<span>s)</span>
+<span>def <span class="ident">character_frequency</span></span>(<span>s: str)</span>
 </code></dt>
 <dd>
 <div class="desc"><p>takes a string a returns a dictionary on character frequency</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def character_frequency(s):
-    &#39;&#39;&#39; takes a string a returns a dictionary on character frequency &#39;&#39;&#39;
+<pre><code class="python">def character_frequency(s: str):
+    &#34;&#34;&#34; takes a string a returns a dictionary on character frequency &#34;&#34;&#34;
     d = {}
     for c in s:
         if c not in d:
             d[c] = 1
         else:
             d[c] += 1
     return d</code></pre>
@@ -245,55 +253,61 @@
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">def huffman_decode(encoded_data, tree):
     root = tree
     s = &#34;&#34;
     for bit in encoded_data:
-        tree = tree.child[int(bit)]
-        if tree.child[0] is None and tree.child[1] is None: 
+        if int(bit) == 0:
+            tree = tree.left
+        else:
+            tree = tree.right
+
+        if tree.left is None and tree.right is None: 
             s += tree.value
             tree = root
     return s</code></pre>
 </details>
 </dd>
 <dt id="dsa.huffman.huffman_encode"><code class="name flex">
-<span>def <span class="ident">huffman_encode</span></span>(<span>string, hd)</span>
+<span>def <span class="ident">huffman_encode</span></span>(<span>st, hd)</span>
 </code></dt>
 <dd>
 <div class="desc"></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def huffman_encode(string, hd):
+<pre><code class="python">def huffman_encode(st, hd):
     s = &#34;&#34;
-    for c in string:
+    for c in st:
         s += hd[c]
     return s</code></pre>
 </details>
 </dd>
 </dl>
 </section>
 <section>
 <h2 class="section-title" id="header-classes">Classes</h2>
 <dl>
 <dt id="dsa.huffman.Node"><code class="flex name class">
 <span>class <span class="ident">Node</span></span>
 <span>(</span><span>left, right, value=None)</span>
 </code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>binary node implementation</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">class Node:
+    &#34;&#34;&#34; binary node implementation &#34;&#34;&#34;
     def __init__(self, left, right, value=None):
-        self.child = [left, right]
+        self.left = left
+        self.right = right
         self.value = value
     
     def __lt__(self, other):
         return False
     
     def __repr__(self):
         if self.value is None:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,78 +1,86 @@
 ************ MMoodduullee ddssaa..hhuuffffmmaann ************
+a collection of Huffman functions
 Expand source code
+""" a collection of Huffman functions """
 import heapq
 
 class Node:
+    """ binary node implementation """
     def __init__(self, left, right, value=None):
-        self.child = [left, right]
+        self.left = left
+        self.right = right
         self.value = value
 
     def __lt__(self, other):
         return False
 
     def __repr__(self):
         if self.value is None:
             return "none"
         else:
             return self.value
 
-def character_frequency(s):
-    ''' takes a string a returns a dictionary on character frequency '''
+def character_frequency(s: str):
+    """ takes a string a returns a dictionary on character frequency """
     d = {}
     for c in s:
         if c not in d:
             d[c] = 1
         else:
             d[c] += 1
     return d
 
-def build_frequency_table(s):
-    ''' accepts a string to encode and returns a heap of the characters '''
+def build_frequency_table(s: str):
+    """ accepts a string to encode and returns a heap of the characters """
     frequency_dictionary = character_frequency(s)
 
     # add to priority queue
     h = []
     for item in frequency_dictionary.items():
         heapq.heappush(h, (item[1], Node(None, None, item[0])))
 
     return h
 
 def build_huffman_tree(heap):
-    ''' accepts a heap and returns a Huffman Tree '''
+    """ accepts a heap and returns a Huffman Tree """
     while len(heap) > 1:
         n1 = heapq.heappop(heap)
         n2 = heapq.heappop(heap)
         node = Node(n1[1], n2[1])
         heapq.heappush(heap, (n1[0] + n2[0], node))
     return heap[0][1]
 
-def build_huffman_dictionary(node, bit_string=""):
-    ''' given a Huffman Node, build a Huffman Dictionary '''
+def build_huffman_dictionary(node, bit_string: str=""):
+    """ given a Huffman Node, build a Huffman Dictionary """
     d = {}
-    if node.child[0] is None and node.child[1] is None:
+    if node.left is None and node.right is None:
         return {node.value: bit_string}
 
-    d.update(build_huffman_dictionary(node.child[0], bit_string + '0'))
-    d.update(build_huffman_dictionary(node.child[1], bit_string + '1'))
+    d.update(build_huffman_dictionary(node.left, bit_string + '0'))
+    d.update(build_huffman_dictionary(node.right, bit_string + '1'))
 
     return d
 
-def huffman_encode(string, hd):
+def huffman_encode(st, hd):
     s = ""
-    for c in string:
+    for c in st:
         s += hd[c]
     return s
 
 def huffman_decode(encoded_data, tree):
     root = tree
     s = ""
     for bit in encoded_data:
-        tree = tree.child[int(bit)]
-        if tree.child[0] is None and tree.child[1] is None:
+        if int(bit) == 0:
+            tree = tree.left
+        else:
+            tree = tree.right
+
+        if tree.left is None and tree.right is None:
             s += tree.value
             tree = root
     return s
 
 def bitstring_to_bytes(s):
     return bytes(int(s[i : i + 8], 2) for i in range(0, len(s), 8))
 
@@ -87,46 +95,46 @@
 
     return s
 ********** FFuunnccttiioonnss **********
   def bitstring_to_bytes(s)
       Expand source code
       def bitstring_to_bytes(s):
           return bytes(int(s[i : i + 8], 2) for i in range(0, len(s), 8))
-  def build_frequency_table(s)
+  def build_frequency_table(s: str)
       accepts a string to encode and returns a heap of the characters
       Expand source code
-      def build_frequency_table(s):
-          ''' accepts a string to encode and returns a heap of the characters
-      '''
+      def build_frequency_table(s: str):
+          """ accepts a string to encode and returns a heap of the characters
+      """
           frequency_dictionary = character_frequency(s)
 
           # add to priority queue
           h = []
           for item in frequency_dictionary.items():
               heapq.heappush(h, (item[1], Node(None, None, item[0])))
 
           return h
-  def build_huffman_dictionary(node, bit_string='')
+  def build_huffman_dictionary(node, bit_string: str = '')
       given a Huffman Node, build a Huffman Dictionary
       Expand source code
-      def build_huffman_dictionary(node, bit_string=""):
-          ''' given a Huffman Node, build a Huffman Dictionary '''
+      def build_huffman_dictionary(node, bit_string: str=""):
+          """ given a Huffman Node, build a Huffman Dictionary """
           d = {}
-          if node.child[0] is None and node.child[1] is None:
+          if node.left is None and node.right is None:
               return {node.value: bit_string}
 
-          d.update(build_huffman_dictionary(node.child[0], bit_string + '0'))
-          d.update(build_huffman_dictionary(node.child[1], bit_string + '1'))
+          d.update(build_huffman_dictionary(node.left, bit_string + '0'))
+          d.update(build_huffman_dictionary(node.right, bit_string + '1'))
 
           return d
   def build_huffman_tree(heap)
       accepts a heap and returns a Huffman Tree
       Expand source code
       def build_huffman_tree(heap):
-          ''' accepts a heap and returns a Huffman Tree '''
+          """ accepts a heap and returns a Huffman Tree """
           while len(heap) > 1:
               n1 = heapq.heappop(heap)
               n2 = heapq.heappop(heap)
               node = Node(n1[1], n2[1])
               heapq.heappush(heap, (n1[0] + n2[0], node))
           return heap[0][1]
   def bytes_to_bitstring(ba, bitlength=8)
@@ -137,50 +145,57 @@
               byte = f"{b:08b}"
               s += byte
 
           byte = f"{ba[-1]:b}".zfill(bitlength)
           s += byte
 
           return s
-  def character_frequency(s)
+  def character_frequency(s: str)
       takes a string a returns a dictionary on character frequency
       Expand source code
-      def character_frequency(s):
-          ''' takes a string a returns a dictionary on character frequency '''
+      def character_frequency(s: str):
+          """ takes a string a returns a dictionary on character frequency """
           d = {}
           for c in s:
               if c not in d:
                   d[c] = 1
               else:
                   d[c] += 1
           return d
   def huffman_decode(encoded_data, tree)
       Expand source code
       def huffman_decode(encoded_data, tree):
           root = tree
           s = ""
           for bit in encoded_data:
-              tree = tree.child[int(bit)]
-              if tree.child[0] is None and tree.child[1] is None:
+              if int(bit) == 0:
+                  tree = tree.left
+              else:
+                  tree = tree.right
+
+              if tree.left is None and tree.right is None:
                   s += tree.value
                   tree = root
           return s
-  def huffman_encode(string, hd)
+  def huffman_encode(st, hd)
       Expand source code
-      def huffman_encode(string, hd):
+      def huffman_encode(st, hd):
           s = ""
-          for c in string:
+          for c in st:
               s += hd[c]
           return s
 ********** CCllaasssseess **********
   class Node (left, right, value=None)
+      binary node implementation
       Expand source code
       class Node:
+          """ binary node implementation """
           def __init__(self, left, right, value=None):
-              self.child = [left, right]
+              self.left = left
+              self.right = right
               self.value = value
 
           def __lt__(self, other):
               return False
 
           def __repr__(self):
               if self.value is None:
```

### Comparing `ucxdsa-2024.4.23/src/html/dsa/index.html` & `ucxdsa-2024.5.9/src/html/dsa/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <html lang="en">
 <head>
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
 <meta name="generator" content="pdoc 0.10.0" />
 <title>dsa API documentation</title>
 <meta name="description" content="dsa package for UC Berkeley Extension&#39;s Computer Science X404.1 Data Structures and Algorithms class
-Last Revision: 2/12/2024" />
+Last Revision: 4/23/2024" />
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
 <link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
 <style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
 <style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
 <style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
 <script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
@@ -20,23 +20,24 @@
 <main>
 <article id="content">
 <header>
 <h1 class="title">Package <code>dsa</code></h1>
 </header>
 <section id="section-intro">
 <p>dsa package for UC Berkeley Extension's Computer Science X404.1 Data Structures and Algorithms class
-Last Revision: 2/12/2024</p>
+Last Revision: 4/23/2024</p>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">&#39;&#39;&#39;
 dsa package for UC Berkeley Extension&#39;s Computer Science X404.1 Data Structures and Algorithms class
-Last Revision: 2/12/2024
-&#39;&#39;&#39;</code></pre>
+Last Revision: 4/23/2024
+&#39;&#39;&#39;
+version = &#39;2024.4.23&#39;</code></pre>
 </details>
 </section>
 <section>
 <h2 class="section-title" id="header-submodules">Sub-modules</h2>
 <dl>
 <dt><code class="name"><a title="dsa.array" href="array.html">dsa.array</a></code></dt>
 <dd>
@@ -56,15 +57,15 @@
 </dd>
 <dt><code class="name"><a title="dsa.heap" href="heap.html">dsa.heap</a></code></dt>
 <dd>
 <div class="desc"></div>
 </dd>
 <dt><code class="name"><a title="dsa.huffman" href="huffman.html">dsa.huffman</a></code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>a collection of Huffman functions</p></div>
 </dd>
 <dt><code class="name"><a title="dsa.pretty_print" href="pretty_print.html">dsa.pretty_print</a></code></dt>
 <dd>
 <div class="desc"></div>
 </dd>
 <dt><code class="name"><a title="dsa.queue" href="queue.html">dsa.queue</a></code></dt>
 <dd>
@@ -72,15 +73,15 @@
 </dd>
 <dt><code class="name"><a title="dsa.singlylinkedlist" href="singlylinkedlist.html">dsa.singlylinkedlist</a></code></dt>
 <dd>
 <div class="desc"></div>
 </dd>
 <dt><code class="name"><a title="dsa.sorttools" href="sorttools.html">dsa.sorttools</a></code></dt>
 <dd>
-<div class="desc"></div>
+<div class="desc"><p>a collection of functions for sort benchmarks</p></div>
 </dd>
 <dt><code class="name"><a title="dsa.stack" href="stack.html">dsa.stack</a></code></dt>
 <dd>
 <div class="desc"></div>
 </dd>
 <dt><code class="name"><a title="dsa.tree" href="tree.html">dsa.tree</a></code></dt>
 <dd>
```

#### html2text {}

```diff
@@ -1,27 +1,30 @@
 ************ PPaacckkaaggee ddssaa ************
 dsa package for UC Berkeley Extension's Computer Science X404.1 Data Structures
-and Algorithms class Last Revision: 2/12/2024
+and Algorithms class Last Revision: 4/23/2024
 Expand source code
 '''
 dsa package for UC Berkeley Extension's Computer Science X404.1 Data Structures
 and Algorithms class
-Last Revision: 2/12/2024
+Last Revision: 4/23/2024
 '''
+version = '2024.4.23'
 ********** SSuubb--mmoodduulleess **********
   _d_s_a_._a_r_r_a_y
   _d_s_a_._d_o_u_b_l_y_l_i_n_k_e_d_l_i_s_t
   _d_s_a_._g_r_a_p_h
   _d_s_a_._h_a_s_h_t_a_b_l_e
   _d_s_a_._h_e_a_p
   _d_s_a_._h_u_f_f_m_a_n
+      a collection of Huffman functions
   _d_s_a_._p_r_e_t_t_y___p_r_i_n_t
   _d_s_a_._q_u_e_u_e
   _d_s_a_._s_i_n_g_l_y_l_i_n_k_e_d_l_i_s_t
   _d_s_a_._s_o_r_t_t_o_o_l_s
+      a collection of functions for sort benchmarks
   _d_s_a_._s_t_a_c_k
   _d_s_a_._t_r_e_e
   _d_s_a_._t_r_i_e
 ************ IInnddeexx ************
     * ******** _SS_uu_bb_--_mm_oo_dd_uu_ll_ee_ss ********
           o _d_s_a_._a_r_r_a_y
           o _d_s_a_._d_o_u_b_l_y_l_i_n_k_e_d_l_i_s_t
```

### Comparing `ucxdsa-2024.4.23/src/html/dsa/pretty_print.html` & `ucxdsa-2024.5.9/src/html/dsa/sorttools.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,214 +1,186 @@
 <!doctype html>
 <html lang="en">
 <head>
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
 <meta name="generator" content="pdoc 0.10.0" />
-<title>dsa.pretty_print API documentation</title>
-<meta name="description" content="" />
+<title>dsa.sorttools API documentation</title>
+<meta name="description" content="a collection of functions for sort benchmarks" />
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
 <link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
 <style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
 <style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
 <style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
 <script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
 <script>window.addEventListener('DOMContentLoaded', () => hljs.initHighlighting())</script>
 </head>
 <body>
 <main>
 <article id="content">
 <header>
-<h1 class="title">Module <code>dsa.pretty_print</code></h1>
+<h1 class="title">Module <code>dsa.sorttools</code></h1>
 </header>
 <section id="section-intro">
+<p>a collection of functions for sort benchmarks</p>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">import math
+<pre><code class="python">&#34;&#34;&#34; a collection of functions for sort benchmarks &#34;&#34;&#34;
+import random
 
-def heap_print(heap):
-    &#39;&#39;&#39; print a heap &#39;&#39;&#39;
-    if len(heap) == 0:
-        return
-    height = math.floor(math.log2(len(heap)))
-    level_str = &#34;&#34;
-    current_level = 0
-    value_width = 3
-    max_width = 2 ** (height - 1) * value_width
-
-    for index, node in enumerate(heap):
-        level = int(math.log2(index + 1))
-        columns = 2 ** (level - 1)
-        column_width = int(max_width / columns)
-        if current_level != level:
-            current_level = level
-            print(level_str)
-            level_str = &#34;&#34;
-        level_str += f&#34;{node:^{column_width}}&#34;
-    print(level_str)
-    print()
-
-
-def tree_to_array(node, index=0, tree_array=None):
-    &#39;&#39;&#39; create an array filled with index and value pairs from a node based tree &#39;&#39;&#39;
-    if not tree_array:
-        tree_array = []
-    if node is None:
-        return
-    tree_array.append((index, node.value))
-    tree_to_array(node.left, index * 2 + 1, tree_array)
-    tree_to_array(node.right, index * 2 + 2, tree_array)
-    
-    return tree_array
-
-def get_tree_height(node):
-    &#39;&#39;&#39; calculate the height of a binary tree &#39;&#39;&#39;
-    if node is None:
-        return 0
-    else:
-        return max(get_tree_height(node.left) + 1, get_tree_height(node.right) + 1)
-
-def fill_complete_tree(tree):
-    &#39;&#39;&#39; make a binary tree a complete tree &#39;&#39;&#39;
-    tree_array = tree_to_array(tree.root)
-    tree_height = get_tree_height(tree.root)
-
-    # build empty complete tree
-    array_size = (2 ** tree_height) - 1
-    new_tree = [ &#34;&#34; ] * array_size
-
-    # fill the complete tree array
-    for index, value in tree_array:
-        new_tree[index] = value
-    return new_tree
-
-def tree_print(tree):
-    &#39;&#39;&#39; pretty print a binary tree &#39;&#39;&#39;
-    complete_tree = fill_complete_tree(tree)
-    heap_print(complete_tree)</code></pre>
+def rand_int_array(n: int, maxnum: int) -&gt; list:
+    &#34;&#34;&#34; 
+    return an array of n integers of random numbers from 0 to maxnum
+
+    Args:
+        n: the number of integers to generate
+        maxnum: the maximum number in a range (0-maxnum inclusive)
+    Returns:
+    array of n integers of random numbers from 0 to maxnum
+    &#34;&#34;&#34;
+    array = [None] * n
+    for i in range(n):
+        array[i] = random.randint(0, maxnum)
+    return array
+
+def filled_array(n):
+    &#34;&#34;&#34; 
+    return an array filled with integers from 0 to n-1
+
+    Args:
+        n: the number of integers to generate
+    Returns:
+    array filled with integers from 0 to n-1
+    &#34;&#34;&#34;
+    array = [None] * n
+    for i in range(n):
+        array[i] = i
+    return array    
+
+def shuffle_array(n):
+    &#34;&#34;&#34; 
+    return a shuffled array filled with integers from 0 to n-1
+
+    Args:
+        n: the number of integers to generate
+    Returns:
+    array shuffled with integers from 0 to n-1
+    &#34;&#34;&#34;
+    array = filled_array(n)
+    for i in range(n):
+        r = random.randint(i, n-1)
+        array[i], array[r] = array[r], array[i]
+    return array</code></pre>
 </details>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
 <h2 class="section-title" id="header-functions">Functions</h2>
 <dl>
-<dt id="dsa.pretty_print.fill_complete_tree"><code class="name flex">
-<span>def <span class="ident">fill_complete_tree</span></span>(<span>tree)</span>
+<dt id="dsa.sorttools.filled_array"><code class="name flex">
+<span>def <span class="ident">filled_array</span></span>(<span>n)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>make a binary tree a complete tree</p></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def fill_complete_tree(tree):
-    &#39;&#39;&#39; make a binary tree a complete tree &#39;&#39;&#39;
-    tree_array = tree_to_array(tree.root)
-    tree_height = get_tree_height(tree.root)
-
-    # build empty complete tree
-    array_size = (2 ** tree_height) - 1
-    new_tree = [ &#34;&#34; ] * array_size
-
-    # fill the complete tree array
-    for index, value in tree_array:
-        new_tree[index] = value
-    return new_tree</code></pre>
-</details>
-</dd>
-<dt id="dsa.pretty_print.get_tree_height"><code class="name flex">
-<span>def <span class="ident">get_tree_height</span></span>(<span>node)</span>
-</code></dt>
-<dd>
-<div class="desc"><p>calculate the height of a binary tree</p></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def get_tree_height(node):
-    &#39;&#39;&#39; calculate the height of a binary tree &#39;&#39;&#39;
-    if node is None:
-        return 0
-    else:
-        return max(get_tree_height(node.left) + 1, get_tree_height(node.right) + 1)</code></pre>
-</details>
-</dd>
-<dt id="dsa.pretty_print.heap_print"><code class="name flex">
-<span>def <span class="ident">heap_print</span></span>(<span>heap)</span>
-</code></dt>
-<dd>
-<div class="desc"><p>print a heap</p></div>
+<div class="desc"><p>return an array filled with integers from 0 to n-1</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>n</code></strong></dt>
+<dd>the number of integers to generate</dd>
+</dl>
+<p>Returns:
+array filled with integers from 0 to n-1</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def heap_print(heap):
-    &#39;&#39;&#39; print a heap &#39;&#39;&#39;
-    if len(heap) == 0:
-        return
-    height = math.floor(math.log2(len(heap)))
-    level_str = &#34;&#34;
-    current_level = 0
-    value_width = 3
-    max_width = 2 ** (height - 1) * value_width
-
-    for index, node in enumerate(heap):
-        level = int(math.log2(index + 1))
-        columns = 2 ** (level - 1)
-        column_width = int(max_width / columns)
-        if current_level != level:
-            current_level = level
-            print(level_str)
-            level_str = &#34;&#34;
-        level_str += f&#34;{node:^{column_width}}&#34;
-    print(level_str)
-    print()</code></pre>
+<pre><code class="python">def filled_array(n):
+    &#34;&#34;&#34; 
+    return an array filled with integers from 0 to n-1
+
+    Args:
+        n: the number of integers to generate
+    Returns:
+    array filled with integers from 0 to n-1
+    &#34;&#34;&#34;
+    array = [None] * n
+    for i in range(n):
+        array[i] = i
+    return array    </code></pre>
 </details>
 </dd>
-<dt id="dsa.pretty_print.tree_print"><code class="name flex">
-<span>def <span class="ident">tree_print</span></span>(<span>tree)</span>
+<dt id="dsa.sorttools.rand_int_array"><code class="name flex">
+<span>def <span class="ident">rand_int_array</span></span>(<span>n: int, maxnum: int) ‑> list</span>
 </code></dt>
 <dd>
-<div class="desc"><p>pretty print a binary tree</p></div>
+<div class="desc"><p>return an array of n integers of random numbers from 0 to maxnum</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>n</code></strong></dt>
+<dd>the number of integers to generate</dd>
+<dt><strong><code>maxnum</code></strong></dt>
+<dd>the maximum number in a range (0-maxnum inclusive)</dd>
+</dl>
+<p>Returns:
+array of n integers of random numbers from 0 to maxnum</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def tree_print(tree):
-    &#39;&#39;&#39; pretty print a binary tree &#39;&#39;&#39;
-    complete_tree = fill_complete_tree(tree)
-    heap_print(complete_tree)</code></pre>
+<pre><code class="python">def rand_int_array(n: int, maxnum: int) -&gt; list:
+    &#34;&#34;&#34; 
+    return an array of n integers of random numbers from 0 to maxnum
+
+    Args:
+        n: the number of integers to generate
+        maxnum: the maximum number in a range (0-maxnum inclusive)
+    Returns:
+    array of n integers of random numbers from 0 to maxnum
+    &#34;&#34;&#34;
+    array = [None] * n
+    for i in range(n):
+        array[i] = random.randint(0, maxnum)
+    return array</code></pre>
 </details>
 </dd>
-<dt id="dsa.pretty_print.tree_to_array"><code class="name flex">
-<span>def <span class="ident">tree_to_array</span></span>(<span>node, index=0, tree_array=None)</span>
+<dt id="dsa.sorttools.shuffle_array"><code class="name flex">
+<span>def <span class="ident">shuffle_array</span></span>(<span>n)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>create an array filled with index and value pairs from a node based tree</p></div>
+<div class="desc"><p>return a shuffled array filled with integers from 0 to n-1</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>n</code></strong></dt>
+<dd>the number of integers to generate</dd>
+</dl>
+<p>Returns:
+array shuffled with integers from 0 to n-1</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def tree_to_array(node, index=0, tree_array=None):
-    &#39;&#39;&#39; create an array filled with index and value pairs from a node based tree &#39;&#39;&#39;
-    if not tree_array:
-        tree_array = []
-    if node is None:
-        return
-    tree_array.append((index, node.value))
-    tree_to_array(node.left, index * 2 + 1, tree_array)
-    tree_to_array(node.right, index * 2 + 2, tree_array)
-    
-    return tree_array</code></pre>
+<pre><code class="python">def shuffle_array(n):
+    &#34;&#34;&#34; 
+    return a shuffled array filled with integers from 0 to n-1
+
+    Args:
+        n: the number of integers to generate
+    Returns:
+    array shuffled with integers from 0 to n-1
+    &#34;&#34;&#34;
+    array = filled_array(n)
+    for i in range(n):
+        r = random.randint(i, n-1)
+        array[i], array[r] = array[r], array[i]
+    return array</code></pre>
 </details>
 </dd>
 </dl>
 </section>
 <section>
 </section>
 </article>
@@ -221,19 +193,17 @@
 <li><h3>Super-module</h3>
 <ul>
 <li><code><a title="dsa" href="index.html">dsa</a></code></li>
 </ul>
 </li>
 <li><h3><a href="#header-functions">Functions</a></h3>
 <ul class="">
-<li><code><a title="dsa.pretty_print.fill_complete_tree" href="#dsa.pretty_print.fill_complete_tree">fill_complete_tree</a></code></li>
-<li><code><a title="dsa.pretty_print.get_tree_height" href="#dsa.pretty_print.get_tree_height">get_tree_height</a></code></li>
-<li><code><a title="dsa.pretty_print.heap_print" href="#dsa.pretty_print.heap_print">heap_print</a></code></li>
-<li><code><a title="dsa.pretty_print.tree_print" href="#dsa.pretty_print.tree_print">tree_print</a></code></li>
-<li><code><a title="dsa.pretty_print.tree_to_array" href="#dsa.pretty_print.tree_to_array">tree_to_array</a></code></li>
+<li><code><a title="dsa.sorttools.filled_array" href="#dsa.sorttools.filled_array">filled_array</a></code></li>
+<li><code><a title="dsa.sorttools.rand_int_array" href="#dsa.sorttools.rand_int_array">rand_int_array</a></code></li>
+<li><code><a title="dsa.sorttools.shuffle_array" href="#dsa.sorttools.shuffle_array">shuffle_array</a></code></li>
 </ul>
 </li>
 </ul>
 </nav>
 </main>
 <footer id="footer">
 <p>Generated by <a href="https://pdoc3.github.io/pdoc" title="pdoc: Python API documentation generator"><cite>pdoc</cite> 0.10.0</a>.</p>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,149 +1,122 @@
-************ MMoodduullee ddssaa..pprreettttyy__pprriinntt ************
+************ MMoodduullee ddssaa..ssoorrttttoooollss ************
+a collection of functions for sort benchmarks
 Expand source code
-import math
+""" a collection of functions for sort benchmarks """
+import random
 
-def heap_print(heap):
-    ''' print a heap '''
-    if len(heap) == 0:
-        return
-    height = math.floor(math.log2(len(heap)))
-    level_str = ""
-    current_level = 0
-    value_width = 3
-    max_width = 2 ** (height - 1) * value_width
-
-    for index, node in enumerate(heap):
-        level = int(math.log2(index + 1))
-        columns = 2 ** (level - 1)
-        column_width = int(max_width / columns)
-        if current_level != level:
-            current_level = level
-            print(level_str)
-            level_str = ""
-        level_str += f"{node:^{column_width}}"
-    print(level_str)
-    print()
-
-
-def tree_to_array(node, index=0, tree_array=None):
-    ''' create an array filled with index and value pairs from a node based
-tree '''
-    if not tree_array:
-        tree_array = []
-    if node is None:
-        return
-    tree_array.append((index, node.value))
-    tree_to_array(node.left, index * 2 + 1, tree_array)
-    tree_to_array(node.right, index * 2 + 2, tree_array)
-
-    return tree_array
-
-def get_tree_height(node):
-    ''' calculate the height of a binary tree '''
-    if node is None:
-        return 0
-    else:
-        return max(get_tree_height(node.left) + 1, get_tree_height(node.right)
-+ 1)
-
-def fill_complete_tree(tree):
-    ''' make a binary tree a complete tree '''
-    tree_array = tree_to_array(tree.root)
-    tree_height = get_tree_height(tree.root)
-
-    # build empty complete tree
-    array_size = (2 ** tree_height) - 1
-    new_tree = [ "" ] * array_size
-
-    # fill the complete tree array
-    for index, value in tree_array:
-        new_tree[index] = value
-    return new_tree
-
-def tree_print(tree):
-    ''' pretty print a binary tree '''
-    complete_tree = fill_complete_tree(tree)
-    heap_print(complete_tree)
+def rand_int_array(n: int, maxnum: int) -> list:
+    """
+    return an array of n integers of random numbers from 0 to maxnum
+
+    Args:
+        n: the number of integers to generate
+        maxnum: the maximum number in a range (0-maxnum inclusive)
+    Returns:
+    array of n integers of random numbers from 0 to maxnum
+    """
+    array = [None] * n
+    for i in range(n):
+        array[i] = random.randint(0, maxnum)
+    return array
+
+def filled_array(n):
+    """
+    return an array filled with integers from 0 to n-1
+
+    Args:
+        n: the number of integers to generate
+    Returns:
+    array filled with integers from 0 to n-1
+    """
+    array = [None] * n
+    for i in range(n):
+        array[i] = i
+    return array
+
+def shuffle_array(n):
+    """
+    return a shuffled array filled with integers from 0 to n-1
+
+    Args:
+        n: the number of integers to generate
+    Returns:
+    array shuffled with integers from 0 to n-1
+    """
+    array = filled_array(n)
+    for i in range(n):
+        r = random.randint(i, n-1)
+        array[i], array[r] = array[r], array[i]
+    return array
 ********** FFuunnccttiioonnss **********
-  def fill_complete_tree(tree)
-      make a binary tree a complete tree
+  def filled_array(n)
+      return an array filled with integers from 0 to n-1
+      ********** AArrggss **********
+        nn
+            the number of integers to generate
+      Returns: array filled with integers from 0 to n-1
       Expand source code
-      def fill_complete_tree(tree):
-          ''' make a binary tree a complete tree '''
-          tree_array = tree_to_array(tree.root)
-          tree_height = get_tree_height(tree.root)
-
-          # build empty complete tree
-          array_size = (2 ** tree_height) - 1
-          new_tree = [ "" ] * array_size
-
-          # fill the complete tree array
-          for index, value in tree_array:
-              new_tree[index] = value
-          return new_tree
-  def get_tree_height(node)
-      calculate the height of a binary tree
+      def filled_array(n):
+          """
+          return an array filled with integers from 0 to n-1
+
+          Args:
+              n: the number of integers to generate
+          Returns:
+          array filled with integers from 0 to n-1
+          """
+          array = [None] * n
+          for i in range(n):
+              array[i] = i
+          return array
+  def rand_int_array(n: int, maxnum: int) ‑> list
+      return an array of n integers of random numbers from 0 to maxnum
+      ********** AArrggss **********
+        nn
+            the number of integers to generate
+        mmaaxxnnuumm
+            the maximum number in a range (0-maxnum inclusive)
+      Returns: array of n integers of random numbers from 0 to maxnum
       Expand source code
-      def get_tree_height(node):
-          ''' calculate the height of a binary tree '''
-          if node is None:
-              return 0
-          else:
-              return max(get_tree_height(node.left) + 1, get_tree_height
-      (node.right) + 1)
-  def heap_print(heap)
-      print a heap
+      def rand_int_array(n: int, maxnum: int) -> list:
+          """
+          return an array of n integers of random numbers from 0 to maxnum
+
+          Args:
+              n: the number of integers to generate
+              maxnum: the maximum number in a range (0-maxnum inclusive)
+          Returns:
+          array of n integers of random numbers from 0 to maxnum
+          """
+          array = [None] * n
+          for i in range(n):
+              array[i] = random.randint(0, maxnum)
+          return array
+  def shuffle_array(n)
+      return a shuffled array filled with integers from 0 to n-1
+      ********** AArrggss **********
+        nn
+            the number of integers to generate
+      Returns: array shuffled with integers from 0 to n-1
       Expand source code
-      def heap_print(heap):
-          ''' print a heap '''
-          if len(heap) == 0:
-              return
-          height = math.floor(math.log2(len(heap)))
-          level_str = ""
-          current_level = 0
-          value_width = 3
-          max_width = 2 ** (height - 1) * value_width
-
-          for index, node in enumerate(heap):
-              level = int(math.log2(index + 1))
-              columns = 2 ** (level - 1)
-              column_width = int(max_width / columns)
-              if current_level != level:
-                  current_level = level
-                  print(level_str)
-                  level_str = ""
-              level_str += f"{node:^{column_width}}"
-          print(level_str)
-          print()
-  def tree_print(tree)
-      pretty print a binary tree
-      Expand source code
-      def tree_print(tree):
-          ''' pretty print a binary tree '''
-          complete_tree = fill_complete_tree(tree)
-          heap_print(complete_tree)
-  def tree_to_array(node, index=0, tree_array=None)
-      create an array filled with index and value pairs from a node based tree
-      Expand source code
-      def tree_to_array(node, index=0, tree_array=None):
-          ''' create an array filled with index and value pairs from a node
-      based tree '''
-          if not tree_array:
-              tree_array = []
-          if node is None:
-              return
-          tree_array.append((index, node.value))
-          tree_to_array(node.left, index * 2 + 1, tree_array)
-          tree_to_array(node.right, index * 2 + 2, tree_array)
-
-          return tree_array
+      def shuffle_array(n):
+          """
+          return a shuffled array filled with integers from 0 to n-1
+
+          Args:
+              n: the number of integers to generate
+          Returns:
+          array shuffled with integers from 0 to n-1
+          """
+          array = filled_array(n)
+          for i in range(n):
+              r = random.randint(i, n-1)
+              array[i], array[r] = array[r], array[i]
+          return array
 ************ IInnddeexx ************
     * ******** SSuuppeerr--mmoodduullee ********
           o _d_s_a
     * ******** _FF_uu_nn_cc_tt_ii_oo_nn_ss ********
-          o _f_i_l_l___c_o_m_p_l_e_t_e___t_r_e_e
-          o _g_e_t___t_r_e_e___h_e_i_g_h_t
-          o _h_e_a_p___p_r_i_n_t
-          o _t_r_e_e___p_r_i_n_t
-          o _t_r_e_e___t_o___a_r_r_a_y
+          o _f_i_l_l_e_d___a_r_r_a_y
+          o _r_a_n_d___i_n_t___a_r_r_a_y
+          o _s_h_u_f_f_l_e___a_r_r_a_y
 Generated by_p_d_o_c_0_._1_0_._0.
```

### Comparing `ucxdsa-2024.4.23/src/html/dsa/queue.html` & `ucxdsa-2024.5.9/src/html/dsa/tree.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,510 +1,663 @@
 <!doctype html>
 <html lang="en">
 <head>
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
 <meta name="generator" content="pdoc 0.10.0" />
-<title>dsa.queue API documentation</title>
+<title>dsa.tree API documentation</title>
 <meta name="description" content="" />
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
 <link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
 <link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
 <style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
 <style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
 <style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
 <script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
 <script>window.addEventListener('DOMContentLoaded', () => hljs.initHighlighting())</script>
 </head>
 <body>
 <main>
 <article id="content">
 <header>
-<h1 class="title">Module <code>dsa.queue</code></h1>
+<h1 class="title">Module <code>dsa.tree</code></h1>
 </header>
 <section id="section-intro">
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">class Queue:
+<pre><code class="python">class Node:
     &#34;&#34;&#34; 
-    A static queue implementation in Python
+    A binary tree node implementation in Python
     &#34;&#34;&#34;
-    def __init__(self, capacity=10):
+    def __init__(self, value, left=None, right=None):
         &#34;&#34;&#34; 
         Args:
-            capacity: the initial size of the stack (defaults to 10)
-        &#34;&#34;&#34;
-        self._array = [None] * capacity
-        self._front = 0
-        #: number of elements in queue
-        self.count = 0
-    
-    def enqueue(self, element):
+            value: value of the node
+            left: left node
+            right: right node
+        &#34;&#34;&#34;
+        self.value = value
+        self.left = left
+        self.right = right
+
+    def print(self, level=0):
+        &#34;&#34;&#34; 
+        Print the contents of a node.
+
+        Args:
+            level: starting level of node
         &#34;&#34;&#34;
-        Enqueue an element into the queue. Raise Exception when trying to enqueue more elements than the capacity.
+        if self.right:
+            self.right.print(level + 1)
+        print(&#34;   &#34; * level + str(self.value))
+        if self.left:
+            self.left.print(level + 1)
 
+class Tree:
+    &#34;&#34;&#34; 
+    A binary search tree implementation in Python
+    &#34;&#34;&#34;
+    def __init__(self, root=None):
+        &#34;&#34;&#34; 
         Args:
-            element: the element to enqueue
+            root: root node of the BST
         &#34;&#34;&#34;
-        if self.count &gt;= len(self._array):
-            raise Exception(&#34;Capacity Reached&#34;)
+        self.root = root
+        
+    def search(self, value):
+        &#34;&#34;&#34; 
+        Search for a value in the binary search tree.
 
-        index = (self._front + self.count) % len(self._array)
-        self._array[index] = element
-        self.count += 1
+        Args:
+            value: value to search for
         
-    def dequeue(self):
+        Returns:
+        node with matching value
+        None if not found
         &#34;&#34;&#34;
-        Dequeue an element from the queue. Raise Exception when there are no elements to dequeue.
+        current = self.root
+        
+        while current is not None:
+            if value == current.value:
+                return current
+            elif value &lt; current.value:
+                current = current.left
+            elif value &gt; current.value:
+                current = current.right
+            else:
+                return None
+        
+        return None
+    
+    def insert(self, value):
+        &#34;&#34;&#34; 
+        Insert a value in the binary search tree.
 
+        Args:
+            value: value to insert
+        
         Returns:
-            the from element in the queue
+        None
         &#34;&#34;&#34;
-        if self.is_empty():
-            raise Exception(&#34;Empty Queue&#34;)
-
-        element = self._array[self._front]
-        self._front += 1
-        if self._front &gt;= len(self._array):
-            self._front = 0
-        self.count -= 1
+        current = self.root
+        if self.root is None:
+            self.root = Node(value)
+            return
+        
+        while current is not None:
+            if value &lt; current.value:
+                if current.left is None:
+                    current.left = Node(value)
+                    return
+                else:
+                    current = current.left
+            elif value &gt; current.value:
+                if current.right is None:
+                    current.right = Node(value)
+                    return
+                else:
+                    current = current.right
+            else:
+                return 
+   
+    def delete(self, value):
+        &#34;&#34;&#34; 
+        Delete a value from the binary search tree.
 
-        return element
-    
-    def peek(self):
-        &#34;&#34;&#34;
-        Return the element in front of the queue. Raise Exception if queue is empty.
+        Args:
+            value: value to delete
+        
+        Returns:
+        None
         &#34;&#34;&#34;
-        if self.is_empty():
-            raise Exception(&#34;Empty Queue&#34;)
-
-        return self._array[self._front]
+        return self.delete_node(value, self.root)
+        
+    def delete_node(self, value, node):
+        &#34;&#34;&#34; 
+        Helper function to delete a value from the binary search tree. (Use delete() instead)
 
-    def is_empty(self):
-        &#34;&#34;&#34;
-        Return a Boolean on whether the stack is empty or not.
-        &#34;&#34;&#34;
-        return self.count == 0
-    
-    def capacity(self):
-        &#34;&#34;&#34;
-        Return the capacity of the queue.
+        Args:
+            value: value to delete
+            node: current node
         &#34;&#34;&#34;
-        return len(self._array)
-
-    def __repr__(self):
-        arr = []
-        for i in range(self.count):
-            index = (i + self._front) % len(self._array)
-            arr.append(str(self._array[index]))
-        arrstr = &#34;, &#34;.join(arr)
-        return f&#34;[{arrstr}] Front: {self._front} count: {self.count} Capacity: {self.capacity()}&#34;
-    
-
-# shrink not implemented
-class DynamicQueue(Queue):
-    &#34;&#34;&#34; 
-    A dynamic queue implementation in Python
-    &#34;&#34;&#34;
-    def __init__(self, capacity=10):
-        super().__init__(capacity)
+        if node is None:
+            return None
+        
+        if value &lt; node.value:
+            node.left = self.delete_node(value, node.left)
+        elif value &gt; node.value:
+            node.right = self.delete_node(value, node.right)
+        else:
+            if node.left is None:
+                branch = node.right
+                node = None
+                return branch
+            elif node.right is None:
+                branch = node.left
+                node = None
+                return branch
+            
+            branch = self.min_node(node.right)
+            node.value = branch.value
+            node.right = self.delete_node(branch.value, node.right)
+            
+        return node
     
-    def grow(self):
+    def min_node(self, node=None):
         &#34;&#34;&#34; 
-        double the capacity of the current array 
+        Return the node with the minimum value in a binary search tree.
+
+        Args:
+            node: starting node
+        
+        Returns:
+        node with the lowest value in the BST
+        None if not found
         &#34;&#34;&#34;
-        new_array = [ None ] * len(self._array) * 2
+        if node is None:
+            node = self.root
         
-        # copy elements
-        for i in range(self.count):
-            new_array[i] = self._array[i + self._front]
-        self._front = 0
-        self._array = new_array
-
-    def check_capacity(self):
+        if node.left is None:
+            return node
+        else:
+            return self.min_node(node.left)
+    
+    def print(self):
         &#34;&#34;&#34; 
-        if count &gt;= capacity, grow the array
-        &#34;&#34;&#34;
-        if self._front + self.count &gt;= len(self._array):
-            self.grow()
-
-    def enqueue(self, element):
-        &#34;&#34;&#34;
-        Enqueue an element into the queue. Increae capacity if count is greater than the capacity.
+        Print the values in the BST.
 
-        Args:
-            element: the element to enqueue
         &#34;&#34;&#34;
-        self.check_capacity()
-        index = self._front + self.count
-        self._array[index] = element
-        self.count += 1</code></pre>
+        self.root.print()
+        
+        </code></pre>
 </details>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
 <h2 class="section-title" id="header-classes">Classes</h2>
 <dl>
-<dt id="dsa.queue.DynamicQueue"><code class="flex name class">
-<span>class <span class="ident">DynamicQueue</span></span>
-<span>(</span><span>capacity=10)</span>
+<dt id="dsa.tree.Node"><code class="flex name class">
+<span>class <span class="ident">Node</span></span>
+<span>(</span><span>value, left=None, right=None)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>A dynamic queue implementation in Python</p>
+<div class="desc"><p>A binary tree node implementation in Python</p>
 <h2 id="args">Args</h2>
 <dl>
-<dt><strong><code>capacity</code></strong></dt>
-<dd>the initial size of the stack (defaults to 10)</dd>
+<dt><strong><code>value</code></strong></dt>
+<dd>value of the node</dd>
+<dt><strong><code>left</code></strong></dt>
+<dd>left node</dd>
+<dt><strong><code>right</code></strong></dt>
+<dd>right node</dd>
 </dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">class DynamicQueue(Queue):
+<pre><code class="python">class Node:
     &#34;&#34;&#34; 
-    A dynamic queue implementation in Python
+    A binary tree node implementation in Python
     &#34;&#34;&#34;
-    def __init__(self, capacity=10):
-        super().__init__(capacity)
-    
-    def grow(self):
+    def __init__(self, value, left=None, right=None):
         &#34;&#34;&#34; 
-        double the capacity of the current array 
-        &#34;&#34;&#34;
-        new_array = [ None ] * len(self._array) * 2
-        
-        # copy elements
-        for i in range(self.count):
-            new_array[i] = self._array[i + self._front]
-        self._front = 0
-        self._array = new_array
+        Args:
+            value: value of the node
+            left: left node
+            right: right node
+        &#34;&#34;&#34;
+        self.value = value
+        self.left = left
+        self.right = right
 
-    def check_capacity(self):
+    def print(self, level=0):
         &#34;&#34;&#34; 
-        if count &gt;= capacity, grow the array
-        &#34;&#34;&#34;
-        if self._front + self.count &gt;= len(self._array):
-            self.grow()
-
-    def enqueue(self, element):
-        &#34;&#34;&#34;
-        Enqueue an element into the queue. Increae capacity if count is greater than the capacity.
+        Print the contents of a node.
 
         Args:
-            element: the element to enqueue
+            level: starting level of node
         &#34;&#34;&#34;
-        self.check_capacity()
-        index = self._front + self.count
-        self._array[index] = element
-        self.count += 1</code></pre>
+        if self.right:
+            self.right.print(level + 1)
+        print(&#34;   &#34; * level + str(self.value))
+        if self.left:
+            self.left.print(level + 1)</code></pre>
 </details>
-<h3>Ancestors</h3>
-<ul class="hlist">
-<li><a title="dsa.queue.Queue" href="#dsa.queue.Queue">Queue</a></li>
-</ul>
 <h3>Methods</h3>
 <dl>
-<dt id="dsa.queue.DynamicQueue.check_capacity"><code class="name flex">
-<span>def <span class="ident">check_capacity</span></span>(<span>self)</span>
-</code></dt>
-<dd>
-<div class="desc"><p>if count &gt;= capacity, grow the array</p></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def check_capacity(self):
-    &#34;&#34;&#34; 
-    if count &gt;= capacity, grow the array
-    &#34;&#34;&#34;
-    if self._front + self.count &gt;= len(self._array):
-        self.grow()</code></pre>
-</details>
-</dd>
-<dt id="dsa.queue.DynamicQueue.enqueue"><code class="name flex">
-<span>def <span class="ident">enqueue</span></span>(<span>self, element)</span>
+<dt id="dsa.tree.Node.print"><code class="name flex">
+<span>def <span class="ident">print</span></span>(<span>self, level=0)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Enqueue an element into the queue. Increae capacity if count is greater than the capacity.</p>
+<div class="desc"><p>Print the contents of a node.</p>
 <h2 id="args">Args</h2>
 <dl>
-<dt><strong><code>element</code></strong></dt>
-<dd>the element to enqueue</dd>
+<dt><strong><code>level</code></strong></dt>
+<dd>starting level of node</dd>
 </dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def enqueue(self, element):
-    &#34;&#34;&#34;
-    Enqueue an element into the queue. Increae capacity if count is greater than the capacity.
+<pre><code class="python">def print(self, level=0):
+    &#34;&#34;&#34; 
+    Print the contents of a node.
 
     Args:
-        element: the element to enqueue
+        level: starting level of node
     &#34;&#34;&#34;
-    self.check_capacity()
-    index = self._front + self.count
-    self._array[index] = element
-    self.count += 1</code></pre>
-</details>
-</dd>
-<dt id="dsa.queue.DynamicQueue.grow"><code class="name flex">
-<span>def <span class="ident">grow</span></span>(<span>self)</span>
-</code></dt>
-<dd>
-<div class="desc"><p>double the capacity of the current array</p></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def grow(self):
-    &#34;&#34;&#34; 
-    double the capacity of the current array 
-    &#34;&#34;&#34;
-    new_array = [ None ] * len(self._array) * 2
-    
-    # copy elements
-    for i in range(self.count):
-        new_array[i] = self._array[i + self._front]
-    self._front = 0
-    self._array = new_array</code></pre>
+    if self.right:
+        self.right.print(level + 1)
+    print(&#34;   &#34; * level + str(self.value))
+    if self.left:
+        self.left.print(level + 1)</code></pre>
 </details>
 </dd>
 </dl>
-<h3>Inherited members</h3>
-<ul class="hlist">
-<li><code><b><a title="dsa.queue.Queue" href="#dsa.queue.Queue">Queue</a></b></code>:
-<ul class="hlist">
-<li><code><a title="dsa.queue.Queue.capacity" href="#dsa.queue.Queue.capacity">capacity</a></code></li>
-<li><code><a title="dsa.queue.Queue.count" href="#dsa.queue.Queue.count">count</a></code></li>
-<li><code><a title="dsa.queue.Queue.dequeue" href="#dsa.queue.Queue.dequeue">dequeue</a></code></li>
-<li><code><a title="dsa.queue.Queue.is_empty" href="#dsa.queue.Queue.is_empty">is_empty</a></code></li>
-<li><code><a title="dsa.queue.Queue.peek" href="#dsa.queue.Queue.peek">peek</a></code></li>
-</ul>
-</li>
-</ul>
 </dd>
-<dt id="dsa.queue.Queue"><code class="flex name class">
-<span>class <span class="ident">Queue</span></span>
-<span>(</span><span>capacity=10)</span>
+<dt id="dsa.tree.Tree"><code class="flex name class">
+<span>class <span class="ident">Tree</span></span>
+<span>(</span><span>root=None)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>A static queue implementation in Python</p>
+<div class="desc"><p>A binary search tree implementation in Python</p>
 <h2 id="args">Args</h2>
 <dl>
-<dt><strong><code>capacity</code></strong></dt>
-<dd>the initial size of the stack (defaults to 10)</dd>
+<dt><strong><code>root</code></strong></dt>
+<dd>root node of the BST</dd>
 </dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">class Queue:
+<pre><code class="python">class Tree:
     &#34;&#34;&#34; 
-    A static queue implementation in Python
+    A binary search tree implementation in Python
     &#34;&#34;&#34;
-    def __init__(self, capacity=10):
+    def __init__(self, root=None):
         &#34;&#34;&#34; 
         Args:
-            capacity: the initial size of the stack (defaults to 10)
+            root: root node of the BST
         &#34;&#34;&#34;
-        self._array = [None] * capacity
-        self._front = 0
-        #: number of elements in queue
-        self.count = 0
-    
-    def enqueue(self, element):
-        &#34;&#34;&#34;
-        Enqueue an element into the queue. Raise Exception when trying to enqueue more elements than the capacity.
+        self.root = root
+        
+    def search(self, value):
+        &#34;&#34;&#34; 
+        Search for a value in the binary search tree.
 
         Args:
-            element: the element to enqueue
+            value: value to search for
+        
+        Returns:
+        node with matching value
+        None if not found
         &#34;&#34;&#34;
-        if self.count &gt;= len(self._array):
-            raise Exception(&#34;Capacity Reached&#34;)
+        current = self.root
+        
+        while current is not None:
+            if value == current.value:
+                return current
+            elif value &lt; current.value:
+                current = current.left
+            elif value &gt; current.value:
+                current = current.right
+            else:
+                return None
+        
+        return None
+    
+    def insert(self, value):
+        &#34;&#34;&#34; 
+        Insert a value in the binary search tree.
 
-        index = (self._front + self.count) % len(self._array)
-        self._array[index] = element
-        self.count += 1
+        Args:
+            value: value to insert
         
-    def dequeue(self):
+        Returns:
+        None
         &#34;&#34;&#34;
-        Dequeue an element from the queue. Raise Exception when there are no elements to dequeue.
+        current = self.root
+        if self.root is None:
+            self.root = Node(value)
+            return
+        
+        while current is not None:
+            if value &lt; current.value:
+                if current.left is None:
+                    current.left = Node(value)
+                    return
+                else:
+                    current = current.left
+            elif value &gt; current.value:
+                if current.right is None:
+                    current.right = Node(value)
+                    return
+                else:
+                    current = current.right
+            else:
+                return 
+   
+    def delete(self, value):
+        &#34;&#34;&#34; 
+        Delete a value from the binary search tree.
 
+        Args:
+            value: value to delete
+        
         Returns:
-            the from element in the queue
+        None
         &#34;&#34;&#34;
-        if self.is_empty():
-            raise Exception(&#34;Empty Queue&#34;)
-
-        element = self._array[self._front]
-        self._front += 1
-        if self._front &gt;= len(self._array):
-            self._front = 0
-        self.count -= 1
+        return self.delete_node(value, self.root)
+        
+    def delete_node(self, value, node):
+        &#34;&#34;&#34; 
+        Helper function to delete a value from the binary search tree. (Use delete() instead)
 
-        return element
-    
-    def peek(self):
-        &#34;&#34;&#34;
-        Return the element in front of the queue. Raise Exception if queue is empty.
+        Args:
+            value: value to delete
+            node: current node
         &#34;&#34;&#34;
-        if self.is_empty():
-            raise Exception(&#34;Empty Queue&#34;)
-
-        return self._array[self._front]
+        if node is None:
+            return None
+        
+        if value &lt; node.value:
+            node.left = self.delete_node(value, node.left)
+        elif value &gt; node.value:
+            node.right = self.delete_node(value, node.right)
+        else:
+            if node.left is None:
+                branch = node.right
+                node = None
+                return branch
+            elif node.right is None:
+                branch = node.left
+                node = None
+                return branch
+            
+            branch = self.min_node(node.right)
+            node.value = branch.value
+            node.right = self.delete_node(branch.value, node.right)
+            
+        return node
+    
+    def min_node(self, node=None):
+        &#34;&#34;&#34; 
+        Return the node with the minimum value in a binary search tree.
 
-    def is_empty(self):
-        &#34;&#34;&#34;
-        Return a Boolean on whether the stack is empty or not.
+        Args:
+            node: starting node
+        
+        Returns:
+        node with the lowest value in the BST
+        None if not found
         &#34;&#34;&#34;
-        return self.count == 0
+        if node is None:
+            node = self.root
+        
+        if node.left is None:
+            return node
+        else:
+            return self.min_node(node.left)
     
-    def capacity(self):
-        &#34;&#34;&#34;
-        Return the capacity of the queue.
-        &#34;&#34;&#34;
-        return len(self._array)
+    def print(self):
+        &#34;&#34;&#34; 
+        Print the values in the BST.
 
-    def __repr__(self):
-        arr = []
-        for i in range(self.count):
-            index = (i + self._front) % len(self._array)
-            arr.append(str(self._array[index]))
-        arrstr = &#34;, &#34;.join(arr)
-        return f&#34;[{arrstr}] Front: {self._front} count: {self.count} Capacity: {self.capacity()}&#34;</code></pre>
+        &#34;&#34;&#34;
+        self.root.print()</code></pre>
 </details>
-<h3>Subclasses</h3>
-<ul class="hlist">
-<li><a title="dsa.queue.DynamicQueue" href="#dsa.queue.DynamicQueue">DynamicQueue</a></li>
-</ul>
-<h3>Instance variables</h3>
-<dl>
-<dt id="dsa.queue.Queue.count"><code class="name">var <span class="ident">count</span></code></dt>
-<dd>
-<div class="desc"><p>number of elements in queue</p></div>
-</dd>
-</dl>
 <h3>Methods</h3>
 <dl>
-<dt id="dsa.queue.Queue.capacity"><code class="name flex">
-<span>def <span class="ident">capacity</span></span>(<span>self)</span>
+<dt id="dsa.tree.Tree.delete"><code class="name flex">
+<span>def <span class="ident">delete</span></span>(<span>self, value)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Return the capacity of the queue.</p></div>
+<div class="desc"><p>Delete a value from the binary search tree.</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>value</code></strong></dt>
+<dd>value to delete</dd>
+</dl>
+<p>Returns:
+None</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def capacity(self):
-    &#34;&#34;&#34;
-    Return the capacity of the queue.
+<pre><code class="python">def delete(self, value):
+    &#34;&#34;&#34; 
+    Delete a value from the binary search tree.
+
+    Args:
+        value: value to delete
+    
+    Returns:
+    None
     &#34;&#34;&#34;
-    return len(self._array)</code></pre>
+    return self.delete_node(value, self.root)</code></pre>
 </details>
 </dd>
-<dt id="dsa.queue.Queue.dequeue"><code class="name flex">
-<span>def <span class="ident">dequeue</span></span>(<span>self)</span>
+<dt id="dsa.tree.Tree.delete_node"><code class="name flex">
+<span>def <span class="ident">delete_node</span></span>(<span>self, value, node)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Dequeue an element from the queue. Raise Exception when there are no elements to dequeue.</p>
-<h2 id="returns">Returns</h2>
-<p>the from element in the queue</p></div>
+<div class="desc"><p>Helper function to delete a value from the binary search tree. (Use delete() instead)</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>value</code></strong></dt>
+<dd>value to delete</dd>
+<dt><strong><code>node</code></strong></dt>
+<dd>current node</dd>
+</dl></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def dequeue(self):
+<pre><code class="python">def delete_node(self, value, node):
+    &#34;&#34;&#34; 
+    Helper function to delete a value from the binary search tree. (Use delete() instead)
+
+    Args:
+        value: value to delete
+        node: current node
     &#34;&#34;&#34;
-    Dequeue an element from the queue. Raise Exception when there are no elements to dequeue.
+    if node is None:
+        return None
+    
+    if value &lt; node.value:
+        node.left = self.delete_node(value, node.left)
+    elif value &gt; node.value:
+        node.right = self.delete_node(value, node.right)
+    else:
+        if node.left is None:
+            branch = node.right
+            node = None
+            return branch
+        elif node.right is None:
+            branch = node.left
+            node = None
+            return branch
+        
+        branch = self.min_node(node.right)
+        node.value = branch.value
+        node.right = self.delete_node(branch.value, node.right)
+        
+    return node</code></pre>
+</details>
+</dd>
+<dt id="dsa.tree.Tree.insert"><code class="name flex">
+<span>def <span class="ident">insert</span></span>(<span>self, value)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Insert a value in the binary search tree.</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>value</code></strong></dt>
+<dd>value to insert</dd>
+</dl>
+<p>Returns:
+None</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def insert(self, value):
+    &#34;&#34;&#34; 
+    Insert a value in the binary search tree.
 
+    Args:
+        value: value to insert
+    
     Returns:
-        the from element in the queue
+    None
     &#34;&#34;&#34;
-    if self.is_empty():
-        raise Exception(&#34;Empty Queue&#34;)
-
-    element = self._array[self._front]
-    self._front += 1
-    if self._front &gt;= len(self._array):
-        self._front = 0
-    self.count -= 1
-
-    return element</code></pre>
+    current = self.root
+    if self.root is None:
+        self.root = Node(value)
+        return
+    
+    while current is not None:
+        if value &lt; current.value:
+            if current.left is None:
+                current.left = Node(value)
+                return
+            else:
+                current = current.left
+        elif value &gt; current.value:
+            if current.right is None:
+                current.right = Node(value)
+                return
+            else:
+                current = current.right
+        else:
+            return </code></pre>
 </details>
 </dd>
-<dt id="dsa.queue.Queue.enqueue"><code class="name flex">
-<span>def <span class="ident">enqueue</span></span>(<span>self, element)</span>
+<dt id="dsa.tree.Tree.min_node"><code class="name flex">
+<span>def <span class="ident">min_node</span></span>(<span>self, node=None)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Enqueue an element into the queue. Raise Exception when trying to enqueue more elements than the capacity.</p>
+<div class="desc"><p>Return the node with the minimum value in a binary search tree.</p>
 <h2 id="args">Args</h2>
 <dl>
-<dt><strong><code>element</code></strong></dt>
-<dd>the element to enqueue</dd>
-</dl></div>
+<dt><strong><code>node</code></strong></dt>
+<dd>starting node</dd>
+</dl>
+<p>Returns:
+node with the lowest value in the BST
+None if not found</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def enqueue(self, element):
-    &#34;&#34;&#34;
-    Enqueue an element into the queue. Raise Exception when trying to enqueue more elements than the capacity.
+<pre><code class="python">def min_node(self, node=None):
+    &#34;&#34;&#34; 
+    Return the node with the minimum value in a binary search tree.
 
     Args:
-        element: the element to enqueue
+        node: starting node
+    
+    Returns:
+    node with the lowest value in the BST
+    None if not found
     &#34;&#34;&#34;
-    if self.count &gt;= len(self._array):
-        raise Exception(&#34;Capacity Reached&#34;)
-
-    index = (self._front + self.count) % len(self._array)
-    self._array[index] = element
-    self.count += 1</code></pre>
+    if node is None:
+        node = self.root
+    
+    if node.left is None:
+        return node
+    else:
+        return self.min_node(node.left)</code></pre>
 </details>
 </dd>
-<dt id="dsa.queue.Queue.is_empty"><code class="name flex">
-<span>def <span class="ident">is_empty</span></span>(<span>self)</span>
+<dt id="dsa.tree.Tree.print"><code class="name flex">
+<span>def <span class="ident">print</span></span>(<span>self)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Return a Boolean on whether the stack is empty or not.</p></div>
+<div class="desc"><p>Print the values in the BST.</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def is_empty(self):
-    &#34;&#34;&#34;
-    Return a Boolean on whether the stack is empty or not.
+<pre><code class="python">def print(self):
+    &#34;&#34;&#34; 
+    Print the values in the BST.
+
     &#34;&#34;&#34;
-    return self.count == 0</code></pre>
+    self.root.print()</code></pre>
 </details>
 </dd>
-<dt id="dsa.queue.Queue.peek"><code class="name flex">
-<span>def <span class="ident">peek</span></span>(<span>self)</span>
+<dt id="dsa.tree.Tree.search"><code class="name flex">
+<span>def <span class="ident">search</span></span>(<span>self, value)</span>
 </code></dt>
 <dd>
-<div class="desc"><p>Return the element in front of the queue. Raise Exception if queue is empty.</p></div>
+<div class="desc"><p>Search for a value in the binary search tree.</p>
+<h2 id="args">Args</h2>
+<dl>
+<dt><strong><code>value</code></strong></dt>
+<dd>value to search for</dd>
+</dl>
+<p>Returns:
+node with matching value
+None if not found</p></div>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
-<pre><code class="python">def peek(self):
-    &#34;&#34;&#34;
-    Return the element in front of the queue. Raise Exception if queue is empty.
-    &#34;&#34;&#34;
-    if self.is_empty():
-        raise Exception(&#34;Empty Queue&#34;)
+<pre><code class="python">def search(self, value):
+    &#34;&#34;&#34; 
+    Search for a value in the binary search tree.
 
-    return self._array[self._front]</code></pre>
+    Args:
+        value: value to search for
+    
+    Returns:
+    node with matching value
+    None if not found
+    &#34;&#34;&#34;
+    current = self.root
+    
+    while current is not None:
+        if value == current.value:
+            return current
+        elif value &lt; current.value:
+            current = current.left
+        elif value &gt; current.value:
+            current = current.right
+        else:
+            return None
+    
+    return None</code></pre>
 </details>
 </dd>
 </dl>
 </dd>
 </dl>
 </section>
 </article>
@@ -518,30 +671,28 @@
 <ul>
 <li><code><a title="dsa" href="index.html">dsa</a></code></li>
 </ul>
 </li>
 <li><h3><a href="#header-classes">Classes</a></h3>
 <ul>
 <li>
-<h4><code><a title="dsa.queue.DynamicQueue" href="#dsa.queue.DynamicQueue">DynamicQueue</a></code></h4>
+<h4><code><a title="dsa.tree.Node" href="#dsa.tree.Node">Node</a></code></h4>
 <ul class="">
-<li><code><a title="dsa.queue.DynamicQueue.check_capacity" href="#dsa.queue.DynamicQueue.check_capacity">check_capacity</a></code></li>
-<li><code><a title="dsa.queue.DynamicQueue.enqueue" href="#dsa.queue.DynamicQueue.enqueue">enqueue</a></code></li>
-<li><code><a title="dsa.queue.DynamicQueue.grow" href="#dsa.queue.DynamicQueue.grow">grow</a></code></li>
+<li><code><a title="dsa.tree.Node.print" href="#dsa.tree.Node.print">print</a></code></li>
 </ul>
 </li>
 <li>
-<h4><code><a title="dsa.queue.Queue" href="#dsa.queue.Queue">Queue</a></code></h4>
+<h4><code><a title="dsa.tree.Tree" href="#dsa.tree.Tree">Tree</a></code></h4>
 <ul class="two-column">
-<li><code><a title="dsa.queue.Queue.capacity" href="#dsa.queue.Queue.capacity">capacity</a></code></li>
-<li><code><a title="dsa.queue.Queue.count" href="#dsa.queue.Queue.count">count</a></code></li>
-<li><code><a title="dsa.queue.Queue.dequeue" href="#dsa.queue.Queue.dequeue">dequeue</a></code></li>
-<li><code><a title="dsa.queue.Queue.enqueue" href="#dsa.queue.Queue.enqueue">enqueue</a></code></li>
-<li><code><a title="dsa.queue.Queue.is_empty" href="#dsa.queue.Queue.is_empty">is_empty</a></code></li>
-<li><code><a title="dsa.queue.Queue.peek" href="#dsa.queue.Queue.peek">peek</a></code></li>
+<li><code><a title="dsa.tree.Tree.delete" href="#dsa.tree.Tree.delete">delete</a></code></li>
+<li><code><a title="dsa.tree.Tree.delete_node" href="#dsa.tree.Tree.delete_node">delete_node</a></code></li>
+<li><code><a title="dsa.tree.Tree.insert" href="#dsa.tree.Tree.insert">insert</a></code></li>
+<li><code><a title="dsa.tree.Tree.min_node" href="#dsa.tree.Tree.min_node">min_node</a></code></li>
+<li><code><a title="dsa.tree.Tree.print" href="#dsa.tree.Tree.print">print</a></code></li>
+<li><code><a title="dsa.tree.Tree.search" href="#dsa.tree.Tree.search">search</a></code></li>
 </ul>
 </li>
 </ul>
 </li>
 </ul>
 </nav>
 </main>
```

#### html2text {}

```diff
@@ -1,398 +1,542 @@
-************ MMoodduullee ddssaa..qquueeuuee ************
+************ MMoodduullee ddssaa..ttrreeee ************
 Expand source code
-class Queue:
+class Node:
     """
-    A static queue implementation in Python
+    A binary tree node implementation in Python
     """
-    def __init__(self, capacity=10):
+    def __init__(self, value, left=None, right=None):
         """
         Args:
-            capacity: the initial size of the stack (defaults to 10)
+            value: value of the node
+            left: left node
+            right: right node
         """
-        self._array = [None] * capacity
-        self._front = 0
-        #: number of elements in queue
-        self.count = 0
+        self.value = value
+        self.left = left
+        self.right = right
 
-    def enqueue(self, element):
+    def print(self, level=0):
         """
-        Enqueue an element into the queue. Raise Exception when trying to
-enqueue more elements than the capacity.
+        Print the contents of a node.
 
         Args:
-            element: the element to enqueue
+            level: starting level of node
         """
-        if self.count >= len(self._array):
-            raise Exception("Capacity Reached")
+        if self.right:
+            self.right.print(level + 1)
+        print("   " * level + str(self.value))
+        if self.left:
+            self.left.print(level + 1)
 
-        index = (self._front + self.count) % len(self._array)
-        self._array[index] = element
-        self.count += 1
+class Tree:
+    """
+    A binary search tree implementation in Python
+    """
+    def __init__(self, root=None):
+        """
+        Args:
+            root: root node of the BST
+        """
+        self.root = root
 
-    def dequeue(self):
+    def search(self, value):
         """
-        Dequeue an element from the queue. Raise Exception when there are no
-elements to dequeue.
+        Search for a value in the binary search tree.
+
+        Args:
+            value: value to search for
 
         Returns:
-            the from element in the queue
+        node with matching value
+        None if not found
         """
-        if self.is_empty():
-            raise Exception("Empty Queue")
+        current = self.root
 
-        element = self._array[self._front]
-        self._front += 1
-        if self._front >= len(self._array):
-            self._front = 0
-        self.count -= 1
+        while current is not None:
+            if value == current.value:
+                return current
+            elif value < current.value:
+                current = current.left
+            elif value > current.value:
+                current = current.right
+            else:
+                return None
 
-        return element
+        return None
 
-    def peek(self):
-        """
-        Return the element in front of the queue. Raise Exception if queue is
-empty.
+    def insert(self, value):
         """
-        if self.is_empty():
-            raise Exception("Empty Queue")
+        Insert a value in the binary search tree.
 
-        return self._array[self._front]
+        Args:
+            value: value to insert
 
-    def is_empty(self):
+        Returns:
+        None
         """
-        Return a Boolean on whether the stack is empty or not.
+        current = self.root
+        if self.root is None:
+            self.root = Node(value)
+            return
+
+        while current is not None:
+            if value < current.value:
+                if current.left is None:
+                    current.left = Node(value)
+                    return
+                else:
+                    current = current.left
+            elif value > current.value:
+                if current.right is None:
+                    current.right = Node(value)
+                    return
+                else:
+                    current = current.right
+            else:
+                return
+
+    def delete(self, value):
         """
-        return self.count == 0
+        Delete a value from the binary search tree.
 
-    def capacity(self):
+        Args:
+            value: value to delete
+
+        Returns:
+        None
         """
-        Return the capacity of the queue.
+        return self.delete_node(value, self.root)
+
+    def delete_node(self, value, node):
         """
-        return len(self._array)
+        Helper function to delete a value from the binary search tree. (Use
+delete() instead)
 
-    def __repr__(self):
-        arr = []
-        for i in range(self.count):
-            index = (i + self._front) % len(self._array)
-            arr.append(str(self._array[index]))
-        arrstr = ", ".join(arr)
-        return f"[{arrstr}] Front: {self._front} count: {self.count} Capacity:
-{self.capacity()}"
+        Args:
+            value: value to delete
+            node: current node
+        """
+        if node is None:
+            return None
 
+        if value < node.value:
+            node.left = self.delete_node(value, node.left)
+        elif value > node.value:
+            node.right = self.delete_node(value, node.right)
+        else:
+            if node.left is None:
+                branch = node.right
+                node = None
+                return branch
+            elif node.right is None:
+                branch = node.left
+                node = None
+                return branch
+
+            branch = self.min_node(node.right)
+            node.value = branch.value
+            node.right = self.delete_node(branch.value, node.right)
 
-# shrink not implemented
-class DynamicQueue(Queue):
-    """
-    A dynamic queue implementation in Python
-    """
-    def __init__(self, capacity=10):
-        super().__init__(capacity)
+        return node
 
-    def grow(self):
-        """
-        double the capacity of the current array
+    def min_node(self, node=None):
         """
-        new_array = [ None ] * len(self._array) * 2
+        Return the node with the minimum value in a binary search tree.
 
-        # copy elements
-        for i in range(self.count):
-            new_array[i] = self._array[i + self._front]
-        self._front = 0
-        self._array = new_array
+        Args:
+            node: starting node
 
-    def check_capacity(self):
-        """
-        if count >= capacity, grow the array
+        Returns:
+        node with the lowest value in the BST
+        None if not found
         """
-        if self._front + self.count >= len(self._array):
-            self.grow()
+        if node is None:
+            node = self.root
+
+        if node.left is None:
+            return node
+        else:
+            return self.min_node(node.left)
 
-    def enqueue(self, element):
+    def print(self):
         """
-        Enqueue an element into the queue. Increae capacity if count is greater
-than the capacity.
+        Print the values in the BST.
 
-        Args:
-            element: the element to enqueue
         """
-        self.check_capacity()
-        index = self._front + self.count
-        self._array[index] = element
-        self.count += 1
+        self.root.print()
+
+
 ********** CCllaasssseess **********
-  class DynamicQueue (capacity=10)
-      A dynamic queue implementation in Python
+  class Node (value, left=None, right=None)
+      A binary tree node implementation in Python
       ********** AArrggss **********
-        ccaappaacciittyy
-            the initial size of the stack (defaults to 10)
+        vvaalluuee
+            value of the node
+        lleefftt
+            left node
+        rriigghhtt
+            right node
       Expand source code
-      class DynamicQueue(Queue):
+      class Node:
           """
-          A dynamic queue implementation in Python
+          A binary tree node implementation in Python
           """
-          def __init__(self, capacity=10):
-              super().__init__(capacity)
-
-          def grow(self):
+          def __init__(self, value, left=None, right=None):
               """
-              double the capacity of the current array
-              """
-              new_array = [ None ] * len(self._array) * 2
-
-              # copy elements
-              for i in range(self.count):
-                  new_array[i] = self._array[i + self._front]
-              self._front = 0
-              self._array = new_array
-
-          def check_capacity(self):
-              """
-              if count >= capacity, grow the array
+              Args:
+                  value: value of the node
+                  left: left node
+                  right: right node
               """
-              if self._front + self.count >= len(self._array):
-                  self.grow()
+              self.value = value
+              self.left = left
+              self.right = right
 
-          def enqueue(self, element):
+          def print(self, level=0):
               """
-              Enqueue an element into the queue. Increae capacity if count is
-      greater than the capacity.
+              Print the contents of a node.
 
               Args:
-                  element: the element to enqueue
+                  level: starting level of node
               """
-              self.check_capacity()
-              index = self._front + self.count
-              self._array[index] = element
-              self.count += 1
-      ******** AAnncceessttoorrss ********
-          * _Q_u_e_u_e
+              if self.right:
+                  self.right.print(level + 1)
+              print("   " * level + str(self.value))
+              if self.left:
+                  self.left.print(level + 1)
       ******** MMeetthhooddss ********
-        def check_capacity(self)
-            if count >= capacity, grow the array
-            Expand source code
-            def check_capacity(self):
-                """
-                if count >= capacity, grow the array
-                """
-                if self._front + self.count >= len(self._array):
-                    self.grow()
-        def enqueue(self, element)
-            Enqueue an element into the queue. Increae capacity if count is
-            greater than the capacity.
+        def print(self, level=0)
+            Print the contents of a node.
             ********** AArrggss **********
-              eelleemmeenntt
-                  the element to enqueue
+              lleevveell
+                  starting level of node
             Expand source code
-            def enqueue(self, element):
+            def print(self, level=0):
                 """
-                Enqueue an element into the queue. Increae capacity if count is
-            greater than the capacity.
+                Print the contents of a node.
 
                 Args:
-                    element: the element to enqueue
-                """
-                self.check_capacity()
-                index = self._front + self.count
-                self._array[index] = element
-                self.count += 1
-        def grow(self)
-            double the capacity of the current array
-            Expand source code
-            def grow(self):
+                    level: starting level of node
                 """
-                double the capacity of the current array
-                """
-                new_array = [ None ] * len(self._array) * 2
-
-                # copy elements
-                for i in range(self.count):
-                    new_array[i] = self._array[i + self._front]
-                self._front = 0
-                self._array = new_array
-      ******** IInnhheerriitteedd mmeemmbbeerrss ********
-          * _QQ_uu_ee_uu_ee:
-                o _c_a_p_a_c_i_t_y
-                o _c_o_u_n_t
-                o _d_e_q_u_e_u_e
-                o _i_s___e_m_p_t_y
-                o _p_e_e_k
-  class Queue (capacity=10)
-      A static queue implementation in Python
+                if self.right:
+                    self.right.print(level + 1)
+                print("   " * level + str(self.value))
+                if self.left:
+                    self.left.print(level + 1)
+  class Tree (root=None)
+      A binary search tree implementation in Python
       ********** AArrggss **********
-        ccaappaacciittyy
-            the initial size of the stack (defaults to 10)
+        rroooott
+            root node of the BST
       Expand source code
-      class Queue:
+      class Tree:
           """
-          A static queue implementation in Python
+          A binary search tree implementation in Python
           """
-          def __init__(self, capacity=10):
+          def __init__(self, root=None):
               """
               Args:
-                  capacity: the initial size of the stack (defaults to 10)
+                  root: root node of the BST
               """
-              self._array = [None] * capacity
-              self._front = 0
-              #: number of elements in queue
-              self.count = 0
+              self.root = root
 
-          def enqueue(self, element):
+          def search(self, value):
               """
-              Enqueue an element into the queue. Raise Exception when trying to
-      enqueue more elements than the capacity.
+              Search for a value in the binary search tree.
 
               Args:
-                  element: the element to enqueue
+                  value: value to search for
+
+              Returns:
+              node with matching value
+              None if not found
               """
-              if self.count >= len(self._array):
-                  raise Exception("Capacity Reached")
+              current = self.root
+
+              while current is not None:
+                  if value == current.value:
+                      return current
+                  elif value < current.value:
+                      current = current.left
+                  elif value > current.value:
+                      current = current.right
+                  else:
+                      return None
 
-              index = (self._front + self.count) % len(self._array)
-              self._array[index] = element
-              self.count += 1
+              return None
 
-          def dequeue(self):
+          def insert(self, value):
               """
-              Dequeue an element from the queue. Raise Exception when there are
-      no elements to dequeue.
+              Insert a value in the binary search tree.
+
+              Args:
+                  value: value to insert
 
               Returns:
-                  the from element in the queue
+              None
               """
-              if self.is_empty():
-                  raise Exception("Empty Queue")
+              current = self.root
+              if self.root is None:
+                  self.root = Node(value)
+                  return
+
+              while current is not None:
+                  if value < current.value:
+                      if current.left is None:
+                          current.left = Node(value)
+                          return
+                      else:
+                          current = current.left
+                  elif value > current.value:
+                      if current.right is None:
+                          current.right = Node(value)
+                          return
+                      else:
+                          current = current.right
+                  else:
+                      return
 
-              element = self._array[self._front]
-              self._front += 1
-              if self._front >= len(self._array):
-                  self._front = 0
-              self.count -= 1
+          def delete(self, value):
+              """
+              Delete a value from the binary search tree.
 
-              return element
+              Args:
+                  value: value to delete
 
-          def peek(self):
-              """
-              Return the element in front of the queue. Raise Exception if
-      queue is empty.
+              Returns:
+              None
               """
-              if self.is_empty():
-                  raise Exception("Empty Queue")
+              return self.delete_node(value, self.root)
 
-              return self._array[self._front]
+          def delete_node(self, value, node):
+              """
+              Helper function to delete a value from the binary search tree.
+      (Use delete() instead)
 
-          def is_empty(self):
+              Args:
+                  value: value to delete
+                  node: current node
               """
-              Return a Boolean on whether the stack is empty or not.
+              if node is None:
+                  return None
+
+              if value < node.value:
+                  node.left = self.delete_node(value, node.left)
+              elif value > node.value:
+                  node.right = self.delete_node(value, node.right)
+              else:
+                  if node.left is None:
+                      branch = node.right
+                      node = None
+                      return branch
+                  elif node.right is None:
+                      branch = node.left
+                      node = None
+                      return branch
+
+                  branch = self.min_node(node.right)
+                  node.value = branch.value
+                  node.right = self.delete_node(branch.value, node.right)
+
+              return node
+
+          def min_node(self, node=None):
               """
-              return self.count == 0
+              Return the node with the minimum value in a binary search tree.
 
-          def capacity(self):
+              Args:
+                  node: starting node
+
+              Returns:
+              node with the lowest value in the BST
+              None if not found
               """
-              Return the capacity of the queue.
+              if node is None:
+                  node = self.root
+
+              if node.left is None:
+                  return node
+              else:
+                  return self.min_node(node.left)
+
+          def print(self):
               """
-              return len(self._array)
+              Print the values in the BST.
 
-          def __repr__(self):
-              arr = []
-              for i in range(self.count):
-                  index = (i + self._front) % len(self._array)
-                  arr.append(str(self._array[index]))
-              arrstr = ", ".join(arr)
-              return f"[{arrstr}] Front: {self._front} count: {self.count}
-      Capacity: {self.capacity()}"
-      ******** SSuubbccllaasssseess ********
-          * _D_y_n_a_m_i_c_Q_u_e_u_e
-      ******** IInnssttaannccee vvaarriiaabblleess ********
-        var count
-            number of elements in queue
+              """
+              self.root.print()
       ******** MMeetthhooddss ********
-        def capacity(self)
-            Return the capacity of the queue.
+        def delete(self, value)
+            Delete a value from the binary search tree.
+            ********** AArrggss **********
+              vvaalluuee
+                  value to delete
+            Returns: None
+            Expand source code
+            def delete(self, value):
+                """
+                Delete a value from the binary search tree.
+
+                Args:
+                    value: value to delete
+
+                Returns:
+                None
+                """
+                return self.delete_node(value, self.root)
+        def delete_node(self, value, node)
+            Helper function to delete a value from the binary search tree. (Use
+            delete() instead)
+            ********** AArrggss **********
+              vvaalluuee
+                  value to delete
+              nnooddee
+                  current node
             Expand source code
-            def capacity(self):
+            def delete_node(self, value, node):
                 """
-                Return the capacity of the queue.
+                Helper function to delete a value from the binary search tree.
+            (Use delete() instead)
+
+                Args:
+                    value: value to delete
+                    node: current node
                 """
-                return len(self._array)
-        def dequeue(self)
-            Dequeue an element from the queue. Raise Exception when there are
-            no elements to dequeue.
-            ********** RReettuurrnnss **********
-            the from element in the queue
+                if node is None:
+                    return None
+
+                if value < node.value:
+                    node.left = self.delete_node(value, node.left)
+                elif value > node.value:
+                    node.right = self.delete_node(value, node.right)
+                else:
+                    if node.left is None:
+                        branch = node.right
+                        node = None
+                        return branch
+                    elif node.right is None:
+                        branch = node.left
+                        node = None
+                        return branch
+
+                    branch = self.min_node(node.right)
+                    node.value = branch.value
+                    node.right = self.delete_node(branch.value, node.right)
+
+                return node
+        def insert(self, value)
+            Insert a value in the binary search tree.
+            ********** AArrggss **********
+              vvaalluuee
+                  value to insert
+            Returns: None
             Expand source code
-            def dequeue(self):
+            def insert(self, value):
                 """
-                Dequeue an element from the queue. Raise Exception when there
-            are no elements to dequeue.
+                Insert a value in the binary search tree.
+
+                Args:
+                    value: value to insert
 
                 Returns:
-                    the from element in the queue
+                None
                 """
-                if self.is_empty():
-                    raise Exception("Empty Queue")
-
-                element = self._array[self._front]
-                self._front += 1
-                if self._front >= len(self._array):
-                    self._front = 0
-                self.count -= 1
-
-                return element
-        def enqueue(self, element)
-            Enqueue an element into the queue. Raise Exception when trying to
-            enqueue more elements than the capacity.
+                current = self.root
+                if self.root is None:
+                    self.root = Node(value)
+                    return
+
+                while current is not None:
+                    if value < current.value:
+                        if current.left is None:
+                            current.left = Node(value)
+                            return
+                        else:
+                            current = current.left
+                    elif value > current.value:
+                        if current.right is None:
+                            current.right = Node(value)
+                            return
+                        else:
+                            current = current.right
+                    else:
+                        return
+        def min_node(self, node=None)
+            Return the node with the minimum value in a binary search tree.
             ********** AArrggss **********
-              eelleemmeenntt
-                  the element to enqueue
+              nnooddee
+                  starting node
+            Returns: node with the lowest value in the BST None if not found
             Expand source code
-            def enqueue(self, element):
+            def min_node(self, node=None):
                 """
-                Enqueue an element into the queue. Raise Exception when trying
-            to enqueue more elements than the capacity.
+                Return the node with the minimum value in a binary search tree.
 
                 Args:
-                    element: the element to enqueue
+                    node: starting node
+
+                Returns:
+                node with the lowest value in the BST
+                None if not found
                 """
-                if self.count >= len(self._array):
-                    raise Exception("Capacity Reached")
+                if node is None:
+                    node = self.root
 
-                index = (self._front + self.count) % len(self._array)
-                self._array[index] = element
-                self.count += 1
-        def is_empty(self)
-            Return a Boolean on whether the stack is empty or not.
+                if node.left is None:
+                    return node
+                else:
+                    return self.min_node(node.left)
+        def print(self)
+            Print the values in the BST.
             Expand source code
-            def is_empty(self):
+            def print(self):
                 """
-                Return a Boolean on whether the stack is empty or not.
+                Print the values in the BST.
+
                 """
-                return self.count == 0
-        def peek(self)
-            Return the element in front of the queue. Raise Exception if queue
-            is empty.
+                self.root.print()
+        def search(self, value)
+            Search for a value in the binary search tree.
+            ********** AArrggss **********
+              vvaalluuee
+                  value to search for
+            Returns: node with matching value None if not found
             Expand source code
-            def peek(self):
+            def search(self, value):
                 """
-                Return the element in front of the queue. Raise Exception if
-            queue is empty.
+                Search for a value in the binary search tree.
+
+                Args:
+                    value: value to search for
+
+                Returns:
+                node with matching value
+                None if not found
                 """
-                if self.is_empty():
-                    raise Exception("Empty Queue")
+                current = self.root
+
+                while current is not None:
+                    if value == current.value:
+                        return current
+                    elif value < current.value:
+                        current = current.left
+                    elif value > current.value:
+                        current = current.right
+                    else:
+                        return None
 
-                return self._array[self._front]
+                return None
 ************ IInnddeexx ************
     * ******** SSuuppeerr--mmoodduullee ********
           o _d_s_a
     * ******** _CC_ll_aa_ss_ss_ee_ss ********
-          o ****** _DD_yy_nn_aa_mm_ii_cc_QQ_uu_ee_uu_ee ******
-                # _c_h_e_c_k___c_a_p_a_c_i_t_y
-                # _e_n_q_u_e_u_e
-                # _g_r_o_w
-          o ****** _QQ_uu_ee_uu_ee ******
-                # _c_a_p_a_c_i_t_y
-                # _c_o_u_n_t
-                # _d_e_q_u_e_u_e
-                # _e_n_q_u_e_u_e
-                # _i_s___e_m_p_t_y
-                # _p_e_e_k
+          o ****** _NN_oo_dd_ee ******
+                # _p_r_i_n_t
+          o ****** _TT_rr_ee_ee ******
+                # _d_e_l_e_t_e
+                # _d_e_l_e_t_e___n_o_d_e
+                # _i_n_s_e_r_t
+                # _m_i_n___n_o_d_e
+                # _p_r_i_n_t
+                # _s_e_a_r_c_h
 Generated by_p_d_o_c_0_._1_0_._0.
```

### Comparing `ucxdsa-2024.4.23/src/html/dsa/stack.html` & `ucxdsa-2024.5.9/src/html/dsa/stack.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/src/ucxdsa.egg-info/PKG-INFO` & `ucxdsa-2024.5.9/src/ucxdsa.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_array.py` & `ucxdsa-2024.5.9/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_doublylinkedlist.py` & `ucxdsa-2024.5.9/tests/test_doublylinkedlist.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_graph_list.py` & `ucxdsa-2024.5.9/tests/test_graph_list.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_graph_matrix.py` & `ucxdsa-2024.5.9/tests/test_graph_matrix.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_hash.py` & `ucxdsa-2024.5.9/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_heap.py` & `ucxdsa-2024.5.9/tests/test_heap.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_huffman.py` & `ucxdsa-2024.5.9/tests/test_huffman.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_linkedlist.py` & `ucxdsa-2024.5.9/tests/test_linkedlist.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_pretty_print.py` & `ucxdsa-2024.5.9/tests/test_pretty_print.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_queue.py` & `ucxdsa-2024.5.9/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_stack.py` & `ucxdsa-2024.5.9/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_tree.py` & `ucxdsa-2024.5.9/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/tests/test_trie.py` & `ucxdsa-2024.5.9/tests/test_trie.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/LICENSE` & `ucxdsa-2024.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.4.23/pyproject.toml` & `ucxdsa-2024.5.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ucxdsa"
-version = "2024.04.23"
+version = "2024.05.09"
 authors = [
   { name="Carl Limsico", email="limsico@berkeley.edu" },
 ]
 description = "Data Structures and Algorithms Source Code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ucxdsa-2024.4.23/PKG-INFO` & `ucxdsa-2024.5.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ucxdsa
-Version: 2024.4.23
+Version: 2024.5.9
 Summary: Data Structures and Algorithms Source Code
 Author-email: Carl Limsico <limsico@berkeley.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

