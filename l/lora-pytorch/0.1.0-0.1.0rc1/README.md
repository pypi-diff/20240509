# Comparing `tmp/lora_pytorch-0.1.0.tar.gz` & `tmp/lora-pytorch-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lora_pytorch-0.1.0.tar", last modified: Thu May  9 17:37:27 2024, max compression
+gzip compressed data, was "lora-pytorch-0.1.0rc1.tar", last modified: Mon Jul 17 17:05:17 2023, max compression
```

## Comparing `lora_pytorch-0.1.0.tar` & `lora-pytorch-0.1.0rc1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:37:27.651122 lora_pytorch-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-09 17:37:27.651122 lora_pytorch-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:37:27.643122 lora_pytorch-0.1.0/lora_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/lora_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/lora_pytorch/lora.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:37:27.647122 lora_pytorch-0.1.0/lora_pytorch/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/lora_pytorch/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/lora_pytorch/modules/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/lora_pytorch/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/lora_pytorch/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/lora_pytorch/modules/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:37:27.647122 lora_pytorch-0.1.0/lora_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-09 17:37:27.000000 lora_pytorch-0.1.0/lora_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-09 17:37:27.000000 lora_pytorch-0.1.0/lora_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:37:27.000000 lora_pytorch-0.1.0/lora_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-09 17:37:27.000000 lora_pytorch-0.1.0/lora_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 17:37:27.000000 lora_pytorch-0.1.0/lora_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-09 17:37:27.651122 lora_pytorch-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:37:27.647122 lora_pytorch-0.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:37:27.647122 lora_pytorch-0.1.0/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/tests/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/tests/modules/test_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/tests/modules/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-09 17:37:21.000000 lora_pytorch-0.1.0/tests/test_lora.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:05:17.406409 lora-pytorch-0.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-17 17:05:17.406409 lora-pytorch-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:05:17.402409 lora-pytorch-0.1.0rc1/lora_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/lora_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/lora_pytorch/lora.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:05:17.406409 lora-pytorch-0.1.0rc1/lora_pytorch/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/lora_pytorch/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/lora_pytorch/modules/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/lora_pytorch/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/lora_pytorch/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/lora_pytorch/modules/conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/lora_pytorch/modules/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:05:17.402409 lora-pytorch-0.1.0rc1/lora_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-17 17:05:17.000000 lora-pytorch-0.1.0rc1/lora_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-17 17:05:17.000000 lora-pytorch-0.1.0rc1/lora_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:05:17.000000 lora-pytorch-0.1.0rc1/lora_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-17 17:05:17.000000 lora-pytorch-0.1.0rc1/lora_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 17:05:17.000000 lora-pytorch-0.1.0rc1/lora_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-17 17:05:17.406409 lora-pytorch-0.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:05:17.406409 lora-pytorch-0.1.0rc1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:05:17.406409 lora-pytorch-0.1.0rc1/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/tests/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/tests/modules/test_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/tests/modules/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-17 17:05:06.000000 lora-pytorch-0.1.0rc1/tests/test_lora.py
```

### Comparing `lora_pytorch-0.1.0/LICENSE` & `lora-pytorch-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `lora_pytorch-0.1.0/lora_pytorch/lora.py` & `lora-pytorch-0.1.0rc1/lora_pytorch/lora.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
         if not enabled:
             self.disable_lora()
         else:
             self.enable_lora()
 
     def forward(self, x: Tensor, *args, **kwargs) -> Tensor:
-        enable_grad = (self.lora_module is None) and torch.is_grad_enabled()
+        enable_grad = (not self.enabled) and torch.is_grad_enabled()
         with torch.set_grad_enabled(enable_grad):
             y = self.module(x, *args, **kwargs)
         if self.enabled and self.lora_module is not None:
             y = y + self.lora_module(x)
 
         return y
 
@@ -175,52 +175,27 @@
             )
 
         if is_root:
             return LoRA(module, None, enabled=enabled)
         else:
             return module
 
-    @property
-    def weight(self) -> Tensor:
-        if not hasattr(self.module, "weight"):
-            raise AttributeError("Module has no attribute 'weight'")
-
-        if self.enabled and self.lora_module is not None:
-            assert hasattr(self.lora_module, "weight")
-            return self.module.weight + self.lora_module.weight
-        else:
-            return self.module.weight
-
-    @property
-    def bias(self) -> Optional[Tensor]:
-        if not hasattr(self.module, "bias"):
-            return None
-
-        if (
-            self.enabled
-            and self.lora_module is not None
-            and hasattr(self.lora_module, "bias")
-        ):
-            return self.module.bias + self.lora_module.bias
-        else:
-            return self.module.bias
-
 
 class MultiheadAttentionLoRA(LoRA[nn.MultiheadAttention]):
     """
     NOTE: MultiheadAttention doesn't quite fit the "sidecar" pattern, like essentially
     every other module does.  Unlike other modules, which typically have a single
     'weight' parameter that is modified by LoRA, MultiheadAttention has multiple
     parameters that are modified by LoRA, and those parameters interact in non-trivial
     ways (via attention) within the module itself.
 
     For that reason, we emulate all of the necessary properties of MultiheadAttention,
-    and reuse the 'forward' method from MultiheadAttention.  This allows us to
-    dynamically compute the LoRA-adjusted parameters without rewriting *all* of the
-    logic from 'MultiheadAttention.forward'.
+    and reuse the 'forward' method from MultiheadAttention.  This is a bit of a hack,
+    but it allows us to dynamically compute the LoRA-adjusted parameters without
+    rewriting *all* of the logic from 'MultiheadAttention.forward'.
     """
 
     def __init__(
         self,
         module: nn.MultiheadAttention,
         lora_module: Optional[MultiheadAttentionLoRAModule],
         enabled: bool = True,
@@ -317,61 +292,57 @@
     @property
     def in_proj_weight(self) -> Tensor:
         in_proj_weight = self.module.in_proj_weight
         if in_proj_weight is None:
             return None
 
         weight = in_proj_weight.data.detach()
-        if (
-            self.enabled
-            and self.lora_module is not None
-            and self.lora_module.in_proj_weight is not None
-        ):
-            return weight + self.lora_module.in_proj_weight
-        else:
+        if (self.lora_module is None) or (self.lora_module.in_proj_weight is None):
             return weight
+        else:
+            return weight + self.lora_module.in_proj_weight
 
     @property
     def in_proj_bias(self) -> Tensor:
         bias = self.module.in_proj_bias
         if bias is None:
             return None
         else:
             return bias.data.detach()
         # TODO: Add support for 'in_proj_bias' in MultiheadAttentionLoRAModule
 
     @property
     def q_proj_weight(self) -> Optional[Tensor]:
         weight = self.module.q_proj_weight.data.detach()
-        if self.enabled and weight is not None and self.lora_module is not None:
-            return weight + self.lora_module.q_proj_weight
-        else:
+        if (weight is None) or (self.lora_module is None):
             return weight
+        else:
+            return weight + self.lora_module.q_proj_weight
 
     @property
     def k_proj_weight(self) -> Optional[Tensor]:
         weight = self.module.k_proj_weight.data.detach()
-        if self.enabled and (weight is not None) and (self.lora_module is not None):
-            return weight + self.lora_module.k_proj_weight
-        else:
+        if (weight is None) or (self.lora_module is None):
             return weight
+        else:
+            return weight + self.lora_module.k_proj_weight
 
     @property
     def v_proj_weight(self) -> Optional[Tensor]:
         weight = self.module.v_proj_weight.data.detach()
-        if self.enabled and (weight is not None) and (self.lora_module is not None):
-            return weight + self.lora_module.v_proj_weight
-        else:
+        if (weight is None) or (self.lora_module is None):
             return weight
+        else:
+            return weight + self.lora_module.v_proj_weight
 
     @property
     def out_proj(self) -> OutProj:
         weight = self.module.out_proj.weight.data.detach()
         bias = self.module.out_proj.bias
-        if self.enabled and self.lora_module is not None:
+        if self.lora_module is not None:
             lora_out_proj = cast(OutProj, self.lora_module.out_proj)
             weight = weight + lora_out_proj.weight
             if (bias is not None) and (lora_out_proj.bias is not None):
                 # Mypy complains about a type mismatch here (Tensor vs. Parameter)
                 # but Parameter is just a subclass of Tensor, so this is fine.
                 bias = bias + lora_out_proj.bias  # type: ignore
```

