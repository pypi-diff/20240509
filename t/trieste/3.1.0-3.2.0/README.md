# Comparing `tmp/trieste-3.1.0.tar.gz` & `tmp/trieste-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trieste-3.1.0.tar", last modified: Tue Mar 26 16:43:43 2024, max compression
+gzip compressed data, was "trieste-3.2.0.tar", last modified: Thu May  9 09:27:45 2024, max compression
```

## Comparing `trieste-3.1.0.tar` & `trieste-3.2.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.809206 trieste-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-26 16:43:34.000000 trieste-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-03-26 16:43:43.809206 trieste-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-03-26 16:43:34.000000 trieste-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-26 16:43:34.000000 trieste-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 16:43:43.809206 trieste-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-03-26 16:43:34.000000 trieste-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.797206 trieste-3.1.0/trieste/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.801206 trieste-3.1.0/trieste/acquisition/
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/combination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.801206 trieste-3.1.0/trieste/acquisition/function/
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20754 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/function/active_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/function/continuous_thompson_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)    36585 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/function/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    77644 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/function/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    35334 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/function/greedy_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    33916 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/function/multi_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/function/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16951 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.805206 trieste-3.1.0/trieste/acquisition/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/multi_objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/multi_objective/dominance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/multi_objective/pareto.py
--rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/multi_objective/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    42509 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)   114208 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9707 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/acquisition/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20957 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/ask_tell_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    49852 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/bayesian_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.805206 trieste-3.1.0/trieste/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.805206 trieste-3.1.0/trieste/experimental/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/experimental/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/experimental/plotting/inequality_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    23612 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/experimental/plotting/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/experimental/plotting/plotting_plotly.py
--rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.805206 trieste-3.1.0/trieste/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.805206 trieste-3.1.0/trieste/models/gpflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27404 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflow/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflow/inducing_point_selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflow/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    91274 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflow/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    41061 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflow/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.809206 trieste-3.1.0/trieste/models/gpflux/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflux/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflux/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflux/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    20658 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/gpflux/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    31342 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.809206 trieste-3.1.0/trieste/models/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15525 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/keras/architectures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/keras/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/keras/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    26847 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/keras/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/keras/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/keras/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.809206 trieste-3.1.0/trieste/objectives/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/objectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/objectives/multi_objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/objectives/multifidelity_objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)    24268 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/objectives/single_objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/objectives/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/observer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    54241 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.809206 trieste-3.1.0/trieste/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13957 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-26 16:43:34.000000 trieste-3.1.0/trieste/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:43:43.809206 trieste-3.1.0/trieste.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-03-26 16:43:43.000000 trieste-3.1.0/trieste.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-26 16:43:43.000000 trieste-3.1.0/trieste.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:43:43.000000 trieste-3.1.0/trieste.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-26 16:43:43.000000 trieste-3.1.0/trieste.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 16:43:43.000000 trieste-3.1.0/trieste.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.022075 trieste-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-09 09:27:37.000000 trieste-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-09 09:27:45.022075 trieste-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-09 09:27:37.000000 trieste-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-09 09:27:37.000000 trieste-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:27:45.022075 trieste-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-09 09:27:37.000000 trieste-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.010075 trieste-3.2.0/trieste/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.010075 trieste-3.2.0/trieste/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/combination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.014075 trieste-3.2.0/trieste/acquisition/function/
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20754 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/continuous_thompson_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36585 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77644 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35334 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/greedy_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33916 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/multi_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/function/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16951 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.014075 trieste-3.2.0/trieste/acquisition/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/multi_objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/multi_objective/dominance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/multi_objective/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/multi_objective/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42509 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117386 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/acquisition/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27114 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/ask_tell_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49911 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/bayesian_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.014075 trieste-3.2.0/trieste/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.014075 trieste-3.2.0/trieste/experimental/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/experimental/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/experimental/plotting/inequality_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23612 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/experimental/plotting/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/experimental/plotting/plotting_plotly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.014075 trieste-3.2.0/trieste/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.018075 trieste-3.2.0/trieste/models/gpflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27404 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/inducing_point_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91274 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41061 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.018075 trieste-3.2.0/trieste/models/gpflux/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflux/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflux/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflux/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20658 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/gpflux/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31342 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.018075 trieste-3.2.0/trieste/models/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15525 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26847 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/keras/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.018075 trieste-3.2.0/trieste/objectives/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/objectives/multi_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/objectives/multifidelity_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24268 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/objectives/single_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/objectives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54241 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.018075 trieste-3.2.0/trieste/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13957 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-09 09:27:37.000000 trieste-3.2.0/trieste/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:27:45.022075 trieste-3.2.0/trieste.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-09 09:27:44.000000 trieste-3.2.0/trieste.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-09 09:27:45.000000 trieste-3.2.0/trieste.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:27:44.000000 trieste-3.2.0/trieste.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-09 09:27:44.000000 trieste-3.2.0/trieste.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 09:27:44.000000 trieste-3.2.0/trieste.egg-info/top_level.txt
```

### Comparing `trieste-3.1.0/LICENSE` & `trieste-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/PKG-INFO` & `trieste-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trieste
-Version: 3.1.0
+Version: 3.2.0
 Summary: A Bayesian optimization research toolbox built on TensorFlow
 Home-page: https://github.com/secondmind-labs/trieste
 Author: The Trieste contributors
 Author-email: labs@secondmind.ai
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `trieste-3.1.0/README.md` & `trieste-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/pyproject.toml` & `trieste-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/setup.py` & `trieste-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/__init__.py` & `trieste-3.2.0/trieste/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/__init__.py` & `trieste-3.2.0/trieste/acquisition/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,21 +96,32 @@
     VectorizedAcquisitionFunctionBuilder,
 )
 from .rule import (
     AcquisitionRule,
     AsynchronousGreedy,
     AsynchronousOptimization,
     BatchHypervolumeSharpeRatioIndicator,
+    BatchTrustRegion,
     BatchTrustRegionBox,
+    BatchTrustRegionProduct,
     DiscreteThompsonSampling,
     EfficientGlobalOptimization,
+    FixedPointTrustRegionDiscrete,
+    HypercubeTrustRegion,
+    LocalDatasetsAcquisitionRule,
     RandomSampling,
     SingleObjectiveTrustRegionBox,
+    SingleObjectiveTrustRegionDiscrete,
     TREGOBox,
     TURBOBox,
+    UpdatableSearchSpace,
+    UpdatableTrustRegion,
+    UpdatableTrustRegionBox,
+    UpdatableTrustRegionDiscrete,
+    UpdatableTrustRegionProduct,
 )
 from .sampler import (
     ExactThompsonSampler,
     GumbelSampler,
     ThompsonSampler,
     ThompsonSamplerFromTrajectory,
 )
```

### Comparing `trieste-3.1.0/trieste/acquisition/combination.py` & `trieste-3.2.0/trieste/acquisition/combination.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/function/__init__.py` & `trieste-3.2.0/trieste/acquisition/function/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/function/active_learning.py` & `trieste-3.2.0/trieste/acquisition/function/active_learning.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/function/continuous_thompson_sampling.py` & `trieste-3.2.0/trieste/acquisition/function/continuous_thompson_sampling.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/function/entropy.py` & `trieste-3.2.0/trieste/acquisition/function/entropy.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/function/function.py` & `trieste-3.2.0/trieste/acquisition/function/function.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/function/greedy_batch.py` & `trieste-3.2.0/trieste/acquisition/function/greedy_batch.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/function/multi_objective.py` & `trieste-3.2.0/trieste/acquisition/function/multi_objective.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/function/utils.py` & `trieste-3.2.0/trieste/acquisition/function/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/interface.py` & `trieste-3.2.0/trieste/acquisition/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/multi_objective/__init__.py` & `trieste-3.2.0/trieste/acquisition/multi_objective/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/multi_objective/dominance.py` & `trieste-3.2.0/trieste/acquisition/multi_objective/dominance.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/multi_objective/pareto.py` & `trieste-3.2.0/trieste/acquisition/multi_objective/pareto.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/multi_objective/partition.py` & `trieste-3.2.0/trieste/acquisition/multi_objective/partition.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/optimizer.py` & `trieste-3.2.0/trieste/acquisition/optimizer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/rule.py` & `trieste-3.2.0/trieste/acquisition/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -987,35 +987,18 @@
             query_points,
             select_output=self._select_output,
         )
 
         return thompson_samples
 
 
-class UpdatableTrustRegion(SearchSpace):
+class UpdatableSearchSpace(SearchSpace):
     """A search space that can be updated."""
 
-    def __init__(
-        self,
-        region_index: Optional[int] = None,
-        input_active_dims: Optional[Union[slice, Sequence[int]]] = None,
-    ) -> None:
-        """
-        :param region_index: The index of the region in a multi-region search space. This is used to
-            identify the local models and datasets to use for acquisition. If `None`, the
-            global models and datasets are used.
-        :param input_active_dims: The active dimensions of the input space, either a slice or list
-            of indices into the columns of the space. If `None`, all dimensions are active.
-
-            When this region is part of a product search-space (via `UpdatableTrustRegionProduct`),
-            this is used to select the active dimensions of the full input space that belong to this
-            region.
-        """
-        self.region_index = region_index
-        self.input_active_dims = input_active_dims
+    def __init__(self) -> None:
         self._initialized = False
 
     @property
     def requires_initialization(self) -> bool:
         """Return `True` if the search space needs to be re-initialized with the latest models
         and datasets, and `False` if it can be just updated."""
         return not self._initialized
