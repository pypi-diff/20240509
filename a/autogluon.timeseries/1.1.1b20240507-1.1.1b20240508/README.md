# Comparing `tmp/autogluon.timeseries-1.1.1b20240507.tar.gz` & `tmp/autogluon.timeseries-1.1.1b20240508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-1.1.1b20240507.tar", last modified: Tue May  7 09:05:14 2024, max compression
+gzip compressed data, was "autogluon.timeseries-1.1.1b20240508.tar", last modified: Wed May  8 09:05:23 2024, max compression
```

## Comparing `autogluon.timeseries-1.1.1b20240507.tar` & `autogluon.timeseries-1.1.1b20240508.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.989650 autogluon.timeseries-1.1.1b20240507/
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-05-07 09:05:14.989650 autogluon.timeseries-1.1.1b20240507/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:05:14.989650 autogluon.timeseries-1.1.1b20240507/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.977650 autogluon.timeseries-1.1.1b20240507/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.977650 autogluon.timeseries-1.1.1b20240507/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.981650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.981650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.981650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45595 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.981650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/metrics/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/metrics/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/metrics/quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.981650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.981650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.981650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31491 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.985650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/chronos/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/chronos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/chronos/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/chronos/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/chronos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.985650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.985650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34017 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.985650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.985650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/local/npts.py
--rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/local/statsforecast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.985650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    81915 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.985650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59104 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.989650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.989650 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/datetime/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/datetime/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/datetime/lags.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/datetime/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/datetime/time_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    19585 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-07 09:03:39.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-07 09:05:14.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:14.981650 autogluon.timeseries-1.1.1b20240507/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-05-07 09:05:14.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-07 09:05:14.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:05:14.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 09:05:14.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-07 09:05:14.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 09:05:14.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:05:14.000000 autogluon.timeseries-1.1.1b20240507/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.728984 autogluon.timeseries-1.1.1b20240508/
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-05-08 09:05:23.728984 autogluon.timeseries-1.1.1b20240508/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:05:23.728984 autogluon.timeseries-1.1.1b20240508/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.716984 autogluon.timeseries-1.1.1b20240508/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.716984 autogluon.timeseries-1.1.1b20240508/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.720984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.720984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.720984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45595 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.720984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/metrics/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/metrics/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/metrics/quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.724984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.724984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.724984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32682 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.724984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/chronos/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/chronos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/chronos/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/chronos/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/chronos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.724984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.724984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34017 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.724984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.724984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/local/npts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/local/statsforecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.724984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81915 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.728984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59104 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.728984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.728984 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/datetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/datetime/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/datetime/lags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/datetime/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/datetime/time_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19585 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-08 09:03:56.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-08 09:05:23.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:23.720984 autogluon.timeseries-1.1.1b20240508/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-05-08 09:05:23.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-08 09:05:23.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:05:23.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 09:05:23.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-08 09:05:23.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 09:05:23.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:05:23.000000 autogluon.timeseries-1.1.1b20240508/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-1.1.1b20240507/PKG-INFO` & `autogluon.timeseries-1.1.1b20240508/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.1.1b20240507
+Version: 1.1.1b20240508
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.1.1b20240507/setup.py` & `autogluon.timeseries-1.1.1b20240508/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/metrics/__init__.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/metrics/abstract.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/metrics/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/metrics/point.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/metrics/point.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/metrics/quantile.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/metrics/quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/metrics/utils.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,36 @@
         self._target_lags: Optional[List[int]] = None
         self._date_features: Optional[List[str]] = None
         self._mlf: Optional[MLForecast] = None
         self._scaler: Optional[BaseTargetTransform] = None
         self._residuals_std_per_item: Optional[pd.Series] = None
         self._avg_residuals_std: Optional[float] = None
         self._train_target_median: Optional[float] = None
+        self._non_boolean_real_covariates: List[str] = []
+
+    @property
+    def tabular_predictor_path(self) -> str:
+        return os.path.join(self.path, "tabular_predictor")
+
+    def save(self, path: str = None, verbose: bool = True) -> str:
+        assert "mean" in self._mlf.models_, "TabularPredictor must be trained before saving"
+        tabular_predictor = self._mlf.models_["mean"].predictor
+        self._mlf.models_["mean"].predictor = None
+        save_path = super().save(path=path, verbose=verbose)
+        self._mlf.models_["mean"].predictor = tabular_predictor
+        return save_path
+
+    @classmethod
+    def load(
+        cls, path: str, reset_paths: bool = True, load_oof: bool = False, verbose: bool = True
+    ) -> "AbstractTimeSeriesModel":
+        model = super().load(path=path, reset_paths=reset_paths, load_oof=load_oof, verbose=verbose)
+        assert "mean" in model._mlf.models_, "Loaded model doesn't have a trained TabularPredictor"
+        model._mlf.models_["mean"].predictor = TabularPredictor.load(model.tabular_predictor_path)
+        return model
 
     def preprocess(self, data: TimeSeriesDataFrame, is_train: bool = False, **kwargs) -> Any:
         if is_train:
             # All-NaN series are removed; partially-NaN series in train_data are handled inside _generate_train_val_dfs
             all_nan_items = data.item_ids[data[self.target].isna().groupby(ITEMID, sort=False).all()]
             if len(all_nan_items):
                 data = data.query("item_id not in @all_nan_items")
