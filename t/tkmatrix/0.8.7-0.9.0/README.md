# Comparing `tmp/tkmatrix-0.8.7.tar.gz` & `tmp/tkmatrix-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkmatrix-0.8.7.tar", last modified: Mon Apr 22 19:58:07 2024, max compression
+gzip compressed data, was "tkmatrix-0.9.0.tar", last modified: Thu May  9 07:17:26 2024, max compression
```

## Comparing `tkmatrix-0.8.7.tar` & `tkmatrix-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:58:07.581429 tkmatrix-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-22 19:58:07.581429 tkmatrix-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:58:07.581429 tkmatrix-0.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:58:07.581429 tkmatrix-0.8.7/tkmatrix/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:58:07.581429 tkmatrix-0.8.7/tkmatrix/custom_algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/custom_algorithms/BlsCustomSearchAlgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/custom_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/custom_algorithms/custom_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/inject_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/inject_rv_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/programmatic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/properties.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/rv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:58:07.581429 tkmatrix-0.8.7/tkmatrix/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/tests/test_tkmatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    46813 2024-04-22 19:57:54.000000 tkmatrix-0.8.7/tkmatrix/tkmatrix_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:58:07.581429 tkmatrix-0.8.7/tkmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-22 19:58:07.000000 tkmatrix-0.8.7/tkmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-22 19:58:07.000000 tkmatrix-0.8.7/tkmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:58:07.000000 tkmatrix-0.8.7/tkmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-22 19:58:07.000000 tkmatrix-0.8.7/tkmatrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 19:58:07.000000 tkmatrix-0.8.7/tkmatrix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:17:26.675708 tkmatrix-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-09 07:17:26.675708 tkmatrix-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 07:17:26.675708 tkmatrix-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:17:26.671708 tkmatrix-0.9.0/tkmatrix/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:17:26.675708 tkmatrix-0.9.0/tkmatrix/custom_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/custom_algorithms/BlsCustomSearchAlgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/custom_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/custom_algorithms/custom_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/inject_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/inject_rv_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/programmatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/rv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:17:26.675708 tkmatrix-0.9.0/tkmatrix/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/tests/test_tkmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44005 2024-05-09 07:17:15.000000 tkmatrix-0.9.0/tkmatrix/tkmatrix_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:17:26.675708 tkmatrix-0.9.0/tkmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-09 07:17:26.000000 tkmatrix-0.9.0/tkmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-09 07:17:26.000000 tkmatrix-0.9.0/tkmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:17:26.000000 tkmatrix-0.9.0/tkmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-09 07:17:26.000000 tkmatrix-0.9.0/tkmatrix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 07:17:26.000000 tkmatrix-0.9.0/tkmatrix.egg-info/top_level.txt
```

### Comparing `tkmatrix-0.8.7/LICENSE` & `tkmatrix-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.8.7/PKG-INFO` & `tkmatrix-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.8.7
+Version: 0.9.0
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
```

### Comparing `tkmatrix-0.8.7/README.md` & `tkmatrix-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.8.7/setup.py` & `tkmatrix-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = "0.8.7"
+version = "0.9.0"
 setuptools.setup(
     name="tkmatrix",
     version=version,
     author="M. Dévora-Pajares & F.J. Pozuelos",
     author_email="mdevorapajares@protonmail.com",
     description="ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets",
     long_description=long_description,
@@ -21,15 +21,15 @@
     ],
     python_requires='>=3.10',
     install_requires=['argparse==1.4.0',
                         'beautifulsoup4==4.9.3',
                         'configparser==5.0.1',
                         "corner==2.1.0",
                         "ellc==1.8.5",
-                        "lcbuilder==0.16.2",
+                        "lcbuilder==0.18.0",
                         "mock==4.0.3",
                         'pyparsing==2.4.7', # Matplotlib dependency
                         "seaborn==0.11.1",
                         'setuptools>=41.0.0',
                         "sklearn==0.0"
     ]
 )
