# Comparing `tmp/mlpro-1.4.2.tar.gz` & `tmp/mlpro-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro-1.4.2.tar", last modified: Tue May  7 13:19:53 2024, max compression
+gzip compressed data, was "mlpro-1.4.3.tar", last modified: Thu May  9 05:32:50 2024, max compression
```

## Comparing `mlpro-1.4.2.tar` & `mlpro-1.4.3.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.525689 mlpro-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-07 13:19:47.000000 mlpro-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 13:19:47.000000 mlpro-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-07 13:19:53.525689 mlpro-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-07 13:19:47.000000 mlpro-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 13:19:49.000000 mlpro-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-07 13:19:53.525689 mlpro-1.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.473690 mlpro-1.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.485690 mlpro-1.4.2/src/mlpro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.485690 mlpro-1.4.2/src/mlpro/bf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.485690 mlpro-1.4.2/src/mlpro/bf/data/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/data/buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/data/datastoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.489690 mlpro-1.4.2/src/mlpro/bf/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26468 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/datasets/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.489690 mlpro-1.4.2/src/mlpro/bf/math/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/math/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/math/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.489690 mlpro-1.4.2/src/mlpro/bf/math/normalizers/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/math/normalizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/math/normalizers/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/math/normalizers/minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/math/normalizers/ztrans.py
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/math/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.489690 mlpro-1.4.2/src/mlpro/bf/ml/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55808 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ml/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.489690 mlpro-1.4.2/src/mlpro/bf/ml/systems/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ml/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ml/systems/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.489690 mlpro-1.4.2/src/mlpro/bf/ml/systems/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ml/systems/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37878 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/mt.py
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.489690 mlpro-1.4.2/src/mlpro/bf/physics/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/physics/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/physics/unitconverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    32607 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.493690 mlpro-1.4.2/src/mlpro/bf/streams/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64843 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.493690 mlpro-1.4.2/src/mlpro/bf/streams/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/samplers/min_wise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/samplers/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/samplers/reservoir_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/samplers/weighted_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.493690 mlpro-1.4.2/src/mlpro/bf/streams/streams/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/streams/clouds.py
--rw-r--r--   0 runner    (1001) docker     (127)    20491 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/streams/clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/streams/csv_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/streams/doublespiral2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/streams/point_outliers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/streams/provider_mlpro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/streams/rnd10d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.493690 mlpro-1.4.2/src/mlpro/bf/streams/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/tasks/deriver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/tasks/rearranger.py
--rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/tasks/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.493690 mlpro-1.4.2/src/mlpro/bf/streams/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/streams/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.497690 mlpro-1.4.2/src/mlpro/bf/systems/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83676 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.497690 mlpro-1.4.2/src/mlpro/bf/systems/pool/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34965 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/doublependulum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/flipflops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.497690 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.477690 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.477690 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.497690 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)    37884 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.497690 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/
--rw-r--r--   0 runner    (1001) docker     (127)   322794 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.477690 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.501690 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl
--rw-r--r--   0 runner    (1001) docker     (127)    52584 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl
--rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl
--rw-r--r--   0 runner    (1001) docker     (127)    58884 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl
--rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/boxontable.xml
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/cartpole.xml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/mlpro.xml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/ur5.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.501690 mlpro-1.4.2/src/mlpro/bf/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.501690 mlpro-1.4.2/src/mlpro/bf/ui/sciui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ui/sciui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ui/sciui/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ui/sciui/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.501690 mlpro-1.4.2/src/mlpro/bf/ui/sciui/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ui/sciui/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24464 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ui/sciui/pool/iis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.501690 mlpro-1.4.2/src/mlpro/bf/ui/sciui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ui/sciui/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/ui/sciui/templates/scenario_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    31658 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/bf/various.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.501690 mlpro-1.4.2/src/mlpro/gt/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.505689 mlpro-1.4.2/src/mlpro/gt/dynamicgames/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/dynamicgames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/dynamicgames/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/dynamicgames/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/dynamicgames/stackelberg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.505689 mlpro-1.4.2/src/mlpro/gt/native/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66293 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/native/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.505689 mlpro-1.4.2/src/mlpro/gt/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.505689 mlpro-1.4.2/src/mlpro/gt/pool/boards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/boards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/boards/bglp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.505689 mlpro-1.4.2/src/mlpro/gt/pool/native/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.505689 mlpro-1.4.2/src/mlpro/gt/pool/native/games/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/native/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/native/games/rockpaperscissors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/native/games/routingproblems_3p.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/native/games/supplydemand_3p.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.505689 mlpro-1.4.2/src/mlpro/gt/pool/native/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/native/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/native/solvers/greedypolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/native/solvers/randomsolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.505689 mlpro-1.4.2/src/mlpro/gt/pool/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/gt/pool/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.505689 mlpro-1.4.2/src/mlpro/oa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.509689 mlpro-1.4.2/src/mlpro/oa/sciui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/sciui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31194 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/sciui/iis.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/sciui/runme.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/sciui/scenario_oa1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.509689 mlpro-1.4.2/src/mlpro/oa/streams/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.509689 mlpro-1.4.2/src/mlpro/oa/streams/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.509689 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.509689 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    16775 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/boundarydetectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.513690 mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.513690 mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.513690 mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/tasks/normalizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.513690 mlpro-1.4.2/src/mlpro/oa/streams/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/streams/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.513690 mlpro-1.4.2/src/mlpro/oa/systems/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/systems/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.513690 mlpro-1.4.2/src/mlpro/oa/systems/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/systems/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/oa/systems/pool/doublependulum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.517690 mlpro-1.4.2/src/mlpro/rl/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    36302 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/models_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/models_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/models_env_ada.py
--rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/models_env_oa.py
--rw-r--r--   0 runner    (1001) docker     (127)    48989 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/models_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.517690 mlpro-1.4.2/src/mlpro/rl/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.517690 mlpro-1.4.2/src/mlpro/rl/pool/actionplanner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/actionplanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/actionplanner/mpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.517690 mlpro-1.4.2/src/mlpro/rl/pool/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50258 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/envs/bglp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/envs/cartpole.py
--rw-r--r--   0 runner    (1001) docker     (127)    44837 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/envs/doublependulum.py
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/envs/gridworld.py
--rw-r--r--   0 runner    (1001) docker     (127)    19097 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/envs/robotinhtm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.517690 mlpro-1.4.2/src/mlpro/rl/pool/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/policies/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/policies/randomgenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.517690 mlpro-1.4.2/src/mlpro/rl/pool/sarsbuffer/
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/sarsbuffer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.517690 mlpro-1.4.2/src/mlpro/rl/pool/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/pool/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65877 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/rl/sciui_rl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.521690 mlpro-1.4.2/src/mlpro/sl/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13144 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.521690 mlpro-1.4.2/src/mlpro/sl/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/fnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/models_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    40710 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/models_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.521690 mlpro-1.4.2/src/mlpro/sl/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.521690 mlpro-1.4.2/src/mlpro/sl/pool/afct/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/pool/afct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.521690 mlpro-1.4.2/src/mlpro/sl/pool/afct/fnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/pool/afct/fnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.521690 mlpro-1.4.2/src/mlpro/sl/pool/afct/fnn/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/pool/afct/fnn/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22451 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/sl/pool/afct/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.521690 mlpro-1.4.2/src/mlpro/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/wrappers/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    38971 2024-05-07 13:19:49.000000 mlpro-1.4.2/src/mlpro/wrappers/mujoco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.525689 mlpro-1.4.2/src/mlpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-07 13:19:53.000000 mlpro-1.4.2/src/mlpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-07 13:19:53.000000 mlpro-1.4.2/src/mlpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:19:53.000000 mlpro-1.4.2/src/mlpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 13:19:53.000000 mlpro-1.4.2/src/mlpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 13:19:53.000000 mlpro-1.4.2/src/mlpro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:19:53.521690 mlpro-1.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-07 13:19:49.000000 mlpro-1.4.2/test/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-07 13:19:49.000000 mlpro-1.4.2/test/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-07 13:19:49.000000 mlpro-1.4.2/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-07 13:19:49.000000 mlpro-1.4.2/test/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-07 13:19:49.000000 mlpro-1.4.2/test/test_pool_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-07 13:19:49.000000 mlpro-1.4.2/test/test_various.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.571494 mlpro-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 05:32:45.000000 mlpro-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-09 05:32:45.000000 mlpro-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-05-09 05:32:50.571494 mlpro-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-09 05:32:45.000000 mlpro-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-09 05:32:46.000000 mlpro-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-09 05:32:50.571494 mlpro-1.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.523494 mlpro-1.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.531494 mlpro-1.4.3/src/mlpro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.535494 mlpro-1.4.3/src/mlpro/bf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.535494 mlpro-1.4.3/src/mlpro/bf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/data/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/data/datastoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.535494 mlpro-1.4.3/src/mlpro/bf/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26468 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/datasets/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.535494 mlpro-1.4.3/src/mlpro/bf/math/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/math/normalizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/normalizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/normalizers/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/normalizers/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/normalizers/ztrans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55808 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ml/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/ml/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ml/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ml/systems/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/ml/systems/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ml/systems/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37878 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/mt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/physics/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/physics/unitconverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32607 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64843 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/streams/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/samplers/min_wise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/samplers/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/samplers/reservoir_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/samplers/weighted_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.543494 mlpro-1.4.3/src/mlpro/bf/streams/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/clouds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20491 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/csv_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/doublespiral2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/point_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/provider_mlpro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/rnd10d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.543494 mlpro-1.4.3/src/mlpro/bf/streams/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/tasks/deriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/tasks/rearranger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/tasks/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.543494 mlpro-1.4.3/src/mlpro/bf/streams/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.543494 mlpro-1.4.3/src/mlpro/bf/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83676 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.543494 mlpro-1.4.3/src/mlpro/bf/systems/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34965 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/doublependulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/flipflops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.543494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.527494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.527494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.547494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    37884 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.547494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/
+-rw-r--r--   0 runner    (1001) docker     (127)   322794 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.527494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.547494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    52584 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    58884 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/boxontable.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/cartpole.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/mlpro.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/ur5.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.547494 mlpro-1.4.3/src/mlpro/bf/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.547494 mlpro-1.4.3/src/mlpro/bf/ui/sciui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/bf/ui/sciui/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24464 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/pool/iis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/bf/ui/sciui/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/templates/scenario_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31658 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/various.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/dynamicgames/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/dynamicgames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/dynamicgames/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/dynamicgames/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/dynamicgames/stackelberg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/native/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66293 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/native/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/pool/boards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/boards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/boards/bglp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/pool/native/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/pool/native/games/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/games/rockpaperscissors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/games/routingproblems_3p.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/games/supplydemand_3p.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/gt/pool/native/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/solvers/greedypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/solvers/randomsolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/gt/pool/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/oa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/oa/sciui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/sciui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31194 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/sciui/iis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/sciui/runme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/sciui/scenario_oa1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/oa/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/oa/streams/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16775 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/boundarydetectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/normalizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/streams/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/systems/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/systems/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/systems/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/systems/pool/doublependulum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.563494 mlpro-1.4.3/src/mlpro/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36302 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/models_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/models_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/models_env_ada.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/models_env_oa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48989 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/models_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.563494 mlpro-1.4.3/src/mlpro/rl/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.563494 mlpro-1.4.3/src/mlpro/rl/pool/actionplanner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/actionplanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/actionplanner/mpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.563494 mlpro-1.4.3/src/mlpro/rl/pool/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50258 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/envs/bglp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/envs/cartpole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44837 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/envs/doublependulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/envs/gridworld.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19097 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/envs/robotinhtm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.563494 mlpro-1.4.3/src/mlpro/rl/pool/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/policies/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/policies/randomgenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/rl/pool/sarsbuffer/
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/sarsbuffer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/rl/pool/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65877 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/sciui_rl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/sl/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13144 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/sl/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/fnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/models_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40710 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/models_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/sl/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/sl/pool/afct/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/pool/afct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/sl/pool/afct/fnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/pool/afct/fnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/sl/pool/afct/fnn/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/pool/afct/fnn/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22451 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/pool/afct/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/wrappers/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38971 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/wrappers/mujoco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.571494 mlpro-1.4.3/src/mlpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-05-09 05:32:50.000000 mlpro-1.4.3/src/mlpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-09 05:32:50.000000 mlpro-1.4.3/src/mlpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:32:50.000000 mlpro-1.4.3/src/mlpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 05:32:50.000000 mlpro-1.4.3/src/mlpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 05:32:50.000000 mlpro-1.4.3/src/mlpro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.571494 mlpro-1.4.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-09 05:32:46.000000 mlpro-1.4.3/test/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-09 05:32:46.000000 mlpro-1.4.3/test/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-09 05:32:46.000000 mlpro-1.4.3/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-09 05:32:46.000000 mlpro-1.4.3/test/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-09 05:32:46.000000 mlpro-1.4.3/test/test_pool_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-09 05:32:46.000000 mlpro-1.4.3/test/test_various.py
```

### Comparing `mlpro-1.4.2/LICENSE` & `mlpro-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/PKG-INFO` & `mlpro-1.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro
-Version: 1.4.2
+Version: 1.4.3
 Summary: MLPro - The Integrative Middleware Framework for Standardized Machine Learning
 Home-page: https://mlpro.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,17 +15,15 @@
 Provides-Extra: full
 Requires-Dist: dill>=0.3.6; extra == "full"
 Requires-Dist: numpy>=1.24.2; extra == "full"
 Requires-Dist: torch>=2.0.0; extra == "full"
 Requires-Dist: matplotlib>=3.7.1; extra == "full"
 Requires-Dist: scipy>=1.10.1; extra == "full"
 Requires-Dist: multiprocess>=0.70.14; extra == "full"
