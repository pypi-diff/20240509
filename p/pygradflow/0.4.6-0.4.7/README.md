# Comparing `tmp/pygradflow-0.4.6.tar.gz` & `tmp/pygradflow-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygradflow-0.4.6.tar", max compression
+gzip compressed data, was "pygradflow-0.4.7.tar", max compression
```

## Comparing `pygradflow-0.4.6.tar` & `pygradflow-0.4.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    10847 2024-05-07 21:24:07.510948 pygradflow-0.4.6/LICENSE
--rw-r--r--   0        0        0      984 2024-05-07 21:24:07.510948 pygradflow-0.4.6/README.md
--rw-r--r--   0        0        0        0 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/__init__.py
--rw-r--r--   0        0        0      872 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/active_set.py
--rw-r--r--   0        0        0     4458 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/cons_problem.py
--rw-r--r--   0        0        0     1749 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/controller.py
--rw-r--r--   0        0        0     2487 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/deriv_check.py
--rw-r--r--   0        0        0     4645 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/display.py
--rw-r--r--   0        0        0     4839 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/eval.py
--rw-r--r--   0        0        0     6380 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/implicit_func.py
--rw-r--r--   0        0        0     5146 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/iterate.py
--rw-r--r--   0        0        0       55 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/log.py
--rw-r--r--   0        0        0     6570 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/newton.py
--rw-r--r--   0        0        0     5173 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/params.py
--rw-r--r--   0        0        0     5111 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/penalty.py
--rw-r--r--   0        0        0     5845 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/problem.py
--rw-r--r--   0        0        0        0 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/py.typed
--rw-r--r--   0        0        0     3378 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/runners/cutest_runner.py
--rw-r--r--   0        0        0      366 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/runners/instance.py
--rw-r--r--   0        0        0     2045 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/runners/qplib_runner.py
--rw-r--r--   0        0        0     8326 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/runners/runner.py
--rw-r--r--   0        0        0     4181 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/scale.py
--rw-r--r--   0        0        0    16537 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/solver.py
--rw-r--r--   0        0        0     1284 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/step/__init__.py
--rw-r--r--   0        0        0     4439 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/step/asymmetric_step_solver.py
--rw-r--r--   0        0        0     5877 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/step/box_control.py
--rw-r--r--   0        0        0     2710 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/step/cond_estimate.py
--rw-r--r--   0        0        0     2431 2024-05-07 21:24:07.510948 pygradflow-0.4.6/pygradflow/step/distance_ratio_control.py
--rw-r--r--   0        0        0     2058 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/step/exact_control.py
--rw-r--r--   0        0        0     3173 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/step/extended_step_solver.py
--rw-r--r--   0        0        0      543 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/step/fixed_control.py
--rw-r--r--   0        0        0     2669 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/step/linear_solver.py
--rw-r--r--   0        0        0     7327 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/step/opti_control.py
--rw-r--r--   0        0        0     2014 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/step/residuum_ratio_control.py
--rw-r--r--   0        0        0     2401 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/step/scaled_step_solver.py
--rw-r--r--   0        0        0     2467 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/step/standard_step_solver.py
--rw-r--r--   0        0        0     4697 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/step/step_control.py
--rw-r--r--   0        0        0     2048 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/step/step_solver.py
--rw-r--r--   0        0        0     4120 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/step/symmetric_step_solver.py
--rw-r--r--   0        0        0      380 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/timer.py
--rw-r--r--   0        0        0     1711 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/transform.py
--rw-r--r--   0        0        0      232 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pygradflow/util.py
--rw-r--r--   0        0        0     1138 2024-05-07 21:24:07.514948 pygradflow-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0    10847 2024-05-09 15:39:27.182897 pygradflow-0.4.7/LICENSE
+-rw-r--r--   0        0        0      984 2024-05-09 15:39:27.182897 pygradflow-0.4.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/active_set.py
+-rw-r--r--   0        0        0     4458 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/cons_problem.py
+-rw-r--r--   0        0        0     1749 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/controller.py
+-rw-r--r--   0        0        0     2487 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/deriv_check.py
+-rw-r--r--   0        0        0     4645 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/display.py
+-rw-r--r--   0        0        0     4839 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/eval.py
+-rw-r--r--   0        0        0     6380 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/implicit_func.py
+-rw-r--r--   0        0        0     5146 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/iterate.py
+-rw-r--r--   0        0        0       55 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/log.py
+-rw-r--r--   0        0        0     6570 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/newton.py
+-rw-r--r--   0        0        0     5559 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/params.py
+-rw-r--r--   0        0        0     5111 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/penalty.py
+-rw-r--r--   0        0        0     5845 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/problem.py
+-rw-r--r--   0        0        0        0 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/py.typed
+-rw-r--r--   0        0        0     3378 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/runners/cutest_runner.py
+-rw-r--r--   0        0        0      366 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/runners/instance.py
+-rw-r--r--   0        0        0     2045 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/runners/qplib_runner.py
+-rw-r--r--   0        0        0     8326 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/runners/runner.py
+-rw-r--r--   0        0        0     5188 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/scale.py
+-rw-r--r--   0        0        0    17435 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/solver.py
+-rw-r--r--   0        0        0     1284 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/step/__init__.py
+-rw-r--r--   0        0        0     4439 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/step/asymmetric_step_solver.py
+-rw-r--r--   0        0        0     5877 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/step/box_control.py
+-rw-r--r--   0        0        0     2710 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/step/cond_estimate.py
+-rw-r--r--   0        0        0     2431 2024-05-09 15:39:27.182897 pygradflow-0.4.7/pygradflow/step/distance_ratio_control.py
+-rw-r--r--   0        0        0     2058 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/exact_control.py
+-rw-r--r--   0        0        0     3173 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/extended_step_solver.py
+-rw-r--r--   0        0        0      543 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/fixed_control.py
+-rw-r--r--   0        0        0     2669 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/linear_solver.py
+-rw-r--r--   0        0        0     7417 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/opti_control.py
+-rw-r--r--   0        0        0     2014 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/residuum_ratio_control.py
+-rw-r--r--   0        0        0     2401 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/scaled_step_solver.py
+-rw-r--r--   0        0        0     2467 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/standard_step_solver.py
+-rw-r--r--   0        0        0     4697 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/step_control.py
+-rw-r--r--   0        0        0     2048 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/step_solver.py
+-rw-r--r--   0        0        0     4120 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/step/symmetric_step_solver.py
+-rw-r--r--   0        0        0      380 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/timer.py
+-rw-r--r--   0        0        0     1711 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/transform.py
+-rw-r--r--   0        0        0      232 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pygradflow/util.py
+-rw-r--r--   0        0        0     1138 2024-05-09 15:39:27.186897 pygradflow-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.7/PKG-INFO
```

### Comparing `pygradflow-0.4.6/LICENSE` & `pygradflow-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/README.md` & `pygradflow-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/active_set.py` & `pygradflow-0.4.7/pygradflow/active_set.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/cons_problem.py` & `pygradflow-0.4.7/pygradflow/cons_problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/controller.py` & `pygradflow-0.4.7/pygradflow/controller.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/deriv_check.py` & `pygradflow-0.4.7/pygradflow/deriv_check.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/display.py` & `pygradflow-0.4.7/pygradflow/display.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/eval.py` & `pygradflow-0.4.7/pygradflow/eval.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/implicit_func.py` & `pygradflow-0.4.7/pygradflow/implicit_func.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/iterate.py` & `pygradflow-0.4.7/pygradflow/iterate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/newton.py` & `pygradflow-0.4.7/pygradflow/newton.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/params.py` & `pygradflow-0.4.7/pygradflow/params.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,14 +121,35 @@
     CheckSecond = 1 << 1
     """
     Check Hessian of Lagrangian (:math:`\\nabla_{xx} \\mathcal{L}(x, y)`)
     """
     CheckAll = CheckFirst | CheckSecond
 
 
