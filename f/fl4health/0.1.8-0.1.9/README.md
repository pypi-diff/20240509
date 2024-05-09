# Comparing `tmp/fl4health-0.1.8.tar.gz` & `tmp/fl4health-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fl4health-0.1.8.tar", max compression
+gzip compressed data, was "fl4health-0.1.9.tar", max compression
```

## Comparing `fl4health-0.1.8.tar` & `fl4health-0.1.9.tar`

### file list

```diff
@@ -1,69 +1,68 @@
--rw-r--r--   0        0        0    11347 2023-11-29 18:32:08.878189 fl4health-0.1.8/LICENSE.md
--rw-r--r--   0        0        0    14144 2023-11-29 18:32:08.878189 fl4health-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/__init__.py
--rw-r--r--   0        0        0        0 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/checkpointing/__init__.py
--rw-r--r--   0        0        0     2727 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/checkpointing/checkpointer.py
--rw-r--r--   0        0        0        0 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/client_managers/__init__.py
--rw-r--r--   0        0        0     1653 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/client_managers/base_sampling_manager.py
--rw-r--r--   0        0        0     1375 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/client_managers/fixed_without_replacement_manager.py
--rw-r--r--   0        0        0     1740 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/client_managers/poisson_sampling_manager.py
--rw-r--r--   0        0        0        0 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/__init__.py
--rw-r--r--   0        0        0     4924 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/apfl_client.py
--rw-r--r--   0        0        0    18554 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/basic_client.py
--rw-r--r--   0        0        0     6135 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/clipping_client.py
--rw-r--r--   0        0        0     5790 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/dynamic_weight_exchange_client.py
--rw-r--r--   0        0        0    10870 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/evaluate_client.py
--rw-r--r--   0        0        0     6428 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/fed_prox_client.py
--rw-r--r--   0        0        0    12395 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/fenda_client.py
--rw-r--r--   0        0        0     2580 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/instance_level_privacy_client.py
--rw-r--r--   0        0        0     6111 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/moon_client.py
--rw-r--r--   0        0        0     4903 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/numpy_fl_client.py
--rw-r--r--   0        0        0    10490 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/scaffold_client.py
--rw-r--r--   0        0        0     5784 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/clients/tabular_data_client.py
--rw-r--r--   0        0        0      769 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/feature_alignment/constants.py
--rw-r--r--   0        0        0     1656 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/feature_alignment/string_columns_transformer.py
--rw-r--r--   0        0        0     5553 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/feature_alignment/tab_features_info_encoder.py
--rw-r--r--   0        0        0     7456 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/feature_alignment/tab_features_preprocessor.py
--rw-r--r--   0        0        0     2755 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/feature_alignment/tabular_feature.py
--rw-r--r--   0        0        0      679 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/feature_alignment/tabular_type.py
--rw-r--r--   0        0        0        0 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/model_bases/__init__.py
--rw-r--r--   0        0        0     3193 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/model_bases/apfl_base.py
--rw-r--r--   0        0        0     2095 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/model_bases/fedper_base.py
--rw-r--r--   0        0        0     2206 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/model_bases/fenda_base.py
--rw-r--r--   0        0        0     1272 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/model_bases/moon_base.py
--rw-r--r--   0        0        0      235 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/model_bases/partial_layer_exchange_model.py
--rw-r--r--   0        0        0        0 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/parameter_exchange/__init__.py
--rw-r--r--   0        0        0     1124 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/parameter_exchange/full_exchanger.py
--rw-r--r--   0        0        0     9723 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/parameter_exchange/layer_exchanger.py
--rw-r--r--   0        0        0      822 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/parameter_exchange/packing_exchanger.py
--rw-r--r--   0        0        0      540 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/parameter_exchange/parameter_exchanger_base.py
--rw-r--r--   0        0        0     3365 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/parameter_exchange/parameter_packer.py
--rw-r--r--   0        0        0        0 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/privacy/__init__.py
--rw-r--r--   0        0        0     8296 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/privacy/fl_accountants.py
--rw-r--r--   0        0        0    10562 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/privacy/moments_accountant.py
--rw-r--r--   0        0        0        0 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/reporting/__init__.py
--rw-r--r--   0        0        0     6751 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/reporting/fl_wanb.py
--rw-r--r--   0        0        0     9352 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/server/base_server.py
--rw-r--r--   0        0        0     5602 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/server/client_level_dp_fed_avg_server.py
--rw-r--r--   0        0        0    10614 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/server/evaluate_server.py
--rw-r--r--   0        0        0     6738 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/server/instance_level_dp_server.py
--rw-r--r--   0        0        0     4089 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/server/polling.py
--rw-r--r--   0        0        0    12022 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/server/scaffold_server.py
--rw-r--r--   0        0        0     8703 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/server/tabular_feature_alignment_server.py
--rw-r--r--   0        0        0        0 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/strategies/__init__.py
--rw-r--r--   0        0        0     2460 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/strategies/aggregate_utils.py
--rw-r--r--   0        0        0    15816 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/strategies/basic_fedavg.py
--rw-r--r--   0        0        0    22571 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/strategies/client_dp_fedavgm.py
--rw-r--r--   0        0        0    11864 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/strategies/fedavg_dynamic_layer.py
--rw-r--r--   0        0        0    12006 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/strategies/fedprox.py
--rw-r--r--   0        0        0     6423 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/strategies/noisy_aggregate.py
--rw-r--r--   0        0        0    17999 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/strategies/scaffold.py
--rw-r--r--   0        0        0      646 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/strategies/strategy_with_poll.py
--rw-r--r--   0        0        0     1154 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/utils/config.py
--rw-r--r--   0        0        0     1271 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/utils/dataset.py
--rw-r--r--   0        0        0     3209 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/utils/load_data.py
--rw-r--r--   0        0        0     4205 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/utils/losses.py
--rw-r--r--   0        0        0    12023 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/utils/metrics.py
--rw-r--r--   0        0        0     5399 2023-11-29 18:32:08.934189 fl4health-0.1.8/fl4health/utils/sampler.py
--rw-r--r--   0        0        0     1159 2023-11-29 18:32:08.938189 fl4health-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    14856 1970-01-01 00:00:00.000000 fl4health-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11347 2023-12-06 21:19:27.297936 fl4health-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0    14217 2023-12-06 21:19:27.297936 fl4health-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-12-06 21:19:27.353936 fl4health-0.1.9/fl4health/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-06 21:19:27.353936 fl4health-0.1.9/fl4health/checkpointing/__init__.py
+-rw-r--r--   0        0        0     2727 2023-12-06 21:19:27.353936 fl4health-0.1.9/fl4health/checkpointing/checkpointer.py
+-rw-r--r--   0        0        0        0 2023-12-06 21:19:27.353936 fl4health-0.1.9/fl4health/client_managers/__init__.py
+-rw-r--r--   0        0        0     1653 2023-12-06 21:19:27.353936 fl4health-0.1.9/fl4health/client_managers/base_sampling_manager.py
+-rw-r--r--   0        0        0     1375 2023-12-06 21:19:27.353936 fl4health-0.1.9/fl4health/client_managers/fixed_without_replacement_manager.py
+-rw-r--r--   0        0        0     1740 2023-12-06 21:19:27.353936 fl4health-0.1.9/fl4health/client_managers/poisson_sampling_manager.py
+-rw-r--r--   0        0        0        0 2023-12-06 21:19:27.353936 fl4health-0.1.9/fl4health/clients/__init__.py
+-rw-r--r--   0        0        0     4971 2023-12-06 21:19:27.353936 fl4health-0.1.9/fl4health/clients/apfl_client.py
+-rw-r--r--   0        0        0    31030 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/clients/basic_client.py
+-rw-r--r--   0        0        0     6194 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/clients/clipping_client.py
+-rw-r--r--   0        0        0     5859 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/clients/dynamic_weight_exchange_client.py
+-rw-r--r--   0        0        0    10636 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/clients/evaluate_client.py
+-rw-r--r--   0        0        0     6487 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/clients/fed_prox_client.py
+-rw-r--r--   0        0        0    12454 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/clients/fenda_client.py
+-rw-r--r--   0        0        0     2639 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/clients/instance_level_privacy_client.py
+-rw-r--r--   0        0        0     6170 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/clients/moon_client.py
+-rw-r--r--   0        0        0    10631 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/clients/scaffold_client.py
+-rw-r--r--   0        0        0     5841 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/clients/tabular_data_client.py
+-rw-r--r--   0        0        0      769 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/feature_alignment/constants.py
+-rw-r--r--   0        0        0     1656 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/feature_alignment/string_columns_transformer.py
+-rw-r--r--   0        0        0     5553 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/feature_alignment/tab_features_info_encoder.py
+-rw-r--r--   0        0        0     7456 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/feature_alignment/tab_features_preprocessor.py
+-rw-r--r--   0        0        0     2755 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/feature_alignment/tabular_feature.py
+-rw-r--r--   0        0        0      679 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/feature_alignment/tabular_type.py
+-rw-r--r--   0        0        0        0 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/model_bases/__init__.py
+-rw-r--r--   0        0        0     3193 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/model_bases/apfl_base.py
+-rw-r--r--   0        0        0     2095 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/model_bases/fedper_base.py
+-rw-r--r--   0        0        0     2206 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/model_bases/fenda_base.py
+-rw-r--r--   0        0        0     1272 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/model_bases/moon_base.py
+-rw-r--r--   0        0        0      235 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/model_bases/partial_layer_exchange_model.py
+-rw-r--r--   0        0        0        0 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/parameter_exchange/__init__.py
+-rw-r--r--   0        0        0     1124 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/parameter_exchange/full_exchanger.py
+-rw-r--r--   0        0        0     9723 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/parameter_exchange/layer_exchanger.py
+-rw-r--r--   0        0        0      822 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/parameter_exchange/packing_exchanger.py
+-rw-r--r--   0        0        0      540 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/parameter_exchange/parameter_exchanger_base.py
+-rw-r--r--   0        0        0     3365 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/parameter_exchange/parameter_packer.py
+-rw-r--r--   0        0        0        0 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/privacy/__init__.py
+-rw-r--r--   0        0        0     8296 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/privacy/fl_accountants.py
+-rw-r--r--   0        0        0    10562 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/privacy/moments_accountant.py
+-rw-r--r--   0        0        0        0 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/reporting/__init__.py
+-rw-r--r--   0        0        0     6751 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/reporting/fl_wanb.py
+-rw-r--r--   0        0        0    10048 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/server/base_server.py
+-rw-r--r--   0        0        0     5698 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/server/client_level_dp_fed_avg_server.py
+-rw-r--r--   0        0        0    11254 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/server/evaluate_server.py
+-rw-r--r--   0        0        0     6797 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/server/instance_level_dp_server.py
+-rw-r--r--   0        0        0     4089 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/server/polling.py
+-rw-r--r--   0        0        0    12163 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/server/scaffold_server.py
+-rw-r--r--   0        0        0     8750 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/server/tabular_feature_alignment_server.py
+-rw-r--r--   0        0        0        0 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/strategies/__init__.py
+-rw-r--r--   0        0        0     2460 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/strategies/aggregate_utils.py
+-rw-r--r--   0        0        0    15816 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/strategies/basic_fedavg.py
+-rw-r--r--   0        0        0    22571 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/strategies/client_dp_fedavgm.py
+-rw-r--r--   0        0        0    11864 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/strategies/fedavg_dynamic_layer.py
+-rw-r--r--   0        0        0    12006 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/strategies/fedprox.py
+-rw-r--r--   0        0        0     6423 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/strategies/noisy_aggregate.py
+-rw-r--r--   0        0        0    17999 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/strategies/scaffold.py
+-rw-r--r--   0        0        0      646 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/strategies/strategy_with_poll.py
+-rw-r--r--   0        0        0     1154 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/utils/config.py
+-rw-r--r--   0        0        0     1271 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/utils/dataset.py
+-rw-r--r--   0        0        0     3209 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/utils/load_data.py
+-rw-r--r--   0        0        0     4205 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/utils/losses.py
+-rw-r--r--   0        0        0    12023 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/utils/metrics.py
+-rw-r--r--   0        0        0     5399 2023-12-06 21:19:27.357936 fl4health-0.1.9/fl4health/utils/sampler.py
+-rw-r--r--   0        0        0     1159 2023-12-06 21:19:27.361936 fl4health-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    14929 1970-01-01 00:00:00.000000 fl4health-0.1.9/PKG-INFO
```

### Comparing `fl4health-0.1.8/LICENSE.md` & `fl4health-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/README.md` & `fl4health-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 We use the standard git development flow of branch and merge to main with PRs on GitHub. At least one member of the core team needs to approve a PR before it can be merged into main. As mentioned above, tests are run automatically on PRs with a merge target of main. Furthermore, a suite of static code checkers and formatters are also run on said PRs. These also need to pass for a PR to be eligible for merging into the main branch of the library. Currently, such checks run on python3.9.
 
 ### Development Requirements
 
 The library dependencies and those for development are listed in the `pyproject.toml` and `requirements.txt` files. You may use whatever virtual environment management tool that you would like. These include conda, poetry, and virtualenv. Poetry is used to produce our releases, which are managed and automated by GitHub.
 