### Comparing `lora_pytorch-0.1.0/lora_pytorch/modules/attention.py` & `lora-pytorch-0.1.0rc1/lora_pytorch/modules/attention.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import NamedTuple, Optional
 
 import torch
+from einops import einsum
 from torch import Tensor, nn
 
 from lora_pytorch.modules.base import BaseLoRAModule
 
 
 class OutProj(NamedTuple):
     weight: Tensor
@@ -57,37 +58,39 @@
 
     @property
     def q_proj_weight(self) -> Tensor:
         # einstein notation
         # - o: output channels
         # - i: input channels
         # - r: rank
-        return torch.einsum("o r, r i -> i o", self.q_out.weight, self.q_in.weight)
+        return einsum(self.q_out.weight, self.q_in.weight, "o r, r i -> i o")
 
     @property
     def k_proj_weight(self) -> Tensor:
-        return torch.einsum("o r, r i -> i o", self.k_out.weight, self.k_in.weight)
+        return einsum(self.k_out.weight, self.k_in.weight, "o r, r i -> i o")
 
     @property
     def v_proj_weight(self) -> Tensor:
-        return torch.einsum("o r, r i -> i o", self.v_out.weight, self.v_in.weight)
+        return einsum(self.v_out.weight, self.v_in.weight, "o r, r i -> i o")
 
     @property
     def in_proj_weight(self) -> Optional[Tensor]:
         if (self.kdim == self.embed_dim) and (self.vdim == self.embed_dim):
             return torch.cat(
                 (self.q_proj_weight, self.k_proj_weight, self.v_proj_weight), dim=0
             )
         else:
             return None
 
     @property
     def out_proj(self) -> OutProj:
-        weight = torch.einsum("o r, r i -> o i", self.o_out.weight, self.o_in.weight)
-        return OutProj(weight=weight, bias=self.o_out.bias)
+        return OutProj(
+            weight=einsum(self.o_out.weight, self.o_in.weight, "o r, r i -> o i"),
+            bias=self.o_out.bias,
+        )
 
     def _reset_parameters(self):
         # NOTE: The original LoRA paper recommends multiplying the output of 'in_proj'
         # by (alpha / rank).  This adds more computation to the forward pass, and it's
         # mathematically equivalent to scaling 'in_proj' by (alpha / rank) ahead of
         # time.  I have chosen the second option for simplicity.
         nn.init.kaiming_uniform_(self.q_in.weight, self.alpha / self.rank)
```

### Comparing `lora_pytorch-0.1.0/lora_pytorch/modules/conv.py` & `lora-pytorch-0.1.0rc1/lora_pytorch/modules/conv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from math import sqrt
 from typing import Optional, Tuple, TypeVar, Union
 
 import torch
+from einops import einsum
 from torch import Tensor, nn
 
 from lora_pytorch.modules.base import BaseLoRAModule
 
 Conv = Union[nn.Conv1d, nn.Conv2d, nn.Conv3d]
 ConvType = TypeVar("ConvType", nn.Conv1d, nn.Conv2d, nn.Conv3d)
 