@@ -1045,14 +1028,75 @@
         """
         Update the search space using the given models and datasets.
 
         :param models: The model for each tag.
         :param datasets: The dataset for each tag.
         """
 
+
+class UpdatableTrustRegion(UpdatableSearchSpace):
+    """An updatable trust region with a concept of a location within a global search space."""
+
+    def __init__(
+        self,
+        region_index: Optional[int] = None,
+        input_active_dims: Optional[Union[slice, Sequence[int]]] = None,
+    ) -> None:
+        """
+        :param region_index: The index of the region in a multi-region search space. This is used to
+            identify the local models and datasets to use for acquisition. If `None`, the
+            global models and datasets are used.
+        :param input_active_dims: The active dimensions of the input space, either a slice or list
+            of indices into the columns of the space. If `None`, all dimensions are active.
+
+            When this region is part of a product search-space (via `UpdatableTrustRegionProduct`),
+            this is used to select the active dimensions of the full input space that belong to this
+            region.
+        """
+        super().__init__()
+        self.region_index = region_index
+        self.input_active_dims = input_active_dims
+
+    def _init_location(
+        self,
+        models: Optional[Mapping[Tag, ProbabilisticModelType]] = None,
+        datasets: Optional[Mapping[Tag, Dataset]] = None,
+        location_candidate: Optional[TensorType] = None,
+    ) -> None:
+        """
+        Initialize the location of the region, either by sampling a new location from the global
+        search space, or by using a candidate location if provided.
+
+        Derived classes can override this method to provide custom initialization logic.
+
+        :param models: The model for each tag.
+        :param datasets: The dataset for each tag.
+        :param location_candidate: A candidate for the location of the search space. If not
+            None, this is used instead of sampling a new location.
+        """
+        if location_candidate is not None:
+            self.location = location_candidate
+        else:
+            self.location = tf.squeeze(self.global_search_space.sample(1), axis=0)
+
+    @property
+    @abstractmethod
+    def location(self) -> TensorType:
+        """The center of the region."""
+
+    @location.setter
+    @abstractmethod
+    def location(self, location: TensorType) -> None:
+        """Set the center of the region."""
+
+    @property
+    @abstractmethod
+    def global_search_space(self) -> SearchSpace:
+        """The global search space this region lives in."""
+
     def _get_tags(self, tags: Set[Tag]) -> Tuple[Set[Tag], Set[Tag]]:
         # Separate tags into local (matching index) and global tags (without matching
         # local tag).
         local_gtags = set()  # Set of global part of all local tags.
         global_tags = set()  # Set of all global tags.
         for tag in tags:
             ltag = LocalizedTag.from_tag(tag)
@@ -1091,15 +1135,17 @@
 
         :param value: The value to select the active input dimensions for.
         :return: The value with the active input dimensions selected.
         """
 
         # No selection for models.
         # Nothing to do if active dimensions are not set.
-        if isinstance(value, ProbabilisticModel) or self.input_active_dims is None:
+        # NOTE: do not replace with isinstance(value, ProbabilisticModel) until
+        # https://github.com/secondmind-labs/trieste/issues/836 has been fixed.
+        if not isinstance(value, (Dataset, tf.Tensor)) or self.input_active_dims is None:
             return value
 
         # Select components of query points for datasets.
         if isinstance(value, Dataset):
             input = value.query_points
         else:
             input = value
@@ -1132,15 +1178,15 @@
     ) -> Mapping[Tag, ProbabilisticModel]:
         ...
 
     def select_in_region(
         self, mapping: Optional[Mapping[Tag, Union[TensorType, Dataset, ProbabilisticModel]]]
     ) -> Optional[Mapping[Tag, Union[TensorType, Dataset, ProbabilisticModel]]]:
         """