+class ScalingType(Enum):
+    """
+    How to scale the problem
+    """
+
+    NoScaling = auto()
+    """
+    No scaling
+    """
+
+    GradJac = auto()
+    """
+    Scale based on gradient and equilibration of constraint Jacobian
+    """
+
+    Custom = auto()
+    """
+    User-provided custom scaling
+    """
+
+
 @dataclass
 class Params:
     """
     Parameters used to solve a :py:class:`pygradflow.problem.Problem`
     using a :py:class:`pygradflow.solver.Solver`
     """
 
@@ -165,14 +186,17 @@
 
     deriv_check: DerivCheck = DerivCheck.NoCheck
     deriv_pert: float = 1e-8
     deriv_tol: float = 1e-4
 
     precision: Precision = Precision.Double
 
+    scaling_type: ScalingType = ScalingType.NoScaling
+    scaling: object = None
+
     validate_input: bool = True
 
     iteration_limit: Optional[int] = None
     time_limit: float = float(np.inf)
     display_interval: float = 0.1
 
     # lower bound on objective function value,
```

### Comparing `pygradflow-0.4.6/pygradflow/penalty.py` & `pygradflow-0.4.7/pygradflow/penalty.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/problem.py` & `pygradflow-0.4.7/pygradflow/problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/runners/cutest_runner.py` & `pygradflow-0.4.7/pygradflow/runners/cutest_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/runners/qplib_runner.py` & `pygradflow-0.4.7/pygradflow/runners/qplib_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/runners/runner.py` & `pygradflow-0.4.7/pygradflow/runners/runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/solver.py` & `pygradflow-0.4.7/pygradflow/solver.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 
 from pygradflow.display import Format, problem_display
 from pygradflow.eval import Evaluator, SimpleEvaluator, ValidatingEvaluator
 from pygradflow.iterate import Iterate
 from pygradflow.log import logger
 from pygradflow.newton import newton_method