@@ -32,18 +33,18 @@
 
     @torch.no_grad()
     def merge(self, module: ConvType, inplace: bool = False) -> ConvType:  # type: ignore
         # einstein notation:
         # - i: in channels
         # - o: out channels
         # - r: rank
-        weight = torch.einsum(
-            "o r ..., r i ... -> o i ...",
+        weight = einsum(
             self.out_conv.weight.data,
             self.in_conv.weight.data,
+            "o r ..., r i ... -> o i ...",
         )
         # TODO: Detailed error message
         assert module.weight.data.shape == weight.shape
 
         if inplace:
             module.weight.data += weight
             return module
@@ -110,16 +111,14 @@
         # time.  I have chosen the second option for simplicity.
         #
         # Normally, the weights of 'in_proj' are initialized with 'kaiming_uniform_',
         # and 'a=sqrt(5)'.  Since we're scaling the weights by (alpha / rank), we
         # should scale 'a' by the same amount.
         nn.init.kaiming_uniform_(self.in_conv.weight, a=(sqrt(5) * alpha / rank))
         nn.init.zeros_(self.out_conv.weight)
-        if self.out_conv.bias is not None:
-            nn.init.zeros_(self.out_conv.bias)
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}({self.in_channels}, {self.out_channels}, "
             f"rank={self.rank}), kernel_size={self.kernel_size}, stride={self.stride}, "
             f"padding={self.padding}, dilation={self.dilation}, bias={self.bias})"
         )
@@ -168,16 +167,14 @@
         # time.  I have chosen the second option for simplicity.
         #
         # Normally, the weights of 'in_proj' are initialized with 'kaiming_uniform_',
         # and 'a=sqrt(5)'.  Since we're scaling the weights by (alpha / rank), we
         # should scale 'a' by the same amount.
         nn.init.kaiming_uniform_(self.in_conv.weight, a=(sqrt(5) * alpha / rank))
         nn.init.zeros_(self.out_conv.weight)
-        if self.out_conv.bias is not None:
-            nn.init.zeros_(self.out_conv.bias)
 
 
 class Conv3dLoRAModule(_ConvLoRA[nn.Conv3d]):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
@@ -219,9 +216,7 @@
         # time.  I have chosen the second option for simplicity.
         #
         # Normally, the weights of 'in_proj' are initialized with 'kaiming_uniform_',
         # and 'a=sqrt(5)'.  Since we're scaling the weights by (alpha / rank), we
         # should scale 'a' by the same amount.
         nn.init.kaiming_uniform_(self.in_conv.weight, a=(sqrt(5) * alpha / rank))
         nn.init.zeros_(self.out_conv.weight)
-        if self.out_conv.bias is not None:
-            nn.init.zeros_(self.out_conv.bias)
```

### Comparing `lora_pytorch-0.1.0/lora_pytorch/modules/linear.py` & `lora-pytorch-0.1.0rc1/lora_pytorch/modules/linear.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import Optional
 
 import torch
