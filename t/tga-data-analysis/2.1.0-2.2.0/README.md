# Comparing `tmp/tga_data_analysis-2.1.0.tar.gz` & `tmp/tga_data_analysis-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tga_data_analysis-2.1.0.tar", last modified: Thu May  2 21:34:02 2024, max compression
+gzip compressed data, was "tga_data_analysis-2.2.0.tar", last modified: Thu May  9 18:09:53 2024, max compression
```

## Comparing `tga_data_analysis-2.1.0.tar` & `tga_data_analysis-2.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:34:02.713221 tga_data_analysis-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-02 21:34:02.713221 tga_data_analysis-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 21:34:02.713221 tga_data_analysis-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:34:02.709221 tga_data_analysis-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:34:02.713221 tga_data_analysis-2.1.0/src/tga_data_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/src/tga_data_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/src/tga_data_analysis/kas_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/src/tga_data_analysis/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)    68222 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/src/tga_data_analysis/tga.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:34:02.713221 tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-02 21:34:02.000000 tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-02 21:34:02.000000 tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:34:02.000000 tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-02 21:34:02.000000 tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 21:34:02.000000 tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:34:02.713221 tga_data_analysis-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/tests/test_deconvolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/tests/test_kas_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/tests/test_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/tests/test_oxidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/tests/test_proximate.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/tests/test_soliddist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:09:53.615387 tga_data_analysis-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-05-09 18:09:53.615387 tga_data_analysis-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7510 2024-05-09 18:09:44.000000 tga_data_analysis-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-09 18:09:44.000000 tga_data_analysis-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:09:53.615387 tga_data_analysis-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:09:53.611387 tga_data_analysis-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:09:53.611387 tga_data_analysis-2.2.0/src/tga_data_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:09:44.000000 tga_data_analysis-2.2.0/src/tga_data_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-09 18:09:44.000000 tga_data_analysis-2.2.0/src/tga_data_analysis/kas_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-09 18:09:44.000000 tga_data_analysis-2.2.0/src/tga_data_analysis/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65836 2024-05-09 18:09:44.000000 tga_data_analysis-2.2.0/src/tga_data_analysis/tga.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:09:53.615387 tga_data_analysis-2.2.0/src/tga_data_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-05-09 18:09:53.000000 tga_data_analysis-2.2.0/src/tga_data_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 18:09:53.000000 tga_data_analysis-2.2.0/src/tga_data_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:09:53.000000 tga_data_analysis-2.2.0/src/tga_data_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-09 18:09:53.000000 tga_data_analysis-2.2.0/src/tga_data_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 18:09:53.000000 tga_data_analysis-2.2.0/src/tga_data_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:09:53.615387 tga_data_analysis-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-09 18:09:44.000000 tga_data_analysis-2.2.0/tests/test_deconvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-09 18:09:44.000000 tga_data_analysis-2.2.0/tests/test_kas_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-09 18:09:44.000000 tga_data_analysis-2.2.0/tests/test_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-09 18:09:44.000000 tga_data_analysis-2.2.0/tests/test_oxidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-09 18:09:44.000000 tga_data_analysis-2.2.0/tests/test_proximate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-09 18:09:44.000000 tga_data_analysis-2.2.0/tests/test_soliddist.py
```

### Comparing `tga_data_analysis-2.1.0/PKG-INFO` & `tga_data_analysis-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tga_data_analysis
-Version: 2.1.0
+Version: 2.2.0
 Summary: Tool for automatic analysis of multiple TGA results
 Author: Matteo Pecchi
 License: MIT
 Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
 Project-URL: Documentation, https://tga-data-analysis.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -111,16 +111,15 @@
 * ``temp_initial_celsius``: The initial temperature where every ``File`` is going to start to ensure uniformity.
 
 * ``temp_lim_dtg_celsius``: The temperature limits for DTG analysis, in Celsius. It should exclude moisture and fixed 
 carbon segments.
 
 * ``temp_unit``: The unit of temperature the project will convert everything to, not the unit in the ``Files``. 
 
-* ``resolution_sec_deg_dtg``: The resolution in seconds per degree for the common temperature vector used in the DTG 
-analysis.
+* ``dtg_basis`` and ``resolution_sec_deg_dtg``: these parameters are no longer available and raise exceptions if specified. The dtg curve is now only computed as dTG/dtime (temperature is used for plotting), but replicates are not interpolated anymore so the resolution reflects the data resolution from the machine.
 
 * ``dtg_window_filter``: The window size for the Savitzky-Golay filter used to smooth the DTG curve.
 
 * ``temp_i_temp_b_threshold``: The fractional threshold for the detection of Ti (t_ignition) and Tb (burnout) calculation in DTG analysis.
 
 **Example**
