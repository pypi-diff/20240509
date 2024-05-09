# Comparing `tmp/first_passage_percolation_sim-0.1.1.tar.gz` & `tmp/first_passage_percolation_sim-0.1.2.tar.gz`

## Comparing `first_passage_percolation_sim-0.1.1.tar` & `first_passage_percolation_sim-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0   726100 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.1/example.ipynb
--rw-r--r--   0        0        0   361067 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.1/doc/assets/heatmap_geom_0_5.png
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.1/src/first_passage_percolation_sim/__init__.py
--rw-r--r--   0        0        0    14505 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.1/src/first_passage_percolation_sim/fpp.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.1/src/first_passage_percolation_sim/fpp.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.1/src/first_passage_percolation_sim/py.typed
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.1/LICENSE
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.1/README.md
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0   726098 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/example.ipynb
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   361067 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/doc/assets/heatmap_geom_0_5.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/src/first_passage_percolation_sim/__init__.py
+-rw-r--r--   0        0        0    14118 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/src/first_passage_percolation_sim/fpp.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/src/first_passage_percolation_sim/fpp.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/src/first_passage_percolation_sim/py.typed
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/LICENSE
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/README.md
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 first_passage_percolation_sim-0.1.2/PKG-INFO
```

### Comparing `first_passage_percolation_sim-0.1.1/example.ipynb` & `first_passage_percolation_sim-0.1.2/example.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992694805194805%*

 * *Differences: {"'cells'": "{0: {'execution_count': 10, 'source': {insert: [(5, 'rng = "*

 * *            "np.random.default_rng(4)')], delete: [5]}}}"}*

```diff
@@ -1,21 +1,21 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 75,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from scipy import stats\n",
                 "\n",
                 "import first_passage_percolation_sim as fpp\n",
                 "\n",
-                "rng = np.random.default_rng(4)\n"
+                "rng = np.random.default_rng(4)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# FirstPassagePercolation object"
```

### Comparing `first_passage_percolation_sim-0.1.1/doc/assets/heatmap_geom_0_5.png` & `first_passage_percolation_sim-0.1.2/doc/assets/heatmap_geom_0_5.png`

 * *Files identical despite different names*

