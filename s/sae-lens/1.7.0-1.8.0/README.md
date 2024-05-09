# Comparing `tmp/sae_lens-1.7.0.tar.gz` & `tmp/sae_lens-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-1.7.0.tar", max compression
+gzip compressed data, was "sae_lens-1.8.0.tar", max compression
```

## Comparing `sae_lens-1.7.0.tar` & `sae_lens-1.8.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2024-05-08 15:47:23.850975 sae_lens-1.7.0/LICENSE
--rw-r--r--   0        0        0     2553 2024-05-08 15:47:23.850975 sae_lens-1.7.0/README.md
--rw-r--r--   0        0        0     1917 2024-05-08 15:47:25.194976 sae_lens-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      939 2024-05-08 15:47:25.194976 sae_lens-1.7.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 15:47:23.858975 sae_lens-1.7.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-05-08 15:47:23.858975 sae_lens-1.7.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-05-08 15:47:23.858975 sae_lens-1.7.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    17062 2024-05-08 15:47:23.858975 sae_lens-1.7.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    20134 2024-05-08 15:47:23.858975 sae_lens-1.7.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     1164 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/pretrained_saes.yaml
--rw-r--r--   0        0        0        0 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/toolkit/__init__.py
--rw-r--r--   0        0        0     2674 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/toolkit/pretrained_sae_loaders.py
--rw-r--r--   0        0        0     6643 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0     1143 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/toolkit/pretrained_saes_directory.py
--rw-r--r--   0        0        0        0 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0      471 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/activation_functions.py
--rw-r--r--   0        0        0    20496 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     5974 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0    13395 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     6713 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     4339 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1020 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     5065 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     8284 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2319 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    20000 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    30629 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     5002 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0      423 2024-05-08 15:47:23.862975 sae_lens-1.7.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 sae_lens-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-09 21:45:26.992473 sae_lens-1.8.0/LICENSE
+-rw-r--r--   0        0        0     2553 2024-05-09 21:45:26.992473 sae_lens-1.8.0/README.md
+-rw-r--r--   0        0        0     1917 2024-05-09 21:45:28.280470 sae_lens-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      939 2024-05-09 21:45:28.280470 sae_lens-1.8.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    17062 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20134 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     1164 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0        0 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     2674 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     6643 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0        0 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/activation_functions.py
+-rw-r--r--   0        0        0    20496 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     6049 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0    13553 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/config.py
+-rw-r--r--   0        0        0     6713 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     4339 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1280 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     5065 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     8403 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2424 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    20000 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    30629 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     5002 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0      423 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 sae_lens-1.8.0/PKG-INFO
```

### Comparing `sae_lens-1.7.0/LICENSE` & `sae_lens-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/README.md` & `sae_lens-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/pyproject.toml` & `sae_lens-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "1.7.0"
+version = "1.8.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `sae_lens-1.7.0/sae_lens/__init__.py` & `sae_lens-1.8.0/sae_lens/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import CacheActivationsRunner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-1.7.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-1.8.0/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-1.8.0/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-1.8.0/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-1.8.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/analysis/tsea.py` & `sae_lens-1.8.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/pretrained_saes.yaml` & `sae_lens-1.8.0/sae_lens/pretrained_saes.yaml`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/toolkit/pretrained_sae_loaders.py` & `sae_lens-1.8.0/sae_lens/toolkit/pretrained_sae_loaders.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-1.8.0/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/toolkit/pretrained_saes_directory.py` & `sae_lens-1.8.0/sae_lens/toolkit/pretrained_saes_directory.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/training/activations_store.py` & `sae_lens-1.8.0/sae_lens/training/activations_store.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/training/cache_activations_runner.py` & `sae_lens-1.8.0/sae_lens/training/cache_activations_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     def __init__(self, cfg: CacheActivationsRunnerConfig):
         self.cfg = cfg
         self.model = load_model(
             model_class_name=cfg.model_class_name,
             model_name=cfg.model_name,
             device=cfg.device,
+            model_from_pretrained_kwargs=cfg.model_from_pretrained_kwargs,
         )
         self.activations_store = ActivationsStore.from_config(
             self.model,
             cfg,
         )
 
         self.file_extension = "safetensors"