```

### Comparing `tga_data_analysis-2.1.0/README.md` & `tga_data_analysis-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,15 @@
 * ``temp_initial_celsius``: The initial temperature where every ``File`` is going to start to ensure uniformity.
 
 * ``temp_lim_dtg_celsius``: The temperature limits for DTG analysis, in Celsius. It should exclude moisture and fixed 
 carbon segments.
 
 * ``temp_unit``: The unit of temperature the project will convert everything to, not the unit in the ``Files``. 
 
-* ``resolution_sec_deg_dtg``: The resolution in seconds per degree for the common temperature vector used in the DTG 
-analysis.
+* ``dtg_basis`` and ``resolution_sec_deg_dtg``: these parameters are no longer available and raise exceptions if specified. The dtg curve is now only computed as dTG/dtime (temperature is used for plotting), but replicates are not interpolated anymore so the resolution reflects the data resolution from the machine.
 
 * ``dtg_window_filter``: The window size for the Savitzky-Golay filter used to smooth the DTG curve.
 
 * ``temp_i_temp_b_threshold``: The fractional threshold for the detection of Ti (t_ignition) and Tb (burnout) calculation in DTG analysis.
 
 **Example**
```

### Comparing `tga_data_analysis-2.1.0/pyproject.toml` & `tga_data_analysis-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tga_data_analysis"
-version = "2.1.0"
+version = "2.2.0"
 authors = [
     { name = "Matteo Pecchi"}
 ]
 description = "Tool for automatic analysis of multiple TGA results"
 readme = "README.md"
 license = { text = "MIT" }
 classifiers = [
```

### Comparing `tga_data_analysis-2.1.0/src/tga_data_analysis/kas_kinetics.py` & `tga_data_analysis-2.2.0/src/tga_data_analysis/kas_kinetics.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,17 @@
         The results are stored within the object for later access and visualization.
         """
 
         r_gas_constant = 8.314462618  # Universal gas constant in J/(mol*K)
         c_to_k = 273.15
 
         for idx, sample in enumerate(self.samples):
-            temp = sample.temp_dtg + c_to_k if sample.temp_unit == "C" else sample.temp_dtg
+            if not sample.dtg_computed:
+                sample.dtg_analysis()
+            temp = sample.temp_dtg() + c_to_k if sample.temp_unit == "C" else sample.temp_dtg()
             alpha_mass = 1 - (sample.mp_db_dtg() - np.min(sample.mp_db_dtg())) / (
                 np.max(sample.mp_db_dtg()) - np.min(sample.mp_db_dtg())
             )
             for alpha_idx, alpha_val in enumerate(self.alpha):
                 conversion_index = np.argmax(alpha_mass > alpha_val)
                 self.x_matrix[alpha_idx, idx] = 1000 / temp[conversion_index]
                 self.y_matrix[alpha_idx, idx] = np.log(
```

### Comparing `tga_data_analysis-2.1.0/src/tga_data_analysis/measure.py` & `tga_data_analysis-2.2.0/src/tga_data_analysis/measure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.1.0/src/tga_data_analysis/tga.py` & `tga_data_analysis-2.2.0/src/tga_data_analysis/tga.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,35 +24,32 @@
         load_skiprows: int = 0,
         time_moist: float = 38.0,
         time_vm: float = 147.0,
         temp_initial_celsius: float = 40,
         temp_lim_dtg_celsius: tuple[float] | None = None,
         temp_unit: Literal["C", "K"] = "C",
         plot_font: Literal["Dejavu Sans", "Times New Roman"] = "Dejavu Sans",
-        dtg_basis: Literal["temperature", "time"] = "temperature",
         temp_i_temp_b_threshold: float = 0.01,  # % of the peak that is used for Ti and Tb
         soliddist_steps_min: list[int] | None = None,
         resolution_sec_deg_dtg: int = 5,
-        dtg_window_filter: int = 101,
+        dtg_window_filter: int | None = 51,
         plot_grid: bool = False,
         auto_save_reports: bool = True,
     ):
         """
         Initialize a new Project instance with various parameters for analysis.
 
         :param folder_path: The path to the folder containing the project data.
         :type folder_path: plib.Path
         :param name: The name of the project. Defaults to the last part of the folder path if None.
         :type name: str, optional
         :param temp_unit: The unit of temperature used in the project ('C':Celsius, 'K':Kelvin).
         :type temp_unit: Literal["C", "K"]
         :param plot_font: The font used in plots, either 'Dejavu Sans' or 'Times New Roman'.
         :type plot_font: Literal["Dejavu Sans", "Times New Roman"]
-        :param dtg_basis: The basis for DTG calculations, either 'temperature' or 'time'.
-        :type dtg_basis: Literal["temperature", "time"]
         :param temp_i_temp_b_threshold: The threshold for Ti and Tb calculation in DTG analysis.
         :type temp_i_temp_b_threshold: float
         :param soliddist_steps_min: Temperature steps (in minutes) at which the weight loss is calculated. If None, default steps are used.
         :type soliddist_steps_min: list[float], optional
         :param resolution_sec_deg_dtg: The resolution in seconds or degrees for DTG analysis.
         :type resolution_sec_deg_dtg: int
         :param dtg_window_filter: The window size for the Savitzky-Golay filter in DTG analysis.
@@ -79,15 +76,14 @@
         if name is None:
             self.name = self.folder_path.parts[-1]
         else:
             self.name = name
         self.temp_unit = temp_unit
         self.plot_font = plot_font
         self.plot_grid = plot_grid
-        self.dtg_basis = dtg_basis
         self.temp_i_temp_b_threshold = temp_i_temp_b_threshold
         self.resolution_sec_deg_dtg = resolution_sec_deg_dtg
         self.dtg_window_filter = dtg_window_filter
         self.load_skiprows = load_skiprows
         self.time_moist = time_moist
         self.time_vm = time_vm
         self.temp_initial_celsius = temp_initial_celsius
@@ -95,41 +91,31 @@
 
         if self.temp_unit == "C":
             self.temp_symbol = "°C"
         elif self.temp_unit == "K":
             self.temp_symbol = "K"
 
         self.tg_label = "TG [wt%]"
-        if self.dtg_basis == "temperature":
-            self.dtg_label = "DTG [wt%/" + self.temp_symbol + "]"
-        elif self.dtg_basis == "time":
-            self.dtg_label = "DTG [wt%/min]"
+        self.dtg_label = "DTG [wt%/min]"
 
         if temp_lim_dtg_celsius is None:
             self.temp_lim_dtg_celsius = (120, 880)
         else:
             self.temp_lim_dtg_celsius = temp_lim_dtg_celsius
-        if soliddist_steps_min is None:
-            self.soliddist_steps_min = [40, 70, 100, 130, 160, 190]
-        else:
-            self.soliddist_steps_min = soliddist_steps_min
+
         if self.temp_unit == "C":
             self.temp_lim_dtg = self.temp_lim_dtg_celsius
         elif self.temp_unit == "K":
             self.temp_lim_dtg = [t + 273.15 for t in self.temp_lim_dtg_celsius]
         else:
             raise ValueError(f"{self.temp_unit = } is not acceptable")
-
-        self.len_dtg_db: int = int(
-            (self.temp_lim_dtg[1] - self.temp_lim_dtg[0]) * self.resolution_sec_deg_dtg
-        )
-        self.temp_dtg: np.ndarray = np.linspace(
-            self.temp_lim_dtg[0], self.temp_lim_dtg[1], self.len_dtg_db
-        )
-
+        if soliddist_steps_min is None:
+            self.soliddist_steps_min = [40, 70, 100, 130, 160, 190]
+        else:
+            self.soliddist_steps_min = soliddist_steps_min
         if column_name_mapping is None:
             self.column_name_mapping = {
                 "Time": "t_min",
                 "Temperature": "T_C",
                 "Weight": "m_p",
                 "Weight.1": "m_mg",
                 "Heat Flow": "heatflow_mW",
@@ -473,16 +459,16 @@
         if samples is None:
             samples = list(self.samples.values())
 
         samplenames = [sample.name for sample in samples]
         if labels is None:
             labels = samplenames
         for sample in samples:
-            if not sample.proximate_computed:
-                sample.proximate_analysis()
+            if not sample.dtg_computed:
+                sample.dtg_analysis()
 
         out_path = plib.Path(self.out_path, "multisample_plots")
         out_path.mkdir(parents=True, exist_ok=True)
         default_kwargs = {
             "filename": filename + "_dtg",
             "out_path": out_path,
             "height": 3.2,
@@ -499,22 +485,22 @@
         myfig = MyFigure(
             rows=1,
             cols=1,
             **kwargs,
         )
         for i, sample in enumerate(samples):
             myfig.axs[0].plot(
-                sample.temp_dtg,
+                sample.temp_dtg.ave(),
                 sample.dtg_db.ave(),
                 color=colors[i],
                 linestyle=linestyles[i],
                 label=labels[i],
             )
             myfig.axs[0].fill_between(
-                sample.temp_dtg,
+                sample.temp_dtg.ave(),
                 sample.dtg_db.ave() - sample.dtg_db.std(),
                 sample.dtg_db.ave() + sample.dtg_db.std(),
                 color=colors[i],
                 alpha=0.3,
             )
         myfig.save_figure()
         return myfig
@@ -546,16 +532,16 @@
         if samples is None:
             samples = list(self.samples.values())
 
         samplenames = [sample.name for sample in samples]
         if labels is None:
             labels = samplenames
         for sample in samples:
-            if not sample.proximate_computed:
-                sample.proximate_analysis()
+            if not sample.dtg_computed:
+                sample.dtg_analysis()
 
         if cut_curves_at_last_step is True:
             index_end = np.argmax(samples[0].time.ave() > samples[0].soliddist_steps_min[-1])
         else:
             index_end = -1
 
         out_path = plib.Path(self.out_path, "multisample_plots")
@@ -710,18 +696,15 @@
         self.out_path = project.out_path
         self.temp_unit = project.temp_unit
         self.temp_symbol = project.temp_symbol
         self.tg_label = project.tg_label
         self.dtg_label = project.dtg_label
         self.plot_font = project.plot_font
         self.plot_grid = project.plot_grid
-        self.dtg_basis = project.dtg_basis
         self.temp_lim_dtg = project.temp_lim_dtg
-        self.len_dtg_db = project.len_dtg_db
-        self.temp_dtg = project.temp_dtg
         self.auto_save_reports = project.auto_save_reports
 
         self.resolution_sec_deg_dtg = project.resolution_sec_deg_dtg
         self.dtg_window_filter = project.dtg_window_filter
         self.temp_initial_celsius = project.temp_initial_celsius
         self.dtg_window_filter = project.dtg_window_filter
         if folder_path is None:
@@ -783,14 +766,15 @@
         self.mp_db: Measure = Measure(name="mp_db")
         self.ash_db: Measure = Measure(name="ash_db")
         self.fc_db: Measure = Measure(name="fc_db")
         self.vm_db: Measure = Measure(name="vm_db")
         self.mp_daf: Measure = Measure(name="mp_daf")
         self.fc_daf: Measure = Measure(name="fc_daf")
         self.vm_daf: Measure = Measure(name="vm_daf")
+        self.temp_dtg: Measure = Measure(name="temp_dtg" + self.temp_unit)
         self.time_dtg: Measure = Measure(name="time_dtg")
         self.mp_db_dtg: Measure = Measure(name="mp_db_dtg")
         self.dtg_db: Measure = Measure(name="dtg_db")
         self.ave_dev_tga_perc: float | None = None
         # oxidation
         self.temp_i_idx: Measure = Measure(name="temp_i_idx")
         self.temp_i: Measure = Measure(name="temp_i_" + self.temp_unit)
@@ -808,24 +792,24 @@
         self.loc_soliddist: Measure = Measure(name="loc_dist")
         # deconvolution
         self.dcv_best_fit: Measure = Measure(name="dcv_best_fit")
         self.dcv_r2: Measure = Measure(name="dcv_r2")
         self.dcv_peaks: list[Measure] = []
         # Flag to track if data is loaded
         self.proximate_computed = False
+        self.dtg_computed = False
         self.files_loaded = False
         self.oxidation_computed = False
         self.soliddist_computed = False
         self.deconv_computed = False
         # for reports
         self.reports: dict[str, pd.DataFrame] = {}
         self.report_types_computed: list[str] = []
 
         self.load_files()
-        self.proximate_analysis()
 
     def _broadcast_value_prop(self, prop: list | str | float | int | bool) -> list:
         """
         Broadcast a single value or a list of values to match the number of replicates.
 
         This method is used internally to ensure that properties like corrections have a value
         for each replicate, even if a single value is provided for all.
@@ -929,16 +913,20 @@
             file["m_p"] = file["m_p"] - np.min(file["m_p"])
             # shift the non-ash fraction up by enough to have ash_ar=correct_ash_fr
             file["m_p"] = file["m_p"] + np.max(file["m_p"]) * (
                 correct_ash_fr / (1 - correct_ash_fr)
             )
             # scale everything to 100 %
             file["m_p"] = file["m_p"] / np.max(file["m_p"]) * 100
+        if "T_C" not in file.columns and "T_K" in file.columns:
+            file["T_C"] = file["T_K"] - 273.15
+        else:
+            file["T_K"] = file["T_C"] + 273.15
         file = file[file["T_C"] >= self.temp_initial_celsius].copy()
-        file["T_K"] = file["T_C"] + 273.15
+
         return file
 
     def load_files(self):
         """
         Load all files associated with this sample, applying necessary corrections and adjustments.
 
         This method loads and processes each file, ensuring consistent data structure and applying
@@ -1007,76 +995,77 @@
 
                 self.vm_daf.add(
                     f, ((self.vm_db.stk(f) - self.ash_db.stk(f)) * 100 / (100 - self.ash_db.stk(f)))
                 )
                 self.fc_daf.add(
                     f, ((self.fc_db.stk(f) - self.ash_db.stk(f)) * 100 / (100 - self.ash_db.stk(f)))
                 )
+        self.proximate_computed = True
 
-            idxs_dtg = [
-                np.argmax(self.temp.stk(f) > self.temp_lim_dtg[0]),
-                np.argmax(self.temp.stk(f) > self.temp_lim_dtg[1]),
-            ]
-            # temp_dtg is taken fixed
+    def dtg_analysis(self):
+        """
+        Compute the derivative thermogravimetric (DTG) data for the sample.
 
-            # time start from 0 and consideres a fixed heating rate
-            self.time_dtg.add(
-                f,
-                np.linspace(
-                    0,
-                    self.time.stk(f)[idxs_dtg[1]] - self.time.stk(f)[idxs_dtg[0]],
-                    self.len_dtg_db,
-                ),
-            )
+        This method calculates the DTG data based on the thermogravimetric data and stores the results
+        in the instance's attributes for later use.
+        """
+        if not self.proximate_computed:
+            self.proximate_analysis()
 
-            self.mp_db_dtg.add(
-                f,
-                np.interp(
-                    self.temp_dtg,
-                    self.temp.stk(f)[idxs_dtg[0] : idxs_dtg[1]],
-                    self.mp_db.stk(f)[idxs_dtg[0] : idxs_dtg[1]],
-                ),
-            )
-            # the combusiton indexes use rates as /min
-            if self.dtg_basis == "temperature":
-                dtg = np.gradient(self.mp_db_dtg.stk(f), self.temp_dtg)
-            if self.dtg_basis == "time":
-                dtg = np.gradient(self.mp_db_dtg.stk(f), self.time_dtg.stk(f))
-            self.dtg_db.add(f, savgol_filter(dtg, self.dtg_window_filter, 1))
+        idxs_in_dtg = []
+        idxs_fin_dtg = []
+        vector_len_dtg = []
+        for f in range(self.n_repl):
+            idxs_in_dtg.append(np.argmax(self.temp.stk(f) > self.temp_lim_dtg[0]))
+            idxs_fin_dtg.append(np.argmax(self.temp.stk(f) > self.temp_lim_dtg[1]))
+            vector_len_dtg.append(idxs_fin_dtg[f] - idxs_in_dtg[f])
+        min_vector_len_dtg = min(vector_len_dtg)
+        idxs_fin_dtg = [initial + min_vector_len_dtg for initial in idxs_in_dtg]
+
+        for f in range(self.n_repl):
+            time_dtg = self.time.stk(f)[idxs_in_dtg[f] : idxs_fin_dtg[f]]
+            self.time_dtg.add(f, time_dtg - np.min(time_dtg))  # starts from 0
+            self.temp_dtg.add(f, self.temp.stk(f)[idxs_in_dtg[f] : idxs_fin_dtg[f]])
+            self.mp_db_dtg.add(f, self.mp_db.stk(f)[idxs_in_dtg[f] : idxs_fin_dtg[f]])
+            dtg_db = np.gradient(self.mp_db_dtg.stk(f), self.time_dtg.stk(f))
+            if self.dtg_window_filter is not None:
+                self.dtg_db.add(f, savgol_filter(dtg_db, self.dtg_window_filter, 1))
+            else:
+                self.dtg_db.add(f, dtg_db)
         # average
         self.ave_dev_tga_perc = np.average(self.mp_db_dtg.std())
         print(f"Average TG [%] St. Dev. for replicates: {self.ave_dev_tga_perc:0.2f} %")
-        self.proximate_computed = True
+        self.dtg_computed = True
 
     def oxidation_analysis(self):
         """
         Conduct oxidation analysis on the sample's data.
 
         This method calculates various oxidation parameters such as the initial oxidation temperature (Ti),
         peak oxidation temperature (Tp), and final oxidation temperature (Tb). It also computes derivative
         parameters like maximum and average rates of weight loss. The results are stored in the instance's
         attributes for further analysis.
         """
-        if not self.proximate_computed:
-            self.proximate_analysis()
+        if not self.dtg_computed:
+            self.dtg_analysis()
 
         for f in range(self.n_repl):
             threshold: float = np.max(np.abs(self.dtg_db.stk(f))) * self.temp_i_temp_b_threshold
             # Ti = T at which dtg > Ti_thresh wt%/min after moisture removal
             self.temp_i_idx.add(f, int(np.argmax(np.abs(self.dtg_db.stk(f)) > threshold)))
-            self.temp_i.add(f, self.temp_dtg[self.temp_i_idx.stk(f)])
+            self.temp_i.add(f, self.temp_dtg.stk(f)[self.temp_i_idx.stk(f)])
             # Tp is the T of max abs(dtg)
             self.temp_p_idx.add(f, int(np.argmax(np.abs(self.dtg_db.stk(f)))))
-            self.temp_p.add(f, self.temp_dtg[self.temp_p_idx.stk(f)])
+            self.temp_p.add(f, self.temp_dtg.stk(f)[self.temp_p_idx.stk(f)])
             # Tb reaches < 1 wt%/min at end of curve
             try:
                 self.temp_b_idx.add(f, int(np.flatnonzero(self.dtg_db.stk(f) < -threshold)[-1]))
             except IndexError:  # the curve nevers goes above 1%
                 self.temp_b_idx.add(f, 0)
-            self.temp_b.add(f, self.temp_dtg[self.temp_b_idx.stk(f)])
+            self.temp_b.add(f, self.temp_dtg.stk(f)[self.temp_b_idx.stk(f)])
 
             self.dwdtemp_max.add(f, np.max(np.abs(self.dtg_db.stk(f))))
             self.dwdtemp_mean.add(f, np.average(np.abs(self.dtg_db.stk(f))))
             # combustion index
             self.s_combustion_index.add(
                 f,
                 (
@@ -1094,16 +1083,16 @@
         """
         Perform solid distribution analysis on the sample's data.
 
         This analysis calculates the weight loss at specified temperature steps, providing insight into
         the solid decomposition process. The results are used for generating solid distribution plots.
 
         """
-        if not self.proximate_computed:
-            self.proximate_analysis()
+        if not self.dtg_computed:
+            self.dtg_analysis()
 
         for f in range(self.n_repl):
             idxs = []
             for step in self.soliddist_steps_min:
                 idxs.append(np.argmax(self.time.stk(f) > step))
             self.temp_soliddist.add(f, self.temp.stk(f)[idxs])
             self.time_soliddist.add(f, self.time.stk(f)[idxs])
@@ -1150,15 +1139,15 @@
         :type sigma_maxs: list[float], optional
         :param amplitude_mins: Minimum allowed values for the amplitudes of the Gaussian peaks. If None, no bounds are applied.
         :type amplitude_mins: list[float], optional
         :param amplitude_maxs: Maximum allowed values for the amplitudes of the Gaussian peaks. If None, no bounds are applied.
         :type amplitude_maxs: list[float], optional
         """
         if not self.proximate_computed:
-            self.proximate_analysis()
+            self.dtg_analysis()
         n_peaks = len(centers)
         # self.dcv_best_fit_stk = np.zeros((self.len_dtg_db, self.n_repl))
         # self.dcv_r2_stk = np.zeros(self.n_repl)
 
         # self.dcv_peaks_stk = np.zeros((self.len_dtg_db, self.n_repl, n_peaks))
         if sigmas is None:
             sigmas = [1] * n_peaks
@@ -1193,18 +1182,18 @@
                 pars[prefix + "sigma"].set(value=sigmas[p], min=sigma_mins[p], max=sigma_maxs[p])
                 pars[prefix + "amplitude"].set(
                     value=amplitudes[p], min=amplitude_mins[p], max=amplitude_maxs[p]
                 )
                 model += peak_model
                 params.update(pars)
 
-            result = model.fit(y, params=params, x=self.temp_dtg)
+            result = model.fit(y, params=params, x=self.temp_dtg.stk(f))
             self.dcv_best_fit.add(f, -result.best_fit)
             self.dcv_r2.add(f, 1 - result.residual.var() / np.var(y))
-            components = result.eval_components(x=self.temp_dtg)
+            components = result.eval_components(x=self.temp_dtg.stk(f))
 
             for p in range(n_peaks):
                 prefix = f"peak_{p}"
                 if prefix in components:
                     self.dcv_peaks[p].add(f, -components[prefix])
                 else:
                     self.dcv_peaks[p].add(f, 0)
@@ -1282,16 +1271,16 @@
         of the sample's thermal decomposition behavior.
 
         :param kwargs: Additional keyword arguments for plot customization.
         :type kwargs: dict
         :return: A MyFigure instance containing the generated plot.
         :rtype: MyFigure
         """
-        if not self.proximate_computed:
-            self.proximate_analysis()
+        if not self.dtg_computed:
+            self.dtg_analysis()
         out_path = plib.Path(self.out_path, "single_sample_plots")
         out_path.mkdir(parents=True, exist_ok=True)
 
         default_kwargs = {
             "filename": self.name + "_tg_dtg",
             "out_path": out_path,
             "height": 8.53,
@@ -1357,45 +1346,17 @@
                 if f == self.n_repl - 1:  # only add at the end
                     mf.axs[0].plot(
                         [], [], marker="x", linestyle="None", color="grey", label="moist_loc"
                     )
                     mf.axs[2].plot(
                         [], [], marker="x", linestyle="None", color="grey", label="moist_loc"
                     )
-                # mf.axs[0].vlines(
-                #     self.time.stk(f)[self.idx_moist.stk(f)],
-                #     self.temp.stk(f)[self.idx_moist.stk(f)] - 50,
-                #     self.temp.stk(f)[self.idx_moist.stk(f)] + 50,
-                #     linestyle=linestyles[f],
-                #     color=colors[f],
-                # )
-                # mf.axs[2].vlines(
-                #     self.time.stk(f)[self.idx_moist.stk(f)],
-                #     self.mp_ar.stk(f)[self.idx_moist.stk(f)] - 5,
-                #     self.mp_ar.stk(f)[self.idx_moist.stk(f)] + 5,
-                #     linestyle=linestyles[f],
-                #     color=colors[f],
-                # )
 
             # only try to plot VM is the analysis includes it
             if self.time_vm:
-                # mf.axs[0].vlines(
-                #     self.time.stk(f)[self.idx_vm.stk(f)],
-                #     self.temp.stk(f)[self.idx_vm.stk(f)] - 50,
-                #     self.temp.stk(f)[self.idx_vm.stk(f)] + 50,
-                #     linestyle=linestyles[f],
-                #     color=colors[f],
-                # )
-                # mf.axs[4].vlines(
-                #     self.time.stk(f)[self.idx_vm.stk(f)],
-                #     self.mp_db.stk(f)[self.idx_vm.stk(f)] - 5,
-                #     self.mp_db.stk(f)[self.idx_vm.stk(f)] + 5,
-                #     linestyle=linestyles[f],
-                #     color=colors[f],
-                # )
                 mf.axs[0].plot(
                     self.time.stk(f)[self.idx_vm.stk(f)],
                     self.temp.stk(f)[self.idx_vm.stk(f)],
                     marker="+",
                     linestyle="None",
                     color=colors[f],
                 )
@@ -1412,15 +1373,15 @@
                     )
                     mf.axs[4].plot(
                         [], [], marker="+", linestyle="None", color="grey", label="vm_loc"
                     )
             # tg plot 1, 3, 5 on the right
             mf.axs[1].plot(
                 self.time_dtg.stk(f),
-                self.temp_dtg,
+                self.temp_dtg.stk(f),
                 color=colors[f],
                 linestyle=linestyles[f],
                 label=self.filenames[f],
             )
             mf.axs[3].plot(
                 self.time_dtg.stk(f),
                 self.mp_db_dtg.stk(f),
@@ -1433,35 +1394,14 @@
                 self.dtg_db.stk(f),
                 color=colors[f],
                 linestyle=linestyles[f],
                 label=self.filenames[f],
             )
             #
             if self.oxidation_computed:
-                # mf.axs[5].vlines(
-                #     self.time_dtg.stk(f)[self.temp_i_idx.stk(f)],
-                #     ymin=-1.5,
-                #     ymax=0,
-                #     linestyle=linestyles[f],
-                #     color=colors[f],
-                # )
-                # mf.axs[5].vlines(
-                #     self.time_dtg.stk(f)[self.temp_p_idx.stk(f)],
-                #     ymin=np.min(self.dtg_db.stk(f)),
-                #     ymax=np.min(self.dtg_db.stk(f)) / 5,
-                #     linestyle=linestyles[f],
-                #     color=colors[f],
-                # )
-                # mf.axs[5].vlines(
-                #     self.time_dtg.stk(f)[self.temp_b_idx.stk(f)],
-                #     ymin=-1.5,
-                #     ymax=0,
-                #     linestyle=linestyles[f],
-                #     color=colors[f],
-                # )
                 mf.axs[5].plot(
                     self.time_dtg.stk(f)[self.temp_i_idx.stk(f)],
                     self.dtg_db.stk(f)[self.temp_i_idx.stk(f)],
                     marker="x",
                     linestyle="None",
                     color=colors[f],
                 )
@@ -1584,28 +1524,33 @@
             rows=self.n_repl,
             cols=1,
             **kwargs,
         )
 
         # Plot DTG data
         for f in range(self.n_repl):
-            mf.axs[f].plot(self.temp_dtg, self.dtg_db.stk(f), color="black", label="DTG")
+            mf.axs[f].plot(
+                self.temp_dtg.stk(f),
+                self.dtg_db.stk(f),
+                color="black",
+                label="DTG",
+            )
             # Plot best fit and individual peaks
             mf.axs[f].plot(
-                self.temp_dtg,
+                self.temp_dtg.stk(f),
                 self.dcv_best_fit.stk(f),
                 label="best fit",
                 color="red",
                 linestyle="--",
             )
             colors_p = colors[:3] + colors[5:]  # avoid using red
             for p, peak in enumerate(self.dcv_peaks):
                 if peak.stk(f) is not None:
                     mf.axs[f].plot(
-                        self.temp_dtg,
+                        self.temp_dtg.stk(f),
                         peak.stk(f),
                         label=peak.name,
                         color=colors_p[p],
                         linestyle=linestyles[p],
                     )
             mf.axs[f].annotate(
                 f"r$^2$={self.dcv_r2.stk(f):.2f}",
```

### Comparing `tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/PKG-INFO` & `tga_data_analysis-2.2.0/src/tga_data_analysis.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tga_data_analysis
-Version: 2.1.0
+Version: 2.2.0
 Summary: Tool for automatic analysis of multiple TGA results
 Author: Matteo Pecchi
 License: MIT
 Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
 Project-URL: Documentation, https://tga-data-analysis.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -111,16 +111,15 @@
 * ``temp_initial_celsius``: The initial temperature where every ``File`` is going to start to ensure uniformity.
 
 * ``temp_lim_dtg_celsius``: The temperature limits for DTG analysis, in Celsius. It should exclude moisture and fixed 
 carbon segments.
 
 * ``temp_unit``: The unit of temperature the project will convert everything to, not the unit in the ``Files``. 
 
-* ``resolution_sec_deg_dtg``: The resolution in seconds per degree for the common temperature vector used in the DTG 
-analysis.
+* ``dtg_basis`` and ``resolution_sec_deg_dtg``: these parameters are no longer available and raise exceptions if specified. The dtg curve is now only computed as dTG/dtime (temperature is used for plotting), but replicates are not interpolated anymore so the resolution reflects the data resolution from the machine.
 
 * ``dtg_window_filter``: The window size for the Savitzky-Golay filter used to smooth the DTG curve.
 
 * ``temp_i_temp_b_threshold``: The fractional threshold for the detection of Ti (t_ignition) and Tb (burnout) calculation in DTG analysis.
 
 **Example**
```

### Comparing `tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/SOURCES.txt` & `tga_data_analysis-2.2.0/src/tga_data_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.1.0/tests/test_deconvolution.py` & `tga_data_analysis-2.2.0/tests/test_deconvolution.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 threshold = 1e-5
 
 
 # %%
 @pytest.mark.parametrize("temp_symbol", ["C", "K"])
 def test_deconvolution_with_temperature(test_dir, temp_symbol):
 
-    proj = Project(test_dir, name="test", temp_unit=temp_symbol)
+    proj = Project(test_dir, name="test", temp_unit=temp_symbol, dtg_window_filter=101)
 
     misc = Sample(
         project=proj, name="misc", filenames=["MIS_1", "MIS_2", "MIS_3"], time_moist=38, time_vm=147
     )
     if temp_symbol == "K":
         misc.deconv_analysis([280 + 273.15, 380 + 273.15])
     else:
         misc.deconv_analysis([280, 380])
 
-    assert abs(min(misc.dcv_best_fit()) + 1.0045394426179157) <= threshold
+    assert abs(min(misc.dcv_best_fit()) + 10.542964622868018) <= threshold
 
 
 # %%
```

### Comparing `tga_data_analysis-2.1.0/tests/test_kas_kinetics.py` & `tga_data_analysis-2.2.0/tests/test_kas_kinetics.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from tga_data_analysis.kas_kinetics import KasSample
 
 threshold = 1e-5
 
 
 # %%
 @pytest.mark.parametrize("temp_symbol", ["C", "K"])
-def test_deconvolution_with_temperature(test_dir, temp_symbol):
+def test_kas_kinetics_with_temperature(test_dir, temp_symbol):
 
     proj = Project(folder_path=test_dir, name="test", temp_unit=temp_symbol)
     cell_ox5 = Sample(
         project=proj,
         name="cell_ox5",
         filenames=["CLSOx5_1", "CLSOx5_2", "CLSOx5_3"],
         time_moist=38,
@@ -45,32 +45,31 @@
         name="cell_ox100",
         load_skiprows=8,
         filenames=["CLSOx100_4", "CLSOx100_5", "CLSOx100_6"],
         time_moist=38,
         time_vm=None,
         heating_rate_deg_min=100,
     )
-    # %%
     cell = KasSample(proj, samples=[cell_ox5, cell_ox10, cell_ox50, cell_ox100], name="cellulose")
     cell.kas_analysis()
     checked_results = [
-        184.43662974,
-        179.45539645,
-        175.97863874,
-        175.39423197,
-        174.07068577,
-        173.61644355,
-        172.75240559,
-        172.29217511,
-        172.20614031,
-        172.57585466,
-        172.27021231,
-        172.9921345,
-        178.61935678,
-        197.75950085,
-        250.29872367,
+        182.98695498901722,
+        177.93533544211007,
+        175.00305447358866,
+        174.24922678890448,
+        173.10247795834562,
+        172.17212058541972,
+        172.38983956887415,
+        171.32000094274244,
+        171.9362038980991,
+        171.33484227896233,
+        171.9242539930856,
+        172.52779644872686,
+        177.92903770087554,
+        195.65939854731468,
+        247.71378828071303,
     ]
     for result, checked_result in zip(list(cell.activation_energy), checked_results):
         assert abs(result - checked_result) <= threshold
 
 
 # %%
```

### Comparing `tga_data_analysis-2.1.0/tests/test_measure.py` & `tga_data_analysis-2.2.0/tests/test_measure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.1.0/tests/test_soliddist.py` & `tga_data_analysis-2.2.0/tests/test_soliddist.py`

 * *Files identical despite different names*

