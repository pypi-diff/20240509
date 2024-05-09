# Comparing `tmp/neuroanalysis-0.0.1.tar.gz` & `tmp/neuroanalysis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/neuroanalysis-0.0.1.tar", last modified: Tue Dec  7 21:00:53 2021, max compression
+gzip compressed data, was "neuroanalysis-0.0.2.tar", last modified: Thu May  9 15:45:35 2024, max compression
```

## Comparing `neuroanalysis-0.0.1.tar` & `neuroanalysis-0.0.2.tar`

### file list

```diff
@@ -1,81 +1,84 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1907 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      824 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis/
--rw-rw-r--   0 martin    (1000) martin    (1000)       22 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis/analyzers/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/analyzers/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      605 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/analyzers/analyzer.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2151 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/analyzers/baseline.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10530 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/analyzers/stim_pulse.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2164 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/baseline.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis/data/
--rw-rw-r--   0 martin    (1000) martin    (1000)       39 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/data/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    49806 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/data/dataset.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis/data/loaders/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/data/loaders/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8461 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/data/loaders/acq4_dataset_loader.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1587 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/data/loaders/loaders.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    22178 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/data/loaders/mies_dataset_loader.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    13959 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/event_detection.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4413 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/filter.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis/fitting/
--rw-rw-r--   0 martin    (1000) martin    (1000)      256 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/fitting/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1142 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/fitting/exp.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      532 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/fitting/fit_scale_offset.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5550 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/fitting/fitmodel.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      464 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/fitting/gaussian.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    17465 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/fitting/psp.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3286 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/fitting/searchfit.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      454 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/fitting/sigmoid.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    32370 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/miesnwb.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis/neuronsim/
--rw-rw-r--   0 martin    (1000) martin    (1000)      160 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/neuronsim/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5365 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/neuronsim/components.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    14517 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/neuronsim/mechanisms.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3963 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/neuronsim/model_cell.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8882 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/neuronsim/sim.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    12943 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/spike_detection.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4654 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/stats.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    29351 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/stimuli.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    12166 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/synaptic_release.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8362 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/test_pulse.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis/ui/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      811 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/baseline.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3836 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/cell_selector.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5335 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/event_detection.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1988 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/filter.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7957 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/fitting.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis/ui/nwb_viewer/
--rw-rw-r--   0 martin    (1000) martin    (1000)       51 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/nwb_viewer/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2476 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/nwb_viewer/analyzer_view.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4227 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/nwb_viewer/sweep_view.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    12671 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/nwb_viewer/viewer.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       50 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/plot_adapter.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2833 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/plot_grid.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1557 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/psp_fitting.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1019 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/signal.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1838 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/spike_detection.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4411 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/sta_analyzer.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2574 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/triggered_average.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2185 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/ui/user_test.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      565 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/units.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis/util/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/util/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      671 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/util/custom_weakref.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4960 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/util/data_test.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      622 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/util/jit.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      174 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/util/lru_cache.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      667 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/util/merge_lists.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7112 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/util/mies_nwb_parsing.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2114 2021-12-02 19:56:08.000000 neuroanalysis-0.0.1/neuroanalysis/util/optional_import.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1907 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2228 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       18 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       14 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/neuroanalysis.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      107 2021-12-07 20:39:30.000000 neuroanalysis-0.0.1/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2021-12-07 21:00:53.000000 neuroanalysis-0.0.1/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     1403 2021-12-07 20:56:53.000000 neuroanalysis-0.0.1/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-09 15:45:35.282481 neuroanalysis-0.0.2/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1095 2021-12-09 22:35:00.000000 neuroanalysis-0.0.2/LICENSE.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)     1749 2024-05-09 15:45:35.282481 neuroanalysis-0.0.2/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      824 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-09 15:45:35.278481 neuroanalysis-0.0.2/neuroanalysis/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       22 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-09 15:45:35.278481 neuroanalysis-0.0.2/neuroanalysis/analyzers/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/analyzers/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      605 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/analyzers/analyzer.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2151 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/analyzers/baseline.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10693 2022-05-31 17:11:36.000000 neuroanalysis-0.0.2/neuroanalysis/analyzers/stim_pulse.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2164 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/baseline.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-09 15:45:35.278481 neuroanalysis-0.0.2/neuroanalysis/data/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       39 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/data/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    49591 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/data/dataset.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-09 15:45:35.278481 neuroanalysis-0.0.2/neuroanalysis/data/loaders/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/data/loaders/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8284 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/data/loaders/acq4_dataset_loader.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1910 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/data/loaders/loaders.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    22178 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/data/loaders/mies_dataset_loader.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    13959 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/event_detection.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4413 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/filter.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-09 15:45:35.278481 neuroanalysis-0.0.2/neuroanalysis/fitting/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      256 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/fitting/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4596 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/fitting/exp.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      532 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/fitting/fit_scale_offset.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5550 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/fitting/fitmodel.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      464 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/fitting/gaussian.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17755 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/fitting/psp.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3286 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/fitting/searchfit.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      454 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/fitting/sigmoid.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    32592 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/miesnwb.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-09 15:45:35.278481 neuroanalysis-0.0.2/neuroanalysis/neuronsim/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      160 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/neuronsim/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5169 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/neuronsim/components.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    14474 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/neuronsim/mechanisms.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3960 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/neuronsim/model_cell.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12640 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/neuronsim/sim.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12943 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/spike_detection.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4654 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/stats.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    31546 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/stimuli.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12166 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/synaptic_release.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7782 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/test_pulse.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-09 15:45:35.282481 neuroanalysis-0.0.2/neuroanalysis/ui/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/ui/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      815 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/baseline.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3836 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/ui/cell_selector.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5339 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/event_detection.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1992 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/filter.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7935 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/fitting.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-09 15:45:35.282481 neuroanalysis-0.0.2/neuroanalysis/ui/nwb_viewer/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       51 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/ui/nwb_viewer/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2492 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/nwb_viewer/analyzer_view.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4243 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/nwb_viewer/sweep_view.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12763 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/nwb_viewer/viewer.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       50 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/ui/plot_adapter.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2794 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/plot_grid.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1561 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/psp_fitting.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      255 2024-03-08 22:13:00.000000 neuroanalysis-0.0.2/neuroanalysis/ui/qt.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1019 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/ui/signal.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1842 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/spike_detection.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4439 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/sta_analyzer.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2578 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/triggered_average.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2213 2024-05-09 15:33:45.000000 neuroanalysis-0.0.2/neuroanalysis/ui/user_test.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      565 2024-04-20 00:13:27.000000 neuroanalysis-0.0.2/neuroanalysis/units.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-09 15:45:35.282481 neuroanalysis-0.0.2/neuroanalysis/util/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/util/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      671 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/util/custom_weakref.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4960 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/util/data_test.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1122 2022-05-31 17:11:36.000000 neuroanalysis-0.0.2/neuroanalysis/util/h5py_wrapper.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      622 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/util/jit.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      174 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/util/lru_cache.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      667 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/util/merge_lists.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7112 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/util/mies_nwb_parsing.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2114 2021-12-02 19:56:08.000000 neuroanalysis-0.0.2/neuroanalysis/util/optional_import.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-09 15:45:35.282481 neuroanalysis-0.0.2/neuroanalysis.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     1749 2024-05-09 15:45:35.000000 neuroanalysis-0.0.2/neuroanalysis.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2298 2024-05-09 15:45:35.000000 neuroanalysis-0.0.2/neuroanalysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-05-09 15:45:35.000000 neuroanalysis-0.0.2/neuroanalysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       18 2024-05-09 15:45:35.000000 neuroanalysis-0.0.2/neuroanalysis.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       14 2024-05-09 15:45:35.000000 neuroanalysis-0.0.2/neuroanalysis.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      107 2021-12-09 22:35:00.000000 neuroanalysis-0.0.2/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2024-05-09 15:45:35.282481 neuroanalysis-0.0.2/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1403 2024-05-09 15:43:10.000000 neuroanalysis-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `neuroanalysis-0.0.1/PKG-INFO` & `neuroanalysis-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: neuroanalysis
-Version: 0.0.1
+Version: 0.0.2
 Summary: Functions and modular user interface tools for analysis of patch clamp experiment data.
 Home-page: https://github.com/AllenInstitute/neuroanalysis
 Author: Luke Campagnola
 Author-email: lukec@alleninstitute.org
 License: MIT
-Description: Neuroanalysis
-        =============
-        
-        Modular and interactive tools for analysis of neurophysiology data, with emphasis on 
-        patch-clamp electrophysiology.
-        
-        * Functions for running common analysis algorithms
-            * Synaptic/calcium event detection and characterization
-            * Synaptic release modeling
-            * VC and CC spike detection and characterization
-            * VC and CC test pulse analysis
-            * Basic signal processing (filtering, baseline removal, etc.)
-        * Data abstraction layer to allow adapting new data formats (see neuroanalysis/data.py)
-        * Re-usable user interface elements for implementing common analysis tasks
-        
-        
-        Status
-        ------
-        
-        This project is early in development and does not yet have a stable API.
-        Issues and pull requests are accepted (see CONTRIBUTING.md), but may not be 
-        reviewed or accepted on any fixed schedule.
-        
-        
-        
-        
-        
-        
 Keywords: neuroscience analysis neurodata without borders nwb
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: lmfit
+Requires-Dist: numpy
+Requires-Dist: scipy
+
+Neuroanalysis
+=============
+
+Modular and interactive tools for analysis of neurophysiology data, with emphasis on 
+patch-clamp electrophysiology.
+
+* Functions for running common analysis algorithms
+    * Synaptic/calcium event detection and characterization
+    * Synaptic release modeling
+    * VC and CC spike detection and characterization
+    * VC and CC test pulse analysis
+    * Basic signal processing (filtering, baseline removal, etc.)
+* Data abstraction layer to allow adapting new data formats (see neuroanalysis/data.py)
+* Re-usable user interface elements for implementing common analysis tasks
+
+
+Status
+------
+
+This project is early in development and does not yet have a stable API.
+Issues and pull requests are accepted (see CONTRIBUTING.md), but may not be 
+reviewed or accepted on any fixed schedule.
+
+
+
+
+
```

### Comparing `neuroanalysis-0.0.1/README.md` & `neuroanalysis-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/analyzers/analyzer.py` & `neuroanalysis-0.0.2/neuroanalysis/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/analyzers/baseline.py` & `neuroanalysis-0.0.2/neuroanalysis/analyzers/baseline.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/analyzers/stim_pulse.py` & `neuroanalysis-0.0.2/neuroanalysis/analyzers/stim_pulse.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,34 +201,38 @@
 
         """
         pre_trace = self.rec['primary']
 
         # Detect pulse times
         pulses = self.pulses()
 
+        # filter out test pulse if it exists
+        stim_pulses = pulses[1:] if self.rec.has_inserted_test_pulse else pulses
+        
         # cut out a chunk for each pulse
         chunks = []
-        for i,pulse in enumerate(pulses):
+        for i,pulse in enumerate(stim_pulses):
             pulse_start_time, pulse_end_time, amp = pulse
             if amp < 0:
                 # assume negative pulses do not evoke spikes
                 # (todo: should be watching for rebound spikes as well)
                 continue
             # cut out a chunk of the recording for spike detection
             start_time = pulse_start_time - 2e-3
             stop_time = pulse_end_time + 4e-3
-            if i < len(pulses) - 1:
+            if i < len(stim_pulses) - 1:
                 # truncate chunk if another pulse is present
-                next_pulse_time = pulses[i+1][0]
+                next_pulse_time = stim_pulses[i+1][0]
                 stop_time = min(stop_time, next_pulse_time)
             chunk = self.rec.time_slice(start_time, stop_time)
             chunk.meta['pulse_edges'] = [pulse_start_time, pulse_end_time]
             chunk.meta['pulse_amplitude'] = amp
             chunk.meta['pulse_n'] = i
             chunks.append(chunk)
+            
         return chunks
 
     def evoked_spikes(self):
         """Given presynaptic Recording, detect action potentials
         evoked by current injection or unclamped spikes evoked by a voltage pulse.
 
         Returns
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/baseline.py` & `neuroanalysis-0.0.2/neuroanalysis/baseline.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/data/dataset.py` & `neuroanalysis-0.0.2/neuroanalysis/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,18 @@
 (as long as the data are reasonably similar), and analysis tools should rely only on this API to ensure
 that they will not need to be rewritten in order to support data collected under different acquisition
 systems.
 
 This abstraction layer also helps to enforce good coding practice by separating data representation,
 analysis, and visualization.
 """
-from __future__ import division
+from collections import OrderedDict
 
 import numpy as np
-import scipy.signal
-from .. import util
-from collections import OrderedDict
-from ..stats import ragged_mean
+
 from ..baseline import float_mode
 from ..filter import downsample
 
 
 class Container(object):
     """Generic hierarchical container. 
     
