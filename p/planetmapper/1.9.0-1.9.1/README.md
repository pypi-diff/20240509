# Comparing `tmp/planetmapper-1.9.0.tar.gz` & `tmp/planetmapper-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.9.0.tar", last modified: Thu Feb  8 17:11:24 2024, max compression
+gzip compressed data, was "planetmapper-1.9.1.tar", last modified: Fri Feb 16 16:25:35 2024, max compression
```

## Comparing `planetmapper-1.9.0.tar` & `planetmapper-1.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 17:11:24.872730 planetmapper-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-08 17:11:09.000000 planetmapper-1.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-02-08 17:11:24.872730 planetmapper-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-02-08 17:11:09.000000 planetmapper-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 17:11:24.868730 planetmapper-1.9.0/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28760 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (127)   109346 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (127)   130670 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 17:11:24.868730 planetmapper-1.9.0/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/data/ring_aliases.json
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)   122623 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    55054 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-02-08 17:11:09.000000 planetmapper-1.9.0/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 17:11:24.872730 planetmapper-1.9.0/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-02-08 17:11:24.000000 planetmapper-1.9.0/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-08 17:11:24.000000 planetmapper-1.9.0/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 17:11:24.000000 planetmapper-1.9.0/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-08 17:11:24.000000 planetmapper-1.9.0/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-08 17:11:24.000000 planetmapper-1.9.0/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-08 17:11:24.000000 planetmapper-1.9.0/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-08 17:11:09.000000 planetmapper-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 17:11:24.872730 planetmapper-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-08 17:11:09.000000 planetmapper-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 17:11:24.872730 planetmapper-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (127)    70762 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (127)    66688 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    34427 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-02-08 17:11:09.000000 planetmapper-1.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 16:25:35.573273 planetmapper-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-16 16:25:22.000000 planetmapper-1.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-02-16 16:25:35.573273 planetmapper-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-02-16 16:25:22.000000 planetmapper-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 16:25:35.569273 planetmapper-1.9.1/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28760 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118674 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130871 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 16:25:35.569273 planetmapper-1.9.1/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/data/ring_aliases.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)   122623 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55054 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-02-16 16:25:22.000000 planetmapper-1.9.1/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 16:25:35.573273 planetmapper-1.9.1/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-02-16 16:25:35.000000 planetmapper-1.9.1/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-16 16:25:35.000000 planetmapper-1.9.1/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 16:25:35.000000 planetmapper-1.9.1/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-16 16:25:35.000000 planetmapper-1.9.1/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-16 16:25:35.000000 planetmapper-1.9.1/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-16 16:25:35.000000 planetmapper-1.9.1/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-16 16:25:22.000000 planetmapper-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 16:25:35.573273 planetmapper-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-16 16:25:22.000000 planetmapper-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 16:25:35.573273 planetmapper-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77527 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67827 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34427 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-02-16 16:25:22.000000 planetmapper-1.9.1/tests/test_utils.py
```

### Comparing `planetmapper-1.9.0/LICENSE.txt` & `planetmapper-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/PKG-INFO` & `planetmapper-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.9.0
+Version: 1.9.1
 Summary: PlanetMapper: A Python package for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
```

### Comparing `planetmapper-1.9.0/README.md` & `planetmapper-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/planetmapper/__init__.py` & `planetmapper-1.9.1/planetmapper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 The core logic of this code is based on conversion between different coordinate systems
 of interest. The `xy` and `radec` coordinate systems define positions from the point of
 view of the observer while the `lonlat` coordinate system defines locations on the
 surface of the target body:
 
 `xy`: image pixel coordinates. These coordinates count the number of pixels in an
-observed image with the bottom left pixel defined as `(0,0)`, and the `x` and `y`
+observed image with the bottom left pixel defined as `(0, 0)`, and the `x` and `y`
 coordinates defined as normal. Integer coordinates represent the middle of the
 corresponding pixel, so `(0, 3)` covers `x` values from -0.5 to 0.5 and `y` values from
 2.5 to 3.5.
 
 `radec`: observer frame RA/Dec sky coordinates. These are the right ascension and
 declination which define the position in the sky of a point from the point of view of
 the observer. These coordinates are expressed in degrees. See
