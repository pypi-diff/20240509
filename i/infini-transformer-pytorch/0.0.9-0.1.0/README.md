# Comparing `tmp/infini_transformer_pytorch-0.0.9.tar.gz` & `tmp/infini_transformer_pytorch-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infini_transformer_pytorch-0.0.9.tar", last modified: Thu May  2 16:34:37 2024, max compression
+gzip compressed data, was "infini_transformer_pytorch-0.1.0.tar", last modified: Thu May  9 13:25:20 2024, max compression
```

## Comparing `infini_transformer_pytorch-0.0.9.tar` & `infini_transformer_pytorch-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:34:37.077998 infini_transformer_pytorch-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 16:34:32.000000 infini_transformer_pytorch-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 16:34:37.073998 infini_transformer_pytorch-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-02 16:34:32.000000 infini_transformer_pytorch-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:34:37.073998 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 16:34:32.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-02 16:34:32.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch/infini_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:34:37.073998 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 16:34:37.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-02 16:34:37.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:34:37.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 16:34:37.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 16:34:37.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:34:37.077998 infini_transformer_pytorch-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 16:34:32.000000 infini_transformer_pytorch-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:25:20.195657 infini_transformer_pytorch-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 13:25:16.000000 infini_transformer_pytorch-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-09 13:25:20.195657 infini_transformer_pytorch-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-09 13:25:16.000000 infini_transformer_pytorch-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:25:20.195657 infini_transformer_pytorch-0.1.0/infini_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-09 13:25:16.000000 infini_transformer_pytorch-0.1.0/infini_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-05-09 13:25:16.000000 infini_transformer_pytorch-0.1.0/infini_transformer_pytorch/infini_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-09 13:25:16.000000 infini_transformer_pytorch-0.1.0/infini_transformer_pytorch/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:25:20.195657 infini_transformer_pytorch-0.1.0/infini_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-09 13:25:20.000000 infini_transformer_pytorch-0.1.0/infini_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-09 13:25:20.000000 infini_transformer_pytorch-0.1.0/infini_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:25:20.000000 infini_transformer_pytorch-0.1.0/infini_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-09 13:25:20.000000 infini_transformer_pytorch-0.1.0/infini_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 13:25:20.000000 infini_transformer_pytorch-0.1.0/infini_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:25:20.195657 infini_transformer_pytorch-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-09 13:25:16.000000 infini_transformer_pytorch-0.1.0/setup.py
```

### Comparing `infini_transformer_pytorch-0.0.9/LICENSE` & `infini_transformer_pytorch-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.9/PKG-INFO` & `infini_transformer_pytorch-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.9
+Version: 0.1.0
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
@@ -13,7 +13,8 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: einops>=0.8.0
 Requires-Dist: rotary-embedding-torch>=0.5.3
 Requires-Dist: torch>=2.0
+Requires-Dist: tqdm
```

### Comparing `infini_transformer_pytorch-0.0.9/infini_transformer_pytorch/infini_transformer.py` & `infini_transformer_pytorch-0.1.0/infini_transformer_pytorch/infini_transformer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,124 @@
-from typing import Tuple, List, Optional
+from __future__ import annotations
+from typing import Tuple, List, NamedTuple
 
 import torch
 from torch import nn, Tensor
 import torch.nn.functional as F
 from torch.nn import Module, ModuleList
 
 from einops import einsum, rearrange, repeat, reduce
 from einops.layers.torch import Rearrange
 
 from rotary_embedding_torch import RotaryEmbedding
 
 # constants
 
-Memories = Tuple[Tensor, Tensor]
+class Memories(NamedTuple):
+    kv_mem: Tensor
+    k_norm: Tensor
+
+class TransformerReturn(NamedTuple):
+    logits: Tensor
+    cached_kvs: List[Tensor] | None
+    past_memories: List[Memories] | None
 
 # helpers
 
 def exists(v):
-    return v
+    return v is not None
 
 def default(v, d):
     return v if exists(v) else d
 
-def detach_memories_(memories: Memories):
+def detach_memories_(memories: List[Memories]):
     for (mem_kv, mem_norm) in memories:
         mem_kv.detach_()
         mem_norm.detach_()
 
+def detach_cached_kv_(cached_kvs: List[Tensor]):
+    for cached_kv in cached_kvs:
+        cached_kv.detach_()
+
 # classes
 
 class RMSNorm(Module):
     def __init__(self, dim):
         super().__init__()
         self.scale = dim ** 0.5
         self.gamma = nn.Parameter(torch.ones(dim))
 
     def forward(self, x):
         return F.normalize(x, dim = -1) * self.scale * self.gamma
 
 class FeedForward(Module):
