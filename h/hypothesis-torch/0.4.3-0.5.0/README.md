# Comparing `tmp/hypothesis_torch-0.4.3.tar.gz` & `tmp/hypothesis_torch-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis_torch-0.4.3.tar", last modified: Sun Apr 28 03:29:51 2024, max compression
+gzip compressed data, was "hypothesis_torch-0.5.0.tar", last modified: Thu May  9 02:58:37 2024, max compression
```

## Comparing `hypothesis_torch-0.4.3.tar` & `hypothesis_torch-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 03:29:51.532723 hypothesis_torch-0.4.3/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8094 2024-04-28 03:29:51.532723 hypothesis_torch-0.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5282 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 03:29:51.528723 hypothesis_torch-0.4.3/hypothesis_torch/
--rw-r--r--   0 root         (0) root         (0)     1300 2024-04-28 03:29:48.000000 hypothesis_torch-0.4.3/hypothesis_torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1408 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/hypothesis_torch/device.py
--rw-r--r--   0 root         (0) root         (0)     2757 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/hypothesis_torch/dtype.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/hypothesis_torch/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     1977 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/hypothesis_torch/inspection_util.py
--rw-r--r--   0 root         (0) root         (0)      735 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/hypothesis_torch/layout.py
--rw-r--r--   0 root         (0) root         (0)      846 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/hypothesis_torch/memory_format.py
--rw-r--r--   0 root         (0) root         (0)    10903 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/hypothesis_torch/module.py
--rw-r--r--   0 root         (0) root         (0)      866 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/hypothesis_torch/register_random_torch_state.py
--rw-r--r--   0 root         (0) root         (0)     9464 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/hypothesis_torch/tensor.py
--rw-r--r--   0 root         (0) root         (0)     1442 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/hypothesis_torch/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 03:29:51.528723 hypothesis_torch-0.4.3/hypothesis_torch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8094 2024-04-28 03:29:51.000000 hypothesis_torch-0.4.3/hypothesis_torch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      613 2024-04-28 03:29:51.000000 hypothesis_torch-0.4.3/hypothesis_torch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 03:29:51.000000 hypothesis_torch-0.4.3/hypothesis_torch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2024-04-28 03:29:51.000000 hypothesis_torch-0.4.3/hypothesis_torch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-28 03:29:51.000000 hypothesis_torch-0.4.3/hypothesis_torch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-28 03:29:51.000000 hypothesis_torch-0.4.3/hypothesis_torch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2215 2024-04-28 03:29:17.000000 hypothesis_torch-0.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 03:29:51.532723 hypothesis_torch-0.4.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 02:58:37.212705 hypothesis_torch-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8094 2024-05-09 02:58:37.212705 hypothesis_torch-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5282 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 02:58:37.208705 hypothesis_torch-0.5.0/hypothesis_torch/
+-rw-r--r--   0 root         (0) root         (0)     1335 2024-05-09 02:58:33.000000 hypothesis_torch-0.5.0/hypothesis_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/hypothesis_torch/device.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/hypothesis_torch/dtype.py
+-rw-r--r--   0 root         (0) root         (0)    10784 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/hypothesis_torch/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/hypothesis_torch/inspection_util.py
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/hypothesis_torch/layout.py
+-rw-r--r--   0 root         (0) root         (0)      846 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/hypothesis_torch/memory_format.py
+-rw-r--r--   0 root         (0) root         (0)    10903 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/hypothesis_torch/module.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/hypothesis_torch/py.typed
+-rw-r--r--   0 root         (0) root         (0)      866 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/hypothesis_torch/register_random_torch_state.py
+-rw-r--r--   0 root         (0) root         (0)     9464 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/hypothesis_torch/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/hypothesis_torch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 02:58:37.212705 hypothesis_torch-0.5.0/hypothesis_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8094 2024-05-09 02:58:37.000000 hypothesis_torch-0.5.0/hypothesis_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      639 2024-05-09 02:58:37.000000 hypothesis_torch-0.5.0/hypothesis_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 02:58:37.000000 hypothesis_torch-0.5.0/hypothesis_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2024-05-09 02:58:37.000000 hypothesis_torch-0.5.0/hypothesis_torch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-09 02:58:37.000000 hypothesis_torch-0.5.0/hypothesis_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-09 02:58:37.000000 hypothesis_torch-0.5.0/hypothesis_torch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2215 2024-05-09 02:58:04.000000 hypothesis_torch-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 02:58:37.212705 hypothesis_torch-0.5.0/setup.cfg
```

### Comparing `hypothesis_torch-0.4.3/LICENSE` & `hypothesis_torch-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.3/PKG-INFO` & `hypothesis_torch-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.4.3
+Version: 0.5.0
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,16 +46,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hypothesis
 Requires-Dist: torch
 Provides-Extra: huggingface
 Requires-Dist: transformers; extra == "huggingface"
 Provides-Extra: dev
