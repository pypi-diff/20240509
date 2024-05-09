# Comparing `tmp/mlx_embedding_models-0.0.8.tar.gz` & `tmp/mlx_embedding_models-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_embedding_models-0.0.8.tar", last modified: Tue May  7 16:56:02 2024, max compression
+gzip compressed data, was "mlx_embedding_models-0.0.9.tar", last modified: Thu May  9 16:06:04 2024, max compression
```

## Comparing `mlx_embedding_models-0.0.8.tar` & `mlx_embedding_models-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-05-07 16:56:02.308948 mlx_embedding_models-0.0.8/
--rw-r--r--   0 benjamin   (501) staff       (20)     1066 2024-02-10 06:19:21.000000 mlx_embedding_models-0.0.8/LICENSE
--rw-r--r--   0 benjamin   (501) staff       (20)     1022 2024-05-07 16:56:02.308778 mlx_embedding_models-0.0.8/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      608 2024-02-11 19:46:40.000000 mlx_embedding_models-0.0.8/README.md
--rw-r--r--   0 benjamin   (501) staff       (20)      463 2024-05-07 16:55:55.000000 mlx_embedding_models-0.0.8/pyproject.toml
--rw-r--r--   0 benjamin   (501) staff       (20)       38 2024-05-07 16:56:02.308992 mlx_embedding_models-0.0.8/setup.cfg
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-05-07 16:56:02.305755 mlx_embedding_models-0.0.8/src/
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-05-07 16:56:02.307611 mlx_embedding_models-0.0.8/src/mlx_embedding_models/
--rw-r--r--   0 benjamin   (501) staff       (20)    12078 2024-05-07 03:44:29.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models/embedding.py
--rw-r--r--   0 benjamin   (501) staff       (20)     4879 2024-03-18 17:56:39.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models/load_utils.py
--rw-r--r--   0 benjamin   (501) staff       (20)     7194 2024-03-08 00:29:04.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models/model.py
--rw-r--r--   0 benjamin   (501) staff       (20)     9624 2024-05-07 16:55:04.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models/nomic_model.py
--rw-r--r--   0 benjamin   (501) staff       (20)     3548 2024-05-03 20:33:59.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models/registry.py
--rw-r--r--   0 benjamin   (501) staff       (20)        0 2024-03-17 17:34:49.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models/test_mteb.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-05-07 16:56:02.308570 mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/
--rw-r--r--   0 benjamin   (501) staff       (20)     1022 2024-05-07 16:56:02.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      497 2024-05-07 16:56:02.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2024-05-07 16:56:02.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       55 2024-05-07 16:56:02.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/requires.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       21 2024-05-07 16:56:02.000000 mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-05-09 16:06:04.043059 mlx_embedding_models-0.0.9/
+-rw-r--r--   0 benjamin   (501) staff       (20)     1066 2024-02-10 06:19:21.000000 mlx_embedding_models-0.0.9/LICENSE
+-rw-r--r--   0 benjamin   (501) staff       (20)     1022 2024-05-09 16:06:04.042821 mlx_embedding_models-0.0.9/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      608 2024-02-11 19:46:40.000000 mlx_embedding_models-0.0.9/README.md
+-rw-r--r--   0 benjamin   (501) staff       (20)      463 2024-05-09 16:05:43.000000 mlx_embedding_models-0.0.9/pyproject.toml
+-rw-r--r--   0 benjamin   (501) staff       (20)       38 2024-05-09 16:06:04.043105 mlx_embedding_models-0.0.9/setup.cfg
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-05-09 16:06:04.040324 mlx_embedding_models-0.0.9/src/
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-05-09 16:06:04.041644 mlx_embedding_models-0.0.9/src/mlx_embedding_models/
+-rw-r--r--   0 benjamin   (501) staff       (20)    12558 2024-05-09 15:58:24.000000 mlx_embedding_models-0.0.9/src/mlx_embedding_models/embedding.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     4879 2024-03-18 17:56:39.000000 mlx_embedding_models-0.0.9/src/mlx_embedding_models/load_utils.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     6337 2024-05-09 16:05:37.000000 mlx_embedding_models-0.0.9/src/mlx_embedding_models/model.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     8065 2024-05-09 15:58:24.000000 mlx_embedding_models-0.0.9/src/mlx_embedding_models/nomic_model.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     3574 2024-05-09 15:58:24.000000 mlx_embedding_models-0.0.9/src/mlx_embedding_models/registry.py
+-rw-r--r--   0 benjamin   (501) staff       (20)        0 2024-03-17 17:34:49.000000 mlx_embedding_models-0.0.9/src/mlx_embedding_models/test_mteb.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2024-05-09 16:06:04.042575 mlx_embedding_models-0.0.9/src/mlx_embedding_models.egg-info/
+-rw-r--r--   0 benjamin   (501) staff       (20)     1022 2024-05-09 16:06:04.000000 mlx_embedding_models-0.0.9/src/mlx_embedding_models.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      497 2024-05-09 16:06:04.000000 mlx_embedding_models-0.0.9/src/mlx_embedding_models.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        1 2024-05-09 16:06:04.000000 mlx_embedding_models-0.0.9/src/mlx_embedding_models.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       55 2024-05-09 16:06:04.000000 mlx_embedding_models-0.0.9/src/mlx_embedding_models.egg-info/requires.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       21 2024-05-09 16:06:04.000000 mlx_embedding_models-0.0.9/src/mlx_embedding_models.egg-info/top_level.txt
```

### Comparing `mlx_embedding_models-0.0.8/LICENSE` & `mlx_embedding_models-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_embedding_models-0.0.8/PKG-INFO` & `mlx_embedding_models-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx_embedding_models
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python utility for text embeddings in MLX.
 Author-email: Benjamin Anderson <ben@trytaylor.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: transformers
