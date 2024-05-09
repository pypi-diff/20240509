# Comparing `tmp/mleko-3.2.0.tar.gz` & `tmp/mleko-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-3.2.0.tar", max compression
+gzip compressed data, was "mleko-4.0.0.tar", max compression
```

## Comparing `mleko-3.2.0.tar` & `mleko-4.0.0.tar`

### file list

```diff
@@ -1,78 +1,86 @@
--rw-r--r--   0        0        0    10947 2024-04-18 20:13:05.988194 mleko-3.2.0/LICENSE
--rw-r--r--   0        0        0     4728 2024-04-18 20:13:05.988194 mleko-3.2.0/README.md
--rw-r--r--   0        0        0     1976 2024-04-18 20:13:37.224223 mleko-3.2.0/mleko/__init__.py
--rw-r--r--   0        0        0      585 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/__init__.py
--rw-r--r--   0        0        0    16986 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/cache_mixin.py
--rw-r--r--   0        0        0     1563 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/base_fingerprinter.py
--rw-r--r--   0        0        0     1012 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py
--rw-r--r--   0        0        0     2989 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/csv_fingerprinter.py
--rw-r--r--   0        0        0     1222 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/dict_fingerprinter.py
--rw-r--r--   0        0        0     5578 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py
--rw-r--r--   0        0        0    14262 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py
--rw-r--r--   0        0        0     1219 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
--rw-r--r--   0        0        0     1360 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/handlers/__init__.py
--rw-r--r--   0        0        0      650 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/handlers/base_cache_handler.py
--rw-r--r--   0        0        0     1102 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/handlers/joblib_cache_handler.py
--rw-r--r--   0        0        0     1196 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/handlers/pickle_cache_handler.py
--rw-r--r--   0        0        0     1508 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/handlers/vaex_cache_handler.py
--rw-r--r--   0        0        0     8312 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/lru_cache_mixin.py
--rw-r--r--   0        0        0      805 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/__init__.py
--rw-r--r--   0        0        0      492 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/convert/__init__.py
--rw-r--r--   0        0        0     1613 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/convert/base_converter.py
--rw-r--r--   0        0        0    15173 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/convert/csv_to_vaex_converter.py
--rw-r--r--   0        0        0     6611 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/data_schema.py
--rw-r--r--   0        0        0     1614 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/__init__.py
--rw-r--r--   0        0        0    11612 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/base_feature_selector.py
--rw-r--r--   0        0        0     7661 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/composite_feature_selector.py
--rw-r--r--   0        0        0     5156 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/invariance_feature_selector.py
--rw-r--r--   0        0        0     5439 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
--rw-r--r--   0        0        0     7257 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
--rw-r--r--   0        0        0     5803 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/variance_feature_selector.py
--rw-r--r--   0        0        0      569 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/filter/__init__.py
--rw-r--r--   0        0        0     1615 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/filter/base_filter.py
--rw-r--r--   0        0        0     3927 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/filter/expression_filter.py
--rw-r--r--   0        0        0     7236 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/filter/imblearn_resampling_filter.py
--rw-r--r--   0        0        0     1197 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/ingest/__init__.py
--rw-r--r--   0        0        0     6188 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/ingest/base_ingester.py
--rw-r--r--   0        0        0    20008 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/ingest/kaggle_ingester.py
--rw-r--r--   0        0        0    12998 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/ingest/s3_ingester.py
--rw-r--r--   0        0        0      680 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/split/__init__.py
--rw-r--r--   0        0        0     1501 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/split/base_splitter.py
--rw-r--r--   0        0        0     4254 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/split/expression_splitter.py
--rw-r--r--   0        0        0     6732 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/split/random_splitter.py
--rw-r--r--   0        0        0     1612 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/__init__.py
--rw-r--r--   0        0        0     9362 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/base_transformer.py
--rw-r--r--   0        0        0     6882 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/composite_transformer.py
--rw-r--r--   0        0        0     4743 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/frequency_encoder_transformer.py
--rw-r--r--   0        0        0    11533 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/label_encoder_transformer.py
--rw-r--r--   0        0        0     3744 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/max_abs_scaler_transformer.py
--rw-r--r--   0        0        0     4150 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/min_max_scaler_transformer.py
--rw-r--r--   0        0        0      388 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/model/__init__.py
--rw-r--r--   0        0        0    18964 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/model/base_model.py
--rw-r--r--   0        0        0    10756 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/model/lgbm_model.py
--rw-r--r--   0        0        0      413 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/model/tune/__init__.py
--rw-r--r--   0        0        0     3767 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/model/tune/base_tuner.py
--rw-r--r--   0        0        0    16740 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/model/tune/optuna_tuner.py
--rw-r--r--   0        0        0      645 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1382 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4497 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     9723 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      874 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     3832 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/convert_step.py
--rw-r--r--   0        0        0     6151 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/feature_select_step.py
--rw-r--r--   0        0        0     2994 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/filter_step.py
--rw-r--r--   0        0        0     2780 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/ingest_step.py
--rw-r--r--   0        0        0     7816 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/model_step.py
--rw-r--r--   0        0        0     2903 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/split_step.py
--rw-r--r--   0        0        0     5744 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/transform_step.py
--rw-r--r--   0        0        0     3430 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/tune_step.py
--rw-r--r--   0        0        0        0 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/py.typed
--rw-r--r--   0        0        0      766 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/utils/__init__.py
--rw-r--r--   0        0        0     9753 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     3431 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/utils/decorators.py
--rw-r--r--   0        0        0      743 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1414 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/utils/tqdm_helpers.py
--rw-r--r--   0        0        0     3641 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/utils/vaex_helpers.py
--rw-r--r--   0        0        0     2608 2024-04-18 20:13:37.224223 mleko-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 mleko-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10947 2024-05-09 10:07:38.962391 mleko-4.0.0/LICENSE
+-rw-r--r--   0        0        0     5019 2024-05-09 10:07:38.962391 mleko-4.0.0/README.md
+-rw-r--r--   0        0        0     1976 2024-05-09 10:08:07.210592 mleko-4.0.0/mleko/__init__.py
+-rw-r--r--   0        0        0      585 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    16986 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0     1560 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1168 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     1012 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py
+-rw-r--r--   0        0        0     2989 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1248 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/json_fingerprinter.py
+-rw-r--r--   0        0        0     5578 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py
+-rw-r--r--   0        0        0    14262 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py
+-rw-r--r--   0        0        0     1219 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0     1832 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/__init__.py
+-rw-r--r--   0        0        0      650 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/base_cache_handler.py
+-rw-r--r--   0        0        0     1102 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/joblib_cache_handler.py
+-rw-r--r--   0        0        0     1251 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/json_cache_handler.py
+-rw-r--r--   0        0        0     1196 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/pickle_cache_handler.py
+-rw-r--r--   0        0        0     1207 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/string_cache_handler.py
+-rw-r--r--   0        0        0     1954 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/vaex_cache_handler.py
+-rw-r--r--   0        0        0     8312 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      805 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      492 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1613 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    15248 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     6592 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/data_schema.py
+-rw-r--r--   0        0        0      774 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/export/__init__.py
+-rw-r--r--   0        0        0      900 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/export/base_exporter.py
+-rw-r--r--   0        0        0     8725 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/export/local_exporter.py
+-rw-r--r--   0        0        0     8191 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/export/s3_exporter.py
+-rw-r--r--   0        0        0     1614 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0    11612 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     7661 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     5156 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5439 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     7257 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5803 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      569 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/filter/__init__.py
+-rw-r--r--   0        0        0     1615 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/filter/base_filter.py
+-rw-r--r--   0        0        0     3927 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/filter/expression_filter.py
+-rw-r--r--   0        0        0     7160 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/filter/imblearn_resampling_filter.py
+-rw-r--r--   0        0        0      878 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     2747 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    20020 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0    11181 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      680 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1501 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     4254 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     6732 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0     1612 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/__init__.py
+-rw-r--r--   0        0        0     9362 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/base_transformer.py
+-rw-r--r--   0        0        0     6882 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/composite_transformer.py
+-rw-r--r--   0        0        0     4743 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/frequency_encoder_transformer.py
+-rw-r--r--   0        0        0    11533 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/label_encoder_transformer.py
+-rw-r--r--   0        0        0     3744 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/max_abs_scaler_transformer.py
+-rw-r--r--   0        0        0     4150 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/min_max_scaler_transformer.py
+-rw-r--r--   0        0        0      388 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/model/__init__.py
+-rw-r--r--   0        0        0    18964 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/model/base_model.py
+-rw-r--r--   0        0        0    10756 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/model/lgbm_model.py
+-rw-r--r--   0        0        0      413 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/model/tune/__init__.py
+-rw-r--r--   0        0        0     3785 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/model/tune/base_tuner.py
+-rw-r--r--   0        0        0    16390 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/model/tune/optuna_tuner.py
+-rw-r--r--   0        0        0      645 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1382 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4658 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     9807 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      928 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     3931 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     3312 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/export_step.py
+-rw-r--r--   0        0        0     6310 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     3115 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/filter_step.py
+-rw-r--r--   0        0        0     2858 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     8139 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/model_step.py
+-rw-r--r--   0        0        0     3002 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0     5933 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/transform_step.py
+-rw-r--r--   0        0        0     3551 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/tune_step.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/py.typed
+-rw-r--r--   0        0        0      977 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     9753 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3431 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/decorators.py
+-rw-r--r--   0        0        0     4724 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0    11820 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/s3_helpers.py
+-rw-r--r--   0        0        0     1414 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     3641 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2608 2024-05-09 10:08:07.210592 mleko-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6323 1970-01-01 00:00:00.000000 mleko-4.0.0/PKG-INFO
```

### Comparing `mleko-3.2.0/LICENSE` & `mleko-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/README.md` & `mleko-4.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 ## Features
 
 `mleko` is engineered to address the end-to-end needs of machine learning pipelines, providing robust, scalable solutions for data science challenges:
 
 - Ingest: Seamlessly integrates with data sources like AWS S3 and Kaggle, offering hassle-free data ingestion and compatibility.
+- Export: Supports exporting data to various formats and platforms, locally or in the cloud, to ensure that your data is accessible and shareable.
 - Convert: Specializes in data format transformations, prominently featuring high-performance conversions from `CSV` to `Vaex DataFrame`, to make your data pipeline-ready.
 - Split: Employs sophisticated data partitioning algorithms, allowing you to segment DataFrames into train, test, and validation sets for effective model training and evaluation.
+  -Filter: Provides a suite of filtering techniques such as resampling or simple expression-based filtering, enabling you to focus on the most relevant data.
 - Feature Selection: Equipped with a suite of feature selection techniques, `mleko` enables model performance by focusing on the most impactful variables.
 - Transformation: Facilitates data manipulations such as Frequency Encoding and Standardization, ensuring that your data conforms to the prerequisites of the machine learning algorithms.
 - Model: Provides a core set of functionalities for machine learning models, including in-built support for hyperparameter tuning, thereby streamlining the path from data to deployable model.
 - Pipeline: Unifies the entire workflow into an intuitive directed acyclic graph (`DAG`) architecture, promoting reproducibility and reducing iteration time and time-to-market for machine learning models.
 
 By integrating these features, `mleko` serves as a comprehensive toolkit for machine learning practitioners looking to build robust models efficiently.
 