@@ -215,15 +212,14 @@
         """Alias for self.contents
         
         This is a convenience property used for traversing the object hierarchy.
         """
         return self.contents
     
     
-
 # class RecordingSequence(Container):
 
 # For now, possibly forever, remove the concept of Sequences from datasets. 
 # It is too hard to decide programatically which sync recordings should make up a sequence,
 # and it is likely that that will change or be highly specific to each type of experiment,
 # and will likely involve manual annotation.
 # So, I think that sorting sync recordings into sequences should be something that happens at a 
@@ -490,27 +486,22 @@
     def time_slice(self, start, stop):
         return RecordingView(self, start, stop)
 
     def __getitem__(self, chan):
         return self._channels[chan]
 
     def data(self):
-        #return np.concatenate([self[ch].data[:,None] for ch in self.channels], axis=1)
         return np.stack([self[ch].data for ch in self.channels], axis=-1)
 
-    # @property
-    # def parent(self):
-    #     return self.sync_recording
-    
     @property
     def children(self):
         return [self[k] for k in self.channels]
 
     def __repr__(self):
-        return "<%s device:%s, channels:%s>" %(self.__class__.__name__, self.device_type, str(self.channels))
+        return f"<{self.__class__.__name__} device:{self.device_type}, channels:{str(self.channels)}>"
 
 
 class RecordingView(Recording):
     """A time-slice of a multi channel recording
     """
     def __init__(self, rec, start, stop):
         self._parent_rec = rec
@@ -716,29 +707,27 @@
             data = self.baseline_data.data
             if len(data) == 0:
                 return None
             self.meta['baseline_rms_noise'] = data.std()
         return self.meta['baseline_rms_noise']
 
     def _descr(self):
-        mode = self.clamp_mode
-        if mode == 'vc':
+        if self.clamp_mode == 'vc':
             hp = self.holding_potential
             if hp is not None:
-                hp = int(np.round(hp*1e3))
-            extra = "mode=VC holding=%s" % hp
-        elif mode == 'ic':
+                hp = int(np.round(hp * 1e3))
+            return f"mode=VC holding={hp}"
+        else:
             hc = self.holding_current
             if hc is not None:
-                hc = int(np.round(hc*1e12))
-            extra = "mode=IC holding=%s" % hc
-        return extra
+                hc = int(np.round(hc * 1e12))
+            return f"mode=IC holding={hc}"
 
     def __repr__(self):
-        return "<%s device:%s %s>" % (self.__class__.__name__, str(self.device_id), self._descr())
+        return f"<{self.__class__.__name__} device:{self.device_id} {self._descr()}>"
 
 
 class TSeries(Container):
     """A homogeneous time series data set. 
     
     This is a representation of a single stream of data recorded over time. The
     data must be representable as a single N-dimensional array where the first
@@ -783,15 +772,15 @@
         The Recording this TSeries is part of.
     loader : a class | None
         A class containing functions for loading data. Required methods:
             get_tseries_data(self) - return a numpy array of values
     meta : 
         Any extra keyword arguments are interpreted as custom metadata and added to ``self.meta``.
     """
-    def __init__(self, data=None, dt=None, t0=None, sample_rate=None, start_time=None, time_values=None, units=None, channel_id=None, recording=None, loader=None, **meta):
+    def __init__(self, data: np.ndarray = None, dt=None, t0=None, sample_rate=None, start_time=None, time_values: np.ndarray = None, units=None, channel_id=None, recording=None, loader=None, **meta):
         Container.__init__(self, loader=loader)
         
         #if data is not None and data.ndim != 1:
         #    raise ValueError("data must be a 1-dimensional array.")
         
         if time_values is not None:
             if data is not None and time_values.shape[0] != data.shape[0]:
@@ -961,15 +950,14 @@
             inds0 = inds1 - 1
             # select closest sample
             dif1 = abs(self.time_values[np.clip(inds1, 0, len(self)-1)] - t)
             dif0 = abs(self.time_values[inds0] - t)
             inds = np.where(dif0 < dif1, inds0, inds1)
             if np.isscalar(t):
                 inds = int(inds)
-            return inds
         else:
             # Be careful to avoid fp precision errors when converting back to integer index
             sample_rate = self._meta.get('sample_rate')
             if sample_rate is None:
                 inds = (t - self.t0) * (1.0 / self.dt)
             else:
                 inds = (t - self.t0) * sample_rate
@@ -980,17 +968,18 @@
                 inds = np.floor(inds)
             elif index_mode == 'ceil':
                 inds = np.ceil(inds)
             else:
                 raise ValueError("index_mode must be 'round', 'ceil', or 'floor'; got %r" % index_mode)
 
             if np.isscalar(t):
-                return int(inds)        
+                inds = int(inds)
             else:
-                return inds.astype(int)
+                inds = inds.astype(int)
+        return min(max(0, inds), len(self) - 1)
 
     @property
     def time_values(self):
         """An array of sample time values.
         
         Time values are specified in seconds relative to start_time.
         
@@ -1147,14 +1136,18 @@
     
     @property
     def recording(self):
         """The Recording that contains this trace.
         """
         return self._recording
 
+    @recording.setter
+    def recording(self, new_val):
+        self._recording = new_val
+
     def copy(self, data=None, time_values=None, **kwds):
         """Return a copy of this TSeries.
         
         The new TSeries will have the same data, timing information, and metadata
         unless otherwise specified in the arguments.
         
         Parameters
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/data/loaders/acq4_dataset_loader.py` & `neuroanalysis-0.0.2/neuroanalysis/data/loaders/acq4_dataset_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from datetime import datetime
 from neuroanalysis.data.loaders.loaders import DatasetLoader
 from acq4.util import DataManager
 from acq4.analysis.dataModels import PatchEPhys
 from neuroanalysis.data.dataset import Recording, SyncRecording, TSeries, PatchClampRecording
 import neuroanalysis.stimuli as stimuli
 
-class Acq4DatasetLoader(DatasetLoader):
 
+class Acq4DatasetLoader(DatasetLoader):
     def __init__(self, filepath):
 
         self._filepath = filepath
 
         self._dh = None ## directory handle
 
     @property
@@ -43,20 +43,19 @@
                 #sequences.append(sequence)
             elif self.dh[seq].info().get('dirType') == 'Protocol':
                 srec = SyncRecording(parent=dataset, key=(seq), loader=self)
                 sync_recs.append(srec)
             elif self.dh[seq].shortName() == 'Patch': ## ignore this for now -- how should this data be represented?
                 continue
             else:
-                raise Exception('Not sure how to handle folder %s' % self.dh[seq].name())
+                raise ValueError(f'Not sure how to handle folder {self.dh[seq].name()}')
 
         #return (sync_recs, sequences)
         return sync_recs
         
-
     def get_recordings(self, sync_rec):
         """Return a dict of {device: Recording}"""
         key = sync_rec.key
         dh = self.dh
         for k in key:
             dh = dh[k]
 
@@ -70,24 +69,25 @@
                 files.append(f)
 
         recordings = {}
         for f in files:
             start_time=datetime.utcfromtimestamp(PatchEPhys.getParent(f, 'Protocol').info()['startTime'])
 
             if PatchEPhys.isClampFile(f):
-                meta = {}
-                meta['file_name'] = f.name()
-                meta['clamp_mode'] = PatchEPhys.getClampMode(f).lower()
+                meta = {
+                    'file_name': f.name(),
+                    'clamp_mode': PatchEPhys.getClampMode(f).lower(),
+                }
                 if meta['clamp_mode'] == 'vc':
                     meta['holding_current'] = PatchEPhys.getClampHoldingLevel(f)
                 elif meta['clamp_mode'] == 'ic':
                     meta['holding_potential'] = PatchEPhys.getClampHoldingLevel(f)
                     meta['bridge_balance'] = PatchEPhys.getBridgeBalanceCompensation(f)
                 else:
-                    raise Exception("dont know how to interpret %s clamp_mode" % meta['clamp_mode'])
+                    raise ValueError(f"dont know how to interpret {meta['clamp_mode']} clamp_mode")
 
                 data = f.read()
                 dt = data.axisValues(1)[1] - data.axisValues(1)[0]
 
                 rec = PatchClampRecording(
                     channels={'primary':TSeries(channel_id='primary', data=data['primary'].asarray(), dt=dt, units=data.columnUnits(0, 'primary'), loader=self),
                               'command':TSeries(channel_id='command', data=data['command'].asarray(), dt=dt, units=data.columnUnits(0, 'command'), loader=self)},
@@ -97,16 +97,14 @@
                     sync_recording=sync_rec,
                     loader=self,
                     **meta
                     )
                 rec['primary']._recording = rec
                 rec['command']._recording = rec
 
-                recordings[f.name(relativeTo=dh)] = rec
-
             else:
                 data = f.read()
                 time_axis = data._getAxis('Time') ## is there a way to do this without using a private MA function?
                 if 'Channel' in data.listColumns().keys():
                     channel_axis = data._getAxis('Channel')
 
                 #dt = data.axisValues(time_axis)[1] - data.axisValues(time_axis)[0]
@@ -125,62 +123,56 @@
                     loader=self,
                     **data.infoCopy()[-1]
                     )
 
                 for k in rec.channels:
                     rec[k]._recording = rec
 
-                recordings[f.name(relativeTo=dh)] = rec
+            recordings[f.name(relativeTo=dh)] = rec
 
         return recordings
 
-
     def get_tseries_data(self, tseries):
         """Return a numpy array of the data in the tseries."""
         #### I don't think we need this because we hand TSeries their data when we instantiate them.
         raise NotImplementedError("Must be implemented in subclass. -- This should only get called if we're using lazy loading.")
 
-    def load_stimulus(self, recording):
-        """Return an instance of stimuli.Stimulus"""
-
-        #### I don't know whether I should try to parse this from metadata, or just find square pulses in the command waveform. 
+    def load_stimulus(self, recording) -> stimuli.Stimulus:
+        #### I don't know whether I should try to parse this from metadata, or just find square pulses in the command waveform.
         ### I think finding square pulses would be simpler, but makes the assumption that pulses are square. Which is probably usually true.
         ### what if I check the wavegenerator widget data for the function name (pulse) and then findSquarepulses, or raise an exception if it's a different function?
-        if isinstance(recording, PatchClampRecording):
-            items = []
-
-            fh = DataManager.getFileHandle(recording.meta['file_name'])
-            seqDir = PatchEPhys.getParent(fh, 'ProtocolSequence')
-            if seqDir is not None:
-                dev_info = seqDir.info()['devices'][recording.device_id]
-
-                if dev_info['mode'].lower() == 'vc':
-                    units = 'V'
-                elif dev_info['mode'].lower() == 'ic':
-                    units = 'A'
-                else:
-                    units = None
+        if not isinstance(recording, PatchClampRecording):
+            raise NotImplementedError('not implemented yet')
+        fh = DataManager.getFileHandle(recording.meta['file_name'])
+        seqDir = PatchEPhys.getParent(fh, 'ProtocolSequence')
+        if seqDir is not None:
+            dev_info = seqDir.info()['devices'][recording.device_id]
+
+            if dev_info['mode'].lower() == 'vc':
+                units = 'V'
+            elif dev_info['mode'].lower() == 'ic':
+                units = 'A'
+            else:
+                units = None
 
-                if dev_info['holdingCheck']:
-                    items.append(stimuli.Offset(dev_info['holdingSpin']))
+            items = []
 