```

### Comparing `tkmatrix-0.8.7/tkmatrix/__main__.py` & `tkmatrix-0.9.0/tkmatrix/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,16 +140,15 @@
                          period_grid=rv['PERIOD_GRID'] if 'PERIOD_GRID' in rv else None,
                          mass_grid=rv['MASS_GRID'] if 'MASS_GRID' in rv else None,
                          period_grid_geom=rv["PERIOD_GRID_GEOM"],
                          mass_grid_geom=rv["MASS_GRID_GEOM"])
             ir.recovery_rv(inject_dir, rv['INITIAL_MASK'] if 'INITIAL_MASK' in rv else None,
                            rv['SNR_THRESHOLD'], rv['RUN_LIMIT'],
                            rv['MAX_PERIOD_SEARCH'], rv['OVERSAMPLING'] if 'OVERSAMPLING' in rv else 1)
-            ir.plot_results(target, inject_dir, period_grid, mass_grid, period_grid_geom=rv["PERIOD_GRID_GEOM"],
-                            radius_grid_geom=rv["MASS_GRID_GEOM"], is_rv=True)
+            ir.plot_results(target, inject_dir, is_rv=True)
     inject_dir, period_grid, radius_grid = ir.inject(matrix_user_properties["PHASES"],
                            matrix_user_properties["MIN_PERIOD"], matrix_user_properties["MAX_PERIOD"],
                            matrix_user_properties["STEPS_PERIOD"],
                            matrix_user_properties["MIN_RADIUS"], matrix_user_properties["MAX_RADIUS"],
                            matrix_user_properties["STEPS_RADIUS"],
                            period_grid=matrix_user_properties['PERIOD_GRID'],
                            radius_grid=matrix_user_properties['RADIUS_GRID'],
@@ -159,10 +158,9 @@
     ir.recovery(inject_dir, matrix_user_properties["SNR_THRESHOLD"],
                 matrix_user_properties["DETREND_METHOD"],
                 matrix_user_properties["DETREND_WS"], matrix_user_properties["FIT_METHOD"],
                 matrix_user_properties["RUN_LIMIT"],
                 custom_search, matrix_user_properties["MAX_PERIOD_SEARCH"], matrix_user_properties["OVERSAMPLING"],
                 matrix_user_properties["SIGNAL_SELECTION_MODE"],
                 use_search_cache=matrix_user_properties["USE_SEARCH_CACHE"])
-    ir.plot_results(target, inject_dir, period_grid, radius_grid, period_grid_geom=matrix_user_properties["PERIOD_GRID_GEOM"],
-                    radius_grid_geom=matrix_user_properties["RADIUS_GRID_GEOM"])
+    ir.plot_results(target, inject_dir)
     print("Execution time: " + str(datetime.datetime.now() - start_time))
```

### Comparing `tkmatrix-0.8.7/tkmatrix/custom_algorithms/BlsCustomSearchAlgorithm.py` & `tkmatrix-0.9.0/tkmatrix/custom_algorithms/BlsCustomSearchAlgorithm.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.8.7/tkmatrix/custom_algorithms/custom_search.py` & `tkmatrix-0.9.0/tkmatrix/custom_algorithms/custom_search.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.8.7/tkmatrix/inject_model.py` & `tkmatrix-0.9.0/tkmatrix/inject_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.8.7/tkmatrix/inject_rv_model.py` & `tkmatrix-0.9.0/tkmatrix/inject_rv_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.8.7/tkmatrix/programmatic.py` & `tkmatrix-0.9.0/tkmatrix/programmatic.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.8.7/tkmatrix/properties.yaml` & `tkmatrix-0.9.0/tkmatrix/properties.yaml`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.8.7/tkmatrix/rv.py` & `tkmatrix-0.9.0/tkmatrix/rv.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.8.7/tkmatrix/tests/test_tkmatrix.py` & `tkmatrix-0.9.0/tkmatrix/tests/test_tkmatrix.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.8.7/tkmatrix/tkmatrix_class.py` & `tkmatrix-0.9.0/tkmatrix/tkmatrix_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -493,65 +493,39 @@
                 os.remove(inject_dir + file)
         if not self.preserve:
             for file in os.listdir(inject_dir):
                 if file.endswith(".csv") and (file.startswith("P") or file.startswith("RV_P")):
                     os.remove(inject_dir + file)
 
     @staticmethod
-    def plot_results(object_id, inject_dir, period_grid=None, radius_grid=None, binning=1, xticks=None, yticks=None,
-                     period_grid_geom="lin", radius_grid_geom="lin", is_rv=False, planets_df=None):
+    def plot_results(object_id, inject_dir, binning=1, xticks=None, yticks=None, is_rv=False, planets_df=None):
         """
         Generates a heat map with the found/not found results for the period/radius grids
 
         :param object_id: the id of the target star
         :param inject_dir: the inject directory where the result files are stored
         :param period_grid: the periods grid array
         :param radius_grid: the radius or mass grid array
         :param binning: the binning to be applied to the grids
         :param xticks: the fixed ticks to be used for the period grid
         :param yticks: the fixed ticks to be used for the radius grid
-        :param period_grid_geom: [lin|log]
-        :param radius_grid_geom: [lin|log]
         :param is_rv: whether to load the rv results or the photometry ones
         :param planets_df: pandas dataframe with radius, period, name, radius_err_up, radius_err_bottom
         """
         filename = '/a_tls_report.csv' if not is_rv else '/a_rv_report.csv'
         column = 'radius' if not is_rv else 'mass'
         column_units = 'R' if not is_rv else 'M'
         df = pd.read_csv(inject_dir + filename, float_precision='round_trip', sep=',',
                          usecols=['period', column, 'found', 'sde'])
         min_period = df["period"].min()
         max_period = df["period"].max()
-        min_rad = df[column].min()
-        max_rad = df[column].max()
         phases = len(df[df["period"] == df["period"].min()][df[column] == df[column].min()])
         phases_str = "phase" if phases == 1 else "phases"
-        bin_nums = int(np.ceil(len(df["period"].unique()) / binning))
-        if period_grid is None:
-            if period_grid_geom == 'lin':
-                step_period = (max_period - min_period) / (len(df["period"].unique()) - 1)
-                step_period = step_period * binning
-                if step_period <= 0:
-                    step_period = 0.1
-                period_grid = np.linspace(min_period, max_period, bin_nums)\
-                    if max_period - min_period > 0 else np.full((1), min_period)
-            else:
-                period_grid = np.logspace(np.log10(min_period), np.log10(max_period), bin_nums)
-        if radius_grid is None:
-            bin_nums = int(np.ceil(len(df[column].unique()) / binning))
-            if radius_grid_geom == 'lin':
-                step_radius = (max_rad - min_rad) / (len(df[column].unique()) - 1)
-                step_radius = step_radius * binning
-                if step_radius <= 0:
-                    step_radius = 0.1
-                radius_grid = np.round(np.linspace(min_rad, max_rad, bin_nums), 2)\
-                    if max_rad - min_rad > 0 else np.full((1), min_rad)
-            else:
-                radius_grid = np.round(np.logspace(np.log10(min_rad), np.log10(max_rad), 2), bin_nums)
-        f = len(period_grid) / len(radius_grid)
+        period_grid = df['period'].unique()
+        radius_grid = df[column].unique()
         bins = [period_grid, radius_grid]
         h1, x, y = np.histogram2d(df['period'][df['found'] == 1], df[column][df['found'] == 1], bins=bins)
         h2, x, y = np.histogram2d(df['period'][df['found'] == 0], df[column][df['found'] == 0], bins=bins)
         normed_hist = (100. * h1 / (h1 + h2))
         fig, ax = plt.subplots(figsize=(2.7 * 5, 5))
         im = plt.imshow(normed_hist.T, origin='lower', extent=(x[0], x[-1], y[0], y[-1]), interpolation='none',
                         aspect='auto', cmap='viridis', vmin=0, vmax=100, rasterized=True)
@@ -569,67 +543,43 @@
             plt.locator_params(axis="x", nbins=plot_bins)
             ax.xaxis.set_major_formatter(FormatStrFormatter('%.' + str(period_ticks_decimals) + 'f'))
         if yticks is not None:
             plt.xticks(yticks)
         ax.tick_params(axis='both', which='major', labelsize=14)
         if planets_df is not None:
             for index, row in planets_df.iterrows():
-                ax.errorbar([row['period']], [row['radius']],
-                            yerr=[np.full(1, row['radius_err_bottom']), np.full(1, row['radius_err_up'])],
+                ax.errorbar([row['period']], [row[column]],
+                            yerr=[np.full(1, row[column + '_err_bottom']), np.full(1, row[column + '_err_up'])],
                             fmt='o', color='firebrick', markersize=12)
         plt.savefig(inject_dir + '/inj-rec' + ('-rv' if is_rv else '') + '.png', bbox_inches='tight', dpi=200)
         plt.close()
 
     @staticmethod
-    def plot_diff(object_id, inject_dir1, inject_dir2, output_dir, binning=1, xticks=None, yticks=None,
-                  period_grid_geom="lin", radius_grid_geom="lin"):
+    def plot_diff(object_id, inject_dir1, inject_dir2, output_dir, binning=1, xticks=None, yticks=None):
         """
         Plots the difference between two results directories.
 
         :param object_id: the target star id
         :param inject_dir1: the results dir number 1
         :param inject_dir2: the results dir number 2
         :param output_dir: the output directory for the plot
         :param binning: the binning to be applied to both axes
         :param xticks: the fixed ticks for the period bar
         :param yticks: the fixed ticks for the radius bar
-        :param period_grid_geom: [lin|log]
-        :param radius_grid_geom: [ling|log]
         """
         df1 = pd.read_csv(inject_dir1 + '/a_tls_report.csv', float_precision='round_trip', sep=',',
                          usecols=['period', 'radius', 'found', 'sde'])
         df2 = pd.read_csv(inject_dir2 + '/a_tls_report.csv', float_precision='round_trip', sep=',',
                          usecols=['period', 'radius', 'found', 'sde'])
         min_period = df1["period"].min()
         max_period = df1["period"].max()
-        min_rad = df1["radius"].min()
-        max_rad = df1["radius"].max()
         phases = len(df1[df1["period"] == df1["period"].min()][df1["radius"] == df1["radius"].min()])
         phases_str = "phase" if phases == 1 else "phases"
-        bin_nums = int(np.ceil(len(df1["period"].unique()) / binning))
-        if period_grid_geom == 'lin':
-            step_period = (max_period - min_period) / (len(df1["period"].unique()) - 1)
-            step_period = step_period * binning
-            if step_period <= 0:
-                step_period = 0.1
-            period_grid = np.linspace(min_period, max_period, bin_nums)\
-                if max_period - min_period > 0 else np.full((1), min_period)
-        else:
-            period_grid = np.logspace(np.log10(min_period), np.log10(max_period), bin_nums)
-        bin_nums = int(np.ceil(len(df1["radius"].unique()) / binning))
-        if radius_grid_geom == 'lin':
-            step_radius = (max_rad - min_rad) / (len(df1["radius"].unique()) - 1)
-            step_radius = step_radius * binning
-            if step_radius <= 0:
-                step_radius = 0.1
-            radius_grid = np.round(np.linspace(min_rad, max_rad, bin_nums), 2)\
-                if max_rad - min_rad > 0 else np.full((1), min_rad)
-        else:
-            radius_grid = np.round(np.logspace(np.log10(min_rad), np.log10(max_rad), 2), bin_nums)
-        f = len(period_grid) / len(radius_grid)
+        period_grid = df1['period'].unique()
+        radius_grid = df1['radius'].unique()
         bins = [period_grid, radius_grid]
         h11, x1, y1 = np.histogram2d(df1['period'][df1['found'] == 1], df1['radius'][df1['found'] == 1], bins=bins)
         h12, x1, y1 = np.histogram2d(df1['period'][df1['found'] == 0], df1['radius'][df1['found'] == 0], bins=bins)
         h21, x2, y2 = np.histogram2d(df2['period'][df2['found'] == 1], df2['radius'][df2['found'] == 1], bins=bins)
         h22, x2, y2 = np.histogram2d(df2['period'][df2['found'] == 0], df2['radius'][df2['found'] == 0], bins=bins)
         h1 = h11 - h12
         h2 = h21 - h22
```

### Comparing `tkmatrix-0.8.7/tkmatrix.egg-info/PKG-INFO` & `tkmatrix-0.9.0/tkmatrix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.8.7
+Version: 0.9.0
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
```

### Comparing `tkmatrix-0.8.7/tkmatrix.egg-info/SOURCES.txt` & `tkmatrix-0.9.0/tkmatrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

