# Comparing `tmp/cvxsimulator-0.9.8.tar.gz` & `tmp/cvxsimulator-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.9.8.tar", max compression
+gzip compressed data, was "cvxsimulator-0.9.9.tar", max compression
```

## Comparing `cvxsimulator-0.9.8.tar` & `cvxsimulator-0.9.9.tar`

### file list

```diff
@@ -1,18 +1,13 @@
--rw-r--r--   0        0        0    10173 2024-01-14 15:12:52.904620 cvxsimulator-0.9.8/LICENSE
--rw-r--r--   0        0        0     4909 2024-01-14 15:12:52.904620 cvxsimulator-0.9.8/README.md
--rw-r--r--   0        0        0      824 2024-01-14 15:12:53.048619 cvxsimulator-0.9.8/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     8308 2024-01-14 15:12:53.048619 cvxsimulator-0.9.8/cvx/simulator/builder.py
--rw-r--r--   0        0        0    13755 2024-01-14 15:12:53.048619 cvxsimulator-0.9.8/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0     3678 2024-01-14 15:12:53.048619 cvxsimulator-0.9.8/cvx/simulator/quantstats/__init__.py
--rw-r--r--   0        0        0     1135 2024-01-14 15:12:53.048619 cvxsimulator-0.9.8/cvx/simulator/quantstats/comments.txt
--rw-r--r--   0        0        0    10751 2024-01-14 15:12:53.052619 cvxsimulator-0.9.8/cvx/simulator/quantstats/reports.py
--rw-r--r--   0        0        0    20368 2024-01-14 15:12:53.052619 cvxsimulator-0.9.8/cvx/simulator/quantstats/stats.py
--rw-r--r--   0        0        0     5133 2024-01-14 15:12:53.052619 cvxsimulator-0.9.8/cvx/simulator/quantstats/utils.py
--rw-r--r--   0        0        0     7195 2024-01-14 15:12:53.052619 cvxsimulator-0.9.8/cvx/simulator/state.py
--rw-r--r--   0        0        0      639 2024-01-14 15:12:53.052619 cvxsimulator-0.9.8/cvx/simulator/utils/__init__.py
--rw-r--r--   0        0        0     2454 2024-01-14 15:12:53.052619 cvxsimulator-0.9.8/cvx/simulator/utils/grid.py
--rw-r--r--   0        0        0      947 2024-01-14 15:12:53.052619 cvxsimulator-0.9.8/cvx/simulator/utils/interpolation.py
--rw-r--r--   0        0        0     2691 2024-01-14 15:12:53.052619 cvxsimulator-0.9.8/cvx/simulator/utils/month.py
--rw-r--r--   0        0        0      969 2024-01-14 15:12:53.052619 cvxsimulator-0.9.8/cvx/simulator/utils/rescale.py
--rw-r--r--   0        0        0      788 2024-01-14 15:13:18.676508 cvxsimulator-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     5547 1970-01-01 00:00:00.000000 cvxsimulator-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-01-14 16:34:08.193494 cvxsimulator-0.9.9/LICENSE
+-rw-r--r--   0        0        0     4909 2024-01-14 16:34:08.193494 cvxsimulator-0.9.9/README.md
+-rw-r--r--   0        0        0      824 2024-01-14 16:34:08.317493 cvxsimulator-0.9.9/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     8308 2024-01-14 16:34:08.317493 cvxsimulator-0.9.9/cvx/simulator/builder.py
+-rw-r--r--   0        0        0    12945 2024-01-14 16:34:08.317493 cvxsimulator-0.9.9/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0     7195 2024-01-14 16:34:08.317493 cvxsimulator-0.9.9/cvx/simulator/state.py
+-rw-r--r--   0        0        0      639 2024-01-14 16:34:08.317493 cvxsimulator-0.9.9/cvx/simulator/utils/__init__.py
+-rw-r--r--   0        0        0     2454 2024-01-14 16:34:08.317493 cvxsimulator-0.9.9/cvx/simulator/utils/grid.py
+-rw-r--r--   0        0        0      947 2024-01-14 16:34:08.317493 cvxsimulator-0.9.9/cvx/simulator/utils/interpolation.py
+-rw-r--r--   0        0        0     2691 2024-01-14 16:34:08.317493 cvxsimulator-0.9.9/cvx/simulator/utils/month.py
+-rw-r--r--   0        0        0      969 2024-01-14 16:34:08.317493 cvxsimulator-0.9.9/cvx/simulator/utils/rescale.py
+-rw-r--r--   0        0        0      924 2024-01-14 16:34:30.729326 cvxsimulator-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     5640 1970-01-01 00:00:00.000000 cvxsimulator-0.9.9/PKG-INFO
```

### Comparing `cvxsimulator-0.9.8/LICENSE` & `cvxsimulator-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.9.8/README.md` & `cvxsimulator-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.9.8/cvx/simulator/__init__.py` & `cvxsimulator-0.9.9/cvx/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.9.8/cvx/simulator/builder.py` & `cvxsimulator-0.9.9/cvx/simulator/builder.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.9.8/cvx/simulator/portfolio.py` & `cvxsimulator-0.9.9/cvx/simulator/portfolio.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,19 +18,16 @@
 from typing import Any
 
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-import cvx.simulator.quantstats as qs
 from cvx.simulator.utils.rescale import returns2prices
 
