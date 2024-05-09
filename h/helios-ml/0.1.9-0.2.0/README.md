# Comparing `tmp/helios_ml-0.1.9.tar.gz` & `tmp/helios_ml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios_ml-0.1.9.tar", last modified: Tue May  7 21:58:01 2024, max compression
+gzip compressed data, was "helios_ml-0.2.0.tar", last modified: Thu May  9 21:15:40 2024, max compression
```

## Comparing `helios_ml-0.1.9.tar` & `helios_ml-0.2.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.875946 helios_ml-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.859946 helios_ml-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-07 21:57:03.000000 helios_ml-0.1.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-07 21:57:03.000000 helios_ml-0.1.9/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 21:57:03.000000 helios_ml-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-07 21:57:03.000000 helios_ml-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-07 21:57:03.000000 helios_ml-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-07 21:58:01.875946 helios_ml-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-07 21:57:03.000000 helios_ml-0.1.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.859946 helios_ml-0.1.9/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/data/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-05-07 21:57:03.000000 helios_ml-0.1.9/data/logo/logo-background.png
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-07 21:57:03.000000 helios_ml-0.1.9/data/logo/logo-transparent.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.859946 helios_ml-0.1.9/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/examples/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-05-07 21:57:03.000000 helios_ml-0.1.9/examples/cifar10/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-07 21:57:03.000000 helios_ml-0.1.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 21:57:03.000000 helios_ml-0.1.9/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-07 21:57:03.000000 helios_ml-0.1.9/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 21:57:03.000000 helios_ml-0.1.9/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 21:58:01.875946 helios_ml-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.859946 helios_ml-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/src/helios/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/src/helios/core/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/core/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/core/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/core/rng.py
--rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/src/helios/data/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/data/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.867946 helios_ml-0.1.9/src/helios/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/losses/weighted_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.867946 helios_ml-0.1.9/src/helios/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/metrics/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.867946 helios_ml-0.1.9/src/helios/model/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.867946 helios_ml-0.1.9/src/helios/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/nn/swa_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.867946 helios_ml-0.1.9/src/helios/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/optim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.867946 helios_ml-0.1.9/src/helios/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/scheduler/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/scheduler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35899 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.871946 helios_ml-0.1.9/src/helios_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-07 21:58:01.000000 helios_ml-0.1.9/src/helios_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-07 21:58:01.000000 helios_ml-0.1.9/src/helios_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 21:58:01.000000 helios_ml-0.1.9/src/helios_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-07 21:58:01.000000 helios_ml-0.1.9/src/helios_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 21:58:01.000000 helios_ml-0.1.9/src/helios_ml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.871946 helios_ml-0.1.9/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.871946 helios_ml-0.1.9/test/registry_test/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/foo.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/func_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.871946 helios_ml-0.1.9/test/registry_test/nested/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/nested/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/nested/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.871946 helios_ml-0.1.9/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-07 21:57:03.000000 helios_ml-0.1.9/tools/generate_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.659035 helios_ml-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.647035 helios_ml-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.647035 helios_ml-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-09 21:15:08.000000 helios_ml-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-09 21:15:08.000000 helios_ml-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-09 21:15:08.000000 helios_ml-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-09 21:15:08.000000 helios_ml-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-09 21:15:08.000000 helios_ml-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-09 21:15:40.659035 helios_ml-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-09 21:15:08.000000 helios_ml-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.647035 helios_ml-0.2.0/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.651035 helios_ml-0.2.0/data/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-05-09 21:15:08.000000 helios_ml-0.2.0/data/logo/logo-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-09 21:15:08.000000 helios_ml-0.2.0/data/logo/logo-transparent.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.647035 helios_ml-0.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.651035 helios_ml-0.2.0/examples/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-05-09 21:15:08.000000 helios_ml-0.2.0/examples/cifar10/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-09 21:15:08.000000 helios_ml-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.651035 helios_ml-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 21:15:08.000000 helios_ml-0.2.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-09 21:15:08.000000 helios_ml-0.2.0/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-09 21:15:08.000000 helios_ml-0.2.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 21:15:40.663035 helios_ml-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.647035 helios_ml-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.651035 helios_ml-0.2.0/src/helios/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.651035 helios_ml-0.2.0/src/helios/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/core/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/core/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/core/rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.651035 helios_ml-0.2.0/src/helios/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/data/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.651035 helios_ml-0.2.0/src/helios/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/losses/weighted_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.655035 helios_ml-0.2.0/src/helios/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/metrics/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.655035 helios_ml-0.2.0/src/helios/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.655035 helios_ml-0.2.0/src/helios/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/nn/swa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.655035 helios_ml-0.2.0/src/helios/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/optim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.655035 helios_ml-0.2.0/src/helios/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/scheduler/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/scheduler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35898 2024-05-09 21:15:08.000000 helios_ml-0.2.0/src/helios/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.659035 helios_ml-0.2.0/src/helios_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-09 21:15:40.000000 helios_ml-0.2.0/src/helios_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-09 21:15:40.000000 helios_ml-0.2.0/src/helios_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:15:40.000000 helios_ml-0.2.0/src/helios_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-09 21:15:40.000000 helios_ml-0.2.0/src/helios_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 21:15:40.000000 helios_ml-0.2.0/src/helios_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.659035 helios_ml-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.659035 helios_ml-0.2.0/test/registry_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/registry_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/registry_test/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/registry_test/foo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/registry_test/func_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.659035 helios_ml-0.2.0/test/registry_test/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/registry_test/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/registry_test/nested/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/registry_test/nested/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/registry_test/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-05-09 21:15:08.000000 helios_ml-0.2.0/test/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:15:40.659035 helios_ml-0.2.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-09 21:15:08.000000 helios_ml-0.2.0/tools/generate_requirements.py
```

### Comparing `helios_ml-0.1.9/.github/workflows/publish.yml` & `helios_ml-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/.github/workflows/tests.yml` & `helios_ml-0.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/.pre-commit-config.yaml` & `helios_ml-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/LICENSE` & `helios_ml-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/PKG-INFO` & `helios_ml-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-ml
-Version: 0.1.9
+Version: 0.2.0
 Summary: A light-weight system for training AI networks using PyTorch
 Author-email: "Mauricio A. Rovira Galvez" <maroviragalvez@outlook.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/marovira/helios-ml
 Project-URL: source, https://github.com/marovira/helios-ml
 Project-URL: issues, https://github.com/marovira/helios-ml/issues
 Project-URL: release notes, https://github.com/marovira/helios-ml/releases
