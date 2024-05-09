# Comparing `tmp/jax_fdm-0.8.3.tar.gz` & `tmp/jax_fdm-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_fdm-0.8.3.tar", last modified: Thu Apr 18 20:12:40 2024, max compression
+gzip compressed data, was "jax_fdm-0.8.4.tar", last modified: Thu May  9 14:21:26 2024, max compression
```

## Comparing `jax_fdm-0.8.3.tar` & `jax_fdm-0.8.4.tar`

### file list

```diff
@@ -1,142 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.812622 jax_fdm-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-18 20:12:32.000000 jax_fdm-0.8.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    19537 2024-04-18 20:12:32.000000 jax_fdm-0.8.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-18 20:12:32.000000 jax_fdm-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-18 20:12:32.000000 jax_fdm-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-04-18 20:12:40.812622 jax_fdm-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-04-18 20:12:32.000000 jax_fdm-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-18 20:12:40.812622 jax_fdm-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.788622 jax_fdm-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.792622 jax_fdm-0.8.3/src/jax_fdm/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.796622 jax_fdm-0.8.3/src/jax_fdm/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/constraint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.796622 jax_fdm-0.8.3/src/jax_fdm/constraints/edge/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/edge/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/edge/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/edge/force.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/edge/length.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.796622 jax_fdm-0.8.3/src/jax_fdm/constraints/network/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/network/force.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/network/length.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/network/network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.796622 jax_fdm-0.8.3/src/jax_fdm/constraints/node/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/node/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/node/curvature.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/node/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/constraints/node/tangent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.796622 jax_fdm-0.8.3/src/jax_fdm/datastructures/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/datastructures/datastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/datastructures/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/datastructures/network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.800622 jax_fdm-0.8.3/src/jax_fdm/equilibrium/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/fdm.py
--rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/loads.py
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.800622 jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    10331 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.800622 jax_fdm-0.8.3/src/jax_fdm/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14171 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/geometry/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.800622 jax_fdm-0.8.3/src/jax_fdm/goals/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/abstract_goal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.800622 jax_fdm-0.8.3/src/jax_fdm/goals/edge/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/direction.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/force.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/length.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/edge/loadpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/goal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.804622 jax_fdm-0.8.3/src/jax_fdm/goals/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/mesh/area.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/mesh/laplacian.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/mesh/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.804622 jax_fdm-0.8.3/src/jax_fdm/goals/network/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/network/laplacian.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/network/loadpath.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/network/network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.804622 jax_fdm-0.8.3/src/jax_fdm/goals/node/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/line.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/plane.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/residual.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/node/tangent.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/goals/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.804622 jax_fdm-0.8.3/src/jax_fdm/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/losses/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/losses/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.808622 jax_fdm-0.8.3/src/jax_fdm/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.808622 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/constrained.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/ipopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/second_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/optimization/recorders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.808622 jax_fdm-0.8.3/src/jax_fdm/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/parameters/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/parameters/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/parameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.808622 jax_fdm-0.8.3/src/jax_fdm/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.808622 jax_fdm-0.8.3/src/jax_fdm/visualization/artists/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/artists/network_artist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.808622 jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.812622 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/loss_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/vector_artist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.812622 jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/network_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-18 20:12:33.000000 jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:40.812622 jax_fdm-0.8.3/src/jax_fdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-04-18 20:12:40.000000 jax_fdm-0.8.3/src/jax_fdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-18 20:12:40.000000 jax_fdm-0.8.3/src/jax_fdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:12:40.000000 jax_fdm-0.8.3/src/jax_fdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:12:40.000000 jax_fdm-0.8.3/src/jax_fdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 20:12:40.000000 jax_fdm-0.8.3/src/jax_fdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 20:12:40.000000 jax_fdm-0.8.3/src/jax_fdm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.436887 jax_fdm-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-09 14:21:11.000000 jax_fdm-0.8.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20050 2024-05-09 14:21:11.000000 jax_fdm-0.8.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-09 14:21:11.000000 jax_fdm-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-09 14:21:11.000000 jax_fdm-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-05-09 14:21:26.436887 jax_fdm-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-05-09 14:21:11.000000 jax_fdm-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-09 14:21:26.440887 jax_fdm-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.412887 jax_fdm-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.420887 jax_fdm-0.8.4/src/jax_fdm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.420887 jax_fdm-0.8.4/src/jax_fdm/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/constraint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.420887 jax_fdm-0.8.4/src/jax_fdm/constraints/edge/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/edge/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/edge/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/edge/force.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/edge/length.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.420887 jax_fdm-0.8.4/src/jax_fdm/constraints/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/network/force.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/network/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/network/network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.424887 jax_fdm-0.8.4/src/jax_fdm/constraints/node/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/node/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/node/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/node/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/constraints/node/tangent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.424887 jax_fdm-0.8.4/src/jax_fdm/datastructures/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/datastructures/datastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/datastructures/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/datastructures/network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.424887 jax_fdm-0.8.4/src/jax_fdm/equilibrium/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/equilibrium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/equilibrium/fdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/equilibrium/loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/equilibrium/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/equilibrium/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/equilibrium/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/equilibrium/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.424887 jax_fdm-0.8.4/src/jax_fdm/equilibrium/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/equilibrium/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/equilibrium/structures/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10331 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/equilibrium/structures/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/equilibrium/structures/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.424887 jax_fdm-0.8.4/src/jax_fdm/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14171 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/geometry/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.428887 jax_fdm-0.8.4/src/jax_fdm/goals/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/abstract_goal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.428887 jax_fdm-0.8.4/src/jax_fdm/goals/edge/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/edge/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/edge/direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/edge/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/edge/force.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/edge/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/edge/loadpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/goal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.428887 jax_fdm-0.8.4/src/jax_fdm/goals/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/mesh/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/mesh/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/mesh/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.428887 jax_fdm-0.8.4/src/jax_fdm/goals/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/network/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/network/loadpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/network/smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.432887 jax_fdm-0.8.4/src/jax_fdm/goals/node/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/node/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/node/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/node/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/node/plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/node/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/node/residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/node/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/node/tangent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/goals/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.432887 jax_fdm-0.8.4/src/jax_fdm/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/losses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/losses/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.432887 jax_fdm-0.8.4/src/jax_fdm/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/optimization/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.432887 jax_fdm-0.8.4/src/jax_fdm/optimization/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/optimization/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/optimization/optimizers/constrained.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/optimization/optimizers/ipopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/optimization/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/optimization/optimizers/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/optimization/optimizers/second_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/optimization/recorders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.432887 jax_fdm-0.8.4/src/jax_fdm/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/parameters/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/parameters/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/parameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.436887 jax_fdm-0.8.4/src/jax_fdm/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.436887 jax_fdm-0.8.4/src/jax_fdm/visualization/artists/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/artists/network_artist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.436887 jax_fdm-0.8.4/src/jax_fdm/visualization/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/notebooks/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/notebooks/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/notebooks/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/notebooks/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.436887 jax_fdm-0.8.4/src/jax_fdm/visualization/plotters/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/plotters/loss_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/plotters/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/plotters/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/plotters/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/plotters/vector_artist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.436887 jax_fdm-0.8.4/src/jax_fdm/visualization/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/viewers/network_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/viewers/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-09 14:21:12.000000 jax_fdm-0.8.4/src/jax_fdm/visualization/viewers/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:21:26.436887 jax_fdm-0.8.4/src/jax_fdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-05-09 14:21:26.000000 jax_fdm-0.8.4/src/jax_fdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-09 14:21:26.000000 jax_fdm-0.8.4/src/jax_fdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:21:26.000000 jax_fdm-0.8.4/src/jax_fdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:21:26.000000 jax_fdm-0.8.4/src/jax_fdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 14:21:26.000000 jax_fdm-0.8.4/src/jax_fdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 14:21:26.000000 jax_fdm-0.8.4/src/jax_fdm.egg-info/top_level.txt
```

### Comparing `jax_fdm-0.8.3/CHANGELOG.md` & `jax_fdm-0.8.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## Unreleased
+## [0.8.4] 2024-05-09
 
 ### Added
 