-    def __init__(self, dim, mult = 4):
+    def __init__(
+        self,
+        dim,
+        mult = 4,
+        dropout = 0.
+    ):
         super().__init__()
         dim_inner = int(mult * dim * 2 / 3)
 
         self.norm = RMSNorm(dim)
         self.proj_in = nn.Linear(dim, dim_inner * 2)
         self.proj_out = nn.Linear(dim_inner, dim)
 
+        self.dropout = nn.Dropout(dropout)
+
     def forward(self, x):
         x = self.norm(x)
         x, gates = self.proj_in(x).chunk(2, dim = -1)
         x = F.gelu(gates) * x
+        x = self.dropout(x)
         return self.proj_out(x)
 
 # attention
 
 class CausalAttention(Module):
     def __init__(
         self,
         dim,
         *,
         dim_head = 128,
         heads = 8,
+        dropout = 0.,
         head_gate_init_value = 10.,
         use_mem_delta_rule = False,
         rotary_emb_linear_attn = False    # unsure whether to apply rotary embeddings to linear attention, so make it an option
     ):
         super().__init__()
         dim_inner = dim_head * heads
         self.scale = dim_head ** -0.5
         self.norm = RMSNorm(dim)
 
         self.rotary_emb = RotaryEmbedding(dim_head)
 
         self.to_qkv = nn.Linear(dim, dim_inner * 3, bias = False)
         self.to_out = nn.Linear(dim_inner, dim, bias = False)
 
+        self.dropout = nn.Dropout(dropout)
+
         self.split_heads = Rearrange('b n (qkv h d) -> qkv b h n d', qkv = 3, h = heads)
         self.merge_heads = Rearrange('b h n d -> b n (h d)')
 
         self.head_gates = nn.Parameter(torch.ones(heads) * head_gate_init_value)
 
         self.use_mem_delta_rule = use_mem_delta_rule
         self.rotary_emb_linear_attn = rotary_emb_linear_attn
 
     def forward(
         self,
         x,
-        past_memories: Optional[Memories] = None,
+        cached_kv: Tensor | None = None,
+        past_memories: Memories | None = None,
+        return_new_memories = False,
         eps = 1e-10
-    ) -> Tuple[Tensor, Memories]:
+    ) -> Tuple[Tensor, Tensor, Memories]:
         """
         ein notation:
 
         b - batch
         h - heads
         n - sequence
         i - source sequence (q)
@@ -104,14 +129,25 @@
         """
 
         x = self.norm(x)
 
         x = self.to_qkv(x)
         q, k, v = self.split_heads(x)
 
+        # handle cached key / values
+
+        if exists(cached_kv):
+            cached_k, cached_v = cached_kv
+            k = torch.cat((cached_k, k), dim = -2)
+            v = torch.cat((cached_v, v), dim = -2)
+
+        # save original keys and values for cached kv
+
+        orig_k, orig_v = k, v
+
         # similarity
 
         q_scaled = q * self.scale
         q_rotated = self.rotary_emb.rotate_queries_or_keys(q_scaled)
         k_rotated = self.rotary_emb.rotate_queries_or_keys(k)
 
         sim = einsum(q_rotated, k_rotated, '... i d, ... j d -> ... i j')
@@ -122,14 +158,18 @@
         causal_mask = torch.ones((i, j), device = sim.device, dtype = torch.bool).triu(j - i + 1)
         sim = sim.masked_fill(causal_mask, -torch.finfo(sim.dtype).max)
 
         # attend
 
         attn = sim.softmax(dim = -1)
 
+        # dropout
+
+        attn = self.dropout(attn)
+
         # aggregate values
 
         out = einsum(attn, v, '... i j, ... j d -> ... i d')
 
         # the main contribution of the paper
         # Katharopoulos linear attention to kv memory of shape (batch, heads, dim keys, dim values)
         # it makes sense the author would try this, as he is ex-shmidhuber lab (linear transformers are fast weights paper)
@@ -160,14 +200,27 @@
             # in paper, they use a sigmoid gating scheme with learned gate per head
 
             gates = rearrange(self.head_gates, 'h -> h 1 1')
             gates = gates.sigmoid()
 
             out = out * gates + mem_out * (1. - gates)  # eq (6) - figure 3 shows how heads emergently specialize to look either at the present, past, or a bit of both
 
+        # merge heads and combine
+
+        out = self.merge_heads(out)
+        out = self.to_out(out)
+
+        # if new memories are not needed, early return
+        # at inference time, kv cache up to segment length and then compress memories into kv
+
+        if not return_new_memories:
+            cached_kv = torch.stack((orig_k, orig_v))
+
+            return out, cached_kv, past_memories
+
         # create the next memories
 
         if exists(past_memories) and self.use_mem_delta_rule:
             delta_v = retrieve_from_kv_memories(k, past_memories)
 
             # eq (5) - the delta rule
             v = v - delta_v