```

### Comparing `planetmapper-1.9.0/planetmapper/base.py` & `planetmapper-1.9.1/planetmapper/base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/planetmapper/basic_body.py` & `planetmapper-1.9.1/planetmapper/basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/planetmapper/body.py` & `planetmapper-1.9.1/planetmapper/body.py`

 * *Files 6% similar despite different names*

```diff
@@ -2290,14 +2290,15 @@
             )
         return kwargs
 
     def _plot_wireframe(
         self,
         *,
         coordinate_func: Callable[[float, float], tuple[float, float]],
+        scale_factor: float | None,
         transform: matplotlib.transforms.Transform | None,
         aspect_adjustable: Literal['box', 'datalim'] | None,
         additional_array_func: (
             Callable[[Iterable, Iterable], tuple[np.ndarray, np.ndarray]] | None
         ) = None,
         ax: Axes | None = None,
         label_poles: bool = True,
@@ -2308,30 +2309,34 @@
         indicate_prime_meridian: bool = False,
         formatting: dict[WireframeComponent, dict[str, Any]] | None = None,
         **common_formatting,
     ) -> Axes:
         """
         Plot generic wireframe representation of the observation.
 
+        See :func:`plot_wireframe_radec` for more details on most arguments.
+
         Args:
             coordinate_func: Function to convert RA/Dec coordinates to the desired
                 coordinate system. Takes two arguments (RA, Dec) and returns two
                 values (x, y).
             transform: Matplotlib transform to apply to the plotted data, after
                 transforming with `coordinate_func`.
             additional_array_func: Function to apply to arrays of converted (x, y)
                 coordinates before plotting. Useful for adding NaNs to arrays to
                 handle wraparound in RA coordinates.
         """
         if ax is None:
             ax = cast(Axes, plt.gca())
+
         if transform is None:
-            transform = ax.transData
-        else:
-            transform = transform + ax.transData
+            transform = matplotlib.transforms.IdentityTransform()
+        if scale_factor is not None:
+            transform += matplotlib.transforms.Affine2D().scale(scale_factor)
+        transform += ax.transData
 
         def array_func(
             ras: np.ndarray, decs: np.ndarray
         ) -> tuple[np.ndarray, np.ndarray]:
             """Transform arrays of coords with coordinate_func"""
             xs, ys = zip(*(coordinate_func(ra, dec) for ra, dec in zip(ras, decs)))
             if additional_array_func is not None:
@@ -2439,62 +2444,67 @@
             ra_prev = ra
         return np.array(ra_out), np.array(dec_out)
 
     def plot_wireframe_radec(
         self,
         ax: Axes | None = None,
         *,
-        dms_ticks: bool = True,
-        add_axis_labels: bool = True,
+        scale_factor: float | None = None,
+        dms_ticks: bool | None = None,
+        add_axis_labels: bool | None = None,
         aspect_adjustable: Literal['box', 'datalim'] | None = 'datalim',
         use_shifted_meridian: bool = False,
         show: bool = False,
         **wireframe_kwargs: Unpack[WireframeKwargs],
     ) -> Axes:
         """
         Plot basic wireframe representation of the observation using RA/Dec sky
         coordinates.
 
         See also :func:`plot_wireframe_km`, :func:`plot_wireframe_angular` and
         :func:`BodyXY.plot_wireframe_xy` to plot the wireframe in other coordinate
-        systems.
+        systems. :func:`plot_wireframe_custom` can also be used to plot a wireframe
+        with a custom coordinate system.
+
+        .. hint::
+
+            See :ref:`the examples page <wireframes>` for more examples of creating
+            wireframe plots.
 
         To plot a wireframe with the default appearance, simply use: ::
 
             body.plot_wireframe_radec()
 
         To customise the appearance of the plot, you can use the `formatting` and
         `**kwargs` arguments which can be used to pass arguments to the Matplotlib
         plotting functions. The `formatting` argument can be used to customise
-        individual components, and the `**kwargs` argument can be used to customise
-        all components at once.
+        individual components, and the `**kwargs` argument can be used to customise all
+        components at once.
 
-        For example, to change the colour of the entire wireframe to red, you can
-        use: ::
+        For example, to change the colour of the entire wireframe to red, you can use:
+        ::
 
             body.plot_wireframe_radec(color='r')
 
         To change just the plotted terminator and dayside limb to red, use: ::
 
             body.plot_wireframe_radec(
                 formatting={
-                    'terminator': {'color': 'r'},
-                    'limb_illuminated': {'color': 'r'},
+                    'terminator': {'color': 'r'}, 'limb_illuminated': {'color': 'r'},
                 },
             )
 
         The order of precedence for the formatting is the `formatting` argument, then
-        `**kwargs`, then the default formatting. For example, the following plot will
-        be red with a thin blue grid and green poles: ::
+        `**kwargs`, then the default formatting. For example, the following plot will be
+        red with a thin blue grid and green poles: ::
 
             body.plot_wireframe_radec(
-                color='r',
-                formatting={
-                    'grid': {'color': 'b', 'linewidth': 0.5, 'linestyle': '-'},
-                    'pole': {'color': 'g'},
+                color='r', formatting={
+                    'grid': {'color': 'b', 'linewidth': 0.5, 'linestyle': '-'}, 'pole':
+                    {'color': 'g'},
                 },
             )
 
         Individual components can be hidden by setting `visible` to `False`. For
         example, to hide the terminator, use: ::
 
             body.plot_wireframe_radec(formatting={'terminator': {'visible': False}})
@@ -2506,57 +2516,81 @@
             import planetmapper
             planetmapper.DEFAULT_WIREFRAME_FORMATTING['grid']['color'] = 'b'
             planetmapper.DEFAULT_WIREFRAME_FORMATTING['grid']['linestyle'] = '--'
 
             body.plot_wireframe_radec() # This would have a blue dashed grid
             body.plot_wireframe_radec(color='r') # This would be red with a dashed grid
 
+        The units of the plotted data can be customised with the `scale_factor`
+        argument, which multiplies coordinates by the given `scale_factor` before
+        plotting. For example: ::
+
+            body.plot_wireframe_radec() # units of degrees
+            body.plot_wireframe_radec(scale_factor=3.14159/180) # units of radians
+
+            body.plot_wireframe_km() # units of km
+            body.plot_wireframe_km(scale_factor=1000) # units of m
+            body.plot_wireframe_km(scale_factor=1/body.r_eq) # units of planet radii
+
+            body.plot_wireframe_angular() # units of arcseconds
+            body.plot_wireframe_angular(scale_factor=1/60) # units of arcminutes
+            body.plot_wireframe_angular(scale_factor=1/3600) # units of degrees
+
         .. warning::
 
-            The plot may appear warped or distorted if the target is near the celestial
-            pole (i.e. the target's declination is near 90° or -90°). This is due to the
-            spherical nature of the RA/Dec coordinate system, which is impossible to
-            represent perfectly on a 2D cartesian plot.
+            Even though the numerical values will be correct, the plot may appear warped
+            or distorted if the target is near the celestial pole (i.e. the target's
+            declination is near 90° or -90°). This is due to the spherical nature of the
+            RA/Dec coordinate system, which is impossible to represent perfectly on a 2D
+            cartesian plot.
 
             :func:`plot_wireframe_angular` can be used as an alternative to
             :func:`plot_wireframe_radec` to plot the wireframe without distortion from
             the choice of coordinate system. By default, the `angular` coordinate system
             is centred on the target body, which minimises any distortion, but the
             origin and rotation of the `angular` coordinates can also be customised as
             needed (e.g. to align it with an instrument's field of view).
 
-        .. hint::
+        .. note::
 
             If the target body is near RA=0°, then the wireframe may be split over two
             halves of the plot. This can be fixed by using
             `body.plot_wireframe_radec(use_shifted_meridian=True)`, which will plot the
             wireframe with RA coordinates between -180° and 180°, rather than the
             default of 0° to 360°.
 
         Args:
             ax: Matplotlib axis to use for plotting. If `ax` is None (the default), uses
                 `plt.gca()` to get the currently active axis.
+            scale_factor: Custom scale factor to apply to the plotted wireframe. This
+                can be used to change units of the plot. If `scale_factor` is used, the
+                plotted coordinates will be multiplied by `scale_factor` before
+                plotting. See the examples above for more details.
             label_poles: Toggle labelling the poles of the target body.
             add_title: Add title generated by :func:`get_description` to the axis.
-            add_axis_labels: Add axis labels.
+            add_axis_labels: Add axis labels to the plot. If `add_axis_labels` is None
+                (the default), then labels will only be added if `scale_factor` is not
+                used.
             grid_interval: Spacing between grid lines in degrees.
             grid_lat_limit: Latitude limit for gridlines. For example, if
                 `grid_lat_limit=60`, then gridlines will only be plotted for latitudes
                 between 60°N and 60°S (inclusive). This can be useful to reduce visual
                 clutter around the poles.
             indicate_equator: Toggle indicating the equator with a solid line.
             indicate_prime_meridian: Toggle indicating the prime meridian with a solid
                 line.
             aspect_adjustable: Set `adjustable` parameter when setting the aspect ratio.
                 Passed to :func:`matplotlib.axes.Axes.set_aspect`. Set to None to skip
                 setting the aspect ratio (generally this is only recommended if you're
                 setting the aspect ratio yourself).
             dms_ticks: Toggle between showing ticks as degrees, minutes and seconds
                 (e.g. 12°34′56″) or decimal degrees (e.g. 12.582). This argument is only
-                applicable for :func:`plot_wireframe_radec`.
+                applicable for :func:`plot_wireframe_radec`. If `dms_ticks` is None (the
+                default), then ticks will only be shown as degrees, minutes and seconds
+                if `scale_factor` is not used.
             use_shifted_meridian: If `use_shifted_meridian=True`, plot the wireframe
                 with RA coordinates between -180° and 180°, rather than the default of
                 0° to 360°. This can be useful for bodies which lie at RA=0°, which can
                 be split over two halves of the plot with the default
                 `use_shifted_meridian=False`. This argument is only applicable for
                 :func:`plot_wireframe_radec`.
             show: Toggle immediately showing the plotted figure with `plt.show()`.
@@ -2585,21 +2619,28 @@
 
         Returns:
             The axis containing the plotted wireframe.
         """
         # TODO maybe add automated warning at high declinations and for ra wraparound
         # TODO maybe add some fixed upper xlim/ylim for RA/Dec plots
 
