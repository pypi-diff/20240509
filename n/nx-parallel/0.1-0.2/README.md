# Comparing `tmp/nx_parallel-0.1.tar.gz` & `tmp/nx_parallel-0.2.tar.gz`

## Comparing `nx_parallel-0.1.tar` & `nx_parallel-0.2.tar`

### file list

```diff
@@ -1,31 +1,77 @@
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nx_parallel-0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 nx_parallel-0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 nx_parallel-0.1/RELEASE.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 nx_parallel-0.1/.github/workflows/label-check.yaml
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 nx_parallel-0.1/.github/workflows/milestone-merged-prs.yaml
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 nx_parallel-0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nx_parallel-0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nx_parallel-0.1/nx_parallel/__init__.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 nx_parallel-0.1/nx_parallel/interface.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nx_parallel-0.1/nx_parallel/algorithms/__init__.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 nx_parallel-0.1/nx_parallel/algorithms/efficiency_measures.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nx_parallel-0.1/nx_parallel/algorithms/isolate.py
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 nx_parallel-0.1/nx_parallel/algorithms/tournament.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 nx_parallel-0.1/nx_parallel/algorithms/vitality.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 nx_parallel-0.1/nx_parallel/algorithms/centrality/__init__.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 nx_parallel-0.1/nx_parallel/algorithms/centrality/betweenness.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nx_parallel-0.1/nx_parallel/utils/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 nx_parallel-0.1/nx_parallel/utils/chunk.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 nx_parallel-0.1/requirements/release.txt
--rw-r--r--   0        0        0   273261 2020-02-02 00:00:00.000000 nx_parallel-0.1/timing/heatmap_all_functions.png
--rw-r--r--   0        0        0    45735 2020-02-02 00:00:00.000000 nx_parallel-0.1/timing/heatmap_betweenness_centrality_timing.png
--rw-r--r--   0        0        0    47279 2020-02-02 00:00:00.000000 nx_parallel-0.1/timing/heatmap_closeness_vitality_timing.png
--rw-r--r--   0        0        0    32267 2020-02-02 00:00:00.000000 nx_parallel-0.1/timing/heatmap_is_reachable_timing.png
--rw-r--r--   0        0        0    41856 2020-02-02 00:00:00.000000 nx_parallel-0.1/timing/heatmap_local_efficiency_timing.png
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 nx_parallel-0.1/timing/timing_all_functions.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 nx_parallel-0.1/timing/timing_comparison.md
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 nx_parallel-0.1/timing/timing_individual_function.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nx_parallel-0.1/.gitignore
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 nx_parallel-0.1/README.md
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 nx_parallel-0.1/pyproject.toml
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 nx_parallel-0.1/PKG-INFO
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nx_parallel-0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 nx_parallel-0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 nx_parallel-0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nx_parallel-0.2/RELEASE.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 nx_parallel-0.2/.github/workflows/label-check.yaml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 nx_parallel-0.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 nx_parallel-0.2/.github/workflows/milestone-merged-prs.yaml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 nx_parallel-0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 nx_parallel-0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0    14698 2020-02-02 00:00:00.000000 nx_parallel-0.2/_nx_parallel/__init__.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 nx_parallel-0.2/_nx_parallel/script.sh
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 nx_parallel-0.2/_nx_parallel/update_get_info.py
+-rw-r--r--   0        0        0   763267 2020-02-02 00:00:00.000000 nx_parallel-0.2/assets/images/backend_box_ss.png
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/asv.conf.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/benchmarks/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/benchmarks/bench_approximation.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/benchmarks/bench_bipartite.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/benchmarks/bench_centrality.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/benchmarks/bench_cluster.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/benchmarks/bench_connectivity.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/benchmarks/bench_efficiency_measures.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/benchmarks/bench_isolate.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/benchmarks/bench_shortest_paths.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/benchmarks/bench_tournament.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/benchmarks/bench_vitality.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 nx_parallel-0.2/benchmarks/benchmarks/common.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/__init__.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/interface.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/cluster.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/efficiency_measures.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/isolate.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/tournament.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/vitality.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/approximation/__init__.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/approximation/connectivity.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/bipartite/__init__.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/bipartite/redundancy.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/centrality/__init__.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/centrality/betweenness.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/centrality/tests/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/centrality/tests/test_betweenness_centrality.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/connectivity/__init__.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/connectivity/connectivity.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/shortest_paths/__init__.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/shortest_paths/generic.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/shortest_paths/unweighted.py
+-rw-r--r--   0        0        0    11014 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/algorithms/shortest_paths/weighted.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/utils/__init__.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 nx_parallel-0.2/nx_parallel/utils/chunk.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 nx_parallel-0.2/requirements/release.txt
+-rw-r--r--   0        0        0   273261 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_all_functions.png
+-rw-r--r--   0        0        0    47096 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_all_pairs_all_shortest_paths_timing.png
+-rw-r--r--   0        0        0    48243 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_all_pairs_bellman_ford_path_length_timing.png
+-rw-r--r--   0        0        0    46046 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_all_pairs_bellman_ford_path_timing.png
+-rw-r--r--   0        0        0    47034 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_all_pairs_dijkstra_path_length_timing.png
+-rw-r--r--   0        0        0    44850 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_all_pairs_dijkstra_path_timing.png
+-rw-r--r--   0        0        0    46566 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_all_pairs_dijkstra_timing.png
+-rw-r--r--   0        0        0    46464 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_all_pairs_node_connectivity_timing.png
+-rw-r--r--   0        0        0    52719 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_all_pairs_shortest_path_length_timing.png
+-rw-r--r--   0        0        0    49282 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_all_pairs_shortest_path_timing.png
+-rw-r--r--   0        0        0    45735 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_betweenness_centrality_timing.png
+-rw-r--r--   0        0        0    47279 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_closeness_vitality_timing.png
+-rw-r--r--   0        0        0    32267 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_is_reachable_timing.png
+-rw-r--r--   0        0        0    45055 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_johnson_timing.png
+-rw-r--r--   0        0        0    41856 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_local_efficiency_timing.png
+-rw-r--r--   0        0        0    44232 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_node_redundancy_timing.png
+-rw-r--r--   0        0        0    45465 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/heatmap_square_clustering_timing.png
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/timing_all_functions.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/timing_comparison.md
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 nx_parallel-0.2/timing/timing_individual_function.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 nx_parallel-0.2/.gitignore
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nx_parallel-0.2/LICENSE.md
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 nx_parallel-0.2/README.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 nx_parallel-0.2/pyproject.toml
+-rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 nx_parallel-0.2/PKG-INFO
```