### Comparing `first_passage_percolation_sim-0.1.1/src/first_passage_percolation_sim/fpp.py` & `first_passage_percolation_sim-0.1.2/src/first_passage_percolation_sim/fpp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,443 +1,451 @@
-from __future__ import annotations
-
-import copy
-import functools
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Protocol
-
-import matplotlib.pyplot as plt
-import numpy as np
-import rustworkx as rw
-from matplotlib import colors as mpl_colors
-from rustworkx.generators import grid_graph
-
-if TYPE_CHECKING:
-    from numpy.random import Generator
-
-
-def check_size_grid(size: int):
-    if size % 2 == 0:
-        msg = "The size of the grid side must be an odd number."
-        raise ValueError(msg)
-
-
-@dataclass
-class CenteredGrid:
-    """Represents a centered grid. That is, the center is at (0, 0) and
-    the indices are from -size_side // 2 to size_side // 2 - 1.
-
-    Attributes
-    ----------
-        array (np.ndarray): The 2-dimensional array representing the grid.
-
-    Properties:
-        size_side (int): The size of one side of the grid.
-        start_index (int): The start index of the grid i.e. -size_side // 2.
-        end_index (int): The end index of the grid i.e. size_side // 2 - 1.
-
-    Methods
-    -------
-        __getitem__(key): Get the value at the specified key in the grid.
-        __setitem__(key, value): Set the value at the specified key in the grid.
-
-    Raises
-    ------
-        ValueError: If the array is not 2-dimensional.
-        IndexError: If the index is out of bounds, i.e., less than -size_side // 2
-            or greater than or equal to size_side // 2.
-
-    """
-
-    array: np.ndarray
-
-    def __post_init__(self):
-        if self.array.ndim != 2:  # noqa: PLR2004
-            msg = "The array must be 2-dimensional."
-            raise ValueError(msg)
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}({self.array})"
-
-    def __str__(self):
-        name = self.__class__.__name__
-        indent = " " * len(name)
-        array_str = np.array2string(
-            self.array, separator=", ", prefix=indent, suffix=","
-        )
-        return f"{name}(\n{indent}{array_str}\n)"
-
-    @property
-    def size_side(self):
-        return self.array.shape[0]
-
-    @property
-    def start_index(self):
-        return -self._center
-
-    @property
-    def end_index(self):
-        return self._center - 1
-
-    @property
-    def _center(self):
-        return self.size_side // 2
-
-    def _transform_index(self, key: int | slice):
-        if isinstance(key, slice):
-            start, stop, step = key.start, key.stop, key.step
-            return slice(
-                self._transform_index(start) if start is not None else None,
-                self._transform_index(stop) if stop is not None else None,
-                step,
-            )
-
-        key_arr = np.asarray(key)
-
-        if (key_arr < -self._center).any() or (key_arr >= self._center).any():
-            msg = f"Index {key} is out of bounds."
-            raise IndexError(msg)
-        return key + self._center
-
-    def _transform_key(self, key: int | tuple) -> Any:
-        if isinstance(key, tuple):
-            return tuple(map(self._transform_index, key))
-        return self._transform_index(key)
-
-    def __getitem__(self, key):
-        key = self._transform_key(key)
-        return self.array[key]
-
-    def __setitem__(self, key, value):
-        key = self._transform_key(key)
-        self.array[key] = value
-
-
-class Dist(Protocol):
-    def rvs(self, size: int, random_state: Generator) -> np.ndarray: ...
-
-
-@functools.cache
-def _get_lengths(graph: rw.PyGraph, source_node: int, dist: Dist, rng, nb_edges):
-    x = dist.rvs(size=nb_edges, random_state=rng)
-    i = 0
-
-    def weight_func(_):
-        nonlocal i
-        w = x[i]
-        i += 1
-        return w
-
-    return dict(rw.dijkstra_shortest_path_lengths(graph, source_node, weight_func))
-
-
-class FirstPassagePercolation:
-    """Represents a First Passage Percolation simulation.
-        Each attribute can be modified after the object creation, except
-        for the graph. However, some changes may require recomputing the lengths by
-        calling the compute_lengths() method.
-
-    Args:
-    ----
-            size_side (int): The size of the grid side.
-            dist (Dist): The distribution object of the
-                random edge weights.
-            rng (numpy.random.Generator, optional): The random number generator.
-                Defaults to np.random.default_rng().
-
-    Attributes:
-    ----------
-            graph (Graph): The grid graph representing the simulation.
-            size_side (int): The size of the grid side.
-            dist (RandFunc): The random function used to generate edge weights.
-            rng (numpy.random.Generator): The random number generator.
-            center_node (int): The index of the center node.
-            lengths (dict): The lengths of the shortest paths from the source node
-                to all other nodes.
-            grid_lengths (CenteredGrid): The lengths of the shortest paths from the
-                source node in a grid format. The center node is at (0, 0). To get the
-                center node to be at (size_side // 2, size_side // 2), take the raw
-                array with grid_lengths.array.
-            nb_nodes (int): The number of nodes in the graph.
-            nb_edges (int): The number of edges in the graph.
-
-    Methods:
-    -------
-            compute_lengths: Apply the Dijkstra algorithm to compute the lengths of the
-                shortest paths from
-                the source node to all other nodes.
-            node_to_ij: Convert a node index to a (i, j) tuple.
-            plot_heatmap: Plot a heatmap of the lengths.
-
-    Examples:
-    --------
-    >>> import numpy as np
-    >>> from scipy.stats import expon
-    >>> from numpy.random import default_rng
-    >>> from matplotlib import pyplot as plt
-    >>> from first_passage_percolation.fpp import FirstPassagePercolation
-    >>> size_side = 11
-    >>> dist = expon(scale=1)
-    >>> rng = default_rng(0)
-    >>> fpp = FirstPassagePercolation(size_side, dist, rng).compute_lengths()
-    >>> fpp.plot_heatmap()
-    <matplotlib.image.AxesImage object at ...>
-
-    We can keep the same object and change the distribution:
-    >>> fpp.dist = expon(scale=2)
-    >>> fpp.compute_lengths().plot_heatmap()
-    <matplotlib.image.AxesImage object at ...>
-
-    """
-
-    def __init__(self, size_side, dist: Dist, rng=None):
-        n = size_side
-        self._size_side = size_side
-        self._graph = grid_graph(n, n)
-        self.dist = dist
-        self.rng = rng or np.random.default_rng()
-        self._lengths = None
-
-        check_size_grid(size_side)
-        if len(self.graph.edge_list()) != 2 * n * (n - 1):
-            msg = "The number of edges is not correct."
-            raise ValueError(msg)
-
-    def __repr__(self):
-        return (
-            "FirstPassagePercolation("
-            f"size_side={self.size_side}, "
-            f"dist={self.dist}, "
-            f"rng={self.rng}"
-            ")"
-        )
-
-    def __eq__(self, value):
-        if not isinstance(value, FirstPassagePercolation):
-            return False
-        return (
-            self.size_side == value.size_side
-            and self.dist == value.dist
-            and self.rng == value.rng
-        )
-
-    def __hash__(self):
-        return hash((self.size_side, self.dist, self.rng))
-
-    def _clear_lengths(self):
-        self._lengths = None
-        self._grid_lengths = None
-
-    def _set_lengths(self, lengths):
-        self._lengths = lengths
-        self._grid_lengths = CenteredGrid(self._get_grid_lengths_positive_indices())
-        self._grid_lengths.array.flags.writeable = False  # make the array read-only
-
-    @property
-    def lengths(self):
-        if self._lengths is None:
-            msg = (
-                "Lengths have not been set yet. "
-                "Call the compute_lengths() method first."
-            )
-            raise ValueError(msg)
-        return self._lengths
-
-    @property
-    def graph(self):
-        return self._graph
-
-    @property
-    def size_side(self):
-        return self._size_side
-
-    @property
-    def dist(self):
-        return self._dist
-
-    @dist.setter
-    def dist(self, value: Dist):
-        self._dist = value
-        self._clear_lengths()
-
-    @property
-    def rng(self):
-        return self._rng
-
-    @rng.setter
-    def rng(self, value):
-        self._rng = value
-        self._clear_lengths()
-
-    @size_side.setter
-    def size_side(self, value):
-        self._size_side = value
-        self._graph = grid_graph(value, value)
-
-    @property
-    def nb_nodes(self):
-        return self.size_side**2
-
-    @property
-    def nb_edges(self):
-        n = self.size_side
-        return 2 * n * (n - 1)
-
-    @property
-    def center_node(self):
-        n = self.size_side
-        return (n - 1) // 2 * (n + 1)
-
-    @property
-    def grid_lengths(self):
-        if self._grid_lengths is None:
-            msg = (
-                "Grid lengths have not been set yet. "
-                "Call the compute_lengths() method first."
-            )
-            raise ValueError(msg)
-        return self._grid_lengths
-
-    def compute_lengths(self):
-        """Apply the Dijkstra algorithm to compute the lengths of the shortest
-        paths from the source node to all other nodes.
-
-        Returns
-        -------
-            FirstPassagePercolation: The object itself.
-
-        """
-        # initialize the random number generator, so that we can reproduce the results
-        rng = copy.deepcopy(self.rng)
-
-        # _lengths is a dict node_id(int): length
-        lengths = _get_lengths(
-            self.graph, self.center_node, self.dist, rng, self.nb_edges
-        )
-        # 0 is omitted in the dict, so we add it manually
-        lengths[self.center_node] = 0
-        self._set_lengths(lengths)
-        return self
-
-    def node_to_ij(self, node):
-        """Convert a node index to a (i, j) tuple.
-
-        Args:
-        ----
-            node (int | np.ndarray): The node index or indices.
-
-        Returns:
-        -------
-            tuple: The (i, j) tuple. If node is an array, the output is
-                (array of i, array of j)
-
-        """
-        n = self.size_side
-        row, col = np.divmod(node, n)
-        return row - n // 2, col - n // 2
-
-    def _get_grid_lengths_positive_indices(self):
-        """Return a size_side x size_side array of the lengths from the source node."""
-        grid = np.zeros(self.nb_nodes, dtype=float)
-        lengths = self.lengths
-        indices = np.fromiter(lengths.keys(), dtype=int, count=self.nb_nodes - 1)
-        vals = np.fromiter(lengths.values(), dtype=float, count=self.nb_nodes - 1)
-        grid[indices] = vals
-        return grid.reshape(self.size_side, self.size_side)
-
-    def plot_heatmap(self, ax=None, **kwargs):
-        """Plot a heatmap of the lengths.
-
-        Args:
-        ----
-            ax (Axes | None): The matplotlib axes.
-            **kwargs: Additional arguments passed to plt.imshow
-                (cmap, interpolation, etc.).
-
-        """
-        ax = ax or plt.gca()
-        return ax.imshow(self.grid_lengths.array, **kwargs)
-
-    def plot_progression(self, t, ax=None, colors=("red", "white"), **kwargs):
-        """Draw the set T(t) := {i : L(i) <= t} in the first color
-        and its complement in the second color.
-
-        Args:
-        ----
-            t (float): The threshold.
-            ax (Axes | None): The matplotlib axes.
-            colors (tuple[str, str]): The colors of the two sets.
-            **kwargs: Additional arguments passed to plt.plot.
-
-        """
-        ax = ax or plt.gca()
-
-        grid = self.grid_lengths.array
-        cmap = mpl_colors.ListedColormap(tuple(reversed(colors)))
-        ax.imshow(grid <= t, cmap=cmap, **kwargs)
-        return ax
-
-
-def lengths_varying_param(
-    dist_func, range_x, size_side, rng, *, positive_indices=False
-):
-    """Generate the grid lengths with varying parameters of the distribution that
-    describes the random edge weights.
-
-    Args:
-    ----
-        dist_func: A function that takes a parameter and return the distribution of
-            the random edge weights.
-        range_x: An iterable representing the range of parameter values.
-        size_side: The size of the grid side.
-        rng: The random number generator.
-        positive_indices (bool): If True, the every index is positive and the center
-            node is at (size_side // 2, size_side // 2). Otherwise, the center node
-            is at (0, 0). Defaults to False.
-
-    Yields:
-    ------
-        The grid lengths with positive indices for each parameter value.
-
-    """
-    it = iter(range_x)
-    ffp = FirstPassagePercolation(size_side, dist_func(next(it)), rng).compute_lengths()
-
-    def get_lengths(ffp):
-        if positive_indices:
-            return ffp.grid_lengths.array
-        return ffp.grid_lengths
-
-    yield get_lengths(ffp)
-    for i in it:
-        ffp.dist = dist_func(i)
-        ffp.compute_lengths()
-        yield get_lengths(ffp)
-
-
-def plot_lengths_varying_param(
-    dist_func, range_x, size_side, rng, *, nb_cols=1, name_x="Parameter", **kwargs
-):
-    """Plot the grid lengths with varying parameters.
-
-    Args:
-    ----
-        dist_func: A function that takes a parameter and return the distribution of
-            the random edge weights.
-        range_x: An iterable representing the range of parameter values.
-        size_side: The size of the grid side.
-        rng: The random number generator.
-        nb_cols: The number of columns in the plot.
-        name_x: The name of the parameter (appear in the title of each subplot)
-        **kwargs: Additional arguments passed to plt.imshow (cmap, interpolation, etc.).
-
-    """
-    nb_vars = len(range_x)
-    nb_rows = nb_vars // nb_cols + (nb_vars % nb_cols != 0)
-    fig, axes = plt.subplots(nb_rows, nb_cols, figsize=(5 * nb_cols, 5 * nb_rows))
-    all_mat = lengths_varying_param(
-        dist_func, range_x, size_side, rng, positive_indices=True
-    )
-    for ax, grid_lengths, x in zip(axes.ravel(), all_mat, range_x, strict=False):
-        ax.imshow(grid_lengths, **kwargs)
-        ax.set_title(f"{name_x} = {x:.2f}")
-    return fig, axes
+from __future__ import annotations
+
+import copy
+import functools
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any, Protocol
+
+import matplotlib.pyplot as plt
+import numpy as np
+import rustworkx as rw
+from matplotlib import colors as mpl_colors
+from rustworkx.generators import grid_graph
+
+if TYPE_CHECKING:
+    from numpy.random import Generator
+
+
+def check_size_grid(size: int):
+    if size % 2 == 0:
+        msg = "The size of the grid side must be an odd number."
+        raise ValueError(msg)
+
+
+@dataclass
+class CenteredGrid:
+    """
+    Represents a centered grid. That is, the center is at (0, 0) and
+    the indices are from -size_side // 2 to size_side // 2 - 1.
+
+    Attributes
+    ----------
+        array (np.ndarray): The 2-dimensional array representing the grid.
+
+    Properties:
+        size_side (int): The size of one side of the grid.
+        start_index (int): The start index of the grid i.e. -size_side // 2.
+        end_index (int): The end index of the grid i.e. size_side // 2 - 1.
+
+    Methods
+    -------
+        __getitem__(key): Get the value at the specified key in the grid.
+        __setitem__(key, value): Set the value at the specified key in the grid.
+
+    Raises
+    ------
+        ValueError: If the array is not 2-dimensional.
+        IndexError: If the index is out of bounds, i.e., less than -size_side // 2
+            or greater than or equal to size_side // 2.
+
+    """
+
+    array: np.ndarray
+
+    def __post_init__(self):
+        if self.array.ndim != 2:  # noqa: PLR2004
+            msg = "The array must be 2-dimensional."
+            raise ValueError(msg)
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}({self.array})"
+
+    def __str__(self):
+        name = self.__class__.__name__
+        indent = " " * len(name)
+        array_str = np.array2string(
+            self.array, separator=", ", prefix=indent, suffix=","
+        )
+        return f"{name}(\n{indent}{array_str}\n)"
+
+    @property
+    def size_side(self):
+        return self.array.shape[0]
+
+    @property
+    def start_index(self):
+        return -self._center
+
+    @property
+    def end_index(self):
+        return self._center - 1
+
+    @property
+    def _center(self):
+        return self.size_side // 2
+
+    def _transform_index(self, key: int | slice):
+        if isinstance(key, slice):
+            start, stop, step = key.start, key.stop, key.step
+            return slice(
+                self._transform_index(start) if start is not None else None,
+                self._transform_index(stop) if stop is not None else None,
+                step,
+            )
+
+        key_arr = np.asarray(key)
+
+        if (key_arr < -self._center).any() or (key_arr >= self._center).any():
+            msg = f"Index {key} is out of bounds."
+            raise IndexError(msg)
+        return key + self._center
+
+    def _transform_key(self, key: int | tuple) -> Any:
+        if isinstance(key, tuple):
+            return tuple(map(self._transform_index, key))
+        return self._transform_index(key)
+
+    def __getitem__(self, key):
+        key = self._transform_key(key)
+        return self.array[key]
+
+    def __setitem__(self, key, value):
+        key = self._transform_key(key)
+        self.array[key] = value
+
+
+class Dist(Protocol):
+    def rvs(self, size: int, random_state: Generator) -> np.ndarray: ...
+
+
+@functools.cache
+def _get_lengths(graph: rw.PyGraph, source_node: int, dist: Dist, rng, nb_edges):
+    x = dist.rvs(size=nb_edges, random_state=rng)
+    i = 0
+
+    def weight_func(_):
+        nonlocal i
+        w = x[i]
+        i += 1
+        return w
+
+    return dict(rw.dijkstra_shortest_path_lengths(graph, source_node, weight_func))
+
+
+class FirstPassagePercolation:
+    """
+    Represents a First Passage Percolation simulation.
+        Each attribute can be modified after the object creation, except
+        for the graph. However, some changes may require recomputing the lengths by
+        calling the compute_lengths() method.
+
+    Args:
+    ----
+            size_side (int): The size of the grid side.
+            dist (Dist): The distribution object of the
+                random edge weights.
+            rng (numpy.random.Generator, optional): The random number generator.
+                Defaults to np.random.default_rng().
+
+    Attributes:
+    ----------
+            graph (Graph): The grid graph representing the simulation.
+            size_side (int): The size of the grid side.
+            dist (RandFunc): The random function used to generate edge weights.
+            rng (numpy.random.Generator): The random number generator.
+            center_node (int): The index of the center node.
+            lengths (dict): The lengths of the shortest paths from the source node
+                to all other nodes.
+            grid_lengths (CenteredGrid): The lengths of the shortest paths from the
+                source node in a grid format. The center node is at (0, 0). To get the
+                center node to be at (size_side // 2, size_side // 2), take the raw
+                array with grid_lengths.array.
+            nb_nodes (int): The number of nodes in the graph.
+            nb_edges (int): The number of edges in the graph.
+
+    Methods:
+    -------
+            compute_lengths: Apply the Dijkstra algorithm to compute the lengths of the
+                shortest paths from
+                the source node to all other nodes.
+            node_to_ij: Convert a node index to a (i, j) tuple.
+            plot_heatmap: Plot a heatmap of the lengths.
+
+    Examples:
+    --------
+    >>> import numpy as np
+    >>> from scipy.stats import expon
+    >>> from numpy.random import default_rng
+    >>> from matplotlib import pyplot as plt
+    >>> from first_passage_percolation.fpp import FirstPassagePercolation
+    >>> size_side = 11
+    >>> dist = expon(scale=1)
+    >>> rng = default_rng(0)
+    >>> fpp = FirstPassagePercolation(size_side, dist, rng).compute_lengths()
+    >>> fpp.plot_heatmap()
+    <matplotlib.image.AxesImage object at ...>
+
+    We can keep the same object and change the distribution:
+    >>> fpp.dist = expon(scale=2)
+    >>> fpp.compute_lengths().plot_heatmap()
+    <matplotlib.image.AxesImage object at ...>
+
+    """
+
+    def __init__(self, size_side, dist: Dist, rng=None):
+        n = size_side
+        self._size_side = size_side
+        self._graph = grid_graph(n, n)
+        self.dist = dist
+        self.rng = rng or np.random.default_rng()
+        self._lengths = None
+
+        check_size_grid(size_side)
+        if len(self.graph.edge_list()) != 2 * n * (n - 1):
+            msg = "The number of edges is not correct."
+            raise ValueError(msg)
+
+    def __repr__(self):
+        return (
+            "FirstPassagePercolation("
+            f"size_side={self.size_side}, "
+            f"dist={self.dist}, "
+            f"rng={self.rng}"
+            ")"
+        )
+
+    def __eq__(self, value):
+        if not isinstance(value, FirstPassagePercolation):
+            return False
+        return (
+            self.size_side == value.size_side
+            and self.dist == value.dist
+            and self.rng == value.rng
+        )
+
+    def __hash__(self):
+        return hash((self.size_side, self.dist, self.rng))
+
+    def _clear_lengths(self):
+        self._lengths = None
+        self._grid_lengths = None
+
+    def _set_lengths(self, lengths):
+        self._lengths = lengths
+        self._grid_lengths = CenteredGrid(self._get_grid_lengths_positive_indices())
+        self._grid_lengths.array.flags.writeable = False  # make the array read-only
+
+    @property
+    def lengths(self):
+        if self._lengths is None:
+            msg = (
+                "Lengths have not been set yet. "
+                "Call the compute_lengths() method first."
+            )
+            raise ValueError(msg)
+        return self._lengths
+
+    @property
+    def graph(self):
+        return self._graph
+
+    @property
+    def size_side(self):
+        return self._size_side
+
+    @property
+    def dist(self):
+        return self._dist
+
+    @dist.setter
+    def dist(self, value: Dist):
+        self._dist = value
+        self._clear_lengths()
+
+    @property
+    def rng(self):
+        return self._rng
+
+    @rng.setter
+    def rng(self, value):
+        self._rng = value
+        self._clear_lengths()
+
+    @size_side.setter
+    def size_side(self, value):
+        self._size_side = value
+        self._graph = grid_graph(value, value)
+
+    @property
+    def nb_nodes(self):
+        return self.size_side**2
+
+    @property
+    def nb_edges(self):
+        n = self.size_side
+        return 2 * n * (n - 1)
+
+    @property
+    def center_node(self):
+        n = self.size_side
+        return (n - 1) // 2 * (n + 1)
+
+    @property
+    def grid_lengths(self):
+        if self._grid_lengths is None:
+            msg = (
+                "Grid lengths have not been set yet. "
+                "Call the compute_lengths() method first."
+            )
+            raise ValueError(msg)
+        return self._grid_lengths
+
+    def compute_lengths(self):
+        """
+        Apply the Dijkstra algorithm to compute the lengths of the shortest
+        paths from the source node to all other nodes.
+
+        Returns
+        -------
+            FirstPassagePercolation: The object itself.
+
+        """
+        # initialize the random number generator, so that we can reproduce the results
+        rng = copy.deepcopy(self.rng)
+
+        # _lengths is a dict node_id(int): length
+        lengths = _get_lengths(
+            self.graph, self.center_node, self.dist, rng, self.nb_edges
+        )
+        # 0 is omitted in the dict, so we add it manually
+        lengths[self.center_node] = 0
+        self._set_lengths(lengths)
+        return self
+
+    def node_to_ij(self, node):
+        """
+        Convert a node index to a (i, j) tuple.
+
+        Args:
+        ----
+            node (int | np.ndarray): The node index or indices.
+
+        Returns:
+        -------
+            tuple: The (i, j) tuple. If node is an array, the output is
+                (array of i, array of j)
+
+        """
+        n = self.size_side
+        row, col = np.divmod(node, n)
+        return row - n // 2, col - n // 2
+
+    def _get_grid_lengths_positive_indices(self):
+        """Return a size_side x size_side array of the lengths from the source node."""
+        grid = np.zeros(self.nb_nodes, dtype=float)
+        lengths = self.lengths
+        indices = np.fromiter(lengths.keys(), dtype=int, count=self.nb_nodes - 1)
+        vals = np.fromiter(lengths.values(), dtype=float, count=self.nb_nodes - 1)
+        grid[indices] = vals
+        return grid.reshape(self.size_side, self.size_side)
+
+    def plot_heatmap(self, ax=None, **kwargs):
+        """
+        Plot a heatmap of the lengths.
+
+        Args:
+        ----
+            ax (Axes | None): The matplotlib axes.
+            **kwargs: Additional arguments passed to plt.imshow
+                (cmap, interpolation, etc.).
+
+        """
+        ax = ax or plt.gca()
+        return ax.imshow(self.grid_lengths.array, **kwargs)
+
+    def plot_progression(self, t, ax=None, colors=("red", "white"), **kwargs):
+        """
+        Draw the set T(t) := {i : L(i) <= t} in the first color
+        and its complement in the second color.
+
+        Args:
+        ----
+            t (float): The threshold.
+            ax (Axes | None): The matplotlib axes.
+            colors (tuple[str, str]): The colors of the two sets.
+            **kwargs: Additional arguments passed to plt.plot.
+
+        """
+        ax = ax or plt.gca()
+
+        grid = self.grid_lengths.array
+        cmap = mpl_colors.ListedColormap(tuple(reversed(colors)))
+        ax.imshow(grid <= t, cmap=cmap, **kwargs)
+        return ax
+
+
+def lengths_varying_param(
+    dist_func, range_x, size_side, rng, *, positive_indices=False
+):
+    """
+    Generate the grid lengths with varying parameters of the distribution that
+    describes the random edge weights.
+
+    Args:
+    ----
+        dist_func: A function that takes a parameter and return the distribution of
+            the random edge weights.
+        range_x: An iterable representing the range of parameter values.
+        size_side: The size of the grid side.
+        rng: The random number generator.
+        positive_indices (bool): If True, the every index is positive and the center
+            node is at (size_side // 2, size_side // 2). Otherwise, the center node
+            is at (0, 0). Defaults to False.
+
+    Yields:
+    ------
+        The grid lengths with positive indices for each parameter value.
+
+    """
+    it = iter(range_x)
+    ffp = FirstPassagePercolation(size_side, dist_func(next(it)), rng).compute_lengths()
+
+    def get_lengths(ffp):
+        if positive_indices:
+            return ffp.grid_lengths.array
+        return ffp.grid_lengths
+
+    yield get_lengths(ffp)
+    for i in it:
+        ffp.dist = dist_func(i)
+        ffp.compute_lengths()
+        yield get_lengths(ffp)
+
+
+def plot_lengths_varying_param(
+    dist_func, range_x, size_side, rng, *, nb_cols=1, name_x="Parameter", **kwargs
+):
+    """
+    Plot the grid lengths with varying parameters.
+
+    Args:
+    ----
+        dist_func: A function that takes a parameter and return the distribution of
+            the random edge weights.
+        range_x: An iterable representing the range of parameter values.
+        size_side: The size of the grid side.
+        rng: The random number generator.
+        nb_cols: The number of columns in the plot.
+        name_x: The name of the parameter (appear in the title of each subplot)
+        **kwargs: Additional arguments passed to plt.imshow (cmap, interpolation, etc.).
+
+    """
+    nb_vars = len(range_x)
+    nb_rows = nb_vars // nb_cols + (nb_vars % nb_cols != 0)
+    fig, axes = plt.subplots(nb_rows, nb_cols, figsize=(5 * nb_cols, 5 * nb_rows))
+    all_mat = lengths_varying_param(
+        dist_func, range_x, size_side, rng, positive_indices=True
+    )
+    for ax, grid_lengths, x in zip(axes.ravel(), all_mat, range_x, strict=False):
+        ax.imshow(grid_lengths, **kwargs)
+        ax.set_title(f"{name_x} = {x:.2f}")
+    return fig, axes
```

### Comparing `first_passage_percolation_sim-0.1.1/src/first_passage_percolation_sim/fpp.pyi` & `first_passage_percolation_sim-0.1.2/src/first_passage_percolation_sim/fpp.pyi`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-from collections.abc import Callable, Generator, Iterable
-from dataclasses import dataclass
-from typing import Any, Literal, Protocol, Self, overload
-
-from matplotlib.axes import Axes
-from matplotlib.figure import Figure
-from matplotlib.image import AxesImage
-from numpy import floating, random, signedinteger
-from numpy.typing import NBitBase, NDArray
-from rustworkx import PyGraph
-
-type FloatArray = NDArray[floating[Any]]
-
-def check_size_grid(size: int) -> None: ...
-@dataclass
-class CenteredGrid:
-    array: FloatArray
-    def __post_init__(self) -> None: ...
-    @property
-    def size_side(self) -> int: ...
-    @property
-    def start_index(self) -> int: ...
-    @property
-    def end_index(self) -> int: ...
-    def __getitem__(self, key) -> FloatArray | float: ...
-    def __setitem__(self, key, value) -> None: ...
-
-class Dist(Protocol):
-    def rvs(self, size: int, random_state: random.Generator) -> NDArray: ...
-
-class FirstPassagePercolation:
-    def __init__(
-        self, size_side: int, dist: Dist, rng: random.Generator | None = None
-    ) -> None: ...
-    def __eq__(self, value: object) -> bool: ...
-    def __hash__(self) -> int: ...
-    @property
-    def lengths(self): ...
-    @property
-    def graph(self) -> PyGraph[int, float]: ...
-    @property
-    def size_side(self) -> int: ...
-    @property
-    def dist(self) -> Dist: ...
-    @dist.setter
-    def dist(self, value: Dist) -> None: ...
-    @property
-    def rng(self) -> random.Generator: ...
-    @rng.setter
-    def rng(self, value: random.Generator) -> None: ...
-    @size_side.setter
-    def size_side(self, value: int) -> None: ...
-    @property
-    def nb_nodes(self) -> int: ...
-    @property
-    def nb_edges(self) -> int: ...
-    @property
-    def center_node(self) -> int: ...
-    @property
-    def grid_lengths(self) -> CenteredGrid: ...
-    def compute_lengths(self) -> Self: ...
-    def node_to_ij(
-        self, node: int | NDArray
-    ) -> tuple[
-        int | NDArray[signedinteger[Any]], int | NDArray[signedinteger[Any]]
-    ]: ...
-    def plot_heatmap(self, ax: Axes | None = None, **kwargs) -> AxesImage: ...
-    def plot_progression(
-        self, t: float, ax: Axes | None = None, colors: tuple[str, str] = ..., **kwargs
-    ) -> Axes: ...
-
-@overload
-def lengths_varying_param[T](
-    dist_func: Callable[[T], Dist],
-    range_x: Iterable[T],
-    size_side: int,
-    rng: random.Generator,
-    *,
-    positive_indices: Literal[True],
-) -> Generator[NDArray, Any, None]: ...
-@overload
-def lengths_varying_param[T](
-    dist_func: Callable[[T], Dist],
-    range_x: Iterable[T],
-    size_side: int,
-    rng: random.Generator,
-    *,
-    positive_indices: Literal[False] = False,
-) -> Generator[CenteredGrid, Any, None]: ...
-def lengths_varying_param[T](
-    dist_func: Callable[[T], Dist],
-    range_x: Iterable[T],
-    size_side: int,
-    rng: random.Generator,
-    *,
-    positive_indices: bool = False,
-) -> Generator[NDArray | CenteredGrid, Any, None]: ...
-def plot_lengths_varying_param[T](
-    dist_func: Callable[[T], Dist],
-    range_x: Iterable[T],
-    size_side: int,
-    rng: random.Generator,
-    nb_cols=1,
-    name_x: str = ...,
-    **kwargs,
-) -> tuple[Figure, Axes]: ...
+from collections.abc import Callable, Generator, Iterable
+from dataclasses import dataclass
+from typing import Any, Literal, Protocol, Self, overload
+
+from matplotlib.axes import Axes
+from matplotlib.figure import Figure
+from matplotlib.image import AxesImage
+from numpy import floating, random, signedinteger
+from numpy.typing import NBitBase, NDArray
+from rustworkx import PyGraph
+
+type FloatArray = NDArray[floating[Any]]
+
+def check_size_grid(size: int) -> None: ...
+@dataclass
+class CenteredGrid:
+    array: FloatArray
+    def __post_init__(self) -> None: ...
+    @property
+    def size_side(self) -> int: ...
+    @property
+    def start_index(self) -> int: ...
+    @property
+    def end_index(self) -> int: ...
+    def __getitem__(self, key) -> FloatArray | float: ...
+    def __setitem__(self, key, value) -> None: ...
+
+class Dist(Protocol):
+    def rvs(self, size: int, random_state: random.Generator) -> NDArray: ...
+
+class FirstPassagePercolation:
+    def __init__(
+        self, size_side: int, dist: Dist, rng: random.Generator | None = None
+    ) -> None: ...
+    def __eq__(self, value: object) -> bool: ...
+    def __hash__(self) -> int: ...
+    @property
+    def lengths(self): ...
+    @property
+    def graph(self) -> PyGraph[int, float]: ...
+    @property
+    def size_side(self) -> int: ...
+    @property
+    def dist(self) -> Dist: ...
+    @dist.setter
+    def dist(self, value: Dist) -> None: ...
+    @property
+    def rng(self) -> random.Generator: ...
+    @rng.setter
+    def rng(self, value: random.Generator) -> None: ...
+    @size_side.setter
+    def size_side(self, value: int) -> None: ...
+    @property
+    def nb_nodes(self) -> int: ...
+    @property
+    def nb_edges(self) -> int: ...
+    @property
+    def center_node(self) -> int: ...
+    @property
+    def grid_lengths(self) -> CenteredGrid: ...
+    def compute_lengths(self) -> Self: ...
+    def node_to_ij(
+        self, node: int | NDArray
+    ) -> tuple[
+        int | NDArray[signedinteger[Any]], int | NDArray[signedinteger[Any]]
+    ]: ...
+    def plot_heatmap(self, ax: Axes | None = None, **kwargs) -> AxesImage: ...
+    def plot_progression(
+        self, t: float, ax: Axes | None = None, colors: tuple[str, str] = ..., **kwargs
+    ) -> Axes: ...
+
+@overload
+def lengths_varying_param[T](
+    dist_func: Callable[[T], Dist],
+    range_x: Iterable[T],
+    size_side: int,
+    rng: random.Generator,
+    *,
+    positive_indices: Literal[True],
+) -> Generator[NDArray, Any, None]: ...
+@overload
+def lengths_varying_param[T](
+    dist_func: Callable[[T], Dist],
+    range_x: Iterable[T],
+    size_side: int,
+    rng: random.Generator,
+    *,
+    positive_indices: Literal[False] = False,
+) -> Generator[CenteredGrid, Any, None]: ...
+def lengths_varying_param[T](
+    dist_func: Callable[[T], Dist],
+    range_x: Iterable[T],
+    size_side: int,
+    rng: random.Generator,
+    *,
+    positive_indices: bool = False,
+) -> Generator[NDArray | CenteredGrid, Any, None]: ...
+def plot_lengths_varying_param[T](
+    dist_func: Callable[[T], Dist],
+    range_x: Iterable[T],
+    size_side: int,
+    rng: random.Generator,
+    nb_cols=1,
+    name_x: str = ...,
+    **kwargs,
+) -> tuple[Figure, Axes]: ...
```