+        # By default, enable dms ticks and axis labels if scale_factor is not used
+        if dms_ticks is None:
+            dms_ticks = scale_factor is None
+        if add_axis_labels is None:
+            add_axis_labels = scale_factor is None
+
         if use_shifted_meridian:
             coordinate_func = lambda ra, dec: ((ra + 180.0) % 360.0 - 180.0, dec)
         else:
             coordinate_func = lambda ra, dec: (ra, dec)
 
         ax = self._plot_wireframe(
             coordinate_func=coordinate_func,
+            scale_factor=scale_factor,
             transform=None,
             aspect_adjustable=None,
             ax=ax,
             additional_array_func=self._add_nans_for_radec_array_wraparounds,
             **wireframe_kwargs,
         )
 
@@ -2615,28 +2656,33 @@
             plt.show()
         return ax
 
     def plot_wireframe_km(
         self,
         ax: Axes | None = None,
         *,
-        add_axis_labels: bool = True,
+        scale_factor: float | None = None,
+        add_axis_labels: bool | None = None,
         aspect_adjustable: Literal['box', 'datalim'] | None = 'datalim',
         show: bool = False,
         **wireframe_kwargs: Unpack[WireframeKwargs],
     ) -> Axes:
         """
         Plot basic wireframe representation of the observation on a target centred
         frame. See :func:`plot_wireframe_radec` for details of accepted arguments.
 
         Returns:
             The axis containing the plotted wireframe.
         """
+        if add_axis_labels is None:
+            add_axis_labels = scale_factor is None
+
         ax = self._plot_wireframe(
             coordinate_func=self.radec2km,
+            scale_factor=scale_factor,
             transform=None,
             aspect_adjustable=aspect_adjustable,
             ax=ax,
             **wireframe_kwargs,
         )
         if add_axis_labels:
             ax.set_xlabel('Projected distance (km)')
@@ -2650,15 +2696,16 @@
     def plot_wireframe_angular(
         self,
         ax: Axes | None = None,
         *,
         origin_ra: float | None = None,
         origin_dec: float | None = None,
         coordinate_rotation: float = 0.0,
-        add_axis_labels: bool = True,
+        scale_factor: float | None = None,
+        add_axis_labels: bool | None = None,
         aspect_adjustable: Literal['box', 'datalim'] | None = 'datalim',
         show: bool = False,
         **wireframe_kwargs: Unpack[WireframeKwargs],
     ) -> Axes:
         """
         Plot basic wireframe representation of the observation on a relative angular
         coordinate frame. See :func:`plot_wireframe_radec` for details of accepted
@@ -2678,27 +2725,156 @@
             origin. This is because spherical coordinates are impossible to represent
             perfectly on a 2D cartesian plot. By default, the `angular` coordinates are
             centred on the target body, minimising any distortion.
 
         Returns:
             The axis containing the plotted wireframe.
         """
+        if add_axis_labels is None:
+            add_axis_labels = scale_factor is None
+
         ax = self._plot_wireframe(
             coordinate_func=lambda ra, dec: self.radec2angular(
                 ra,
                 dec,
                 origin_ra=origin_ra,
                 origin_dec=origin_dec,
                 coordinate_rotation=coordinate_rotation,
             ),
+            scale_factor=scale_factor,
             transform=None,
             aspect_adjustable=aspect_adjustable,
             ax=ax,
             **wireframe_kwargs,
         )
         if add_axis_labels:
             ax.set_xlabel('Angular distance (arcsec)')
             ax.set_ylabel('Angular distance (arcsec)')
 
         if show:
             plt.show()
         return ax
