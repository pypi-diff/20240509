# Comparing `tmp/dqc_toolkit-0.1.0rc1.tar.gz` & `tmp/dqc_toolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqc_toolkit-0.1.0rc1.tar", last modified: Tue Apr 23 18:03:43 2024, max compression
+gzip compressed data, was "dqc_toolkit-0.1.1.tar", last modified: Thu May  9 15:12:27 2024, max compression
```

## Comparing `dqc_toolkit-0.1.0rc1.tar` & `dqc_toolkit-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 18:03:43.355005 dqc_toolkit-0.1.0rc1/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/LICENSE
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4693 2024-04-23 18:03:43.354399 dqc_toolkit-0.1.0rc1/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1652 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/README.md
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 18:03:43.334724 dqc_toolkit-0.1.0rc1/dqc/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      115 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      585 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/base.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)    15192 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/crossval.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 18:03:43.343010 dqc_toolkit-0.1.0rc1/dqc/utils/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      353 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/utils/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7220 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/utils/_curation.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4894 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/utils/_dataprocessing.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3117 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/utils/_sanitychecks.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      959 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/utils/logging.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1943 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/utils/noise_utils.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      635 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/dqc/version.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 18:03:43.351783 dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4693 2024-04-23 18:03:43.000000 dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      471 2024-04-23 18:03:43.000000 dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-23 18:03:43.000000 dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      335 2024-04-23 18:03:43.000000 dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/requires.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       25 2024-04-23 18:03:43.000000 dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/top_level.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1684 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/pyproject.toml
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-23 18:03:43.355143 dqc_toolkit-0.1.0rc1/setup.cfg
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 18:03:43.350078 dqc_toolkit-0.1.0rc1/tests/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/tests/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/tests/conftest.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     6342 2024-04-23 17:47:16.000000 dqc_toolkit-0.1.0rc1/tests/test_crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-05-09 15:12:27.863687 dqc_toolkit-0.1.1/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-04-23 18:52:52.000000 dqc_toolkit-0.1.1/LICENSE
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     5120 2024-05-09 15:12:27.863083 dqc_toolkit-0.1.1/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2038 2024-04-24 07:04:52.000000 dqc_toolkit-0.1.1/README.md
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-05-09 15:12:27.833966 dqc_toolkit-0.1.1/dqc/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      115 2024-04-23 18:52:52.000000 dqc_toolkit-0.1.1/dqc/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      585 2024-05-09 02:58:48.000000 dqc_toolkit-0.1.1/dqc/base.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)    14923 2024-05-09 14:45:57.000000 dqc_toolkit-0.1.1/dqc/crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-05-09 15:12:27.846983 dqc_toolkit-0.1.1/dqc/utils/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      353 2024-04-23 18:52:52.000000 dqc_toolkit-0.1.1/dqc/utils/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7220 2024-04-23 18:52:52.000000 dqc_toolkit-0.1.1/dqc/utils/_curation.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4894 2024-04-23 18:52:52.000000 dqc_toolkit-0.1.1/dqc/utils/_dataprocessing.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3117 2024-05-09 02:58:48.000000 dqc_toolkit-0.1.1/dqc/utils/_sanitychecks.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      959 2024-04-23 18:52:52.000000 dqc_toolkit-0.1.1/dqc/utils/logging.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1943 2024-04-23 18:52:52.000000 dqc_toolkit-0.1.1/dqc/utils/noise_utils.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      628 2024-05-09 14:50:02.000000 dqc_toolkit-0.1.1/dqc/version.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-05-09 15:12:27.858419 dqc_toolkit-0.1.1/dqc_toolkit.egg-info/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     5120 2024-05-09 15:12:27.000000 dqc_toolkit-0.1.1/dqc_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      471 2024-05-09 15:12:27.000000 dqc_toolkit-0.1.1/dqc_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-05-09 15:12:27.000000 dqc_toolkit-0.1.1/dqc_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      347 2024-05-09 15:12:27.000000 dqc_toolkit-0.1.1/dqc_toolkit.egg-info/requires.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       25 2024-05-09 15:12:27.000000 dqc_toolkit-0.1.1/dqc_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1696 2024-05-09 14:49:07.000000 dqc_toolkit-0.1.1/pyproject.toml
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-05-09 15:12:27.863876 dqc_toolkit-0.1.1/setup.cfg
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-05-09 15:12:27.855934 dqc_toolkit-0.1.1/tests/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-04-23 18:52:52.000000 dqc_toolkit-0.1.1/tests/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-27 08:39:10.000000 dqc_toolkit-0.1.1/tests/conftest.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     6413 2024-05-09 14:45:57.000000 dqc_toolkit-0.1.1/tests/test_crossval.py
```

### Comparing `dqc_toolkit-0.1.0rc1/LICENSE` & `dqc_toolkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0rc1/PKG-INFO` & `dqc_toolkit-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqc-toolkit
-Version: 0.1.0rc1
+Version: 0.1.1
 Summary: Data Quality Check for Machine Learning
 Author-email: Sumanth S Prabhu <sumanthprabhu.104@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sumanthprabhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,25 +49,30 @@
 Requires-Dist: scikit-learn>=1.3.2
 Requires-Dist: ruff>=0.3.4
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Requires-Dist: mkdocs-material==9.5.17; extra == "docs"
 Requires-Dist: mkdocstrings[python]==1.9.2; extra == "docs"
 Requires-Dist: mkdocstrings-crystal==0.3.7; extra == "docs"
