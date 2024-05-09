# Comparing `tmp/scores-0.71.tar.gz` & `tmp/scores-0.72.tar.gz`

## Comparing `scores-0.71.tar` & `scores-0.72.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.71/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.71/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.71/environment.yml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.71/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.71/py.typed
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.71/readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.71/setup.cfg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.71/.binder/postBuild
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.71/.binder/requirements.txt
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scores-0.71/.github/pull_request_template.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scores-0.71/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 scores-0.71/.github/ISSUE_TEMPLATE/new_score.md
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scores-0.71/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.71/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.71/.github/workflows/run-pre-commit.yml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 scores-0.71/src/scores/__init__.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.71/src/scores/functions.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.71/src/scores/sample_data.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.71/src/scores/typing.py
--rw-r--r--   0        0        0    15729 2020-02-02 00:00:00.000000 scores-0.71/src/scores/utils.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.71/src/scores/categorical/__init__.py
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.71/src/scores/categorical/binary_impl.py
--rw-r--r--   0        0        0    14019 2020-02-02 00:00:00.000000 scores-0.71/src/scores/categorical/contingency_impl.py
--rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.71/src/scores/categorical/multicategorical_impl.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.71/src/scores/continuous/__init__.py
--rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.71/src/scores/continuous/flip_flop_impl.py
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.71/src/scores/continuous/murphy_impl.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.71/src/scores/continuous/quantile_loss_impl.py
--rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.71/src/scores/continuous/standard_impl.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.71/src/scores/pandas/__init__.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.71/src/scores/pandas/continuous.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.71/src/scores/pandas/typing.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.71/src/scores/probability/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.71/src/scores/probability/brier_impl.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.71/src/scores/probability/checks.py
--rw-r--r--   0        0        0    37852 2020-02-02 00:00:00.000000 scores-0.71/src/scores/probability/crps_impl.py
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.71/src/scores/probability/roc_impl.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.71/src/scores/processing/__init__.py
--rw-r--r--   0        0        0    12458 2020-02-02 00:00:00.000000 scores-0.71/src/scores/processing/discretise.py
--rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.71/src/scores/processing/isoreg_impl.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.71/src/scores/processing/matching.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.71/src/scores/processing/cdf/__init__.py
--rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.71/src/scores/processing/cdf/cdf_functions.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.71/src/scores/stats/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.71/src/scores/stats/statistical_tests/__init__.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.71/src/scores/stats/statistical_tests/acovf.py
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.71/src/scores/stats/statistical_tests/diebold_mariano_impl.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.71/.gitignore
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.71/LICENSE
--rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 scores-0.71/README.md
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 scores-0.71/pyproject.toml
--rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 scores-0.71/PKG-INFO
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.72/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.72/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.72/environment.yml
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.72/mkdocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.72/py.typed
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.72/readthedocs.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.72/setup.cfg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.72/.binder/postBuild
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.72/.binder/requirements.txt
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scores-0.72/.github/pull_request_template.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scores-0.72/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 scores-0.72/.github/ISSUE_TEMPLATE/new_score.md
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scores-0.72/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.72/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.72/.github/workflows/run-pre-commit.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 scores-0.72/src/scores/__init__.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.72/src/scores/functions.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.72/src/scores/sample_data.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.72/src/scores/typing.py
+-rw-r--r--   0        0        0    15729 2020-02-02 00:00:00.000000 scores-0.72/src/scores/utils.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.72/src/scores/categorical/__init__.py
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.72/src/scores/categorical/binary_impl.py
+-rw-r--r--   0        0        0    14019 2020-02-02 00:00:00.000000 scores-0.72/src/scores/categorical/contingency_impl.py
+-rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.72/src/scores/categorical/multicategorical_impl.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.72/src/scores/continuous/__init__.py
+-rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.72/src/scores/continuous/flip_flop_impl.py
+-rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.72/src/scores/continuous/murphy_impl.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.72/src/scores/continuous/quantile_loss_impl.py
+-rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.72/src/scores/continuous/standard_impl.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.72/src/scores/pandas/__init__.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.72/src/scores/pandas/continuous.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.72/src/scores/pandas/typing.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.72/src/scores/probability/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.72/src/scores/probability/brier_impl.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.72/src/scores/probability/checks.py
+-rw-r--r--   0        0        0    37852 2020-02-02 00:00:00.000000 scores-0.72/src/scores/probability/crps_impl.py
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.72/src/scores/probability/roc_impl.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.72/src/scores/processing/__init__.py
+-rw-r--r--   0        0        0    12458 2020-02-02 00:00:00.000000 scores-0.72/src/scores/processing/discretise.py
+-rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.72/src/scores/processing/isoreg_impl.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.72/src/scores/processing/matching.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.72/src/scores/processing/cdf/__init__.py
+-rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.72/src/scores/processing/cdf/cdf_functions.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.72/src/scores/stats/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.72/src/scores/stats/statistical_tests/__init__.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.72/src/scores/stats/statistical_tests/acovf.py
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.72/src/scores/stats/statistical_tests/diebold_mariano_impl.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.72/.gitignore
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.72/LICENSE
+-rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 scores-0.72/README.md
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 scores-0.72/pyproject.toml
+-rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 scores-0.72/PKG-INFO
```

### Comparing `scores-0.71/.pre-commit-config.yaml` & `scores-0.72/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.71/CODE_OF_CONDUCT.md` & `scores-0.72/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scores-0.71/readthedocs.yaml` & `scores-0.72/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.71/.binder/requirements.txt` & `scores-0.72/.binder/requirements.txt`

 * *Files identical despite different names*

### Comparing `scores-0.71/.github/pull_request_template.md` & `scores-0.72/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `scores-0.71/.github/ISSUE_TEMPLATE/feature_request.md` & `scores-0.72/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scores-0.71/.github/ISSUE_TEMPLATE/new_score.md` & `scores-0.72/.github/ISSUE_TEMPLATE/new_score.md`

 * *Files identical despite different names*