+
+    def plot_wireframe_custom(
+        self,
+        ax: Axes | None = None,
+        coordinate_func: Callable[[float, float], tuple[float, float]] | None = None,
+        *,
+        transform: matplotlib.transforms.Transform | None = None,
+        additional_array_func: (
+            Callable[[Iterable, Iterable], tuple[np.ndarray, np.ndarray]] | None
+        ) = None,
+        **wireframe_kwargs: Unpack[WireframeKwargs],
+    ) -> Axes:
+        """
+        Plot a custom wireframe representation of the observation, using a user-defined
+        coordinate system.
+
+        This can be used to create a custom wireframe plot variant, similar to the
+        :func:`plot_wireframe_radec`, :func:`plot_wireframe_km`,
+        :func:`plot_wireframe_angular` and :func:`BodyXY.plot_wireframe_xy` methods. All
+        wireframe variants use the same plotting code internally, and this method allows
+        the internal wireframe plotting code to be accessed directly, with custom
+        arguments. Most wireframe uses are covered by the built-in wireframe plotting
+        methods but this method can be useful when plotting with custom projections or
+        complex coordinate systems.
+
+        .. hint::
+
+            If you just want to change the units of a wireframe plot, this can be done
+            with the `scale_factor` argument of the built-in wireframe plotting methods.
+            For example, `body.plot_wireframe_angular(scale_factor=1/60)` will plot the
+            wireframe with units of arcminutes (rather than the default arcseconds).
+
+        The `coordinate_func` and `transform` arguments are used to convert data in
+        RA/Dec coordinates into the desired coordinate system and apply any additional
+        Matplotlib transforms desired to the plotted data. Both of these arguments are
+        optional, so generally you will only need to specify a value for
+        `coordinate_func`.
+
+        For example, this approximately replicates the :func:`plot_wireframe_km` method,
+        by using :func:`radec2km` to convert RA/Dec coordinates to km coordinates: ::
+
+            ax = body.plot_wireframe_custom(coordinate_func=body.radec2km)
+            ax.set_aspect(1)
+            ax.set_xlabel('Projected distance (km)')
+            ax.set_ylabel('Projected distance (km)')
+
+        Or to plot a wireframe in custom 'angular' coordinates that are reflected in the
+        y direction, you could use: ::
+
+            def coordinate_func(ra, dec):
+                x, y = body.radec2angular(ra, dec)
+                return x, -y
+
+            ax = body.plot_wireframe_custom(coordinate_func=coordinate_func)
+            ax.set_aspect(1)
+
+        The `transform` argument is mainly useful if you wish to create an interactive
+        wireframe plot, where the plotted data can be changed after plotting (like in
+        the PlanetMapper GUI). If both `coordinate_func` and `transform` are provided,
+        then the `transform` is applied to the plotted data after transforming with
+        `coordinate_func`. The plotting functionality when both `coordinate_func` and
+        `transform` are provided can therefore be simplified as: ::
+
+            x, y = coordinate_func(ra, dec)
+            ax.scatter(x, y, transform=transform)
+
+        The `additional_array_func` argument can be used to specify a function to apply
+        to arrays before plotting any linear features (e.g. the limb, gridlines, rings).
+        For example, this is used internally in :func:`plot_wireframe_radec` to add NaNs
+        into arrays of data whenever the coordinates wrap from one side of the axis to
+        the other (to prevent lines being drawn across the entire axis). If specified,
+        this function is applied after first converting the data with `coordinate_func`
+        and before applying any `transform` argument, and is only applied to data
+        plotted with Matplotlib's `plot` function. The plotting functionality when
+        `coordinate_func`, `transform` and `additional_array_func` are provided can
+        therefore be simplified as: ::
+
+            # plotting arrays of ra and dec coordinates
+            xs, ys = zip(*(coordinate_func(ra, dec) for ra, dec in zip(ras, decs)))
+            xs, ys = additional_array_func(xs, ys)
+            ax.plot(xs, ys, transform=transform)
+
+            # plotting individual ra and dec coordinates
+            x, y = coordinate_func(ra, dec)
+            ax.scatter(x, y, transform=transform)
+
+        .. note::
+
+            This method does not set the aspect ratio of the plot, so you will usually
+            need to do this yourself to ensure the plot is not distorted. For example,
+            to set the aspect ratio to 1, you can use `ax.set_aspect(1)`.
+
+        Args:
+            ax: Matplotlib axis to use for plotting. If `ax` is None (the default), uses
+                `plt.gca()` to get the currently active axis.
+            coordinate_func: Function to convert RA/Dec coordinates to the desired
+                coordinate system. Takes two arguments (RA, Dec) and returns two values
+                (x, y). If this is not provided, then the default no-op function
+                `coordinate_func=lambda ra, dec: (ra, dec)` is used.
+            transform: Matplotlib transform to apply to the plotted data, after
+                transforming with `coordinate_func`. If this is not provided, then no
+                additional transform is applied.
+            additional_array_func: Optional function to apply to iterable of converted
+                (x, y) coordinates before plotting any linear features (e.g. the limb,
+                gridlines, rings). This should take two iterables of x and y coordinates
+                and return two arrays x and y coordinates to plot. The lengths of the
+                input coordinates do not have to be the same as the lengths of the
+                output coordinates, so `additional_array_func` can be used to add or
+                remove points from the plotted data as needed. However, the length of
+                the output x array should be the same as the length of the output y
+                array. If this is not provided, then no additional function is applied.
+            **wireframe_kwargs: See :func:`plot_wireframe_radec` for details of
+                additional arguments.
+        """
+        if coordinate_func is None:
+            coordinate_func = lambda ra, dec: (ra, dec)
+        return self._plot_wireframe(
+            coordinate_func=coordinate_func,
+            scale_factor=None,
+            transform=transform,
+            aspect_adjustable=None,
+            ax=ax,
+            additional_array_func=additional_array_func,
+            **wireframe_kwargs,
+        )
```

### Comparing `planetmapper-1.9.0/planetmapper/body_xy.py` & `planetmapper-1.9.1/planetmapper/body_xy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1172,38 +1172,43 @@
         return (-0.5 < x < self._nx - 0.5) and (-0.5 < y < self._ny - 0.5)
 
     # Plotting
     def plot_wireframe_xy(
         self,
         ax: Axes | None = None,
         *,
-        add_axis_labels: bool = True,
+        scale_factor: float | None = None,
+        add_axis_labels: bool | None = None,
         aspect_adjustable: Literal['box', 'datalim'] | None = 'box',
         show: bool = False,
         **wireframe_kwargs: Unpack[WireframeKwargs],
     ) -> Axes:
         """
         Plot basic wireframe representation of the observation using image pixel
         coordinates. See :func:`Body.plot_wireframe_radec` for details of accepted
         arguments.
 
-        Returns:r
+        Returns:
             The axis containing the plotted wireframe.
         """