-        Select items belonging to this region for acquisition.
+        Select items belonging to this region for, e.g., acquisition.
 
         :param mapping: The mapping of items for each tag.
         :return: The items belonging to this region (or `None` if there aren't any).
         """
         if mapping is None:
             _mapping = {}
         elif self.region_index is None:
@@ -1480,188 +1526,295 @@
         for tag, dataset in datasets.items():
             if not LocalizedTag.from_tag(tag).is_local:
                 filtered_datasets[tag] = dataset
 
         return filtered_datasets
 
 
-class UpdatableTrustRegionBox(Box, UpdatableTrustRegion):
+class HypercubeTrustRegion(UpdatableTrustRegion):
     """
-    A simple updatable box search space with a centre location and an associated global search
-    space.
+    An abstract updatable trust region that defines a hypercube region in the global search space.
+    The region is defined by a location and a size in each dimension. This class is used to
+    implement different types of search spaces, e.g. continuous (SingleObjectiveTrustRegionBox) and
+    discrete (SingleObjectiveTrustRegionDiscrete).
+
+    Derived classes must implement the `_update_domain` method to update the domain of the region
+    based on the location and size.
+
+    In the default implementation, the region is updated based on the minimum observed value in
+    the region from a single objective dataset. The region is expanded if the minimum is improved,
+    and contracted otherwise. Derived classes can override how this minimum is calculated, e.g. by
+    utilizing multiple datasets.
     """
 
     def __init__(
         self,
-        global_search_space: SearchSpace,
-        region_index: Optional[int] = None,
-        input_active_dims: Optional[Union[slice, Sequence[int]]] = None,
-    ):
-        """
-        :param global_search_space: The global search space this search space lives in.
-        :param region_index: The index of the region in a multi-region search space. This is used to
-            identify the local models and datasets to use for acquisition. If `None`, the
-            global models and datasets are used.
-        :param input_active_dims: The active dimensions of the input space, either a slice or list
-            of indices into the columns of the space. If `None`, all dimensions are active.
-        """
-        Box.__init__(self, global_search_space.lower, global_search_space.upper)
-        UpdatableTrustRegion.__init__(self, region_index, input_active_dims)
-        self._global_search_space = global_search_space
-        # Random initial location in the global search space.
-        self.location = tf.squeeze(global_search_space.sample(1), axis=0)
-
-    @property
-    def location(self) -> TensorType:
-        """The centre of the box."""
-        return self._location
-
-    @location.setter
-    def location(self, location: TensorType) -> None:
-        self._location = location
-
-    @property
-    def global_search_space(self) -> SearchSpace:
-        """The global search space this search space lives in."""
-        return self._global_search_space
-
-
-class SingleObjectiveTrustRegionBox(UpdatableTrustRegionBox):
-    """An updatable box search space for use with trust region acquisition rules."""
-
-    def __init__(
-        self,
-        global_search_space: SearchSpace,
         beta: float = 0.7,
         kappa: float = 1e-4,
         zeta: float = 0.5,
         min_eps: float = 1e-2,
-        region_index: Optional[int] = None,
-        input_active_dims: Optional[Union[slice, Sequence[int]]] = None,
     ):
         """
-        Calculates the bounds of the box from the location/centre and global bounds.
+        Calculates the bounds of the region from the location/center and global bounds.
 
-        :param global_search_space: The global search space this search space lives in.
         :param beta: The inverse of the trust region contraction factor.
         :param kappa: Scales the threshold for the minimal improvement required for a step to be
             considered a success.
         :param zeta: The initial size of the trust region is ``zeta`` times the size of the global
             search space.
         :param min_eps: The minimal size of the search space. If the size of the search space is
             smaller than this, the search space is reinitialized.
-        :param region_index: The index of the region in a multi-region search space. This is used to
-            identify the local models and datasets to use for acquisition. If `None`, the
-            global models and datasets are used.
-        :param input_active_dims: The active dimensions of the input space, either a slice or list
-            of indices into the columns of the space. If `None`, all dimensions are active.
         """
-        super().__init__(global_search_space, region_index, input_active_dims)
         self._beta = beta
         self._kappa = kappa
         self._zeta = zeta
         self._min_eps = min_eps
-
         self._step_is_success = False
-        self.eps = 0.0
+        # Randomly pick initial value of `self.location` for setting the bounds from the
+        # global search space.
+        self._init_location()
         self._init_eps()
-        self._update_bounds()
+        self._update_domain()
+        # Initial value of the region minimum is set to infinity as we have not yet observed any
+        # data.
         self._y_min = np.inf
 
+    def _init_eps(self) -> None:
+        self.eps = self._zeta * (self.global_search_space.upper - self.global_search_space.lower)
+
+    @abstractmethod
+    def _update_domain(self) -> None:
+        """Update the local domain of the region."""
+        ...
+
     @property
     def requires_initialization(self) -> bool:
         """
         Return `True` if the search space needs to be initialized, and `False` otherwise.
 
-        If uninitialized, or the size of the box is less than the minimum size, re-initialize
-        the box.
+        If uninitialized, or the size of the region is less than the minimum size, re-initialize
+        the region.
         """
         return not self._initialized or tf.reduce_any(self.eps < self._min_eps)
 
-    def _init_eps(self) -> None:
-        self.eps = self._zeta * (self.global_search_space.upper - self.global_search_space.lower)
-
-    def _update_bounds(self) -> None:
-        self._lower = tf.reduce_max(
-            [self.global_search_space.lower, self.location - self.eps], axis=0
-        )
-        self._upper = tf.reduce_min(
-            [self.global_search_space.upper, self.location + self.eps], axis=0
-        )
-
     def initialize(
         self,
         models: Optional[Mapping[Tag, ProbabilisticModelType]] = None,
         datasets: Optional[Mapping[Tag, Dataset]] = None,
+        location_candidate: Optional[TensorType] = None,
     ) -> None:
         """
-        Initialize the box by sampling a location from the global search space and setting the
-        bounds.
+        Initialize the region by sampling a location from the global search space and setting the
+        local region bounds around it.
+
+        :param models: The model for each tag.
+        :param datasets: The dataset for each tag.
+        :param location_candidate: A candidate for the location of the search space. If not
+            None, this is used instead of sampling a new location.
         """
-        datasets = self.select_in_region(datasets)
 
-        self.location = tf.squeeze(self.global_search_space.sample(1), axis=0)
+        # This returns datasets that are relevant for this region only, for each tag present in the
+        # dataset. Per tag it return a local dataset with a matching region index where it can;
+        # failing that it will return the global dataset for that tag.
+        datasets = self.select_in_region(datasets)
+        self._init_location(models, datasets, location_candidate=location_candidate)
         self._step_is_success = False
         self._init_eps()
-        self._update_bounds()
+        self._update_domain()
         _, self._y_min = self.get_dataset_min(datasets)
         self._initialized = True
 
     def update(
         self,
         models: Optional[Mapping[Tag, ProbabilisticModelType]] = None,
         datasets: Optional[Mapping[Tag, Dataset]] = None,
     ) -> None:
         """
-        Update this box, including centre/location, using the given dataset.
+        Update this region, including center/location, using the given dataset.
 
         If the new optimum improves over the previous optimum by some threshold (that scales
         linearly with ``kappa``), the previous acquisition is considered successful.
 
         If the previous acquisition was successful, the size is increased by a factor
         ``1 / beta``. Conversely, if it was unsuccessful, the size is reduced by the factor
         ``beta``.
+
+        :param models: The model for each tag.
+        :param datasets: The dataset for each tag.
         """
-        datasets = self.select_in_region(datasets)
+        datasets = self.select_in_region(datasets)  # See `select_in_region` comment above.
         x_min, y_min = self.get_dataset_min(datasets)
-        self.location = x_min
 
         tr_volume = tf.reduce_prod(self.upper - self.lower)
         self._step_is_success = y_min < self._y_min - self._kappa * tr_volume
         self.eps = self.eps / self._beta if self._step_is_success else self.eps * self._beta
-        self._update_bounds()
-        self._y_min = y_min
+
+        # Only update the location if the step was successful.
+        if self._step_is_success:
+            self.location = x_min
+            self._y_min = y_min
+
+        self._update_domain()
+
+    @check_shapes(
+        "query_points: [N, D]",
+        "values: [N, 1]",
+        "return[0]: [D]",
+        "return[1]: []",
+    )
+    def get_values_min(
+        self,
+        query_points: TensorType,
+        values: TensorType,
+        num_query_points: Optional[int] = None,
+        in_region_only: bool = True,
+    ) -> Tuple[TensorType, TensorType]:
+        """
+        Calculate the minimum of the region over the given values, returning the query point and
+        value of the minimum. Optionally, only consider query points that are contained in the
+        region.
+
+        :param query_points: The query points corresponding to the values.
+        :param values: The values to find the minimum over.
+        :param num_query_points: The number of latest query points to use for calculating the
+            minimum. If None, all query points are used.
+        :param in_region_only: If True, only consider points contained in the region.
+        :return: The query point and value of the minimum.
+        """
+
+        if num_query_points is None:
+            qps = query_points
+        else:
+            qps = query_points[-num_query_points:]
+
+        if in_region_only:
+            in_tr = self.contains(qps)  # Only consider points in the region.
+            in_tr_obs = tf.where(
+                tf.expand_dims(in_tr, axis=-1),
+                values,
+                tf.constant(np.inf, dtype=values.dtype),
+            )
+        else:
+            in_tr_obs = values  # Consider all points.
+
+        ix = tf.argmin(in_tr_obs)
+        x_min = tf.gather(qps, ix)
+        y_min = tf.gather(in_tr_obs, ix)
+
+        return tf.squeeze(x_min, axis=0), tf.squeeze(y_min)
 
     @check_shapes(
         "return[0]: [D]",
         "return[1]: []",
     )
     def get_dataset_min(
         self, datasets: Optional[Mapping[Tag, Dataset]]
     ) -> Tuple[TensorType, TensorType]:
-        """Calculate the minimum of the box using the given dataset."""
+        """
+        Calculate the minimum of the region using the given dataset, returning the query point and
+        value of the minimum.
+
+        The default implementation supports a single objective dataset only. This can be
+        overridden by subclasses to support multiple datasets.
+
+        :param datasets: The datasets to use for finding the minimum.
+        :return: The query point and value of the minimum.
+        """
+
         if (
             datasets is None
             or len(datasets) != 1
             or LocalizedTag.from_tag(next(iter(datasets))).global_tag != OBJECTIVE
         ):
             raise ValueError("""a single OBJECTIVE dataset must be provided""")
         dataset = next(iter(datasets.values()))
+        return self.get_values_min(dataset.query_points, dataset.observations, in_region_only=True)
 
-        in_tr = self.contains(dataset.query_points)
-        in_tr_obs = tf.where(
-            tf.expand_dims(in_tr, axis=-1),
-            dataset.observations,
-            tf.constant(np.inf, dtype=dataset.observations.dtype),
-        )
-        ix = tf.argmin(in_tr_obs)
-        x_min = tf.gather(dataset.query_points, ix)
-        y_min = tf.gather(in_tr_obs, ix)
 
-        return tf.squeeze(x_min, axis=0), tf.squeeze(y_min)
+class UpdatableTrustRegionBox(Box, UpdatableTrustRegion):
+    """
+    A simple updatable box search space with a center location and an associated global search
+    space.
+    """
+
+    def __init__(
+        self,
+        global_search_space: Box,
+        region_index: Optional[int] = None,
+        input_active_dims: Optional[Union[slice, Sequence[int]]] = None,
+    ):
+        """
+        :param global_search_space: The global search space this search space lives in.
+        :param region_index: The index of the region in a multi-region search space. This is used to
+            identify the local models and datasets to use for acquisition. If `None`, the
+            global models and datasets are used.
+        :param input_active_dims: The active dimensions of the input space, either a slice or list
+            of indices into the columns of the space. If `None`, all dimensions are active.
+        """
+        Box.__init__(self, global_search_space.lower, global_search_space.upper)
+        UpdatableTrustRegion.__init__(self, region_index, input_active_dims)
+        self._global_search_space = global_search_space
+
+    @property
+    def location(self) -> TensorType:
+        return self._location
+
+    @location.setter
+    def location(self, location: TensorType) -> None:
+        self._location = location
+
+    @property
+    def global_search_space(self) -> Box:
+        return self._global_search_space
+
+    def _get_bounds_within_distance(self, eps: TensorType) -> Tuple[TensorType, TensorType]:
+        # Helper method to get the box bounds within a distance `eps` of the region location.
+        lower = tf.reduce_max([self.global_search_space.lower, self.location - eps], axis=0)
+        upper = tf.reduce_min([self.global_search_space.upper, self.location + eps], axis=0)
+        return lower, upper
+
+
+class SingleObjectiveTrustRegionBox(UpdatableTrustRegionBox, HypercubeTrustRegion):
+    """
+    An updatable continuous trust region that defines a box region in the global search space.
+    The region is updated based on the best point found in the region.
+    """
+
+    def __init__(
+        self,
+        global_search_space: Box,
+        beta: float = 0.7,
+        kappa: float = 1e-4,
+        zeta: float = 0.5,
+        min_eps: float = 1e-2,
+        region_index: Optional[int] = None,
+        input_active_dims: Optional[Union[slice, Sequence[int]]] = None,
+    ):
+        """
+        Calculates the bounds of the box from the location/center and global bounds.
+
+        :param global_search_space: The global search space this search space lives in.
+        :param beta: The inverse of the trust region contraction factor.
+        :param kappa: Scales the threshold for the minimal improvement required for a step to be
+            considered a success.
+        :param zeta: The initial size of the trust region is ``zeta`` times the size of the global
+            search space.
+        :param min_eps: The minimal size of the search space. If the size of the search space is
+            smaller than this, the search space is reinitialized.
+        :param region_index: The index of the region in a multi-region search space. This is used to
+            identify the local models and datasets to use for acquisition. If `None`, the
+            global models and datasets are used.
+        :param input_active_dims: The active dimensions of the input space, either a slice or list
+            of indices into the columns of the space. If `None`, all dimensions are active.
+        """
+        UpdatableTrustRegionBox.__init__(self, global_search_space, region_index, input_active_dims)
+        HypercubeTrustRegion.__init__(self, beta, kappa, zeta, min_eps)
+
+    def _update_domain(self) -> None:
+        self._lower, self._upper = self._get_bounds_within_distance(self.eps)
 
 
 class BatchTrustRegionBox(BatchTrustRegion[ProbabilisticModelType, UpdatableTrustRegionBox]):
     """
     Implements the :class:`BatchTrustRegion` *trust region* acquisition rule for box regions.
     This is intended to be used for single-objective optimization with batching.
     """
@@ -1679,14 +1832,17 @@
             # Note: the reason we don't create the default subspaces in `__init__` is because we
             # don't have the global search space at that point.
             if isinstance(self._rule, EfficientGlobalOptimization):
                 num_query_points = self._rule._num_query_points
             else:
                 num_query_points = 1
 
+            assert isinstance(
+                search_space, Box
+            ), f"search space should be a Box, got {type(search_space)}"
             init_subspaces: Tuple[UpdatableTrustRegionBox, ...] = tuple(
                 SingleObjectiveTrustRegionBox(search_space) for _ in range(num_query_points)
             )
             self._subspaces = init_subspaces
             for index, subspace in enumerate(self._subspaces):
                 subspace.region_index = index  # Override the index.
             self._tags = tuple(str(index) for index in range(self.num_local_datasets))
@@ -1734,15 +1890,15 @@
     **Note:** The acquisition search space will never extend beyond the boundary of the
     ``global_search_space``. For a local search, the actual search space will be the
     intersection of the trust region and ``global_search_space``.
     """
 
     def __init__(
         self,
-        global_search_space: SearchSpace,
+        global_search_space: Box,
         beta: float = 0.7,
         kappa: float = 1e-4,
         min_eps: float = 1e-2,
         region_index: Optional[int] = None,
         input_active_dims: Optional[Union[slice, Sequence[int]]] = None,
     ):
         self._is_global = False
@@ -1763,38 +1919,39 @@
     @eps.setter
     def eps(self, eps: TensorType) -> None:
         """Set the size of the search space."""
         # Don't change the eps in global mode.
         if not self._is_global:
             self._eps = eps
 
-    def _update_bounds(self) -> None:
+    def _update_domain(self) -> None:
         self._is_global = self._step_is_success or not self._is_global
 
         # Use global bounds in global mode.
         if self._is_global:
             self._lower = self.global_search_space.lower
             self._upper = self.global_search_space.upper
         else:
-            super()._update_bounds()
+            super()._update_domain()
 
     def initialize(
         self,
         models: Optional[Mapping[Tag, ProbabilisticModelType]] = None,
         datasets: Optional[Mapping[Tag, Dataset]] = None,
+        location_candidate: Optional[TensorType] = None,
     ) -> None:
         # `True` if the search space is global, else `False` if it is local.
         # May be a scalar boolean `TensorType` instead of a `bool`.
         #
         # Start in global mode at construction time. Use local mode for subsequent
-        # re-initializations. Note the calls to `_update_bounds` switch the mode, so the values
+        # re-initializations. Note the calls to `_update_domain` switch the mode, so the values
         # here are inverted.
         self._is_global = self._initialized
 
-        super().initialize(models, datasets)
+        super().initialize(models, datasets, location_candidate=location_candidate)
 
     def get_datasets_filter_mask(
         self, datasets: Optional[Mapping[Tag, Dataset]]
     ) -> Optional[Mapping[Tag, tf.Tensor]]:
         # Only select the region datasets for filtering. Don't directly filter the global dataset.
         assert (
             self.region_index is not None
@@ -1811,37 +1968,32 @@
                 if LocalizedTag.from_tag(tag).local_index == self.region_index
             }
 
     @inherit_check_shapes
     def get_dataset_min(
         self, datasets: Optional[Mapping[Tag, Dataset]]
     ) -> Tuple[TensorType, TensorType]:
-        """Calculate the minimum of the box using the given dataset."""
         if (
             datasets is None
             or len(datasets) != 1
             or LocalizedTag.from_tag(next(iter(datasets))).global_tag != OBJECTIVE
         ):
             raise ValueError("""a single OBJECTIVE dataset must be provided""")
         dataset = next(iter(datasets.values()))
 
         # Always return the global minimum.
-        ix = tf.argmin(dataset.observations)
-        x_min = tf.gather(dataset.query_points, ix)
-        y_min = tf.gather(dataset.observations, ix)
-
-        return tf.squeeze(x_min, axis=0), tf.squeeze(y_min)
+        return self.get_values_min(dataset.query_points, dataset.observations, in_region_only=False)
 
 
 class TURBOBox(UpdatableTrustRegionBox):
     """Implements the TURBO algorithm as detailed in :cite:`eriksson2019scalable`."""
 
     def __init__(
         self,
-        global_search_space: SearchSpace,
+        global_search_space: Box,
         L_min: Optional[float] = None,
         L_init: Optional[float] = None,
         L_max: Optional[float] = None,
         success_tolerance: int = 3,
         failure_tolerance: Optional[int] = None,
         region_index: Optional[int] = None,
         input_active_dims: Optional[Union[slice, Sequence[int]]] = None,
@@ -1858,14 +2010,15 @@
         :param region_index: The index of the region in a multi-region search space. This is used to
             identify the local models and datasets to use for acquisition. If `None`, the
             global models and datasets are used.
         :param input_active_dims: The active dimensions of the input space, either a slice or list
             of indices into the columns of the space. If `None`, all dimensions are active.
         """
         super().__init__(global_search_space, region_index, input_active_dims)
+        self._init_location()
 
         search_space_max_width = tf.reduce_max(
             global_search_space.upper - global_search_space.lower
         )
         if L_min is None:
             L_min = (0.5**7) * search_space_max_width
         if L_init is None:
@@ -1900,15 +2053,15 @@
             raise ValueError(
                 f"success tolerance must be an integer greater than 0, got {self.failure_tolerance}"
             )
 
         self.y_min = np.inf
         # Initialise to the full global search space size.
         self.tr_width = global_search_space.upper - global_search_space.lower
-        self._update_bounds()
+        self._update_domain()
 
     def _set_tr_width(self, models: Optional[Mapping[Tag, ProbabilisticModelType]] = None) -> None:
         # Set the width of the trust region based on the local model.
         if (
             models is None
             or len(models) != 1
             or LocalizedTag.from_tag(next(iter(models))).global_tag != OBJECTIVE
@@ -1921,23 +2074,23 @@
 
         lengthscales = (
             model.get_kernel().lengthscales
         )  # stretch region according to model lengthscales
 
         # Select the input lengthscales that are active for this region.
         if tf.size(lengthscales) > 1:
-            lengthscales = self.with_input_active_dims(lengthscales)
+            lengthscales = self.with_input_active_dims(tf.convert_to_tensor(lengthscales))
 
         self.tr_width = (
             lengthscales
             * self.L
             / tf.reduce_prod(lengthscales) ** (1.0 / self.global_search_space.lower.shape[-1])
         )  # keep volume fixed
 
-    def _update_bounds(self) -> None:
+    def _update_domain(self) -> None:
         self._lower = tf.reduce_max(
             [self.global_search_space.lower, self.location - self.tr_width / 2.0], axis=0
         )
         self._upper = tf.reduce_min(
             [self.global_search_space.upper, self.location + self.tr_width / 2.0], axis=0
         )
 
@@ -1951,15 +2104,15 @@
         x_min, self.y_min = self.get_dataset_min(datasets)
         self.location: TensorType = x_min
 
         self.L, self.failure_counter, self.success_counter = self.L_init, 0, 0
 
         models = self.select_in_region(models)
         self._set_tr_width(models)
-        self._update_bounds()
+        self._update_domain()
         self._initialized = True
 
     def update(
         self,
         models: Optional[Mapping[Tag, ProbabilisticModelType]] = None,
         datasets: Optional[Mapping[Tag, Dataset]] = None,
     ) -> None:
@@ -1985,15 +2138,15 @@
 
         self.L = tf.minimum(self.L, self.L_max)
         if self.L < self.L_min:  # if gets too small then start again
             self.L, self.failure_counter, self.success_counter = self.L_init, 0, 0
 
         models = self.select_in_region(models)
         self._set_tr_width(models)
-        self._update_bounds()
+        self._update_domain()
 
     @check_shapes(
         "return[0]: [D]",
         "return[1]: []",
     )
     def get_dataset_min(
         self, datasets: Optional[Mapping[Tag, Dataset]]
@@ -2035,23 +2188,55 @@
         """
         # Ensure global_points is a copied tensor, in case a variable is passed in.
         DiscreteSearchSpace.__init__(self, tf.constant(global_search_space.points))
         UpdatableTrustRegion.__init__(self, region_index, input_active_dims)
         self._global_search_space = global_search_space
 
     @property
-    @abstractmethod
     def location(self) -> TensorType:
-        """Center of the region."""
+        return tf.reshape(tf.gather(self.global_search_space.points, self._location_ix), (-1,))
+
+    @location.setter
+    def location(self, location: TensorType) -> None:
+        # Keep the index of the location in the global search space, instead of directly storing
+        # the location.
+        location_ix = tf.where(tf.reduce_all(self.global_search_space.points == location, axis=-1))
+        if tf.size(location_ix) == 0:
+            raise ValueError(f"location {location} not found in the global search space")
+        self._location_ix = tf.squeeze(location_ix, axis=-1)
 
     @property
     def global_search_space(self) -> DiscreteSearchSpace:
-        """The global space this search space lives in."""
         return self._global_search_space
 
+    def _compute_global_distances(self) -> TensorType:
+        # Helper method to compute and return pairwise distances along each axis in the
+        # global search space.
+        points = self.global_search_space.points
+        return tf.abs(
+            tf.expand_dims(points, -2) - tf.expand_dims(points, -3)
+        )  # [num_points, num_points, D]
+
+    def _get_points_within_distance(
+        self, global_distances: TensorType, eps: TensorType
+    ) -> TensorType:
+        # Helper method to return subset of global points within a given `eps` distance of the
+        # region location. Takes the precomputed pairwise distances tensor and the trust region
+        # size `eps`.
+
+        # Indices of the neighbors within the trust region.
+        neighbors_mask = tf.reduce_all(
+            tf.gather(global_distances, self._location_ix) <= eps, axis=-1
+        )
+        neighbors_mask = tf.reshape(neighbors_mask, (-1,))
+        neighbor_ixs = tf.where(neighbors_mask)
+        neighbor_ixs = tf.squeeze(neighbor_ixs, axis=-1)
+        # Points within the trust region (including the location point).
+        return tf.gather(self.global_search_space.points, neighbor_ixs)
+
 
 class FixedPointTrustRegionDiscrete(UpdatableTrustRegionDiscrete):
     """
     A discrete trust region with a fixed point location that does not change across active learning
     steps. The fixed point is selected at random from the global (discrete) search space at
     initialization time.
     """
@@ -2060,40 +2245,35 @@
         self,
         global_search_space: DiscreteSearchSpace,
         region_index: Optional[int] = None,
         input_active_dims: Optional[Union[slice, Sequence[int]]] = None,
     ):
         super().__init__(global_search_space, region_index, input_active_dims)
         # Random initial point from the global search space.
-        self._points = self.global_search_space.sample(1)
-
-    @property
-    def location(self) -> TensorType:
-        """The location point of the region."""
-        return tf.squeeze(self._points, axis=0)  # Only one point.
+        self._init_location()
 
     def initialize(
         self,
         models: Optional[Mapping[Tag, ProbabilisticModelType]] = None,
         datasets: Optional[Mapping[Tag, Dataset]] = None,
     ) -> None:
         # Pick a random point from the global search space.
-        self._points = self.global_search_space.sample(1)
+        self._init_location(models, datasets)
         self._initialized = True
 
     def update(
         self,
         models: Optional[Mapping[Tag, ProbabilisticModelType]] = None,
         datasets: Optional[Mapping[Tag, Dataset]] = None,
     ) -> None:
         # Keep the point fixed, no updates needed.
         pass
 
 
-class SingleObjectiveTrustRegionDiscrete(UpdatableTrustRegionDiscrete):
+class SingleObjectiveTrustRegionDiscrete(UpdatableTrustRegionDiscrete, HypercubeTrustRegion):
     """
     An updatable discrete trust region that maintains a set of neighboring points around a
     single location point, allowing for local exploration of the search space. The region is
     updated based on the best point found in the region.
 
     This trust region is designed for discrete numerical variables. As it uses axis-aligned
     Euclidean distance to determine the neighbors within the region, it is not suitable for
@@ -2130,179 +2310,39 @@
             smaller than this, the search space is reinitialized.
         :param region_index: The index of the region in a multi-region search space. This is used to
             identify the local models and datasets to use for acquisition. If `None`, the
             global models and datasets are used.
         :param input_active_dims: The active dimensions of the input space, either a slice or list
             of indices into the columns of the space. If `None`, all dimensions are active.
         """
-        super().__init__(global_search_space, region_index, input_active_dims)
-        self._beta = beta
-        self._kappa = kappa
-        self._zeta = zeta
-        self._min_eps = min_eps
-        self._step_is_success = False
-        self._init_location()
-        self._compute_global_distances()
-        self._init_eps()
-        self._update_neighbors()
-        self._y_min = np.inf
-
-    @property
-    def requires_initialization(self) -> bool:
-        """
-        Return `True` if the search space needs to be initialized, and `False` otherwise.
-
-        If uninitialized, or the size of the region is less than the minimum size, re-initialize
-        the region.
-        """
-        return not self._initialized or tf.reduce_any(self.eps < self._min_eps)
-
-    @property
-    def location(self) -> TensorType:
-        """Center point of the region."""
-        return tf.reshape(tf.gather(self.global_search_space.points, self._location_ix), (-1,))
-
-    def _init_location(self) -> None:
-        # Random initial location index from the global search space.
-        self._location_ix = tf.random.categorical(
-            tf.ones(
-                (
-                    1,
-                    self.global_search_space.points.shape[0],
-                )
-            ),
-            1,
-        )[0]
-
-    def _init_eps(self) -> None:
-        self.eps = self._zeta * (self.global_search_space.upper - self.global_search_space.lower)
-
-    def _compute_global_distances(self) -> None:
-        # Pairwise distances along each axis in the global search space.
-        points = self.global_search_space.points
-        self._global_distances = tf.abs(
-            tf.expand_dims(points, -2) - tf.expand_dims(points, -3)
-        )  # [num_points, num_points, D]
-
-    def _update_neighbors(self) -> None:
-        # Indices of the neighbors within the trust region.
-        neighbors_mask = tf.reduce_all(
-            tf.gather(self._global_distances, self._location_ix) <= self.eps, axis=-1
-        )
-        neighbors_mask = tf.reshape(neighbors_mask, (-1,))
-        self._neighbor_ixs = tf.where(neighbors_mask)
-        self._neighbor_ixs = tf.squeeze(self._neighbor_ixs, axis=-1)
-        # Points within the trust region (including the location point).
-        self._points = tf.gather(self.global_search_space.points, self._neighbor_ixs)
-
-    def initialize(
-        self,
-        models: Optional[Mapping[Tag, ProbabilisticModelType]] = None,
-        datasets: Optional[Mapping[Tag, Dataset]] = None,
-    ) -> None:
-        """
-        Initialize the region by sampling a location from the global search space and selecting
-        the neighboring points within the trust region.
-
-        :param models: The model for each tag.
-        :param datasets: The dataset for each tag.
-        """
-
-        datasets = self.select_in_region(datasets)
-        self._init_location()
-        self._step_is_success = False
-        self._init_eps()
-        self._update_neighbors()
-        _, self._y_min = self.get_dataset_min(datasets)
-        self._initialized = True
-
-    def update(
-        self,
-        models: Optional[Mapping[Tag, ProbabilisticModelType]] = None,
-        datasets: Optional[Mapping[Tag, Dataset]] = None,
-    ) -> None:
-        """
-        Update this region, including location and neighbors, using the given dataset.
-
-        If the new optimum improves over the previous optimum by some threshold (that scales
-        linearly with ``kappa``), the previous acquisition is considered successful.
-
-        If the previous acquisition was successful, the size is increased by a factor
-        ``1 / beta``. Conversely, if it was unsuccessful, the size is reduced by the factor
-        ``beta``.
-
-        :param models: The model for each tag.
-        :param datasets: The dataset for each tag.
-        """
-
-        datasets = self.select_in_region(datasets)
-        x_min, y_min = self.get_dataset_min(datasets)
-        self._location_ix = tf.where(
-            tf.reduce_all(self.global_search_space.points == x_min, axis=-1)
-        )
-        self._location_ix = tf.squeeze(self._location_ix, axis=-1)
-
-        tr_volume = tf.reduce_prod(self.upper - self.lower)
-        self._step_is_success = y_min < self._y_min - self._kappa * tr_volume
-        self.eps = self.eps / self._beta if self._step_is_success else self.eps * self._beta
-        self._update_neighbors()
-        self._y_min = y_min
-
-    @check_shapes(
-        "return[0]: [D]",
-        "return[1]: []",
-    )
-    def get_dataset_min(
-        self, datasets: Optional[Mapping[Tag, Dataset]]
-    ) -> Tuple[TensorType, TensorType]:
-        """
-        Calculate the minimum of the region using the given dataset.
-
-        :param datasets: The datasets to use for finding the minimum.
-        """
-        if (
-            datasets is None
-            or len(datasets) != 1
-            or LocalizedTag.from_tag(next(iter(datasets))).global_tag != OBJECTIVE
-        ):
-            raise ValueError("""a single OBJECTIVE dataset must be provided""")
-        dataset = next(iter(datasets.values()))
-
-        in_tr = self.contains(dataset.query_points)
-        in_tr_obs = tf.where(
-            tf.expand_dims(in_tr, axis=-1),
-            dataset.observations,
-            tf.constant(np.inf, dtype=dataset.observations.dtype),
+        UpdatableTrustRegionDiscrete.__init__(
+            self, global_search_space, region_index, input_active_dims
         )
-        ix = tf.argmin(in_tr_obs)
-        x_min = tf.gather(dataset.query_points, ix)
-        y_min = tf.gather(in_tr_obs, ix)
-
-        return tf.squeeze(x_min, axis=0), tf.squeeze(y_min)
-
+        # Need to compute the distances before initializing `HypercubeTrustRegion` as it
+        # uses the distances to set the initial location and update the bounds.
+        self._global_distances = self._compute_global_distances()
+        HypercubeTrustRegion.__init__(self, beta, kappa, zeta, min_eps)
 
-UpdatableTrustRegionWithGlobalSearchSpace = Union[
-    UpdatableTrustRegionBox, UpdatableTrustRegionDiscrete
-]
-"""A type alias for updatable trust regions with a global search space."""
+    def _update_domain(self) -> None:
+        self._points = self._get_points_within_distance(self._global_distances, self.eps)
 
 
 class UpdatableTrustRegionProduct(TaggedProductSearchSpace, UpdatableTrustRegion):
     """
     An updatable mixed search space that is the product of multiple updatable trust sub-regions.
 
     This is useful for combining different types of search spaces, such as continuous and discrete,
     to form a mixed search space for trust region acquisition rules.
 
     Note: the dtype of all the component search spaces must be the same.
     """
 
     def __init__(
         self,
-        regions: Sequence[UpdatableTrustRegionWithGlobalSearchSpace],
+        regions: Sequence[UpdatableTrustRegion],
         tags: Optional[Sequence[str]] = None,
         region_index: Optional[int] = None,
     ):
         """
         :param regions: The trust sub-regions to be combined to create a product trust region.
         :param tags: An optional list of tags giving the unique identifiers of the region's
             sub-regions.
@@ -2370,15 +2410,15 @@
         self._region_index = region_index
         # Override the region index for each sub-region. These would either already be set to the
         # same value (assert in __init__), or None.
         for region in self.regions.values():
             region.region_index = region_index
 
     @property
-    def regions(self) -> Mapping[str, UpdatableTrustRegionWithGlobalSearchSpace]:
+    def regions(self) -> Mapping[str, UpdatableTrustRegion]:
         """The sub-regions of the product trust region."""
         _regions = {}
         for tag, region in self._spaces.items():
             assert isinstance(region, (UpdatableTrustRegionBox, UpdatableTrustRegionDiscrete))
             _regions[tag] = region
         return _regions
 
@@ -2386,14 +2426,18 @@
     def location(self) -> TensorType:
         """
         The location of the product trust region, concatenated from the locations of the
         sub-regions.
         """
         return tf.concat([region.location for region in self.regions.values()], axis=-1)
 
+    @location.setter
+    def location(self, location: TensorType) -> None:
+        raise NotImplementedError("setting the location of a product region is not supported")
+
     @property
     def global_search_space(self) -> TaggedProductSearchSpace:
         """The global search space this search space lives in."""
         return self._global_search_space
 
     def initialize(
         self,
@@ -2464,29 +2508,31 @@
             # Note: the reason we don't create the default subspaces in `__init__` is because we
             # don't have the global search space at that point.
             if isinstance(self._rule, EfficientGlobalOptimization):
                 num_query_points = self._rule._num_query_points
             else:
                 num_query_points = 1
 
-            def create_subregions() -> Sequence[UpdatableTrustRegionWithGlobalSearchSpace]:
+            def create_subregions() -> Sequence[UpdatableTrustRegion]:
                 # Take a global product search space and convert each of its subspaces to an
                 # updatable trust sub-region. These sub-regions are then used to create a
                 # trust region product.
                 assert isinstance(
                     search_space, TaggedProductSearchSpace
                 ), "search_space should be a TaggedProductSearchSpace"
 
-                subregions: List[UpdatableTrustRegionWithGlobalSearchSpace] = []
+                subregions: List[UpdatableTrustRegion] = []
                 for tag in search_space.subspace_tags:
                     subspace = search_space.get_subspace(tag)
                     if isinstance(subspace, DiscreteSearchSpace):
                         subregions.append(FixedPointTrustRegionDiscrete(subspace))
-                    else:
+                    elif isinstance(subspace, Box):
                         subregions.append(SingleObjectiveTrustRegionBox(subspace))
+                    else:
+                        raise ValueError(f"unsupported search space type: {type(subspace)}")
                 return subregions
 
             init_subspaces: Tuple[UpdatableTrustRegionProduct, ...] = tuple(
                 UpdatableTrustRegionProduct(create_subregions()) for _ in range(num_query_points)
             )
             self._subspaces = init_subspaces
             for index, subspace in enumerate(self._subspaces):
```

### Comparing `trieste-3.1.0/trieste/acquisition/sampler.py` & `trieste-3.2.0/trieste/acquisition/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/acquisition/utils.py` & `trieste-3.2.0/trieste/acquisition/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 import functools
-from typing import Dict, Mapping, Tuple, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Union
 
 import tensorflow as tf
 from check_shapes import check_shapes
 
 from ..data import Dataset
 from ..models import ProbabilisticModelType
 from ..observer import OBJECTIVE
@@ -158,31 +158,53 @@
     """
     return {LocalizedTag(key, i): copy.deepcopy(global_model) for i in range(num_local_models)}
 
 
 def with_local_datasets(
     datasets: Mapping[Tag, Dataset],
     num_local_datasets: int,
+    local_dataset_indices: Optional[Sequence[TensorType]] = None,
 ) -> Dict[Tag, Dataset]:
     """
-    Helper method to add local datasets if they do not already exist, by copying global datasets.
+    Helper method to add local datasets if they do not already exist, by copying global datasets
+    or a subset thereof.
 
     :param datasets: The original datasets.
     :param num_local_datasets: The number of local datasets to add per global tag.
+    :param local_dataset_indices: Optional sequence of indices, indicating which parts of
+        the global datasets should be copied. If None then the entire datasets are copied.
     :return: The updated mapping of datasets.
     """
+    if local_dataset_indices is not None and len(local_dataset_indices) != num_local_datasets:
+        raise ValueError(
+            f"local_dataset_indices should have {num_local_datasets} entries, "
+            f"has {len(local_dataset_indices)}"
+        )
+
     updated_datasets = {}
     for tag in datasets:
         updated_datasets[tag] = datasets[tag]
         ltag = LocalizedTag.from_tag(tag)
         if not ltag.is_local:
             for i in range(num_local_datasets):
                 target_ltag = LocalizedTag(ltag.global_tag, i)
                 if target_ltag not in datasets:
-                    updated_datasets[target_ltag] = datasets[tag]
+                    if local_dataset_indices is None:
+                        updated_datasets[target_ltag] = datasets[tag]
+                    else:
+                        # TODO: use sparse tensors instead
+                        updated_datasets[target_ltag] = Dataset(
+                            query_points=tf.gather(
+                                datasets[tag].query_points, local_dataset_indices[i]
+                            ),
+                            observations=tf.gather(
+                                datasets[tag].observations, local_dataset_indices[i]
+                            ),
+                        )
+
     return updated_datasets
 
 
 @check_shapes(
     "points: [n_points, ...]",
     "return: [n_points]",
 )
```

### Comparing `trieste-3.1.0/trieste/ask_tell_optimization.py` & `trieste-3.2.0/trieste/ask_tell_optimization.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 """
 
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from copy import deepcopy
-from typing import Dict, Generic, Mapping, Type, TypeVar, cast, overload
+from dataclasses import dataclass
+from typing import Dict, Generic, Mapping, Optional, Sequence, Type, TypeVar, cast, overload
+
+import tensorflow as tf
 
 from .models.utils import optimize_model_and_save_result
 
 try:
     import pandas as pd
 except ModuleNotFoundError:
     pd = None
@@ -65,14 +68,29 @@
     "ProbabilisticModelType", bound=ProbabilisticModel, contravariant=True
 )
 """ Contravariant type variable bound to :class:`ProbabilisticModel`. """
 
 AskTellOptimizerType = TypeVar("AskTellOptimizerType")
 
 
+@dataclass(frozen=True)
+class AskTellOptimizerState(Generic[StateType, ProbabilisticModelType]):
+    """
+    Internal state for an Ask/Tell optimizer. This can be obtained using the optimizer's
+    `to_state` method, and can be used to initialise a new instance of the optimizer.
+    """
+
+    record: Record[StateType, ProbabilisticModelType]
+    """ A record of the current state of the optimization. """
+
+    local_data_ixs: Optional[Sequence[TensorType]]
+    """ Indices to the local data, for LocalDatasetsAcquisitionRule rules
+    when `track_data` is `False`. """
+
+
 class AskTellOptimizerABC(ABC, Generic[SearchSpaceType, ProbabilisticModelType]):
     """
     This class provides Ask/Tell optimization interface. It is designed for those use cases
     when control of the optimization loop by Trieste is impossible or not desirable.
     For the default use case with model training, refer to :class:`AskTellOptimizer`.
     For more details about the Bayesian Optimization routine, refer to :class:`BayesianOptimizer`.
     """
@@ -81,26 +99,30 @@
     def __init__(
         self,
         search_space: SearchSpaceType,
         datasets: Mapping[Tag, Dataset],
         models: Mapping[Tag, ProbabilisticModelType],
         *,
         fit_model: bool = True,
+        track_data: bool = True,
+        local_data_ixs: Optional[Sequence[TensorType]] = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
         search_space: SearchSpaceType,
         datasets: Mapping[Tag, Dataset],
         models: Mapping[Tag, ProbabilisticModelType],
         acquisition_rule: AcquisitionRule[TensorType, SearchSpaceType, ProbabilisticModelType],
         *,
         fit_model: bool = True,
+        track_data: bool = True,
+        local_data_ixs: Optional[Sequence[TensorType]] = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
         search_space: SearchSpaceType,
@@ -108,37 +130,43 @@
         models: Mapping[Tag, ProbabilisticModelType],
         acquisition_rule: AcquisitionRule[
             State[StateType | None, TensorType], SearchSpaceType, ProbabilisticModelType
         ],
         acquisition_state: StateType | None,
         *,
         fit_model: bool = True,
+        track_data: bool = True,
+        local_data_ixs: Optional[Sequence[TensorType]] = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
         search_space: SearchSpaceType,
         datasets: Dataset,
         models: ProbabilisticModelType,
         *,
         fit_model: bool = True,
+        track_data: bool = True,
+        local_data_ixs: Optional[Sequence[TensorType]] = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
         search_space: SearchSpaceType,
         datasets: Dataset,
         models: ProbabilisticModelType,
         acquisition_rule: AcquisitionRule[TensorType, SearchSpaceType, ProbabilisticModelType],
         *,
         fit_model: bool = True,
+        track_data: bool = True,
+        local_data_ixs: Optional[Sequence[TensorType]] = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
         search_space: SearchSpaceType,
@@ -146,14 +174,16 @@
         models: ProbabilisticModelType,
         acquisition_rule: AcquisitionRule[
             State[StateType | None, TensorType], SearchSpaceType, ProbabilisticModelType
         ],
         acquisition_state: StateType | None = None,
         *,
         fit_model: bool = True,
+        track_data: bool = True,
+        local_data_ixs: Optional[Sequence[TensorType]] = None,
     ):
         ...
 
     def __init__(
         self,
         search_space: SearchSpaceType,
         datasets: Mapping[Tag, Dataset] | Dataset,
@@ -163,42 +193,47 @@
             SearchSpaceType,
             ProbabilisticModelType,
         ]
         | None = None,
         acquisition_state: StateType | None = None,
         *,
         fit_model: bool = True,
+        track_data: bool = True,
+        local_data_ixs: Optional[Sequence[TensorType]] = None,
     ):
         """
         :param search_space: The space over which to search for the next query point.
         :param datasets: Already observed input-output pairs for each tag.
         :param models: The model to use for each :class:`~trieste.data.Dataset` in
             ``datasets``.
         :param acquisition_rule: The acquisition rule, which defines how to search for a new point
             on each optimization step. Defaults to
             :class:`~trieste.acquisition.rule.EfficientGlobalOptimization` with default
             arguments. Note that if the default is used, this implies the tags must be
             `OBJECTIVE` and the search space can be any :class:`~trieste.space.SearchSpace`.
         :param acquisition_state: The optional acquisition state for stateful acquisitions.
         :param fit_model: If `True` (default), models passed in will be optimized on the given data.
             If `False`, the models are assumed to be optimized already.
+        :param track_data: If `True` (default), the optimizer will track the changing
+            datasets via a local copy. If `False`, it will infer new datasets from
+            updates to the global datasets (optionally using `local_data_ixs` and indices passed
+            in to `tell`).
+        :param local_data_ixs: Indices to the local data in the initial datasets. If unspecified,
+            assumes that the initial datasets are global.
         :raise ValueError: If any of the following are true:
             - the keys in ``datasets`` and ``models`` do not match
             - ``datasets`` or ``models`` are empty
             - default acquisition is used but incompatible with other inputs
         """
         self._search_space = search_space
         self._acquisition_state = acquisition_state
 
         if not datasets or not models:
             raise ValueError("dicts of datasets and models must be populated.")
 
-        # Copy the dataset so we don't change the one provided by the user.
-        datasets = deepcopy(datasets)
-
         if isinstance(datasets, Dataset):
             datasets = {OBJECTIVE: datasets}
         if not isinstance(models, Mapping):
             models = {OBJECTIVE: models}
 
         # reassure the type checker that everything is tagged
         datasets = cast(Dict[Tag, Dataset], datasets)
@@ -212,14 +247,15 @@
             raise ValueError(
                 f"datasets and models should contain the same keys. Got {datasets_keys} and"
                 f" {models_keys} respectively."
             )
 
         self._datasets = datasets
         self._models = models
+        self.track_data = track_data
 
         self._query_plot_dfs: dict[int, pd.DataFrame] = {}
         self._observation_plot_dfs = observation_plot_init(self._datasets)
 
         if acquisition_rule is None:
             if self._datasets.keys() != {OBJECTIVE}:
                 raise ValueError(
@@ -230,28 +266,33 @@
             self._acquisition_rule = cast(
                 AcquisitionRule[TensorType, SearchSpaceType, ProbabilisticModelType],
                 EfficientGlobalOptimization(),
             )
         else:
             self._acquisition_rule = acquisition_rule
 
-        # In order to support local datasets, account for the case where there may be an initial
-        # dataset that is not tagged per region. In this case, only the global dataset will
-        # exist in datasets. We want to copy this initial dataset to all the regions.
-        # Copy the global dataset if the local version for the subspace is not available.
-        #
-        # Only applies to a subset of acquisition rules, i.e. ones that have subspaces and
-        # hence use local datasets.
         if isinstance(self._acquisition_rule, LocalDatasetsAcquisitionRule):
-            self._datasets = with_local_datasets(
-                self._datasets, self._acquisition_rule.num_local_datasets
-            )
-        self._filtered_datasets = self._acquisition_rule.filter_datasets(
-            self._models, self._datasets
-        )
+            # In order to support local datasets, account for the case where there may be an initial
+            # dataset that is not tagged per region. In this case, only the global dataset will
+            # exist in datasets. We want to copy this initial dataset to all the regions.
+            num_local_datasets = self._acquisition_rule.num_local_datasets
+            if self.track_data:
+                datasets = self._datasets = with_local_datasets(self._datasets, num_local_datasets)
+            else:
+                self._dataset_len = self.dataset_len(self._datasets)
+                if local_data_ixs is not None:
+                    self._dataset_ixs = list(local_data_ixs)
+                else:
+                    self._dataset_ixs = [
+                        tf.range(self._dataset_len) for _ in range(num_local_datasets)
+                    ]
+                datasets = with_local_datasets(
+                    self._datasets, num_local_datasets, self._dataset_ixs
+                )
+        self._filtered_datasets = self._acquisition_rule.filter_datasets(self._models, datasets)
 
         if fit_model:
             with Timer() as initial_model_fitting_timer:
                 for tag, model in self._models.items():
                     # Prefer local dataset if available.
                     tags = [tag, LocalizedTag.from_tag(tag).global_tag]
                     _, dataset = get_value_for_tag(self._filtered_datasets, *tags)
@@ -290,14 +331,22 @@
         datasets: Mapping[Tag, Dataset] = ignoring_local_tags(self.datasets)
         if len(datasets) == 1:
             return next(iter(datasets.values()))
         else:
             raise ValueError(f"Expected a single dataset, found {len(datasets)}")
 
     @property
+    def local_data_ixs(self) -> Optional[Sequence[TensorType]]:
+        """Indices to the local data. Only stored for LocalDatasetsAcquisitionRule rules
+        when `track_data` is `False`."""
+        if isinstance(self._acquisition_rule, LocalDatasetsAcquisitionRule) and not self.track_data:
+            return self._dataset_ixs
+        return None
+
+    @property
     def models(self) -> Mapping[Tag, ProbabilisticModelType]:
         """The current models."""
         return self._models
 
     @models.setter
     def models(self, models: Mapping[Tag, ProbabilisticModelType]) -> None:
         """Update the current models."""
@@ -332,25 +381,39 @@
 
     @property
     def acquisition_state(self) -> StateType | None:
         """The current acquisition state."""
         return self._acquisition_state
 
     @classmethod
+    def dataset_len(cls, datasets: Mapping[Tag, Dataset]) -> int:
+        """Helper method for inferring the global dataset size."""
+        dataset_lens = {
+            len(dataset.query_points)
+            for tag, dataset in datasets.items()
+            if not LocalizedTag.from_tag(tag).is_local
+        }
+        if len(dataset_lens) != 1:
+            raise ValueError(f"Expected unique global dataset size, got {dataset_lens}")
+        return next(iter(dataset_lens))
+
+    @classmethod
     def from_record(
         cls: Type[AskTellOptimizerType],
         record: Record[StateType, ProbabilisticModelType]
         | FrozenRecord[StateType, ProbabilisticModelType],
         search_space: SearchSpaceType,
         acquisition_rule: AcquisitionRule[
             TensorType | State[StateType | None, TensorType],
             SearchSpaceType,
             ProbabilisticModelType,
         ]
         | None = None,
+        track_data: bool = True,
+        local_data_ixs: Optional[Sequence[TensorType]] = None,
     ) -> AskTellOptimizerType:
         """Creates new :class:`~AskTellOptimizer` instance from provided optimization state.
         Model training isn't triggered upon creation of the instance.
 
         :param record: Optimization state record.
         :param search_space: The space over which to search for the next query point.
         :param acquisition_rule: The acquisition rule, which defines how to search for a new point
@@ -368,14 +431,16 @@
         return cls(  # type: ignore
             search_space,
             record.datasets,
             record.models,
             acquisition_rule=acquisition_rule,
             acquisition_state=record.acquisition_state,
             fit_model=False,
+            track_data=track_data,
+            local_data_ixs=local_data_ixs,
         )
 
     def to_record(self, copy: bool = True) -> Record[StateType, ProbabilisticModelType]:
         """Collects the current state of the optimization, which includes datasets,
         models and acquisition state (if applicable).
 
         :param copy: Whether to return a copy of the current state or the original. Copying
@@ -406,14 +471,30 @@
             is not supported for all model types. However, continuing the optimization will
             modify the original state.
         :return: A :class:`~trieste.data.OptimizationResult` object.
         """
         record: Record[StateType, ProbabilisticModelType] = self.to_record(copy=copy)
         return OptimizationResult(Ok(record), [])
 
+    def to_state(
+        self, copy: bool = False
+    ) -> AskTellOptimizerState[StateType, ProbabilisticModelType]:
+        """Returns the AskTellOptimizer state, comprising the current optimization state
+        alongside any internal AskTellOptimizer state.
+
+        :param copy: Whether to return a copy of the current state or the original. Copying
+            is not supported for all model types. However, continuing the optimization will
+            modify the original state.
+        :return: An :class:`AskTellOptimizerState` object.
+        """
+        return AskTellOptimizerState(
+            record=self.to_record(copy=copy),
+            local_data_ixs=self.local_data_ixs,
+        )
+
     def ask(self) -> TensorType:
         """Suggests a point (or points in batch mode) to observe by optimizing the acquisition
         function. If the acquisition is stateful, its state is saved.
 
         :return: A :class:`TensorType` instance representing suggested point(s).
         """
         # This trick deserves a comment to explain what's going on
@@ -443,51 +524,97 @@
                     query_points,
                     query_point_generation_timer,
                     self._query_plot_dfs,
                 )
 
         return query_points
 
-    def tell(self, new_data: Mapping[Tag, Dataset] | Dataset) -> None:
+    def tell(
+        self,
+        new_data: Mapping[Tag, Dataset] | Dataset,
+        new_data_ixs: Optional[Sequence[TensorType]] = None,
+    ) -> None:
         """Updates optimizer state with new data.
 
-        :param new_data: New observed data.
+        :param new_data: New observed data. If `track_data` is `False`, this refers to all
+            the data.
+        :param new_data_ixs: Indices to the new observed local data, if `track_data` is `False`.
+            If unspecified, inferred from the change in dataset sizes.
         :raise ValueError: If keys in ``new_data`` do not match those in already built dataset.
         """
         if isinstance(new_data, Dataset):
             new_data = {OBJECTIVE: new_data}
 
         # The datasets must have the same keys as the existing datasets. Only exception is if
-        # the existing datasets are all global, in which case the dataset will be appropriately
-        # updated below for the next iteration.
-        datasets_indices = {LocalizedTag.from_tag(tag).local_index for tag in self._datasets.keys()}
-        if self._datasets.keys() != new_data.keys() and datasets_indices != {None}:
+        # the existing datasets are all global and the new data contains local datasets too.
+        if all(LocalizedTag.from_tag(tag).local_index is None for tag in self._datasets.keys()):
+            global_old = {LocalizedTag.from_tag(tag).global_tag for tag in self._datasets.keys()}
+            global_new = {LocalizedTag.from_tag(tag).global_tag for tag in new_data.keys()}
+            if global_new != global_old:
+                raise ValueError(
+                    f"new_data global keys {global_new} doesn't "
+                    f"match dataset global keys {global_old}"
+                )
+        elif self._datasets.keys() != new_data.keys():
             raise ValueError(
                 f"new_data keys {new_data.keys()} doesn't "
                 f"match dataset keys {self._datasets.keys()}"
             )
 
-        for tag, new_dataset in new_data.items():
-            self._datasets[tag] += new_dataset
-        self._filtered_datasets = self._acquisition_rule.filter_datasets(
-            self._models, self._datasets
-        )
+        if self.track_data:
+            for tag, new_dataset in new_data.items():
+                self._datasets[tag] += new_dataset
+            datasets: Mapping[Tag, Dataset] = self._datasets
+        elif not isinstance(self._acquisition_rule, LocalDatasetsAcquisitionRule):
+            datasets = new_data
+        else:
+            num_local_datasets = len(self._dataset_ixs)
+            if new_data_ixs is None:
+                # infer dataset indices from change in dataset sizes
+                new_dataset_len = self.dataset_len(new_data)
+                num_new_points = new_dataset_len - self._dataset_len
+                if num_new_points < 0 or num_new_points % num_local_datasets != 0:
+                    raise ValueError(
+                        "Cannot infer new data points as datasets haven't increased by "
+                        f"a multiple of {num_local_datasets}"
+                    )
+                for i in range(num_local_datasets):
+                    self._dataset_ixs[i] = tf.concat(
+                        [
+                            self._dataset_ixs[i],
+                            tf.range(0, num_new_points, num_local_datasets) + self._dataset_len + i,
+                        ],
+                        -1,
+                    )
+            else:
+                # use explicit indices
+                if len(new_data_ixs) != num_local_datasets:
+                    raise ValueError(
+                        f"new_data_ixs has {len(new_data_ixs)} entries, "
+                        f"expected {num_local_datasets}"
+                    )
+                for i in range(num_local_datasets):
+                    self._dataset_ixs[i] = tf.concat([self._dataset_ixs[i], new_data_ixs[i]], -1)
+            datasets = with_local_datasets(new_data, num_local_datasets, self._dataset_ixs)
+            self._dataset_len = self.dataset_len(datasets)
+
+        self._filtered_datasets = self._acquisition_rule.filter_datasets(self._models, datasets)
 
         with Timer() as model_fitting_timer:
             for tag, model in self._models.items():
                 # Always use the matching dataset to the model. If the model is
                 # local, then the dataset should be too by this stage.
                 dataset = self._filtered_datasets[tag]
                 self.update_model(model, dataset)
 
         summary_writer = logging.get_tensorboard_writer()
         if summary_writer:
             with summary_writer.as_default(step=logging.get_step_number()):
                 write_summary_observations(
-                    self._datasets,
+                    datasets,
                     self._models,
                     new_data,
                     model_fitting_timer,
                     self._observation_plot_dfs,
                 )
```

### Comparing `trieste-3.1.0/trieste/bayesian_optimizer.py` & `trieste-3.2.0/trieste/bayesian_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -995,14 +995,17 @@
     models: Mapping[Tag, ProbabilisticModel],
     tagged_output: Mapping[Tag, TensorType],
     model_fitting_timer: Timer,
     observation_plot_dfs: MutableMapping[Tag, pd.DataFrame],
 ) -> None:
     """Write TensorBoard summary for the current step observations."""
     for tag in models:
+        if tag not in tagged_output:
+            continue
+
         with tf.name_scope(f"{tag}.model"):
             models[tag].log(datasets[tag])
 
         output_dim = tf.shape(tagged_output[tag].observations)[-1]
         for i in tf.range(output_dim):
             suffix = f"[{i}]" if output_dim > 1 else ""
             if tf.size(tagged_output[tag].observations) > 0:
```

### Comparing `trieste-3.1.0/trieste/data.py` & `trieste-3.2.0/trieste/data.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/experimental/plotting/__init__.py` & `trieste-3.2.0/trieste/experimental/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/experimental/plotting/inequality_constraints.py` & `trieste-3.2.0/trieste/experimental/plotting/inequality_constraints.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/experimental/plotting/plotting.py` & `trieste-3.2.0/trieste/experimental/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/experimental/plotting/plotting_plotly.py` & `trieste-3.2.0/trieste/experimental/plotting/plotting_plotly.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/logging.py` & `trieste-3.2.0/trieste/logging.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/__init__.py` & `trieste-3.2.0/trieste/models/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflow/__init__.py` & `trieste-3.2.0/trieste/models/gpflow/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflow/builders.py` & `trieste-3.2.0/trieste/models/gpflow/builders.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflow/inducing_point_selectors.py` & `trieste-3.2.0/trieste/models/gpflow/inducing_point_selectors.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflow/interface.py` & `trieste-3.2.0/trieste/models/gpflow/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflow/models.py` & `trieste-3.2.0/trieste/models/gpflow/models.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflow/optimizer.py` & `trieste-3.2.0/trieste/models/gpflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflow/sampler.py` & `trieste-3.2.0/trieste/models/gpflow/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflow/utils.py` & `trieste-3.2.0/trieste/models/gpflow/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflux/__init__.py` & `trieste-3.2.0/trieste/models/gpflux/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflux/builders.py` & `trieste-3.2.0/trieste/models/gpflux/builders.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflux/interface.py` & `trieste-3.2.0/trieste/models/gpflux/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflux/models.py` & `trieste-3.2.0/trieste/models/gpflux/models.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/gpflux/sampler.py` & `trieste-3.2.0/trieste/models/gpflux/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/interfaces.py` & `trieste-3.2.0/trieste/models/interfaces.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/keras/__init__.py` & `trieste-3.2.0/trieste/models/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/keras/architectures.py` & `trieste-3.2.0/trieste/models/keras/architectures.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/keras/builders.py` & `trieste-3.2.0/trieste/models/keras/builders.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/keras/interface.py` & `trieste-3.2.0/trieste/models/keras/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/keras/models.py` & `trieste-3.2.0/trieste/models/keras/models.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/keras/sampler.py` & `trieste-3.2.0/trieste/models/keras/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/keras/utils.py` & `trieste-3.2.0/trieste/models/keras/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/optimizer.py` & `trieste-3.2.0/trieste/models/optimizer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/models/utils.py` & `trieste-3.2.0/trieste/models/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/objectives/__init__.py` & `trieste-3.2.0/trieste/objectives/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/objectives/multi_objectives.py` & `trieste-3.2.0/trieste/objectives/multi_objectives.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/objectives/multifidelity_objectives.py` & `trieste-3.2.0/trieste/objectives/multifidelity_objectives.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/objectives/single_objectives.py` & `trieste-3.2.0/trieste/objectives/single_objectives.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/objectives/utils.py` & `trieste-3.2.0/trieste/objectives/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/observer.py` & `trieste-3.2.0/trieste/observer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/space.py` & `trieste-3.2.0/trieste/space.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/types.py` & `trieste-3.2.0/trieste/types.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/utils/__init__.py` & `trieste-3.2.0/trieste/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/utils/misc.py` & `trieste-3.2.0/trieste/utils/misc.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste/version.py` & `trieste-3.2.0/trieste/version.py`

 * *Files identical despite different names*

### Comparing `trieste-3.1.0/trieste.egg-info/PKG-INFO` & `trieste-3.2.0/trieste.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trieste
-Version: 3.1.0
+Version: 3.2.0
 Summary: A Bayesian optimization research toolbox built on TensorFlow
 Home-page: https://github.com/secondmind-labs/trieste
 Author: The Trieste contributors
 Author-email: labs@secondmind.ai
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `trieste-3.1.0/trieste.egg-info/SOURCES.txt` & `trieste-3.2.0/trieste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