```

### Comparing `sae_lens-1.7.0/sae_lens/training/config.py` & `sae_lens-1.8.0/sae_lens/training/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,15 @@
 
     # Misc
     resume: bool = False
     n_checkpoints: int = 0
     checkpoint_path: str = "checkpoints"
     verbose: bool = True
     model_kwargs: dict[str, Any] = field(default_factory=dict)
+    model_from_pretrained_kwargs: dict[str, Any] = field(default_factory=dict)
     sae_lens_version: str = field(default_factory=lambda: __version__)
     sae_lens_training_version: str = field(default_factory=lambda: __version__)
 
     def __post_init__(self):
         if self.use_cached_activations and self.cached_activations_path is None:
             self.cached_activations_path = _default_cached_activations_path(
                 self.dataset_path,
@@ -324,14 +325,15 @@
 
     # Activation caching stuff
     shuffle_every_n_buffers: int = 10
     n_shuffles_with_last_section: int = 10
     n_shuffles_in_entire_dir: int = 10
     n_shuffles_final: int = 100
     model_kwargs: dict[str, Any] = field(default_factory=dict)
+    model_from_pretrained_kwargs: dict[str, Any] = field(default_factory=dict)
 
     def __post_init__(self):
         # Autofill cached_activations_path unless the user overrode it
         if self.new_cached_activations_path is None:
             self.new_cached_activations_path = _default_cached_activations_path(
                 self.dataset_path,
                 self.model_name,
```

### Comparing `sae_lens-1.7.0/sae_lens/training/evals.py` & `sae_lens-1.8.0/sae_lens/training/evals.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/training/geometric_median.py` & `sae_lens-1.8.0/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/training/lm_runner.py` & `sae_lens-1.8.0/sae_lens/training/lm_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/training/optim.py` & `sae_lens-1.8.0/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/training/sae_group.py` & `sae_lens-1.8.0/sae_lens/training/sae_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,16 @@
             # need to add fields to old configs
             if not hasattr(cfg, "model_kwargs"):
                 cfg.model_kwargs = {}
             if not hasattr(cfg, "sae_lens_version"):
                 cfg.sae_lens_version = "0.0.0"
             if not hasattr(cfg, "sae_lens_training_version"):
                 cfg.sae_lens_training_version = "0.0.0"
+            if not hasattr(cfg, "model_from_pretrained_kwargs"):
+                cfg.model_from_pretrained_kwargs = {}
             sparse_autoencoder = SparseAutoencoder(cfg=cfg)
             # add dummy scaling factor to the state dict
             group["state_dict"]["scaling_factor"] = torch.ones(
                 cfg.d_sae, dtype=cfg.dtype, device=cfg.device
             )
             sparse_autoencoder.load_state_dict(group["state_dict"])
             group = cls(cfg)
```

### Comparing `sae_lens-1.7.0/sae_lens/training/session_loader.py` & `sae_lens-1.8.0/sae_lens/training/session_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,10 +63,13 @@
 
         Abstracted to allow for easy modification.
         """
 
         # Todo: add check that model_name is valid
 
         model = load_model(
-            self.cfg.model_class_name, model_name, device=self.cfg.device
+            self.cfg.model_class_name,
+            model_name,
+            device=self.cfg.device,
+            model_from_pretrained_kwargs=self.cfg.model_from_pretrained_kwargs,
         )
         return model
```

### Comparing `sae_lens-1.7.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-1.8.0/sae_lens/training/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/training/toy_model_runner.py` & `sae_lens-1.8.0/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/training/toy_models.py` & `sae_lens-1.8.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-1.8.0/sae_lens/training/train_sae_on_language_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-1.8.0/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.7.0/PKG-INFO` & `sae_lens-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 1.7.0
+Version: 1.8.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