### Comparing `nx_parallel-0.1/RELEASE.md` & `nx_parallel-0.2/RELEASE.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,10 +50,10 @@
 
       https://github.com/networkx/nx-parallel/tags
 
 - Update `__version__` in `nx_parallel/__init__.py`.
 
 - Commit changes:
 
-      git add pyproject.toml
+      git add nx_parallel/__init__.py
       git commit -m 'Bump version'
       git push origin main
```

### Comparing `nx_parallel-0.1/.github/workflows/release.yml` & `nx_parallel-0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `nx_parallel-0.1/.github/workflows/test.yml` & `nx_parallel-0.2/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -12,35 +12,32 @@
     defaults:
       run:
         shell: bash -l {0}
     strategy:
       # fail-fast: true
       matrix:
         os: ["ubuntu-latest", "macos-latest", "windows-latest"]
-        python-version: ["3.11", "3.12"]
+        python-version: ["3.10", "3.11", "3.12"]
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - name: Conda
-        uses: conda-incubator/setup-miniconda@v2
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v5
         with:
-          auto-update-conda: true
           python-version: ${{ matrix.python-version }}
-          channels: conda-forge
-          activate-environment: testing
       - name: Install dependencies
         run: |
-          conda install -c conda-forge joblib scipy pandas pytest-cov pytest-randomly
+          python -m pip install scipy pandas pytest-cov pytest-randomly
             # matplotlib lxml pygraphviz pydot sympy  # Extra networkx deps we don't need yet
           python -m pip install git+https://github.com/networkx/networkx.git@main
           python -m pip install .
           echo "Done with installing"
       - name: PyTest
         run: |
-          NETWORKX_GRAPH_CONVERT=parallel \
           NETWORKX_TEST_BACKEND=parallel \
           NETWORKX_FALLBACK_TO_NX=True \
                 python -m pytest --pyargs networkx
-
-          python -m pytest --doctest-modules --pyargs nx_parallel
+      - name: Additional Tests for nx-parallel
+        run: |
+          pytest nx_parallel
```

### Comparing `nx_parallel-0.1/timing/heatmap_all_functions.png` & `nx_parallel-0.2/timing/heatmap_all_functions.png`

 * *Files identical despite different names*