-Requires-Dist: optuna>=3.1.1; extra == "full"
-Requires-Dist: hyperopt>=0.2.7; extra == "full"
-Requires-Dist: mujoco!=3.1.4,>=2.3.3; extra == "full"
+Requires-Dist: mujoco==3.1.3; extra == "full"
 Requires-Dist: lxml>=4.9.2; extra == "full"
 Requires-Dist: pandas>=2.1.3; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro/badge/?version=latest)](https://mlpro.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro.svg)](https://badge.fury.io/py/mlpro)
 [![Anaconda-Version Badge](https://anaconda.org/mlpro/mlpro/badges/version.svg)](https://anaconda.org/mlpro/mlpro)
```

### Comparing `mlpro-1.4.2/README.md` & `mlpro-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/setup.cfg` & `mlpro-1.4.3/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro
-version = 1.4.2
+version = 1.4.3
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro - The Integrative Middleware Framework for Standardized Machine Learning
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro.readthedocs.io
 project_urls = 
@@ -28,17 +28,15 @@
 full = 
 	dill>=0.3.6
 	numpy>=1.24.2
 	torch>=2.0.0
 	matplotlib>=3.7.1
 	scipy>=1.10.1
 	multiprocess>=0.70.14
-	optuna>=3.1.1
-	hyperopt>=0.2.7
-	mujoco>=2.3.3,!=3.1.4
+	mujoco==3.1.3
 	lxml>=4.9.2
 	pandas>=2.1.3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mlpro-1.4.2/src/mlpro/bf/data/buffers.py` & `mlpro-1.4.3/src/mlpro/bf/data/buffers.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/data/datastoring.py` & `mlpro-1.4.3/src/mlpro/bf/data/datastoring.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/datasets/basics.py` & `mlpro-1.4.3/src/mlpro/bf/datasets/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/events.py` & `mlpro-1.4.3/src/mlpro/bf/events.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/exceptions.py` & `mlpro-1.4.3/src/mlpro/bf/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/math/basics.py` & `mlpro-1.4.3/src/mlpro/bf/math/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/math/geometry.py` & `mlpro-1.4.3/src/mlpro/bf/math/geometry.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/math/normalizers/basics.py` & `mlpro-1.4.3/src/mlpro/bf/math/normalizers/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/math/normalizers/minmax.py` & `mlpro-1.4.3/src/mlpro/bf/math/normalizers/minmax.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/math/normalizers/ztrans.py` & `mlpro-1.4.3/src/mlpro/bf/math/normalizers/ztrans.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/math/properties.py` & `mlpro-1.4.3/src/mlpro/bf/math/properties.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/ml/basics.py` & `mlpro-1.4.3/src/mlpro/bf/ml/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/ml/systems/basics.py` & `mlpro-1.4.3/src/mlpro/bf/ml/systems/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/mt.py` & `mlpro-1.4.3/src/mlpro/bf/mt.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/ops.py` & `mlpro-1.4.3/src/mlpro/bf/ops.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/physics/basics.py` & `mlpro-1.4.3/src/mlpro/bf/physics/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/physics/unitconverter.py` & `mlpro-1.4.3/src/mlpro/bf/physics/unitconverter.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/plot.py` & `mlpro-1.4.3/src/mlpro/bf/plot.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/models.py` & `mlpro-1.4.3/src/mlpro/bf/streams/models.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/samplers/min_wise.py` & `mlpro-1.4.3/src/mlpro/bf/streams/samplers/min_wise.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/samplers/random.py` & `mlpro-1.4.3/src/mlpro/bf/streams/samplers/random.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/samplers/reservoir_sampling.py` & `mlpro-1.4.3/src/mlpro/bf/streams/samplers/reservoir_sampling.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/samplers/weighted_random.py` & `mlpro-1.4.3/src/mlpro/bf/streams/samplers/weighted_random.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/streams/clouds.py` & `mlpro-1.4.3/src/mlpro/bf/streams/streams/clouds.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/streams/clusters.py` & `mlpro-1.4.3/src/mlpro/bf/streams/streams/clusters.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/streams/csv_file.py` & `mlpro-1.4.3/src/mlpro/bf/streams/streams/csv_file.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/streams/doublespiral2d.py` & `mlpro-1.4.3/src/mlpro/bf/streams/streams/doublespiral2d.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/streams/point_outliers.py` & `mlpro-1.4.3/src/mlpro/bf/streams/streams/point_outliers.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/streams/provider_mlpro.py` & `mlpro-1.4.3/src/mlpro/bf/streams/streams/provider_mlpro.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/streams/rnd10d.py` & `mlpro-1.4.3/src/mlpro/bf/streams/streams/rnd10d.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/tasks/deriver.py` & `mlpro-1.4.3/src/mlpro/bf/streams/tasks/deriver.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/tasks/rearranger.py` & `mlpro-1.4.3/src/mlpro/bf/streams/tasks/rearranger.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/streams/tasks/windows.py` & `mlpro-1.4.3/src/mlpro/bf/streams/tasks/windows.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/basics.py` & `mlpro-1.4.3/src/mlpro/bf/systems/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/doublependulum.py` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/doublependulum.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/flipflops.py` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/flipflops.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/boxontable.xml` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/boxontable.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/cartpole.xml` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/cartpole.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/mlpro.xml` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/mlpro.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/pendulum.xml` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/pendulum.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/systems/pool/mujoco/ur5.xml` & `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/ur5.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/ui/sciui/framework.py` & `mlpro-1.4.3/src/mlpro/bf/ui/sciui/framework.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/ui/sciui/main.py` & `mlpro-1.4.3/src/mlpro/bf/ui/sciui/main.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/ui/sciui/pool/iis.py` & `mlpro-1.4.3/src/mlpro/bf/ui/sciui/pool/iis.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py` & `mlpro-1.4.3/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/ui/sciui/templates/scenario_test.py` & `mlpro-1.4.3/src/mlpro/bf/ui/sciui/templates/scenario_test.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/bf/various.py` & `mlpro-1.4.3/src/mlpro/bf/various.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/gt/dynamicgames/basics.py` & `mlpro-1.4.3/src/mlpro/gt/dynamicgames/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/gt/dynamicgames/potential.py` & `mlpro-1.4.3/src/mlpro/gt/dynamicgames/potential.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/gt/dynamicgames/stackelberg.py` & `mlpro-1.4.3/src/mlpro/gt/dynamicgames/stackelberg.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/gt/native/basics.py` & `mlpro-1.4.3/src/mlpro/gt/native/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/gt/pool/boards/bglp.py` & `mlpro-1.4.3/src/mlpro/gt/pool/boards/bglp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py` & `mlpro-1.4.3/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py` & `mlpro-1.4.3/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/gt/pool/native/games/rockpaperscissors.py` & `mlpro-1.4.3/src/mlpro/gt/pool/native/games/rockpaperscissors.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/gt/pool/native/games/routingproblems_3p.py` & `mlpro-1.4.3/src/mlpro/gt/pool/native/games/routingproblems_3p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/gt/pool/native/games/supplydemand_3p.py` & `mlpro-1.4.3/src/mlpro/gt/pool/native/games/supplydemand_3p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/gt/pool/native/solvers/greedypolicy.py` & `mlpro-1.4.3/src/mlpro/gt/pool/native/solvers/greedypolicy.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/gt/pool/native/solvers/randomsolver.py` & `mlpro-1.4.3/src/mlpro/gt/pool/native/solvers/randomsolver.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/sciui/iis.py` & `mlpro-1.4.3/src/mlpro/oa/sciui/iis.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/sciui/runme.py` & `mlpro-1.4.3/src/mlpro/oa/sciui/runme.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/sciui/scenario_oa1.py` & `mlpro-1.4.3/src/mlpro/oa/sciui/scenario_oa1.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/basics.py` & `mlpro-1.4.3/src/mlpro/oa/streams/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,45 +7,50 @@
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2023-06-08  0.0.0     SK       Creation
 ## -- 2023-09-12  1.0.0     SK       Release
 ## -- 2023-11-21  1.0.1     SK       Time Stamp update
 ## -- 2024-02-25  1.1.0     SK       Visualisation update
 ## -- 2024-04-10  1.2.0     DA/SK    Refactoring
 ## -- 2024-04-11  1.3.0     DA       Class Anomaly: extensions on methods update_plot_*
+## -- 2024-05-07  1.3.1     SK       Bug fix related to p_instances
+## -- 2024-05-09  1.3.2     DA       Bugfix in method Anomaly._update_plot()
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.3.0 (2024-04-11)
+Ver. 1.3.2 (2024-05-09)
 
 This module provides templates for anomaly detection to be used in the context of online adaptivity.
 """
 
-from matplotlib.figure import Figure
 from mlpro.bf.various import Id
 from mlpro.bf.plot import Plottable, PlotSettings
 from mlpro.bf.events import Event
 from mlpro.bf.streams import Instance
 
 
 
+
+
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class Anomaly (Id, Event, Plottable):
     """
     This is the base class for anomaly events which can be raised by the anomaly detectors when an
     anomaly is detected.
 
     Parameters
     ----------
-    p_id
-        Optional external id.
+    p_instances : Instance
+        List of instances. Default value = None.
+    p_ano_scores : list
+        List of anomaly scores of instances. Default = None.
     p_visualize : bool
         Boolean switch for visualisation. Default = False.
-    p_color : string
-        Color of the anomaly during visualization.
+    p_raising_object : object
+        Reference of the object raised. Default = None.
     **p_kwargs
         Further optional keyword arguments.
     """
 
     C_TYPE                  = 'Anomaly'
 
     C_PLOT_ACTIVE           = True
@@ -53,70 +58,70 @@
     C_PLOT_VALID_VIEWS      = [ PlotSettings.C_VIEW_2D, 
                                 PlotSettings.C_VIEW_3D, 
                                 PlotSettings.C_VIEW_ND ]
     C_PLOT_DEFAULT_VIEW     = PlotSettings.C_VIEW_ND
 
 ## -------------------------------------------------------------------------------------------------
     def __init__(self,
-                 p_instance : Instance = None,
+                 p_instances: list[Instance] = None,
                  p_ano_scores : list = None,
                  p_visualize : bool = False,
                  p_raising_object : object = None,
                  p_det_time : str = None,
                  **p_kwargs):
         
         Id.__init__( self, p_id = 0 )
         Event.__init__( self, p_raising_object=p_raising_object,
                         p_tstamp=p_det_time, **p_kwargs)
         Plottable.__init__( self, p_visualize = p_visualize )
 
-        self.instance : Instance = p_instance
+        self.instances : Instance | list[Instance] = p_instances
         self.ano_scores = p_ano_scores
 
 
 ## -------------------------------------------------------------------------------------------------
-    def get_instance(self) -> Instance:
-        return self.instance
+    def get_instances(self) -> list[Instance]:
+        return self.instances
     
 
 ## -------------------------------------------------------------------------------------------------
     def get_ano_scores(self):
         return self.ano_scores
     
 
 ## -------------------------------------------------------------------------------------------------
     def update_plot( self, 
                      p_axlimits_changed : bool = False,
                      p_xlim = None,
                      p_ylim = None,
                      p_zlim = None,
-                     **p_kwargs):
+                     **p_kwargs ):
         
         return super().update_plot( p_axlimits_changed = p_axlimits_changed,
                                     p_xlim = p_xlim,
                                     p_ylim = p_ylim,
                                     p_zlim = p_zlim,
                                     **p_kwargs)
     
 
 ## -------------------------------------------------------------------------------------------------
     def _update_plot_2d( self, 
                          p_settings: PlotSettings, 
                          p_axlimits_changed : bool, 
-                         P_xlim,
+                         p_xlim,
                          p_ylim,
                          **p_kwargs ):
         pass
 
 
 ## -------------------------------------------------------------------------------------------------
     def _update_plot_3d( self, 
                          p_settings: PlotSettings, 
                          p_axlimits_changed : bool, 
-                         P_xlim,
+                         p_xlim,
                          p_ylim,
                          p_zlim,
                          **p_kwargs ):
         pass
 
 
 ## -------------------------------------------------------------------------------------------------
```

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2023-06-08  0.0.0     SK       Creation
 ## -- 2023-09-12  1.0.0     SK       Release
 ## -- 2023-11-21  1.0.1     SK       Time Stamp update
 ## -- 2024-02-25  1.1.0     SK       Visualisation update
 ## -- 2024-04-10  1.2.0     DA/SK    Refactoring
+## -- 2024-05-07  1.2.1     SK       Bug fix on groupanomaly visualisation
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.2.0 (2024-04-10)
+Ver. 1.2.1 (2024-05-07)
 
 This module provides templates for anomaly detection to be used in the context of online adaptivity.
 """
 
 from mlpro.bf.plot import PlotSettings
 from mlpro.bf.streams import Instance
 from mlpro.oa.streams.tasks.anomalydetectors.anomalies.basics import Anomaly
@@ -35,28 +36,29 @@
     
     """
 
     C_NAME      = 'Group'
 
 ## -------------------------------------------------------------------------------------------------
     def __init__(self,
-                 p_instances : Instance = None,
+                 p_instances : list[Instance] = None,
                  p_ano_scores : list = None,
                  p_visualize : bool = False,
                  p_raising_object : object = None,
                  p_det_time : str = None,
                  p_mean : float= None,
                  p_mean_deviation : float = None,
                  **p_kwargs):
         super().__init__(p_instance=p_instances, p_ano_scores=p_ano_scores,
                          p_visualize=p_visualize, p_raising_object=p_raising_object,
                          p_det_time=p_det_time, **p_kwargs)
         
         self.instances = p_instances
         p_ano_scores = p_ano_scores
+        self.plot_update = True
 
 
 ## -------------------------------------------------------------------------------------------------
     def set_instances(self, p_instances, p_ano_scores):
         self.instances = p_instances
         self.ano_scores = p_ano_scores
 
@@ -76,30 +78,30 @@
         Parameters:
         ax (matplotlib.axes.Axes): The axes object to draw the shaded region on.
         x1, x2 (float): x-coordinates of the left and right edges of the rectangle.
         y1, y2 (float): y-coordinates of the bottom and top edges of the rectangle.
         color (str): Color of the shaded region.
         alpha (float): Transparency of the shaded region (default is 0.5).
         """
-        super()._update_plot_nd(p_settings, **p_kwargs)
+        if not self.plot_update: return
     
         label = self.C_NAME[0]
-        x1 = self.get_instance()[0].get_id()
-        x2 = self.get_instance()[-1].get_id()
+        x1 = self.get_instances()[0].get_id()
+        x2 = self.get_instances()[-1].get_id()
         a=[]
         b=[]
-        for instance in self.get_instance():
+        for instance in self.get_instances():
             a.append(instance.get_feature_data().get_values())
         for x in a:
             b.extend(x)
         y1 = min(b)
         y2 = max(b)
 
         if self._rect is None:
-            self._rect = patches.Rectangle((x1, y1), x2 - x1, y2 - y1, linewidth=0, edgecolor='none', facecolor='yellow', alpha=0.3)
+            self._rect = patches.Rectangle((x1, y1), x2 - x1, y2 - y1, linewidth=1, edgecolor='black', facecolor='yellow', alpha=0.5)
             self._plot_rectangle = p_settings.axes.add_patch(self._rect)
             self._plot_rectangle_t = p_settings.axes.text((x1+x2)/2, 0, label, color='b' )
 
         else:
             self._rect.set_x(x1)
             self._rect.set_y(y1)
             self._rect.set_width(x2 - x1)
```

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2023-06-08  0.0.0     SK       Creation
 ## -- 2023-09-12  1.0.0     SK       Release
 ## -- 2023-11-21  1.0.1     SK       Time Stamp update
 ## -- 2024-02-25  1.1.0     SK       Visualisation update
 ## -- 2024-04-10  1.2.0     DA/SK    Refactoring
 ## -- 2024-04-16  1.3.0     DA       Finished visualisation
+## -- 2024-05-07  1.3.1     SK       Bug fix related to p_instances
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.3.0 (2024-04-16)
+Ver. 1.3.1 (2024-05-07)
 
 This module provides templates for anomaly detection to be used in the context of online adaptivity.
 """
 
 from mlpro.bf.plot import PlotSettings
 from mlpro.bf.streams import Instance
 from mlpro.oa.streams.tasks.anomalydetectors.anomalies.basics import Anomaly
@@ -38,30 +39,30 @@
     C_NAME              = 'Point'
 
     C_PLOT_CH_SIZE      = 0.06           # Crosshair size in % of visible axes area
     C_PLOT_CH_OFFSET    = 0.4            # Crosshair distance from the center in [0,1]
 
 ## -------------------------------------------------------------------------------------------------
     def __init__(self,
-                 p_instance : Instance = None,
+                 p_instances : list[Instance] = None,
                  p_ano_scores : list = None,
                  p_visualize : bool = False,
                  p_raising_object : object = None,
                  p_det_time : str = None,
                  p_deviation : float=None,
                  **p_kwargs):
         
-        super().__init__( p_instance=p_instance, 
+        super().__init__( p_instances=p_instances, 
                           p_ano_scores=p_ano_scores,
                           p_visualize=p_visualize, 
                           p_raising_object=p_raising_object,
                           p_det_time=p_det_time, 
                           **p_kwargs )
         
-        self.instance = p_instance
+        self.instances = p_instances
         self.ano_scores = p_ano_scores
 
 
 ## -------------------------------------------------------------------------------------------------
     def _init_plot_2d(self, p_figure: Figure, p_settings: PlotSettings):
         self._plot_line_x1 = None
         self._plot_line_x2 = None
@@ -84,15 +85,15 @@
 
 
 ## -------------------------------------------------------------------------------------------------
     def _update_plot_2d(self, p_settings: PlotSettings, p_axlimits_changed: bool, p_xlim, p_ylim, **p_kwargs):
 
         if ( self._plot_line_x1 is not None ) and not p_axlimits_changed: return
 
-        inst           = self.get_instance()
+        inst           = self.get_instances()[-1]
         feature_values = inst.get_feature_data().get_values()  
 
         len_x          = ( p_xlim[1] - p_xlim[0] ) * self.C_PLOT_CH_SIZE / 2
         len_y          = ( p_ylim[1] - p_ylim[0] ) * self.C_PLOT_CH_SIZE / 2
 
         offset_x       = len_x * self.C_PLOT_CH_OFFSET
         offset_y       = len_y * self.C_PLOT_CH_OFFSET
@@ -126,15 +127,15 @@
 
 
 ## -------------------------------------------------------------------------------------------------
     def _update_plot_3d(self, p_settings: PlotSettings, p_axlimits_changed: bool, p_xlim, p_ylim, p_zlim, **p_kwargs):
 
         if ( self._plot_line_x1 is not None ) and not p_axlimits_changed: return
 
-        inst           = self.get_instance()
+        inst           = self.get_instances()[-1]
         feature_values = inst.get_feature_data().get_values()  
 
         len_x          = ( p_xlim[1] - p_xlim[0] ) * self.C_PLOT_CH_SIZE / 2
         len_y          = ( p_ylim[1] - p_ylim[0] ) * self.C_PLOT_CH_SIZE / 2
         len_z          = ( p_zlim[1] - p_zlim[0] ) * self.C_PLOT_CH_SIZE / 2
 
         offset_x       = len_x * self.C_PLOT_CH_OFFSET
@@ -186,15 +187,15 @@
 
         
 ## -------------------------------------------------------------------------------------------------
     def _update_plot_nd(self, p_settings: PlotSettings, p_axlimits_changed: bool, p_ylim, **p_kwargs):
 
         if ( self._plot_line is not None ) and not p_axlimits_changed: return
         
-        inst_id = self.get_instance().get_id()
+        inst_id = self.get_instances()[-1].get_id()
         xpos    = [inst_id, inst_id]
         
         if self._plot_line is None:
             label = 'PO(' + str(self.get_id()) + ')'
             self._plot_line  = p_settings.axes.plot(xpos, p_ylim, color='r', linestyle='dashed', lw=1)[0]
             self._plot_label = p_settings.axes.text(inst_id, p_ylim[1], label, color='r' )
```

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2023-06-08  0.0.0     SK       Creation
 ## -- 2023-09-12  1.0.0     SK       Release
 ## -- 2023-11-21  1.0.1     SK       Time Stamp update
 ## -- 2024-02-25  1.1.0     SK       Visualisation update
-## -- 2024-04-10  1.2.0     DA/SK    Refactoring
+## -- 2024-04-10  1.2.0     DA/SK    
+## -- 2024-05-07  1.2.1     SK       Bug fix on groupanomaly visualisation
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.2.0 (2024-04-10)
+Ver. 1.2.1 (2024-05-07)
 
 This module provides templates for anomaly detection to be used in the context of online adaptivity.
 """
 
 from mlpro.oa.streams.basics import *
-from mlpro.oa.streams.tasks.anomalydetectors.anomalies import GroupAnomaly
 from mlpro.oa.streams.tasks.anomalydetectors.basics import AnomalyDetector
+from mlpro.oa.streams.tasks.anomalydetectors.anomalies import *
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class AnomalyDetectorPAGA(AnomalyDetector):
     """
@@ -54,16 +55,16 @@
                          p_range_max = p_range_max,
                          p_ada = p_ada,
                          p_duplicate_data = p_duplicate_data,
                          p_visualize = p_visualize,
                          p_logging = p_logging,
                          **p_kwargs)
         
-        self.group_anomalies = []
-        self.group_anomalies_instances = []
+        self.group_anomalies : list[Anomaly] = []
+        self.group_anomalies_instances : list[Instance] = []
         self.group_ano_scores = []
         self.group_anomaly_det = p_group_anomaly_det
 
 
 ## -------------------------------------------------------------------------------------------------
     def _buffer_anomaly(self, p_anomaly):
         """
@@ -78,30 +79,30 @@
         -------
         p_anomaly : Anomaly
             Modified Anomaly object.
         """
 
         if self.group_anomaly_det:
             self.group_anomalies.append(p_anomaly)
-            self.group_anomalies_instances.append(p_anomaly.get_instance()[-1])
+            self.group_anomalies_instances.append(p_anomaly.get_instances()[-1])
             self.group_ano_scores.append(p_anomaly.get_ano_scores())
 
             if len(self.group_anomalies_instances) > 1:
 
-                if int(p_anomaly.get_instance()[-1].get_id()) - 1 == int(self.group_anomalies_instances[-2].get_id()):
+                if int(p_anomaly.get_instances()[-1].get_id()) - 1 == int(self.group_anomalies_instances[-2].get_id()):
 
                     if len(self.group_anomalies_instances) == 3:
 
                         for i in range(2):
                             self.remove_anomaly(self.group_anomalies[i])
                         self._ano_id -= 2
                         anomaly = GroupAnomaly(p_instances=self.group_anomalies_instances,
                                                p_ano_scores=self.group_ano_scores, p_visualize=self._visualize,
                                                p_raising_object=self,
-                                               p_det_time=str(p_anomaly.get_instance()[-1].get_tstamp()))
+                                               p_det_time=str(p_anomaly.get_instances()[-1].get_tstamp()))
                         anomaly.set_id( p_id = self._get_next_anomaly_id() )
                         self._anomalies[anomaly.get_id()] = anomaly
                         self.group_anomalies = []
                         self.group_anomalies.append(anomaly)
                         return anomaly
 
                     elif len(self.group_anomalies_instances) > 3:
@@ -111,19 +112,22 @@
                         
                     else:
                         p_anomaly.set_id( p_id = self._get_next_anomaly_id() )
                         self._anomalies[p_anomaly.get_id()] = p_anomaly
                         return p_anomaly
                     
                 else:
+                    for anomaly in self.group_anomalies:
+                        if isinstance(anomaly, GroupAnomaly):
+                            anomaly.plot_update = False
                     self.group_anomalies = []
                     self.group_anomalies_instances = []
                     self.group_ano_scores = []
                     self.group_anomalies.append(p_anomaly)
-                    self.group_anomalies_instances.append(p_anomaly.get_instance()[-1])
+                    self.group_anomalies_instances.append(p_anomaly.get_instances()[-1])
                     self.group_ano_scores.append(p_anomaly.get_ano_scores())
                     p_anomaly.set_id( p_id = self._get_next_anomaly_id() )
                     self._anomalies[p_anomaly.get_id()] = p_anomaly
                     return p_anomaly
             else:
                 p_anomaly.set_id( p_id = self._get_next_anomaly_id() )
                 self._anomalies[p_anomaly.get_id()] = p_anomaly
```

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/boundarydetectors.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/boundarydetectors.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/basics.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/centroid.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/centroid.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/streams/tasks/normalizers.py` & `mlpro-1.4.3/src/mlpro/oa/streams/tasks/normalizers.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/systems/basics.py` & `mlpro-1.4.3/src/mlpro/oa/systems/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/oa/systems/pool/doublependulum.py` & `mlpro-1.4.3/src/mlpro/oa/systems/pool/doublependulum.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/models.py` & `mlpro-1.4.3/src/mlpro/rl/models.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/models_agents.py` & `mlpro-1.4.3/src/mlpro/rl/models_agents.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/models_env.py` & `mlpro-1.4.3/src/mlpro/rl/models_env.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/models_env_ada.py` & `mlpro-1.4.3/src/mlpro/rl/models_env_ada.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/models_env_oa.py` & `mlpro-1.4.3/src/mlpro/rl/models_env_oa.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/models_train.py` & `mlpro-1.4.3/src/mlpro/rl/models_train.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/pool/actionplanner/mpc.py` & `mlpro-1.4.3/src/mlpro/rl/pool/actionplanner/mpc.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/pool/envs/bglp.py` & `mlpro-1.4.3/src/mlpro/rl/pool/envs/bglp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/pool/envs/cartpole.py` & `mlpro-1.4.3/src/mlpro/rl/pool/envs/cartpole.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/pool/envs/doublependulum.py` & `mlpro-1.4.3/src/mlpro/rl/pool/envs/doublependulum.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/pool/envs/gridworld.py` & `mlpro-1.4.3/src/mlpro/rl/pool/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/pool/envs/robotinhtm.py` & `mlpro-1.4.3/src/mlpro/rl/pool/envs/robotinhtm.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/pool/policies/dummy.py` & `mlpro-1.4.3/src/mlpro/rl/pool/policies/dummy.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/pool/policies/randomgenerator.py` & `mlpro-1.4.3/src/mlpro/rl/pool/policies/randomgenerator.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py` & `mlpro-1.4.3/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py` & `mlpro-1.4.3/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/rl/sciui_rl.py` & `mlpro-1.4.3/src/mlpro/rl/sciui_rl.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/sl/basics.py` & `mlpro-1.4.3/src/mlpro/sl/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py` & `mlpro-1.4.3/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/sl/fnn.py` & `mlpro-1.4.3/src/mlpro/sl/fnn.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/sl/models_eval.py` & `mlpro-1.4.3/src/mlpro/sl/models_eval.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/sl/models_train.py` & `mlpro-1.4.3/src/mlpro/sl/models_train.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py` & `mlpro-1.4.3/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/sl/pool/afct/pytorch.py` & `mlpro-1.4.3/src/mlpro/sl/pool/afct/pytorch.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/wrappers/basics.py` & `mlpro-1.4.3/src/mlpro/wrappers/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro/wrappers/mujoco.py` & `mlpro-1.4.3/src/mlpro/wrappers/mujoco.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/src/mlpro.egg-info/PKG-INFO` & `mlpro-1.4.3/src/mlpro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro
-Version: 1.4.2
+Version: 1.4.3
 Summary: MLPro - The Integrative Middleware Framework for Standardized Machine Learning
 Home-page: https://mlpro.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,17 +15,15 @@
 Provides-Extra: full
 Requires-Dist: dill>=0.3.6; extra == "full"
 Requires-Dist: numpy>=1.24.2; extra == "full"
 Requires-Dist: torch>=2.0.0; extra == "full"
 Requires-Dist: matplotlib>=3.7.1; extra == "full"
 Requires-Dist: scipy>=1.10.1; extra == "full"
 Requires-Dist: multiprocess>=0.70.14; extra == "full"
-Requires-Dist: optuna>=3.1.1; extra == "full"
-Requires-Dist: hyperopt>=0.2.7; extra == "full"
-Requires-Dist: mujoco!=3.1.4,>=2.3.3; extra == "full"
+Requires-Dist: mujoco==3.1.3; extra == "full"
 Requires-Dist: lxml>=4.9.2; extra == "full"
 Requires-Dist: pandas>=2.1.3; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro/badge/?version=latest)](https://mlpro.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro.svg)](https://badge.fury.io/py/mlpro)
 [![Anaconda-Version Badge](https://anaconda.org/mlpro/mlpro/badges/version.svg)](https://anaconda.org/mlpro/mlpro)
```

### Comparing `mlpro-1.4.2/src/mlpro.egg-info/SOURCES.txt` & `mlpro-1.4.3/src/mlpro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/test/test_buffer.py` & `mlpro-1.4.3/test/test_buffer.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/test/test_environment.py` & `mlpro-1.4.3/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/test/test_examples.py` & `mlpro-1.4.3/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/test/test_math.py` & `mlpro-1.4.3/test/test_math.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/test/test_pool_policies.py` & `mlpro-1.4.3/test/test_pool_policies.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.2/test/test_various.py` & `mlpro-1.4.3/test/test_various.py`

 * *Files identical despite different names*