-                stim_pulses = PatchEPhys.getStimParams(fh)
+            if dev_info['holdingCheck']:
+                items.append(stimuli.Offset(dev_info['holdingSpin']))
 
-                for p in stim_pulses:
-                    if p['function_type'] == 'pulse':
-                        items.append(stimuli.SquarePulse(p['start'], p['length'], p['amplitude']))
-                    elif p['function_type'] == 'pulseTrain':
-                        items.append(stimuli.SquarePulseTrain(p['start'], p['pulse_number'], p['length'], p['amplitude'], p['period']))
+            stim_pulses = PatchEPhys.getStimParams(fh)
 
-                desc = seqDir.shortName()[:-4]
-                return stimuli.Stimulus(desc, items=items, units=units)
+            for p in stim_pulses:
+                if p['function_type'] == 'pulse':
+                    items.append(stimuli.SquarePulse(p['start'], p['length'], p['amplitude']))
+                elif p['function_type'] == 'pulseTrain':
+                    items.append(stimuli.SquarePulseTrain(p['start'], p['pulse_number'], p['length'], p['amplitude'], p['period']))
 
-        else:
-            raise Exception('not implemented yet')
-        
+            desc = seqDir.shortName()[:-4]
+            return stimuli.Stimulus(desc, items=items, units=units)
 
     def load_stimulus_items(self, recording):
         """Return a list of Stimulus instances. 
         Used with LazyLoadStimulus to parse stimuli when they are needed."""
         raise NotImplementedError("Must be implemented in subclass.")
 
     def load_test_pulse(self, recording):
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/data/loaders/loaders.py` & `neuroanalysis-0.0.2/neuroanalysis/data/loaders/loaders.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,43 @@
+import numpy as np
 
+from neuroanalysis.data import PatchClampRecording, SyncRecording
+from neuroanalysis.stimuli import Stimulus
+from neuroanalysis.test_pulse import PatchClampTestPulse
 
-class DatasetLoader():
+
+class DatasetLoader(object):
     """An abstract base class for Dataset loaders."""
     
-    def get_dataset_name(self):
+    def get_dataset_name(self) -> str:
         """Return a string with the name of this dataset."""
         raise NotImplementedError("Must be implemented in subclass.")
 
-    def get_sync_recordings(self, dataset):
+    def get_sync_recordings(self, dataset) -> list[SyncRecording]:
         """Return a tuple (list of SyncRecordings, list of RecordingSequences)."""
         raise NotImplementedError("Must be implemented in subclass.")
 
-    def get_recordings(self, sync_rec):
+    def get_recordings(self, sync_rec) -> dict[str, PatchClampRecording]:
         """Return a dict of {device: Recording}"""
         raise NotImplementedError("Must be implemented in subclass.")
 
-    def get_tseries_data(self, tseries):
+    def get_tseries_data(self, tseries) -> np.ndarray:
         """Return a numpy array of the data in the tseries."""
         raise NotImplementedError("Must be implemented in subclass.")
 
-    def load_stimulus(self, recording):
+    def load_stimulus(self, recording) -> Stimulus:
         """Return an instance of stimuli.Stimulus"""
         raise NotImplementedError("Must be implemented in subclass.")
 
-    def load_stimulus_items(self, recording):
+    def load_stimulus_items(self, recording) -> list[Stimulus]:
         """Return a list of Stimulus instances. 
         Used with LazyLoadStimulus to parse stimuli when they are needed."""
         raise NotImplementedError("Must be implemented in subclass.")
 
-    def load_test_pulse(self, recording):
+    def load_test_pulse(self, recording) -> PatchClampTestPulse:
         """Return a PatchClampTestPulse."""
         raise NotImplementedError("Must be implemented in subclass.")
 
     def find_nearest_test_pulse(self, recording):
         raise NotImplementedError("Must be implemented in subclass.")
 
     def get_baseline_regions(self, recording):
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/data/loaders/mies_dataset_loader.py` & `neuroanalysis-0.0.2/neuroanalysis/data/loaders/mies_dataset_loader.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/event_detection.py` & `neuroanalysis-0.0.2/neuroanalysis/event_detection.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/filter.py` & `neuroanalysis-0.0.2/neuroanalysis/filter.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/fitting/fit_scale_offset.py` & `neuroanalysis-0.0.2/neuroanalysis/fitting/fit_scale_offset.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/fitting/fitmodel.py` & `neuroanalysis-0.0.2/neuroanalysis/fitting/fitmodel.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/fitting/psp.py` & `neuroanalysis-0.0.2/neuroanalysis/fitting/psp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from __future__ import print_function, division
-
-import sys, json, warnings
+import json, warnings
 import numpy as np
 import scipy.optimize
+from scipy.special import lambertw
 from ..data import Trace
 from ..util.data_test import DataTestCase
 from ..baseline import float_mode
 from .fitmodel import FitModel
 from .searchfit import SearchFit
 from ..util.jit import numba_jit
 from ..util.lru_cache import lru_cache
@@ -69,17 +68,24 @@
         output[mask] = yoffset + (amp / max_val) * Psp._psp_inner(xoff[mask], rise_tau, rise_power, decay_tau)
         
         if not np.all(np.isfinite(output)):
             raise ValueError("Parameters are invalid: xoffset=%f, yoffset=%f, rise_tau=%f, decay_tau=%f, amp=%f, rise_power=%f, isfinite(x)=%s" % (xoffset, yoffset, rise_tau, decay_tau, amp, rise_power, np.all(np.isfinite(x))))
         return output
             
     @staticmethod
-    @lru_cache(maxsize=4096)
     def _compute_rise_tau(rise_time, rise_power, decay_tau):
-        return scipy.optimize.fsolve(Psp._rise_time_from_tau, (rise_time,), (rise_time, rise_power, decay_tau))[0]
+        # rt1 = scipy.optimize.fsolve(Psp._rise_time_from_tau, (rise_time,), (rise_time, rise_power, decay_tau))[0]
+
+        rt_over_td = min(rise_time / (rise_power * decay_tau), 0.99999)            
+
+        # lambert W returns real solutions for k=0 and k=-1, but we don't necessarily know which is better..
+        denom = np.real(lambertw(-rt_over_td * np.exp(-rt_over_td), k=-1) + rt_over_td)
+
+        rt2 = - rise_time / denom
+        return rt2
 
     @staticmethod
     @numba_jit(nopython=True)
     def _rise_time_from_tau(rise_tau, rise_time, rise_power, decay_tau):
         return rise_tau * np.log(1 + (decay_tau * rise_power / rise_tau)) - rise_time
 
     @staticmethod
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/fitting/searchfit.py` & `neuroanalysis-0.0.2/neuroanalysis/fitting/searchfit.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/miesnwb.py` & `neuroanalysis-0.0.2/neuroanalysis/miesnwb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import print_function, division
 import sys
 from datetime import datetime
 from collections import OrderedDict
 import numpy as np
-import h5py
+from .util import h5py_wrapper
 
 from .data import Dataset, SyncRecording, PatchClampRecording, TSeries
 from .test_pulse import PatchClampTestPulse
 from . import stimuli
 
 
 class MiesNwb(Dataset):
@@ -198,15 +198,15 @@
         self.hdf.close()
         self._hdf = None
 
     def open(self):
         if self._hdf is not None:
             return
         try:
-            self._hdf = h5py.File(self.filename, 'r')
+            self._hdf = h5py_wrapper.File(self.filename, 'r')
         except Exception:
             print("Error opening: %s" % self.filename)
             raise
 
     def __enter__(self):
         self.open()
         return self
@@ -262,21 +262,21 @@
                     entry[f] = rec[i, :8]
                 entry['stim'] = {f:rec[self._notebook_keys[f], 8] for f in stim_fields}
                 self._tp_entries.append(entry)
         return self._tp_entries
 
 
 class MiesTSeries(TSeries):
-    def __init__(self, recording, chan):
+    def __init__(self, recording, chan, units=None):
         start = recording._meta['start_time']
         
         # Note: this is also available in meta()['Minimum Sampling interval'],
         # but that key is missing in some older NWB files.
         dt = recording.primary_hdf.attrs['IGORWaveScaling'][1,0] / 1000.
-        TSeries.__init__(self, recording=recording, channel_id=chan, dt=dt, start_time=start)
+        TSeries.__init__(self, recording=recording, channel_id=chan, dt=dt, start_time=start, units=units)
     
     @property
     def data(self):
         if self._data is None:
             rec = self.recording
             chan = self.channel_id
             if chan == 'primary':
@@ -337,28 +337,32 @@
         self.meta['holding_current'] = (
             None if nb['I-Clamp Holding Level'] is None
             else nb['I-Clamp Holding Level'] * 1e-12
         )   
         self._meta['notebook'] = nb
         if nb['Clamp Mode'] == 0:
             self._meta['clamp_mode'] = 'vc'
+            primary_units = 'A'
+            command_units = 'V'
         else:
             self._meta['clamp_mode'] = 'ic'
             self._meta['bridge_balance'] = (
                 0.0 if nb['Bridge Bal Enable'] == 0.0 or nb['Bridge Bal Value'] is None
                 else nb['Bridge Bal Value'] * 1e6
             )
+            primary_units = 'V'
+            command_units = 'A'
         self._meta['lpf_cutoff'] = nb['LPF Cutoff']
         offset = nb['Pipette Offset']  # sometimes the pipette offset recording can fail??
         self._meta['pipette_offset'] = None if offset is None else offset * 1e-3
         datetime = MiesNwb.igorpro_date(nb['TimeStamp'])
         self.meta['start_time'] = datetime
 
-        self._channels['primary'] = MiesTSeries(self, 'primary')
-        self._channels['command'] = MiesTSeries(self, 'command')
+        self._channels['primary'] = MiesTSeries(self, 'primary', units=primary_units)
+        self._channels['command'] = MiesTSeries(self, 'command', units=command_units)
 
     @property
     def stimulus(self):
         stim = self._meta.get('stimulus', None)
         if stim is None:
             stim = MiesStimulus(self)
             self._meta['stimulus'] = stim
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/neuronsim/components.py` & `neuroanalysis-0.0.2/neuroanalysis/neuronsim/components.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,27 +28,26 @@
         """
         raise NotImplementedError()
 
     @property
     def name(self):
         if self._name is None:
             # pick a name that is unique to the section we live in
-            
+
             # first collect all names
             names = []
             if self._section is None:
                 return None
-            for o in self._section.mechanisms:
-                if isinstance(o, Mechanism) and o._name is None:
-                    # skip to avoid recursion
-                    continue
-                names.append(o.name)
-                
+            names.extend(
+                o.name
+                for o in self._section.mechanisms
+                if not isinstance(o, Mechanism) or o._name is not None
+            )
             # iterate until we find an unused name
-            pfx = self._section.name + '.'
+            pfx = f'{self._section.name}.'
             name = pfx + self.type
             i = 1
             while name in names:
                 name = pfx + self.type + str(i)
                 i += 1
             self._name = name
         return self._name
@@ -140,15 +139,15 @@
     
     def __init__(self, radius=None, cap=10*pF, vm=-65*mV, **kwds):
         self.cap_bar = 1 * uF/cm**2
         if radius is None:
             self.cap = cap
             self.area = cap / self.cap_bar
         else:
-            self.area = 4 * 3.1415926 * radius**2
+            self.area = 4 / 3 * 3.1415926 * radius**2
             self.cap = self.area * self.cap_bar
         self.ek = -77*mV
         self.ena = 50*mV
         self.ecl = -70*mV
         init_state = OrderedDict([('V', vm)])
         SimObject.__init__(self, init_state, **kwds)
         self.dep_state_vars['I'] = self.current
@@ -158,33 +157,26 @@
         assert mech._section is None
         mech._section = self
         self.mechanisms.append(mech)
         self._sub_objs.append(mech)
         return mech
 
     def derivatives(self, state):
-        Im = 0
-        for mech in self.mechanisms:
-            if not mech.enabled:
-                continue
-            Im += mech.current(state)
-            
-        dv = Im / self.cap
-        return [dv]
+        Im = sum(mech.current(state) for mech in self.mechanisms if mech.enabled)
+        return [Im / self.cap]
     
     def current(self, state):
         """Return the current flowing across the membrane capacitance.
         """
         dv = self.derivatives(state)[0]
         return - self.cap * dv
 
     def conductance(self, state):
         """Return the total conductance of all channels in this section.
         
         This is for introspection; not used by the integrator.
         """
-        g = 0
-        for mech in self.mechanisms:
-            if not isinstance(mech, Channel) or not mech.enabled:
-                continue
-            g += mech.conductance(state)
-        return g
+        return sum(
+            mech.conductance(state)
+            for mech in self.mechanisms
+            if isinstance(mech, Channel) and mech.enabled
+        )
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/neuronsim/mechanisms.py` & `neuroanalysis-0.0.2/neuroanalysis/neuronsim/mechanisms.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 Simple neuron simulator for Python.
 Also simulates voltage clamp and current clamp with access resistance.
 
 Luke Campagnola 2015
 """
 
 from collections import OrderedDict