### Comparing `first_passage_percolation_sim-0.1.1/LICENSE` & `first_passage_percolation_sim-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-MIT License
-
-Copyright (c) 2024-present arnaud-ma <arnaudma.code@gmail.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+MIT License
+
+Copyright (c) 2024-present arnaud-ma <arnaudma.code@gmail.com>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `first_passage_percolation_sim-0.1.1/pyproject.toml` & `first_passage_percolation_sim-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,131 +1,133 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "first-passage-percolation-sim"
-version = "0.1.1"
-description = 'Simulations of the first passage percolation on the square lattice'
-readme = "README.md"
-requires-python = ">=3.12"
-license = "MIT"
-keywords = [
-  "first-passage-percolation",
-  "percolation",
-  "simulation",
-  "square-lattice",
-  "probability",
-  "graph-theory",
-]
-authors = [{ name = "arnaud-ma", email = "arnaudma.code@gmail.com" }]
-classifiers = [
-  "Development Status :: 4 - Beta",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3.12",
-  "Programming Language :: Python :: Implementation :: CPython",
-]
-dependencies = ["numpy >= 1.26", "rustworkx >= 0.14", "matplotlib >= 3.8"]
-
-[project.urls]
-Documentation = "https://github.com/unknown/first-passage-percolation#readme"
-Issues = "https://github.com/unknown/first-passage-percolation/issues"
-Source = "https://github.com/unknown/first-passage-percolation"
-
-
-[tool.ruff]
-fix = true
-preview = true
-unsafe-fixes = false
-line-length = 88
-src = ["src", "tests"]
-
-[tool.ruff.format]
-indent-style = "space"
-docstring-code-format = true
-docstring-code-line-length = 72
-skip-magic-trailing-comma = true
-
-[tool.ruff.lint]
-preview = true
-extend-select = ["ALL"]
-extend-ignore = [
-  # undocumented docstrings
-  "D100", # public module
-  "D101", # public class
-  "D102", # public method
-  "D103", # public function
-  "D104", # public package
-  "D105", # magic method
-  "D106", # public nested class
-  "D107", # public init method
-  "D205", # blank line after summary
-  # ^todo tags
-  "TD002",  # author on TODO tag
-  "TD003",  # link on TODO tag
-  "FIX002", # check for todo tags
-
-  "SLF001", # private member
-  "CPY",    # Copyrigth
-  "ANN",    # Annotations
-  "ARG001", # unused func arguments
-  "ARG002", # unused method arguments
-  "RET506", # Unnecessary `elif` after `raise` statement"
-  "PGH003", # code-error on type: ignore
-
-  # conflicts with formatter https://docs.astral.sh/ruff/formatter/#conflicting-lint-rules
-  "W191",   # tab indent
-  "W293",   # blank line at end of file
-  "E111",   # indentation is not a multiple of four
-  "E114",   # indentation is not a multiple of four (comment)
-  "E117",   # over-indented
-  "E301",   # expected 1 blank line, found 0
-  "E302",   # expected 2 blank lines, found 1
-  "E305",   # expected 2 blank lines after class or function definition, found 1
-  "E701",   # multiple statements on one line (colon)
-  "E702",   # multiple statements on one line (semicolon)
-  "E703",   # statement ends with a semicolon
-  "D206",   # Docstring is indented
-  "D300",   # Use """triple double quotes"""
-  "COM812", # missing trailing comma
-  "COM819", # trailing comma in a tuple
-  "ISC001", # missing space after comma
-  "ISC002", # missing space before comma
-  "I001",   # isort
-
-  # debug
-  "T201", # print statements
-
-  # Unwanted
-  "FURB140", # itertools.starmap instead of comprehension
-  "PLR0904", # too many public methods
-  "ERA001",  # commented code
-
-  # Conflicts with the ide
-  "F841", # local variable is assigned to but never used
-
-  "EXE", # executable (shebang, etc.)
-]
-
-[tool.ruff.lint.pylint]
-max-args = 10
-
-
-[tool.ruff.lint.extend-per-file-ignores]
-"*.pyi" = ["E999", "F401", "E501"]                # syntax error, unused import, line too long
-"__init__.py" = ["F401"]
-"*.ipynb" = ["F401"]                              # unused import
-"tests/*" = ["S", "PLR2004", "PLR6301", "TID252"]
-
-
-[tool.pyright]
-# deactivate pyright features that are already covered by ruff
-# actually only enables type checking
-# https://microsoft.github.io/pyright/#/configuration?id=diagnostic-rule-defaults for more info
-typeCheckingMode = "standard"
-reportGeneralTypeIssues = true
-reportMissingTypeStubs = false
-reportUndefinedVariable = false
-reportUnusedVariable = false
-reportUnusedClass = false
-reportUnusedFunction = false
-reportUnaccessedMember = false
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "first-passage-percolation-sim"
+version = "0.1.2"
+description = 'Simulations of the first passage percolation on the square lattice'
+readme = "README.md"
+requires-python = ">=3.12"
+license = "MIT"
+keywords = [
+  "first-passage-percolation",
+  "percolation",
+  "simulation",
+  "square-lattice",
+  "probability",
+  "graph-theory",
+]
+authors = [{ name = "arnaud-ma", email = "arnaudma.code@gmail.com" }]
+classifiers = [
+  "Development Status :: 4 - Beta",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: Implementation :: CPython",
+]
+dependencies = ["numpy >= 1.26", "rustworkx >= 0.14", "matplotlib >= 3.8"]
+
+[project.urls]
+Documentation = "https://github.com/unknown/first-passage-percolation#readme"
+Issues = "https://github.com/unknown/first-passage-percolation/issues"
+Source = "https://github.com/unknown/first-passage-percolation"
+
+
+[tool.ruff]
+fix = true
+preview = true
+unsafe-fixes = false
+line-length = 88
+src = ["src", "tests"]
+
+[tool.ruff.format]
+indent-style = "space"
+docstring-code-format = true
+docstring-code-line-length = 72
+skip-magic-trailing-comma = true
+
+[tool.ruff.lint]
+preview = true
+extend-select = ["ALL"]
+extend-ignore = [
+  # undocumented docstrings
+  "D100", # public module
+  "D101", # public class
+  "D102", # public method
+  "D103", # public function
+  "D104", # public package
+  "D105", # magic method
+  "D106", # public nested class
+  "D107", # public init method
+  "D205", # blank line after summary
+  "D203", # blank line before class docstring
+  "D212", # multi-line docstring summary should start at the first line
+  # ^todo tags
+  "TD002",  # author on TODO tag
+  "TD003",  # link on TODO tag
+  "FIX002", # check for todo tags
+
+  "SLF001", # private member
+  "CPY",    # Copyrigth
+  "ANN",    # Annotations
+  "ARG001", # unused func arguments
+  "ARG002", # unused method arguments
+  "RET506", # Unnecessary `elif` after `raise` statement"
+  "PGH003", # code-error on type: ignore
+
+  # conflicts with formatter https://docs.astral.sh/ruff/formatter/#conflicting-lint-rules
+  "W191",   # tab indent
+  "W293",   # blank line at end of file
+  "E111",   # indentation is not a multiple of four
+  "E114",   # indentation is not a multiple of four (comment)
+  "E117",   # over-indented
+  "E301",   # expected 1 blank line, found 0
+  "E302",   # expected 2 blank lines, found 1
+  "E305",   # expected 2 blank lines after class or function definition, found 1
+  "E701",   # multiple statements on one line (colon)
+  "E702",   # multiple statements on one line (semicolon)
+  "E703",   # statement ends with a semicolon
+  "D206",   # Docstring is indented
+  "D300",   # Use """triple double quotes"""
+  "COM812", # missing trailing comma
+  "COM819", # trailing comma in a tuple
+  "ISC001", # missing space after comma
+  "ISC002", # missing space before comma
+  "I001",   # isort
+
+  # debug
+  "T201", # print statements
+
+  # Unwanted
+  "FURB140", # itertools.starmap instead of comprehension
+  "PLR0904", # too many public methods
+  "ERA001",  # commented code
+
+  # Conflicts with the ide
+  "F841", # local variable is assigned to but never used
+
+  "EXE", # executable (shebang, etc.)
+]
+
+[tool.ruff.lint.pylint]
+max-args = 10
+
+
+[tool.ruff.lint.extend-per-file-ignores]
+"*.pyi" = ["E999", "F401", "E501"]                # syntax error, unused import, line too long
+"__init__.py" = ["F401"]
+"*.ipynb" = ["F401"]                              # unused import
+"tests/*" = ["S", "PLR2004", "PLR6301", "TID252"]
+
+
+[tool.pyright]
+# deactivate pyright features that are already covered by ruff
+# actually only enables type checking
+# https://microsoft.github.io/pyright/#/configuration?id=diagnostic-rule-defaults for more info
+typeCheckingMode = "standard"
+reportGeneralTypeIssues = true
+reportMissingTypeStubs = false
+reportUndefinedVariable = false
+reportUnusedVariable = false
+reportUnusedClass = false
+reportUnusedFunction = false
+reportUnaccessedMember = false
```