@@ -177,35 +230,32 @@
 
         if exists(past_memories):
             past_memories_kv, past_memories_norm = past_memories
 
             new_memories_kv = new_memories_kv + past_memories_kv          # eq (4)
             new_memories_norm = new_memories_norm + past_memories_norm    # eq (4)
 
-        new_memories = (new_memories_kv, new_memories_norm)
+        new_memories = Memories(new_memories_kv, new_memories_norm)
 
-        # merge heads and combine
-
-        out = self.merge_heads(out)
-        out = self.to_out(out)
-
-        return out, new_memories
+        return out, None, new_memories
 
 # main class
 
 class InfiniTransformer(Module):
     def __init__(
         self,
         *,
         num_tokens,
         dim,
         depth,
         dim_head = 128,
         heads = 8,
+        attn_dropout = 0.,
         ff_mult = 4,
+        ff_dropout = 0.,
         use_mem_delta_rule = False,     # in the paper, the delta rule didn't seem to do that much, but will include for completeness
         rotary_emb_linear_attn = False
     ):
         super().__init__()
 
         self.token_emb = nn.Embedding(num_tokens, dim)
 
@@ -214,52 +264,76 @@
         for _ in range(depth):
 
             attn = CausalAttention(
                 dim = dim,
                 dim_head = dim_head,
                 heads = heads,
                 use_mem_delta_rule = use_mem_delta_rule,
-                rotary_emb_linear_attn = rotary_emb_linear_attn
+                rotary_emb_linear_attn = rotary_emb_linear_attn,
+                dropout = attn_dropout
             )
 
             ff = FeedForward(
                 dim = dim,
-                mult = ff_mult
+                mult = ff_mult,
+                dropout = ff_dropout
             )
 
             self.layers.append(ModuleList([attn, ff]))
 
         self.norm = RMSNorm(dim)
         self.to_logits = nn.Linear(dim, num_tokens)
 
     def forward(
         self,
         x,
-        past_memories: Optional[List[Memories]] = None,
-        return_memories = False,
+        past_memories: List[Memories] | None = None,
+        cached_kv: List[Tensor] | None = None,
+        return_new_memories = False,
         detach_memories = False
-    ):
+    ) -> TransformerReturn:
+
         x = self.token_emb(x)
 
+        new_cached_kv = []
         new_memories = []
+
+        # iterators for cached key / values and past compressed memories
+
+        cached_kv_iter = iter(default(cached_kv, []))
         past_memories_iter = iter(default(past_memories, []))
 
+        # going through layers of infini-transformer
+
         for attn, ff in self.layers:
-            past_memories = next(past_memories_iter, None)
-            attn_out, layer_new_memories = attn(x, past_memories = past_memories)
+
+            attn_out, layer_cached_kv, layer_new_memories = attn(
+                x,
+                cached_kv = next(cached_kv_iter, None),
+                past_memories = next(past_memories_iter, None),
+                return_new_memories = return_new_memories
+            )
 
             x = attn_out + x
             x = ff(x) + x
 
+            new_cached_kv.append(layer_cached_kv)
             new_memories.append(layer_new_memories)
 
+        # final norm
+
         embed = self.norm(x)
 
+        # logits
+
         logits = self.to_logits(embed)
 
-        if not return_memories:
-            return logits
+        if detach_memories:
+            detach_cached_kv_(new_cached_kv)
+
+        if not return_new_memories:
+            return TransformerReturn(logits, new_cached_kv, past_memories)
 
         if detach_memories:
             detach_memories_(new_memories)
 
-        return logits, new_memories
+        return TransformerReturn(logits, None, new_memories)
```

### Comparing `infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/PKG-INFO` & `infini_transformer_pytorch-0.1.0/infini_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.9
+Version: 0.1.0
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
@@ -13,7 +13,8 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: einops>=0.8.0
 Requires-Dist: rotary-embedding-torch>=0.5.3
 Requires-Dist: torch>=2.0
+Requires-Dist: tqdm
```

### Comparing `infini_transformer_pytorch-0.0.9/setup.py` & `infini_transformer_pytorch-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'infini-transformer-pytorch',
   packages = find_packages(exclude = []),
-  version = '0.0.9',
+  version = '0.1.0',
   license='MIT',
   description = 'Infini-Transformer in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/infini-transformer-pytorch',
   keywords = [
@@ -18,14 +18,15 @@
     'long context',
     'memory'
   ],
   install_requires=[
     'einops>=0.8.0',
     'rotary-embedding-torch>=0.5.3',
     'torch>=2.0',
+    'tqdm'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.7',
```