+
 import numpy as np
 import scipy.interpolate
-from ..units import *
+
 from .components import Mechanism, Channel
+from ..units import MOhm, us, ms, mS, pF, pA, mV, cm
 
 
 class PatchClamp(Mechanism):
     type = 'PatchClamp'
     
     def __init__(self, mode='ic', ra=2*MOhm, cpip=0.5*pF, **kwds):
         self.ra = ra
@@ -34,22 +36,20 @@
         """
         assert cmd.ndim == 1 and cmd.shape[0] > 0
         if len(self.cmd_queue) == 0:
             next_start = self.last_time + dt
         else:
             last_start, last_dt, last_cmd = self.cmd_queue[-1]
             next_start = last_start + len(last_cmd) * last_dt
-            
+
         if start is None:
             start = next_start
-        else:
-            if start < next_start:
-                raise ValueError('Cannot start next command before %f; asked for %f.' % 
-                                 (next_start, start))
-        
+        elif start < next_start:
+            raise ValueError(f'Cannot start next command before {next_start:f}; asked for {start:f}.')
+
         self.cmd_queue.append((start, dt, cmd))
         return start
     
     def queue_commands(self, cmds, dt):
         """Queue multiple commands for execution.
         """
         return [self.queue_command(c, dt) for c in cmds]
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/neuronsim/model_cell.py` & `neuroanalysis-0.0.2/neuroanalysis/neuronsim/model_cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from . import Sim, Section, Leak, LGKfast, LGKslow, LGNa, Noise, PatchClamp
 from ..data import TSeries, PatchClampRecording
-from ..units import um, mS, uV, mV, pA, cm, MOhm, ms
+from ..units import mS, uV, mV, pA, cm, MOhm, ms
 
 
 class ModelCell(object):
     """A simulated patch-clamped neuron for generating test data.
     """
     def __init__(self):
         self.sim = Sim()
@@ -19,15 +19,15 @@
         radius = (5e-10 / (4*np.pi)) ** 0.5
         self.soma = Section(name='soma', radius=radius)
         self.sim.add(self.soma)
 
         # Add channels to the membrane
         self.mechs = {
             'leak': Leak(gbar=1.0*mS/cm**2, erev=-75*mV),
-            'leak0': Leak(gbar=0, erev=0), # simulate dying cell
+            'leak0': Leak(gbar=0, erev=0),  # simulate dying cell
             'lgkfast': LGKfast(gbar=225*mS/cm**2),
             'lgkslow': LGKslow(gbar=0.225*mS/cm**2),
             'lgkna': LGNa(),
             'noise': Noise(),  # adds realism, but slows down the integrator a lot.
         }
         for m in self.mechs.values():
             self.soma.add(m)
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/neuronsim/sim.py` & `neuroanalysis-0.0.2/neuroanalysis/neuronsim/sim.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,272 +6,364 @@
 Luke Campagnola 2015
 github.com/campagnola/neurodemo
 """
 
 from collections import OrderedDict
 import numpy as np
 import scipy.integrate
-from ..units import us
+from ..units import us, ms
+
+
+class SimState(object):
+    """Contains the state of all diff. eq. variables in the simulation.
+
+    During simulation runs, this is used to carry information about all
+    variables at the current timepoint. After the simulation finishes, this is
+    used to carry all state variable data collected during the simulation.
+
+    Parameters
+    ==========
+        difeq_vars: list
+            Names of all diff. eq. state variables
+        dep_vars: dict
+            Name:function pairs for all dependent variables that may be computed
+        difeq_state: list
+            Initial values for all dif. eq. state variables
+        extra:
+            Extra name:value pairs that may be accessed from this object
+    """
+
+    def __init__(self, difeq_vars, dep_vars=None, difeq_state=None, integrator='odeint', **extra):
+        self.difeq_vars = difeq_vars
+        # record indexes of difeq vars for fast retrieval
+        self.indexes = dict([(k, i) for i, k in enumerate(difeq_vars)])
+
+        self.dep_vars = dep_vars
+        self.state = difeq_state
+
+        self.extra = extra
+        self.integrator = integrator
+
+    def set_state(self, difeq_state):
+        self.state = difeq_state
+
+    def __getitem__(self, key):
+        if isinstance(key, slice):
+            return self.get_slice(key)
+        # allow lookup by (object, var)
+        if isinstance(key, tuple):
+            key = f"{key[0].name}.{key[1]}"
+        try:
+            # try this first for speed
+            return self.state[self.indexes[key]]
+        except KeyError:
+            if key in self.dep_vars:
+                return self.dep_vars[key](self)
+            else:
+                return self.extra[key]
+
+    def keys(self):
+        return self.difeq_vars + list(self.extra.keys())
+        # return list(self.indexes.keys()) + list(self.dep_vars.keys()) + list(self.extra.keys())
+
+    def __contains__(self, key):
+        # allow lookup by (object, var)
+        if isinstance(key, tuple):
+            key = f"{key[0].name}.{key[1]}"
+        return key in self.indexes or key in self.dep_vars or key in self.extra
+
+    def __str__(self):
+        rep = f"SimState {id(self)}:\n"
+        if self.state is not None:
+            for i, k in enumerate(self.difeq_vars):
+                rep += f"  {k} = {self.state[i][-1]}\n"
+        else:
+            rep += "  (no state)\n"
+        return rep
+
+    def get_final_state(self):
+        """Return a dictionary of all diff. eq. state variables and dependent
+        variables for all objects in the simulation.
+        """
+        return self.get_state_at_index(-1)
+
+    def get_state_at_time(self, t):
+        index = np.searchsorted(self['t'], t)
+        return self.get_state_at_index(index)
+
+    def get_state_at_index(self, index):
+        s = self.copy()
+        clip = not np.isscalar(self["t"])
+        if clip:
+            # only get results for the last timepoint
+            s.set_state(self.state[:, index])
+
+        state = {}
+        for k in self.difeq_vars:
+            state[k] = s[k]
+        for k in self.dep_vars:
+            state[k] = s[k]
+        for k, v in self.extra.items():
+            if clip:
+                state[k] = v[index]
+            else:
+                state[k] = v
+
+        return state
+
+    def get_slice(self, sl):
+        kwds = {'difeq_state': self.state[:, sl]}
+        for k, v in self.extra.items():
+            kwds[k] = v[sl]
+        return self.copy(**kwds)
+
+    def copy(self, **kwds):
+        default_kwds = {
+            'difeq_vars': self.difeq_vars,
+            'dep_vars': self.dep_vars,
+            'difeq_state': self.state,
+            'integrator': self.integrator,
+        }
+        default_kwds.update(self.extra)
+        default_kwds.update(kwds)
+        return SimState(**default_kwds)
 
 
 class Sim(object):
     """Simulator for a collection of objects that derive from SimObject
     """
-    def __init__(self, objects=None, temp=37.0, dt=10*us):
+    def __init__(self, objects=None, temp=37.0, dt=10*us, integrator:str='solve_ivp'):
         self._objects = []
         self._all_objs = None
         self._time = 0.0
         self.temp = temp
         self.dt = dt
-        self.odeint_args = {
-            'h0': 1*us,
-            'hmax': 100*us,
-            'rtol': 1e-6, 
-            'atol': 1e-6, 
-            'full_output': 1,
-        }
+        self.integrator = integrator
+        self._simstate = None
         if objects is not None:
             for obj in objects:
                 self.add(obj)
 
+    def set_integrator(self, integrator:str):
+        if integrator not in {"odeint", "solve_ivp"}:
+            raise ValueError(f"Unknown integrator: {integrator}")
+        self.integrator = integrator
+
+    def change_dt(self, newdt:float=100e-6):
+        newdt = np.clip(newdt, 5*us, 1*ms)
+        self.dt = newdt
+    
     def add(self, obj):
         assert obj._sim is None
         obj._sim = self
         self._objects.append(obj)
         return obj
 
     def all_objects(self):
         """Ordered dictionary of all objects to be simulated, keyed by their names.
         """
         if self._all_objs is None:
             objs = OrderedDict()
             for o in self._objects:
                 if not o.enabled:
                     continue
-                for k,v in o.all_objects().items():
+                for k, v in o.all_objects().items():
                     if k in objs:
-                        raise NameError('Multiple objects with same name "%s": %s, %s' % (k, objs[k], v))
+                        raise NameError(f'Multiple objects with same name "{k}": {objs[k]}, {v}')
                     objs[k] = v
             self._all_objs = objs
         return self._all_objs
     
     @property
     def time(self):
         return self._time
 
-    def run(self, samples=1000, **kwds):
+    def run(self, samples:int=1000, **kwds) -> SimState:
         """Run the simulation until a number of *samples* have been acquired.
-        
+
         Extra keyword arguments are passed to `scipy.integrate.odeint()`.
         """
-        opts = self.odeint_args.copy()
-        opts.update(kwds)
-        
+        # print("Integrator: ", self.integrator)
         # reset all_objs cache in case some part of the sim has changed
         self._all_objs = None
         all_objs = self.all_objects().values()
-        
+
         # check that there is something to simulate
         if len(all_objs) == 0:
             raise RuntimeError("No objects added to simulation.")
-        
+
         # Collect / prepare state variables for integration
         init_state = []
         difeq_vars = []
         dep_vars = {}
         for o in all_objs:
-            pfx = o.name + '.'
-            for k,v in o.difeq_state().items():
+            pfx = f'{o.name}.'
+            for k, v in o.difeq_state().items():
                 difeq_vars.append(pfx + k)
                 init_state.append(v)
-            for k,v in o.dep_state_vars.items():
+            for k, v in o.dep_state_vars.items():
                 dep_vars[pfx + k] = v
         self._simstate = SimState(difeq_vars, dep_vars)
         t = np.arange(0, samples) * self.dt + self._time
 
-        # Run the simulation
-        result, info = scipy.integrate.odeint(self.derivatives, init_state, t, **opts)
-        
-        # Update current state variables
-        p = 0
-        for o in all_objs:
-            nvar = len(o.difeq_state())
-            o.update_state(result[-1, p:p+nvar])
-            p += nvar
-            
-        self._last_run_time = t
-        return SimState(difeq_vars, dep_vars, result.T, t=t)
+        opts = {"rtol": 1e-6, "atol": 1e-8, "hmax": 5e-4, "full_output": 1}
+        opts.update(kwds)
+
+        if self.integrator == 'odeint':
+            # Run the simulation
+            result, info = scipy.integrate.odeint(self.derivatives, init_state, t, tfirst=True, **opts)
+
+            # Update current state variables
+            p = 0
+            for o in all_objs:
+                nvar = len(o.difeq_state())
+                o.update_state(result[-1, p : p + nvar])
+                p += nvar
+            self._time = t[-1]
+            # print(f"   {self.integrator:s}  final state = {str(result.T[:, -1]):s}")
+            # print("   start, finished at : ", t[0],t[-1])
+            # print("   np.min(result.T): ", np.min(result.T), np.max(result.T))
+            return SimState(difeq_vars, dep_vars, result.T, integrator=self.integrator, t=t)
+
+        elif self.integrator == 'solve_ivp':
+            """Notes:
+            Different integrators were tried. 
+            LSODA works ok; RK's seem to stall on AP. 
+            Radau and BDF are very fast, but take some large steps, so the calculation of where the 
+            pulse array is in the derivative via get_cmd are not always correct -
+            the algorithm might step a long time into the future, invalidating all the
+            commands in the queue, which are removed. Thus, only the first cmd
+            is executed.
+            Probably should not pop the queue in get_cmd until we are certain at THIS
+            level (or maybe in runner?) that the trigger arrays are actually finished. 
+            """
+            # in future we will need to implement this instead: 
+            result = scipy.integrate.solve_ivp(
+                self.derivatives,
+                t_span=(t[0], t[-1]),
+                t_eval=t,
+                y0=init_state,
+                method="LSODA",  # runs ok with LSODA
+
+                dense_output=False,
+                # args=dep_vars,
+                rtol = opts['rtol'], #**opts,
+                atol = opts['atol'],
+                max_step = opts['hmax'],
+            )
+            # Update current state variables
+            p = 0
+            for o in all_objs:
+                nvar = len(o.difeq_state())
+                # print("solve ivp state: ", p, nvar, result.y[p:p+nvar, -1])
+                o.update_state(result.y[p:p+nvar, -1])
+                p += nvar
+            self._time = t[-1]
+            # print(f"\n   {self.integrator:s}  {str(result.y[:, -1]):s}")
+            # print("   start, finished at : ", t[0],t[-1])
+            # print("    np.min(result.y): ", np.min(result.y), np.max(result.y))
 