-from pygradflow.params import Params
+from pygradflow.params import Params, ScalingType
 from pygradflow.penalty import penalty_strategy
 from pygradflow.problem import Problem
 from pygradflow.scale import Scaling
 from pygradflow.step.step_control import (
     StepController,
     StepControlResult,
     step_controller,
@@ -192,41 +192,27 @@
     conditions.
     """
 
     def __init__(
         self,
         problem: Problem,
         params: Params = Params(),
-        scaling: Optional[Scaling] = None,
     ) -> None:
         """
         Creates a new solver
 
         Parameters
         ----------
         problem: pygradflow.problem.Problem
             The problem to be solved
         params: pygradflow.params.Params
             Parameters used by the solver
         """
         self.orig_problem = problem
         self.params = params
-        self.scaling = scaling
-
-        self.transform = Transformation(problem, params, scaling)
-
-        self.problem = self.transform.trans_problem
-
-        if params.validate_input:
-            self.evaluator: Evaluator = ValidatingEvaluator(self.problem, params)
-        else:
-            self.evaluator = SimpleEvaluator(self.problem, params)
-
-        self.penalty = penalty_strategy(self.problem, params)
-        self.rho = -1.0
 
     def compute_step(
         self,
         controller: StepController,
         iterate: Iterate,
         dt: float,
         display: bool,
@@ -341,14 +327,76 @@
         (x_init, y_init) = transform.transform_sol(x_init, y_init)
 
         x = x_init.astype(dtype)
         y = y_init.astype(dtype)
 
         return Iterate(problem, params, x, y, self.evaluator)
 
+    def _create_scaling(self, x0):
+        params = self.params
+        problem = self.orig_problem
+
+        scaling_type = params.scaling_type
+
+        if params.scaling is not None:
+            assert scaling_type == ScalingType.Custom
+            return params.scaling
+
+        if scaling_type == ScalingType.NoScaling:
+            return None
+        elif scaling_type == ScalingType.GradJac:
+            obj_grad = problem.obj_grad(x0)
+            cons_jac = None
+            if problem.num_cons > 0:
+                cons_jac = problem.cons_jac(x0)
+
+            return Scaling.from_grad_jac(obj_grad, cons_jac)
+        elif scaling_type == ScalingType.Custom:
+            raise ValueError("Custom scaling requires explicit scaling")
+        else:
+            raise ValueError(f"Unknown scaling type {scaling_type}")
+
+    def _create_transformed_problem(self, x0):
+        self.scaling = self._create_scaling(x0)
+
+        orig_problem = self.orig_problem
+        params = self.params
+
+        self.transform = Transformation(orig_problem, params, self.scaling)
+        self.problem = self.transform.trans_problem
+
+        pass
+
+    def _check_terminate(self, iterate, iteration, timer):
+        params = self.params
+
+        if (params.iteration_limit is not None) and (
+            iteration >= params.iteration_limit
+        ):
+            logger.debug("Iteration limit reached")
+            return SolverStatus.IterationLimit
+
+        if timer.reached_time_limit():
+            logger.debug("Reached time limit")
+            return SolverStatus.TimeLimit
+
+        if iterate.total_res <= params.opt_tol:
+            logger.debug("Convergence achieved")
+            return SolverStatus.Optimal
+
+        if iterate.locally_infeasible(params.opt_tol, params.local_infeas_tol):
+            logger.debug("Local infeasibility detected")
+            return SolverStatus.LocallyInfeasible
+
+        if (iterate.obj <= params.obj_lower_limit) and (
+            iterate.is_feasible(params.opt_tol)
+        ):
+            logger.debug("Unboundedness detected")
+            return SolverStatus.Unbounded
+
     def solve(
         self, x0: Optional[np.ndarray] = None, y0: Optional[np.ndarray] = None
     ) -> SolverResult:
         """
         Solves the problem starting from the given primal / dual point
 
         Parameters
@@ -360,16 +408,26 @@
 
         Returns
         -------
         pygradflow.solver.SolverResult
             The result of the solving process, including primal and dual
             solutions
         """
-        problem = self.problem
+
+        self._create_transformed_problem(x0)
         params = self.params
+        problem = self.problem
+
+        if params.validate_input:
+            self.evaluator: Evaluator = ValidatingEvaluator(self.problem, params)
+        else:
+            self.evaluator = SimpleEvaluator(self.problem, params)
+
+        self.penalty = penalty_strategy(self.problem, params)
+        self.rho = -1.0
 
         display = problem_display(problem, params)
 
         n = problem.num_vars
         m = problem.num_cons
 
         iterate = self._create_initial_iterate(x0, y0)
@@ -401,33 +459,16 @@
 
         last_active_set = None
         last_display_iteration = -1
 
         timer = Timer(params.time_limit)
 
         while True:
-            if line_diff == header_interval:
-                line_diff = 0
-                logger.info(display.header)
-
-            if iterate.total_res <= params.opt_tol:
-                logger.debug("Convergence achieved")
-                status = SolverStatus.Optimal
-                break
-
-            if iterate.locally_infeasible(params.opt_tol, params.local_infeas_tol):
-                logger.debug("Local infeasibility detected")
-                status = SolverStatus.LocallyInfeasible
-                break
-
-            if (iterate.obj <= params.obj_lower_limit) and (
-                iterate.is_feasible(params.opt_tol)
-            ):
-                logger.debug("Unboundedness detected")
-                status = SolverStatus.Unbounded
+            status = self._check_terminate(iterate, iteration, timer)
+            if status is not None:
                 break
 
             curr_time = time.time()
             display_iterate = curr_time - last_time >= params.display_interval
 
             step_result = self.compute_step(
                 controller, iterate, 1.0 / lamb, display_iterate, timer
@@ -444,19 +485,14 @@
                 raise Exception(
                     f"Inverse step size {lamb} exceeded maximum {params.lamb_max} (incorrect derivatives?)"
                 )
 
             primal_step_norm = np.linalg.norm(next_iterate.x - iterate.x)
             dual_step_norm = np.linalg.norm(next_iterate.y - iterate.y)
 
-            if timer.reached_time_limit():
-                logger.debug("Reached time limit")
-                status = SolverStatus.TimeLimit
-                break
-
             if display_iterate:
                 last_time = curr_time
                 line_diff += 1
 
                 state = dict()
                 state["iterate"] = iterate
 
@@ -502,21 +538,14 @@
                     status = SolverStatus.Optimal
                     break
 
             iteration += 1
             last_active_set = step_result.active_set
             # last_active_set = iterate.active_set
 
-            if (params.iteration_limit is not None) and (
-                iteration >= params.iteration_limit
-            ):
-                status = SolverStatus.IterationLimit
-                logger.debug("Iteration limit reached")
-                break
-
         total_time = timer.elapsed()
 
         direct_dist = iterate.dist(initial_iterate)
 
         assert path_dist >= direct_dist
 
         dist_factor = path_dist / direct_dist if direct_dist != 0.0 else 1.0
```

### Comparing `pygradflow-0.4.6/pygradflow/step/__init__.py` & `pygradflow-0.4.7/pygradflow/step/__init__.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/asymmetric_step_solver.py` & `pygradflow-0.4.7/pygradflow/step/asymmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/box_control.py` & `pygradflow-0.4.7/pygradflow/step/box_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/cond_estimate.py` & `pygradflow-0.4.7/pygradflow/step/cond_estimate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/distance_ratio_control.py` & `pygradflow-0.4.7/pygradflow/step/distance_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/exact_control.py` & `pygradflow-0.4.7/pygradflow/step/exact_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/extended_step_solver.py` & `pygradflow-0.4.7/pygradflow/step/extended_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/fixed_control.py` & `pygradflow-0.4.7/pygradflow/step/fixed_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/linear_solver.py` & `pygradflow-0.4.7/pygradflow/step/linear_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/opti_control.py` & `pygradflow-0.4.7/pygradflow/step/opti_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 from pygradflow.iterate import Iterate
 from pygradflow.step.step_control import (
     StepController,
     StepControlResult,
     StepSolverError,
 )
 
-# Replace w by v = w / sqrt(lambda) in the augmented Lagrangian
-# to avoid numerical issues
-rescaled = True
-
 
 class ImplicitProblem(cyipopt.Problem):
     """
     Solves the primal-dual proximally regularized problem
      .. math::
         \\begin{align}
             \\min_{x \\in \\mathbb{R}^{n}, w \\in \\mathbb{R}^{n}} \\quad
@@ -29,23 +25,28 @@
         \\end{align}
 
     whose optimum coincides with the implicit Euler step of the augmented Lagrangian
     of the original problem. The problem is solved using Ipopt with a limited-memory
     BFGS Hessian approximation.
     """
 
-    def __init__(self, iterate, lamb, rho):
+    def __init__(self, iterate, lamb, rho, rescaled=True):
+        # Resacled:
+        # Replace w by v = w / sqrt(lambda) in the augmented Lagrangian
+        # to avoid numerical issues
         assert lamb >= 0
         assert rho >= 0
 
         self.iterate = iterate
         self.eval = iterate.eval
         self.lamb = lamb
         self.rho = rho
 
+        self.rescaled = rescaled
+
         problem = iterate.problem
         prob_num_vars = problem.num_vars
         prob_num_cons = problem.num_cons
 
         num_vars = prob_num_vars + prob_num_cons
         num_cons = prob_num_cons
 
@@ -81,15 +82,15 @@
         eval = self.eval
         obj = eval.obj(x)
         cons = eval.cons(x)
         aug_obj = obj + (rho / 2) * np.dot(cons, cons)
 
         xdiff = x - self.iterate.x
 
-        if rescaled:
+        if self.rescaled:
             wdiff = w - math.sqrt(lamb) * self.iterate.y
             aug_obj += (lamb / 2) * np.dot(xdiff, xdiff) + (1 / 2) * np.dot(
                 wdiff, wdiff
             )
         else:
             wdiff = w - self.iterate.y
             aug_obj += (lamb / 2) * (np.dot(xdiff, xdiff) + np.dot(wdiff, wdiff))
@@ -110,15 +111,15 @@
         rho = self.rho
         lamb = self.lamb
 
         cons_prod = cons_jac.T.dot(cons)
 
         gradx = obj_grad + rho * cons_prod + lamb * (x - self.iterate.x)
 
-        if rescaled:
+        if self.rescaled:
             gradw = w - math.sqrt(lamb) * self.iterate.y
         else:
             gradw = lamb * (w - self.iterate.y)
         grad = np.concatenate([gradx, gradw])
 
         assert grad.shape == (self.num_vars,)
         assert np.isfinite(grad).all()
@@ -129,15 +130,15 @@
         assert z.shape == (self.num_vars,)
         (x, w) = np.split(z, [self.prob_num_vars])
 
         eval = self.eval
         prob_cons = eval.cons(x)
         lamb = self.lamb
 
-        if rescaled:
+        if self.rescaled:
             cons = prob_cons + math.sqrt(lamb) * w
         else:
             cons = prob_cons + lamb * w
 
         assert cons.shape == (self.num_cons,)
         assert np.isfinite(cons).all()
 
@@ -148,15 +149,15 @@
         (x, w) = np.split(z, [self.prob_num_vars])
 
         eval = self.eval
         problem = self.problem
         jac_x = eval.cons_jac(x).tocoo()
         data_x = jac_x.data
 
-        if rescaled:
+        if self.rescaled:
             data_w = np.full((problem.num_cons,), math.sqrt(self.lamb))
         else:
             data_w = np.full((problem.num_cons,), self.lamb)
 
         assert self._jac_nnz is not None
 
         data = np.concatenate([data_x, data_w])
@@ -203,15 +204,15 @@
         raise NotImplementedError()
 
     def set_options(self, timer):
         import logging
 
         logging.getLogger("cyipopt").setLevel(logging.WARNING)
         self.add_option("print_level", 0)
-        self.add_option("derivative_test", "first-order")
+        # self.add_option("derivative_test", "first-order")
         self.add_option("hessian_approximation", "limited-memory")
 
         remaining = timer.remaining()
 
         if remaining <= 0.0:
             raise StepSolverError("Time limit reached")
         elif np.isfinite(remaining):
```

### Comparing `pygradflow-0.4.6/pygradflow/step/residuum_ratio_control.py` & `pygradflow-0.4.7/pygradflow/step/residuum_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/scaled_step_solver.py` & `pygradflow-0.4.7/pygradflow/step/scaled_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/standard_step_solver.py` & `pygradflow-0.4.7/pygradflow/step/standard_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/step_control.py` & `pygradflow-0.4.7/pygradflow/step/step_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/step_solver.py` & `pygradflow-0.4.7/pygradflow/step/step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/step/symmetric_step_solver.py` & `pygradflow-0.4.7/pygradflow/step/symmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pygradflow/transform.py` & `pygradflow-0.4.7/pygradflow/transform.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.6/pyproject.toml` & `pygradflow-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygradflow"
-version = "0.4.6"
+version = "0.4.7"
 description = "PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs."
 authors = ["Christoph Hansknecht <christoph.hansknecht@tu-clausthal.de>"]
 readme = "README.md"
 repository = "https://github.com/chrhansk/pygradflow"
 documentation = "https://pygradflow.readthedocs.io"
```

### Comparing `pygradflow-0.4.6/PKG-INFO` & `pygradflow-0.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygradflow
-Version: 0.4.6
+Version: 0.4.7
 Summary: PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs.
 Home-page: https://github.com/chrhansk/pygradflow
 Author: Christoph Hansknecht
 Author-email: christoph.hansknecht@tu-clausthal.de
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