### Comparing `nx_parallel-0.1/timing/heatmap_betweenness_centrality_timing.png` & `nx_parallel-0.2/timing/heatmap_betweenness_centrality_timing.png`

 * *Files identical despite different names*

### Comparing `nx_parallel-0.1/timing/heatmap_closeness_vitality_timing.png` & `nx_parallel-0.2/timing/heatmap_closeness_vitality_timing.png`

 * *Files identical despite different names*

### Comparing `nx_parallel-0.1/timing/heatmap_is_reachable_timing.png` & `nx_parallel-0.2/timing/heatmap_is_reachable_timing.png`

 * *Files identical despite different names*

### Comparing `nx_parallel-0.1/timing/heatmap_local_efficiency_timing.png` & `nx_parallel-0.2/timing/heatmap_local_efficiency_timing.png`

 * *Files identical despite different names*

### Comparing `nx_parallel-0.1/timing/timing_all_functions.py` & `nx_parallel-0.2/timing/timing_all_functions.py`

 * *Files identical despite different names*

### Comparing `nx_parallel-0.1/timing/timing_comparison.md` & `nx_parallel-0.2/timing/timing_comparison.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-Timing Comparisons
+# Timing Comparisons
 
 ---
 
 Model: 13-inch MacBook Pro (2020)
 
 CPU: 2 GHz Quad-Core Intel Core i5
 
 RAM: 16 GB LPDDR4X at 3733 MHz
 
 Code to generate heatmaps in timing_individual_function.py and timing_all_functions.py.
 
-### All parallelized functions at this time:
+## All parallelized functions at this time:
 
 ![alt text](heatmap_all_functions.png)
 
-### Individual functions:
+## Individual functions:
 
 betweenness_centrality
 ![alt text](heatmap_betweenness_centrality_timing.png)
 
 closeness_vitality
 ![alt text](heatmap_closeness_vitality_timing.png)
 
 local_efficiency
 ![alt text](heatmap_local_efficiency_timing.png)
 
 tournament is_reachable
 ![alt text](heatmap_is_reachable_timing.png)
+
+all_pairs_bellman_ford_path
+![alt text](heatmap_all_pairs_bellman_ford_path_timing.png)
```

### Comparing `nx_parallel-0.1/timing/timing_individual_function.py` & `nx_parallel-0.2/timing/timing_individual_function.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,88 @@
 import time
+import random
+import types
 
 import networkx as nx
 import pandas as pd
 import seaborn as sns
 from matplotlib import pyplot as plt
 
-import nx_parallel
+import nx_parallel as nxp
 
 # Code to create README heatmaps for individual function currFun
 heatmapDF = pd.DataFrame()
-number_of_nodes_list = [10, 50, 100, 300, 500]
+# for bipartite graphs
+# n = [50, 100, 200, 400]
+# m = [25, 50, 100, 200]
+number_of_nodes_list = [75, 150, 300, 600]
+weighted = False
 pList = [1, 0.8, 0.6, 0.4, 0.2]
-currFun = nx.betweenness_centrality
-for i in range(0, len(pList)):
-    p = pList[i]
-    for j in range(0, len(number_of_nodes_list)):
-        num = number_of_nodes_list[j]
-
+currFun = nx.bipartite.node_redundancy
+currFun = nx.square_clustering
+for p in pList:
+    for num in range(len(number_of_nodes_list)):
         # create original and parallel graphs
-        G = nx.fast_gnp_random_graph(num, p, directed=False)
-        H = nx_parallel.ParallelGraph(G)
+        G = nx.fast_gnp_random_graph(
+            number_of_nodes_list[num], p, seed=42, directed=True
+        )
+
+        """
+        # for bipartite.node_redundancy
+        G = nx.bipartite.random_graph(n[num], m[num], p, seed=42, directed=True)
+        for i in G.nodes:
+            l = list(G.neighbors(i))
+            if len(l) == 0:
+                v = random.choice(list(G.nodes) - [i,])
+                G.add_edge(i, v)
+                G.add_edge(i, random.choice([node for node in G.nodes if node != i]))
+            elif len(l) == 1:
+                G.add_edge(i, random.choice([node for node in G.nodes if node != i and node not in list(G.neighbors(i))]))
+        """
+
+        # for weighted graphs
+        if weighted:
+            random.seed(42)
+            for u, v in G.edges():
+                G[u][v]["weight"] = random.random()
+
+        H = nxp.ParallelGraph(G)
 
         # time both versions and update heatmapDF
         t1 = time.time()