+from einops import einsum
 from torch import Tensor, nn
 
 from lora_pytorch.modules.base import BaseLoRAModule
 
 
 class LinearLoRAModule(BaseLoRAModule[nn.Linear]):
     def __init__(
@@ -56,15 +57,15 @@
 
     @torch.no_grad()
     def merge(self, module: nn.Linear, inplace: bool = False) -> nn.Linear:
         # einstein notation:
         # - i: input features
         # - o: output features
         # - r: rank
-        lora_weight = torch.einsum("i r, r o -> o i", self.in_proj, self.out_proj)
+        lora_weight = einsum(self.in_proj, self.out_proj, "i r, r o -> o i")
 
         if inplace:
             module.weight.data += lora_weight
             return module
 
         out = nn.Linear(
             in_features=module.in_features,
@@ -72,11 +73,7 @@
             bias=module.bias is not None,
             device=module.weight.device,
             dtype=module.weight.dtype,
         )
         out.weight.data = module.weight.data + lora_weight
         out.bias = module.bias
         return out
-
-    @property
-    def weight(self) -> Tensor:
-        return torch.einsum("i r, r o -> o i", self.in_proj, self.out_proj)
```

### Comparing `lora_pytorch-0.1.0/lora_pytorch.egg-info/SOURCES.txt` & `lora-pytorch-0.1.0rc1/lora_pytorch.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 lora_pytorch.egg-info/dependency_links.txt
 lora_pytorch.egg-info/requires.txt
 lora_pytorch.egg-info/top_level.txt
 lora_pytorch/modules/__init__.py
 lora_pytorch/modules/attention.py
 lora_pytorch/modules/base.py
 lora_pytorch/modules/conv.py
+lora_pytorch/modules/conv_transpose.py
 lora_pytorch/modules/linear.py
 tests/test_lora.py
 tests/modules/__init__.py
 tests/modules/test_conv.py
 tests/modules/test_linear.py
```

### Comparing `lora_pytorch-0.1.0/setup.py` & `lora-pytorch-0.1.0rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,26 +14,15 @@
 
     if version.lower().startswith("fatal"):
         version = "0.0.0"
 
     return version
 
 
-extras_require = {
-    "test": [
-        "black==23.12.0",
-        "flake8",
-        "isort",
-        "mypy==1.8.0",
-        "pytest",
-        "pytest-cov",
-        "torchtext",
-        "torchvision",
-    ]
-}
+extras_require = {"test": ["black", "flake8", "isort", "mypy", "pytest", "pytest-cov"]}
 extras_require["dev"] = ["pre-commit", *extras_require["test"]]
 all_require = [r for reqs in extras_require.values() for r in reqs]
 extras_require["all"] = all_require
 
 
 setup(
     name="lora-pytorch",
@@ -42,14 +31,15 @@
     author_email="frank.odom.iii@gmail.com",
     url="https://github.com/fkodom/lora-pytorch",
     packages=setuptools.find_packages(exclude=["tests"]),
     description="project_description",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     install_requires=[
+        "einops>=0.6.0,<1.0.0",
         "torch>=1.7.0,<3.0.0",
     ],
     extras_require=extras_require,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
```

### Comparing `lora_pytorch-0.1.0/tests/modules/test_conv.py` & `lora-pytorch-0.1.0rc1/tests/modules/test_conv.py`

 * *Files identical despite different names*

### Comparing `lora_pytorch-0.1.0/tests/modules/test_linear.py` & `lora-pytorch-0.1.0rc1/tests/modules/test_linear.py`

 * *Files identical despite different names*

### Comparing `lora_pytorch-0.1.0/tests/test_lora.py` & `lora-pytorch-0.1.0rc1/tests/test_lora.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from copy import deepcopy
 from functools import partial
-from typing import Callable, Generator, Tuple
+from typing import Generator
 
 import pytest
 import torch
-from pytest import FixtureRequest
-from torch import Tensor, nn
-from torchtext.functional import to_tensor
-from torchtext.models import XLMR_BASE_ENCODER
+from torch import nn
 from torchvision.models import ResNet18_Weights, ViT_B_32_Weights, resnet18, vit_b_32
 
 from lora_pytorch.lora import LoRA
 
 DEVICE = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-DTYPE = torch.float64  # for better precision/stability when testing LoRA
 # Force CUDA ops to be deterministic
 torch.backends.cudnn.deterministic = True
 torch.backends.cudnn.benchmark = False
 
 
 def _init_random_lora_module(module: nn.Module):
     for child in module.children():
@@ -51,22 +47,21 @@
         embed_dim,
         num_heads,
         bias=bias,
         kdim=kvdim,
         vdim=kvdim,
         batch_first=batch_first,
         device=DEVICE,
-        dtype=DTYPE,
     ).eval()
     if batch_first:
-        q = torch.randn(1, 16, embed_dim, device=DEVICE, dtype=DTYPE)
-        kv = torch.randn(1, 16, kvdim, device=DEVICE, dtype=DTYPE)
+        q = torch.randn(1, 16, embed_dim, device=DEVICE)
+        kv = torch.randn(1, 16, kvdim, device=DEVICE)
     else:
-        q = torch.randn(16, 1, embed_dim, device=DEVICE, dtype=DTYPE)
-        kv = torch.randn(16, 1, kvdim, device=DEVICE, dtype=DTYPE)
+        q = torch.randn(16, 1, embed_dim, device=DEVICE)
+        kv = torch.randn(16, 1, kvdim, device=DEVICE)
 
     y1, _ = model(q, kv, kv)
 
     lora = LoRA.from_module(model, rank=rank)
     lora.eval()
     y2, _ = lora(q, kv, kv)
     # By default, LoRA is initialized so that output is the same as the original model.
@@ -106,21 +101,21 @@
         partial(resnet18, weights=ResNet18_Weights.DEFAULT),
         partial(vit_b_32, weights=ViT_B_32_Weights.DEFAULT),
         # TODO: If we figure out how to use 'rank < groups' in LoRA, we can also
         # test models with grouped convolutions. e.g.:
         # partial(mobilenet_v3_small, weights=MobileNet_V3_Small_Weights.DEFAULT),
     ],
 )