-Requires-Dist: ruff==0.4.1; extra == "dev"
-Requires-Dist: pytest==8.1.1; extra == "dev"
+Requires-Dist: ruff==0.4.3; extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 
 # hypothesis-torch
 Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
```

### Comparing `hypothesis_torch-0.4.3/README.md` & `hypothesis_torch-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.3/hypothesis_torch/__init__.py` & `hypothesis_torch-0.5.0/hypothesis_torch/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
 """
 
-__version__ = "0.4.3"
+__version__ = "0.5.0"
 import importlib.util
 
 from hypothesis_torch.device import (
     device_strategy,
     AVAILABLE_CPU_DEVICES,
     AVAILABLE_CUDA_DEVICES,
     AVAILABLE_MPS_DEVICES,
@@ -30,8 +30,8 @@
 from hypothesis_torch.module import linear_network_strategy, same_shape_activation_strategy
 from hypothesis_torch.register_random_torch_state import TORCH_RANDOM_WRAPPER
 from hypothesis_torch.tensor import tensor_strategy
 
 
 if importlib.util.find_spec("transformers") is not None:
     # Import Hugging Face strategies if transformers is installed
-    from hypothesis_torch.huggingface import transformer_strategy
+    from hypothesis_torch.huggingface import transformer_strategy, OFFICIALLY_SUPPORTED_TRANSFORMERS
```

### Comparing `hypothesis_torch-0.4.3/hypothesis_torch/device.py` & `hypothesis_torch-0.5.0/hypothesis_torch/device.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.3/hypothesis_torch/dtype.py` & `hypothesis_torch-0.5.0/hypothesis_torch/dtype.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.3/hypothesis_torch/inspection_util.py` & `hypothesis_torch-0.5.0/hypothesis_torch/inspection_util.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.3/hypothesis_torch/layout.py` & `hypothesis_torch-0.5.0/hypothesis_torch/layout.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.3/hypothesis_torch/memory_format.py` & `hypothesis_torch-0.5.0/hypothesis_torch/memory_format.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.3/hypothesis_torch/module.py` & `hypothesis_torch-0.5.0/hypothesis_torch/module.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.3/hypothesis_torch/register_random_torch_state.py` & `hypothesis_torch-0.5.0/hypothesis_torch/register_random_torch_state.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.3/hypothesis_torch/tensor.py` & `hypothesis_torch-0.5.0/hypothesis_torch/tensor.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.3/hypothesis_torch/utils.py` & `hypothesis_torch-0.5.0/hypothesis_torch/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.4.3/hypothesis_torch.egg-info/PKG-INFO` & `hypothesis_torch-0.5.0/hypothesis_torch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.4.3
+Version: 0.5.0
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,16 +46,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hypothesis
 Requires-Dist: torch
 Provides-Extra: huggingface
 Requires-Dist: transformers; extra == "huggingface"
 Provides-Extra: dev
-Requires-Dist: ruff==0.4.1; extra == "dev"
-Requires-Dist: pytest==8.1.1; extra == "dev"
+Requires-Dist: ruff==0.4.3; extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 
 # hypothesis-torch
 Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
```

### Comparing `hypothesis_torch-0.4.3/hypothesis_torch.egg-info/SOURCES.txt` & `hypothesis_torch-0.5.0/hypothesis_torch.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 hypothesis_torch/device.py
 hypothesis_torch/dtype.py
 hypothesis_torch/huggingface.py
 hypothesis_torch/inspection_util.py
 hypothesis_torch/layout.py
 hypothesis_torch/memory_format.py
 hypothesis_torch/module.py
+hypothesis_torch/py.typed
 hypothesis_torch/register_random_torch_state.py
 hypothesis_torch/tensor.py
 hypothesis_torch/utils.py
 hypothesis_torch.egg-info/PKG-INFO
 hypothesis_torch.egg-info/SOURCES.txt
 hypothesis_torch.egg-info/dependency_links.txt
 hypothesis_torch.egg-info/entry_points.txt
```

### Comparing `hypothesis_torch-0.4.3/pyproject.toml` & `hypothesis_torch-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 _ = "hypothesis_torch.register_random_torch_state:_register_random_torch_state"
 
 [project.optional-dependencies]
 huggingface = [
   "transformers",
 ]
 dev = [
-  "ruff==0.4.1",
-  "pytest==8.1.1",
+  "ruff==0.4.3",
+  "pytest==8.2.0",
   "pytest-cov==5.0.0"
 ]
 
 [project.urls]
 Homepage = "https://github.com/qthequartermasterman/hypothesis-torch"
 Documentation = "https://github.com/qthequartermasterman/hypothesis-torch"
 Repository = "https://github.com/qthequartermasterman/hypothesis-torch.git"
```

