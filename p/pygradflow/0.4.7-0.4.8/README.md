# Comparing `tmp/pygradflow-0.4.7.tar.gz` & `tmp/pygradflow-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygradflow-0.4.7.tar", max compression
+gzip compressed data, was "pygradflow-0.4.8.tar", max compression
```

## Comparing `pygradflow-0.4.7.tar` & `pygradflow-0.4.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    10847 2024-05-09 15:39:27.182897 pygradflow-0.4.7/LICENSE
--rw-r--r--   0        0        0      984 2024-05-09 15:39:27.182897 pygradflow-0.4.7/README.md
--rw-r--r--   0        0        0        0 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/__init__.py
--rw-r--r--   0        0        0      872 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/active_set.py
--rw-r--r--   0        0        0     4458 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/cons_problem.py
--rw-r--r--   0        0        0     1749 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/controller.py
--rw-r--r--   0        0        0     2487 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/deriv_check.py
--rw-r--r--   0        0        0     4645 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/display.py
--rw-r--r--   0        0        0     4839 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/eval.py
--rw-r--r--   0        0        0     6380 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/implicit_func.py
--rw-r--r--   0        0        0     5146 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/iterate.py
--rw-r--r--   0        0        0       55 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/log.py
--rw-r--r--   0        0        0     6570 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/newton.py
--rw-r--r--   0        0        0     5559 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/params.py
--rw-r--r--   0        0        0     5111 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/penalty.py
--rw-r--r--   0        0        0     5845 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/problem.py
--rw-r--r--   0        0        0        0 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/py.typed
--rw-r--r--   0        0        0     3378 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/runners/cutest_runner.py
--rw-r--r--   0        0        0      366 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/runners/instance.py
--rw-r--r--   0        0        0     2045 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/runners/qplib_runner.py
--rw-r--r--   0        0        0     8326 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/runners/runner.py
--rw-r--r--   0        0        0     5188 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/scale.py
--rw-r--r--   0        0        0    17435 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/solver.py
--rw-r--r--   0        0        0     1284 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/step/__init__.py
--rw-r--r--   0        0        0     4439 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/step/asymmetric_step_solver.py
--rw-r--r--   0        0        0     5877 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/step/box_control.py
--rw-r--r--   0        0        0     2710 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/step/cond_estimate.py
--rw-r--r--   0        0        0     2431 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/step/distance_ratio_control.py
--rw-r--r--   0        0        0     2058 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/exact_control.py
--rw-r--r--   0        0        0     3173 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/extended_step_solver.py
--rw-r--r--   0        0        0      543 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/fixed_control.py
--rw-r--r--   0        0        0     2669 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/linear_solver.py
--rw-r--r--   0        0        0     7417 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/opti_control.py
--rw-r--r--   0        0        0     2014 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/residuum_ratio_control.py
--rw-r--r--   0        0        0     2401 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/scaled_step_solver.py
--rw-r--r--   0        0        0     2467 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/standard_step_solver.py
--rw-r--r--   0        0        0     4697 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/step_control.py
--rw-r--r--   0        0        0     2048 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/step_solver.py
--rw-r--r--   0        0        0     4120 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/symmetric_step_solver.py
--rw-r--r--   0        0        0      380 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/timer.py
--rw-r--r--   0        0        0     1711 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/transform.py
--rw-r--r--   0        0        0      232 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/util.py
--rw-r--r--   0        0        0     1138 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    10847 2024-05-09 16:18:52.182761 pygradflow-0.4.8/LICENSE
+-rw-r--r--   0        0        0      984 2024-05-09 16:18:52.182761 pygradflow-0.4.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/active_set.py
+-rw-r--r--   0        0        0     4458 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/cons_problem.py
+-rw-r--r--   0        0        0     1749 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/controller.py
+-rw-r--r--   0        0        0     2487 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/deriv_check.py
+-rw-r--r--   0        0        0     4645 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/display.py
+-rw-r--r--   0        0        0     4839 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/eval.py
+-rw-r--r--   0        0        0     6380 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/implicit_func.py
+-rw-r--r--   0        0        0     5146 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/iterate.py
+-rw-r--r--   0        0        0       55 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/log.py
+-rw-r--r--   0        0        0     6570 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/newton.py
+-rw-r--r--   0        0        0     5559 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/params.py
+-rw-r--r--   0        0        0     5111 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/penalty.py
+-rw-r--r--   0        0        0     5845 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/problem.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/py.typed
+-rw-r--r--   0        0        0     3378 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/runners/cutest_runner.py
+-rw-r--r--   0        0        0      366 2024-05-09 16:18:52.182761 pygradflow-0.4.8/pygradflow/runners/instance.py
+-rw-r--r--   0        0        0     2045 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/runners/qplib_runner.py
+-rw-r--r--   0        0        0     8326 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/runners/runner.py
+-rw-r--r--   0        0        0     5188 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/scale.py
+-rw-r--r--   0        0        0    17435 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/solver.py
+-rw-r--r--   0        0        0     1284 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/__init__.py
+-rw-r--r--   0        0        0     4439 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/asymmetric_step_solver.py
+-rw-r--r--   0        0        0     5877 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/box_control.py
+-rw-r--r--   0        0        0     2710 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/cond_estimate.py
+-rw-r--r--   0        0        0     2431 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/distance_ratio_control.py
+-rw-r--r--   0        0        0     2058 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/exact_control.py
+-rw-r--r--   0        0        0     3173 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/extended_step_solver.py
+-rw-r--r--   0        0        0      543 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/fixed_control.py
+-rw-r--r--   0        0        0     2669 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/linear_solver.py
+-rw-r--r--   0        0        0     7537 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/opti_control.py
+-rw-r--r--   0        0        0     2014 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/residuum_ratio_control.py
+-rw-r--r--   0        0        0     2401 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/scaled_step_solver.py
+-rw-r--r--   0        0        0     2467 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/standard_step_solver.py
+-rw-r--r--   0        0        0     4697 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/step_control.py
+-rw-r--r--   0        0        0     2048 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/step_solver.py
+-rw-r--r--   0        0        0     4120 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/step/symmetric_step_solver.py
+-rw-r--r--   0        0        0      380 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/timer.py
+-rw-r--r--   0        0        0     1711 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/transform.py
+-rw-r--r--   0        0        0      232 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pygradflow/util.py
+-rw-r--r--   0        0        0     1138 2024-05-09 16:18:52.186761 pygradflow-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.8/PKG-INFO
```

### Comparing `pygradflow-0.4.7/LICENSE` & `pygradflow-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/README.md` & `pygradflow-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/active_set.py` & `pygradflow-0.4.8/pygradflow/active_set.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/cons_problem.py` & `pygradflow-0.4.8/pygradflow/cons_problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/controller.py` & `pygradflow-0.4.8/pygradflow/controller.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/deriv_check.py` & `pygradflow-0.4.8/pygradflow/deriv_check.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/display.py` & `pygradflow-0.4.8/pygradflow/display.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/eval.py` & `pygradflow-0.4.8/pygradflow/eval.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/implicit_func.py` & `pygradflow-0.4.8/pygradflow/implicit_func.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/iterate.py` & `pygradflow-0.4.8/pygradflow/iterate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/newton.py` & `pygradflow-0.4.8/pygradflow/newton.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/params.py` & `pygradflow-0.4.8/pygradflow/params.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/penalty.py` & `pygradflow-0.4.8/pygradflow/penalty.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/problem.py` & `pygradflow-0.4.8/pygradflow/problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/runners/cutest_runner.py` & `pygradflow-0.4.8/pygradflow/runners/cutest_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/runners/qplib_runner.py` & `pygradflow-0.4.8/pygradflow/runners/qplib_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/runners/runner.py` & `pygradflow-0.4.8/pygradflow/runners/runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/scale.py` & `pygradflow-0.4.8/pygradflow/scale.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/solver.py` & `pygradflow-0.4.8/pygradflow/solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/__init__.py` & `pygradflow-0.4.8/pygradflow/step/__init__.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/asymmetric_step_solver.py` & `pygradflow-0.4.8/pygradflow/step/asymmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/box_control.py` & `pygradflow-0.4.8/pygradflow/step/box_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/cond_estimate.py` & `pygradflow-0.4.8/pygradflow/step/cond_estimate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/distance_ratio_control.py` & `pygradflow-0.4.8/pygradflow/step/distance_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/exact_control.py` & `pygradflow-0.4.8/pygradflow/step/exact_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/extended_step_solver.py` & `pygradflow-0.4.8/pygradflow/step/extended_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/fixed_control.py` & `pygradflow-0.4.8/pygradflow/step/fixed_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/linear_solver.py` & `pygradflow-0.4.8/pygradflow/step/linear_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/opti_control.py` & `pygradflow-0.4.8/pygradflow/step/opti_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 
 import cyipopt
 import numpy as np
 