-    def derivatives(self, state, t):
+            return SimState(difeq_vars, dep_vars, result.y, integrator=self.integrator, t=t)
+
+    def derivatives(self, t, state):
         objs = self.all_objects().values()
-        self._simstate.state = state
+
+        # bug: the integrators may trash their outputs later;
+        # copy them before that can happen
+        self._simstate.state = state.copy()
+
         self._simstate.extra['t'] = t
-        
-        # Record the time of the last simulated sample. Note that this is NOT
-        # the same as the last _requested_ sample; the integrator may go farther
-        # depending on its time step
-        self._time = t
-        
         d = []
         for o in objs:
             d.extend(o.derivatives(self._simstate))
-            
         return d
 
     @property
     def last_state(self):
         """Return the last values of all state variables in a SimState object.
         """
         return self._simstate
-        
     
-class SimState(object):
-    """Contains the state of all diff. eq. variables in the simulation.
-    
-    During simulation runs, this is used to carry information about all
-    variables at the current timepoint. After the simulation finishes, this is
-    used to carry all state variable data collected during the simulation.
-    
-    Parameters
-    ==========
-        difeq_vars: list
-            Names of all diff. eq. state variables
-        dep_vars: dict
-            Name:function pairs for all dependent variables that may be computed
-        difeq_state: list
-            Initial values for all dif. eq. state variables
-        extra:
-            Extra name:value pairs that may be accessed from this object
-    """
-    def __init__(self, difeq_vars, dep_vars=None, difeq_state=None, **extra):
-        self.difeq_vars = difeq_vars
-        # record indexes of difeq vars for fast retrieval
-        self.indexes = dict([(k, i) for i,k in enumerate(difeq_vars)])
-            
-        self.dep_vars = dep_vars
-        self.state = difeq_state
-        self.extra = extra
-        
-    def set_state(self, difeq_state):
-        self.state = difeq_state
-        
-    def __getitem__(self, key):
-        # allow lookup by (object, var)
-        if isinstance(key, tuple):
-            key = key[0].name + '.' + key[1]
-        try:
-            # try this first for speed
-            return self.state[self.indexes[key]]
-        except KeyError:
-            if key in self.dep_vars:
-                return self.dep_vars[key](self)
-            else:
-                return self.extra[key]
-
-    def keys(self):
-        return self.difeq_vars + list(self.extra.keys())
-
-    def __repr__(self):
-        rep = 'SimState:\n'
-        for i,k in enumerate(self.difeq_vars):
-            rep += '  %s = %s\n' % (k, self.state[i])
-        return rep
-
-    def get_final_state(self):
-        """Return a dictionary of all diff. eq. state variables and dependent
-        variables for all objects in the simulation.
+    def state(self):
+        """Return dictionary of all dependent and independent state
+        variables.
         """
         state = {}
-        s = self.copy()
-        clip = not np.isscalar(self['t'])
-        if clip:
-            # only get results for the last timepoint
-            s.set_state(self.state[:, -1])
-        
-        for k in self.difeq_vars:
-            state[k] = s[k]
-        for k in self.dep_vars:
-            state[k] = s[k]
-        for k,v in self.extra.items():
-            if clip:
-                state[k] = v[-1]
-            else:
+        for o in self.all_objects():
+            for k, v in o.state(self._simstate).items():
                 state[k] = v
-        
         return state
 
-    def copy(self):
-        return SimState(self.difeq_vars, self.dep_vars, self.state, **self.extra)
-            
 
 class SimObject(object):
     """
     Base class for objects that participate in integration by providing a set
     of state variables and their derivatives.
     """
+
     instance_count = 0
-    
+
     def __init__(self, init_state, name=None):
         self._sim = None
         if name is None:
             i = self.instance_count
             type(self).instance_count = i + 1
             if i == 0:
                 name = self.type
             else:
-                name = self.type + '%d' % i
+                name = self.type + "%d" % i
         self._name = name
         self.enabled = True
         self._init_state = init_state.copy()  # in case we want to reset
         self._current_state = init_state.copy()
         self._sub_objs = []
         self.records = []
         self._rec_dtype = [(sv, float) for sv in init_state.keys()]
-        
+
         # maps name:function for computing state vars that can be computed from
-        # a SimState instance.   
+        # a SimState instance.
         self.dep_state_vars = {}
 
     @property
     def name(self):
         return self._name
-        
+
     def all_objects(self):
         """SimObjects are organized in a hierarchy. This method returns an ordered
         dictionary of all enabled SimObjects in this branch of the hierarchy, beginning
         with self.
         """
         objs = OrderedDict()
         objs[self.name] = self
         for o in self._sub_objs:
             if not o.enabled:
                 continue
             objs.update(o.all_objects())
         return objs
-    
+
     def difeq_state(self):
         """An ordered dictionary of all variables required to solve the
         diff. eq. for this object.
         """
         return self._current_state
 
     def update_state(self, result):
         """Update diffeq state variables with their last simulated values.
         These will be used to initialize the solver when the next simulation
         begins.
         """
-        for i,k in enumerate(self._current_state.keys()):
+        for i, k in enumerate(self._current_state.keys()):
             self._current_state[k] = result[i]
 
     def derivatives(self, state):
         """Return derivatives of all state variables.
-        
+
         Must be reimplemented in subclasses. This is used by the ODE solver
         to integrate during the simulation; should be as fast as possible.
         """
         raise NotImplementedError()
 
     @property
     def sim(self):
-        """The Sim instance in which this object is being used.
-        """
+        """The Sim instance in which this object is being used."""
         return self._sim
+
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/spike_detection.py` & `neuroanalysis-0.0.2/neuroanalysis/spike_detection.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/stats.py` & `neuroanalysis-0.0.2/neuroanalysis/stats.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/stimuli.py` & `neuroanalysis-0.0.2/neuroanalysis/stimuli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf8
-from __future__ import division, print_function
 from collections import OrderedDict
 import numpy as np
 from .util.custom_weakref import WeakRef
 from .data import TSeries
+from .fitting import psp
 
 
 def load_stimulus(state):
     """Re-create a Stimulus structure from a previously saved state.
 
     States are generated using Stimulus.save().
     """
@@ -368,15 +368,15 @@
     def mask(self, **kwds):
         trace = Stimulus.mask(self, **kwds)
         start = self.global_start_time
         trace.time_slice(start, start+self.duration, index_mode=kwds.get('index_mode')).data[:] = True
         return trace
 
 
-def find_square_pulses(trace, baseline=None):
+def find_square_pulses(trace, baseline=None) -> list[SquarePulse]:
     """Return a list of SquarePulse instances describing square pulses found
     in the stimulus.
     
     A pulse is defined as any contiguous region of the stimulus waveform
     that has a constant value other than the baseline. If no baseline is
     specified, then the first sample in the stimulus is used.
     
@@ -402,14 +402,15 @@
             stop = changes[i+1] if (i+1 < len(changes)) else len(trace)
             t_start = trace.time_at(start)
             duration = (stop - start) * trace.dt
             pulses.append(SquarePulse(start_time=t_start, duration=duration, amplitude=amp, units=trace.units))
             pulses[-1].pulse_number = i
     return pulses
 