+        if add_axis_labels is None:
+            add_axis_labels = scale_factor is None
+
         # Use combo of corodinate_func and matplotlib transform so that the plot can be
         # updated with new disc parameters without having to replot the entire thing
         ax = self._plot_wireframe(
             coordinate_func=self.radec2angular,
+            scale_factor=scale_factor,
             transform=self._get_matplotlib_angular_fixed2xy_transform(),
             aspect_adjustable=aspect_adjustable,
             ax=ax,
             **wireframe_kwargs,
         )
 
-        if self._test_if_img_size_valid():
+        if self._test_if_img_size_valid() and scale_factor is None:
             ax.set_xlim(-0.5, self._nx - 0.5)
             ax.set_ylim(-0.5, self._ny - 0.5)
         if add_axis_labels:
             ax.set_xlabel('x (pixels)')
             ax.set_ylabel('y (pixels)')
 
         if show:
```

### Comparing `planetmapper-1.9.0/planetmapper/cli.py` & `planetmapper-1.9.1/planetmapper/cli.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/planetmapper/data/rings.json` & `planetmapper-1.9.1/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/planetmapper/data_loader.py` & `planetmapper-1.9.1/planetmapper/data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/planetmapper/gui.py` & `planetmapper-1.9.1/planetmapper/gui.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/planetmapper/kernel_downloader.py` & `planetmapper-1.9.1/planetmapper/kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/planetmapper/observation.py` & `planetmapper-1.9.1/planetmapper/observation.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/planetmapper/progress.py` & `planetmapper-1.9.1/planetmapper/progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/planetmapper/utils.py` & `planetmapper-1.9.1/planetmapper/utils.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.9.1/planetmapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.9.0
+Version: 1.9.1
 Summary: PlanetMapper: A Python package for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
```

### Comparing `planetmapper-1.9.0/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.9.1/planetmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/pyproject.toml` & `planetmapper-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/setup.py` & `planetmapper-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/tests/test_base.py` & `planetmapper-1.9.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/tests/test_basic_body.py` & `planetmapper-1.9.1/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/tests/test_body.py` & `planetmapper-1.9.1/tests/test_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     SpiceKERNELVARNOTFOUND,
     SpiceSPKINSUFFDATA,
 )
 
 import planetmapper
 import planetmapper.base
 import planetmapper.progress
+import planetmapper.utils
 from planetmapper import Body
 
 
 class TestBody(common_testing.BaseTestCase):
     def setUp(self):
         planetmapper.set_kernel_path(common_testing.KERNEL_PATH)
         self.body = Body('Jupiter', observer='HST', utc='2005-01-01T00:00:00')
@@ -1725,14 +1726,145 @@
         fig, ax = plt.subplots()
         jupiter_from_amalthea.plot_wireframe_radec(ax, use_shifted_meridian=True)
         xlim = ax.get_xlim()
         self.assertTrue(60 > xlim[0] > 10)
         self.assertTrue(-10 > xlim[1] > -60)
         plt.close(fig)
 