-The easiest way to create and activate a virtual environment is
+The easiest way to create and activate a virtual environment is by using the [virtualenv](https://pypi.org/project/virtualenv/) package:
 ```bash
 virtualenv "ENV_PATH"
 source "ENV_PATH/bin/activate"
 pip install --upgrade pip
 pip install -r requirements.txt
 ```
```

### Comparing `fl4health-0.1.8/fl4health/checkpointing/checkpointer.py` & `fl4health-0.1.9/fl4health/checkpointing/checkpointer.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/client_managers/base_sampling_manager.py` & `fl4health-0.1.9/fl4health/client_managers/base_sampling_manager.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/client_managers/fixed_without_replacement_manager.py` & `fl4health-0.1.9/fl4health/client_managers/fixed_without_replacement_manager.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/client_managers/poisson_sampling_manager.py` & `fl4health-0.1.9/fl4health/client_managers/poisson_sampling_manager.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/clients/apfl_client.py` & `fl4health-0.1.9/fl4health/clients/apfl_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,17 @@
     def __init__(
         self,
         data_path: Path,
         metrics: Sequence[Metric],
         device: torch.device,
         loss_meter_type: LossMeterType = LossMeterType.AVERAGE,
         checkpointer: Optional[TorchCheckpointer] = None,
+        seed: Optional[int] = None,
     ) -> None:
-        super().__init__(data_path, metrics, device, loss_meter_type, checkpointer)
+        super().__init__(data_path, metrics, device, loss_meter_type, checkpointer, seed=seed)
 
         self.model: ApflModule
         self.learning_rate: float
         self.optimizer: torch.optim.Optimizer
         self.local_optimizer: torch.optim.Optimizer
 
     def is_start_of_local_training(self, step: int) -> bool:
```

### Comparing `fl4health-0.1.8/fl4health/clients/basic_client.py` & `fl4health-0.1.9/fl4health/clients/basic_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import copy
+import random
+import string
 from logging import INFO
 from pathlib import Path
-from typing import Any, Dict, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, Optional, Sequence, Tuple, Type, TypeVar, Union
 
+import numpy as np
 import torch
 import torch.nn as nn
+from flwr.client import NumPyClient
 from flwr.common.logger import log
 from flwr.common.typing import Config, NDArrays, Scalar
 from torch.nn.modules.loss import _Loss
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader
 
 from fl4health.checkpointing.checkpointer import TorchCheckpointer
-from fl4health.clients.numpy_fl_client import NumpyFlClient
 from fl4health.parameter_exchange.full_exchanger import FullParameterExchanger
 from fl4health.parameter_exchange.parameter_exchanger_base import ParameterExchanger
 from fl4health.reporting.fl_wanb import ClientWandBReporter
 from fl4health.utils.losses import Losses, LossMeter, LossMeterType
 from fl4health.utils.metrics import Metric, MetricManager
 
+T = TypeVar("T")
 
-class BasicClient(NumpyFlClient):
+
+class BasicClient(NumPyClient):
     def __init__(
         self,
         data_path: Path,
         metrics: Sequence[Metric],
         device: torch.device,
         loss_meter_type: LossMeterType = LossMeterType.AVERAGE,
         checkpointer: Optional[TorchCheckpointer] = None,
+        seed: Optional[int] = None,
     ) -> None:
         """
         Base FL Client with functionality to train, evaluate, log, report and checkpoint.
         User is responsible for implementing methods: get_model, get_optimizer, get_data_loaders, get_criterion
         Other methods can be overriden to achieve custom functionality.
 
         Args:
@@ -40,38 +46,177 @@
             device (torch.device): Device indicator for where to send the model, batches, labels etc. Often 'cpu' or
                 'cuda'
             loss_meter_type (LossMeterType, optional): Type of meter used to track and compute the losses over
                 each batch. Defaults to LossMeterType.AVERAGE.
             checkpointer (Optional[TorchCheckpointer], optional): Checkpointer to be used for client-side
                 checkpointing. Defaults to None.
         """
-        super().__init__(data_path, device)
+
+        self._maybe_fix_random_seeds(seed)
+
+        self.data_path = data_path
+        self.device = device
         self.metrics = metrics
         self.checkpointer = checkpointer
+
+        self.client_name = self.generate_hash()
+        self.initialized = False  # Whether or not the client has been setup
+        self.model_weights_initialized = False
+
+        # Loss and Metric management
         self.train_loss_meter = LossMeter.get_meter_by_type(loss_meter_type)
         self.val_loss_meter = LossMeter.get_meter_by_type(loss_meter_type)
-
         self.train_metric_manager = MetricManager(metrics=self.metrics, metric_manager_name="train")
         self.val_metric_manager = MetricManager(metrics=self.metrics, metric_manager_name="val")
 
+        # Optional variable to store the weights that the client was initialized with during each round of training
+        self.initial_weights: Optional[NDArrays] = None
+
+        self.wandb_reporter: Optional[ClientWandBReporter] = None
+        self.total_steps: int = 0  # Need to track total_steps across rounds for WANDB reporting
+
+        # Attributes to be initialized in setup_client
+        self.parameter_exchanger: ParameterExchanger
         self.model: nn.Module
         self.optimizer: torch.optim.Optimizer
-
         self.train_loader: DataLoader
         self.val_loader: DataLoader
         self.num_train_samples: int
         self.num_val_samples: int
         self.learning_rate: float
 
-        # Need to track total_steps across rounds for WANDB reporting
-        self.total_steps: int = 0
+    def _maybe_fix_random_seeds(self, seed: Optional[int] = None) -> None:
+        """
+        If seed value is provided, fix random seeds for reproducibility of results.
+
+        Args:
+            seed (int): The seed value to be used for random number generators.
+        """
+        if seed is None:
+            log(INFO, "No seed provided. Using random seed.")
+        else:
+            log(INFO, f"Setting seed to {seed}")
+            random.seed(seed)
+            np.random.seed(seed)
+            torch.manual_seed(seed)
+
+    def _maybe_checkpoint(self, current_metric_value: float) -> None:
+        """
+        If checkpointer exists, maybe checkpoint model based on the current comparison metric value.
+
+        Args:
+            current_metric_value (float): The metric value obtained by the current model.
+                Used to decide if to checkpoint model by checkpointer.
+        """
+        if self.checkpointer:
+            self.checkpointer.maybe_checkpoint(self.model, current_metric_value)
+
+    def generate_hash(self, length: int = 8) -> str:
+        """
+        Generates unique hash used as id for client.
+
+        Args:
+           length (int): The length of the hash.
+
+        Returns:
+            str: client id
+        """
+        return "".join(random.choice(string.ascii_lowercase) for i in range(length))
+
+    def get_parameters(self, config: Config) -> NDArrays:
+        """
+        Determines which parameters are sent back to the server for aggregation. This uses a parameter exchanger to
+        determine parameters sent.
+        Args:
+            config (Config): The config is sent by the FL server to allow for customization in the function if desired.
+
+        Returns:
+            NDArrays: These are the parameters to be sent to the server. At minimum they represent the relevant model
+                parameters to be aggregated, but can contain more information.
+        """
+
+        assert self.model is not None and self.parameter_exchanger is not None
+        return self.parameter_exchanger.push_parameters(self.model, config=config)
+
+    def set_parameters(self, parameters: NDArrays, config: Config) -> None:
+        """
+        Sets the local model parameters transfered from the server using a parameter exchanger to coordinate how
+        parameters are set. If it's the first time the model is being initialized, we assume the full model is being
+        initialized and use the FullParameterExchanger() to set all model weights.
+        Args:
+            parameters (NDArrays): Parameters have information about model state to be added to the relevant client
+                model but may contain more information than that.
+            config (Config): The config is sent by the FL server to allow for customization in the function if desired.
+        """
+        assert self.model is not None
+        if not self.model_weights_initialized:
+            self.initialize_all_model_weights(parameters, config)
+        else:
+            assert self.parameter_exchanger is not None
+            self.parameter_exchanger.pull_parameters(parameters, self.model, config)
+
+    def initialize_all_model_weights(self, parameters: NDArrays, config: Config) -> None:
+        """
+        If this is the first time we're initializing the model weights, we use the FullParameterExchanger to
+        initialize all model components
+
+        Args:
+            parameters (NDArrays): Model parameters to be injected into the client model
+            config (Config): The config is sent by the FL server to allow for customization in the function if desired.
+        """
+        FullParameterExchanger().pull_parameters(parameters, self.model, config)
+        self.model_weights_initialized = True
+
+    def narrow_config_type(self, config: Config, config_key: str, narrow_type_to: Type[T]) -> T:
+        """
+        Checks if a config_key exists in config and if so, verify it is of type narrow_type_to.
+
+        Args:
+            config (Config): The config object from the server.
+            config_key (str): The key to check config for.
+            narrow_type_to (Type[T]): The expected type of config[config_key]
+
+        Returns:
+            T: The type-checked value at config[config_key]
+
+        Raises:
+            ValueError: If config[config_key] is not of type narrow_type_to or
+                if the config_key is not present in config.
+        """
+        if config_key not in config:
+            raise ValueError(f"{config_key} is not present in the Config.")
+
+        config_value = config[config_key]
+        if isinstance(config_value, narrow_type_to):
+            return config_value
+        else:
+            raise ValueError(f"Provided configuration key ({config_key}) value does not have correct type")
+
+    def shutdown(self) -> None:
+        """
+        Shuts down the client. Involves shutting down W&B reporter if one exists.
+        """
+        if self.wandb_reporter:
+            self.wandb_reporter.shutdown_reporter()
 
     def process_config(self, config: Config) -> Tuple[Union[int, None], Union[int, None], int]:
         """
-        Method to ensure the required keys are present in config and extracts the values.
+        Method to ensure the required keys are present in config and extracts values to be returned.
+
+        Args:
+            config (Config): The config from the server.
+
+        Returns:
+            Tuple[Union[int, None], Union[int, None], int]: Returns the local_epochs, local_steps and
+                current_server_round. Ensures only one of local_epochs and local_steps is defined in the config
+                and sets the one that is not to None.
+
+        Raises:
+            ValueError: If the config contains both local_steps and local epochs or if local_steps, local_epochs or
+                current_server_round is of the wrong type (int).
         """
         current_server_round = self.narrow_config_type(config, "current_server_round", int)
 
         if ("local_epochs" in config) and ("local_steps" in config):
             raise ValueError("Config cannot contain both local_epochs and local_steps. Please specify only one.")
         elif "local_epochs" in config:
             local_epochs = self.narrow_config_type(config, "local_epochs", int)
@@ -82,14 +227,28 @@
         else:
             raise ValueError("Must specify either local_epochs or local_steps in the Config.")
 
         # Either local epochs or local steps is none based on what key is passed in the config
         return local_epochs, local_steps, current_server_round
 
     def fit(self, parameters: NDArrays, config: Config) -> Tuple[NDArrays, int, Dict[str, Scalar]]:
+        """
+        Processes config, initializes client (if first round) and performs training based on the passed config.
+
+        Args:
+            parameters (NDArrays): The parameters of the model to be used in fit.
+            config (NDArrays): The config from the server.
+
+        Returns:
+            Tuple[NDArrays, int, Dict[str, Scalar]]: The parameters following the local training along with the
+            number of samples in the local training dataset and the computed metrics throughout the fit.
+
+        Raises:
+            ValueError: If local_steps or local_epochs is not specified in config.
+        """
         local_epochs, local_steps, current_server_round = self.process_config(config)
 
         if not self.initialized:
             self.setup_client(config)
 
         self.set_parameters(parameters, config)
 
@@ -109,14 +268,25 @@
         return (
             self.get_parameters(config),
             self.num_train_samples,
             metrics,
         )
 
     def evaluate(self, parameters: NDArrays, config: Config) -> Tuple[float, int, Dict[str, Scalar]]:
+        """
+        Evaluates the model on the validation set.
+
+        Args:
+            parameters (NDArrays): The parameters of the model to be evaluated.
+            config (NDArrays): The config object from the server.
+
+        Returns:
+            Tuple[float, int, Dict[str, Scalar]]: A loss associated with the evaluation, the number of samples in the
+                validation set and the metric_values associated with evaluation.
+        """
         if not self.initialized:
             self.setup_client(config)
 
         self.set_parameters(parameters, config)
         loss, metric_values = self.validate()
         # EvaluateRes should return the loss, number of examples on client, and a dictionary holding metrics
         # calculation results.
@@ -130,14 +300,24 @@
         self,
         loss_dict: Dict[str, float],
         metrics_dict: Dict[str, Scalar],
         current_round: Optional[int] = None,
         current_epoch: Optional[int] = None,
         is_validation: bool = False,
     ) -> None:
+        """
+        Handles the logging of losses, metrics and other information to the output file.
+
+        Args:
+            loss_dict (Dict[str, float]): A dictionary of losses to log.
+            metrics_dict (Dict[str, Scalar]): A dictionary of the metric to log.
+            current_round (Optional[int]): The current FL round (ie current server round).
+            current_epoch (Optional[int]): The current epoch of local training.
+            is_validation (bool): Whether or not this logging is for validation set.
+        """
         initial_log_str = f"Current FL Round: {str(current_round)}\t" if current_round is not None else ""
         initial_log_str += f"Current Epoch: {str(current_epoch)}" if current_epoch is not None else ""
         if initial_log_str != "":
             log(INFO, initial_log_str)
 
         metric_string = "\t".join([f"{key}: {str(val)}" for key, val in metrics_dict.items()])
         loss_string = "\t".join([f"{key}: {str(val)}" for key, val in loss_dict.items()])
@@ -149,14 +329,22 @@
 
     def _handle_reporting(
         self,
         loss_dict: Dict[str, float],
         metric_dict: Dict[str, Scalar],
         current_round: Optional[int] = None,
     ) -> None:
+        """
+        Handles reporting of losses and metrics to W&B.
+
+        Args:
+            loss_dict (Dict[str, float]): A dictionary of losses to log.
+            metrics_dict (Dict[str, Scalar]): A dictionary of metrics to log.
+            current_round (Optional[int]): The current FL round.
+        """
         # If reporter is None we do not report to wandb and return
         if self.wandb_reporter is None:
             return
 
         # If no current_round is passed or current_round is None, set current_round to 0
         # This situation only arises when we do local finetuning and call train_by_epochs or train_by_steps explicitly
         current_round = current_round if current_round is not None else 0
@@ -165,16 +353,25 @@
         reporting_dict.update({"step": self.total_steps})
         reporting_dict.update(loss_dict)
         reporting_dict.update(metric_dict)
         self.wandb_reporter.report_metrics(reporting_dict)
 
     def train_step(self, input: torch.Tensor, target: torch.Tensor) -> Tuple[Losses, Dict[str, torch.Tensor]]:
         """
-        Given input and target, generate predictions, compute loss, optionally update metrics if they exist.
+        Given a single batch of input and target data, generate predictions, compute loss, update parameters and
+        optionally update metrics if they exist. (ie backprop on a single batch of data).
         Assumes self.model is in train model already.
+
+        Args:
+            input (torch.Tensor): The input to be fed into the model.
+            target (torch.Tensor): The target corresponding to the input.
+
+        Returns:
+            Tuple[Losses, Dict[str, torch.Tensor]]: The losses object from the train step along with
+                a dictionary of any predictions produced by the model.
         """
         # Clear gradients from optimizer if they exist
         self.optimizer.zero_grad()
 
         # Call user defined methods to get predictions and compute loss
         preds, features = self.predict(input)
         losses = self.compute_loss(preds, features, target)
@@ -183,28 +380,47 @@
         losses.backward.backward()
         self.optimizer.step()
 
         return losses, preds
 
     def val_step(self, input: torch.Tensor, target: torch.Tensor) -> Tuple[Losses, Dict[str, torch.Tensor]]:
         """
-        Given input and target, compute loss, update loss and metrics
+        Given input and target, compute loss, update loss and metrics.
         Assumes self.model is in eval mode already.
+
+        Args:
+            input (torch.Tensor): The input to be fed into the model.
+            target (torch.Tensor): The target corresponding to the input.
+
+        Returns:
+            Tuple[Losses, Dict[str, torch.Tensor]]: The losses object from the val step along with
+            a dictionary of the predictions produced by the model.
         """
 
         # Get preds and compute loss
         with torch.no_grad():
             preds, features = self.predict(input)
             losses = self.compute_loss(preds, features, target)
 
         return losses, preds
 
     def train_by_epochs(
         self, epochs: int, current_round: Optional[int] = None
     ) -> Tuple[Dict[str, float], Dict[str, Scalar]]:
+        """
+        Train locally for the specified number of epochs.
+
+        Args:
+            epochs (int): The number of epochs for local training.
+            current_round (Optional[int]): The current FL round.
+
+        Returns:
+            Tuple[Dict[str, float], Dict[str, Scalar]]: The loss and metrics dictionary from the local training.
+                Loss is a dictionary of one or more losses that represent the different components of the loss.
+        """
         self.model.train()
         local_step = 0
         for local_epoch in range(epochs):
             self.train_metric_manager.clear()
             self.train_loss_meter.clear()
             for input, target in self.train_loader:
                 input, target = input.to(self.device), target.to(self.device)
@@ -224,14 +440,24 @@
 
         # Return final training metrics
         return loss_dict, metrics
 
     def train_by_steps(
         self, steps: int, current_round: Optional[int] = None
     ) -> Tuple[Dict[str, float], Dict[str, Scalar]]:
+        """
+        Train locally for the specified number of steps.
+
+        Args:
+            steps (int): The number of steps to train locally.
+
+        Returns:
+            Tuple[Dict[str, float], Dict[str, Scalar]]: The loss and metrics dictionary from the local training.
+                Loss is a dictionary of one or more losses that represent the different components of the loss.
+        """
         self.model.train()
 
         # Pass loader to iterator so we can step through train loader
         train_iterator = iter(self.train_loader)
 
         self.train_loss_meter.clear()
         self.train_metric_manager.clear()