```

### Comparing `helios_ml-0.1.9/README.rst` & `helios_ml-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/data/logo/logo-background.png` & `helios_ml-0.2.0/data/logo/logo-background.png`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/data/logo/logo-transparent.png` & `helios_ml-0.2.0/data/logo/logo-transparent.png`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/examples/cifar10/cifar10.py` & `helios_ml-0.2.0/examples/cifar10/cifar10.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/pyproject.toml` & `helios_ml-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/core/__init__.py` & `helios_ml-0.2.0/src/helios/core/__init__.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/core/cuda.py` & `helios_ml-0.2.0/src/helios/core/cuda.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/core/distributed.py` & `helios_ml-0.2.0/src/helios/core/distributed.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/core/logging.py` & `helios_ml-0.2.0/src/helios/core/logging.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/core/rng.py` & `helios_ml-0.2.0/src/helios/core/rng.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/core/utils.py` & `helios_ml-0.2.0/src/helios/core/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/data/__init__.py` & `helios_ml-0.2.0/src/helios/data/__init__.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/data/datamodule.py` & `helios_ml-0.2.0/src/helios/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/data/functional.py` & `helios_ml-0.2.0/src/helios/data/functional.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/data/samplers.py` & `helios_ml-0.2.0/src/helios/data/samplers.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/data/transforms.py` & `helios_ml-0.2.0/src/helios/data/transforms.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/losses/utils.py` & `helios_ml-0.2.0/src/helios/losses/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/losses/weighted_loss.py` & `helios_ml-0.2.0/src/helios/losses/weighted_loss.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/metrics/functional.py` & `helios_ml-0.2.0/src/helios/metrics/functional.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,70 +109,48 @@
     pp = pos_count / total_count
     precision_at_i = np.sum(pp)
     precision_at_i = precision_at_i / (total + epsilon)
 
     return precision_at_i
 
 