+Requires-Dist: mike==2.0.0; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest>=8.1.1; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pytest>=8.1.1; extra == "dev"
 Requires-Dist: mkdocs==1.5.3; extra == "dev"
 Requires-Dist: mkdocs-material==9.5.17; extra == "dev"
 Requires-Dist: mkdocstrings[python]==0.24.3; extra == "dev"
 Requires-Dist: mkdocstrings-crystal==0.3.7; extra == "dev"
 
+![](https://img.shields.io/github/actions/workflow/status/sumanthprabhu/DQC-Toolkit/test.yml) ![](https://img.shields.io/website?url=https%3A%2F%2Fsumanthprabhu.github.io%2FDQC-Toolkit%2F&label=docs
+) ![](https://img.shields.io/pypi/pyversions/DQC-Toolkit) ![](https://img.shields.io/pypi/v/DQC-Toolkit) ![](https://img.shields.io/pypi/l/DQC-toolkit)
+
 ![](/docs/images/dqc-toolkit.svg)
 
+
 DQC Toolkit is a Python library and framework designed with the goal to facilitate improvement of Machine Learning models by identifying and mitigating label errors in training dataset. Currently, DQC toolkit offers `CrossValCurate` for curation of text classification datasets (binary / multi-class) using cross validation based selection.
 
 ## Installation
 
 Installation of DQC-toolkit can be done as shown below
 ```python
 pip install dqc-toolkit
@@ -81,18 +86,18 @@
 ```python linenums="1"
 
 from dqc import CrossValCurate
 
 cvc = CrossValCurate()
 data_curated = cvc.fit_transform(data[['text', 'label']])
 ```
-The result stored in `data_curated` is a pandas dataframe similar to `data` with the following columns -
+The result stored in `data_curated` which is a pandas dataframe similar to `data` with the following columns -
 ```python
 >>> data_curated.columns
 ['text', 'label', 'label_correctness_score', 'is_label_correct', 'predicted_label', 'prediction_probability']
 ```
 
 * `'label_correctness_score'` represents a normalized score quantifying the correctness of `'label'`. 
 * `'is_label_correct'` is a boolean flag indicating whether the given `'label'` is correct (`True`) or incorrect (`False`). 
 * `'predicted_label'` and `'prediction_probability'` represent the curation model's prediction and the corresponding probability score. 
  
-For more details regarding different hyperparameters available in `CrossValCurate`, please refer to the [API documentation](docs/api/crossval).
+For more details regarding different hyperparameters available in `CrossValCurate`, please refer to the [API documentation](https://sumanthprabhu.github.io/DQC-Toolkit/).
```

### Comparing `dqc_toolkit-0.1.0rc1/README.md` & `dqc_toolkit-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+![](https://img.shields.io/github/actions/workflow/status/sumanthprabhu/DQC-Toolkit/test.yml) ![](https://img.shields.io/website?url=https%3A%2F%2Fsumanthprabhu.github.io%2FDQC-Toolkit%2F&label=docs
+) ![](https://img.shields.io/pypi/pyversions/DQC-Toolkit) ![](https://img.shields.io/pypi/v/DQC-Toolkit) ![](https://img.shields.io/pypi/l/DQC-toolkit)
+
 ![](/docs/images/dqc-toolkit.svg)
 
+
 DQC Toolkit is a Python library and framework designed with the goal to facilitate improvement of Machine Learning models by identifying and mitigating label errors in training dataset. Currently, DQC toolkit offers `CrossValCurate` for curation of text classification datasets (binary / multi-class) using cross validation based selection.
 
 ## Installation
 
 Installation of DQC-toolkit can be done as shown below
 ```python
 pip install dqc-toolkit
@@ -17,18 +21,18 @@
 ```python linenums="1"
 
 from dqc import CrossValCurate
 
 cvc = CrossValCurate()
 data_curated = cvc.fit_transform(data[['text', 'label']])
 ```
-The result stored in `data_curated` is a pandas dataframe similar to `data` with the following columns -
+The result stored in `data_curated` which is a pandas dataframe similar to `data` with the following columns -
 ```python
 >>> data_curated.columns
 ['text', 'label', 'label_correctness_score', 'is_label_correct', 'predicted_label', 'prediction_probability']
 ```
 
 * `'label_correctness_score'` represents a normalized score quantifying the correctness of `'label'`. 
 * `'is_label_correct'` is a boolean flag indicating whether the given `'label'` is correct (`True`) or incorrect (`False`). 
 * `'predicted_label'` and `'prediction_probability'` represent the curation model's prediction and the corresponding probability score. 
  
-For more details regarding different hyperparameters available in `CrossValCurate`, please refer to the [API documentation](docs/api/crossval).
+For more details regarding different hyperparameters available in `CrossValCurate`, please refer to the [API documentation](https://sumanthprabhu.github.io/DQC-Toolkit/).
```

### Comparing `dqc_toolkit-0.1.0rc1/dqc/base.py` & `dqc_toolkit-0.1.1/dqc/base.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0rc1/dqc/crossval.py` & `dqc_toolkit-0.1.1/dqc/crossval.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import pandas as pd
 from sentence_transformers import SentenceTransformer
 from sklearn.base import ClassifierMixin
 from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
 from sklearn.linear_model import LogisticRegression
-from sklearn.preprocessing import MinMaxScaler
+from sklearn.preprocessing import normalize
 from tqdm import tqdm
 
 from dqc.base import BaseCurate
 from dqc.utils import (
     Logger,
     SentenceTransformerVectorizer,
     _data_splitter,
@@ -28,15 +28,15 @@
 
 class CrossValCurate(BaseCurate):
     """
     Args:
         curate_feature_extractor (Union[str, TfidfVectorizer, CountVectorizer, SentenceTransformer], optional): Feature extraction method to be used during curation. Accepts string values 'TfidfVectorizer', 'CountVectorizer' which map to `sklearn.feature_extraction.text.TfidfVectorizer` and `sklearn.feature_extraction.text.CountVectorizer` objects respectively. Also accepts explicit instances of `sklearn.feature_extraction.text.TfidfVectorizer` / `sklearn.feature_extraction.text.CountVectorizer`.  Additionally, supports `SentenceTransformer` model object or a string matching the name of a `SentenceTransformer` model hosted on HuggingFace Model Hub. Defaults to 'TfidfVectorizer'.
         curate_model (str, optional): Machine learning model that is trained with `curate_feature_extractor` based features during curation. Accepts any instance of scikit-learn classifier that implement `predict_proba()` method. Defaults to `sklearn.linear_model.LogisticRegression`.
         calibration_method (Union[str, None], optional): Approach to be used for calibration of `curate_model` predictions. Defaults to 'calibrate_using_baseline'.
-        correctness_threshold (float, optional): Minimum prediction probability using `curate_model` to consider the corresponding sample as 'correctly labelled'. Defaults to 0.5.
+        correctness_threshold (float, optional): Minimum prediction probability using `curate_model` to consider the corresponding sample as 'correctly labelled'. Defaults to 0.0.
         n_splits (int, optional): Number of splits to use when running cross-validation based curation.
         verbose (bool, optional): Sets the verbosity level during execution. `True` indicates logging level INFO and `False` indicates logging level 'ERROR'.
 
     Examples:
     Assuming `data` is a pandas dataframe containing samples with noisy labels, here is how you would use `CrossValCurate` -
     ```python
 
@@ -60,15 +60,15 @@
     def __init__(
         self,
         curate_feature_extractor: Union[
             str, TfidfVectorizer, CountVectorizer, SentenceTransformerVectorizer
         ] = "TfidfVectorizer",
         curate_model: Union[str, ClassifierMixin] = LogisticRegression(),
         calibration_method: Union[str, None] = "calibrate_using_baseline",
-        correctness_threshold: float = 0.5,
+        correctness_threshold: float = 0.0,
         n_splits: int = 5,
         verbose: bool = False,
         **options,
     ):
         super().__init__(**options)
 
         self.curate_feature_extractor, self.curate_model, self.calibration_method = (
@@ -117,15 +117,15 @@
 
         Returns:
             bool: `True` if we are confident that the label assigned is correct
                 else `False`
         """
         threshold = self.correctness_threshold
         if (row["predicted_label"] == row[self.y_col_name_int]) and (
-            row["label_correctness_score"] > threshold
+            row["label_correctness_score"] >= threshold
         ):
             return True
         return False
 
     def _set_verbosity(self, verbose: bool):
         """Set logger level based on user input for parameter `verbose`
 
@@ -159,28 +159,26 @@
         label_correctness_scores = [
             pred_prob_matrix[row_index, label_list.index(label)]
             for row_index, label in enumerate(input_labels)
         ]
 
         return preds, pred_probs, label_correctness_scores
 
-    def _get_baselines(self, data_with_noisy_labels: pd.DataFrame) -> pd.DataFrame:
+    def _get_baselines(self, input_data: pd.DataFrame) -> pd.DataFrame:
         """Computes the baseline prediction probabilities using
           input label distribution
 
         Args:
-            data_with_noisy_labels (pd.DataFrame): Input data with
+            input_data (pd.DataFrame): Input data with
                                             corresponding noisy labels
 
         Returns:
             pd.DataFrame: Labels and corresponding probabilities
         """
-        thresholds_df = (
-            data_with_noisy_labels[self.y_col_name_int].value_counts(1)
-        ).reset_index()
+        thresholds_df = (input_data[self.y_col_name_int].value_counts(1)).reset_index()
         thresholds_df.columns = [self.y_col_name_int, "probability"]
         return thresholds_df
 
     def _calibrate_using_baseline(
         self,
         input_labels: List[Union[int, str]],
         pred_prob_matrix: np.ndarray,
@@ -219,20 +217,19 @@
             right_on=self.y_col_name_int,
             how="inner",
         ).reset_index(drop=True)
 
         baseline_probs.drop("label_list", axis=1, inplace=True)
 
         prob_array = baseline_probs["probability"].values
-        pred_prob_matrix = (pred_prob_matrix - prob_array) / prob_array
 
-        if not self.scaler:
-            self.scaler = MinMaxScaler()
+        # Calibrate prediction probabilities using baseline probabilities
+        pred_prob_matrix = (pred_prob_matrix - prob_array) / prob_array
 
-        pred_prob_matrix = self.scaler.fit_transform(pred_prob_matrix)
+        pred_prob_matrix = normalize(pred_prob_matrix, norm="l2")
 
         calibrated_predictions = [
             label_list[index] for index in np.argmax(pred_prob_matrix, axis=1)
         ]
         calibrated_probabilities = np.max(pred_prob_matrix, axis=1).tolist()
         label_correctness_scores = [
             pred_prob_matrix[row_index, label_list.index(label)]
@@ -267,39 +264,38 @@
                 3) 'label_correctness_score' - Label correctness scores based on prediction probabilities \n
                 4) 'is_label_correct' - An indicator variable (True / False) classifying samples as correctly / incorrectly labelled.
         """
         _is_valid(data_with_noisy_labels, X_col_name, y_col_name)
         n_splits = self.n_splits
         options["num_samples"] = len(data_with_noisy_labels)
 
-        # TBD
-        # 'max_features': min(options["num_samples"] // 10, options.get("max_features", 1000))
-
+        # Make a copy of `data_with_noisy_labels` to prevent accidental modification
+        input_data = data_with_noisy_labels.copy()
         logger.info("Pre-processing the data..")
         dp = _DataProcessor(
             random_state=self.random_state,
         )
 
-        data_with_noisy_labels, row_id_col, y_col_name_int = dp._preprocess(
-            data_with_noisy_labels, y_col_name=y_col_name
+        input_data, row_id_col, y_col_name_int = dp._preprocess(
+            input_data, y_col_name=y_col_name
         )
 
         # y_col_name_int needs to be accessed downstream
         self.y_col_name_int = y_col_name_int
 
         data_columns = [X_col_name, y_col_name_int]
         logger.info(
             f"Building the curation pipeline with {n_splits}-fold cross validation.."
         )
         self.curate_pipeline = _get_pipeline(
             self.curate_feature_extractor, self.curate_model, **options
         )
 
         split_indices = _data_splitter(
-            data_with_noisy_labels,
+            input_data,
             X_col_name=X_col_name,
             y_col_name_int=y_col_name_int,
             n_splits=self.n_splits,
         )
 
         # Lists to store predictions
         predictions = []
@@ -307,26 +303,26 @@
         label_correctness_scores = []
 
         # Keep track of shuffled data
         row_ids = []
 
         if self.calibration_method == "calibrate_using_baseline":
             logger.info("Computing baseline predictions for each label..")
-            baseline_probs = self._get_baselines(data_with_noisy_labels[data_columns])
+            baseline_probs = self._get_baselines(input_data[data_columns])
 
         # Iterate through kfold splits
         for train_index, val_index in tqdm(split_indices):
             # Split the data
             X_train, X_val = (
-                data_with_noisy_labels.loc[train_index, X_col_name].values,
-                data_with_noisy_labels.loc[val_index, X_col_name].values,
+                input_data.loc[train_index, X_col_name].values,
+                input_data.loc[val_index, X_col_name].values,
             )
             y_train, y_val = (
-                data_with_noisy_labels.loc[train_index, y_col_name_int].values,
-                data_with_noisy_labels.loc[val_index, y_col_name_int].values,
+                input_data.loc[train_index, y_col_name_int].values,
+                input_data.loc[val_index, y_col_name_int].values,
             )
 
             # Train the model
             self.curate_pipeline.fit(X_train, y_train)
             classes_ = self.curate_pipeline.classes_.tolist()
 
             # Make predictions on the validation set
@@ -343,34 +339,29 @@
                 y_preds, y_pred_probs, label_cscores = self._no_calibration(
                     y_val, y_pred_probs, label_list=classes_
                 )
 
             predictions.extend(y_preds)
             prediction_probabilities.extend(y_pred_probs)
             label_correctness_scores.extend(label_cscores)
-            row_ids.extend(data_with_noisy_labels.loc[val_index, row_id_col].values)
+            row_ids.extend(input_data.loc[val_index, row_id_col].values)
 
         # Order dataframe according to `rowids``
 
         row_id_df = pd.DataFrame()
         row_id_df[row_id_col] = pd.Series(row_ids)
-        data_with_noisy_labels = pd.merge(
-            row_id_df, data_with_noisy_labels, how="left", on=row_id_col
-        )
+        input_data = pd.merge(row_id_df, input_data, how="left", on=row_id_col)
 
         # Add results as columns
-        data_with_noisy_labels["label_correctness_score"] = pd.Series(
-            label_correctness_scores
-        )
-        data_with_noisy_labels["predicted_label"] = pd.Series(predictions)
-        data_with_noisy_labels["prediction_probability"] = pd.Series(
-            prediction_probabilities
-        )
+        input_data["label_correctness_score"] = pd.Series(label_correctness_scores)
+        input_data["predicted_label"] = pd.Series(predictions)
+        input_data["prediction_probability"] = pd.Series(prediction_probabilities)
 
         logger.info("Identifying the correctly labelled samples..")
-        data_with_noisy_labels["is_label_correct"] = (
-            data_with_noisy_labels.progress_apply(self._is_confident, axis=1)
+        input_data["is_label_correct"] = input_data.progress_apply(
+            self._is_confident, axis=1
         )
 
         return dp._postprocess(
-            data_with_noisy_labels, display_cols=data_columns + self.result_col_list
+            input_data,
+            display_cols=list(data_with_noisy_labels.columns) + self.result_col_list,
         )
```

### Comparing `dqc_toolkit-0.1.0rc1/dqc/utils/_curation.py` & `dqc_toolkit-0.1.1/dqc/utils/_curation.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0rc1/dqc/utils/_dataprocessing.py` & `dqc_toolkit-0.1.1/dqc/utils/_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0rc1/dqc/utils/_sanitychecks.py` & `dqc_toolkit-0.1.1/dqc/utils/_sanitychecks.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0rc1/dqc/utils/logging.py` & `dqc_toolkit-0.1.1/dqc/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0rc1/dqc/utils/noise_utils.py` & `dqc_toolkit-0.1.1/dqc/utils/noise_utils.py`

 * *Files identical despite different names*

### Comparing `dqc_toolkit-0.1.0rc1/dqc/version.py` & `dqc_toolkit-0.1.1/dqc/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import platform
 
 import sentence_transformers
 import sklearn
 import transformers
 
-__version__ = "0.1.0-beta5"
-
+__version__ = "0.1.1"
 
 def show_versions():
     """Print useful debugging information
 
     Returns:
         dict: Dictionary object containing system information
     """
```

### Comparing `dqc_toolkit-0.1.0rc1/dqc_toolkit.egg-info/PKG-INFO` & `dqc_toolkit-0.1.1/dqc_toolkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqc-toolkit
-Version: 0.1.0rc1
+Version: 0.1.1
 Summary: Data Quality Check for Machine Learning
 Author-email: Sumanth S Prabhu <sumanthprabhu.104@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sumanthprabhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,25 +49,30 @@
 Requires-Dist: scikit-learn>=1.3.2
 Requires-Dist: ruff>=0.3.4
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Requires-Dist: mkdocs-material==9.5.17; extra == "docs"
 Requires-Dist: mkdocstrings[python]==1.9.2; extra == "docs"
 Requires-Dist: mkdocstrings-crystal==0.3.7; extra == "docs"
+Requires-Dist: mike==2.0.0; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest>=8.1.1; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pytest>=8.1.1; extra == "dev"
 Requires-Dist: mkdocs==1.5.3; extra == "dev"
 Requires-Dist: mkdocs-material==9.5.17; extra == "dev"
 Requires-Dist: mkdocstrings[python]==0.24.3; extra == "dev"
 Requires-Dist: mkdocstrings-crystal==0.3.7; extra == "dev"
 
+![](https://img.shields.io/github/actions/workflow/status/sumanthprabhu/DQC-Toolkit/test.yml) ![](https://img.shields.io/website?url=https%3A%2F%2Fsumanthprabhu.github.io%2FDQC-Toolkit%2F&label=docs
+) ![](https://img.shields.io/pypi/pyversions/DQC-Toolkit) ![](https://img.shields.io/pypi/v/DQC-Toolkit) ![](https://img.shields.io/pypi/l/DQC-toolkit)
+
 ![](/docs/images/dqc-toolkit.svg)
 
+
 DQC Toolkit is a Python library and framework designed with the goal to facilitate improvement of Machine Learning models by identifying and mitigating label errors in training dataset. Currently, DQC toolkit offers `CrossValCurate` for curation of text classification datasets (binary / multi-class) using cross validation based selection.
 
 ## Installation
 
 Installation of DQC-toolkit can be done as shown below
 ```python
 pip install dqc-toolkit
@@ -81,18 +86,18 @@
 ```python linenums="1"
 
 from dqc import CrossValCurate
 
 cvc = CrossValCurate()
 data_curated = cvc.fit_transform(data[['text', 'label']])
 ```
-The result stored in `data_curated` is a pandas dataframe similar to `data` with the following columns -
+The result stored in `data_curated` which is a pandas dataframe similar to `data` with the following columns -
 ```python
 >>> data_curated.columns
 ['text', 'label', 'label_correctness_score', 'is_label_correct', 'predicted_label', 'prediction_probability']
 ```
 
 * `'label_correctness_score'` represents a normalized score quantifying the correctness of `'label'`. 
 * `'is_label_correct'` is a boolean flag indicating whether the given `'label'` is correct (`True`) or incorrect (`False`). 
 * `'predicted_label'` and `'prediction_probability'` represent the curation model's prediction and the corresponding probability score. 
  
-For more details regarding different hyperparameters available in `CrossValCurate`, please refer to the [API documentation](docs/api/crossval).
+For more details regarding different hyperparameters available in `CrossValCurate`, please refer to the [API documentation](https://sumanthprabhu.github.io/DQC-Toolkit/).
```

### Comparing `dqc_toolkit-0.1.0rc1/pyproject.toml` & `dqc_toolkit-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dqc-toolkit"
-version = "0.1.0-rc1"
+version = "0.1.1"
 authors = [
   { name="Sumanth S Prabhu", email="sumanthprabhu.104@gmail.com" },
 ]
 description = "Data Quality Check for Machine Learning"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
@@ -38,15 +38,16 @@
   "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 [project.optional-dependencies]
 docs = [
 	"mkdocs==1.5.3",
 	"mkdocs-material==9.5.17",
 	"mkdocstrings[python]==1.9.2",
-	"mkdocstrings-crystal==0.3.7"
+	"mkdocstrings-crystal==0.3.7",
+	"mike==2.0.0"
 ]
 test = [
     "pytest>=8.1.1"
 ]
 dev = [
   "pytest>=8.1.1",
 	"mkdocs==1.5.3",
```

### Comparing `dqc_toolkit-0.1.0rc1/tests/test_crossval.py` & `dqc_toolkit-0.1.1/tests/test_crossval.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,16 @@
             "prediction_probability",
             "predicted_label",
             "label_correctness_score",
             "is_label_correct",
         ]
     )
 
+    assert len(data_curated.columns) == len(sampled_data.columns) + 4
+
     # Check data types
     assert all(
         data_curated[col].dtype == dtype
         for col, dtype in [
             ("prediction_probability", float),
             ("label_correctness_score", float),
             ("is_label_correct", bool),
```