@@ -258,14 +484,20 @@
         # Log results and maybe report via WANDB
         self._handle_logging(loss_dict, metrics, current_round=current_round)
         self._handle_reporting(loss_dict, metrics, current_round=current_round)
 
         return loss_dict, metrics
 
     def validate(self) -> Tuple[float, Dict[str, Scalar]]:
+        """
+        Validate the current model on the entire validation dataset.
+
+        Returns:
+            Tuple[float, Dict[str, Scalar]]: The validation loss and a dictionary of metrics from validation.
+        """
         self.model.eval()
         self.val_metric_manager.clear()
         self.val_loss_meter.clear()
         with torch.no_grad():
             for input, target in self.val_loader:
                 input, target = input.to(self.device), target.to(self.device)
                 losses, preds = self.val_step(input, target)
@@ -281,23 +513,34 @@
         # Checkpoint based on loss which is output of user defined compute_loss method
         self._maybe_checkpoint(loss_dict["checkpoint"])
         return loss_dict["checkpoint"], metrics
 
     def get_properties(self, config: Config) -> Dict[str, Scalar]:
         """
         Return properties (train and validation dataset sample counts) of client.
+
+        Args:
+            config (Config): The config from the server.
+
+        Returns:
+            Dict[str, Scalar]: A dictionary with two entries corresponding to the sample counts in
+                the train and validation set.
         """
         if not self.initialized:
             self.setup_client(config)
 
         return {"num_train_samples": self.num_train_samples, "num_val_samples": self.num_val_samples}
 
     def setup_client(self, config: Config) -> None:
         """
         Set dataloaders, optimizers, parameter exchangers and other attributes derived from these.
+        Then set initialized attribute to True.
+
+        Args:
+            config (Config): The config from the server.
         """
         # Explicitly send the model to the desired device. This is idempotent.
         self.model = self.get_model(config).to(self.device)
         train_loader, val_loader = self.get_data_loaders(config)
         self.train_loader = train_loader
         self.val_loader = val_loader
 
@@ -310,19 +553,25 @@
         self.set_optimizer(config)
         self.learning_rate = self.optimizer.defaults["lr"]
         self.criterion = self.get_criterion(config).to(self.device)
         self.parameter_exchanger = self.get_parameter_exchanger(config)
 
         self.wandb_reporter = ClientWandBReporter.from_config(self.client_name, config)
 
-        super().setup_client(config)
+        self.initialized = True
 
     def get_parameter_exchanger(self, config: Config) -> ParameterExchanger:
         """
         Returns Full Parameter Exchangers. Subclasses that require custom Parameter Exchangers can override this.
+
+        Args:
+            config (Config): The config from server.
+
+        Returns:
+            ParameterExchanger: Used to exchange parameters between server and client.
         """
         return FullParameterExchanger()
 
     def predict(self, input: torch.Tensor) -> Tuple[Dict[str, torch.Tensor], Dict[str, torch.Tensor]]:
         """
         Computes the prediction(s), and potentially features, of the model(s) given the input.
 
@@ -330,14 +579,18 @@
             input (torch.Tensor): Inputs to be fed into the model.
 
         Returns:
             Tuple[Dict[str, torch.Tensor], Dict[str, torch.Tensor]]: A tuple in which the first element
             contains predictions indexed by name and the second element contains intermediate activations
             index by name. By passing features, we can compute losses such as the model contrasting loss in MOON.
             All predictions included in dictionary will be used to compute metrics.
+
+        Raises:
+            ValueError: Occurs when something other than a tensor or dict of tensors is returned by the model
+            forward.
         """
         preds = self.model(input)
 
         if isinstance(preds, dict):
             return preds, {}
         elif isinstance(preds, torch.Tensor):
             return {"prediction": preds}, {}
@@ -364,14 +617,17 @@
         return losses
 
     def set_optimizer(self, config: Config) -> None:
         """
         Method called in the the setup_client method to set optimizer attribute returned by used-defined get_optimizer.
         In the simplest case, get_optimizer returns an optimizer. For more advanced use cases where a dictionary of
         string and optimizer are returned (ie APFL), the use must override this method.
+
+        Args:
+            config (Config): The config from the server.
         """
         optimizer = self.get_optimizer(config)
         assert not isinstance(optimizer, dict)
         self.optimizer = optimizer
 
     def clone_and_freeze_model(self, model: nn.Module) -> nn.Module:
         """Clone and freeze model for use in various loss calculation.
@@ -386,46 +642,92 @@
         cloned_model = copy.deepcopy(model)
         for param in cloned_model.parameters():
             param.requires_grad = False
         cloned_model.eval()
 
         return cloned_model
 
-    def get_data_loaders(self, config: Config) -> Tuple[DataLoader, DataLoader]:
+    def get_data_loaders(self, config: Config) -> Tuple[DataLoader, ...]:
         """
         User defined method that returns a PyTorch Train DataLoader
         and a PyTorch Validation DataLoader
+
+        Args:
+            config (Config): The config from the server.
+
+        Returns:
+            Tuple[DataLoader, ...]: Tuple of length 2. The client train and validation loader.
+
+        Raises:
+            NotImplementedError: To be defined in child class.
         """
         raise NotImplementedError
 
     def get_criterion(self, config: Config) -> _Loss:
         """
         User defined method that returns PyTorch loss to train model.
+
+        Args:
+            config (Config): The config from the server.
+
+        Raises:
+            NotImplementedError: To be defined in child class.
         """
         raise NotImplementedError
 
     def get_optimizer(self, config: Config) -> Union[Optimizer, Dict[str, Optimizer]]:
         """
         Method to be defined by user that returns the PyTorch optimizer used to train models locally
         Return value can be a single torch optimizer or a dictionary of string and torch optimizer.
+        Returning multiple optimizers is useful in methods like APFL which has a different optimizer
+        for the local and global models.
+
+        Args:
+            config (Config): The config sent from the server.
+
+        Returns:
+            Union[Optimizer, Dict[str, Optimizer]]: An optimizer or dictionary of optimizers to
+            train model.
+
+        Raises:
+            NotImplementedError: To be defined in child class.
         """
         raise NotImplementedError
 
     def get_model(self, config: Config) -> nn.Module:
         """
-        User defined method that Returns PyTorch model
+        User defined method that returns PyTorch model.
+
+        Args:
+            config (Config): The config from the server.
+
+        Returns:
+            nn.Module: The client model.
+
+        Raises:
+            NotImplementedError: To be defined in child class.
         """
         raise NotImplementedError
 
     def update_after_train(self, local_steps: int, loss_dict: Dict[str, float]) -> None:
         """
-        Called after training with the number of local_steps performed over the FL round and
-        the corresponding loss dictionary.
+        Hook method called after training with the number of local_steps performed over the FL round and
+        the corresponding loss dictionary. For example, used by Scaffold to update the control variates
+        after a local round of training. Also used by FedProx to update the current loss based on the loss
+        returned during training.
+
+        Args:
+            local_steps (int): The number of steps in the local training.
+            loss_dict (Dict[str, float]): A dictionary of losses from local training.
         """
         pass
 
     def update_after_step(self, step: int) -> None:
         """
-        Called after local train step on client. step is an integer that represents
-        the local training step that was most recently completed.
+        Hook method called after local train step on client. step is an integer that represents
+        the local training step that was most recently completed. For example, used by the APFL
+        method to update the alpha value after a training a step.
+
+        Args:
+            step (int): The step number in local training that was most recently completed.
         """
         pass
```

### Comparing `fl4health-0.1.8/fl4health/clients/clipping_client.py` & `fl4health-0.1.9/fl4health/clients/clipping_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,23 @@
     def __init__(
         self,
         data_path: Path,
         metrics: Sequence[Metric],
         device: torch.device,
         loss_meter_type: LossMeterType = LossMeterType.AVERAGE,
         checkpointer: Optional[TorchCheckpointer] = None,
+        seed: Optional[int] = None,
     ) -> None:
         super().__init__(
             data_path=data_path,
             metrics=metrics,
             device=device,
             loss_meter_type=loss_meter_type,
             checkpointer=checkpointer,
+            seed=seed,
         )
         self.parameter_exchanger: ParameterExchangerWithPacking[float]
         self.clipping_bound: Optional[float] = None
         self.adaptive_clipping: Optional[bool] = None
 
     def calculate_parameters_norm(self, parameters: NDArrays) -> float:
         layer_inner_products = [pow(linalg.norm(layer_weights), 2) for layer_weights in parameters]
```

### Comparing `fl4health-0.1.8/fl4health/clients/dynamic_weight_exchange_client.py` & `fl4health-0.1.9/fl4health/clients/dynamic_weight_exchange_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 from pathlib import Path
-from typing import Sequence
+from typing import Optional, Sequence
 
 import torch
 import torch.nn as nn
 from flwr.common.typing import Config, NDArrays
 
 from fl4health.clients.basic_client import BasicClient
 from fl4health.parameter_exchange.layer_exchanger import NormDriftParameterExchanger
@@ -16,14 +16,15 @@
 class DynamicWeightExchangeClient(BasicClient):
     def __init__(
         self,
         data_path: Path,
         metrics: Sequence[Metric],
         device: torch.device,
         loss_meter_type: LossMeterType = LossMeterType.AVERAGE,
+        seed: Optional[int] = None,
     ) -> None:
         """
         Dynamic weight exchange client used to exchange a dynamic subset of layers per client.
 
         Args:
             data_path (Path): path to the data to be used to load the data for client-side training
             metrics (Sequence[Metric]): Metrics to be computed based on the labels and predictions of the client model