+        # Test scalings
+        self._test_wireframe_scaling(
+            self.body.plot_wireframe_radec,
+            'Right Ascension',
+            'Declination',
+            [
+                (
+                    None,
+                    (196.3774505836621, 196.36652066566225),
+                    (-5.570996600931527, -5.560591073745357),
+                ),
+                (
+                    50,
+                    (9818.872529183103, 9818.326033283114),
+                    (-278.54983004657635, -278.0295536872678),
+                ),
+                (
+                    123456.786,
+                    (24244128.89193274, 24242779.519385245),
+                    (-687777.3351679309, -686492.7022248907),
+                ),
+                (
+                    1e-06,
+                    (0.00019637745058366206, 0.00019636652066566226),
+                    (-5.570996600931527e-06, -5.560591073745357e-06),
+                ),
+            ],
+        )
+        self._test_wireframe_scaling(
+            self.body.plot_wireframe_km,
+            'Projected distance (km)',
+            'Projected distance (km)',
+            [
+                (
+                    None,
+                    (-78640.99608058519, 78641.15962987275),
+                    (-73550.89564237543, 73551.12774884349),
+                ),
+                (
+                    50,
+                    (-3932049.804029259, 3932057.981493638),
+                    (-3677544.782118771, 3677556.387442174),
+                ),
+                (
+                    123456.786,
+                    (-9708764623.947643, 9708784815.21704),
+                    (-9080357183.429073, 9080385838.54763),
+                ),
+                (
+                    1e-06,
+                    (-0.07864099608058517, 0.07864115962987274),
+                    (-0.07355089564237542, 0.07355112774884348),
+                ),
+            ],
+        )
+
+        self._test_wireframe_scaling(
+            self.body.plot_wireframe_angular,
+            'Angular distance (arcsec)',
+            'Angular distance (arcsec)',
+            [
+                (
+                    None,
+                    (-19.581092792776644, 19.58110648969864),
+                    (-18.729913838924922, 18.729984031278835),
+                ),
+                (
+                    50,
+                    (-979.0546396388322, 979.055324484932),
+                    (-936.4956919462461, 936.4992015639417),
+                ),
+                (
+                    123456.786,
+                    (-2417418.7825639686, 2417420.473541936),
+                    (-2312334.9646105925, 2312343.6303330082),
+                ),
+                (
+                    1e-06,
+                    (-1.9581092792776644e-05, 1.9581106489698642e-05),
+                    (-1.872991383892492e-05, 1.8729984031278834e-05),
+                ),
+            ],
+        )
+
+        with self.subTest('radec dms ticks'):
+            fig, ax = plt.subplots()
+            self.body.plot_wireframe_radec(ax)
+            for axis in (ax.xaxis, ax.yaxis):
+                self.assertIsInstance(
+                    axis.get_major_formatter(), planetmapper.utils.DMSFormatter
+                )
+                self.assertIsInstance(
+                    axis.get_major_locator(), planetmapper.utils.DMSLocator
+                )
+            plt.close(fig)
+
+            fig, ax = plt.subplots()
+            self.body.plot_wireframe_radec(ax, scale_factor=10)
+            for axis in (ax.xaxis, ax.yaxis):
+                self.assertNotIsInstance(
+                    axis.get_major_formatter(), planetmapper.utils.DMSFormatter
+                )
+                self.assertNotIsInstance(
+                    axis.get_major_locator(), planetmapper.utils.DMSLocator
+                )
+            plt.close(fig)
+
+            for dms_ticks in (True, False):
+                for scale_factor in (None, 10):
+                    with self.subTest(dms_ticks=dms_ticks, scale_factor=scale_factor):
+                        fig, ax = plt.subplots()
+                        self.body.plot_wireframe_radec(
+                            ax, dms_ticks=dms_ticks, scale_factor=scale_factor
+                        )
+                        for axis in (ax.xaxis, ax.yaxis):
+                            self.assertEqual(
+                                isinstance(
+                                    axis.get_major_formatter(),
+                                    planetmapper.utils.DMSFormatter,
+                                ),
+                                dms_ticks,
+                            )
+                            self.assertEqual(
+                                isinstance(
+                                    axis.get_major_locator(),
+                                    planetmapper.utils.DMSLocator,
+                                ),
+                                dms_ticks,
+                            )
+                        plt.close(fig)
+
     def test_get_local_affine_transform_matrix(self):
         tests: list[
             tuple[
                 Callable[[float, float], tuple[float, float]],
                 tuple[float, float],
                 np.ndarray,
             ]
@@ -1887,7 +2019,54 @@
 
                 self.body.matplotlib_km2radec_transform(ax)
                 t1 = self.body.matplotlib_km2radec_transform(ax)
                 t2 = self.body.matplotlib_km2radec_transform(ax)
                 self.assertEqual(t1, t2)
 
         plt.close(fig)
+
+    def test_plot_wireframe_custom(self):
+        arguments_and_limits: list[
+            tuple[
+                dict,
+                tuple[float, float],
+                tuple[float, float],
+            ]
+        ] = [
+            (
+                {},
+                (196.36652066566225, 196.3774505836621),
+                (-5.570996600931527, -5.560591073745357),
+            ),
+            (
+                dict(coordinate_func=None, transform=None),
+                (196.36652066566225, 196.3774505836621),
+                (-5.570996600931527, -5.560591073745357),
+            ),
+            (
+                dict(coordinate_func=self.body.radec2km),
+                (-78640.99608058519, 78641.15962987275),
+                (-73550.89564237543, 73551.12774884349),
+            ),
+            (
+                dict(transform=self.body.matplotlib_radec2km_transform()),
+                (-78666.01732656956, 78665.97486374379),
+                (-73527.70551617145, 73527.85605175495),
+            ),
+            (
+                dict(
+                    coordinate_func=self.body.radec2angular,
+                    transform=self.body.matplotlib_angular2radec_transform(),
+                ),
+                (196.36652066335904, 196.37745058135863),
+                (-5.570996601039565, -5.560591073731259),
+            ),
+        ]
+        atol = 1e-5
+        rtol = 1e-2
+        for kwargs, xlim, ylim in arguments_and_limits:
+            with self.subTest(kwargs):
+                fig, ax = plt.subplots()
+                self.body.plot_wireframe_custom(ax, **kwargs)
+                self.assertArraysClose(ax.get_xlim(), xlim, atol=atol, rtol=rtol)
+                self.assertArraysClose(ax.get_ylim(), ylim, atol=atol, rtol=rtol)
+                plt.close(fig)
```

### Comparing `planetmapper-1.9.0/tests/test_body_xy.py` & `planetmapper-1.9.1/tests/test_body_xy.py`

 * *Files 1% similar despite different names*

```diff
@@ -713,14 +713,48 @@
             lat_coords=np.linspace(0, 90, 3),
         )
         self.assertEqual(len(ax.get_lines()), 17)
         self.assertEqual(len(ax.get_images()), 0)
         self.assertEqual(len(ax.get_children()), 29)
         plt.close(fig)
 