-def vision_model(request: FixtureRequest) -> Generator[nn.Module, None, None]:
-    yield request.param().eval().to(device=DEVICE, dtype=DTYPE)
+def vision_model(request) -> Generator[nn.Module, None, None]:
+    yield request.param().eval().to(DEVICE)
 
 
 @torch.no_grad()
 def test_vision_model(vision_model: nn.Module, rank: int):
-    x = torch.randn(1, 3, 224, 224, device=DEVICE, dtype=DTYPE)
+    x = torch.randn(1, 3, 224, 224, device=DEVICE)
     y1 = vision_model(x)
 
     lora = LoRA.from_module(vision_model, rank=rank)
     lora.eval()
     y2 = lora(x)
     # By default, LoRA is initialized so that output is the same as the original model.
     assert torch.allclose(y1, y2)
@@ -132,78 +127,89 @@
 
     lora.disable_lora()
     y4 = lora(x)
     assert torch.allclose(y1, y4, atol=1e-5)
 
     lora.enable_lora()
     y5 = lora(x)
-    torch.testing.assert_allclose(y3, y5, rtol=1e-4, atol=1e-4)
+    assert torch.allclose(y3, y5, atol=1e-4)
 
     merged = lora.merge_lora(inplace=False)
     assert not isinstance(merged, LoRA)
     y6 = merged(x)
-    torch.testing.assert_allclose(y5, y6, rtol=1e-4, atol=1e-4)
+    assert torch.allclose(y5, y6, atol=1e-4)
 
     lora_copy = deepcopy(lora)
     merged2 = lora_copy.merge_lora(inplace=True)
     assert not isinstance(merged2, LoRA)
     y7 = merged2(x)
     assert torch.allclose(y5, y7, atol=1e-4)
 
     removed = lora.remove_lora()
     y8 = removed(x)
     assert torch.allclose(y1, y8, atol=1e-4)
 
 
-@pytest.fixture(
-    params=[XLMR_BASE_ENCODER],
-)
-def text_model(
-    request,
-) -> Generator[Tuple[nn.Module, Callable[[str], Tensor]], None, None]:
-    bundle = request.param
-    model = bundle.get_model().eval().to(DEVICE)
-    transform = bundle.transform()
-    yield model, transform
-
-
-@torch.no_grad()
-def test_text_model(text_model: Tuple[nn.Module, Callable[[str], Tensor]], rank: int):
-    model, transform = text_model
-    texts = ["Hello, world!"]
-    x = to_tensor(transform(texts)).to(DEVICE)
-
-    y1 = model(x)
+# TODO: After enabling "fast path" for TransformerEncoder and TransformerDecoder
+# in LoRA, we can test these models.
 