@@ -35,14 +36,15 @@
                 checkpointing. Defaults to None.
         """
         super().__init__(
             data_path=data_path,
             metrics=metrics,
             device=device,
             loss_meter_type=loss_meter_type,
+            seed=seed,
         )
         # Initial model parameters to be used in calculating weight shifts during training
         self.initial_model: nn.Module
         # Parameter exchanger to be used in server-client exchange of dynamic layers.
         self.parameter_exchanger: NormDriftParameterExchanger
 
     def setup_client(self, config: Config) -> None:
```

### Comparing `fl4health-0.1.8/fl4health/clients/evaluate_client.py` & `fl4health-0.1.9/fl4health/clients/evaluate_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,72 +5,87 @@
 import torch
 import torch.nn as nn
 from flwr.common.logger import log
 from flwr.common.typing import Config, NDArrays, Scalar
 from torch.nn.modules.loss import _Loss
 from torch.utils.data import DataLoader
 
-from fl4health.clients.numpy_fl_client import NumpyFlClient
+from fl4health.clients.basic_client import BasicClient
 from fl4health.parameter_exchange.full_exchanger import FullParameterExchanger
 from fl4health.parameter_exchange.parameter_exchanger_base import ParameterExchanger
 from fl4health.utils.losses import Losses, LossMeter, LossMeterType
 from fl4health.utils.metrics import Metric, MetricManager
 
 
-class EvaluateClient(NumpyFlClient):
+class EvaluateClient(BasicClient):
     """
     This client implements an evaluation only flow. That is, there is no expectation of parameter exchange with the
     server past the model initialization stage. The implementing client should instantiate a global model if one is
     expected from the server, which will be loaded using the passed parameters. If a model checkpoint path is provided
     the client attempts to load a local model from the specified path.
     """
 
     def __init__(
         self,
         data_path: Path,
         metrics: Sequence[Metric],
         device: torch.device,
         loss_meter_type: LossMeterType = LossMeterType.AVERAGE,
         model_checkpoint_path: Optional[Path] = None,
+        seed: Optional[int] = None,
     ) -> None:
-        super().__init__(data_path=data_path, device=device)
+
+        self._maybe_fix_random_seeds(seed)
+
+        # EvaluateClient does not call BasicClient constructor and sets attributes
+        # in a custom way to account for the fact it does not involve any training
+        self.client_name = self.generate_hash()
+        self.data_path = data_path
+        self.device = device
         self.model_checkpoint_path = model_checkpoint_path
         self.metrics = metrics
-        self.local_model: Optional[nn.Module] = None
-        self.global_model: Optional[nn.Module] = None
+        self.initialized = False
+
         # This data loader should be instantiated as the one on which to run evaluation
-        self.data_loader: DataLoader
-        self.criterion: _Loss
         self.global_loss_meter = LossMeter.get_meter_by_type(loss_meter_type)
         self.global_metric_manager = MetricManager(self.metrics, "global_eval_manager")
         self.local_loss_meter = LossMeter.get_meter_by_type(loss_meter_type)
         self.local_metric_manager = MetricManager(self.metrics, "local_eval_manager")
 
+        # The attributes to be set in setup_client
+        # Models corresponding to client-side and server-side checkpoints,
+        # if they exist, to be evaluated on the clients dataset.
+        self.data_loader: DataLoader
+        self.criterion: _Loss
+        self.local_model: Optional[nn.Module] = None
+        self.global_model: Optional[nn.Module] = None
+
     def get_parameters(self, config: Dict[str, Scalar]) -> NDArrays:
         raise ValueError("Get Parameters is not impelmented for an Evaluation-Only Client")
 
     def fit(self, parameters: NDArrays, config: Config) -> Tuple[NDArrays, int, Dict[str, Scalar]]:
         raise ValueError("Fit is not implemented for an Evaluation-Only Client")
 
     def setup_client(self, config: Config) -> None:
         """
         Set dataloaders, parameter exchangers and other attributes for the client
         """
-        self.data_loader = self.get_data_loader(config)
+        (data_loader,) = self.get_data_loader(config)
+        self.data_loader = data_loader
         self.global_model = self.initialize_global_model(config)
         self.local_model = self.get_local_model(config)
 
         # The following lines are type ignored because torch datasets are not "Sized"
         # IE __len__ is considered optionally defined. In practice, it is almost always defined
         # and as such, we will make that assumption.
         self.num_samples = len(self.data_loader.dataset)  # type: ignore
 
         self.criterion = self.get_criterion(config)
         self.parameter_exchanger = self.get_parameter_exchanger(config)
-        super().setup_client(config)
+        self.initialized = True
 
     def set_parameters(self, parameters: NDArrays, config: Config) -> None:
         # Sets the global model parameters transfered from the server using a parameter exchanger to coordinate how
         # parameters are set
         if len(parameters) > 0:
             # If a non-empty set of parameters are passed, then they are inserted into a global model to be evaluated.
             # If none are provided or a global model is not instantiated, then we only evaluate a local model
@@ -94,15 +109,18 @@
         # calculation results.
         return (
             loss,
             self.num_samples,
             metric_values,
         )
 
-    def _handle_logging(self, losses: Losses, metrics_dict: Dict[str, Scalar], is_global: bool) -> None:
+    def _handle_logging(  # type: ignore
+        self, losses: Losses, metrics_dict: Dict[str, Scalar], is_global: bool
+    ) -> None:
+
         metric_string = "\t".join([f"{key}: {str(val)}" for key, val in metrics_dict.items()])
         loss_string = "\t".join([f"{key}: {str(val)}" for key, val in losses.as_dict().items()])
         eval_prefix = "Global Model" if is_global else "Local Model"
         log(
             INFO,
             f"Client Evaluation {eval_prefix} Losses: {loss_string} \n"
             f"Client Evaluation {eval_prefix} Metrics: {metric_string}",
@@ -114,18 +132,18 @@
         model.eval()
         metric_meter.clear()
         loss_meter.clear()
 
         with torch.no_grad():
             for inputs, targets in self.data_loader:
                 inputs, targets = inputs.to(self.device), targets.to(self.device)
-                preds = model(inputs)
-                losses = self.compute_loss(preds, targets)
+                preds = {"prediction": model(inputs)}
+                losses = self.compute_loss(preds, {}, targets)
 
-                metric_meter.update({"predictions": preds}, targets)
+                metric_meter.update(preds, targets)
                 loss_meter.update(losses)
 
         metrics = metric_meter.compute()
         losses = loss_meter.compute()
         self._handle_logging(losses, metrics, is_global)
         return losses, metrics
 
@@ -186,41 +204,20 @@
         """
         Parameter exchange is assumed to always be full for evaluation only clients. If there are partial weights
         exchanged during training, we assume that the checkpoint has been saved locally. However, this functionality
         may be overridden if a different exchanger is needed
         """
         return FullParameterExchanger()
 
-    def predict(self, input: torch.Tensor) -> torch.Tensor:
-        """
-        Return predictions when given input. User can override for more complex logic.
-        """
-        return self.model(input)
-
-    def compute_loss(self, preds: torch.Tensor, target: torch.Tensor) -> Losses:
-        """
-        Computes loss given preds and torch and the user defined criterion. Optionally includes dictionary of
-        loss components if you wish to train the total loss as well as sub losses if they exist.
-        """
-        loss = self.criterion(preds, target)
-        losses = Losses(checkpoint=loss, backward=loss)
-        return losses
-
-    def get_data_loader(self, config: Config) -> DataLoader:
+    def get_data_loader(self, config: Config) -> Tuple[DataLoader]:
         """
         User defined method that returns a PyTorch DataLoader for validation
         """
         raise NotImplementedError
 
-    def get_criterion(self, config: Config) -> _Loss:
-        """
-        User defined method that returns PyTorch loss to train model.
-        """
-        raise NotImplementedError
-
     def initialize_global_model(self, config: Config) -> Optional[nn.Module]:
         """
         User defined method that to initializes a global model to potentially be hydrated by parameters sent by the
         server, by default, no global model is assumed to exist unless specified by the user
         """
         return None
```

### Comparing `fl4health-0.1.8/fl4health/clients/fed_prox_client.py` & `fl4health-0.1.9/fl4health/clients/fed_prox_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,23 @@
     def __init__(
         self,
         data_path: Path,
         metrics: Sequence[Metric],
         device: torch.device,
         loss_meter_type: LossMeterType = LossMeterType.AVERAGE,
         checkpointer: Optional[TorchCheckpointer] = None,
+        seed: Optional[int] = None,
     ) -> None:
         super().__init__(
             data_path=data_path,
             metrics=metrics,
             device=device,
             loss_meter_type=loss_meter_type,
             checkpointer=checkpointer,
+            seed=seed,
         )
         self.initial_tensors: List[torch.Tensor]
         self.parameter_exchanger: ParameterExchangerWithPacking
         self.proximal_weight: float
         self.current_loss: float
 
     def get_proximal_loss(self) -> torch.Tensor:
```

### Comparing `fl4health-0.1.8/fl4health/clients/fenda_client.py` & `fl4health-0.1.9/fl4health/clients/fenda_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,23 @@
         device: torch.device,
         loss_meter_type: LossMeterType = LossMeterType.AVERAGE,
         checkpointer: Optional[TorchCheckpointer] = None,
         temperature: Optional[float] = 0.5,
         perfcl_loss_weights: Optional[Tuple[float, float]] = None,
         cos_sim_loss_weight: Optional[float] = None,
         contrastive_loss_weight: Optional[float] = None,
+        seed: Optional[int] = None,
     ) -> None:
         super().__init__(
             data_path=data_path,
             metrics=metrics,
             device=device,
             loss_meter_type=loss_meter_type,
             checkpointer=checkpointer,
+            seed=seed,
         )
         """This module is used to init fenda client with various auxiliary loss functions.
         These losses will be activated only when their weights are not 0.0.
         Args:
             data_path: Path to the data directory.
             metrics: List of metrics to be used for evaluation.
             device: Device to be used for training.
```

### Comparing `fl4health-0.1.8/fl4health/clients/instance_level_privacy_client.py` & `fl4health-0.1.9/fl4health/clients/instance_level_privacy_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,23 @@
     def __init__(
         self,
         data_path: Path,
         metrics: Sequence[Metric],
         device: torch.device,
         loss_meter_type: LossMeterType = LossMeterType.AVERAGE,
         checkpointer: Optional[TorchCheckpointer] = None,
+        seed: Optional[int] = None,
     ) -> None:
         super().__init__(
             data_path=data_path,
             metrics=metrics,
             device=device,
             loss_meter_type=loss_meter_type,
             checkpointer=checkpointer,
+            seed=seed,
         )
         self.clipping_bound: float
         self.noise_multiplier: float
 
     def setup_client(self, config: Config) -> None:
         # Ensure that clipping bound and noise multiplier is present in config
         # Set attributes to be used when setting DP training