+- Added `NetworkSmoothGoal` to smoothen the shape of a network based on the fairness energy of its nodes w.r.t. their immediate neighborhood.
+- Implemented `Graph.adjacency` to access the connectivity among nodes/vertices to compute new goals. 
+- Added `adjacency_matrix` as numpy-only function to assemble `Graph.adjacency`. The function is largely inspired by `compas.matrices.adjacency_matrix`.
+
 ### Changed
 
+- Now we use `time.perf_counter` instead of `time.time` to measure logic execution time more accurately.
+
 ### Removed
 
 
 ## [0.8.3] 2024-04-18
 
 ### Added
```

### Comparing `jax_fdm-0.8.3/LICENSE` & `jax_fdm-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/PKG-INFO` & `jax_fdm-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax_fdm
-Version: 0.8.3
+Version: 0.8.4
 Summary: Auto-differentiable and hardware-accelerated force density method
 Home-page: https://github.com/arpastrana/jax_fdm
 Author: Rafael Pastrana
 Author-email: arpastrana@princeton.edu
 License: MIT license
 Keywords: jax,automatic-differentiation,architecture,form-finding,structural-design
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jax_fdm-0.8.3/README.md` & `jax_fdm-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/setup.cfg` & `jax_fdm-0.8.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/setup.py` & `jax_fdm-0.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 long_description = read("README.md")
 requirements = read("requirements.txt").split("\n")
 optional_requirements = {}
 
 setup(
     name="jax_fdm",
-    version="0.8.3",
+    version="0.8.4",
     description="Auto-differentiable and hardware-accelerated force density method",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arpastrana/jax_fdm",
     author="Rafael Pastrana",
     author_email="arpastrana@princeton.edu",
     license="MIT license",
```

### Comparing `jax_fdm-0.8.3/src/jax_fdm/__init__.py` & `jax_fdm-0.8.4/src/jax_fdm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import jax.numpy as jnp
 
 
 __author__ = ["Rafael Pastrana"]
 __copyright__ = "Rafael Pastrana"
 __license__ = "MIT License"
 __email__ = "arpastrana@princeton.edu"
-__version__ = "0.8.3"
+__version__ = "0.8.4"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
```

### Comparing `jax_fdm-0.8.3/src/jax_fdm/constraints/constraint.py` & `jax_fdm-0.8.4/src/jax_fdm/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/constraints/edge/angle.py` & `jax_fdm-0.8.4/src/jax_fdm/constraints/edge/angle.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/constraints/node/coordinates.py` & `jax_fdm-0.8.4/src/jax_fdm/constraints/node/coordinates.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/constraints/node/curvature.py` & `jax_fdm-0.8.4/src/jax_fdm/constraints/node/curvature.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/constraints/node/normal.py` & `jax_fdm-0.8.4/src/jax_fdm/constraints/node/normal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/constraints/node/tangent.py` & `jax_fdm-0.8.4/src/jax_fdm/constraints/node/tangent.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/datastructures/datastructure.py` & `jax_fdm-0.8.4/src/jax_fdm/datastructures/datastructure.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/datastructures/mesh.py` & `jax_fdm-0.8.4/src/jax_fdm/datastructures/mesh.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/datastructures/network.py` & `jax_fdm-0.8.4/src/jax_fdm/datastructures/network.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/equilibrium/fdm.py` & `jax_fdm-0.8.4/src/jax_fdm/equilibrium/fdm.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/equilibrium/loads.py` & `jax_fdm-0.8.4/src/jax_fdm/equilibrium/loads.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/equilibrium/models.py` & `jax_fdm-0.8.4/src/jax_fdm/equilibrium/models.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/equilibrium/solvers.py` & `jax_fdm-0.8.4/src/jax_fdm/equilibrium/solvers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/equilibrium/sparse.py` & `jax_fdm-0.8.4/src/jax_fdm/equilibrium/sparse.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/equilibrium/states.py` & `jax_fdm-0.8.4/src/jax_fdm/equilibrium/states.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/mixins.py` & `jax_fdm-0.8.4/src/jax_fdm/equilibrium/structures/mixins.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/structures.py` & `jax_fdm-0.8.4/src/jax_fdm/equilibrium/structures/structures.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/equilibrium/structures/topology.py` & `jax_fdm-0.8.4/src/jax_fdm/equilibrium/structures/topology.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import numpy as np
+from scipy.sparse import coo_matrix
 
 import jax
 import jax.numpy as jnp
 
 import equinox as eqx
 
 from compas.numerical import connectivity_matrix
 from compas.numerical import face_matrix as compas_face_matrix
 from compas.utilities import pairwise
 
 from jax.experimental.sparse import BCOO
 
+from jax_fdm import DTYPE_NP
 from jax_fdm import DTYPE_INT_NP
 from jax_fdm import DTYPE_JAX
 
 from jax_fdm.equilibrium.structures.mixins import IndexingMixins
 from jax_fdm.equilibrium.structures.mixins import MeshIndexingMixins
 
 
@@ -26,23 +28,25 @@
     """
     A graph.
     """
     nodes: np.ndarray
     edges: np.ndarray
     edges_indexed: jax.Array
     connectivity: jax.Array
+    adjacency: jax.Array
 
     def __init__(self, nodes, edges):
         self.nodes = nodes
 
         assert edges.shape[1] == 2, "Edges in graph must connect exactly 2 nodes"
         self.edges = edges
         self.edges_indexed = self._edges_indexed()
 
         self.connectivity = self._connectivity_matrix()
+        self.adjacency = self._adjacency_matrix()
 
     @property
     def num_nodes(self):
         """
         The number of nodes.
         """
         return self.nodes.size
@@ -58,14 +62,22 @@
         """
         The connectivity matrix between edges and nodes.
         """
         edges_indexed = self.edges_indexed
 
         return jnp.array(connectivity_matrix(edges_indexed, "array"), dtype=DTYPE_JAX)
 
+    def _adjacency_matrix(self):
+        """
+        The adjacency matrix between nodes and nodes.
+        """
+        edges_indexed = self.edges_indexed
+
+        return jnp.array(adjacency_matrix(edges_indexed, "array"), dtype=DTYPE_JAX)
+
 
 class GraphSparse(Graph):
     """
     A sparse graph.
     """
     def _connectivity_matrix(self):
         """
@@ -111,14 +123,24 @@
         The connectivity matrix between edges and nodes in SciPy CSC format.
         """
         # TODO: Refactor GraphSparse to return a JAX sparse matrix instead
         edges_indexed = self.edges_indexed
 
         return connectivity_matrix(edges_indexed, "csc")
 
+    def _adjacency_matrix(self):
+        """
+        The adjacency matrix between nodes and nodes.
+        """
+        edges_indexed = self.edges_indexed
+
+        A = adjacency_matrix(edges_indexed, "coo")
+
+        return BCOO.from_scipy_sparse(A).todense()
+
 
 # ==========================================================================
 # Mesh
 # ==========================================================================
 
 class Mesh(Graph, MeshIndexingMixins):
     """
@@ -327,17 +349,62 @@
     for face in face_vertices:
         face_clean = [vertex for vertex in face if vertex >= 0]
         face_vertices_clean.append(face_clean)
 
     return compas_face_matrix(face_vertices_clean, rtype, normalize)
 
 
+def adjacency_matrix(edges, rtype="array"):
+    """
+    Creates a vertex-vertex adjacency matrix.
+
+    It expects that vertices / nodes are continuously indexed (no skips),
+    and that edges are indexed from 0 to len(vertices) / len(nodes).
+    """
+    num_vertices = np.max(np.ravel(edges)) + 1
+
+    # rows and columns indices for the COO format
+    rows = np.hstack([edges[:, 0], edges[:, 1]])  # add edges in both directions for undirected graph
+    cols = np.hstack([edges[:, 1], edges[:, 0]])
+
+    # data to fill in (all 1s for the existence of edges)
+    data = np.ones(len(rows), dtype=DTYPE_NP)
+
+    # create the COO matrix
+    A = coo_matrix(
+        (data, (rows, cols)),
+        shape=(num_vertices, num_vertices)
+    )
+
+    # convert to floating point matrix
+    return _return_matrix(A.asfptype(), rtype)
+
+
+def _return_matrix(M, rtype):
+    if rtype == "list":
+        return M.toarray().tolist()
+    if rtype == "array":
+        return M.toarray()
+    if rtype == "csr":
+        return M.tocsr()
+    if rtype == "csc":
+        return M.tocsc()
+    if rtype == "coo":
+        return M.tocoo()
+    return M
+
+
+# ==========================================================================
+# Main
+# ==========================================================================
+
 if __name__ == "__main__":
 
     from compas.datastructures import Mesh as CMesh
+    from compas.numerical import adjacency_matrix as adjacency_matrix_compas
 
     num_nodes = 5
     nodes = list(range(num_nodes))
     edges = [edge for edge in pairwise(nodes)]
 
     nodes = jnp.array(nodes, dtype=jnp.int64)
     edges = jnp.array(edges, dtype=jnp.int64)
@@ -370,24 +437,34 @@
 
     assert jnp.allclose(graph_sparse.connectivity,
                         graph.connectivity)
 
     cmesh = CMesh.from_meshgrid(2.0, 2)
     print(cmesh)
 
+    # test connectivity edges faces
     C = mesh_connectivity_edges_faces(cmesh)
     cmesh_faces = [cmesh.face_vertices(fkey) for fkey in cmesh.faces()]
     # cmesh_faces[0].append(-1)
 
     vertices_array = np.asarray(list(cmesh.vertices()))
     faces_array = np.asarray(cmesh_faces)
     edges_array = np.asarray(list(cmesh.edges()))
     mesh = MeshSparse(vertices_array, faces_array, edges_array)
 
-    jnp.allclose(C, mesh.connectivity_edges_faces.todense())
+    jnp.allclose(C, mesh.connectivity_edges_faces)
+
+    # test adjacency matrix
+    vertex_index = cmesh.vertex_index()
+    adjacency = [[vertex_index[nbr] for nbr in cmesh.vertex_neighbors(vertex)] for vertex in cmesh.vertices()]
+    A_c = adjacency_matrix_compas(adjacency, rtype="array")
+
+    A = mesh.adjacency.todense()
+    jnp.allclose(A, A_c)
+
     # def f(g):
     #     return jnp.sum(jnp.square(g.nodes - 1.0))
 
     # y = f(graph)
     # print(y)
 
     # from jax import jit
```

### Comparing `jax_fdm-0.8.3/src/jax_fdm/geometry/geometry.py` & `jax_fdm-0.8.4/src/jax_fdm/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/abstract_goal.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/abstract_goal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/edge/angle.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/edge/angle.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/edge/direction.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/edge/direction.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/edge/edge.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/edge/edge.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/edge/force.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/edge/force.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/edge/length.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/edge/length.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/goal.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/goal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/helpers.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/helpers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/mesh/area.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/mesh/area.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/mesh/laplacian.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/mesh/laplacian.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/network/laplacian.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/network/laplacian.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/network/loadpath.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/network/loadpath.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/node/coordinates.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/node/coordinates.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/node/line.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/node/line.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/node/node.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/node/node.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/node/normal.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/node/normal.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/node/plane.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/node/plane.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/node/residual.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/node/residual.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/goals/node/tangent.py` & `jax_fdm-0.8.4/src/jax_fdm/goals/node/tangent.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/losses/errors.py` & `jax_fdm-0.8.4/src/jax_fdm/losses/errors.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/losses/loss.py` & `jax_fdm-0.8.4/src/jax_fdm/losses/loss.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/optimization/collections.py` & `jax_fdm-0.8.4/src/jax_fdm/optimization/collections.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/constrained.py` & `jax_fdm-0.8.4/src/jax_fdm/optimization/optimizers/constrained.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/ipopt.py` & `jax_fdm-0.8.4/src/jax_fdm/optimization/optimizers/ipopt.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/optimizer.py` & `jax_fdm-0.8.4/src/jax_fdm/optimization/optimizers/optimizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A gradient-based optimizer.
 """
-from time import time
+from time import perf_counter
 from itertools import groupby
 from functools import partial
 
 import jax.numpy as jnp
 
 from jax import jit
 from jax import grad
@@ -126,54 +126,36 @@
 
         loss_fn = partial(self.loss, loss=loss, model=model, structure=structure)
         loss_and_grad_fn = value_and_grad(loss_fn)
         if jit_fn:
             loss_and_grad_fn = jit(loss_and_grad_fn)
 
         print("Warming up the pressure cooker...")
-        start_time = time()
+        start_time = perf_counter()
         loss_val, grad_val = loss_and_grad_fn(x)
-        print(f"\tLoss and grad warmup time: {(time() - start_time):.4} seconds")
+        print(f"\tLoss and grad warmup time: {(perf_counter() - start_time):.4} seconds")
         print(f"\tInitial loss value: {loss_val:.4}")
         print(f"\tInitial gradient norm: {jnp.linalg.norm(grad_val):.4}")
         assert jnp.sum(jnp.isnan(grad_val)) == 0, "NaNs found in gradient calculation!"
 
-        # print("Warming up the pressure cooker...")
-        # start_time = time()
-        # loss_val = loss(x)
-        # print(f"\tInitial loss value: {loss_val:.4}")
-        # print(f"\tLoss warmup time: {(time() - start_time):.4} seconds")
-
-        # gradient of the loss function
-        # if jit_fn:
-        #     grad_loss = self.gradient(loss)  # w.r.t. first function argument
-        # else:
-        #     grad_loss = grad(loss)
-
-        # start_time = time()
-        # g = grad_loss(x)
-        # assert jnp.sum(jnp.isnan(g)) == 0, "NaNs found in gradient calculation!"
-        # print(f"\tInitial gradient norm: {jnp.linalg.norm(g):.4}")
-        # print(f"\tGradient warmup time: {(time() - start_time):.4} seconds")
-
         # gradient of the loss function
         hessian_fn = self.hessian(loss_fn)  # w.r.t. first function argument
         if hessian_fn:
             if jit_fn:
                 hessian_fn = jit(hessian_fn)
-            start_time = time()
+            start_time = perf_counter()
             _ = hessian_fn(x)
-            print(f"\tHessian warmup time: {(time() - start_time):.4} seconds")
+            print(f"\tHessian warmup time: {(perf_counter() - start_time):.4} seconds")
 
         # constraints
         constraints = constraints or []
         if constraints:
-            start_time = time()
+            start_time = perf_counter()
             constraints = self.constraints(constraints, model, structure, x)
-            print(f"\tConstraints warmup time: {(time() - start_time):.4} seconds")
+            print(f"\tConstraints warmup time: {(perf_counter() - start_time):.4} seconds")
 
         opt_kwargs = {"fun": loss_and_grad_fn,
                       "jac": True,
                       "hess": hessian_fn,
                       "method": self.name,
                       "x0": x,
                       "tol": tol,
@@ -185,25 +167,25 @@
         return opt_kwargs
 
     def solve(self, opt_problem):
         """
         Solve an optimization problem by minimizing a loss function via gradient descent.
         """
         print(f"Optimization with {self.name} started...")
-        start_time = time()
+        start_time = perf_counter()
 
         # minimize
         res_q = self._minimize(opt_problem)
         loss_and_grad_fn = opt_problem["fun"]
         loss_val, grad_val = loss_and_grad_fn(res_q.x)
 
         print(res_q.message)
         print(f"Final gradient norm: {jnp.linalg.norm(grad_val):.4}")
         print(f"Final loss in {res_q.nit} iterations: {res_q.fun:.4}")
-        print(f"Optimization elapsed time: {time() - start_time} seconds")
+        print(f"Optimization elapsed time: {perf_counter() - start_time} seconds")
 
         return res_q.x
 
     @staticmethod
     def _minimize(opt_problem):
         """
         Scipy backend method to minimize a loss function.
```

### Comparing `jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/scipy.py` & `jax_fdm-0.8.4/src/jax_fdm/optimization/optimizers/scipy.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/optimization/optimizers/second_order.py` & `jax_fdm-0.8.4/src/jax_fdm/optimization/optimizers/second_order.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/optimization/recorders.py` & `jax_fdm-0.8.4/src/jax_fdm/optimization/recorders.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/parameters/helpers.py` & `jax_fdm-0.8.4/src/jax_fdm/parameters/helpers.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/parameters/manager.py` & `jax_fdm-0.8.4/src/jax_fdm/parameters/manager.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/parameters/parameters.py` & `jax_fdm-0.8.4/src/jax_fdm/parameters/parameters.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/visualization/artists/network_artist.py` & `jax_fdm-0.8.4/src/jax_fdm/visualization/artists/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/network_artist.py` & `jax_fdm-0.8.4/src/jax_fdm/visualization/notebooks/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/shapes.py` & `jax_fdm-0.8.4/src/jax_fdm/visualization/notebooks/shapes.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/visualization/notebooks/viewer.py` & `jax_fdm-0.8.4/src/jax_fdm/visualization/notebooks/viewer.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/loss_plotter.py` & `jax_fdm-0.8.4/src/jax_fdm/visualization/plotters/loss_plotter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from time import time
+from time import perf_counter
 
 import matplotlib.pyplot as plt
 
 import numpy as np
 
 from jax import vmap
 
@@ -25,15 +25,15 @@
         self.fig = plt.figure(**kwargs)
 
     def plot(self, history, print_breakdown=True, plot_legend=True):
         """
         Plot the loss function and its error components on a list of fdm parameter states.
         """
         print("\nPlotting loss function...")
-        start_time = time()
+        start_time = perf_counter()
 
         # Create batched parameter state
         params = jtu.tree_map(lambda leaf: jnp.asarray(leaf, dtype=DTYPE_JAX),
                               history,
                               is_leaf=lambda y: isinstance(y, list))
 
         # Model is dense because it dense supports vmapping and sparse does not
@@ -72,15 +72,15 @@
         plt.ylabel("Loss")
         plt.yscale("log")
         plt.grid()
 
         if plot_legend:
             plt.legend()
 
-        print(f"Plotting time: {(time() - start_time):.4} seconds")
+        print(f"Plotting time: {(perf_counter() - start_time):.4} seconds")
 
         return losses
 
     def show(self):
         """
         Display the plot.
         """
```

### Comparing `jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/network_artist.py` & `jax_fdm-0.8.4/src/jax_fdm/visualization/plotters/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/register.py` & `jax_fdm-0.8.4/src/jax_fdm/visualization/plotters/register.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/visualization/plotters/vector_artist.py` & `jax_fdm-0.8.4/src/jax_fdm/visualization/plotters/vector_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/network_artist.py` & `jax_fdm-0.8.4/src/jax_fdm/visualization/viewers/network_artist.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm/visualization/viewers/viewer.py` & `jax_fdm-0.8.4/src/jax_fdm/visualization/viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `jax_fdm-0.8.3/src/jax_fdm.egg-info/PKG-INFO` & `jax_fdm-0.8.4/src/jax_fdm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax_fdm
-Version: 0.8.3
+Version: 0.8.4
 Summary: Auto-differentiable and hardware-accelerated force density method
 Home-page: https://github.com/arpastrana/jax_fdm
 Author: Rafael Pastrana
 Author-email: arpastrana@princeton.edu
 License: MIT license
 Keywords: jax,automatic-differentiation,architecture,form-finding,structural-design
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jax_fdm-0.8.3/src/jax_fdm.egg-info/SOURCES.txt` & `jax_fdm-0.8.4/src/jax_fdm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 src/jax_fdm/goals/mesh/area.py
 src/jax_fdm/goals/mesh/laplacian.py
 src/jax_fdm/goals/mesh/mesh.py
 src/jax_fdm/goals/network/__init__.py
 src/jax_fdm/goals/network/laplacian.py
 src/jax_fdm/goals/network/loadpath.py
 src/jax_fdm/goals/network/network.py
+src/jax_fdm/goals/network/smoothing.py
 src/jax_fdm/goals/node/__init__.py
 src/jax_fdm/goals/node/coordinates.py
 src/jax_fdm/goals/node/line.py
 src/jax_fdm/goals/node/node.py
 src/jax_fdm/goals/node/normal.py
 src/jax_fdm/goals/node/plane.py
 src/jax_fdm/goals/node/point.py
```