```

### Comparing `mlx_embedding_models-0.0.8/README.md` & `mlx_embedding_models-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mlx_embedding_models-0.0.8/src/mlx_embedding_models/embedding.py` & `mlx_embedding_models-0.0.9/src/mlx_embedding_models/embedding.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 def pool(
     pooling_strategy: Literal["mean", "cls", "first", "max"],
     normalize: bool,
     last_hidden_state: mx.array,  # B, L, D
     pooler_output: Optional[mx.array] = None,  # B, D
     mask: Optional[mx.array] = None,  # B, L
+    apply_ln: bool = False,
+    dimension: int = None
 ) -> mx.array:
     """
     Pool output fron a sentence transformer model into one embedding.
     Use MLX tensors as input, return MLX tensor as output.
     : last_hidden_state: B, L, D
     : pooler_output: B, D
     : mask: B, L
@@ -45,14 +47,21 @@
             pooled = last_hidden_state[:, 0, :]
         else:
             pooled = pooler_output
     else:
         raise NotImplementedError(
             f"pooling strategy {pooling_strategy} not implemented"
         )
+    if apply_ln:
+        pooled = mx.fast.layer_norm(pooled, None, None, 1e-5)
+
+    if dimension is not None:
+        # truncate if trained with matryoshka
+        pooled = pooled[:, :dimension]
+
     if normalize:
         pooled = pooled / mx.linalg.norm(pooled, axis=-1, keepdims=True)
 
     return pooled
 
 class EmbeddingModel:
     """
@@ -63,37 +72,41 @@
         self,
         model_path: str,
         pooling_strategy: Literal["mean", "cls", "first", "max"],
         normalize: bool,
         max_length: int,
         nomic_bert: bool = False,
         lm_head: bool = False,
+        apply_ln: bool = False,
     ):
         if nomic_bert:
             self.model = NomicBert.from_pretrained(model_path, lm_head=lm_head)
         else:
             self.model = Bert.from_pretrained(model_path, lm_head=lm_head)
         self.tokenizer = AutoTokenizer.from_pretrained(model_path)
         self.pooling_strategy = pooling_strategy
         self.normalize = normalize
         self.max_length = max_length
 
+        self.apply_ln = apply_ln
+
     @classmethod
     def from_registry(cls, model_name: str):
         """
         Initialize from the model registry.
         """
         model_config = registry[model_name]
         return cls(
             model_path=model_config["repo"],
             pooling_strategy=model_config["pooling_strategy"],
             normalize=model_config["normalize"],
             max_length=model_config["max_length"],
             lm_head=model_config.get("lm_head", False),
             nomic_bert="nomic" in model_name,
+            apply_ln=model_config.get("apply_ln", False),
         )
     
     def _tokenize(
         self, 
         sentences,
         min_length: Optional[int] = None # if provided, we add [MASK] tokens to short queries
     ) -> ak.Array:
@@ -245,15 +258,17 @@
                 last_hidden_state, pooler_output = self.model(**batch)
                 # TODO: pooling bug due to not using mask
                 embs = pool(
                     self.pooling_strategy,
                     self.normalize,
                     last_hidden_state,
                     pooler_output,
-                    mask=batch.get("attention_mask", None)
+                    mask=batch.get("attention_mask", None),
+                    apply_ln=self.apply_ln,
+                    dimension=kwargs.get("dimension", None),
                 )
                 mx.eval(embs)
                 output_embeddings.append(embs)
                 pbar.update(len(batch["input_ids"]))
                 del batch
             # we're done with this seqlen, clear the cache
             mx.metal.clear_cache()
```

### Comparing `mlx_embedding_models-0.0.8/src/mlx_embedding_models/load_utils.py` & `mlx_embedding_models-0.0.9/src/mlx_embedding_models/load_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_embedding_models-0.0.8/src/mlx_embedding_models/model.py` & `mlx_embedding_models-0.0.9/src/mlx_embedding_models/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,43 +2,17 @@
 # https://github.com/ml-explore/mlx-examples
 
 import tempfile
 from typing import Tuple, Union, Optional
 import mlx.core as mx
 import mlx.nn as nn
 import numpy as np
-from transformers import AutoConfig, BertConfig, RobertaConfig, DistilBertConfig
+from transformers import AutoConfig, BertConfig, RobertaConfig, DistilBertConfig, XLMRobertaConfig
 from .load_utils import convert, convert_distilbert, bert_config_from_distilbert
 