-def _mae_torch(pred: torch.Tensor, gt: torch.Tensor) -> float:
+def _mae(pred: npt.NDArray, gt: npt.NDArray, scale: float = 1.0) -> float:
     """
-    MAE Torch implementation. See calculate_mae_torch for details.
+    MAE implementation. See calculate_mae for details.
 
     Args:
-        pred (torch.Tensor): predicate (inferred) images in range [0, 255]
-        gt (torch.Tensor): ground-truth images in range [0, 255]
+        pred (torch.Tensor): predicate tensor.
+        gt (torch.Tensor): ground-truth tensor.
+        scale (float): the scaling factor used in the tensor data (if any).
 
     Returns:
         float: the MAE score.
     """
-    h, w = gt.shape[0:2]
-    sum_error = torch.sum(torch.absolute(torch.sub(pred.float(), gt.float())))
-    mae_error = torch.divide(sum_error, float(h) * float(w) * 2550 + 1e-4)
+    n = np.prod(gt.shape)
+    sum_error = np.sum(np.abs(np.subtract(np.float32(pred), np.float32(gt))))
+    mae_error = np.divide(sum_error, n * scale + 1e-4)
     return float(mae_error)
 
 
-def _f1_score_torch(
-    pd: torch.Tensor, gt: torch.Tensor
-) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+def _mae_torch(pred: torch.Tensor, gt: torch.Tensor, scale: float = 1.0) -> float:
     """
-    Calculate the following scores: precision, recall, and F1 for torch.
-
-    See calculate_precision/recall/f1_torch for details.
+    MAE Torch implementation. See calculate_mae_torch for details.
 
     Args:
-        pd (torch.Tensor): predicate tensor.
+        pred (torch.Tensor): predicate tensor.
         gt (torch.Tensor): ground-truth tensor.
+        scale (float): the scaling factor used in the tensor data (if any).
 
     Returns:
-        tuple[torch.Tensor, torch.Tensor, torch.Tensor]: the precision, recall, and F1
-        scores, respectively.
+        float: the MAE score.
     """