```

### Comparing `fl4health-0.1.8/fl4health/clients/moon_client.py` & `fl4health-0.1.9/fl4health/clients/moon_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,21 +24,23 @@
         metrics: Sequence[Metric],
         device: torch.device,
         loss_meter_type: LossMeterType = LossMeterType.AVERAGE,
         checkpointer: Optional[TorchCheckpointer] = None,
         temperature: float = 0.5,
         contrastive_weight: float = 10,
         len_old_models_buffer: int = 1,
+        seed: Optional[int] = None,
     ) -> None:
         super().__init__(
             data_path=data_path,
             metrics=metrics,
             device=device,
             loss_meter_type=loss_meter_type,
             checkpointer=checkpointer,
+            seed=seed,
         )
         self.cos_sim = torch.nn.CosineSimilarity(dim=-1).to(self.device)
         self.ce_criterion = torch.nn.CrossEntropyLoss().to(self.device)
         self.contrastive_weight = contrastive_weight
         self.temperature = temperature
 
         # Saving previous local models and global model at each communication round to compute contrastive loss
```

### Comparing `fl4health-0.1.8/fl4health/clients/scaffold_client.py` & `fl4health-0.1.9/fl4health/clients/scaffold_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,23 @@
     def __init__(
         self,
         data_path: Path,
         metrics: Sequence[Metric],
         device: torch.device,
         loss_meter_type: LossMeterType = LossMeterType.AVERAGE,
         checkpointer: Optional[TorchCheckpointer] = None,
+        seed: Optional[int] = None,
     ) -> None:
         super().__init__(
             data_path=data_path,
             metrics=metrics,
             device=device,
             loss_meter_type=loss_meter_type,
             checkpointer=checkpointer,
+            seed=seed,
         )
         self.learning_rate: float  # eta_l in paper
         self.client_control_variates: Optional[NDArrays] = None  # c_i in paper
         self.client_control_variates_updates: Optional[NDArrays] = None  # delta_c_i in paper
         self.server_control_variates: Optional[NDArrays] = None  # c in paper
         self.optimizer: torch.optim.SGD  # Scaffold require vanilla SGD as optimizer
         self.server_model_weights: Optional[NDArrays] = None  # x in paper
@@ -216,25 +218,28 @@
     def __init__(
         self,
         data_path: Path,
         metrics: Sequence[Metric],
         device: torch.device,
         loss_meter_type: LossMeterType = LossMeterType.AVERAGE,
         checkpointer: Optional[TorchCheckpointer] = None,
+        seed: Optional[int] = None,
     ) -> None:
         ScaffoldClient.__init__(
             self,
             data_path=data_path,
             metrics=metrics,
             device=device,
             loss_meter_type=loss_meter_type,
             checkpointer=checkpointer,
+            seed=seed,
         )
 
         InstanceLevelPrivacyClient.__init__(
             self,
             data_path=data_path,
             metrics=metrics,
             device=device,
             loss_meter_type=loss_meter_type,
             checkpointer=checkpointer,
+            seed=seed,
         )
```

### Comparing `fl4health-0.1.8/fl4health/clients/tabular_data_client.py` & `fl4health-0.1.9/fl4health/clients/tabular_data_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from logging import INFO
 from pathlib import Path
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Optional, Sequence, Union
 
 import pandas as pd
 import torch
 from flwr.common.logger import log
 from flwr.common.typing import Config, NDArray, Scalar
 from sklearn.pipeline import Pipeline
 
 from fl4health.clients.basic_client import BasicClient
-from fl4health.feature_alignment.constants import FEATURE_INFO, FORMAT_SPECIFIED, INPUT_DIMENSION, OUTPUT_DIMENSION
+from fl4health.feature_alignment.constants import FEATURE_INFO, INPUT_DIMENSION, OUTPUT_DIMENSION, SOURCE_SPECIFIED
 from fl4health.feature_alignment.tab_features_info_encoder import TabularFeaturesInfoEncoder
 from fl4health.feature_alignment.tab_features_preprocessor import TabularFeaturesPreprocessor
 from fl4health.utils.metrics import Metric
 
 
 class TabularDataClient(BasicClient):
     def __init__(
         self,
         data_path: Path,
         metrics: Sequence[Metric],
         device: torch.device,
         id_column: str,
         targets: Union[str, List[str]],
+        seed: Optional[int] = None,
     ) -> None:
-        super().__init__(data_path, metrics, device)
+        super().__init__(data_path, metrics, device, seed=seed)
         self.tabular_features_info_encoder: TabularFeaturesInfoEncoder
         self.tabular_features_preprocessor: TabularFeaturesPreprocessor
         self.df: pd.DataFrame
         self.input_dimension: int
         self.output_dimension: int
         self.id_column = id_column
         self.targets = targets
@@ -38,25 +39,25 @@
         self.feature_specific_pipelines: Dict[str, Pipeline] = {}
 
     def setup_client(self, config: Config) -> None:
         """
         Initialize the client by encoding the information of its tabular data
         and initializing the corresponding TabularFeaturesPreprocessor.
 
-        config[FORMAT_SPECIFIED] indicates whether the server has obtained
+        config[SOURCE_SPECIFIED] indicates whether the server has obtained
         the source of information to perform feature alignment.
         If it is True, it means the server has obtained such information
         (either a priori or by polling a client).
         So the client will encode that information and use it instead
         to perform feature preprocessing.
         """
-        format_specified = self.narrow_config_type(config, FORMAT_SPECIFIED, bool)
+        source_specified = self.narrow_config_type(config, SOURCE_SPECIFIED, bool)
         self.df = self.get_data_frame(config)
 
-        if format_specified:
+        if source_specified:
             # Since the server has obtained its source of information,
             # the client will encode that instead.
             self.tabular_features_info_encoder = TabularFeaturesInfoEncoder.from_json(
                 self.narrow_config_type(config, FEATURE_INFO, str)
             )
             self.tabular_features_preprocessor = TabularFeaturesPreprocessor(self.tabular_features_info_encoder)
 
@@ -69,15 +70,15 @@
             )
 
             # Obtain the input and output dimensions to be sent to
             # the server for global model initialization. Assuming
             # that the first dimension is the number of rows.
             self.input_dimension = self.aligned_features.shape[1]
             self.output_dimension = self.tabular_features_info_encoder.get_target_dimension()
-            log(INFO, f"input dimension: {self.input_dimension}, output_dimension: {self.output_dimension}")
+            log(INFO, f"input dimension: {self.input_dimension}, target dimension: {self.output_dimension}")
 
             super().setup_client(config)
 
             # freeing the memory of aligned features/targets and data.
             del self.aligned_features
             del self.aligned_targets
             del self.df
@@ -106,16 +107,16 @@
         dimensions so the server can use them to initialize the global model.
 
         First initializes the client because this is called prior to the first
         federated learning round.
         """
         if not self.initialized:
             self.setup_client(config)
-        format_specified = self.narrow_config_type(config, FORMAT_SPECIFIED, bool)
-        if not format_specified:
+        source_specified = self.narrow_config_type(config, SOURCE_SPECIFIED, bool)
+        if not source_specified:
             return {
                 FEATURE_INFO: self.tabular_features_info_encoder.to_json(),
             }
         else:
             return {
                 INPUT_DIMENSION: self.input_dimension,
                 OUTPUT_DIMENSION: self.output_dimension,
```

### Comparing `fl4health-0.1.8/fl4health/feature_alignment/constants.py` & `fl4health-0.1.9/fl4health/feature_alignment/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 TextFeatureTransformer = Union[CountVectorizer, TfidfTransformer, TfidfVectorizer, HashingVectorizer]
 
 # constants used in config for communication between
 # the server and clients.
 
 # FORMAT_SPECIFIED indicates whether the server has the "source of truth"
 # to be used for feature alignment.
-FORMAT_SPECIFIED = "format_specified"
+SOURCE_SPECIFIED = "source_specified"
 
 # FEATURE_INFO refers to the encoded feature information (source of truth).
 FEATURE_INFO = "feature_info"
 
 # These are used to initialize a global model on the server's side.
 INPUT_DIMENSION = "input_dimension"
 OUTPUT_DIMENSION = "output_dimension"
```

### Comparing `fl4health-0.1.8/fl4health/feature_alignment/string_columns_transformer.py` & `fl4health-0.1.9/fl4health/feature_alignment/string_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/feature_alignment/tab_features_info_encoder.py` & `fl4health-0.1.9/fl4health/feature_alignment/tab_features_info_encoder.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/feature_alignment/tab_features_preprocessor.py` & `fl4health-0.1.9/fl4health/feature_alignment/tab_features_preprocessor.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/feature_alignment/tabular_feature.py` & `fl4health-0.1.9/fl4health/feature_alignment/tabular_feature.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/feature_alignment/tabular_type.py` & `fl4health-0.1.9/fl4health/feature_alignment/tabular_type.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/model_bases/apfl_base.py` & `fl4health-0.1.9/fl4health/model_bases/apfl_base.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/model_bases/fedper_base.py` & `fl4health-0.1.9/fl4health/model_bases/fedper_base.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/model_bases/fenda_base.py` & `fl4health-0.1.9/fl4health/model_bases/fenda_base.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/model_bases/moon_base.py` & `fl4health-0.1.9/fl4health/model_bases/moon_base.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/parameter_exchange/full_exchanger.py` & `fl4health-0.1.9/fl4health/parameter_exchange/full_exchanger.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/parameter_exchange/layer_exchanger.py` & `fl4health-0.1.9/fl4health/parameter_exchange/layer_exchanger.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/parameter_exchange/packing_exchanger.py` & `fl4health-0.1.9/fl4health/parameter_exchange/packing_exchanger.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/parameter_exchange/parameter_exchanger_base.py` & `fl4health-0.1.9/fl4health/parameter_exchange/parameter_exchanger_base.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/parameter_exchange/parameter_packer.py` & `fl4health-0.1.9/fl4health/parameter_exchange/parameter_packer.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/privacy/fl_accountants.py` & `fl4health-0.1.9/fl4health/privacy/fl_accountants.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/privacy/moments_accountant.py` & `fl4health-0.1.9/fl4health/privacy/moments_accountant.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/reporting/fl_wanb.py` & `fl4health-0.1.9/fl4health/reporting/fl_wanb.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/server/base_server.py` & `fl4health-0.1.9/fl4health/server/base_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import random
 from logging import INFO, WARNING
 from typing import Dict, Generic, List, Optional, Tuple, TypeVar
 
+import numpy as np
+import torch
 import torch.nn as nn
 from flwr.common.logger import log
 from flwr.common.parameter import parameters_to_ndarrays
 from flwr.common.typing import Scalar
 from flwr.server.client_manager import ClientManager
 from flwr.server.history import History
 from flwr.server.server import EvaluateResultsAndFailures, Server
@@ -20,14 +23,15 @@
 class FlServer(Server):
     def __init__(
         self,
         client_manager: ClientManager,
         strategy: Optional[Strategy] = None,
         wandb_reporter: Optional[ServerWandBReporter] = None,
         checkpointer: Optional[TorchCheckpointer] = None,
+        seed: Optional[int] = None,
     ) -> None:
         """
         Base Server for the library to facilitate strapping additional/useful machinery to the base flwr server.
 
         Args:
             client_manager (ClientManager): Determines the mechanism by which clients are sampled by the server, if
                 they are to be sampled at all.