-from pygradflow.eval import astype
+from pygradflow.eval import EvalError, astype
 from pygradflow.implicit_func import ImplicitFunc
 from pygradflow.iterate import Iterate
 from pygradflow.step.step_control import (
     StepController,
     StepControlResult,
     StepSolverError,
 )
@@ -223,20 +223,23 @@
 
         self.set_options(timer)
         x0 = iterate.x
         y0 = iterate.y
         z0 = np.concatenate([x0, y0])
 
         # Solve using Ipopt
-        z, info = super().solve(z0)
+        try:
+            z, info = super().solve(z0)
+        except EvalError:
+            raise StepSolverError("Failed to evaluate subproblem")
 
         assert np.isfinite(z).all()
 
         if info["status"] not in [0, 1]:
-            raise StepSolverError("Ipopt failed to solve the problem")
+            raise StepSolverError("Ipopt failed to solve subproblem")
 
         x = z[: self.prob_num_vars]
         y = info["mult_g"]
 
         return (x, y)
```

### Comparing `pygradflow-0.4.7/pygradflow/step/residuum_ratio_control.py` & `pygradflow-0.4.8/pygradflow/step/residuum_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/scaled_step_solver.py` & `pygradflow-0.4.8/pygradflow/step/scaled_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/standard_step_solver.py` & `pygradflow-0.4.8/pygradflow/step/standard_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/step_control.py` & `pygradflow-0.4.8/pygradflow/step/step_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/step_solver.py` & `pygradflow-0.4.8/pygradflow/step/step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/step/symmetric_step_solver.py` & `pygradflow-0.4.8/pygradflow/step/symmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pygradflow/transform.py` & `pygradflow-0.4.8/pygradflow/transform.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.7/pyproject.toml` & `pygradflow-0.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygradflow"
-version = "0.4.7"
+version = "0.4.8"
 description = "PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs."
 authors = ["Christoph Hansknecht <christoph.hansknecht@tu-clausthal.de>"]
 readme = "README.md"
 repository = "https://github.com/chrhansk/pygradflow"
 documentation = "https://pygradflow.readthedocs.io"
```

### Comparing `pygradflow-0.4.7/PKG-INFO` & `pygradflow-0.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygradflow
-Version: 0.4.7
+Version: 0.4.8
 Summary: PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs.
 Home-page: https://github.com/chrhansk/pygradflow
 Author: Christoph Hansknecht
 Author-email: christoph.hansknecht@tu-clausthal.de
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

