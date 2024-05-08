# Comparing `tmp/auto_circuit-0.1.2.tar.gz` & `tmp/auto_circuit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_circuit-0.1.2.tar", max compression
+gzip compressed data, was "auto_circuit-0.1.3.tar", max compression
```

## Comparing `auto_circuit-0.1.2.tar` & `auto_circuit-0.1.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1276 2024-05-06 00:21:23.358464 auto_circuit-0.1.2/README.md
--rw-r--r--   0        0        0    14880 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/data.py
--rw-r--r--   0        0        0     8438 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/experiment_utils.py
--rw-r--r--   0        0        0    10338 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/experiments.py
--rw-r--r--   0        0        0    13917 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/language_rotations.py
--rw-r--r--   0        0        0     6259 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/area_under_curve.py
--rw-r--r--   0        0        0     3741 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/avoid_edges.py
--rw-r--r--   0        0        0     9754 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/completeness_metrics/same_under_knockouts.py
--rw-r--r--   0        0        0     8595 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/completeness_metrics/train_same_under_knockouts.py
--rw-r--r--   0        0        0     8888 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/docstring_official.py
--rw-r--r--   0        0        0     5322 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/greaterthan_official.py
--rw-r--r--   0        0        0    11697 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/ioi_official.py
--rw-r--r--   0        0        0     8481 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/sports_players_official.py
--rw-r--r--   0        0        0     4896 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/tracr/reverse_official.py
--rw-r--r--   0        0        0     4648 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/tracr/xproportion_official.py
--rw-r--r--   0        0        0     4396 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/measure_roc.py
--rw-r--r--   0        0        0     4070 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/roc_plot.py
--rw-r--r--   0        0        0     2091 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/answer_diff.py
--rw-r--r--   0        0        0     5344 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/answer_diff_percent.py
--rw-r--r--   0        0        0     2208 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/answer_value.py
--rw-r--r--   0        0        0     2709 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/correct_answer_percent.py
--rw-r--r--   0        0        0     2264 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/kl_div.py
--rw-r--r--   0        0        0     7097 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/measure_prune_metrics.py
--rw-r--r--   0        0        0     6360 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/prune_metrics.py
--rw-r--r--   0        0        0     3896 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/prune_metrics_plot.py
--rw-r--r--   0        0        0     6359 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_scores_similarity.py
--rw-r--r--   0        0        0     5426 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/micro_model_utils.py
--rw-r--r--   0        0        0     6135 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/sparse_autoencoders/autoencoder_training.py
--rw-r--r--   0        0        0    11709 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/sparse_autoencoders/autoencoder_transformer.py
--rw-r--r--   0        0        0     7190 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/sparse_autoencoders/sparse_autoencoder.py
--rw-r--r--   0        0        0     9047 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/task_projectors/projector_transformer.py
--rw-r--r--   0        0        0     5846 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/task_projectors/task_projector.py
--rw-r--r--   0        0        0    12255 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/task_projectors/task_projector_training.py
--rw-r--r--   0        0        0     7950 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/tracr_model_utils.py
--rw-r--r--   0        0        0     7622 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/transformer_lens_utils.py
--rw-r--r--   0        0        0    14863 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/playground.py
--rw-r--r--   0        0        0     5123 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune.py
--rw-r--r--   0        0        0     7888 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/ACDC.py
--rw-r--r--   0        0        0     1718 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/activation_magnitude.py
--rw-r--r--   0        0        0     3759 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/circuit_probing.py
--rw-r--r--   0        0        0     4373 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/edge_attribution_patching.py
--rw-r--r--   0        0        0     1054 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/ground_truth.py
--rw-r--r--   0        0        0     5064 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/mask_gradient.py
--rw-r--r--   0        0        0     2699 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/parameter_integrated_gradients.py
--rw-r--r--   0        0        0    10248 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/prune_algos.py
--rw-r--r--   0        0        0      994 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/random_edges.py
--rw-r--r--   0        0        0    11955 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/subnetwork_probing.py
--rw-r--r--   0        0        0     7465 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/pythia-2_8b-sports.py
--rw-r--r--   0        0        0    16984 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/tasks.py
--rw-r--r--   0        0        0     3729 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/tracr_experiments.py
--rw-r--r--   0        0        0    11715 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/types.py
--rw-r--r--   0        0        0     6091 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/uniqueness_experiments.py
--rw-r--r--   0        0        0     6775 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/ablation_activations.py
--rw-r--r--   0        0        0      590 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/custom_tqdm.py
--rw-r--r--   0        0        0    19341 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/graph_utils.py
--rw-r--r--   0        0        0     7165 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/misc.py
--rw-r--r--   0        0        0     6295 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/patch_wrapper.py
--rw-r--r--   0        0        0     9609 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/patchable_model.py
--rw-r--r--   0        0        0     9933 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/tensor_ops.py
--rw-r--r--   0        0        0    11460 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/visualize.py
--rw-r--r--   0        0        0     1397 2024-05-06 00:23:34.131356 auto_circuit-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 auto_circuit-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1276 2024-05-08 23:47:50.241213 auto_circuit-0.1.3/README.md
+-rw-r--r--   0        0        0    14880 2024-05-08 23:47:50.241213 auto_circuit-0.1.3/auto_circuit/data.py
+-rw-r--r--   0        0        0     8438 2024-05-08 23:47:50.241213 auto_circuit-0.1.3/auto_circuit/experiment_utils.py
+-rw-r--r--   0        0        0    10338 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/experiments.py
+-rw-r--r--   0        0        0    13917 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/language_rotations.py
+-rw-r--r--   0        0        0     6259 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/area_under_curve.py
+-rw-r--r--   0        0        0     3741 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/avoid_edges.py
+-rw-r--r--   0        0        0     9754 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/completeness_metrics/same_under_knockouts.py
+-rw-r--r--   0        0        0     8595 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/completeness_metrics/train_same_under_knockouts.py
+-rw-r--r--   0        0        0     8888 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/docstring_official.py
+-rw-r--r--   0        0        0     5322 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/greaterthan_official.py
+-rw-r--r--   0        0        0    11697 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/ioi_official.py
+-rw-r--r--   0        0        0     8481 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/sports_players_official.py
+-rw-r--r--   0        0        0     4896 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/tracr/reverse_official.py
+-rw-r--r--   0        0        0     4648 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/tracr/xproportion_official.py
+-rw-r--r--   0        0        0     4396 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/measure_roc.py
+-rw-r--r--   0        0        0     4070 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/roc_plot.py
+-rw-r--r--   0        0        0     2091 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/answer_diff.py
+-rw-r--r--   0        0        0     5344 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/answer_diff_percent.py
+-rw-r--r--   0        0        0     2208 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/answer_value.py
+-rw-r--r--   0        0        0     2709 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/correct_answer_percent.py
+-rw-r--r--   0        0        0     2264 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/kl_div.py
+-rw-r--r--   0        0        0     7097 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/measure_prune_metrics.py
+-rw-r--r--   0        0        0     6360 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/prune_metrics.py
+-rw-r--r--   0        0        0     3896 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/prune_metrics_plot.py
+-rw-r--r--   0        0        0     6359 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_scores_similarity.py
+-rw-r--r--   0        0        0     5426 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/micro_model_utils.py
+-rw-r--r--   0        0        0     6135 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/sparse_autoencoders/autoencoder_training.py
+-rw-r--r--   0        0        0    11781 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/sparse_autoencoders/autoencoder_transformer.py
+-rw-r--r--   0        0        0     7190 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/sparse_autoencoders/sparse_autoencoder.py
+-rw-r--r--   0        0        0     9123 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/task_projectors/projector_transformer.py
+-rw-r--r--   0        0        0     5846 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/task_projectors/task_projector.py
+-rw-r--r--   0        0        0    12255 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/task_projectors/task_projector_training.py
+-rw-r--r--   0        0        0     7950 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/tracr_model_utils.py
+-rw-r--r--   0        0        0     7694 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/transformer_lens_utils.py
+-rw-r--r--   0        0        0    14863 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/playground.py
+-rw-r--r--   0        0        0     5123 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune.py
+-rw-r--r--   0        0        0     7888 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/ACDC.py
+-rw-r--r--   0        0        0     1718 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/activation_magnitude.py
+-rw-r--r--   0        0        0     3759 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/circuit_probing.py
+-rw-r--r--   0        0        0     4373 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/edge_attribution_patching.py
+-rw-r--r--   0        0        0     1054 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/ground_truth.py
+-rw-r--r--   0        0        0     5064 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/mask_gradient.py
+-rw-r--r--   0        0        0     2699 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/parameter_integrated_gradients.py
+-rw-r--r--   0        0        0    10248 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/prune_algos.py
+-rw-r--r--   0        0        0      994 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/random_edges.py
+-rw-r--r--   0        0        0    11955 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/subnetwork_probing.py
+-rw-r--r--   0        0        0     7465 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/pythia-2_8b-sports.py
+-rw-r--r--   0        0        0    16984 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/tasks.py
+-rw-r--r--   0        0        0     3729 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/tracr_experiments.py
+-rw-r--r--   0        0        0    11715 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/types.py
+-rw-r--r--   0        0        0     6091 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/uniqueness_experiments.py
+-rw-r--r--   0        0        0     6775 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/ablation_activations.py
+-rw-r--r--   0        0        0      590 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/custom_tqdm.py
+-rw-r--r--   0        0        0    19341 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/graph_utils.py
+-rw-r--r--   0        0        0     7165 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/misc.py
+-rw-r--r--   0        0        0     6295 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/patch_wrapper.py
+-rw-r--r--   0        0        0     9609 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/patchable_model.py
+-rw-r--r--   0        0        0     9933 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/tensor_ops.py
+-rw-r--r--   0        0        0    11460 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/visualize.py
+-rw-r--r--   0        0        0     1397 2024-05-08 23:49:49.105869 auto_circuit-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 auto_circuit-0.1.3/PKG-INFO
```

### Comparing `auto_circuit-0.1.2/README.md` & `auto_circuit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/data.py` & `auto_circuit-0.1.3/auto_circuit/data.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/experiment_utils.py` & `auto_circuit-0.1.3/auto_circuit/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/experiments.py` & `auto_circuit-0.1.3/auto_circuit/experiments.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/language_rotations.py` & `auto_circuit-0.1.3/auto_circuit/language_rotations.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/area_under_curve.py` & `auto_circuit-0.1.3/auto_circuit/metrics/area_under_curve.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/avoid_edges.py` & `auto_circuit-0.1.3/auto_circuit/metrics/avoid_edges.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/completeness_metrics/same_under_knockouts.py` & `auto_circuit-0.1.3/auto_circuit/metrics/completeness_metrics/same_under_knockouts.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/completeness_metrics/train_same_under_knockouts.py` & `auto_circuit-0.1.3/auto_circuit/metrics/completeness_metrics/train_same_under_knockouts.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/docstring_official.py` & `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/docstring_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/greaterthan_official.py` & `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/greaterthan_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/ioi_official.py` & `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/ioi_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/sports_players_official.py` & `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/sports_players_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/tracr/reverse_official.py` & `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/tracr/reverse_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/tracr/xproportion_official.py` & `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/tracr/xproportion_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/measure_roc.py` & `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/measure_roc.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/roc_plot.py` & `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/roc_plot.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/answer_diff.py` & `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/answer_diff.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/answer_diff_percent.py` & `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/answer_diff_percent.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/answer_value.py` & `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/answer_value.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/correct_answer_percent.py` & `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/correct_answer_percent.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/kl_div.py` & `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/kl_div.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/measure_prune_metrics.py` & `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/measure_prune_metrics.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/prune_metrics.py` & `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/prune_metrics.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/prune_metrics_plot.py` & `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/prune_metrics_plot.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/metrics/prune_scores_similarity.py` & `auto_circuit-0.1.3/auto_circuit/metrics/prune_scores_similarity.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/model_utils/micro_model_utils.py` & `auto_circuit-0.1.3/auto_circuit/model_utils/micro_model_utils.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/model_utils/sparse_autoencoders/autoencoder_training.py` & `auto_circuit-0.1.3/auto_circuit/model_utils/sparse_autoencoders/autoencoder_training.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/model_utils/sparse_autoencoders/autoencoder_transformer.py` & `auto_circuit-0.1.3/auto_circuit/model_utils/sparse_autoencoders/autoencoder_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,16 @@
 
 def factorized_src_nodes(model: AutoencoderTransformer) -> Set[SrcNode]:
     """Get the source part of each edge in the factorized graph, grouped by layer.
     Graph is factorized following the Mathematical Framework paper."""
     assert model.cfg.use_attn_result  # Get attention head outputs separately
     assert model.cfg.use_attn_in  # Get attention head inputs separately
     assert model.cfg.use_split_qkv_input  # Separate Q, K, V input for each head