+
 def find_noisy_square_pulses(trace, baseline=None, std_threshold=5.0, min_duration=0, min_amplitude=0):
     """Return a list of SquarePulse instances describing square pulses found
     in the given trace.
     
     A pulse is defined as any contiguous region of the stimulus waveform
     that has a value outside the amp_threshold or std_threshold from the 
     baseline. If no baseline is specified, then the first 200 samples in the 
@@ -780,7 +781,66 @@
 
     def mask(self, **kwds):
         trace = Stimulus.mask(self, **kwds)
         start = self.global_start_time
         chunk = trace.time_slice(start, start+self.duration, index_mode=kwds.get('index_mode'))
         chunk.data[:] = True
         return trace
+
+
+class Psp(Stimulus):
+    """A PSP- or PSC-shaped stimulus.
+
+    This shape is the product of rising and decaying exponentials. See ``neuroanalysis.fitting.psp.Psp``.
+
+    Parameters
+    ----------
+    start_time : float
+        The starting time (s) of the stimulus.
+    rise_time : float
+        Time (s) from stimulus start until the peak of the PSP shape.
+    decay_tau : float
+        Exponential decay time constant (s).
+    amplitude : float
+        The peak amplitude of the PSP shape.
+    rise_power : float
+        Exponent modifying the rising exponential (default is 2; larger values yield a slower initial activation, 1 yields instantaneous activation).
+    description : str
+        Optional string describing the stimulus.
+    units : str | None
+        Optional string describing the units of values in the stimulus.
+
+    """
+    _attributes = Stimulus._attributes + ['rise_time', 'decay_tau', 'amplitude', 'rise_power']
+
+    def __init__(self, start_time, rise_time, decay_tau, amplitude, rise_power=2, description="frequency chirp", units=None, parent=None):
+        self.rise_time = rise_time
+        self.decay_tau = decay_tau
+        self.amplitude = amplitude
+        self.rise_power = rise_power
+        Stimulus.__init__(self, description=description, start_time=start_time, parent=parent, units=units)
+
+    @property
+    def duration(self):
+        return 15 * max(self.rise_time, self.decay_tau)
+
+    def eval(self, **kwds):
+        trace = Stimulus.eval(self, **kwds)
+        start = self.global_start_time
+        chunk = trace.time_slice(start, start + self.duration, index_mode=kwds.get('index_mode'))
+        chunk.data[:] += psp.Psp.psp_func(
+            x=chunk.time_values,
+            xoffset=start,
+            yoffset=0,
+            rise_time=self.rise_time,
+            decay_tau=self.decay_tau,
+            amp=self.amplitude,
+            rise_power=self.rise_power,
+        )
+        return trace
+
+    def mask(self, **kwds):
+        trace = Stimulus.mask(self, **kwds)
+        start = self.global_start_time
+        chunk = trace.time_slice(start, start+self.duration, index_mode=kwds.get('index_mode'))
+        chunk.data[:] = True
+        return trace
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/synaptic_release.py` & `neuroanalysis-0.0.2/neuroanalysis/synaptic_release.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/test_pulse.py` & `neuroanalysis-0.0.2/neuroanalysis/test_pulse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 import numpy as np
 
 from .data import PatchClampRecording, TSeries
-from .fitting import Exp
+from .fitting.exp import exp_fit, fit_double_exp_decay
 from .stimuli import find_square_pulses
 
 
 class PatchClampTestPulse(PatchClampRecording):
     """A PatchClampRecording that contains a subthreshold, square pulse stimulus.
     """
-    def __init__(self, rec, indices=None):
-        self._parent_recording = rec
-        
+    def __init__(self, rec: PatchClampRecording, indices=None):
         if indices is None:
             indices = (0, len(rec['primary']))
         self._indices = indices
         start, stop = indices
-        
+
         pri = rec['primary'][start:stop]
         cmd = rec['command'][start:stop]
-        
+
         # find pulse
-        pulses = find_square_pulses(cmd)        
+        pulses = find_square_pulses(cmd)
         if len(pulses) == 0:
-            raise ValueError("Could not find square pulse in command waveform.")
+            raise ValueError("Could not find square pulse in command waveform. Consider using `indices`.")
         elif len(pulses) > 1:
-            raise ValueError("Found multiple square pulse in command waveform.")
+            raise ValueError("Found multiple square pulse in command waveform. Consider using `indices`.")
         pulse = pulses[0]
         pulse.description = 'test pulse'
-        
-        PatchClampRecording.__init__(self,
-            device_type=rec.device_type, 
+        super().__init__(
+            recording=rec,
+            device_type=rec.device_type,
             device_id=rec.device_id,
             start_time=rec.start_time,
-            channels={'primary': pri, 'command': cmd}
-        )        
-        self._meta['stimulus'] = pulse
-                           
-        for k in ['clamp_mode', 'holding_potential', 'holding_current', 'bridge_balance',
-                  'lpf_cutoff', 'pipette_offset']:
-            self._meta[k] = rec._meta[k]
-            
+            channels={'primary': pri, 'command': cmd},
+            stimulus=pulse,
+            clamp_mode=rec.clamp_mode,
+            holding_potential=rec._meta['holding_potential'],
+            holding_current=rec._meta['holding_current'],
+            bridge_balance=rec._meta['bridge_balance'],
+            lpf_cutoff=rec._meta['lpf_cutoff'],
+            pipette_offset=rec._meta['pipette_offset'],
+        )
         self._analysis = None
-        
+        # expose these for display and debugging
+        self.main_fit_result = None
+        self.main_fit_trace = None
+        self.fit_result_with_transient = None
+        self.fit_trace_with_transient = None
+        self.initial_double_fit_trace = None
+
     @property
     def indices(self):
         return self._indices
-        
+
     @property
     def access_resistance(self):
         """The access resistance measured from this test pulse.
         
         Includes the bridge balance resistance if the recording was made in
         current clamp mode.
         """
@@ -89,152 +94,111 @@
  
     @property
     def analysis(self):
         if self._analysis is None:
             self._analyze()
         return self._analysis
  
-    @property
-    def parent(self):
-        """The recording in which this test pulse is embedded.
-        """
-        return self._parent_recording
-
     def _analyze(self):
         # adapted from ACQ4
         
-        meta = self.meta
         pulse_amp = self.stimulus.amplitude
         clamp_mode = self.clamp_mode
         
         data = self['primary']
-        pulse_start = data.index_at(self.stimulus.start_time)
-        pulse_stop = data.index_at(self.stimulus.start_time + self.stimulus.duration)
+        
+        pulse_start = data.t0 + self.stimulus.start_time
+        pulse_stop = pulse_start + self.stimulus.duration
         dt = data.dt
         
         # Extract specific time segments
-        nudge = int(50e-6 / dt)
-        base = data[:pulse_start-nudge]
-        pulse = data[pulse_start+nudge:pulse_stop-nudge]
-        pulse_end = pulse[int(len(pulse)*2./3.):]  # last 1/3 of pulse response 
-        end = data[pulse_stop+nudge:]
-        
-        # Exponential fit
-
-        # predictions
+        padding = 50e-6
+        base = data.time_slice(None, pulse_start-padding)
+        pulse = data.time_slice(pulse_start+padding, pulse_stop-padding)
         base_median = np.median(base.data)
-        access_r = 10e6
-        input_r = 200e6
-        if clamp_mode == 'vc':
-            ari = pulse_amp / access_r
-            iri = pulse_amp / input_r
-            params = {
-                'xoffset': (pulse.t0, 'fixed'),
-                'yoffset': base_median + iri,
-                'amp': ari - iri,
-                'tau': (1e-3, 0.1e-3, 50e-3),
-            }
-        else:
-            bridge = meta['bridge_balance']
-            arv = pulse_amp * (access_r - bridge)
-            irv = pulse_amp * input_r
-            params = {
-                'xoffset': pulse.t0,
-                'yoffset': base_median+arv+irv,
-                'amp': -irv,
-                'tau': (10e-3, 1e-3, 50e-3),
-            }
-            
-        fit_kws = {'tol': 1e-4}
-        model = Exp()
-        
-        # ignore initial transients when fitting
-        fit_region = pulse.time_slice(pulse.t0 + 150e-6, None)
-        
-        result = model.fit(fit_region.data, x=fit_region.time_values, fit_kws=fit_kws, params=params)
-        fit = result.best_values
-        err = model.nrmse(result)
-        
-        self.fit_trace = TSeries(result.eval(), time_values=fit_region.time_values)
-        
-        ### fit again using shorter data
-        ### this should help to avoid fitting against h-currents
-        #tau4 = fit1[0][2]*10
-        #t0 = pulse.xvals('Time')[0]
-        #shortPulse = pulse['Time': t0:t0+tau4]
-        #if shortPulse.shape[0] > 10:  ## but only if we can get enough samples from this
-            #tVals2 = shortPulse.xvals('Time')-params['delayTime']
-            #fit1 = scipy.optimize.leastsq(
-                #lambda v, t, y: y - expFn(v, t), pred1, 
-                #args=(tVals2, shortPulse['primary'].view(np.ndarray) - baseMean),
-                #maxfev=200, full_output=1)
+        prepulse_median = np.median(data.time_slice(pulse_start-5e-3, pulse_start).data)
 
-        ## Handle analysis differently depending on clamp mode
+        # start by fitting the exponential decay from the post-pipette capacitance, ignoring initial transients
+        main_fit_region = pulse.time_slice(pulse.t0 + 150e-6, None)
+        self.main_fit_result = exp_fit(main_fit_region)
+        main_fit_yoffset, main_fit_amp, main_fit_tau = self.main_fit_result['fit']
+        self.main_fit_trace = TSeries(self.main_fit_result['model'](pulse.time_values), time_values=pulse.time_values)
+
+        # now fit with the initial transients included as an additional exponential decay
+        try:
+            self.fit_result_with_transient = fit_double_exp_decay(
+                data, pulse, base_median, pulse_start, self.main_fit_result['model'])
+            transient_yoffset = self.fit_result_with_transient['fit'][0]
+
+            self.fit_trace_with_transient = TSeries(
+                self.fit_result_with_transient['model'](pulse.time_values), time_values=pulse.time_values)
+            self.initial_double_fit_trace = TSeries(
+                self.fit_result_with_transient['guessed_model'](pulse.time_values), time_values=pulse.time_values)
+        except ValueError:
+            transient_yoffset = self.main_fit_result['model'](pulse.t0)
+
+        # Handle analysis differently depending on clamp mode
         if clamp_mode == 'vc':
-            hp = self.meta['holding_potential']
-            if hp is not None:
-                # we can only report base voltage if metadata includes holding potential
-                base_v = self['command'].data[0] + hp
-            else:
-                base_v = None
+            base_v = self._meta.get('holding_potential', self['command'].data[0])
             base_i = base_median
             
-            input_step = fit['yoffset'] - base_i
+            input_step = main_fit_yoffset - base_i
             
             peak_rgn = pulse.time_slice(pulse.t0, pulse.t0 + 1e-3)
             if pulse_amp >= 0:
                 input_step = max(1e-16, input_step)
                 access_step = peak_rgn.data.max() - base_i
                 access_step = max(1e-16, access_step)
             else:
                 input_step = min(-1e-16, input_step)
                 access_step = peak_rgn.data.min() - base_i
                 access_step = min(-1e-16, access_step)
-            
+
             access_r = pulse_amp / access_step
             input_r = pulse_amp / input_step
-            
-            # No capacitance in VC mode yet; the methods
-            # we've tried don't work very well.
-            tau = None
-            cap = None
-        
-        else:
+            cap = main_fit_tau * (1 / access_r + 1 / input_r)
+
+        else:  # IC mode
             base_v = base_median
-            hc = self.meta['holding_current']
-            if hc is not None:
-                # we can only report base current if metadata includes holding current
-                base_i = self['command'].data[0] + hc
-            else:
-                base_i = None
-            y0 = result.eval(x=pulse.t0)
+            base_i = self._meta.get('holding_current', self['command'].data[0])
+            # y0 = self.fit_result['model'](pulse_start)
+            y0 = transient_yoffset
             
             if pulse_amp >= 0:
-                v_step = max(1e-5, fit['yoffset'] - y0)
+                v_step = max(1e-5, main_fit_yoffset - y0)
             else:
-                v_step = min(-1e-5, fit['yoffset'] - y0)
+                v_step = min(-1e-5, main_fit_yoffset - y0)
                 
             if pulse_amp == 0:
                 pulse_amp = 1e-14
                 
             input_r = (v_step / pulse_amp)
-            access_r = ((y0 - base_median) / pulse_amp) + bridge
-            tau = fit['tau']
-            cap = tau / input_r
+            access_r = ((y0 - prepulse_median) / pulse_amp) + self.meta['bridge_balance']
+            cap = main_fit_tau / input_r
 
         self._analysis = {
+            'steady_state_resistance': input_r + access_r,
             'input_resistance': input_r,
             'access_resistance': access_r,
             'capacitance': cap,
-            'time_constant': tau,
+            'time_constant': main_fit_tau,
+            'fit_yoffset': main_fit_yoffset,
+            'fit_xoffset': pulse.t0,
+            'fit_amplitude': main_fit_amp,
             'baseline_potential': base_v,
             'baseline_current': base_i,
         }
-        self._fit_result = result
-    
+
+    @property
+    def plot_units(self):
+        return 'A' if self.clamp_mode == 'vc' else 'V'
+
+    @property
+    def plot_title(self):
+        return 'pipette potential' if self.clamp_mode == 'vc' else 'pipette current'
+
     def plot(self):
-        self.analysis
+        assert self.analysis is not None
         import pyqtgraph as pg
-        name, units = ('pipette potential', 'V') if self.clamp_mode == 'ic' else ('pipette current', 'A')
-        plt = pg.plot(labels={'left': (name, units), 'bottom': ('time', 's')})
+        plt = pg.plot(labels={'left': (self.plot_title, self.plot_units), 'bottom': ('time', 's')})
         plt.plot(self['primary'].time_values, self['primary'].data)
-        plt.plot(self.fit_trace.time_values, self.fit_trace.data, pen='b')
+        plt.plot(self.fit_trace_with_transient.time_values, self.fit_trace_with_transient.data, pen='b')
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/baseline.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/baseline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pyqtgraph as pg
-from pyqtgraph.Qt import QtGui, QtCore
+from pyqtgraph.Qt import QtWidgets, QtCore
 import pyqtgraph.parametertree as pt
 
 from ..baseline import mode_detrend
 
 
 class BaselineRemover(QtCore.QObject):
     """Removes baseline from signal.
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/cell_selector.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/cell_selector.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/event_detection.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/event_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pyqtgraph as pg
-from pyqtgraph.Qt import QtGui, QtCore
+from pyqtgraph.Qt import QtWidgets, QtCore
 import pyqtgraph.parametertree as pt
 import numpy as np
 import scipy.ndimage as ndi
 
 from ..event_detection import threshold_events, exp_deconvolve
 from ..baseline import float_mode
 from .filter import SignalFilter
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/filter.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pyqtgraph as pg
-from pyqtgraph.Qt import QtGui, QtCore
+from pyqtgraph.Qt import QtWidgets, QtCore
 import pyqtgraph.parametertree as pt
 from scipy.ndimage import gaussian_filter
 
 from ..filter import remove_artifacts, bessel_filter
 
 
 class SignalFilter(QtCore.QObject):
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/fitting.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/fitting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from collections import OrderedDict
 import numpy as np
 import scipy.stats
-from pyqtgraph.Qt import QtGui, QtCore
+from pyqtgraph.Qt import QtWidgets, QtCore
 import pyqtgraph as pg
-import pyqtgraph.parametertree
 import lmfit.minimizer 
-import sys
 
 
-class FitExplorer(QtGui.QWidget):
+class FitExplorer(QtWidgets.QWidget):
     def __init__(self, fit=None, model=None, data=None, args=None):