-    gt_num = torch.sum((gt > 128).float() * 1)
-
-    pp = pd[gt > 128]
-    nn = pd[gt <= 128]
-
-    pp_hist = torch.histc(pp, bins=255, min=0, max=255)
-    nn_hist = torch.histc(nn, bins=255, min=0, max=255)
-
-    pp_hist_flip = torch.flipud(pp_hist)
-    nn_hist_flip = torch.flipud(nn_hist)
-
-    pp_hist_flip_cum = torch.cumsum(pp_hist_flip, dim=0)
-    nn_hist_flip_cum = torch.cumsum(nn_hist_flip, dim=0)
-
-    precision = (pp_hist_flip_cum) / (pp_hist_flip_cum + nn_hist_flip_cum + 1e-4)
-    recall = (pp_hist_flip_cum) / (gt_num + 1e-4)
-    f1 = (1 + 0.3) * precision * recall / (0.3 * precision + recall + 1e-4)
-
-    return (
-        torch.reshape(precision, (1, precision.shape[0])),
-        torch.reshape(recall, (1, recall.shape[0])),
-        torch.reshape(f1, (1, f1.shape[0])),
-    )
+    n = torch.prod(torch.tensor(gt.shape))
+    sum_error = torch.sum(torch.absolute(torch.sub(pred.float(), gt.float())))
+    mae_error = torch.divide(sum_error, n * scale + 1e-4)
+    return float(mae_error)
 
 
 def calculate_psnr(
     img: npt.NDArray,
     img2: npt.NDArray,
     crop_border: int,
     input_order: str = "HWC",
@@ -379,69 +357,51 @@
             continue
         mAP_sum += _average_precision(scores, targets)
         class_count += 1
 
     return 100 * (mAP_sum / class_count)
 
 
-def calculate_mae_torch(pred: torch.Tensor, gt: torch.Tensor) -> float:
+def calculate_mae(pred: npt.NDArray, gt: npt.NDArray, scale: float = 1.0) -> float:
     """
     Compute the MAE (Mean-Average Precision) score.
 
     Implementation follows: https://en.wikipedia.org/wiki/Mean_absolute_error
+    The scale argument is used in the event that the input arrays are not in the range
+    [0, 1] but instead have been scaled to be in the range [0, N] where N is the factor.
+    For example, if the arrays are images in the range [0, 255], then the scaling factor
+    should be set to 255. If the arrays are already in the range [0, 1], then the scale
+    can be omitted.
 
     Args:
-        pred (torch.Tensor): predicate (inferred) images in range [0, 255]
-        gt (torch.Tensor): ground-truth images in range [0, 255]
+        pred (npt.NDArray): predicate (inferred) array
+        gt (npt.NDArray): ground-truth array
+        scale (float): scaling factor that was used on the input arrays (if any)
 
     Returns:
         float: the MAE score.
     """
-    return _mae_torch(pred, gt)
-
-
-def calculate_precision_torch(pred: torch.Tensor, gt: torch.Tensor) -> float:
-    """
-    Compute the Precision score.
-
-    Implementation follows:  https://en.wikipedia.org/wiki/Precision_and_recall
-
-    Args:
-        pred (torch.Tensor): predicate (inferred) images in range [0, 255]
-        gt (torch.Tensor): ground-truth images in range [0, 255]
-
-    Returns:
-        float: the precision score.
-    """
-    return _f1_score_torch(pred, gt)[0].cpu().data.numpy()
+    return _mae(pred, gt, scale)
 
 
-def calculate_recall_torch(pred: torch.Tensor, gt: torch.Tensor) -> float:
-    """
-    Compute the Recall score.
-
-    Implementation follows:  https://en.wikipedia.org/wiki/Precision_and_recall
-
-    Args:
-        pred (torch.Tensor): predicate (inferred) images in range [0, 255]
-        gt (torch.Tensor): ground-truth images in range [0, 255]
-
-    Returns:
-        float: the recall score.
-    """
-    return _f1_score_torch(pred, gt)[1].cpu().data.numpy()
-
-
-def calculate_f1_torch(pred: torch.Tensor, gt: torch.Tensor) -> float:
+def calculate_mae_torch(
+    pred: torch.Tensor, gt: torch.Tensor, scale: float = 1.0
+) -> float:
     """
-    Compute the F1 score.
+    Compute the MAE (Mean-Average Precision) score.
 
-    Implementation follows: https://en.wikipedia.org/wiki/F-score
+    Implementation follows: https://en.wikipedia.org/wiki/Mean_absolute_error
+    The scale argument is used in the event that the input tensors are not in the range
+    [0, 1] but instead have been scaled to be in the range [0, N] where N is the factor.
+    For example, if the tensors are images in the range [0, 255], then the scaling factor
+    should be set to 255. If the tensors are already in the range [0, 1], then the scale
+    can be omitted.
 
     Args:
-        pred (torch.Tensor): predicate (inferred) images in range [0, 255]
-        gt (torch.Tensor): ground-truth images in range [0, 255]
+        pred (torch.Tensor): predicate (inferred) tensor
+        gt (torch.Tensor): ground-truth tensor
+        scale (float): scaling factor that was used on the input tensors (if any)
 
     Returns:
-        float: the F1 score.
+        float: the MAE score.
     """
-    return _f1_score_torch(pred, gt)[2].cpu().data.numpy()
+    return _mae_torch(pred, gt)
```

### Comparing `helios_ml-0.1.9/src/helios/metrics/metrics.py` & `helios_ml-0.2.0/src/helios/metrics/metrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 import numpy.typing as npt
 import torch
 from torch import nn
 
 from helios import core
 
 from .functional import (
-    calculate_f1_torch,
+    calculate_mae,
     calculate_mae_torch,
     calculate_mAP,
-    calculate_precision_torch,
     calculate_psnr,
     calculate_psnr_torch,
-    calculate_recall_torch,
     calculate_ssim,
     calculate_ssim_torch,
 )
 
 METRICS_REGISTRY = core.Registry("metrics")
 
 
@@ -66,16 +64,16 @@
     def forward(
         self, img: npt.NDArray | torch.Tensor, img2: npt.NDArray | torch.Tensor
     ) -> float:
         """
         Calculate the PSNR metric.
 
         Args:
-            img (np.ndarray): Images with range [0, 255].
-            img2 (np.ndarray): Images with range [0, 255].
+            img (np.ndarray | torch.Tensor): Images with range [0, 255].
+            img2 (np.ndarray | torch.Tensor): Images with range [0, 255].
 
         Returns:
             float: PSNR value.
         """
         if isinstance(img, torch.Tensor) and isinstance(img2, torch.Tensor):
             return calculate_psnr_torch(
                 img, img2, self._crop_border, self._test_y_channel
@@ -120,16 +118,16 @@
     def forward(
         self, img: npt.NDArray | torch.Tensor, img2: npt.NDArray | torch.Tensor
     ) -> float:
         """
         Calculate the SSIM metric.
 
         Args:
-            img (np.ndarray): Images with range [0, 255].
-            img2 (np.ndarray): Images with range [0, 255].
+            img (np.ndarray | torch.Tensor): Images with range [0, 255].
+            img2 (np.ndarray | torch.Tensor): Images with range [0, 255].
 
         Returns:
             float: PSNR value.
         """
         if isinstance(img, torch.Tensor) and isinstance(img2, torch.Tensor):
             return calculate_ssim_torch(
                 img, img2, self._crop_border, self._test_y_channel
@@ -162,91 +160,42 @@
         """
         return calculate_mAP(targs, preds)
 
 
 @METRICS_REGISTRY.register
 class CalculateMAE(nn.Module):
     """
-    Calculate the mAP (Mean Average Precision).
-
-    Implementation follows:
-    https://en.wikipedia.org/wiki/Evaluation_measures_(information_retrieval)#Mean_average_precision
-    """
-
-    def forward(self, pred: torch.Tensor, gt: torch.Tensor) -> float:
-        """
-        Calculate the mAP (Mean Average Precision).
-
-        Args:
-            targs (np.ndarray): target (inferred) labels in range [0, 1].
-            preds (np.ndarray): predicate labels in range [0, 1].
-
-        Returns:
-            float: the mAP score
-        """
-        return calculate_mae_torch(pred, gt)
-
-
-@METRICS_REGISTRY.register
-class CalculatePrecision(nn.Module):
-    """
-    Compute the Precision score.
-
-    Implementation follows:  https://en.wikipedia.org/wiki/Precision_and_recall
-    """
-
-    def forward(self, pred: torch.Tensor, gt: torch.Tensor) -> float:
-        """
-        Compute the Precision score.
+    Compute the MAE (Mean-Average Precision) score.
 
-        Args:
-            pred (torch.Tensor): predicate (inferred) images in range [0, 255]
-            gt (torch.Tensor): ground-truth images in range [0, 255]
-
-        Returns:
-            float: the precision score.
-        """
-        return calculate_precision_torch(pred, gt)
-
-
-@METRICS_REGISTRY.register
-class CalculateRecall(nn.Module):
-    """
-    Compute the Recall score.
-
-    Implementation follows:  https://en.wikipedia.org/wiki/Precision_and_recall
-    """
-
-    def forward(self, pred: torch.Tensor, gt: torch.Tensor) -> float:
-        """
-        Compute the Recall score.
+    Implementation follows: https://en.wikipedia.org/wiki/Mean_absolute_error
+    The scale argument is used in the event that the input tensors are not in the range
+    [0, 1] but instead have been scaled to be in the range [0, N] where N is the factor.
+    For example, if the tensors are images in the range [0, 255], then the scaling factor
+    should be set to 255. If the tensors are already in the range [0, 1], then the scale
+    can be omitted.
 
-        Args:
-            pred (torch.Tensor): predicate (inferred) images in range [0, 255]
-            gt (torch.Tensor): ground-truth images in range [0, 255]
-
-        Returns:
-            float: the recall score.
-        """
-        return calculate_recall_torch(pred, gt)
-
-
-@METRICS_REGISTRY.register
-class CalculateF1(nn.Module):
+    Args:
+        scale (float): scaling factor that was used on the input tensors (if any)
     """
-    Compute the F1 score.
 
-    Implementation follows: https://en.wikipedia.org/wiki/F-score
-    """
+    def __init__(self, scale: float = 1):
+        """Construct the MAE metric."""
+        super().__init__()
+        self._scale = scale
 
-    def forward(self, pred: torch.Tensor, gt: torch.Tensor) -> float:
+    def forward(
+        self, pred: npt.NDArray | torch.Tensor, gt: npt.NDArray | torch.Tensor
+    ) -> float:
         """
-        Compute the F1 score.
+        Calculate the MAE metric.
 
         Args:
-            pred (torch.Tensor): predicate (inferred) images in range [0, 255]
-            gt (torch.Tensor): ground-truth images in range [0, 255]
+            pred (np.ndarray | torch.Tensor): predicate (inferred) data.
+            gt (np.ndarray | torch.Tensor): ground-truth data.
 
         Returns:
-            float: the F1 score.
+            float: the MAE score
         """
-        return calculate_f1_torch(pred, gt)
+        if isinstance(pred, torch.Tensor) and isinstance(gt, torch.Tensor):
+            return calculate_mae_torch(pred, gt, self._scale)
+        assert isinstance(pred, np.ndarray) and isinstance(gt, np.ndarray)
+        return calculate_mae(pred, gt, self._scale)
```

### Comparing `helios_ml-0.1.9/src/helios/model/model.py` & `helios_ml-0.2.0/src/helios/model/model.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/model/utils.py` & `helios_ml-0.2.0/src/helios/model/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/nn/swa_utils.py` & `helios_ml-0.2.0/src/helios/nn/swa_utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/nn/utils.py` & `helios_ml-0.2.0/src/helios/nn/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/onnx.py` & `helios_ml-0.2.0/src/helios/onnx.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/optim/utils.py` & `helios_ml-0.2.0/src/helios/optim/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/scheduler/schedulers.py` & `helios_ml-0.2.0/src/helios/scheduler/schedulers.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/scheduler/utils.py` & `helios_ml-0.2.0/src/helios/scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/src/helios/trainer.py` & `helios_ml-0.2.0/src/helios/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -679,15 +679,15 @@
         state.
 
         Args:
             state (TrainingState): the current training state.
         """
         chkpt_root = core.get_from_optional(self._chkpt_root)
 
-        epoch = state.global_epoch + 1
+        epoch = state.global_epoch
         ite = state.current_iteration
         filename = f"{self.model.save_name}_epoch_{epoch}_iter_{ite}"
         filename = self.model.append_metadata_to_chkpt_name(filename)
         filename += ".pth"
 
         state_dict: dict[str, typing.Any] = {}
         state_dict["training_state"] = state.dict()
@@ -772,32 +772,30 @@
 
         sampler.start_iter = state.dataset_iter
         self.model.train()
 
         for epoch in itertools.count(start=state.global_epoch):
             if training_done:
                 break
+
+            state.global_epoch += 1
             root_logger.info(f"Starting epoch {epoch + 1}")
             sampler.set_epoch(epoch)
             epoch_start = time.time()
 
             iter_timer.start()
             for batch in dataloader:
                 state.global_iteration += 1
                 if state.global_iteration % accumulation_steps == 0:
                     state.current_iteration += 1
                     state.running_iter += 1
                     current_iteration_changed = True
                 else:
                     current_iteration_changed = False
 
-                if state.current_iteration > total_steps:
-                    training_done = True
-                    break
-
                 self.model.on_training_batch_start(state)
                 self.model.train_step(batch, state)
                 iter_timer.record()
                 state.average_iter_time = iter_timer.get_average_time()
                 self.model.on_training_batch_end(
                     state,
                     should_log=(
@@ -841,16 +839,19 @@
                     training_done = True
                     break
 
                 if self.model.should_training_stop():
                     training_done = True
                     break
 
+                if state.current_iteration >= total_steps:
+                    training_done = True
+                    break
+
             state.dataset_iter = 0
-            state.global_epoch += 1
 
             root_logger.info(
                 f"Epoch {epoch + 1} completed in {time.time() - epoch_start:.2f}s"
             )
 
     def _train_on_epoch(self, state: TrainingState) -> None:
         """
@@ -892,14 +893,16 @@
             else itertools.count(start=state.global_epoch)
         )
 
         for epoch in iterator:
             if training_done:
                 break
 
+            state.global_epoch += 1
+
             if state.global_epoch > total_steps:
                 training_done = True
                 break
 
             root_logger.info(f"Starting epoch {epoch + 1}")
             sampler.set_epoch(epoch)
             epoch_start = time.time()
@@ -929,15 +932,14 @@
                         ),
                     )
                     state.dataset_iter += 1
                     if not ite_pbar.update():
                         ite_pbar.refresh()
 
             state.dataset_iter = 0
-            state.global_epoch += 1
 
             if val_freq is not None and state.global_epoch % val_freq == 0:
                 self._validate(state.validation_cycles)
                 state.running_iter = 0
                 if not self.model.have_metrics_improved():
                     state.early_stop_count += 1
                 else:
```

### Comparing `helios_ml-0.1.9/src/helios_ml.egg-info/PKG-INFO` & `helios_ml-0.2.0/src/helios_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-ml
-Version: 0.1.9
+Version: 0.2.0
 Summary: A light-weight system for training AI networks using PyTorch
 Author-email: "Mauricio A. Rovira Galvez" <maroviragalvez@outlook.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/marovira/helios-ml
 Project-URL: source, https://github.com/marovira/helios-ml
 Project-URL: issues, https://github.com/marovira/helios-ml/issues
 Project-URL: release notes, https://github.com/marovira/helios-ml/releases
```

### Comparing `helios_ml-0.1.9/src/helios_ml.egg-info/SOURCES.txt` & `helios_ml-0.2.0/src/helios_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/test/conftest.py` & `helios_ml-0.2.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/test/test_core.py` & `helios_ml-0.2.0/test/test_core.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/test/test_data.py` & `helios_ml-0.2.0/test/test_data.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/test/test_losses.py` & `helios_ml-0.2.0/test/test_losses.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/test/test_model.py` & `helios_ml-0.2.0/test/test_model.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/test/test_nn.py` & `helios_ml-0.2.0/test/test_nn.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/test/test_onnx.py` & `helios_ml-0.2.0/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/test/test_trainer.py` & `helios_ml-0.2.0/test/test_trainer.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.9/tools/generate_requirements.py` & `helios_ml-0.2.0/tools/generate_requirements.py`

 * *Files identical despite different names*