### Comparing `first_passage_percolation_sim-0.1.1/PKG-INFO` & `first_passage_percolation_sim-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: first-passage-percolation-sim
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simulations of the first passage percolation on the square lattice
 Project-URL: Documentation, https://github.com/unknown/first-passage-percolation#readme
 Project-URL: Issues, https://github.com/unknown/first-passage-percolation/issues
 Project-URL: Source, https://github.com/unknown/first-passage-percolation
 Author-email: arnaud-ma <arnaudma.code@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -17,23 +17,23 @@
 Requires-Dist: matplotlib>=3.8
 Requires-Dist: numpy>=1.26
 Requires-Dist: rustworkx>=0.14
 Description-Content-Type: text/markdown
 
 # first passage percolation
 
-This package provides simulation tools for first passage percolation on the square lattice. See the [`example.ipynb`](github.com/arnaud-ma.com/example.ipynb) file for the usage of the package.
+This package provides simulation tools for first passage percolation on the square lattice. See the [`example.ipynb`](example.ipynb) file for the usage of the package.
 
 ## Simple example
 
 ```python
-import first_passage_percolation as fpp
+import first_passage_percolation_sim as fpp
 from scipy.stats import geom
 
-(fpp.FirstPassagePercolation(size=201, dist=stats.geom(0.5))
+(fpp.FirstPassagePercolation(size=201, dist=geom(0.5))
     .compute_lengths()
     .plot_heatmap(cmap="inferno")
 )
 ```
 
 <p align="center">
 <img src="doc/assets/heatmap_geom_0_5.png" alt="drawing" width="400"/>
```