-
-# class FastAttention(nn.Module):
-#     def __init__(self, config: Union[BertConfig, RobertaConfig]):
-#         super().__init__()
-#         self.num_heads = config.num_attention_heads
-#         self.query_proj = nn.Linear(config.hidden_size, config.hidden_size, bias=True)
-#         self.key_proj = nn.Linear(config.hidden_size, config.hidden_size, bias=True)
-#         self.value_proj = nn.Linear(config.hidden_size, config.hidden_size, bias=True)
-#         self.out_proj = nn.Linear(config.hidden_size, config.hidden_size, bias=True)
-#         self.scale = 1 / (config.hidden_size ** 0.5)
-    
-#     def shape(self, tensor: mx.array):
-#         B, L, D = tensor.shape
-#         tensor = tensor.reshape(B, L, self.num_heads, D // self.num_heads)
-#         return tensor.transpose(0, 2, 1, 3)
-
-#     def __call__(self, x, mask):
-#         q = self.query_proj(x)
-#         k = self.key_proj(x)
-#         v = self.value_proj(x)
-#         q, k, v = map(self.shape, (q, k, v))
-#         attn_out = mx.fast.scaled_dot_product_attention(
-#             q, k, v, mask, self.scale
-#         )
-#         return self.out_proj(attn_out)
-
 class TransformerEncoderLayer(nn.Module):
     """
     A transformer encoder layer with (the original BERT) post-normalization.
     """
 
     def __init__(
         self,
@@ -173,14 +147,19 @@
         elif isinstance(config, RobertaConfig):
             config = RobertaConfig.from_pretrained(model_path)
             tensors = convert(model_path, lm_head=lm_head)
         elif isinstance(config, DistilBertConfig):
             config = DistilBertConfig.from_pretrained(model_path)
             config = bert_config_from_distilbert(config)
             tensors = convert_distilbert(model_path, lm_head=lm_head)
+        elif isinstance(config, XLMRobertaConfig):
+            config = XLMRobertaConfig.from_pretrained(model_path)
+            tensors = convert(model_path, lm_head=lm_head)
+        else:
+            raise ValueError(f"Config {config} not supported")
         model = cls(config, lm_head=lm_head)
 
         # print all keys in model
         # print(model)
         
         # use npz extension
         with tempfile.NamedTemporaryFile(suffix=".npz") as f:
```

### Comparing `mlx_embedding_models-0.0.8/src/mlx_embedding_models/nomic_model.py` & `mlx_embedding_models-0.0.9/src/mlx_embedding_models/nomic_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -61,78 +61,29 @@
 
     def __call__(self, x):
         y = self.fc11(x)
         gate = self.fc12(x)
         y = y * self.activation(gate)
         y = self.fc2(y)
         return y
-
-
-class NomicRoPE(nn.Module):
-    def __init__(self, dims, base=10000.0, scale=1.0, offset=0):
-        super().__init__()
-        self.dims = dims
-        self.base = base
-        self.scale = scale
-        self.offset = offset
-        
-    def __call__(self, x, offset=0):
-        if x.ndim < 3:
-            raise ValueError(f"[rope] Input must have at least 3 dimensions but got input with {x.ndim} dimensions.")
-
-        scale = self.scale
-        base = self.base
-        dims = self.dims
-
-        
-        shape = x.shape
-        N = x.shape[1] + offset
-        
-        # Compute sines and cosines
-        half_dims = dims // 2
-        positions = mx.arange(offset, N, dtype=x.dtype) * scale
-        freqs = mx.arange(0, half_dims, dtype=x.dtype)
-        freqs = mx.exp(-freqs * mx.array(base).log() / half_dims)
-        theta = mx.expand_dims(positions, 1) * mx.expand_dims(freqs, 0)
-        coss = mx.cos(theta)
-        sins = mx.sin(theta)
-
-        def rotate_half(x):
-            x1, x2 = mx.split(x, 2, axis=-1)
-            return mx.concatenate((-x2, x1), axis=-1)
-        
-        def apply_rope(x, coss, sins):
-            return x * coss + rotate_half(x) * sins
-        
-        out_s = list(x.shape)
-        out_s[-1] = half_dims
-        out_s[-1] = dims
-        repeated_cos = mx.tile(coss, (1, 2))
-        coss = repeated_cos.reshape(coss.shape[:-1] + (1, 2 * coss.shape[-1]))
-
-        repeated_sin = mx.tile(sins, (1, 2))
-        sins = repeated_sin.reshape(sins.shape[:-1] + (1, 2 * sins.shape[-1]))
-        
-        out = apply_rope(x, coss, sins)
-        
-        return mx.reshape(out, shape)
     
 class NomicBertAttention(nn.Module):
     def __init__(self, config: AutoConfig):
         super().__init__()
         self.embed_dim = config.n_embd
         self.num_heads = config.n_head
         assert self.embed_dim % self.num_heads == 0, "embed_dim must be divisible by num_heads"
         self.head_dim = self.embed_dim // self.num_heads
         self.norm_factor = math.sqrt(self.head_dim)
         self.rotary_emb_dim = int(self.head_dim * config.rotary_emb_fraction)
         
         if self.rotary_emb_dim > 0:
-            self.rotary_emb = NomicRoPE(
+            self.rotary_emb = nn.RoPE(
                 dims=self.rotary_emb_dim,
+                traditional=config.rotary_emb_interleaved,
                 base=config.rotary_emb_base, # increase to extrapolate to docs > 2048 tokens
                 scale=1.0
             )
         self.Wqkv = nn.Linear(config.n_embd, 3 * config.n_embd, bias=config.qkv_proj_bias)
         self.out_proj = nn.Linear(config.n_embd, config.n_embd, bias=config.qkv_proj_bias)
     
     @staticmethod
@@ -145,19 +96,19 @@
     
     def __call__(self, x, mask):
         qkv = self.Wqkv(x)
         B, S, _ = qkv.shape
         qkv = qkv.reshape(B, S, 3, self.num_heads, self.head_dim)
         q, k, v = qkv[:, :, 0], qkv[:, :, 1], qkv[:, :, 2] # b, s, h, d
 
+        q, k, v = map(self.shape, (q, k, v)) # b, h, s, d
+
         if self.rotary_emb_dim > 0:
             q, k = self.rotary_emb(q), self.rotary_emb(k)
 
-        q, k, v = map(self.shape, (q, k, v)) # b, h, s, d
-
         attention_scores = q @ k.transpose(0, 1, 3, 2) / self.norm_factor
         if mask is not None:
             attention_scores += mask
 
         attentions_probs: mx.array = mx.softmax(attention_scores, axis=-1) # B, H, S, S
         attn_output = attentions_probs @ v
         attn_output = attn_output.transpose(0, 2, 1, 3).reshape(B, S, -1)
```

### Comparing `mlx_embedding_models-0.0.8/src/mlx_embedding_models/registry.py` & `mlx_embedding_models-0.0.9/src/mlx_embedding_models/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     },
     "nomic-text-v1.5": {
         "repo": "nomic-ai/nomic-embed-text-v1.5",
         "max_length": 2048,
         "pooling_strategy": "mean",
         "normalize": True,
         "ndim": 768,
+        "apply_ln": True,
     },
     # 24 layers, 1024-dim
     "bge-large": {
         "repo": "BAAI/bge-large-en-v1.5",
         "max_length": 512,
         "pooling_strategy": "first",
         "normalize": True,
```

### Comparing `mlx_embedding_models-0.0.8/src/mlx_embedding_models.egg-info/PKG-INFO` & `mlx_embedding_models-0.0.9/src/mlx_embedding_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx_embedding_models
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python utility for text embeddings in MLX.
 Author-email: Benjamin Anderson <ben@trytaylor.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: transformers
```