-        QtGui.QWidget.__init__(self)
+        QtWidgets.QWidget.__init__(self)
         self.model = model if model is not None else fit.model
         self.args = args
         self.data = data
         self.fit = None
         
-        self.layout = QtGui.QGridLayout()
+        self.layout = QtWidgets.QGridLayout()
         self.setLayout(self.layout)
-        self.splitter = QtGui.QSplitter(QtCore.Qt.Horizontal)
+        self.splitter = QtWidgets.QSplitter(QtCore.Qt.Horizontal)
         self.layout.addWidget(self.splitter)
         self.ptree = pg.parametertree.ParameterTree(showHeader=False)
         self.splitter.addWidget(self.ptree)
         self.plot = pg.PlotWidget()
         self.splitter.addWidget(self.plot)
         
         self.params = pg.parametertree.Parameter.create(name='param_root', type='group',
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/nwb_viewer/analyzer_view.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/nwb_viewer/analyzer_view.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pyqtgraph as pg
-from pyqtgraph.Qt import QtGui, QtCore
+from pyqtgraph.Qt import QtWidgets, QtCore
 from ..plot_grid import PlotGrid
 
 
-class AnalyzerView(QtGui.QWidget):
+class AnalyzerView(QtWidgets.QWidget):
     """A sweep analyzer of unspecified function.
     """
     def __init__(self, parent=None):
         self.sweeps = []
 
-        QtGui.QWidget.__init__(self, parent)
+        QtWidgets.QWidget.__init__(self, parent)
 
-        self.layout = QtGui.QGridLayout()
+        self.layout = QtWidgets.QGridLayout()
         self.setLayout(self.layout)
         self.layout.setContentsMargins(0, 0, 0, 0)
 
         self.plots = PlotGrid(parent=self)
         self.layout.addWidget(self.plots, 0, 0)
 
         self.params = pg.parametertree.Parameter(name='params', type='group', children=[
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/nwb_viewer/sweep_view.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/nwb_viewer/sweep_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 from scipy.ndimage import gaussian_filter
 import pyqtgraph as pg
 import pyqtgraph.reload
-from pyqtgraph.Qt import QtGui, QtCore
+from pyqtgraph.Qt import QtWidgets, QtCore
 from ..plot_grid import PlotGrid
 from ...miesnwb import MiesNwb
 
 
-class SweepView(QtGui.QWidget):
+class SweepView(QtWidgets.QWidget):
     def __init__(self, parent=None):
         self.sweeps = []
         self.chans = None
 
-        QtGui.QWidget.__init__(self, parent)
+        QtWidgets.QWidget.__init__(self, parent)
 
-        self.layout = QtGui.QGridLayout()
+        self.layout = QtWidgets.QGridLayout()
         self.setLayout(self.layout)
         self.layout.setContentsMargins(0, 0, 0, 0)
 
         self.plots = PlotGrid(parent=self)
         self.layout.addWidget(self.plots, 0, 0)
 
         self.params = pg.parametertree.Parameter(name='params', type='group', children=[
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/nwb_viewer/viewer.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/nwb_viewer/viewer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import pyqtgraph as pg
-from pyqtgraph.Qt import QtGui, QtCore
+from pyqtgraph.Qt import QtWidgets, QtCore
 from neuroanalysis.miesnwb import MiesNwb
 from ..signal import SignalBlock
 
 from .sweep_view import SweepView
 from .analyzer_view import AnalyzerView
 from ...util.merge_lists import merge_lists
 
 
-class MiesNwbExplorer(QtGui.QSplitter):
+class MiesNwbExplorer(QtWidgets.QSplitter):
     """Widget for listing and selecting recordings in a MIES-generated NWB file.
     """
     selection_changed = QtCore.Signal(object)
     channels_changed = QtCore.Signal(object)
     check_state_changed = QtCore.Signal(object)
 
     def __init__(self, nwb=None):
-        QtGui.QSplitter.__init__(self)
+        QtWidgets.QSplitter.__init__(self)
         self.setOrientation(QtCore.Qt.Vertical)
 
         self._nwb = None
         self._channel_selection = {}
 
-        self._sel_box = QtGui.QWidget()
-        self._sel_box_layout = QtGui.QHBoxLayout()
+        self._sel_box = QtWidgets.QWidget()
+        self._sel_box_layout = QtWidgets.QHBoxLayout()
         self._sel_box_layout.setContentsMargins(0, 0, 0, 0)
         self._sel_box.setLayout(self._sel_box_layout)
         self.addWidget(self._sel_box)
-        self.sweep_tree = QtGui.QTreeWidget()
+        self.sweep_tree = QtWidgets.QTreeWidget()
         columns = ['ID', 'Stim Name', 'Clamp Mode', 'Holding V', 'Holding I']
         self.sweep_tree.setColumnCount(len(columns))
         self.sweep_tree.setHeaderLabels(columns)
-        self.sweep_tree.setSelectionMode(QtGui.QAbstractItemView.ExtendedSelection)
+        self.sweep_tree.setSelectionMode(QtWidgets.QAbstractItemView.ExtendedSelection)
         self._sel_box_layout.addWidget(self.sweep_tree)
         
-        self.channel_list = QtGui.QListWidget()
+        self.channel_list = QtWidgets.QListWidget()
         self.channel_list.setMaximumWidth(50)
         self._sel_box_layout.addWidget(self.channel_list)
         self.channel_list.itemChanged.connect(self._channel_list_changed)
 
-        self.meta_tree = QtGui.QTreeWidget()
+        self.meta_tree = QtWidgets.QTreeWidget()
         self.addWidget(self.meta_tree)
 
         self.set_nwb(nwb)
 
         self.sweep_tree.itemSelectionChanged.connect(self._selection_changed)
         self.sweep_tree.itemChanged.connect(self._tree_item_changed)
 
@@ -84,20 +84,20 @@
 
                 hc = rec.holding_current
                 if hc is not None:
                     I_holdings += '%d '% (int(hc*1e12))
                 else:
                     I_holdings += '?? '
                     
-            item = QtGui.QTreeWidgetItem([str(i), stim_name, modes, V_holdings, I_holdings])
+            item = QtWidgets.QTreeWidgetItem([str(i), stim_name, modes, V_holdings, I_holdings])
             item.setCheckState(0, QtCore.Qt.Unchecked)
             item.data = sweep
             self.sweep_tree.addTopLevelItem(item)
  
-        self.sweep_tree.header().resizeSections(QtGui.QHeaderView.ResizeToContents)
+        self.sweep_tree.header().resizeSections(QtWidgets.QHeaderView.ResizeToContents)
 
     def selection(self):
         """Return a list of selected groups and/or sweeps. 
         """
         items = self.sweep_tree.selectedItems()
         selection = []
         for item in items:
@@ -147,15 +147,15 @@
                     #item = item.sweeps[0]
                 channels.extend(item.devices)
             channels = list(set(channels))
             channels.sort()
             
             # add new items to the channel list, all selected
             for ch in channels:
-                item = QtGui.QListWidgetItem(str(ch))
+                item = QtWidgets.QListWidgetItem(str(ch))
                 item.channel_index = ch
                 self._channel_selection.setdefault(ch, True)
                 # restore previous check state, if any.
                 checkstate = QtCore.Qt.Checked if self._channel_selection.setdefault(ch, True) else QtCore.Qt.Unchecked
                 item.setCheckState(checkstate)
                 self.channel_list.addItem(item)
         finally:
@@ -180,64 +180,64 @@
         keys = list(meta[0].keys())
         for m in meta[1:]:
             keys = merge_lists(keys, list(m.keys()))
         
         for k in keys:
             vals = [m.get(k) for m in meta]
             if isinstance(vals[0], dict):
-                item = QtGui.QTreeWidgetItem([k] + [''] * len(meta))
+                item = QtWidgets.QTreeWidgetItem([k] + [''] * len(meta))
                 self._populate_meta_tree(vals, item)
             else:
-                item = QtGui.QTreeWidgetItem([k] + [str(v) for v in vals])
+                item = QtWidgets.QTreeWidgetItem([k] + [str(v) for v in vals])
             root.addChild(item)
 
     def _tree_item_changed(self, item, col):
         if col != 0:
             return
         self.check_state_changed.emit(self)
         
     def _channel_list_changed(self, item):
         self.channels_changed.emit(self.selected_channels())
         self._channel_selection[item.channel_index] = item.checkState() == QtCore.Qt.Checked
 
 
-class MiesNwbViewer(QtGui.QWidget):
+class MiesNwbViewer(QtWidgets.QWidget):
     """Combination of a MiesNwvExplorer for selecting sweeps and a tab widget
     containing multiple views, each performing a different analysis.
     """
     analyzer_changed = QtCore.Signal(object)
     
     def __init__(self, nwb=None):
-        QtGui.QWidget.__init__(self)
+        QtWidgets.QWidget.__init__(self)
         self.nwb = nwb
         
-        self.layout = QtGui.QGridLayout()
+        self.layout = QtWidgets.QGridLayout()
         self.layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(self.layout)
 
-        self.hsplit = QtGui.QSplitter()
+        self.hsplit = QtWidgets.QSplitter()
         self.hsplit.setOrientation(QtCore.Qt.Horizontal)
         self.layout.addWidget(self.hsplit, 0, 0)
         
-        self.vsplit = QtGui.QSplitter()
+        self.vsplit = QtWidgets.QSplitter()
         self.vsplit.setOrientation(QtCore.Qt.Vertical)
         self.hsplit.addWidget(self.vsplit)
 
         self.explorer = MiesNwbExplorer(self.nwb)
         self.explorer.selection_changed.connect(self.data_selection_changed)
         self.explorer.channels_changed.connect(self.data_selection_changed)
         self.vsplit.addWidget(self.explorer)
 
         self.ptree = pg.parametertree.ParameterTree()
         self.vsplit.addWidget(self.ptree)
         
-        self.tabs = QtGui.QTabWidget()
+        self.tabs = QtWidgets.QTabWidget()
         self.hsplit.addWidget(self.tabs)
         
-        self.reload_btn = QtGui.QPushButton("Reload views")
+        self.reload_btn = QtWidgets.QPushButton("Reload views")
         self.reload_btn.clicked.connect(self.reload_views)
         self.vsplit.addWidget(self.reload_btn)
 
         self.views = []
         self.create_views()
         
         self.resize(1400, 800)
@@ -315,19 +315,19 @@
         ]
 
         for name, view in self.views:
             self.tabs.addTab(view, name)
 
 
 
-class AnalysisView(QtGui.QWidget):
+class AnalysisView(QtWidgets.QWidget):
     """Example skeleton for an analysis view.
     """
     def __init__(self, parent=None):
-        QtGui.QWidget.__init__(self, parent)
+        QtWidgets.QWidget.__init__(self, parent)
         
         # Views must have self.params
         # This implements the controls that are unique to this view.
         self.params = pg.parametertree.Parameter(name='params', type='group', children=[
             {'name': 'lowpass', 'type': 'float', 'value': 0, 'limits': [0, None], 'step': 1},
             {'name': 'average', 'type': 'bool', 'value': False},
         ])
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/plot_grid.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/plot_grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pyqtgraph as pg
-from pyqtgraph.Qt import QtGui, QtCore
+from . import qt
 
 
-class PlotGrid(QtGui.QWidget):
+class PlotGrid(qt.QWidget):
     def __init__(self, parent=None):
-        QtGui.QWidget.__init__(self, parent)
+        qt.QWidget.__init__(self, parent)
         
         self.rows = 0
         self.cols = 0
         self.plots = []
-        
-        self.layout = QtGui.QGridLayout()
+
+        self.layout = qt.QGridLayout()
         self.layout.setSpacing(0)
         self.layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(self.layout)
 
         self.grid = pg.GraphicsLayoutWidget()
         self.grid.ci.layout.setSpacing(0)
         self.layout.addWidget(self.grid)
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/psp_fitting.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/psp_fitting.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """
     def __init__(self, title=None):
         self.pw = pg.GraphicsLayoutWidget()
         self.plt1 = self.pw.addPlot(title=title)
         
         self.console = pg.console.ConsoleWidget()
         
-        self.widget = pg.QtGui.QSplitter(pg.QtCore.Qt.Vertical)
+        self.widget = pg.QtWidgets.QSplitter(pg.QtCore.Qt.Vertical)
         self.widget.addWidget(self.pw)        
         self.widget.addWidget(self.console)
         self.widget.resize(1000, 600)
         self.widget.setSizes([400, 200])
         self.widget.show()
     
     def clear(self):
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/signal.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/signal.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/spike_detection.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/spike_detection.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.plt2 = self.pw.addPlot(row=1, col=0)
         self.plt2.setXLink(self.plt1)
         self.plt3 = self.pw.addPlot(row=2, col=0)
         self.plt3.setXLink(self.plt1)
         
         self.console = pg.console.ConsoleWidget()
         
-        self.widget = pg.QtGui.QSplitter(pg.QtCore.Qt.Vertical)
+        self.widget = pg.QtWidgets.QSplitter(pg.QtCore.Qt.Vertical)
         self.widget.addWidget(self.pw)        
         self.widget.addWidget(self.console)
         self.widget.resize(1000, 900)
         self.widget.setSizes([800, 200])
         self.widget.show()
     
     def clear(self):
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/sta_analyzer.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/sta_analyzer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 import pyqtgraph as pg
-from pyqtgraph.Qt import QtGui, QtCore
+from pyqtgraph.Qt import QtWidgets, QtCore
 import pyqtgraph.parametertree as pt
 from .cell_selector import CellSelector
 from .event_detection import EventDetector
 from .triggered_average import TriggeredAverager
 from ..data import TSeries
 
 
-class STAAnalyzer(QtGui.QWidget):
+class STAAnalyzer(QtWidgets.QWidget):
     """Analyzer for running spike-triggered averaging on BOb calcium imaging data.
     
     Features:
     
     * Select cells from a list of pre-segmented ROIs
     * Detect spikes using exponential deconvolution
     * Plot calcium signal and deconvolved signal
@@ -40,19 +40,19 @@
 
         # setup averager
         self.averager = TriggeredAverager()
         
         # make stimulus frame locations easier to look up
         self.lsn_id = None
         
-        QtGui.QWidget.__init__(self)
-        self.hs = pg.QtGui.QSplitter()
+        QtWidgets.QWidget.__init__(self)
+        self.hs = pg.QtWidgets.QSplitter()
         self.hs.setOrientation(pg.QtCore.Qt.Horizontal)
 
-        self.vs1 = pg.QtGui.QSplitter()
+        self.vs1 = pg.QtWidgets.QSplitter()
         self.vs1.setOrientation(pg.QtCore.Qt.Vertical)
 
         self.params = pt.Parameter(name='params', type='group', children=[
             self.cell_selector.params,
             self.spike_detector.params,
             self.averager.params,
         ])
@@ -62,15 +62,15 @@
         self.vs1.addWidget(self.tree)
 
         self.expt_imv = pg.ImageView()
         self.cell_selector.set_imageview(self.expt_imv)
         
         self.vs1.addWidget(self.expt_imv)
 
-        self.vs2 = pg.QtGui.QSplitter()
+        self.vs2 = pg.QtWidgets.QSplitter()
         self.vs2.setOrientation(pg.QtCore.Qt.Vertical)
 
         self.plt1 = pg.PlotWidget()
         self.plt2 = pg.PlotWidget()
         self.plt2.setXLink(self.plt1)
         self.spike_detector.set_plots(self.plt1, self.plt2)
 
@@ -80,15 +80,15 @@
         self.vs2.addWidget(self.plt1)
         self.vs2.addWidget(self.plt2)
         self.vs2.addWidget(self.sta_imv)
 
         self.hs.addWidget(self.vs1)
         self.hs.addWidget(self.vs2)
         
-        self.layout = QtGui.QGridLayout()
+        self.layout = QtWidgets.QGridLayout()
         self.setLayout(self.layout)
         self.layout.addWidget(self.hs)
         
         self.resize(1400, 800)
         self.hs.setSizes([600, 600])
         self.show()
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/triggered_average.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/triggered_average.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pyqtgraph as pg
-from pyqtgraph.Qt import QtGui, QtCore
+from pyqtgraph.Qt import QtWidgets, QtCore
 import pyqtgraph.parametertree as pt
 import numpy as np
 import scipy.ndimage as ndi
 
 
 class TriggeredAverager(QtCore.QObject):
     parameters_changed = QtCore.Signal(object)  # self
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/ui/user_test.py` & `neuroanalysis-0.0.2/neuroanalysis/ui/user_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 import pyqtgraph as pg
 
 
 class UserTestUi(object):
     def __init__(self, expected_display, current_display):
         pg.mkQApp()
 
-        self.widget = pg.QtGui.QSplitter(pg.QtCore.Qt.Vertical)
+        self.widget = pg.QtWidgets.QSplitter(pg.QtCore.Qt.Vertical)
         self.widget.resize(1600, 1000)
 
-        self.display_splitter = pg.QtGui.QSplitter(pg.QtCore.Qt.Horizontal)
+        self.display_splitter = pg.QtWidgets.QSplitter(pg.QtCore.Qt.Horizontal)
         self.widget.addWidget(self.display_splitter)
         
         self.display1 = expected_display
         self.display2 = current_display
         self.display_splitter.addWidget(self.display1.widget)
         self.display_splitter.addWidget(self.display2.widget)
 
-        self.ctrl = pg.QtGui.QWidget()
+        self.ctrl = pg.QtWidgets.QWidget()
         self.widget.addWidget(self.ctrl)
-        self.ctrl_layout = pg.QtGui.QVBoxLayout()
+        self.ctrl_layout = pg.QtWidgets.QVBoxLayout()
         self.ctrl.setLayout(self.ctrl_layout)
         self.diff_widget = pg.DiffTreeWidget()
         self.ctrl_layout.addWidget(self.diff_widget)
 
-        self.pass_btn = pg.QtGui.QPushButton('pass')
-        self.fail_btn = pg.QtGui.QPushButton('fail')
+        self.pass_btn = pg.QtWidgets.QPushButton('pass')
+        self.fail_btn = pg.QtWidgets.QPushButton('fail')
         self.ctrl_layout.addWidget(self.pass_btn)
         self.ctrl_layout.addWidget(self.fail_btn)
 
         self.pass_btn.clicked.connect(self.pass_clicked)
         self.fail_btn.clicked.connect(self.fail_clicked)
 
         self.last_btn_clicked = None
@@ -40,15 +40,15 @@
 
     def fail_clicked(self):
         self.last_btn_clicked = 'fail'
 
     def user_passfail(self):
         self.widget.show()
         while True:
-            pg.QtGui.QApplication.processEvents()
+            pg.QtWidgets.QApplication.processEvents()
             last_btn_clicked = self.last_btn_clicked
             self.last_btn_clicked = None
 
             if last_btn_clicked == 'fail' or not self.widget.isVisible():
                 raise Exception("User rejected test result.")
             elif last_btn_clicked == 'pass':
                 break
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis/units.py` & `neuroanalysis-0.0.2/neuroanalysis/units.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/util/custom_weakref.py` & `neuroanalysis-0.0.2/neuroanalysis/util/custom_weakref.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/util/data_test.py` & `neuroanalysis-0.0.2/neuroanalysis/util/data_test.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/util/jit.py` & `neuroanalysis-0.0.2/neuroanalysis/util/jit.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/util/merge_lists.py` & `neuroanalysis-0.0.2/neuroanalysis/util/merge_lists.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/util/mies_nwb_parsing.py` & `neuroanalysis-0.0.2/neuroanalysis/util/mies_nwb_parsing.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis/util/optional_import.py` & `neuroanalysis-0.0.2/neuroanalysis/util/optional_import.py`

 * *Files identical despite different names*

### Comparing `neuroanalysis-0.0.1/neuroanalysis.egg-info/PKG-INFO` & `neuroanalysis-0.0.2/neuroanalysis.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: neuroanalysis
-Version: 0.0.1
+Version: 0.0.2
 Summary: Functions and modular user interface tools for analysis of patch clamp experiment data.
 Home-page: https://github.com/AllenInstitute/neuroanalysis
 Author: Luke Campagnola
 Author-email: lukec@alleninstitute.org
 License: MIT
-Description: Neuroanalysis
-        =============
-        
-        Modular and interactive tools for analysis of neurophysiology data, with emphasis on 
-        patch-clamp electrophysiology.
-        
-        * Functions for running common analysis algorithms
-            * Synaptic/calcium event detection and characterization
-            * Synaptic release modeling
-            * VC and CC spike detection and characterization
-            * VC and CC test pulse analysis
-            * Basic signal processing (filtering, baseline removal, etc.)
-        * Data abstraction layer to allow adapting new data formats (see neuroanalysis/data.py)
-        * Re-usable user interface elements for implementing common analysis tasks
-        
-        
-        Status
-        ------
-        
-        This project is early in development and does not yet have a stable API.
-        Issues and pull requests are accepted (see CONTRIBUTING.md), but may not be 
-        reviewed or accepted on any fixed schedule.
-        
-        
-        
-        
-        
-        
 Keywords: neuroscience analysis neurodata without borders nwb
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: lmfit
+Requires-Dist: numpy
+Requires-Dist: scipy
+
+Neuroanalysis
+=============
+
+Modular and interactive tools for analysis of neurophysiology data, with emphasis on 
+patch-clamp electrophysiology.
+
+* Functions for running common analysis algorithms
+    * Synaptic/calcium event detection and characterization
+    * Synaptic release modeling
+    * VC and CC spike detection and characterization
+    * VC and CC test pulse analysis
+    * Basic signal processing (filtering, baseline removal, etc.)
+* Data abstraction layer to allow adapting new data formats (see neuroanalysis/data.py)
+* Re-usable user interface elements for implementing common analysis tasks
+
+
+Status
+------
+
+This project is early in development and does not yet have a stable API.
+Issues and pull requests are accepted (see CONTRIBUTING.md), but may not be 
+reviewed or accepted on any fixed schedule.
+
+
+
+
+
```

### Comparing `neuroanalysis-0.0.1/neuroanalysis.egg-info/SOURCES.txt` & `neuroanalysis-0.0.2/neuroanalysis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 pyproject.toml
 setup.py
 neuroanalysis/__init__.py
 neuroanalysis/baseline.py
 neuroanalysis/event_detection.py
 neuroanalysis/filter.py
@@ -45,24 +46,26 @@
 neuroanalysis/ui/cell_selector.py
 neuroanalysis/ui/event_detection.py
 neuroanalysis/ui/filter.py
 neuroanalysis/ui/fitting.py
 neuroanalysis/ui/plot_adapter.py
 neuroanalysis/ui/plot_grid.py
 neuroanalysis/ui/psp_fitting.py
+neuroanalysis/ui/qt.py
 neuroanalysis/ui/signal.py
 neuroanalysis/ui/spike_detection.py
 neuroanalysis/ui/sta_analyzer.py
 neuroanalysis/ui/triggered_average.py
 neuroanalysis/ui/user_test.py
 neuroanalysis/ui/nwb_viewer/__init__.py
 neuroanalysis/ui/nwb_viewer/analyzer_view.py
 neuroanalysis/ui/nwb_viewer/sweep_view.py
 neuroanalysis/ui/nwb_viewer/viewer.py
 neuroanalysis/util/__init__.py
 neuroanalysis/util/custom_weakref.py
 neuroanalysis/util/data_test.py
+neuroanalysis/util/h5py_wrapper.py
 neuroanalysis/util/jit.py
 neuroanalysis/util/lru_cache.py
 neuroanalysis/util/merge_lists.py
 neuroanalysis/util/mies_nwb_parsing.py
 neuroanalysis/util/optional_import.py
```

### Comparing `neuroanalysis-0.0.1/setup.py` & `neuroanalysis-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,9 +32,9 @@
     keywords="neuroscience analysis neurodata without borders nwb",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="neuroanalysis",
     packages=find_packages(),
     url="https://github.com/AllenInstitute/neuroanalysis",
-    version="0.0.1",
+    version="0.0.2",
 )
```