-    assert model.cfg.use_hook_mlp_in  # Get MLP input BEFORE layernorm
+    if not model.cfg.attn_only:
+        assert model.cfg.use_hook_mlp_in  # Get MLP input BEFORE layernorm
     assert not model.cfg.attn_only
 
     layers, idxs = count(), count()
     nodes = set()
     nodes.add(
         SrcNode(
             name="Resid Start",
@@ -244,15 +245,16 @@
 ) -> Set[DestNode]:
     """Get the destination part of each edge in the factorized graph, grouped by layer.
     Graph is factorized following the Mathematical Framework paper."""
     if separate_qkv:
         assert model.cfg.use_split_qkv_input  # Separate Q, K, V input for each head
     else:
         assert model.cfg.use_attn_in
-    assert model.cfg.use_hook_mlp_in  # Get MLP input BEFORE layernorm
+    if not model.cfg.attn_only:
+        assert model.cfg.use_hook_mlp_in  # Get MLP input BEFORE layernorm
     layers = count(1)
     nodes = set()
     for block_idx in range(model.cfg.n_layers):
         layer = next(layers)
         for head_idx in range(model.cfg.n_heads):
             if separate_qkv:
                 for letter in ["Q", "K", "V"]:
```

### Comparing `auto_circuit-0.1.2/auto_circuit/model_utils/sparse_autoencoders/sparse_autoencoder.py` & `auto_circuit-0.1.3/auto_circuit/model_utils/sparse_autoencoders/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/model_utils/task_projectors/projector_transformer.py` & `auto_circuit-0.1.3/auto_circuit/model_utils/task_projectors/projector_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,15 +143,16 @@
 #     """Get the source part of each edge in the factorized graph, grouped by layer.
 #     Graph is factorized following the Mathematical Framework paper."""
 #     assert model.cfg.use_attn_result  # Get attention head outputs separately
 #     assert (
 #         model.cfg.use_attn_in
 #     )  # Get attention head inputs separately (but Q, K, V are still combined)
 #     assert model.cfg.use_split_qkv_input  # Separate Q, K, V input for each head
-#     assert model.cfg.use_hook_mlp_in  # Get MLP input BEFORE layernorm
+#     if not model.cfg.attn_only:
+#         assert model.cfg.use_hook_mlp_in  # Get MLP input BEFORE layernorm
 #     layers, idxs = count(), count()
 #     nodes = set()
 #     nodes.add(
 #         SrcNode(
 #             name="Resid Start",
 #             module_name="blocks.0.hook_resid_pre",
 #             layer=next(layers),
@@ -196,15 +197,16 @@
 #     """Get the destination part of each edge in the factorized graph, grouped by layer
 #     Graph is factorized following the Mathematical Framework paper."""
 #     assert model.cfg.use_attn_result  # Get attention head outputs separately
 #     assert (
 #         model.cfg.use_attn_in
 #     )  # Get attention head inputs separately (but Q, K, V are still combined)
 #     # assert model.cfg.use_split_qkv_input  # Separate Q, K, V input for each head
-#     assert model.cfg.use_hook_mlp_in  # Get MLP input BEFORE layernorm
+#     if not model.cfg.attn_only:
+#         assert model.cfg.use_hook_mlp_in  # Get MLP input BEFORE layernorm
 #     layers, idxs = count(1), count()
 #     nodes = set()
 #     for block_idx in range(model.cfg.n_layers):
 #         layer = next(layers)
 #         for head_idx in range(model.cfg.n_heads):
 #             nodes.add(
 #                 DestNode(
```

### Comparing `auto_circuit-0.1.2/auto_circuit/model_utils/task_projectors/task_projector.py` & `auto_circuit-0.1.3/auto_circuit/model_utils/task_projectors/task_projector.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/model_utils/task_projectors/task_projector_training.py` & `auto_circuit-0.1.3/auto_circuit/model_utils/task_projectors/task_projector_training.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/model_utils/tracr_model_utils.py` & `auto_circuit-0.1.3/auto_circuit/model_utils/tracr_model_utils.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/model_utils/transformer_lens_utils.py` & `auto_circuit-0.1.3/auto_circuit/model_utils/transformer_lens_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     [Elhage et al. (2021)](https://transformer-circuits.pub/2021/framework/index.html).
     See also [Molina (2023)](https://arxiv.org/pdf/2309.07315.pdf) for a good
     explanation.
 
     ![](../../assets/Factorized_Transformer.png)
     """
     assert model.cfg.use_attn_result  # Get attention head outputs separately
-    assert model.cfg.use_hook_mlp_in  # Get MLP input BEFORE layernorm
+    if not model.cfg.attn_only:
+        assert model.cfg.use_hook_mlp_in  # Get MLP input BEFORE layernorm
     layers, idxs = count(), count()
     nodes = set()
     nodes.add(
         SrcNode(
             name="Resid Start",
             module_name="blocks.0.hook_resid_pre",
             layer=next(layers),
@@ -71,15 +72,16 @@
 
     ![](../../assets/Factorized_Transformer.png)
     """
     if separate_qkv:
         assert model.cfg.use_split_qkv_input  # Separate Q, K, V input for each head
     else:
         assert model.cfg.use_attn_in
-    assert model.cfg.use_hook_mlp_in  # Get MLP input BEFORE layernorm
+    if not model.cfg.attn_only:
+        assert model.cfg.use_hook_mlp_in  # Get MLP input BEFORE layernorm
     layers = count(1)
     nodes = set()
     for block_idx in range(model.cfg.n_layers):
         layer = next(layers)
         for head_idx in range(model.cfg.n_heads):
             if separate_qkv:
                 for letter in ["Q", "K", "V"]:
```

### Comparing `auto_circuit-0.1.2/auto_circuit/playground.py` & `auto_circuit-0.1.3/auto_circuit/playground.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/prune.py` & `auto_circuit-0.1.3/auto_circuit/prune.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/prune_algos/ACDC.py` & `auto_circuit-0.1.3/auto_circuit/prune_algos/ACDC.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/prune_algos/activation_magnitude.py` & `auto_circuit-0.1.3/auto_circuit/prune_algos/activation_magnitude.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/prune_algos/circuit_probing.py` & `auto_circuit-0.1.3/auto_circuit/prune_algos/circuit_probing.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/prune_algos/edge_attribution_patching.py` & `auto_circuit-0.1.3/auto_circuit/prune_algos/edge_attribution_patching.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/prune_algos/ground_truth.py` & `auto_circuit-0.1.3/auto_circuit/prune_algos/ground_truth.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/prune_algos/mask_gradient.py` & `auto_circuit-0.1.3/auto_circuit/prune_algos/mask_gradient.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/prune_algos/parameter_integrated_gradients.py` & `auto_circuit-0.1.3/auto_circuit/prune_algos/parameter_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/prune_algos/prune_algos.py` & `auto_circuit-0.1.3/auto_circuit/prune_algos/prune_algos.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/prune_algos/random_edges.py` & `auto_circuit-0.1.3/auto_circuit/prune_algos/random_edges.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/prune_algos/subnetwork_probing.py` & `auto_circuit-0.1.3/auto_circuit/prune_algos/subnetwork_probing.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/pythia-2_8b-sports.py` & `auto_circuit-0.1.3/auto_circuit/pythia-2_8b-sports.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/tasks.py` & `auto_circuit-0.1.3/auto_circuit/tasks.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/tracr_experiments.py` & `auto_circuit-0.1.3/auto_circuit/tracr_experiments.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/types.py` & `auto_circuit-0.1.3/auto_circuit/types.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/uniqueness_experiments.py` & `auto_circuit-0.1.3/auto_circuit/uniqueness_experiments.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/utils/ablation_activations.py` & `auto_circuit-0.1.3/auto_circuit/utils/ablation_activations.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/utils/custom_tqdm.py` & `auto_circuit-0.1.3/auto_circuit/utils/custom_tqdm.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/utils/graph_utils.py` & `auto_circuit-0.1.3/auto_circuit/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/utils/misc.py` & `auto_circuit-0.1.3/auto_circuit/utils/misc.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/utils/patch_wrapper.py` & `auto_circuit-0.1.3/auto_circuit/utils/patch_wrapper.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/utils/patchable_model.py` & `auto_circuit-0.1.3/auto_circuit/utils/patchable_model.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/utils/tensor_ops.py` & `auto_circuit-0.1.3/auto_circuit/utils/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/auto_circuit/visualize.py` & `auto_circuit-0.1.3/auto_circuit/visualize.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.2/pyproject.toml` & `auto_circuit-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auto-circuit"
-version = "0.1.2"  # This isn't used. Version set during Github action.
+version = "0.1.3"  # This isn't used. Version set during Github action.
 description = ""
 authors = ["UFO-101 <josephmiller101@gmail.com>"]
 readme = "README.md"
 packages = [{include = "auto_circuit"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `auto_circuit-0.1.2/PKG-INFO` & `auto_circuit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-circuit
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: UFO-101
 Author-email: josephmiller101@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