@@ -37,18 +41,35 @@
             wandb_reporter (Optional[ServerWandBReporter], optional): To be provided if the server is to log
                 information and results to a Weights and Biases account. If None is provided, no logging occurs.
                 Defaults to None.
             checkpointer (Optional[TorchCheckpointer], optional): To be provided if the server should perform
                 server side checkpointing based on some criteria. If none, then no server-side checkpointing is
                 performed. Defaults to None.
         """
+        self._maybe_fix_random_seeds(seed)
+
         super().__init__(client_manager=client_manager, strategy=strategy)
         self.wandb_reporter = wandb_reporter
         self.checkpointer = checkpointer
 
+    def _maybe_fix_random_seeds(self, seed: Optional[int] = None) -> None:
+        """
+        If seed value is provided, fix random seeds for reproducibility of results.
+
+        Args:
+            seed (int): The seed value to be used for random number generators.
+        """
+        if seed is None:
+            log(INFO, "No seed provided. Using random seed.")
+        else:
+            log(INFO, f"Setting seed to {seed}")
+            random.seed(seed)
+            np.random.seed(seed)
+            torch.manual_seed(seed)
+
     def fit(self, num_rounds: int, timeout: Optional[float]) -> History:
         history = super().fit(num_rounds, timeout)
         if self.wandb_reporter:
             # report history to W and B
             self.wandb_reporter.report_metrics(num_rounds, history)
         return history
 
@@ -142,14 +163,15 @@
         self,
         client_manager: ClientManager,
         model: nn.Module,
         parameter_exchanger: ExchangerType,
         wandb_reporter: Optional[ServerWandBReporter] = None,
         strategy: Optional[Strategy] = None,
         checkpointer: Optional[TorchCheckpointer] = None,
+        seed: Optional[int] = None,
     ) -> None:
         """
         This is a standard FL server but equipped with the assumption that the parameter exchanger is capable of
         hydrating the provided server model fully such that it can be checkpointed. For custom checkpointing
         functionality, one need only override _hydrate_model_for_checkpointing.
 
         Args:
@@ -163,15 +185,15 @@
             wandb_reporter (Optional[ServerWandBReporter], optional): To be provided if the server is to log
                 information and results to a Weights and Biases account. If None is provided, no logging occurs.
                 Defaults to None.
             checkpointer (Optional[TorchCheckpointer], optional): To be provided if the server should perform
                 server side checkpointing based on some criteria. If none, then no server-side checkpointing is
                 performed. Defaults to None.
         """
-        super().__init__(client_manager, strategy, wandb_reporter, checkpointer)
+        super().__init__(client_manager, strategy, wandb_reporter, checkpointer, seed)
         self.server_model = model
         # To facilitate model rehydration from server-side state for checkpointing
         self.parameter_exchanger = parameter_exchanger
 
     def _hydrate_model_for_checkpointing(self) -> nn.Module:
         model_ndarrays = parameters_to_ndarrays(self.parameters)
         self.parameter_exchanger.pull_parameters(model_ndarrays, self.server_model)
```

### Comparing `fl4health-0.1.8/fl4health/server/client_level_dp_fed_avg_server.py` & `fl4health-0.1.9/fl4health/server/client_level_dp_fed_avg_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         client_manager: ClientManager,
         strategy: ClientLevelDPFedAvgM,
         server_noise_multiplier: float,
         num_server_rounds: int,
         wandb_reporter: Optional[ServerWandBReporter] = None,
         checkpointer: Optional[TorchCheckpointer] = None,
         delta: Optional[int] = None,
+        seed: Optional[int] = None,
     ) -> None:
         """
         Server to be used in case of Client Level Differential Privacy with Federated Averaging.
 
         Args:
             client_manager (ClientManager): Determines the mechanism by which clients are sampled by the server, if
                 they are to be sampled at all.
@@ -46,15 +47,19 @@
             checkpointer (Optional[TorchCheckpointer], optional): To be provided if the server should perform
                 server side checkpointing based on some criteria. If none, then no server-side checkpointing is
                 performed. Defaults to None.
             delta (Optional[float], optional): The delta value for epislon-delta DP accounting. If None it defaults to
                 being 1/total_samples in the FL run. Defaults to None.
         """
         super().__init__(
-            client_manager=client_manager, strategy=strategy, wandb_reporter=wandb_reporter, checkpointer=checkpointer
+            client_manager=client_manager,
+            strategy=strategy,
+            wandb_reporter=wandb_reporter,
+            checkpointer=checkpointer,
+            seed=seed,
         )
         self.accountant: ClientLevelAccountant
         self.server_noise_multiplier = server_noise_multiplier
         self.num_server_rounds = num_server_rounds
         self.delta = delta
 
     def fit(self, num_rounds: int, timeout: Optional[float]) -> History:
```

### Comparing `fl4health-0.1.8/fl4health/server/evaluate_server.py` & `fl4health-0.1.9/fl4health/server/evaluate_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import random
 import timeit
 from logging import INFO, WARNING
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
+import numpy as np
 import torch
 from flwr.common import EvaluateIns, EvaluateRes, MetricsAggregationFn, Parameters, Scalar
 from flwr.common.logger import log
 from flwr.common.parameter import ndarrays_to_parameters
 from flwr.server.client_manager import ClientManager
 from flwr.server.client_proxy import ClientProxy
 from flwr.server.history import History
@@ -21,14 +23,15 @@
         client_manager: ClientManager,
         fraction_evaluate: float,
         model_checkpoint_path: Optional[Path] = None,
         evaluate_config: Optional[Dict[str, Scalar]] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         accept_failures: bool = True,
         min_available_clients: int = 1,
+        seed: Optional[int] = None,
     ) -> None:
         """
         Args:
             client_manager (ClientManager): Determines the mechanism by which clients are sampled by the server, if
                 they are to be sampled at all.
             fraction_evaluate (float): Fraction of clients used during evaluation.
             model_checkpoint_path (Optional[Path], optional): Server side model checkpoint path to load global model
@@ -37,14 +40,15 @@
                 on clients. Defaults to None.
             evaluate_metrics_aggregation_fn (Optional[MetricsAggregationFn], optional):  Metrics aggregation function.
                  Defaults to None.
             accept_failures (bool, optional): Whether or not accept rounds containing failures. Defaults to True.
             min_available_clients (int, optional): Minimum number of total clients in the system. Defaults to 1.
                 Defaults to 1.
         """
+        self._maybe_fix_random_seeds(seed)
         # We aren't aggregating model weights, so setting the strategy to be none.
         super().__init__(client_manager=client_manager, strategy=None)
         self.model_checkpoint_path = model_checkpoint_path
         # Load model parameters if checkpoint provided, otherwise leave as empty params
         if model_checkpoint_path:
             self.parameters = self.load_model_checkpoint_to_parameters()
         self.fraction_evaluate = fraction_evaluate
@@ -55,14 +59,29 @@
         if self.fraction_evaluate < 1.0:
             log(
                 INFO,
                 f"Fraction Evaluate is {self.fraction_evaluate}. "
                 "Thus, some clients may not participate in evaluation",
             )
 
+    def _maybe_fix_random_seeds(self, seed: Optional[int] = None) -> None:
+        """
+        If seed value is provided, fix random seeds for reproducibility of results.
+
+        Args:
+            seed (int): The seed value to be used for random number generators.
+        """
+        if seed is None:
+            log(INFO, "No seed provided. Using random seed.")
+        else:
+            log(INFO, f"Setting seed to {seed}")
+            random.seed(seed)
+            np.random.seed(seed)
+            torch.manual_seed(seed)
+
     def load_model_checkpoint_to_parameters(self) -> Parameters:
         assert self.model_checkpoint_path
         log(INFO, f"Loading model checkpoint at: {self.model_checkpoint_path.__str__()}")
         model = torch.load(self.model_checkpoint_path)
         # Extracting all parameters from the model to be sent to the clients
         parameters = ndarrays_to_parameters([val.cpu().numpy() for _, val in model.state_dict().items()])
         log(INFO, "Model loaded and state converted to parameters")
```

### Comparing `fl4health-0.1.8/fl4health/server/instance_level_dp_server.py` & `fl4health-0.1.9/fl4health/server/instance_level_dp_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         num_server_rounds: int,
         strategy: BasicFedAvg,
         local_epochs: Optional[int] = None,
         local_steps: Optional[int] = None,
         wandb_reporter: Optional[ServerWandBReporter] = None,
         checkpointer: Optional[TorchCheckpointer] = None,
         delta: Optional[float] = None,
+        seed: Optional[int] = None,
     ) -> None:
         """
         Server to be used in case of Instance Level Differential Privacy with Federated Averaging.
         Modified the fit function to poll clients for sample counts prior to the first round of FL.
 
         Args:
             client_manager (ClientManager): Determines the mechanism by which clients are sampled by the server, if