@@ -52,15 +54,15 @@
 
 ## Release History
 
 See our [changelog](https://github.com/klarna-incubator/mleko/tree/main/CHANGELOG.md).
 
 ## Acknowledgements
 
-The development of `mleko` was significantly influenced by existing work of the following individuals:
+The development of `mleko` was influenced by existing work of the following individuals:
 
 - **Felipe Breve Siola** ([fsiola](https://github.com/fsiola))
 - **Sai Ma** ([metanouvelle](https://github.com/metanouvelle))
 - **Ahmet Anil Pala** ([aanilpala](https://github.com/aanilpala))
 
 Their insights and contributions provided a solid foundation for this library. We appreciate their effort and recognize their contributions that led to the creation of `mleko`.
```

### Comparing `mleko-3.2.0/mleko/__init__.py` & `mleko-4.0.0/mleko/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 By integrating these features, `mleko` serves as a comprehensive toolkit for machine learning
 practitioners looking to build robust models efficiently.
 """
 
 from __future__ import annotations
 
 
-__version__ = "3.2.0"
+__version__ = "4.0.0"
```

### Comparing `mleko-3.2.0/mleko/cache/__init__.py` & `mleko-4.0.0/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/cache/cache_mixin.py` & `mleko-4.0.0/mleko/cache/cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/cache/fingerprinters/__init__.py` & `mleko-4.0.0/mleko/cache/fingerprinters/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 such as Vaex DataFrames or CSV files. These fingerprints can be used to track changes in data and support
 caching mechanisms.
 
 The following fingerprinting utilities are provided:
     - `BaseFingerprinter`: The base class for all fingerprinters.
     - `CSVFingerprinter`: A fingerprinter for CSV files.
     - `VaexFingerprinter`: A fingerprinter for Vaex DataFrames.
-    - `DictFingerprinter`: A fingerprinter for dictionaries.
+    - `JsonFingerprinter`: A fingerprinter for JSON data.
     - `CallableSourceFingerprinter`: A fingerprinter for Python Callables that hashes the source code of the Callable
         to generate a fingerprint.
     - `OptunaSamplerFingerprinter`: A fingerprinter for Optuna samplers.
     - `OptunaPrunerFingerprinter`: A fingerprinter for Optuna pruners.
 """
 
 from __future__ import annotations
 
 from .base_fingerprinter import BaseFingerprinter
 from .callable_source_fingerprinter import CallableSourceFingerprinter
 from .csv_fingerprinter import CSVFingerprinter
-from .dict_fingerprinter import DictFingerprinter
+from .json_fingerprinter import JsonFingerprinter
 from .optuna_pruner_fingerprinter import OptunaPrunerFingerprinter
 from .optuna_sampler_fingerprinter import OptunaSamplerFingerprinter
 from .vaex_fingerprinter import VaexFingerprinter
 
 
 __all__ = [
     "BaseFingerprinter",
     "CallableSourceFingerprinter",
     "CSVFingerprinter",
     "VaexFingerprinter",
     "OptunaPrunerFingerprinter",
     "OptunaSamplerFingerprinter",
-    "DictFingerprinter",
+    "JsonFingerprinter",
 ]
```

### Comparing `mleko-3.2.0/mleko/cache/fingerprinters/base_fingerprinter.py` & `mleko-4.0.0/mleko/cache/fingerprinters/base_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py` & `mleko-4.0.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/cache/fingerprinters/csv_fingerprinter.py` & `mleko-4.0.0/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/cache/fingerprinters/dict_fingerprinter.py` & `mleko-4.0.0/mleko/cache/fingerprinters/json_fingerprinter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-"""The module contains a fingerprinter for dictionaries."""
+"""The module contains a fingerprinter for JSON data."""
 
 from __future__ import annotations
 
 import hashlib
 import json
 from typing import Any
 
 from .base_fingerprinter import BaseFingerprinter
 
 
-class DictFingerprinter(BaseFingerprinter):
-    """Class to generate unique fingerprints for dictionaries."""
+class JsonFingerprinter(BaseFingerprinter):
+    """Class to generate unique fingerprints for valid JSON data."""
 
-    def fingerprint(self, data: dict[str, Any] | None) -> str:
-        """Generate a fingerprint string for a given dictionary.
+    def fingerprint(self, data: dict[str, Any] | list[Any] | None) -> str:
+        """Generate a fingerprint string for a given JSON.
 
         Args:
-            data: The dictionary to dump.
+            data: The JSON data to generate a fingerprint for.
 
         Returns:
-            A fingerprint that uniquely identifies the dictionary.
+            A fingerprint that uniquely identifies the JSON data.
         """
 
         def deep_sort(obj: dict | Any):
             """Recursively sort nested dicts.
 
             Args:
                 obj: The dict or object to sort.
```

### Comparing `mleko-3.2.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py` & `mleko-4.0.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py` & `mleko-4.0.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/cache/fingerprinters/vaex_fingerprinter.py` & `mleko-4.0.0/mleko/cache/fingerprinters/vaex_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/cache/handlers/__init__.py` & `mleko-4.0.0/mleko/cache/handlers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,27 +5,37 @@
     - `reader`: A function that takes a Path object as input and returns the deserialized data stored in the cache file.
     - `suffix`: The suffix of the cache files.
 
 The following cache handlers are provided by the subpackage:
     - `JOBLIB_CACHE_HANDLER`: A cache handler for Python objects using joblib
     - `PICKLE_CACHE_HANDLER`: A cache handler for pickling Python objects.
     - `VAEX_DATAFRAME_CACHE_HANDLER`: A cache handler for `vaex` DataFrames.
+    - `JSON_CACHE_HANDLER`: A cache handler for serializing and deserializing data using JSON.
+    - `STRING_CACHE_HANDLER`: A cache handler for serializing and deserializing string data.
 """
 
 from .base_cache_handler import CacheHandler
 from .joblib_cache_handler import JOBLIB_CACHE_HANDLER, read_joblib, write_joblib
+from .json_cache_handler import JSON_CACHE_HANDLER, read_json, write_json
 from .pickle_cache_handler import PICKLE_CACHE_HANDLER, read_pickle, write_pickle
+from .string_cache_handler import STRING_CACHE_HANDLER, read_string, write_string
 from .vaex_cache_handler import VAEX_DATAFRAME_CACHE_HANDLER, read_vaex_dataframe, write_vaex_dataframe
 
 
 __all__ = [
     "CacheHandler",
     "JOBLIB_CACHE_HANDLER",
     "PICKLE_CACHE_HANDLER",
     "VAEX_DATAFRAME_CACHE_HANDLER",
+    "JSON_CACHE_HANDLER",
+    "STRING_CACHE_HANDLER",
     "read_joblib",
     "write_joblib",
     "read_pickle",
     "write_pickle",
     "read_vaex_dataframe",
     "write_vaex_dataframe",
+    "read_json",
+    "write_json",
+    "read_string",
+    "write_string",
 ]
```

### Comparing `mleko-3.2.0/mleko/cache/handlers/base_cache_handler.py` & `mleko-4.0.0/mleko/cache/handlers/base_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/cache/handlers/joblib_cache_handler.py` & `mleko-4.0.0/mleko/cache/handlers/joblib_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/cache/handlers/pickle_cache_handler.py` & `mleko-4.0.0/mleko/cache/handlers/pickle_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/cache/handlers/vaex_cache_handler.py` & `mleko-4.0.0/mleko/cache/handlers/vaex_cache_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,19 +29,32 @@
     Args:
         cache_file_path: The path of the cache file to be written.
         output: The Vaex DataFrame to be saved in the cache file.
     """
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", "invalid value encountered in cast")
         with tqdm(total=100, desc=f"Writing DataFrame to {cache_file_path.suffix} file") as pbar:
-            output.export_arrow(
-                cache_file_path,
-                progress=set_tqdm_percent_wrapper(pbar),
-                parallel=True,
-                chunk_size=262_144,
-            )
+            progress_bar = set_tqdm_percent_wrapper(pbar)
+            parallel = True
+            chunk_size = 262_144
+
+            if cache_file_path.suffix == ".csv":
+                output.export_csv(
+                    cache_file_path,
+                    progress=progress_bar,
+                    parallel=parallel,
+                    chunk_size=chunk_size,
+                    backend="arrow",
+                )
+            else:
+                output.export(
+                    cache_file_path,
+                    progress=progress_bar,
+                    parallel=parallel,
+                    chunk_size=chunk_size,
+                )
 
 
 VAEX_DATAFRAME_CACHE_HANDLER = CacheHandler(
     writer=write_vaex_dataframe, reader=read_vaex_dataframe, suffix="arrow", can_handle_none=False
 )
 """A CacheHandler for `vaex` DataFrames."""
```

### Comparing `mleko-3.2.0/mleko/cache/lru_cache_mixin.py` & `mleko-4.0.0/mleko/cache/lru_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/__init__.py` & `mleko-4.0.0/mleko/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/convert/base_converter.py` & `mleko-4.0.0/mleko/dataset/convert/base_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/convert/csv_to_vaex_converter.py` & `mleko-4.0.0/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,14 +281,15 @@
             dtypes[col] = "string"
         for col in forced_boolean_columns:
             dtypes[col] = "boolean"
 
         df_chunk = vaex.from_csv_arrow(
             file_path,
             read_options=arrow_csv.ReadOptions(use_threads=True),
+            parse_options=arrow_csv.ParseOptions(newlines_in_values=True),
             convert_options=arrow_csv.ConvertOptions(
                 column_types=dtypes,
                 null_values=na_values,
                 true_values=true_values,
                 false_values=false_values,
                 strings_can_be_null=True,
                 quoted_strings_can_be_null=True,
```

### Comparing `mleko-3.2.0/mleko/dataset/data_schema.py` & `mleko-4.0.0/mleko/dataset/data_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module for DataSchema class, used for storing type information about the dataset."""
 
 from __future__ import annotations
 
 import copy
 from typing import Literal
 
-from mleko.cache.fingerprinters.dict_fingerprinter import DictFingerprinter
+from mleko.cache.fingerprinters import JsonFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 
 
 logger = CustomLogger()
 """The logger for the module."""
 
 DataType = Literal["numerical", "categorical", "boolean", "datetime", "timedelta"]
@@ -59,30 +59,30 @@
 
         Args:
             other: Object to compare with.
 
         Returns:
             True if the two DataSchema objects are equal, False otherwise.
         """
-        return isinstance(other, DataSchema) and DictFingerprinter().fingerprint(
+        return isinstance(other, DataSchema) and JsonFingerprinter().fingerprint(
             self.to_dict()
-        ) == DictFingerprinter().fingerprint(other.to_dict())
+        ) == JsonFingerprinter().fingerprint(other.to_dict())
 
     def __hash__(self) -> int:
         """Get the hash of the DataSchema.
 
         Warning:
             This method is not intended to be used for stable hashing across runs. Please
-            refer to the `DictFingerprinter` class in the `mleko.utils.fingerprinter` module
+            refer to the `JsonFingerprinter` class in the `mleko.utils.fingerprinter` module
             for stable hashing of the DataSchema.
 
         Returns:
             Hash of the DataSchema.
         """
-        return hash(DictFingerprinter().fingerprint(self.to_dict()))
+        return hash(JsonFingerprinter().fingerprint(self.to_dict()))
 
     def __repr__(self) -> str:
         """Get the string representation of DataSchema.
 
         Returns:
             String representation of DataSchema.
         """
```

### Comparing `mleko-3.2.0/mleko/dataset/feature_select/__init__.py` & `mleko-4.0.0/mleko/dataset/feature_select/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/feature_select/base_feature_selector.py` & `mleko-4.0.0/mleko/dataset/feature_select/base_feature_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Hashable
 
 import vaex
 
-from mleko.cache.fingerprinters import DictFingerprinter, VaexFingerprinter
+from mleko.cache.fingerprinters import JsonFingerprinter, VaexFingerprinter
 from mleko.cache.handlers import JOBLIB_CACHE_HANDLER, VAEX_DATAFRAME_CACHE_HANDLER
 from mleko.cache.lru_cache_mixin import LRUCacheMixin
 from mleko.dataset.data_schema import DataSchema
 from mleko.utils.custom_logger import CustomLogger
 
 
 logger = CustomLogger()
@@ -88,15 +88,15 @@
         Returns:
             Updated DataSchema and fitted feature selector.
         """
         ds, feature_selector = self._cached_execute(
             lambda_func=lambda: self._fit(data_schema, dataframe),
             cache_key_inputs=[
                 self._fingerprint(),
-                (data_schema.to_dict(), DictFingerprinter()),
+                (data_schema.to_dict(), JsonFingerprinter()),
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=JOBLIB_CACHE_HANDLER,
             disable_cache=disable_cache,
         )
@@ -131,15 +131,15 @@
             logger.error(msg)
             raise RuntimeError(msg)
 
         ds, df = self._cached_execute(
             lambda_func=lambda: self._transform(data_schema, dataframe),
             cache_key_inputs=[
                 self._fingerprint(),
-                (data_schema.to_dict(), DictFingerprinter()),
+                (data_schema.to_dict(), JsonFingerprinter()),
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=[JOBLIB_CACHE_HANDLER, VAEX_DATAFRAME_CACHE_HANDLER],
             disable_cache=disable_cache,
         )
@@ -166,15 +166,15 @@
         Returns:
             Tuple of updated DataSchema, fitted feature selector, and transformed DataFrame.
         """
         ds, feature_selector, df = self._cached_execute(
             lambda_func=lambda: self._fit_transform(data_schema, dataframe),
             cache_key_inputs=[
                 self._fingerprint(),
-                (data_schema.to_dict(), DictFingerprinter()),
+                (data_schema.to_dict(), JsonFingerprinter()),
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=[JOBLIB_CACHE_HANDLER, JOBLIB_CACHE_HANDLER, VAEX_DATAFRAME_CACHE_HANDLER],
             disable_cache=disable_cache,
         )
```

### Comparing `mleko-3.2.0/mleko/dataset/feature_select/composite_feature_selector.py` & `mleko-4.0.0/mleko/dataset/feature_select/composite_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/feature_select/invariance_feature_selector.py` & `mleko-4.0.0/mleko/dataset/feature_select/invariance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/feature_select/missing_rate_feature_selector.py` & `mleko-4.0.0/mleko/dataset/feature_select/missing_rate_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py` & `mleko-4.0.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/feature_select/variance_feature_selector.py` & `mleko-4.0.0/mleko/dataset/feature_select/variance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/filter/__init__.py` & `mleko-4.0.0/mleko/dataset/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/filter/base_filter.py` & `mleko-4.0.0/mleko/dataset/filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/filter/expression_filter.py` & `mleko-4.0.0/mleko/dataset/filter/expression_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from pathlib import Path
 
 import vaex
 
-from mleko.cache.fingerprinters import DictFingerprinter, VaexFingerprinter
+from mleko.cache.fingerprinters import JsonFingerprinter, VaexFingerprinter
 from mleko.cache.handlers.vaex_cache_handler import VAEX_DATAFRAME_CACHE_HANDLER
 from mleko.dataset.data_schema import DataSchema
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 
 from .base_filter import BaseFilter
 
@@ -77,15 +77,15 @@
         Returns:
             The filtered dataframe.
         """
         return self._cached_execute(
             lambda_func=lambda: self._filter(data_schema, dataframe),
             cache_key_inputs=[
                 self._expression,
-                (data_schema.to_dict(), DictFingerprinter()),
+                (data_schema.to_dict(), JsonFingerprinter()),
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=VAEX_DATAFRAME_CACHE_HANDLER,
             disable_cache=disable_cache,
         )
```

### Comparing `mleko-3.2.0/mleko/dataset/filter/imblearn_resampling_filter.py` & `mleko-4.0.0/mleko/dataset/filter/imblearn_resampling_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from pathlib import Path
 
 import numpy as np
 import pyarrow as pa
 import vaex
 from imblearn.under_sampling.base import BaseSampler
 
-from mleko.cache.fingerprinters.dict_fingerprinter import DictFingerprinter
-from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
+from mleko.cache.fingerprinters import JsonFingerprinter, VaexFingerprinter
 from mleko.cache.handlers.vaex_cache_handler import VAEX_DATAFRAME_CACHE_HANDLER
 from mleko.dataset.data_schema import DataSchema
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.vaex_helpers import get_column, get_columns, get_indices
 
 from .base_filter import BaseFilter
@@ -93,17 +92,17 @@
         Returns:
             The filtered DataFrame.
         """
         return self._cached_execute(
             lambda_func=lambda: self._filter(data_schema, dataframe),
             cache_key_inputs=[
                 self._sampler.__class__.__qualname__,
-                (self._sampler.get_params(deep=True), DictFingerprinter()),
+                (self._sampler.get_params(deep=True), JsonFingerprinter()),
                 self._target_column,
-                (data_schema.to_dict(), DictFingerprinter()),
+                (data_schema.to_dict(), JsonFingerprinter()),
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=VAEX_DATAFRAME_CACHE_HANDLER,
             disable_cache=disable_cache,
         )
```

### Comparing `mleko-3.2.0/mleko/dataset/ingest/__init__.py` & `mleko-4.0.0/mleko/dataset/ingest/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,22 +2,19 @@
 
 This subpackage contains classes designed to easily fetch data from different sources, like AWS S3 or Kaggle,
 and store them locally in specified destination directories. The main classes are 'BaseIngester', an abstract base
 class for implementing specific data source classes, along with concrete implementations.
 
 The following ingester classes are provided by the subpackage:
     - `BaseIngester`: The abstract base class for all ingesters.
-        - `LocalFileEntry`: A class representing a local file entry.
-        - `LocalManifest`: A class representing a local manifest.
-        - `LocalManifestHandler`: A class for handling local manifests.
     - `S3Ingester`: An ingester for fetching data from AWS S3.
     - `KaggleIngester`: An ingester for fetching data from Kaggle.
 """
 
 from __future__ import annotations
 
-from .base_ingester import BaseIngester, LocalFileEntry, LocalManifest, LocalManifestHandler
+from .base_ingester import BaseIngester
 from .kaggle_ingester import KaggleIngester
 from .s3_ingester import S3Ingester
 
 
-__all__ = ["BaseIngester", "S3Ingester", "KaggleIngester", "LocalFileEntry", "LocalManifest", "LocalManifestHandler"]
+__all__ = ["BaseIngester", "S3Ingester", "KaggleIngester"]
```

### Comparing `mleko-3.2.0/mleko/dataset/ingest/kaggle_ingester.py` & `mleko-4.0.0/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,17 @@
 from pathlib import Path
 from typing import NamedTuple
 
 import requests
 from requests.auth import HTTPBasicAuth
 from tqdm.auto import tqdm
 
-from mleko.utils.custom_logger import CustomLogger
-from mleko.utils.decorators import auto_repr
+from mleko.utils import CustomLogger, LocalFileEntry, LocalManifestHandler, auto_repr
 
-from .base_ingester import BaseIngester, LocalFileEntry, LocalManifestHandler
+from .base_ingester import BaseIngester
 
 
 logger = CustomLogger()
 """A module-level custom logger."""
 
 
 class KaggleCredentials(NamedTuple):
@@ -189,15 +188,15 @@
     @auto_repr
     def __init__(
         self,
         owner_slug: str,
         dataset_slug: str,
         file_pattern: str | list[str] = "*",
         dataset_id: str | None = None,
-        cache_directory: str | Path = "data/kaggle-ingester",
+        destination_directory: str | Path = "data/kaggle-ingester",
         dataset_version: str | int | None = None,
         kaggle_api_credentials_file: str | Path | None = None,
         num_workers: int = 64,
     ) -> None:
         """Initializes a `KaggleIngester` instance to fetch data from a specific Kaggle dataset.
 
         In order to use `KaggleIngester`, valid Kaggle API credentials are required. These credentials can be obtained
@@ -222,15 +221,15 @@
             owner_slug: The owner's Kaggle username or organization name.
             dataset_slug: The dataset's unique Kaggle identifier (slug).
             file_pattern: Pattern to match the files to download, e.g. `*.csv` or [`*.csv`, `*.json`], etc.
                 For more information, see https://docs.python.org/3/library/fnmatch.html.
             dataset_id: Id of the dataset to be used instead of the default fingerprint (MD5 hash of the owner slug,
                 dataset version, and dataset slug). Note that this will overwrite any existing dataset with the same
                 name in the destination directory, so make sure to use a unique name.
-            cache_directory: The directory where the downloaded files will be stored.
+            destination_directory: The directory where the downloaded files will be stored.
             dataset_version: The specific dataset version number to download. If not provided,
                 the latest version will be fetched.
             kaggle_api_credentials_file: Path to a Kaggle API credentials JSON file. If not
                 provided, environment variables or the default file location will be used.
             num_workers: Number of concurrent threads to use when downloading files.
 
         Examples:
@@ -247,17 +246,17 @@
             [PosixPath('~/data/covid-19/file_1.zip'), PosixPath('~/data/covid-19/file_2.zip')]
         """
         dataset_id = (
             dataset_id
             if dataset_id is not None
             else hashlib.md5((owner_slug + dataset_slug + str(dataset_version)).encode()).hexdigest()
         )
-        super().__init__(cache_directory, dataset_id)
+        super().__init__(destination_directory, dataset_id)
         self._local_manifest_handler = LocalManifestHandler(
-            self._cache_directory / f"{self._fingerprint}.manifest.json"
+            self._destination_directory / f"{self._fingerprint}.manifest.json"
         )
         self._owner_slug = owner_slug
         self._dataset_slug = dataset_slug
         self._dataset_version = dataset_version
         self._kaggle_config = KaggleCredentialsManager.get_kaggle_credentials(kaggle_api_credentials_file)
         self._num_workers = num_workers
 
@@ -285,47 +284,47 @@
         if self._dataset_version:
             params["datasetVersionNumber"] = str(self._dataset_version)
         kaggle_manifest = self._build_kaggle_manifest(params)
 
         if force_recompute:
             logger.info(
                 f"\033[33mForce Cache Refresh\033[0m: Downloading files matching {self._file_pattern} from "
-                f"{dataset_path} to {self._cache_directory} from Kaggle."
+                f"{dataset_path} to {self._destination_directory} from Kaggle."
             )
         else:
             if self._is_local_dataset_fresh(kaggle_manifest):
                 logger.info("\033[32mCache Hit\033[0m: Local dataset is up to date with Kaggle, skipping download.")
                 local_file_names = set(self._local_manifest_handler.get_file_names())
                 kaggle_file_names: set[str] = {kaggle_file.name for kaggle_file in kaggle_manifest}
                 files_to_delete = list(local_file_names.difference(kaggle_file_names))
 
                 if len(files_to_delete) > 0:
                     logger.info(
                         f"Deleting {len(files_to_delete)} files from "
-                        f"{self._cache_directory} that are no longer present in Kaggle or filtered out."
+                        f"{self._destination_directory} that are no longer present in Kaggle or filtered out."
                     )
 
                 self._delete_local_files(files_to_delete)
                 self._local_manifest_handler.remove_files(files_to_delete)
                 return self._get_full_file_paths(self._local_manifest_handler.get_file_names())
 
             logger.info(
                 f"\033[31mCache Miss\033[0m: Downloading files matching {self._file_pattern} from "
-                f"{dataset_path} to {self._cache_directory} from Kaggle."
+                f"{dataset_path} to {self._destination_directory} from Kaggle."
             )
 
         self._delete_local_files(self._local_manifest_handler.get_file_names())
         kaggle_file_paths = [f"{dataset_path}/{file_metadata.name}" for file_metadata in kaggle_manifest]
         if len(kaggle_file_paths) > 0:
             self._kaggle_fetch_files(kaggle_file_paths, params)
             self._local_manifest_handler.set_files(
                 [
                     LocalFileEntry(
                         name=Path(kaggle_file_paths[0]).name,
-                        size=os.path.getsize(self._cache_directory / Path(kaggle_file_paths[0]).name),
+                        size=os.path.getsize(self._destination_directory / Path(kaggle_file_paths[0]).name),
                     )
                 ]
             )
             logger.info(f"Finished downloading {len(kaggle_file_paths)} files from Kaggle.")
 
         return self._get_full_file_paths(self._local_manifest_handler.get_file_names())
 
@@ -384,15 +383,15 @@
         Args:
             kaggle_file_path: The Kaggle file path to download.
             params: The request parameters containing the dataset version number, if applicable.
 
         Raises:
             HTTPError: If there is an error in the HTTP response while downloading file from Kaggle.
         """
-        local_file_path = self._cache_directory / Path(kaggle_file_path).name
+        local_file_path = self._destination_directory / Path(kaggle_file_path).name
         response = requests.get(
             f"{self._KAGGLE_DATASET_URL}/download/{kaggle_file_path}",
             params=params,
             auth=HTTPBasicAuth(self._kaggle_config.username, self._kaggle_config.key),
             timeout=5,
             stream=True,
         )
@@ -441,15 +440,15 @@
         Args:
             files_metadata: A list containing the metadata of the files in the Kaggle dataset.
 
         Returns:
             True if the local dataset files are up to date, False otherwise.
         """
         for file in files_metadata:
-            local_file_path = self._cache_directory / file.name
+            local_file_path = self._destination_directory / file.name
             if (
                 not local_file_path.exists()
                 or file.total_bytes != os.path.getsize(local_file_path)
                 or file.creation_timestamp > os.path.getmtime(local_file_path)
             ):
                 return False
         return True
```

### Comparing `mleko-3.2.0/mleko/dataset/ingest/s3_ingester.py` & `mleko-4.0.0/mleko/dataset/ingest/s3_ingester.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,28 @@
 """Module for fetching data from AWS S3 and storing it locally using the `S3Ingester` class."""
 
 from __future__ import annotations
 
 import hashlib
 import os
 from concurrent import futures
-from dataclasses import dataclass
-from datetime import date
-from fnmatch import fnmatch
+from itertools import repeat
 from pathlib import Path
 
-import boto3
-from boto3.s3.transfer import TransferConfig as BotoTransferConfig
-from botocore.config import Config as BotoConfig
 from tqdm.auto import tqdm
 
-from mleko.utils.custom_logger import CustomLogger
-from mleko.utils.decorators import auto_repr
+from mleko.utils import CustomLogger, LocalFileEntry, LocalManifestHandler, S3Client, auto_repr
 
-from .base_ingester import BaseIngester, LocalFileEntry, LocalManifestHandler
+from .base_ingester import BaseIngester
 
 
 logger = CustomLogger()
 """A module-level custom logger."""
 
 
-@dataclass
-class S3FileManifest:
-    """Manifest entry for a single S3 file."""
-
-    key: Path
-    """Key of the file, the full path of the file in the S3 bucket including the key prefix."""
-
-    size: int
-    """Size of the file in bytes."""
-
-    last_modified: date
-    """Last modified date of the file."""
-
-
 class S3Ingester(BaseIngester):
     """`S3Ingester` provides a convenient interface for fetching data from AWS S3 buckets and storing it locally.
 
     This class interacts with AWS S3 to download specified data from an S3 bucket.
     It supports manifest-based caching, enabling more efficient data fetching by verifying if the
     local dataset is up-to-date before downloading.
     """
@@ -50,261 +30,196 @@
     @auto_repr
     def __init__(
         self,
         s3_bucket_name: str,
         s3_key_prefix: str,
         file_pattern: str | list[str] = "*",
         dataset_id: str | None = None,
-        cache_directory: str | Path = "data/s3-ingester",
+        destination_directory: str | Path = "data/s3-ingester",
         aws_profile_name: str | None = None,
         aws_region_name: str = "eu-west-1",
-        num_workers: int = 64,
-        check_s3_timestamps: bool = True,
+        max_concurrent_files: int = 64,
+        workers_per_file: int = 1,
+        manifest_file_name: str | None = "manifest",
+        s3_timestamp_tolerance: int = -1,
     ) -> None:
         """Initializes the S3 bucket client, configures the cache directory, and sets client-related parameters.
 
         Note:
             The S3 bucket client is initialized using the provided AWS profile and region. If no profile is provided,
             the default profile will be used. If no region is provided, the default region will be used.
 
             The profile and region is read from the AWS credentials file located at '~/.aws/credentials'.
 
+        Warning:
+            The `max_concurrent_files` and `workers_per_file` parameters are used to control the
+            number of concurrent downloads and parts downloaded per file, respectively. These parameters should be
+            set based on the available system resources and the S3 bucket's performance limits. The total number of
+            concurrent threads is the product of these two parameters
+            (i.e., `max_concurrent_files * workers_per_file`).
+
         Args:
             s3_bucket_name: Name of the S3 bucket containing the data.
             s3_key_prefix: Prefix of the S3 keys for the files to download
             file_pattern: Pattern to match the files to download, e.g. `*.csv` or [`*.csv`, `*.json`], etc.
                 For more information, see https://docs.python.org/3/library/fnmatch.html.
             dataset_id: Id of the dataset to be used instead of the default fingerprint (MD5 hash of the bucket
                 name, key prefix, and region name). Note that this will overwrite any existing dataset with the same
                 name in the cache directory, so make sure to use a unique name.
-            cache_directory: Directory to store the fetched data locally.
+            destination_directory: Directory to store the fetched data locally.
             aws_profile_name: AWS profile name to use.
             aws_region_name: AWS region name where the S3 bucket is located.
-            num_workers: Number of workers to use for concurrent downloads.
-            check_s3_timestamps: Whether to check if all S3 files have the same timestamp.
+            max_concurrent_files: Maximum number of files to download concurrently.
+            workers_per_file: Number of parts to download concurrently for each file. This is useful for
+                downloading large files faster, as it allows for parallel downloads of different parts of the file.
+            manifest_file_name: Name of the manifest file located on S3. If provided, the manifest from S3 will
+                be used to determine the files to include, before applying the file pattern.
+            s3_timestamp_tolerance: Tolerance in hours for the difference in last modified timestamps of files in the S3
+                bucket. If the difference is greater than this value, an exception will be raised. If set to -1, no
+                check will be performed.
 
         Examples:
             >>> from mleko.dataset.sources import S3Ingester
             >>> s3_ingester = S3Ingester(
             ...     s3_bucket_name="mleko-datasets",
             ...     s3_key_prefix="kaggle/ashishpatel26/indian-food-101",
             ...     file_pattern="file_*.csv",
             ...     dataset_id="indian_food", # Optional, but will store the data in "./data/indian_food/" instead of
             ...                               # "./data/<fingerprint>/".
             ...     aws_profile_name="mleko",
             ...     aws_region_name="eu-west-1",
-            ...     num_workers=64,
-            ...     check_s3_timestamps=True,
+            ...     s3_timestamp_tolerance=2,
             ... )
             >>> s3_ingester.fetch_data()
             [PosixPath('data/indian_food/indian_food.csv')]
         """
         dataset_id = (
             dataset_id
             if dataset_id is not None
             else hashlib.md5((s3_bucket_name + s3_key_prefix + aws_region_name).encode()).hexdigest()
         )
-        super().__init__(cache_directory, dataset_id)
+        super().__init__(destination_directory, dataset_id)
         self._local_manifest_handler = LocalManifestHandler(
-            self._cache_directory / f"{self._fingerprint}.manifest.json"
+            self._destination_directory / f"{self._fingerprint}.manifest.json"
         )
         self._s3_bucket_name = s3_bucket_name
         self._s3_key_prefix = s3_key_prefix
         self._aws_profile_name = aws_profile_name
         self._aws_region_name = aws_region_name
-        self._s3_client = self._get_s3_client(self._aws_profile_name, self._aws_region_name)
-        self._num_workers = num_workers
-        self._check_s3_timestamps = check_s3_timestamps
+        self._s3_client = S3Client(self._aws_profile_name, self._aws_region_name)
+        self._max_concurrent_files = max_concurrent_files
+        self._workers_per_file = workers_per_file
+        self._manifest_file_name = manifest_file_name
+        self._s3_timestamp_tolerance = s3_timestamp_tolerance
 
         if isinstance(file_pattern, str):
             file_pattern = [file_pattern]
         self._file_pattern = file_pattern
 
     def fetch_data(self, force_recompute: bool = False) -> list[Path]:
-        """Downloads the data from the S3 bucket and stores it in the 'cache_directory'.
+        """Downloads the data from the S3 bucket and stores it in the 'destination_directory'.
 
-        If 'force_recompute' is False, verifies whether the data in the local 'cache_directory' is current
+        If 'force_recompute' is False, verifies whether the data in the local 'destination_directory' is current
         with the S3 bucket contents based on the manifest file, and skips downloading if it is up to date.
 
         Args:
             force_recompute: Whether to force the data source to recompute its output, even if it already exists.
 
         Raises:
             Exception: If files in the S3 bucket have different last modified dates, indicating potential corruption
                        or duplication.
+            FileNotFoundError: If no files matching the file pattern are found in the S3 bucket.
 
         Returns:
             A list of Path objects pointing to the downloaded data files.
         """
-        self._s3_client = self._get_s3_client(self._aws_profile_name, self._aws_region_name)
-        s3_manifest = self._build_s3_manifest()
+        self._s3_client.refresh_client()
+        s3_manifest = self._s3_client.get_s3_manifest(
+            bucket_name=self._s3_bucket_name,
+            key_prefix=self._s3_key_prefix,
+            manifest_file_name=self._manifest_file_name,
+            file_pattern=self._file_pattern,
+        )
+        if len(s3_manifest) == 0:
+            msg = (
+                f"No files matching {self._file_pattern} found in S3 bucket "
+                f"{self._s3_bucket_name}/{self._s3_key_prefix}."
+            )
+            logger.error(msg)
+            raise FileNotFoundError(msg)
+        logger.info(f"Found {len(s3_manifest)} file(s) matching any of {self._file_pattern} in S3 bucket.")
 
-        if self._check_s3_timestamps:
-            modification_dates = {key.last_modified for key in s3_manifest}
-            if len(modification_dates) > 1:
-                error_msg = "Files in S3 are from muliples dates. This might mean the data is corrupted/duplicated."
+        s3_path_string = f"s3://{Path(self._s3_bucket_name) / self._s3_key_prefix}/"
+        if self._s3_timestamp_tolerance >= 0:
+            modification_datetimes = [key.last_modified for key in s3_manifest]
+            diff_modification_datetimes = max(modification_datetimes) - min(modification_datetimes)
+            if diff_modification_datetimes.total_seconds() > self._s3_timestamp_tolerance * 3600:
+                error_msg = (
+                    f"Files in S3 bucket {s3_path_string} have last modified "
+                    f"timestamps differing by more than {self._s3_timestamp_tolerance} hours. "
+                    f"Potential corruption or duplication detected."
+                )
                 logger.error(error_msg)
                 raise Exception(error_msg)
 
         if force_recompute:
             logger.info(
                 f"\033[33mForce Cache Refresh\033[0m: Downloading files matching {self._file_pattern} from "
-                f"{self._s3_bucket_name}/{self._s3_key_prefix} to {self._cache_directory} from S3."
+                f"{s3_path_string} to {self._destination_directory}."
             )
         else:
-            if self._is_local_dataset_fresh(s3_manifest):
+            if self._s3_client.is_local_dataset_up_to_date(self._destination_directory, s3_manifest):
                 logger.info(
                     "\033[32mCache Hit\033[0m: Local dataset is up to date with S3 bucket contents, "
                     "skipping download."
                 )
                 local_file_names = set(self._local_manifest_handler.get_file_names())
                 s3_file_names: set[str] = {s3_file.key.name for s3_file in s3_manifest}
                 files_to_delete = list(local_file_names.difference(s3_file_names))
 
                 if len(files_to_delete) > 0:
                     logger.info(
                         f"Deleting {len(files_to_delete)} files from "
-                        f"{self._cache_directory} that are no longer present in S3 or filtered out."
+                        f"{self._destination_directory} that are no longer present in S3 or filtered out."
                     )
 
                 self._delete_local_files(files_to_delete)
                 self._local_manifest_handler.remove_files(files_to_delete)
                 return self._get_full_file_paths(self._local_manifest_handler.get_file_names())
 
             logger.info(
-                f"\033[31mCache Miss\033[0m: Downloading {self._s3_bucket_name}/{self._s3_key_prefix} to "
-                f"{self._cache_directory} from S3."
+                f"\033[31mCache Miss\033[0m: Downloading files matching {self._file_pattern} from "
+                f"{s3_path_string} to {self._destination_directory}."
             )
 
         self._delete_local_files(self._local_manifest_handler.get_file_names())
         keys_to_download: list[str] = [str(s3_file.key) for s3_file in s3_manifest]
         if len(keys_to_download) > 0:
             self._s3_fetch_all(keys_to_download)
             self._local_manifest_handler.set_files(
                 [
-                    LocalFileEntry(name=Path(key).name, size=os.path.getsize(self._cache_directory / Path(key).name))
+                    LocalFileEntry(
+                        name=Path(key).name, size=os.path.getsize(self._destination_directory / Path(key).name)
+                    )
                     for key in keys_to_download
                 ]
             )
             logger.info(f"Finished downloading {len(keys_to_download)} files from S3.")
 
         return self._get_full_file_paths(self._local_manifest_handler.get_file_names())
 
-    def _build_s3_manifest(self) -> list[S3FileManifest]:
-        """Builds a manifest from the S3 response.
-
-        The manifest contains the S3 keys, sizes, and last modified dates of the files in the S3 bucket.
-
-        Raises:
-            FileNotFoundError: If no files matching the file pattern are found in the S3 bucket.
-
-        Returns:
-            A list of `S3FileManifest` objects containing the S3 keys, sizes, and last modified dates of the files in
-            the S3 bucket.
-        """
-        resp = self._s3_client.list_objects(
-            Bucket=self._s3_bucket_name,
-            Prefix=self._s3_key_prefix,
-        )
-
-        s3_manifest: list[S3FileManifest] = [
-            S3FileManifest(key=Path(key["Key"]), size=key["Size"], last_modified=key["LastModified"].date())
-            for key in resp.get("Contents", [])
-            if "LastModified" in key
-            and "Key" in key
-            and "Size" in key
-            and any(fnmatch(Path(key["Key"]).name, pattern) for pattern in self._file_pattern)
-        ]
-
-        if len(s3_manifest) == 0:
-            msg = (
-                f"No files matching {self._file_pattern} found in S3 bucket "
-                f"{self._s3_bucket_name}/{self._s3_key_prefix}."
-            )
-            logger.error(msg)
-            raise FileNotFoundError(msg)
-        logger.info(f"Found {len(s3_manifest)} file(s) matching any of {self._file_pattern} in S3 bucket.")
-
-        return s3_manifest
-
-    def _get_s3_client(
-        self,
-        aws_profile_name: str | None,
-        aws_region_name: str,
-    ):
-        """Creates an S3 client using the provided AWS profile and region.
-
-        Args:
-            aws_profile_name: AWS profile name to use.
-            aws_region_name: AWS region name where the S3 bucket is located.
-
-        Returns:
-            An S3 client configured with the specified profile and region.
-        """
-        credentials = boto3.Session(
-            region_name=aws_region_name,
-            profile_name=aws_profile_name,
-        ).get_credentials()
-
-        if credentials is None:
-            msg = "AWS credentials not found. Please ensure that your AWS credentials are correctly set up."
-            logger.error(msg)
-            raise ValueError(msg)
-
-        client_config = BotoConfig(max_pool_connections=100)
-        return boto3.client(
-            "s3",  # type: ignore
-            aws_access_key_id=credentials.access_key,
-            aws_secret_access_key=credentials.secret_key,
-            aws_session_token=credentials.token,
-            region_name=aws_region_name,
-            config=client_config,
-        )
-
-    def _s3_fetch_file(self, key: str) -> None:
-        """Downloads a single file from the S3 bucket to the destination specified in the constructor.
-
-        Args:
-            key: S3 key of the file to download.
-        """
-        gb = 1024**3
-        transfer_config = BotoTransferConfig(
-            use_threads=False,
-            multipart_threshold=int(0.5 * gb),  # Multipart transfer if file > 500MB
-        )
-        file_path = self._cache_directory / Path(key).name
-        with open(file_path, "wb") as data:
-            self._s3_client.download_fileobj(
-                Bucket=self._s3_bucket_name,
-                Key=key,
-                Fileobj=data,
-                Config=transfer_config,
-            )
-
     def _s3_fetch_all(self, keys: list[str]) -> None:
         """Downloads all specified files from the S3 bucket to the local directory concurrently.
 
         Args:
             keys: List of S3 keys for the files to download.
         """
         with tqdm(total=len(keys), desc="Downloading files from S3") as pbar:
-            with futures.ThreadPoolExecutor(max_workers=self._num_workers) as executor:
+            with futures.ThreadPoolExecutor(max_workers=min(len(keys), self._max_concurrent_files)) as executor:
                 for _ in executor.map(
-                    self._s3_fetch_file,
+                    self._s3_client.download_file,
+                    repeat(self._destination_directory),
+                    repeat(self._s3_bucket_name),
                     keys,
+                    repeat(self._workers_per_file),
                 ):
                     pbar.update(1)
-
-    def _is_local_dataset_fresh(self, s3_manifest: list[S3FileManifest]) -> bool:
-        """Checks if the local dataset is up-to-date with the S3 manifest.
-
-        Args:
-            s3_manifest: Manifest built from S3 response.
-
-        Returns:
-            True if the local dataset is up-to-date, False otherwise.
-        """
-        for s3_file in s3_manifest:
-            local_file_path = self._cache_directory / s3_file.key.name
-            if not local_file_path.exists() or s3_file.size != os.path.getsize(local_file_path):
-                return False
-        return True
```

### Comparing `mleko-3.2.0/mleko/dataset/split/__init__.py` & `mleko-4.0.0/mleko/dataset/split/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/split/base_splitter.py` & `mleko-4.0.0/mleko/dataset/split/base_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/split/expression_splitter.py` & `mleko-4.0.0/mleko/dataset/split/expression_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/split/random_splitter.py` & `mleko-4.0.0/mleko/dataset/split/random_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/transform/__init__.py` & `mleko-4.0.0/mleko/dataset/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/transform/base_transformer.py` & `mleko-4.0.0/mleko/dataset/transform/base_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Hashable
 
 import vaex
 
-from mleko.cache.fingerprinters import DictFingerprinter, VaexFingerprinter
+from mleko.cache.fingerprinters import JsonFingerprinter, VaexFingerprinter
 from mleko.cache.handlers.joblib_cache_handler import JOBLIB_CACHE_HANDLER
 from mleko.cache.handlers.vaex_cache_handler import VAEX_DATAFRAME_CACHE_HANDLER
 from mleko.cache.lru_cache_mixin import LRUCacheMixin
 from mleko.dataset.data_schema import DataSchema
 from mleko.utils.custom_logger import CustomLogger
 
 
@@ -72,15 +72,15 @@
         Returns:
             Updated data schema and fitted transformer.
         """
         ds, transformer = self._cached_execute(
             lambda_func=lambda: self._fit(data_schema, dataframe),
             cache_key_inputs=[
                 self._fingerprint(),
-                (data_schema.to_dict(), DictFingerprinter()),
+                (data_schema.to_dict(), JsonFingerprinter()),
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=JOBLIB_CACHE_HANDLER,
             disable_cache=disable_cache,
         )
@@ -115,15 +115,15 @@
             logger.error(msg)
             raise RuntimeError(msg)
 
         ds, df = self._cached_execute(
             lambda_func=lambda: self._transform(data_schema, dataframe),
             cache_key_inputs=[
                 self._fingerprint(),
-                (data_schema.to_dict(), DictFingerprinter()),
+                (data_schema.to_dict(), JsonFingerprinter()),
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=[JOBLIB_CACHE_HANDLER, VAEX_DATAFRAME_CACHE_HANDLER],
             disable_cache=disable_cache,
         )
@@ -150,15 +150,15 @@
         Returns:
             Tuple of updated data schema, fitted transformer, and transformed DataFrame.
         """
         ds, transformer, df = self._cached_execute(
             lambda_func=lambda: self._fit_transform(data_schema, dataframe),
             cache_key_inputs=[
                 self._fingerprint(),
-                (data_schema.to_dict(), DictFingerprinter()),
+                (data_schema.to_dict(), JsonFingerprinter()),
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=[JOBLIB_CACHE_HANDLER, JOBLIB_CACHE_HANDLER, VAEX_DATAFRAME_CACHE_HANDLER],
             disable_cache=disable_cache,
         )
```

### Comparing `mleko-3.2.0/mleko/dataset/transform/composite_transformer.py` & `mleko-4.0.0/mleko/dataset/transform/composite_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/transform/frequency_encoder_transformer.py` & `mleko-4.0.0/mleko/dataset/transform/frequency_encoder_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/transform/label_encoder_transformer.py` & `mleko-4.0.0/mleko/dataset/transform/label_encoder_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 from pathlib import Path
 from typing import Hashable
 
 import vaex
 import vaex.array_types
 
-from mleko.cache.fingerprinters import DictFingerprinter
+from mleko.cache.fingerprinters import JsonFingerprinter
 from mleko.dataset.data_schema import DataSchema
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.vaex_helpers import get_column
 
 from .base_transformer import BaseTransformer
 
@@ -191,15 +191,15 @@
         Returns:
             A hashable object that uniquely identifies the transformer.
         """
         return (
             super()._fingerprint(),
             self._allow_unseen,
             self._encode_null,
-            DictFingerprinter().fingerprint(self._label_dict),
+            JsonFingerprinter().fingerprint(self._label_dict),
         )
 
     def _fit_using_label_dict(self, feature: str, observed_labels: list[str]) -> bool:
         """Attempts to fit the label dictionary for the specified feature.
 
         If the label dictionary is not provided or the feature is not in the label dictionary, the function will
         return False. Otherwise, it will fit the label dictionary and return True.
```

### Comparing `mleko-3.2.0/mleko/dataset/transform/max_abs_scaler_transformer.py` & `mleko-4.0.0/mleko/dataset/transform/max_abs_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/dataset/transform/min_max_scaler_transformer.py` & `mleko-4.0.0/mleko/dataset/transform/min_max_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/model/base_model.py` & `mleko-4.0.0/mleko/model/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, Hashable, Union
 
 import pandas as pd
 import vaex
 
-from mleko.cache.fingerprinters import DictFingerprinter, VaexFingerprinter
+from mleko.cache.fingerprinters import JsonFingerprinter, VaexFingerprinter
 from mleko.cache.handlers import JOBLIB_CACHE_HANDLER, VAEX_DATAFRAME_CACHE_HANDLER
 from mleko.cache.lru_cache_mixin import LRUCacheMixin
 from mleko.dataset.data_schema import DataSchema
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.vaex_helpers import HashableVaexDataFrame, get_columns
 
 
@@ -143,17 +143,17 @@
                 self._fingerprint(),
                 (
                     (
                         {**self._hyperparameters, **hyperparameters}
                         if hyperparameters is not None
                         else self._hyperparameters
                     ),
-                    DictFingerprinter(),
+                    JsonFingerprinter(),
                 ),
-                (data_schema.to_dict(), DictFingerprinter()),
+                (data_schema.to_dict(), JsonFingerprinter()),
                 (train_dataframe, VaexFingerprinter()),
                 (validation_dataframe, VaexFingerprinter()) if validation_dataframe is not None else "None",
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=JOBLIB_CACHE_HANDLER,
             disable_cache=disable_cache,
@@ -189,16 +189,16 @@
             logger.error(msg)
             raise RuntimeError(msg)
 
         return self._cached_execute(
             lambda_func=lambda: self._transform(data_schema, dataframe),
             cache_key_inputs=[
                 self._fingerprint(),
-                (self._hyperparameters, DictFingerprinter()),
-                (data_schema.to_dict(), DictFingerprinter()),
+                (self._hyperparameters, JsonFingerprinter()),
+                (data_schema.to_dict(), JsonFingerprinter()),
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=VAEX_DATAFRAME_CACHE_HANDLER,
             disable_cache=disable_cache,
         )
@@ -251,17 +251,17 @@
                 self._fingerprint(),
                 (
                     (
                         {**self._hyperparameters, **hyperparameters}
                         if hyperparameters is not None
                         else self._hyperparameters
                     ),
-                    DictFingerprinter(),
+                    JsonFingerprinter(),
                 ),
-                (data_schema.to_dict(), DictFingerprinter()),
+                (data_schema.to_dict(), JsonFingerprinter()),
                 (train_dataframe, VaexFingerprinter()),
                 (validation_dataframe, VaexFingerprinter()) if validation_dataframe is not None else None,
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
             cache_handlers=[
                 JOBLIB_CACHE_HANDLER,
```

### Comparing `mleko-3.2.0/mleko/model/lgbm_model.py` & `mleko-4.0.0/mleko/model/lgbm_model.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/model/tune/base_tuner.py` & `mleko-4.0.0/mleko/model/tune/base_tuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Hashable
 
 import vaex
 
-from mleko.cache.fingerprinters import DictFingerprinter, VaexFingerprinter
-from mleko.cache.handlers import JOBLIB_CACHE_HANDLER, PICKLE_CACHE_HANDLER
+from mleko.cache.fingerprinters import JsonFingerprinter, VaexFingerprinter
+from mleko.cache.handlers import JOBLIB_CACHE_HANDLER, JSON_CACHE_HANDLER, PICKLE_CACHE_HANDLER
 from mleko.cache.lru_cache_mixin import LRUCacheMixin
 from mleko.dataset.data_schema import DataSchema
 from mleko.model.base_model import HyperparametersType
 
 
 class BaseTuner(LRUCacheMixin, ABC):
     """Abstract base class for hyperparameter tuners."""
@@ -54,20 +54,20 @@
             is specific to each tuner, please refer to the documentation of the tuner
             for more information.
         """
         return self._cached_execute(
             lambda_func=lambda: self._tune(data_schema, dataframe),
             cache_key_inputs=[
                 self._fingerprint(),
-                (data_schema.to_dict(), DictFingerprinter()),
+                (data_schema.to_dict(), JsonFingerprinter()),
                 (dataframe, VaexFingerprinter()),
             ],
             cache_group=cache_group,
             force_recompute=force_recompute,
-            cache_handlers=[JOBLIB_CACHE_HANDLER, JOBLIB_CACHE_HANDLER, PICKLE_CACHE_HANDLER],
+            cache_handlers=[JSON_CACHE_HANDLER, JOBLIB_CACHE_HANDLER, PICKLE_CACHE_HANDLER],
             disable_cache=disable_cache,
         )
 
     @abstractmethod
     def _tune(
         self, data_schema: DataSchema, dataframe: vaex.DataFrame
     ) -> tuple[HyperparametersType, float | list[float] | tuple[float, ...], Any]:
```

### Comparing `mleko-3.2.0/mleko/model/tune/optuna_tuner.py` & `mleko-4.0.0/mleko/model/tune/optuna_tuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 from optuna.storages import RDBStorage
 from optuna_dashboard import save_note
 from tqdm.auto import tqdm
 
 from mleko import __version__ as mleko_version
 from mleko.cache.fingerprinters import (
     CallableSourceFingerprinter,
+    JsonFingerprinter,
     OptunaPrunerFingerprinter,
     OptunaSamplerFingerprinter,
 )
-from mleko.cache.fingerprinters.dict_fingerprinter import DictFingerprinter
 from mleko.dataset.data_schema import DataSchema
 from mleko.model.base_model import HyperparametersType
 from mleko.utils.custom_logger import CustomLogger
 
 from .base_tuner import BaseTuner
 
 
@@ -203,20 +203,14 @@
 
         optuna_logger = logging.getLogger("optuna")
         for handler in optuna_logger.handlers:
             optuna_logger.removeHandler(handler)
         for handler in logger.handlers:
             optuna_logger.addHandler(handler)
 
-        if self._storage is not None:
-            storage_name = self._storage if isinstance(self._storage, str) else self._storage.url
-            logger.info(
-                f"Optuna study named {self._study_name!r} is stored in {storage_name}, use optuna-dashboard to view it."
-            )
-
     def _tune(
         self, data_schema: DataSchema, dataframe: vaex.DataFrame
     ) -> tuple[HyperparametersType, float | list[float] | tuple[float, ...], optuna.study.Study]:
         """Perform the hyperparameter tuning.
 
         Args:
             data_schema: Data schema for the DataFrame.
@@ -338,15 +332,15 @@
             OptunaSamplerFingerprinter().fingerprint(self._sampler),
             OptunaPrunerFingerprinter().fingerprint(self._pruner),
             self._random_state,
             (
                 self._storage
                 if isinstance(self._storage, str)
                 else (
-                    self._storage.url + DictFingerprinter().fingerprint(self._storage.engine_kwargs)
+                    self._storage.url + JsonFingerprinter().fingerprint(self._storage.engine_kwargs)
                     if self._storage is not None
                     else None
                 )
             ),
             self._load_if_exists,
         )
```

### Comparing `mleko-3.2.0/mleko/pipeline/__init__.py` & `mleko-4.0.0/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/pipeline/data_container.py` & `mleko-4.0.0/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/pipeline/pipeline.py` & `mleko-4.0.0/mleko/pipeline/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         """
         self._steps = steps if steps is not None else []
 
     def __repr__(self) -> str:
         """Returns a string representation of the Pipeline, including the ordered list of steps.
 
         Returns:
-            String representaition of Pipeline that includes the class name and each step in the order they appear
+            String representation of Pipeline that includes the class name and each step in the order they appear
             in the pipeline, numbered for easier identification.
         """
         cls_name = type(self).__name__
         steps_str = "\n".join([f"  {index + 1}. {step!r}" for index, step in enumerate(self._steps)])
         return f"{cls_name}:\n{steps_str}"
 
     def add_step(self, step: PipelineStep) -> None:
@@ -54,32 +54,35 @@
         appended to the pipeline when calling the `run` method.
 
         Args:
             step: The PipelineStep instance to be added at the end of the pipeline's steps list.
         """
         self._steps.append(step)
 
-    def run(self, data_container: DataContainer | None = None, force_recompute: bool = False) -> DataContainer:
+    def run(
+        self, data_container: DataContainer | None = None, force_recompute: bool = False, disable_cache: bool = False
+    ) -> DataContainer:
         """Executes the pipeline steps in the order they were added, passing output from one to the next.
 
         Processes the initial given data or an empty data container through each step in the pipeline.
         The output of each step is passed as input to the next step, allowing the given input to be transformed
         through the whole sequence of steps.
 
         Args:
             data_container: An optional DataContainer instance carrying the input data to be processed by the
                             first step in the pipeline. If not provided, an empty DataContainer instance will be
                             created automatically, and the first step's execute method must handle it.
             force_recompute: Whether to force the pipeline to recompute its output, even if it already exists.
+            disable_cache: Whether to disable the `mleko` caching mechanism for the pipeline execution.
 
         Returns:
             The output as a DataContainer instance from the last step in the pipeline after processing the data.
         """
         if data_container is None:
             logger.info("No data container provided. Creating an empty one.")
             data_container = DataContainer()
 
         for i, step in enumerate(self._steps):
             logger.info(f"Executing step {i+1}/{len(self._steps)}: {step.__class__.__name__}.")
-            data_container = step.execute(data_container, force_recompute)
+            data_container = step.execute(data_container, force_recompute, disable_cache)
             logger.info(f"Finished step {i+1}/{len(self._steps)} execution.")
         return data_container
```

### Comparing `mleko-3.2.0/mleko/pipeline/pipeline_step.py` & `mleko-4.0.0/mleko/pipeline/pipeline_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,24 +82,25 @@
         self._outputs = outputs
         self._cache_group = cache_group
 
         self._validate_inputs()
         self._validate_outputs()
 
     @abstractmethod
-    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool, disable_cache: bool) -> DataContainer:
         """Execute the data processing operation associated with this pipeline step.
 
         The `execute` method is the main entry point for the data processing operation associated with this step.
         It receives a `DataContainer` instance as input, containing the data to be processed by this step.
         The method should perform the processing operation and return the processed data as a `DataContainer` instance.
 
         Args:
             data_container: Input data for this step's processing operation.
             force_recompute: Whether to force the step to recompute its output, even if it already exists.
+            disable_cache: If set to True, disables the cache.
 
         Raises:
             NotImplementedError: Must be implemented by subclass.
         """
         raise NotImplementedError
 
     @abstractmethod
```

### Comparing `mleko-3.2.0/mleko/pipeline/steps/convert_step.py` & `mleko-4.0.0/mleko/pipeline/steps/convert_step.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,34 +63,35 @@
             inputs: A dictionary of input keys following the `ConvertStepInputType` schema.
             outputs: A dictionary of output keys following the `ConvertStepOutputType` schema.
             cache_group: The cache group to use.
         """
         super().__init__(inputs, outputs, cache_group)
         self._converter = converter
 
-    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool, disable_cache: bool) -> DataContainer:
         """Perform data format conversion using the configured converter.
 
         Args:
             data_container: Contains a list of file Paths to be converted.
             force_recompute: Whether to force the step to recompute its output, even if it already exists.
+            disable_cache: If set to True, disables the cache.
 
         Raises:
             ValueError: If the input data types are invalid.
 
         Returns:
             A DataContainer containing the result.
         """
         file_paths = self._validate_and_get_input(self._inputs["file_paths"], list, data_container)
         if not all(isinstance(e, Path) or isinstance(e, str) for e in file_paths):
             msg = "Invalid data type: {type(file_paths)}. Expected List[Path] or List[str]."
             logger.error(msg)
             raise ValueError(msg)
 
-        data_schema, dataframe = self._converter.convert(file_paths, self._cache_group, force_recompute)
+        data_schema, dataframe = self._converter.convert(file_paths, self._cache_group, force_recompute, disable_cache)
         data_container.data[self._outputs["data_schema"]] = data_schema
         data_container.data[self._outputs["dataframe"]] = dataframe
         return data_container
 
     def _get_input_model(self) -> type[ConvertStepInputType]:
         """Get the input type for the ConvertStep.
```

### Comparing `mleko-3.2.0/mleko/pipeline/steps/feature_select_step.py` & `mleko-4.0.0/mleko/pipeline/steps/feature_select_step.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,43 +85,46 @@
                 `FeatureSelectStepOutputTransformType`, or `FeatureSelectStepOutputFitTransformType` schema depending
                 on the action.
             cache_group: The cache group to use.
         """
         super().__init__(action, inputs, outputs, cache_group)
         self._feature_selector = feature_selector
 
-    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool, disable_cache: bool) -> DataContainer:
         """Perform feature selection using the configured feature selector.
 
         Args:
             data_container: Contains the input DataFrame.
             force_recompute: Whether to force the step to recompute its output, even if it already exists.
+            disable_cache: If set to True, disables the cache.
 
         Returns:
             A DataContainer containing the result depending on the action.
         """
         data_schema = self._validate_and_get_input(self._inputs["data_schema"], DataSchema, data_container)
         dataframe = self._validate_and_get_input(self._inputs["dataframe"], DataFrame, data_container)
 
         if self._action == "fit":
             self._outputs = cast(FeatureSelectStepOutputFitType, self._outputs)
             ds, feature_selector = self._feature_selector.fit(
-                data_schema, dataframe, self._cache_group, force_recompute
+                data_schema, dataframe, self._cache_group, force_recompute, disable_cache
             )
             data_container.data[self._outputs["data_schema"]] = ds
             data_container.data[self._outputs["feature_selector"]] = feature_selector
         elif self._action == "transform":
             self._outputs = cast(FeatureSelectStepOutputTransformType, self._outputs)
-            ds, df = self._feature_selector.transform(data_schema, dataframe, self._cache_group, force_recompute)
+            ds, df = self._feature_selector.transform(
+                data_schema, dataframe, self._cache_group, force_recompute, disable_cache
+            )
             data_container.data[self._outputs["data_schema"]] = ds
             data_container.data[self._outputs["dataframe"]] = df
         elif self._action == "fit_transform":
             self._outputs = cast(FeatureSelectStepOutputFitTransformType, self._outputs)
             ds, feature_selector, df = self._feature_selector.fit_transform(
-                data_schema, dataframe, self._cache_group, force_recompute
+                data_schema, dataframe, self._cache_group, force_recompute, disable_cache
             )
             data_container.data[self._outputs["data_schema"]] = ds
             data_container.data[self._outputs["feature_selector"]] = feature_selector
             data_container.data[self._outputs["dataframe"]] = df
         return data_container
 
     def _get_input_model(self) -> type[FeatureSelectStepInputType]:
```

### Comparing `mleko-3.2.0/mleko/pipeline/steps/filter_step.py` & `mleko-4.0.0/mleko/pipeline/steps/filter_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,28 +52,31 @@
             inputs: A dictionary of input keys following the `FilterStepInputType` schema.
             outputs: A dictionary of output keys following the `FilterStepOutputType` schema.
             cache_group: The cache group to use.
         """
         super().__init__(inputs, outputs, cache_group)
         self._filter = filter
 
-    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool, disable_cache: bool) -> DataContainer:
         """Perform data filtering using the configured filter.
 
         Args:
             data_container: Contains the DataFrame to be filtered.
             force_recompute: Whether to force the step to recompute its output, even if it already exists.
+            disable_cache: If set to True, disables the cache.
 
         Returns:
             A DataContainer containing the result.
         """
         data_schema = self._validate_and_get_input(self._inputs["data_schema"], DataSchema, data_container)
         dataframe = self._validate_and_get_input(self._inputs["dataframe"], DataFrame, data_container)
 
-        filtered_dataframe = self._filter.filter(data_schema, dataframe, self._cache_group, force_recompute)
+        filtered_dataframe = self._filter.filter(
+            data_schema, dataframe, self._cache_group, force_recompute, disable_cache
+        )
         data_container.data[self._outputs["dataframe"]] = filtered_dataframe
         return data_container
 
     def _get_input_model(self) -> type[FilterStepInputType]:
         """Get the input type for the FilterStep.
 
         Returns:
```

### Comparing `mleko-3.2.0/mleko/pipeline/steps/ingest_step.py` & `mleko-4.0.0/mleko/pipeline/steps/ingest_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,20 +47,21 @@
             ingester: The data source from which to fetch the data, a BaseIngester instance.
             inputs: A dictionary of input keys following the `IngestStepInputType` schema.
             outputs: A dictionary of output keys following the `IngestStepOutputType` schema.
         """
         super().__init__(inputs, outputs, None)
         self._ingester = ingester
 
-    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool, disable_cache: bool) -> DataContainer:
         """Fetch data from the configured data source and return a DataContainer with fetched files.
 
         Args:
             data_container: Input data for this step's processing operation.
             force_recompute: Whether to force the step to recompute its output, even if it already exists.
+            disable_cache: Not used for ingestion steps.
 
         Returns:
             A DataContainer containing the result.
         """
         files = self._ingester.fetch_data(force_recompute)
         data_container.data[self._outputs["file_paths"]] = files
         return data_container
```

### Comparing `mleko-3.2.0/mleko/pipeline/steps/model_step.py` & `mleko-4.0.0/mleko/pipeline/steps/model_step.py`

 * *Files 12% similar despite different names*

```diff
@@ -103,20 +103,21 @@
             outputs: A list of output keys following the `ModelStepOutputFitType`, `ModelStepOutputTransformType`, or
                 `ModelStepOutputFitTransformType` schema, depending on the action.
             cache_group: The cache group to use.
         """
         super().__init__(action, inputs, outputs, cache_group)
         self._model = model
 
-    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool, disable_cache: bool) -> DataContainer:
         """Perform actions using the configured model.
 
         Args:
             data_container: Contains the input.
             force_recompute: Whether to force the step to recompute its output, even if it already exists.
+            disable_cache: If set to True, disables the cache.
 
         Returns:
             A DataContainer containing the output of the action performed by the step, either the fitted model,
             the predictions on the DataFrame, or both.
         """
         data_schema = self._validate_and_get_input(self._inputs["data_schema"], DataSchema, data_container)
         dataframe = self._validate_and_get_input(self._inputs["dataframe"], DataFrame, data_container)
@@ -130,26 +131,38 @@
             hyperparameters: HyperparametersType | None = self._validate_and_get_input(
                 self._inputs["hyperparameters"], dict, data_container, is_optional=True
             )
 
         if self._action == "fit":
             self._outputs = cast(ModelStepOutputFitType, self._outputs)
             model, metrics = self._model.fit(
-                data_schema, dataframe, df_validation, hyperparameters, self._cache_group, force_recompute
+                data_schema,
+                dataframe,
+                df_validation,
+                hyperparameters,
+                self._cache_group,
+                force_recompute,
+                disable_cache,
             )
             data_container.data[self._outputs["model"]] = model
             data_container.data[self._outputs["metrics"]] = metrics
         elif self._action == "transform":
             self._outputs = cast(ModelStepOutputTransformType, self._outputs)
-            df = self._model.transform(data_schema, dataframe, self._cache_group, force_recompute)
+            df = self._model.transform(data_schema, dataframe, self._cache_group, force_recompute, disable_cache)
             data_container.data[self._outputs["dataframe"]] = df
         elif self._action == "fit_transform":
             self._outputs = cast(ModelStepOutputFitTransformType, self._outputs)
             model, metrics, df, df_validation = self._model.fit_transform(
-                data_schema, dataframe, df_validation, hyperparameters, self._cache_group, force_recompute
+                data_schema,
+                dataframe,
+                df_validation,
+                hyperparameters,
+                self._cache_group,
+                force_recompute,
+                disable_cache,
             )
             data_container.data[self._outputs["model"]] = model
             data_container.data[self._outputs["metrics"]] = metrics
             data_container.data[self._outputs["dataframe"]] = df
             if self._outputs["validation_dataframe"] is not None:
                 data_container.data[self._outputs["validation_dataframe"]] = df_validation
         return data_container
```

### Comparing `mleko-3.2.0/mleko/pipeline/steps/split_step.py` & `mleko-4.0.0/mleko/pipeline/steps/split_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,27 +51,28 @@
             inputs: A dictionary of input keys following the `SplitStepInputType` schema.
             outputs: A dictionary of output keys following the `SplitStepOutputType` schema.
             cache_group: The cache group to use.
         """
         super().__init__(inputs, outputs, cache_group)
         self._splitter = splitter
 
-    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool, disable_cache: bool) -> DataContainer:
         """Perform data splitting using the configured splitter.
 
         Args:
             data_container: Contains the DataFrame to be split.
             force_recompute: Whether to force the step to recompute its output, even if it already exists.
+            disable_cache: If set to True, disables the cache.
 
         Returns:
             A DataContainer containing the result.
         """
         dataframe = self._validate_and_get_input(self._inputs["dataframe"], DataFrame, data_container)
 
-        df1, df2 = self._splitter.split(dataframe, self._cache_group, force_recompute)
+        df1, df2 = self._splitter.split(dataframe, self._cache_group, force_recompute, disable_cache)
         data_container.data[self._outputs["dataframe_1"]] = df1
         data_container.data[self._outputs["dataframe_2"]] = df2
         return data_container
 
     def _get_input_model(self) -> type[SplitStepInputType]:
         """Get the input type for the SplitStep.
```

### Comparing `mleko-3.2.0/mleko/pipeline/steps/transform_step.py` & `mleko-4.0.0/mleko/pipeline/steps/transform_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,41 +80,46 @@
                 `TransformStepOutputTransformType`, or `TransformStepOutputFitTransformType` schemas, depending on
                 the action.
             cache_group: The cache group to use.
         """
         super().__init__(action, inputs, outputs, cache_group)
         self._transformer = transformer
 
-    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool, disable_cache: bool) -> DataContainer:
         """Perform transformation using the configured transformer.
 
         Args:
             data_container: Contains the input DataFrame.
             force_recompute: Whether to force the step to recompute its output, even if it already exists.
+            disable_cache: If set to True, disables the cache.
 
         Returns:
             A DataContainer containing the result depending on the action.
         """
         data_schema = self._validate_and_get_input(self._inputs["data_schema"], DataSchema, data_container)
         dataframe = self._validate_and_get_input(self._inputs["dataframe"], DataFrame, data_container)
 
         if self._action == "fit":
             self._outputs = cast(TransformStepOutputFitType, self._outputs)
-            ds, transformer = self._transformer.fit(data_schema, dataframe, self._cache_group, force_recompute)
+            ds, transformer = self._transformer.fit(
+                data_schema, dataframe, self._cache_group, force_recompute, disable_cache
+            )
             data_container.data[self._outputs["data_schema"]] = ds
             data_container.data[self._outputs["transformer"]] = transformer
         elif self._action == "transform":
             self._outputs = cast(TransformStepOutputTransformType, self._outputs)
-            ds, df = self._transformer.transform(data_schema, dataframe, self._cache_group, force_recompute)
+            ds, df = self._transformer.transform(
+                data_schema, dataframe, self._cache_group, force_recompute, disable_cache
+            )
             data_container.data[self._outputs["data_schema"]] = ds
             data_container.data[self._outputs["dataframe"]] = df
         elif self._action == "fit_transform":
             self._outputs = cast(TransformStepOutputFitTransformType, self._outputs)
             ds, transformer, df = self._transformer.fit_transform(
-                data_schema, dataframe, self._cache_group, force_recompute
+                data_schema, dataframe, self._cache_group, force_recompute, disable_cache
             )
             data_container.data[self._outputs["data_schema"]] = ds
             data_container.data[self._outputs["transformer"]] = transformer
             data_container.data[self._outputs["dataframe"]] = df
         return data_container
 
     def _get_input_model(self) -> type[TransformStepInputType]:
```

### Comparing `mleko-3.2.0/mleko/pipeline/steps/tune_step.py` & `mleko-4.0.0/mleko/pipeline/steps/tune_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,29 +58,32 @@
             inputs: A dictionary of input keys following the `TuneStepInputType` schema.
             outputs: A dictionary of output keys following the `TuneStepOutputType` schema.
             cache_group: The cache group to use.
         """
         super().__init__(inputs, outputs, cache_group)
         self._tuner = tuner
 
-    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool, disable_cache: bool) -> DataContainer:
         """Perform hyperparameter tuning.
 
         Args:
             data_container: Contains the input.
             force_recompute: Whether to force the step to recompute its output, even if it already exists.
+            disable_cache: If set to True, disables the cache.
 
         Returns:
             A DataContainer containing the output of the tuning step. It contains the best hyperparameters, the best
             objective score, and an optional metadata object.
         """
         data_schema = self._validate_and_get_input(self._inputs["data_schema"], DataSchema, data_container)
         dataframe = self._validate_and_get_input(self._inputs["dataframe"], DataFrame, data_container)
 
-        hyperparameters, score, metadata = self._tuner.tune(data_schema, dataframe, self._cache_group, force_recompute)
+        hyperparameters, score, metadata = self._tuner.tune(
+            data_schema, dataframe, self._cache_group, force_recompute, disable_cache
+        )
         data_container.data[self._outputs["hyperparameters"]] = hyperparameters
         data_container.data[self._outputs["score"]] = score
         data_container.data[self._outputs["metadata"]] = metadata
         return data_container
 
     def _get_input_model(self) -> type[TuneStepInputType]:
         """Get the input model for the TuneStep.
```

### Comparing `mleko-3.2.0/mleko/utils/__init__.py` & `mleko-4.0.0/mleko/utils/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,23 +4,29 @@
 logger, decorators, and helper functions for working with `vaex` DataFrames and `tqdm` progress bars.
 """
 
 from __future__ import annotations
 
 from .custom_logger import CustomLogger
 from .decorators import auto_repr, timing
-from .file_helpers import clear_directory
+from .file_helpers import LocalFileEntry, LocalManifest, LocalManifestHandler, clear_directory
+from .s3_helpers import S3Client, S3FileManifest
 from .tqdm_helpers import set_tqdm_percent_wrapper
 from .vaex_helpers import get_column, get_columns, get_filtered_df, get_indices
 
 
 __all__ = [
     "CustomLogger",
     "auto_repr",
     "timing",
     "clear_directory",
+    "LocalFileEntry",
+    "LocalManifest",
+    "LocalManifestHandler",
     "set_tqdm_percent_wrapper",
     "get_column",
     "get_columns",
     "get_filtered_df",
     "get_indices",
+    "S3Client",
+    "S3FileManifest",
 ]
```

### Comparing `mleko-3.2.0/mleko/utils/custom_logger.py` & `mleko-4.0.0/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/utils/decorators.py` & `mleko-4.0.0/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/utils/tqdm_helpers.py` & `mleko-4.0.0/mleko/utils/tqdm_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/mleko/utils/vaex_helpers.py` & `mleko-4.0.0/mleko/utils/vaex_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-3.2.0/pyproject.toml` & `mleko-4.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "3.2.0"
+version = "4.0.0"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/klarna-incubator/mleko"
 repository = "https://github.com/klarna-incubator/mleko"
 documentation = "https://mleko.readthedocs.io"
```

### Comparing `mleko-3.2.0/PKG-INFO` & `mleko-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 3.2.0
+Version: 4.0.0
 Summary: ML-Ekosystem
 Home-page: https://github.com/klarna-incubator/mleko
 License: Apache-2.0
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.1,<3.11.dev0
 Classifier: Development Status :: 4 - Beta
@@ -48,16 +48,18 @@
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 ## Features
 
 `mleko` is engineered to address the end-to-end needs of machine learning pipelines, providing robust, scalable solutions for data science challenges:
 
 - Ingest: Seamlessly integrates with data sources like AWS S3 and Kaggle, offering hassle-free data ingestion and compatibility.
+- Export: Supports exporting data to various formats and platforms, locally or in the cloud, to ensure that your data is accessible and shareable.
 - Convert: Specializes in data format transformations, prominently featuring high-performance conversions from `CSV` to `Vaex DataFrame`, to make your data pipeline-ready.
 - Split: Employs sophisticated data partitioning algorithms, allowing you to segment DataFrames into train, test, and validation sets for effective model training and evaluation.
+  -Filter: Provides a suite of filtering techniques such as resampling or simple expression-based filtering, enabling you to focus on the most relevant data.
 - Feature Selection: Equipped with a suite of feature selection techniques, `mleko` enables model performance by focusing on the most impactful variables.
 - Transformation: Facilitates data manipulations such as Frequency Encoding and Standardization, ensuring that your data conforms to the prerequisites of the machine learning algorithms.
 - Model: Provides a core set of functionalities for machine learning models, including in-built support for hyperparameter tuning, thereby streamlining the path from data to deployable model.
 - Pipeline: Unifies the entire workflow into an intuitive directed acyclic graph (`DAG`) architecture, promoting reproducibility and reducing iteration time and time-to-market for machine learning models.
 
 By integrating these features, `mleko` serves as a comprehensive toolkit for machine learning practitioners looking to build robust models efficiently.
 
@@ -84,15 +86,15 @@
 
 ## Release History
 
 See our [changelog](https://github.com/klarna-incubator/mleko/tree/main/CHANGELOG.md).
 
 ## Acknowledgements
 
-The development of `mleko` was significantly influenced by existing work of the following individuals:
+The development of `mleko` was influenced by existing work of the following individuals:
 
 - **Felipe Breve Siola** ([fsiola](https://github.com/fsiola))
 - **Sai Ma** ([metanouvelle](https://github.com/metanouvelle))
 - **Ahmet Anil Pala** ([aanilpala](https://github.com/aanilpala))
 
 Their insights and contributions provided a solid foundation for this library. We appreciate their effort and recognize their contributions that led to the creation of `mleko`.
```