-qs.extend_pandas()
-
 
 @dataclass(frozen=True)
 class Portfolio:
     prices: pd.DataFrame
     units: pd.DataFrame
     aum: float | pd.Series
 
@@ -241,41 +238,14 @@
         for each asset (as represented in the equity dataframe)
         by the total portfolio value (as represented in the nav dataframe).
         Both dataframes are assumed to have the same dimensions.
         The resulting dataframe will show the relative weight
         of each asset in the portfolio at each point in time."""
         return self.equity.apply(lambda x: x / self.nav)
 
-    def metrics(
-        self,
-        rf: float = 0.0,
-        mode: str = "basic",
-        compound: bool = True,
-        periods_per_year: int = 252,
-        prepare_returns: bool = True,
-        match_dates: bool = True,
-        **kwargs: Any,
-    ) -> pd.DataFrame:
-        """
-        The metrics method calculates the performance metrics of an EquityPortfolio object.
-
-        :param kwargs:
-        :return:
-        """
-        return qs.reports.metrics(
-            returns=self.nav.pct_change().dropna(),
-            rf=rf,
-            mode=mode,
-            compounded=compound,
-            periods_per_year=periods_per_year,
-            prepare_returns=prepare_returns,
-            match_dates=match_dates,
-            **kwargs,
-        )
-
     def snapshot(
         self,
         benchmark: Any = None,
         title: str = "Portfolio Summary",
         log_scale: bool = False,
         label_strategy: str = "Strategy",
         label_benchmark: str = "Benchmark",
```

### Comparing `cvxsimulator-0.9.8/cvx/simulator/state.py` & `cvxsimulator-0.9.9/cvx/simulator/state.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.9.8/cvx/simulator/utils/__init__.py` & `cvxsimulator-0.9.9/cvx/simulator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.9.8/cvx/simulator/utils/grid.py` & `cvxsimulator-0.9.9/cvx/simulator/utils/grid.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.9.8/cvx/simulator/utils/interpolation.py` & `cvxsimulator-0.9.9/cvx/simulator/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.9.8/cvx/simulator/utils/month.py` & `cvxsimulator-0.9.9/cvx/simulator/utils/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.9.8/cvx/simulator/utils/rescale.py` & `cvxsimulator-0.9.9/cvx/simulator/utils/rescale.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.9.8/pyproject.toml` & `cvxsimulator-0.9.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.9.8"
+version = "v0.9.9"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 homepage = "https://www.cvxgrp.org/simulator"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 numpy = "*"
 pandas = "*"
-scipy = ">=1.2.0"
 plotly = "*"
+ipython = { version = "*", optional = true }
+quantstats = { version = "*", optional = true }
+
+[tool.poetry.extras]
+quantstats = ["quantstats", "ipython"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-cov = "*"
 pre-commit = "*"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `cvxsimulator-0.9.8/PKG-INFO` & `cvxsimulator-0.9.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.9.8
+Version: 0.9.9
 Summary: Simple simulator for investors
 Home-page: https://www.cvxgrp.org/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: quantstats
+Requires-Dist: ipython ; extra == "quantstats"
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: plotly
-Requires-Dist: scipy (>=1.2.0)
+Requires-Dist: quantstats ; extra == "quantstats"
 Project-URL: Repository, https://github.com/cvxgrp/simulator
 Description-Content-Type: text/markdown
 
 # [cvxsimulator](https://www.cvxgrp.org/simulator/book)
 
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
```