@@ -58,14 +59,15 @@
                 being 1/total_samples in the FL run. Defaults to None.
         """
         super().__init__(
             client_manager=client_manager,
             strategy=strategy,
             wandb_reporter=wandb_reporter,
             checkpointer=checkpointer,
+            seed=seed,
         )
 
         # Ensure that one of local_epochs and local_steps is passed (and not both)
         assert isinstance(local_epochs, int) ^ isinstance(local_steps, int)
         self.accountant: FlInstanceLevelAccountant
         self.local_steps = local_steps
         self.local_epochs = local_epochs
```

### Comparing `fl4health-0.1.8/fl4health/server/polling.py` & `fl4health-0.1.9/fl4health/server/polling.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/server/scaffold_server.py` & `fl4health-0.1.9/fl4health/server/scaffold_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     def __init__(
         self,
         client_manager: ClientManager,
         strategy: Scaffold,
         wandb_reporter: Optional[ServerWandBReporter] = None,
         checkpointer: Optional[TorchCheckpointer] = None,
         warm_start: bool = False,  # Whether or not to initialize control variates of each client as local gradient
+        seed: Optional[int] = None,
     ) -> None:
         """
         Custom FL Server for scaffold algorithm to handle warm initialization of control variates
         as specified in https://arxiv.org/abs/1910.06378.
 
         Args:
             client_manager (ClientManager): Determines the mechanism by which clients are sampled by the server, if
@@ -46,14 +47,15 @@
         """
         FlServer.__init__(
             self,
             client_manager=client_manager,
             strategy=strategy,
             wandb_reporter=wandb_reporter,
             checkpointer=checkpointer,
+            seed=seed,
         )
         self.warm_start = warm_start
 
     def _get_initial_parameters(self, timeout: Optional[float]) -> Parameters:
         """
         Overrides the _get_initial_parameters in the flwr server base class to strap on the possibility of a
         warm_start for SCAFFOLD. Initializes parameters (models weights and control variates) of the server.
@@ -143,14 +145,15 @@
         strategy: Scaffold,
         local_epochs: Optional[int] = None,
         local_steps: Optional[int] = None,
         delta: Optional[float] = None,
         wandb_reporter: Optional[ServerWandBReporter] = None,
         checkpointer: Optional[TorchCheckpointer] = None,
         warm_start: bool = False,
+        seed: Optional[int] = None,
     ) -> None:
         """
         Custom FL Server for Instance Level Differentially Private Scaffold algorithm as specified in
         https://arxiv.org/abs/2111.09278
 
         Args:
             client_manager (ClientManager): Determines the mechanism by which clients are sampled by the server, if
@@ -184,25 +187,27 @@
         ScaffoldServer.__init__(
             self,
             client_manager=client_manager,
             strategy=strategy,
             wandb_reporter=wandb_reporter,
             checkpointer=checkpointer,
             warm_start=warm_start,
+            seed=seed,
         )
         InstanceLevelDPServer.__init__(
             self,
             client_manager=client_manager,
             strategy=strategy,
             noise_multiplier=noise_multiplier,
             local_epochs=local_epochs,
             local_steps=local_steps,
             batch_size=batch_size,
             delta=delta,
             num_server_rounds=num_server_rounds,
+            seed=seed,
         )
 
     def fit(self, num_rounds: int, timeout: Optional[float]) -> History:
         """
         Run DP Scaffold algorithm for the specified number of rounds.
 
         Args:
```

### Comparing `fl4health-0.1.8/fl4health/server/tabular_feature_alignment_server.py` & `fl4health-0.1.9/fl4health/server/tabular_feature_alignment_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from flwr.server.client_manager import ClientManager
 from flwr.server.history import History
 
 from fl4health.checkpointing.checkpointer import TorchCheckpointer
 from fl4health.feature_alignment.constants import (
     CURRENT_SERVER_ROUND,
     FEATURE_INFO,
-    FORMAT_SPECIFIED,
     INPUT_DIMENSION,
     OUTPUT_DIMENSION,
+    SOURCE_SPECIFIED,
 )
 from fl4health.feature_alignment.tab_features_info_encoder import TabularFeaturesInfoEncoder
 from fl4health.reporting.fl_wanb import ServerWandBReporter
 from fl4health.server.base_server import FlServer
 from fl4health.server.polling import poll_clients
 from fl4health.strategies.basic_fedavg import BasicFedAvg
 
@@ -51,33 +51,34 @@
         client_manager: ClientManager,
         config: Config,
         initialize_parameters: Callable[..., Parameters],
         strategy: BasicFedAvg,
         wandb_reporter: Optional[ServerWandBReporter] = None,
         checkpointer: Optional[TorchCheckpointer] = None,
         tabular_features_source_of_truth: Optional[TabularFeaturesInfoEncoder] = None,
+        seed: Optional[int] = None,
     ) -> None:
         if strategy.on_fit_config_fn is not None:
             log(WARNING, "strategy.on_fit_config_fn will be overwritten.")
         if strategy.initial_parameters is not None:
             log(WARNING, "strategy.initial_parameters will be overwritten.")
 
-        super().__init__(client_manager, strategy, wandb_reporter, checkpointer)
+        super().__init__(client_manager, strategy, wandb_reporter, checkpointer, seed=seed)
         # The server performs one or two rounds of polls before the normal federated training.
         # The first one gathers feature information if the server does not already have it,
         # and the second one gathers the input/output dimensions of the model.
         self.initial_polls_complete = False
         self.tab_features_info = tabular_features_source_of_truth
         self.config = config
         self.initialize_parameters = initialize_parameters
-        self.format_info_gathered = False
+        self.source_info_gathered = False
         self.dimension_info: Dict[str, int] = {}
         # ensure that self.strategy has type BasicFedAvg so its on_fit_config_fn can be specified.
         assert isinstance(self.strategy, BasicFedAvg)
-        self.strategy.on_fit_config_fn = partial(fit_config, self.config, self.format_info_gathered)
+        self.strategy.on_fit_config_fn = partial(fit_config, self.config, self.source_info_gathered)
 
     def _set_dimension_info(self, input_dimension: int, output_dimension: int) -> None:
         self.dimension_info[INPUT_DIMENSION] = input_dimension
         self.dimension_info[OUTPUT_DIMENSION] = output_dimension
 
     def _get_initial_parameters(self, timeout: Optional[float]) -> Parameters:
         assert INPUT_DIMENSION in self.dimension_info and OUTPUT_DIMENSION in self.dimension_info
@@ -105,17 +106,17 @@
                     INFO,
                     "Features information source already specified. Sending to clients to perform feature alignment.",
                 )
                 feature_info_source = self.tab_features_info.to_json()
 
             # the feature information is sent to clients through the config parameter.
             self.config[FEATURE_INFO] = feature_info_source
-            self.format_info_gathered = True
+            self.source_info_gathered = True
 
-            self.strategy.on_fit_config_fn = partial(fit_config, self.config, self.format_info_gathered)
+            self.strategy.on_fit_config_fn = partial(fit_config, self.config, self.source_info_gathered)
 
             # Now the server waits until feature alignment is performed on the clients' side
             # and subsequently requests the input and output dimensions, which are needed for initializing
             # the global model.
             input_dimension, output_dimension = self.poll_clients_for_dimension_info(timeout)
             log(DEBUG, f"input dimension: {input_dimension}, output dimension: {output_dimension}")
             self._set_dimension_info(input_dimension, output_dimension)
@@ -153,11 +154,11 @@
         assert len(results) == 1
         input_dimension = int(results[0][1].properties[INPUT_DIMENSION])
         output_dimension = int(results[0][1].properties[OUTPUT_DIMENSION])
 
         return input_dimension, output_dimension
 
 
-def fit_config(config: Config, format_specified: bool, current_server_round: int) -> Config:
-    config[FORMAT_SPECIFIED] = format_specified
+def fit_config(config: Config, source_specified: bool, current_server_round: int) -> Config:
+    config[SOURCE_SPECIFIED] = source_specified
     config[CURRENT_SERVER_ROUND] = current_server_round
     return config
```

### Comparing `fl4health-0.1.8/fl4health/strategies/aggregate_utils.py` & `fl4health-0.1.9/fl4health/strategies/aggregate_utils.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/strategies/basic_fedavg.py` & `fl4health-0.1.9/fl4health/strategies/basic_fedavg.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/strategies/client_dp_fedavgm.py` & `fl4health-0.1.9/fl4health/strategies/client_dp_fedavgm.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/strategies/fedavg_dynamic_layer.py` & `fl4health-0.1.9/fl4health/strategies/fedavg_dynamic_layer.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/strategies/fedprox.py` & `fl4health-0.1.9/fl4health/strategies/fedprox.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/strategies/noisy_aggregate.py` & `fl4health-0.1.9/fl4health/strategies/noisy_aggregate.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/strategies/scaffold.py` & `fl4health-0.1.9/fl4health/strategies/scaffold.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/strategies/strategy_with_poll.py` & `fl4health-0.1.9/fl4health/strategies/strategy_with_poll.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/utils/config.py` & `fl4health-0.1.9/fl4health/utils/config.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/utils/dataset.py` & `fl4health-0.1.9/fl4health/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/utils/load_data.py` & `fl4health-0.1.9/fl4health/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/utils/losses.py` & `fl4health-0.1.9/fl4health/utils/losses.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/utils/metrics.py` & `fl4health-0.1.9/fl4health/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/fl4health/utils/sampler.py` & `fl4health-0.1.9/fl4health/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.8/pyproject.toml` & `fl4health-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fl4health"
-version = "0.1.8"
+version = "0.1.9"
 description = "Federated Learning for Health"
 authors = ["Vector AI Engineering <fl4health@vectorinstitute.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `fl4health-0.1.8/PKG-INFO` & `fl4health-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fl4health
-Version: 0.1.8
+Version: 0.1.9
 Summary: Federated Learning for Health
 License: Apache-2.0
 Author: Vector AI Engineering
 Author-email: fl4health@vectorinstitute.ai
 Requires-Python: >=3.9.0,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -164,15 +164,15 @@
 
 We use the standard git development flow of branch and merge to main with PRs on GitHub. At least one member of the core team needs to approve a PR before it can be merged into main. As mentioned above, tests are run automatically on PRs with a merge target of main. Furthermore, a suite of static code checkers and formatters are also run on said PRs. These also need to pass for a PR to be eligible for merging into the main branch of the library. Currently, such checks run on python3.9.
 
 ### Development Requirements
 
 The library dependencies and those for development are listed in the `pyproject.toml` and `requirements.txt` files. You may use whatever virtual environment management tool that you would like. These include conda, poetry, and virtualenv. Poetry is used to produce our releases, which are managed and automated by GitHub.
 
-The easiest way to create and activate a virtual environment is
+The easiest way to create and activate a virtual environment is by using the [virtualenv](https://pypi.org/project/virtualenv/) package:
 ```bash
 virtualenv "ENV_PATH"
 source "ENV_PATH/bin/activate"
 pip install --upgrade pip
 pip install -r requirements.txt
 ```
```