-    lora = LoRA.from_module(model, rank=rank)
-    lora.eval()
-    y2 = lora(x)
-    # By default, LoRA is initialized so that output is the same as the original model
-    assert torch.allclose(y1, y2)
-    # In order to test enable/disable/remove/merge functions, we need to randomly
-    # initialize the LoRA weights, so that the outputs are different.
-    _init_random_lora_module(lora)
-    y3 = lora(x)
-    assert not torch.allclose(y1, y3, atol=1e-5)
+# from typing import Callable, Generator, Tuple
 
-    lora.disable_lora()
-    y4 = lora(x)
-    assert torch.allclose(y1, y4, atol=1e-5)
-
-    lora.enable_lora()
-    y5 = lora(x)
-    assert torch.allclose(y3, y5, atol=1e-4)
-
-    merged = lora.merge_lora(inplace=False)
-    assert not isinstance(merged, LoRA)
-    y6 = merged(x)
-    assert torch.allclose(y5, y6, atol=1e-4)
-
-    lora_copy = deepcopy(lora)
-    merged2 = lora_copy.merge_lora(inplace=True)
-    assert not isinstance(merged2, LoRA)
-    y7 = merged2(x)
-    assert torch.allclose(y5, y7, atol=1e-4)
-
-    removed = lora.remove_lora()
-    y8 = removed(x)
-    assert torch.allclose(y1, y8, atol=1e-4)
+# import pytest
+# import torch
+# from torch import Tensor, nn
+# from torchtext.functional import to_tensor
+# from torchtext.models import XLMR_BASE_ENCODER
+
+# @pytest.fixture(
+#     params=[XLMR_BASE_ENCODER],
+# )
+# def text_model(
+#     request,
+# ) -> Generator[Tuple[nn.Module, Callable[[str], Tensor]], None, None]:
+#     bundle = request.param
+#     model = bundle.get_model().eval().to(DEVICE)
+#     transform = bundle.transform()
+#     yield model, transform
+
+
+# @torch.no_grad()
+# def test_text_model(text_model: Tuple[nn.Module, Callable[[str], Tensor]], rank: int):
+#     model, transform = text_model
+#     texts = ["Hello, world!"]
+#     x = to_tensor(transform(texts)).to(DEVICE)
+
+#     y1 = model(x)
+
+#     lora = LoRA.from_module(model, rank=rank)
+#     lora.eval()
+#     y2 = lora(x)
+#     # By default, LoRA is initialized so that output is the same as the original model.
+#     assert torch.allclose(y1, y2)
+#     # In order to test enable/disable/remove/merge functions, we need to randomly
+#     # initialize the LoRA weights, so that the outputs are different.
+#     _init_random_lora_module(lora)
+#     y3 = lora(x)
+#     assert not torch.allclose(y1, y3, atol=1e-5)
+
+#     lora.disable_lora()
+#     y4 = lora(x)
+#     assert torch.allclose(y1, y4, atol=1e-5)
+
+#     lora.enable_lora()
+#     y5 = lora(x)
+#     assert torch.allclose(y3, y5, atol=1e-4)
+
+#     merged = lora.merge_lora(inplace=False)
+#     assert not isinstance(merged, LoRA)
+#     y6 = merged(x)
+#     assert torch.allclose(y5, y6, atol=1e-4)
+
+#     lora_copy = deepcopy(lora)
+#     merged2 = lora_copy.merge_lora(inplace=True)
+#     assert not isinstance(merged2, LoRA)
+#     y7 = merged2(x)
+#     assert torch.allclose(y5, y7, atol=1e-4)
+
+#     removed = lora.remove_lora()
+#     y8 = removed(x)
+#     assert torch.allclose(y1, y8, atol=1e-4)
```