+        self._test_wireframe_scaling(
+            self.body.plot_wireframe_xy,
+            'x (pixels)',
+            'y (pixels)',
+            [
+                (None, (-0.5, 14.5), (-0.5, 9.5)),
+                (
+                    1,
+                    (2.6023360665508823, 12.397667359351928),
+                    (0.3152347289140154, 9.684782827744533),
+                ),
+                (
+                    1.0,
+                    (2.6023360665508823, 12.397667359351928),
+                    (0.3152347289140154, 9.684782827744533),
+                ),
+                (
+                    50,
+                    (130.11680332754412, 619.8833679675964),
+                    (15.761736445700745, 484.2391413872267),
+                ),
+                (
+                    123456.786,
+                    (321276.04686825396, 1530576.166082696),
+                    (38917.86646730556, 1195652.1610213316),
+                ),
+                (
+                    1e-06,
+                    (2.6023360665508817e-06, 1.239766735935193e-05),
+                    (3.152347289140152e-07, 9.684782827744531e-06),
+                ),
+            ],
+        )
+
     def test_get_wireframe_overlay(self):
         img = self.body.get_wireframe_overlay_img(output_size=100)
         self.assertEqual(max(img.shape), 100)
         self.assertEqual(len(img.shape), 2)
 
         img = self.body.get_wireframe_overlay_map(output_size=100)
         self.assertEqual(max(img.shape), 100)
@@ -1553,15 +1587,14 @@
 
         self.body.imshow_map(np.ones((180, 360)))
         plt.close('all')
 
     def test_matplotlib_transforms(self):
         self.body.set_disc_params(2, 1, 3.5, 45.678)
         self.body.set_img_size(15, 10)
-        # XXX add angular
 
         # Test outputs
         self.assertArraysClose(
             self.body.matplotlib_radec2xy_transform().get_matrix(),
             array(
                 [
                     [-4.87436799e02, 5.01041734e02, 9.85096272e04],
```

### Comparing `planetmapper-1.9.0/tests/test_cli.py` & `planetmapper-1.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/tests/test_common.py` & `planetmapper-1.9.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/tests/test_data_loader.py` & `planetmapper-1.9.1/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/tests/test_init.py` & `planetmapper-1.9.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/tests/test_kernel_downloader.py` & `planetmapper-1.9.1/tests/test_kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/tests/test_observation.py` & `planetmapper-1.9.1/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/tests/test_progress.py` & `planetmapper-1.9.1/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.9.0/tests/test_utils.py` & `planetmapper-1.9.1/tests/test_utils.py`

 * *Files identical despite different names*