-        c = currFun(H)
+        c1 = currFun(H)
+        if isinstance(c1, types.GeneratorType):
+            d = dict(c1)
         t2 = time.time()
         parallelTime = t2 - t1
         t1 = time.time()
-        c = currFun(G)
+        c2 = currFun(G)
+        if isinstance(c2, types.GeneratorType):
+            d = dict(c2)
         t2 = time.time()
         stdTime = t2 - t1
         timesFaster = stdTime / parallelTime
-        heatmapDF.at[j, i] = timesFaster
+        heatmapDF.at[number_of_nodes_list[num], p] = timesFaster
         print("Finished " + str(currFun))
 
 # Code to create for row of heatmap specifically for tournaments
-# for i in range(0, len(pList)):
-#     p = pList[i]
-#     for j in range(0, len(number_of_nodes_list)):
-#         num = number_of_nodes_list[j]
+# for p in pList:
+#     for num in number_of_nodes_list):
 #         G = nx.tournament.random_tournament(num)
 #         H = nx_parallel.ParallelDiGraph(G)
 #         t1 = time.time()
 #         c = nx.tournament.is_reachable(H, 1, num)
 #         t2 = time.time()
 #         parallelTime = t2-t1
 #         t1 = time.time()
 #         c = nx.tournament.is_reachable(G, 1, num)
 #         t2 = time.time()
 #         stdTime = t2-t1
 #         timesFaster = stdTime/parallelTime
-#         heatmapDF.at[j, 3] = timesFaster
+#         heatmapDF.at[num, 3] = timesFaster
 
 # plotting the heatmap with numbers and a green color scheme
 plt.figure(figsize=(20, 4))
 hm = sns.heatmap(data=heatmapDF.T, annot=True, cmap="Greens", cbar=True)
 
 # Remove the tick labels on both axes
 hm.set_yticklabels(pList)
@@ -62,15 +90,15 @@
 # Adding x-axis labels
 hm.set_xticklabels(number_of_nodes_list)
 
 # Rotating the x-axis labels for better readability (optional)
 plt.xticks(rotation=45)
 plt.yticks(rotation=20)
 plt.title(
-    "Small Scale Demo: Times Speedups of " + currFun.__name__ + " compared to networkx"
+    "Small Scale Demo: Times Speedups of " + currFun.__name__ + " compared to NetworkX"
 )
 plt.xlabel("Number of Vertices")
 plt.ylabel("Edge Probability")
 print(currFun.__name__)
 
 # displaying the plotted heatmap
 plt.tight_layout()
```

### Comparing `nx_parallel-0.1/.gitignore` & `nx_parallel-0.2/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -123,7 +123,11 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# asv 
+results/
+html/
```

### Comparing `nx_parallel-0.1/pyproject.toml` & `nx_parallel-0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "nx-parallel"
 authors = [
     {name = "NetworkX Devs", email = "networkx-core@discuss.scientific-python.org"},
 ]
 description = "An experimental parallel backend for NetworkX"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 keywords = ["networkx", "algorithms", "parallel"]
 license = {text = "BSD-3-Clause"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "networkx",
@@ -23,22 +23,29 @@
 
 [tool.hatch.version]
 path = "nx_parallel/__init__.py"
 
 [project.optional-dependencies]
 developer = [
     'pre-commit',
-    'pytest',
+]
+test = [
+    'pytest>=7.2',
+    'numpy>=1.23',
+    'scipy>=1.9,!=1.11.0,!=1.11.1',
 ]
 
-[project.entry-points."networkx.plugins"]
+[project.entry-points."networkx.backends"]
 parallel = "nx_parallel.interface:Dispatcher"
 
-[tool.setuptools]
-py-modules = []
+[project.entry-points."networkx.backend_info"]
+parallel = "_nx_parallel:get_info"
+
+[tool.hatch.build.targets.wheel]
+packages = ["_nx_parallel", "nx_parallel",]
 
 [tool.ruff]
 line-length = 88
-target-version = 'py311'
+target-version = 'py310'
 
-[tool.ruff.per-file-ignores]
-"__init__.py" = ['I', 'F403']
+[tool.ruff.lint]
+per-file-ignores = { "__init__.py" = ['I', 'F403'] }
```