### Comparing `scores-0.71/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md` & `scores-0.72/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `scores-0.71/.github/workflows/python-app.yml` & `scores-0.72/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `scores-0.71/.github/workflows/run-pre-commit.yml` & `scores-0.72/.github/workflows/run-pre-commit.yml`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/__init__.py` & `scores-0.72/src/scores/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import scores.functions
 import scores.pandas
 import scores.probability
 import scores.processing
 import scores.sample_data
 import scores.stats.statistical_tests  # noqa: F401
 
-__version__ = "v0.71"
+__version__ = "v0.72"
 
 __all__ = [
     "scores.categorical",
     "scores.contingency",
     "scores.continuous",
     "scores.functions",
     "scores.pandas",
```

### Comparing `scores-0.71/src/scores/functions.py` & `scores-0.72/src/scores/functions.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/sample_data.py` & `scores-0.72/src/scores/sample_data.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/typing.py` & `scores-0.72/src/scores/typing.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/utils.py` & `scores-0.72/src/scores/utils.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/categorical/__init__.py` & `scores-0.72/src/scores/categorical/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/categorical/binary_impl.py` & `scores-0.72/src/scores/categorical/binary_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/categorical/contingency_impl.py` & `scores-0.72/src/scores/categorical/contingency_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/categorical/multicategorical_impl.py` & `scores-0.72/src/scores/categorical/multicategorical_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/continuous/__init__.py` & `scores-0.72/src/scores/continuous/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/continuous/flip_flop_impl.py` & `scores-0.72/src/scores/continuous/flip_flop_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/continuous/murphy_impl.py` & `scores-0.72/src/scores/continuous/murphy_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/continuous/quantile_loss_impl.py` & `scores-0.72/src/scores/continuous/quantile_loss_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/continuous/standard_impl.py` & `scores-0.72/src/scores/continuous/standard_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/pandas/continuous.py` & `scores-0.72/src/scores/pandas/continuous.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/probability/__init__.py` & `scores-0.72/src/scores/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/probability/brier_impl.py` & `scores-0.72/src/scores/probability/brier_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/probability/checks.py` & `scores-0.72/src/scores/probability/checks.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/probability/crps_impl.py` & `scores-0.72/src/scores/probability/crps_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/probability/roc_impl.py` & `scores-0.72/src/scores/probability/roc_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/processing/__init__.py` & `scores-0.72/src/scores/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/processing/discretise.py` & `scores-0.72/src/scores/processing/discretise.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/processing/isoreg_impl.py` & `scores-0.72/src/scores/processing/isoreg_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/processing/matching.py` & `scores-0.72/src/scores/processing/matching.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/processing/cdf/cdf_functions.py` & `scores-0.72/src/scores/processing/cdf/cdf_functions.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/stats/statistical_tests/acovf.py` & `scores-0.72/src/scores/stats/statistical_tests/acovf.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/src/scores/stats/statistical_tests/diebold_mariano_impl.py` & `scores-0.72/src/scores/stats/statistical_tests/diebold_mariano_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.71/.gitignore` & `scores-0.72/.gitignore`

 * *Files identical despite different names*

### Comparing `scores-0.71/LICENSE` & `scores-0.72/LICENSE`

 * *Files identical despite different names*

### Comparing `scores-0.71/README.md` & `scores-0.72/README.md`

 * *Files identical despite different names*

### Comparing `scores-0.71/pyproject.toml` & `scores-0.72/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scores-0.71/PKG-INFO` & `scores-0.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scores
-Version: 0.71
+Version: 0.72
 Summary: Scores is a package containing mathematical functions for the verification, evaluation and optimisation of model outputs and predictions.
 Project-URL: Homepage, http://www.bom.gov.au
 Author-email: Tennessee Leeuwenburg <tennessee.leeuwenburg@bom.gov.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