@@ -248,18 +270,17 @@
             selected_columns += [self.target]
             column_name_mapping[self.target] = MLF_TARGET
 
         df = pd.DataFrame(data)[selected_columns].reset_index()
         if static_features is not None:
             df = pd.merge(df, static_features, how="left", on=ITEMID, suffixes=(None, "_static_feat"))
 
-        for col in self.metadata.known_covariates_real:
+        for col in self._non_boolean_real_covariates:
             # Normalize non-boolean features using mean_abs scaling
-            if not df[col].isin([0, 1]).all():
-                df[f"__scaled_{col}"] = df[col] / df[col].abs().groupby(df[ITEMID]).mean().reindex(df[ITEMID]).values
+            df[f"__scaled_{col}"] = df[col] / df[col].abs().groupby(df[ITEMID]).mean().reindex(df[ITEMID]).values
 
         # Convert float64 to float32 to reduce memory usage
         float64_cols = list(df.select_dtypes(include="float64"))
         df[float64_cols] = df[float64_cols].astype("float32")
 
         # We assume that df is sorted by 'unique_id' inside `TimeSeriesPredictor._check_and_prepare_data_frame`
         return df.rename(columns=column_name_mapping)
@@ -273,14 +294,17 @@
         **kwargs,
     ) -> None:
         from mlforecast import MLForecast
 
         self._check_fit_params()
         fit_start_time = time.time()
         self._train_target_median = train_data[self.target].median()
+        for col in self.metadata.known_covariates_real:
+            if not train_data[col].isin([0, 1]).all():
+                self._non_boolean_real_covariates.append(col)
         # TabularEstimator is passed to MLForecast later to include tuning_data
         model_params = self._get_model_params()
 
         mlforecast_init_args = self._get_mlforecast_init_args(train_data, model_params)
         self._mlf = MLForecast(models={}, freq=self.freq, **mlforecast_init_args)
 
         # We generate train/val splits from train_data and ignore val_data to avoid overfitting
@@ -288,15 +312,15 @@
             train_data,
             max_num_items=model_params["max_num_items"],
             max_num_samples=model_params["max_num_samples"],
         )
 
         estimator = TabularEstimator(
             predictor_init_kwargs={
-                "path": os.path.join(self.path, "tabular_predictor"),
+                "path": self.tabular_predictor_path,
                 "verbosity": verbosity - 2,
                 "label": MLF_TARGET,
                 **self._get_extra_tabular_init_kwargs(),
             },
             predictor_fit_kwargs={
                 "tuning_data": val_df.drop(columns=[MLF_ITEMID]),
                 "time_limit": None if time_limit is None else time_limit - (time.time() - fit_start_time),
```

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/chronos/model.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/chronos/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/chronos/pipeline.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/chronos/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/chronos/utils.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/chronos/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/local/npts.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/local/npts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/datetime/base.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/datetime/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/datetime/lags.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/datetime/lags.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/datetime/seasonality.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/datetime/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/datetime/time_features.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/datetime/time_features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-1.1.1b20240508/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-1.1.1b20240508/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.1.1b20240507
+Version: 1.1.1b20240508
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-1.1.1b20240508/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.1b20240507/src/autogluon.timeseries.egg-info/requires.txt` & `autogluon.timeseries-1.1.1b20240508/src/autogluon.timeseries.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 networkx<4,>=3.0
 statsforecast<1.5,>=1.4.0
 mlforecast<0.10.1,>=0.10.0
 utilsforecast<0.0.11,>=0.0.10
 tqdm<5,>=4.38
 orjson~=3.9
 tensorboard<3,>=2.9
-autogluon.core[raytune]==1.1.1b20240507
-autogluon.common==1.1.1b20240507
-autogluon.tabular[catboost,lightgbm,xgboost]==1.1.1b20240507
+autogluon.core[raytune]==1.1.1b20240508
+autogluon.common==1.1.1b20240508
+autogluon.tabular[catboost,lightgbm,xgboost]==1.1.1b20240508
 
 [all]
 optimum[onnxruntime]<1.19,>=1.17
 
 [chronos-onnx]
 optimum[onnxruntime]<1.19,>=1.17
```

