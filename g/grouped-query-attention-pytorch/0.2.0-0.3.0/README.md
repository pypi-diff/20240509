# Comparing `tmp/grouped_query_attention_pytorch-0.2.0.tar.gz` & `tmp/grouped_query_attention_pytorch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grouped_query_attention_pytorch-0.2.0.tar", last modified: Thu Aug  3 00:46:07 2023, max compression
+gzip compressed data, was "grouped_query_attention_pytorch-0.3.0.tar", last modified: Thu May  9 19:07:30 2024, max compression
```

## Comparing `grouped_query_attention_pytorch-0.2.0.tar` & `grouped_query_attention_pytorch-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.959612 grouped_query_attention_pytorch-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-08-03 00:46:07.959612 grouped_query_attention_pytorch-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)   335190 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/doc/attention.png
--rw-r--r--   0 runner    (1001) docker     (123)    37835 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/doc/benchmark_attention.png
--rw-r--r--   0 runner    (1001) docker     (123)    37657 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/doc/benchmark_t5.png
--rw-r--r--   0 runner    (1001) docker     (123)   118342 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/doc/benchmark_t5_original.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/utils/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-08-03 00:46:07.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-03 00:46:07.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:46:07.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-03 00:46:07.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 00:46:07.000000 grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.955612 grouped_query_attention_pytorch-0.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/scripts/benchmark_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/scripts/benchmark_t5.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 00:46:07.959612 grouped_query_attention_pytorch-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:46:07.959612 grouped_query_attention_pytorch-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/tests/test_t5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-03 00:45:52.000000 grouped_query_attention_pytorch-0.2.0/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:07:30.432461 grouped_query_attention_pytorch-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:07:30.424461 grouped_query_attention_pytorch-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:07:30.424461 grouped_query_attention_pytorch-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-09 19:07:30.432461 grouped_query_attention_pytorch-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:07:30.428461 grouped_query_attention_pytorch-0.3.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)   335190 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/doc/attention.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37835 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/doc/benchmark_attention.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37657 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/doc/benchmark_t5.png
+-rw-r--r--   0 runner    (1001) docker     (127)   118342 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/doc/benchmark_t5_original.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:07:30.428461 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:07:30.428461 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch/utils/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:07:30.428461 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-09 19:07:30.000000 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-09 19:07:30.000000 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 19:07:30.000000 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-09 19:07:30.000000 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 19:07:30.000000 grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:07:30.428461 grouped_query_attention_pytorch-0.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/scripts/benchmark_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/scripts/benchmark_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 19:07:30.432461 grouped_query_attention_pytorch-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:07:30.428461 grouped_query_attention_pytorch-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/tests/test_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-09 19:07:24.000000 grouped_query_attention_pytorch-0.3.0/tests/test_transformer.py
```

### Comparing `grouped_query_attention_pytorch-0.2.0/.github/workflows/publish.yaml` & `grouped_query_attention_pytorch-0.3.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/.github/workflows/test.yaml` & `grouped_query_attention_pytorch-0.3.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/.gitignore` & `grouped_query_attention_pytorch-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/LICENSE` & `grouped_query_attention_pytorch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/PKG-INFO` & `grouped_query_attention_pytorch-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: grouped_query_attention_pytorch
-Version: 0.2.0
-Summary: grouped-query-attention-pytorch
-Author-email: Frank Odom <frank.odom.iii@gmail.com>
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: t5
-License-File: LICENSE
-
 # grouped-query-attention-pytorch
 
 (Unofficial) PyTorch implementation of grouped-query attention (GQA) from [GQA: Training Generalized Multi-Query Transformer Models from Multi-Head Checkpoints](https://arxiv.org/pdf/2305.13245.pdf)
 
 <img src="doc/attention.png" alt="compare-attention-mechanisms" width="600"/>
 
 ### Includes:
```

### Comparing `grouped_query_attention_pytorch-0.2.0/README.md` & `grouped_query_attention_pytorch-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: grouped_query_attention_pytorch
+Version: 0.3.0
+Summary: grouped-query-attention-pytorch
+Author-email: Frank Odom <frank.odom.iii@gmail.com>
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: einops~=0.6.0
+Requires-Dist: torch>=1.8.0
+Requires-Dist: torchscale~=0.2.0
+Provides-Extra: test
+Requires-Dist: black; extra == "test"
+Requires-Dist: kaleido; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: plotly; extra == "test"
+Requires-Dist: pre-commit; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: ruff; extra == "test"
+Requires-Dist: xformers==0.0.20; extra == "test"
+Provides-Extra: t5
+Requires-Dist: sentencepiece; extra == "t5"
+Requires-Dist: transformers<4.32,>=4.5.0; extra == "t5"
+
 # grouped-query-attention-pytorch
 
 (Unofficial) PyTorch implementation of grouped-query attention (GQA) from [GQA: Training Generalized Multi-Query Transformer Models from Multi-Head Checkpoints](https://arxiv.org/pdf/2305.13245.pdf)
 
 <img src="doc/attention.png" alt="compare-attention-mechanisms" width="600"/>
 
 ### Includes:
```

### Comparing `grouped_query_attention_pytorch-0.2.0/doc/attention.png` & `grouped_query_attention_pytorch-0.3.0/doc/attention.png`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/doc/benchmark_attention.png` & `grouped_query_attention_pytorch-0.3.0/doc/benchmark_attention.png`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/doc/benchmark_t5.png` & `grouped_query_attention_pytorch-0.3.0/doc/benchmark_t5.png`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/doc/benchmark_t5_original.png` & `grouped_query_attention_pytorch-0.3.0/doc/benchmark_t5_original.png`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/attention.py` & `grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch/attention.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,66 +81,54 @@
         )
 
     if scale is None:
         scale = query.size(-1) ** 0.5
     query = query / scale
 
     num_head_groups = hq // hk
-    if num_head_groups > 1 or force_grouped:
-        # Separate the query heads into 'num_head_groups' chunks, and fold the group
-        # dimension into the batch dimension.  This allows us to compute the attention
-        # for each head in parallel, then sum over all of the groups at the end.
-        query = rearrange(query, "b (h g) n d -> b g h n d", g=num_head_groups)
-        similarity = einsum(query, key, "b g h n d, b h s d -> b h n s")
-    else:
-        # If the number of query/key heads is equal, we can skip grouping the queries,
-        # and just use the standard sdot product attention.
-        similarity = einsum(query, key, "b h n d, b h s d -> b h n s")
+    query = rearrange(query, "b (h g) n d -> b g h n d", g=num_head_groups)
+    similarity = einsum(query, key, "b g h n d, b h s d -> b g h n s")
 
     if is_causal:
         # Mask out the upper triangular portion of the attention matrix. This prevents
         # the model from attending to tokens in the future.
-        mask = torch.ones(
-            (bq, nq, nk),
-            device=query.device,
-            dtype=torch.bool,
-        ).tril_()
+        mask = torch.ones((bq, nq, nk), device=query.device, dtype=torch.bool).tril_()
 
     if mask is not None:
         # Expand mask to match the shape of the attention matrix.
         # If mask is 2D, assume that it is applied to the key/value sequence dimension.
         # Else if mask is 3D, assume that it is applied to the query/key/value sequence
         # dimension for all attention heads.
         #
         # Users could also provide a 4D mask, which is applied to the query/key/value
         # sequence dimension for each attention head (though I don't have a particular
         # use case in mind for that).
         if mask.ndim == 2:
-            mask = rearrange(mask, "b s -> b () () s")
+            mask = rearrange(mask, "b s -> b () () () s")
         elif mask.ndim == 3:
-            mask = rearrange(mask, "b n s -> b () n s")
+            mask = rearrange(mask, "b n s -> b () () n s")
         # Mask similarity values by setting them to negative infinity.  This guarantees
         # that they will not contribute to the softmax computation below.
         similarity.masked_fill_(~mask, torch.finfo(similarity.dtype).min)
 
-    attention = F.softmax(similarity / scale, dim=-1)
+    attention = F.softmax(similarity, dim=-1)
     if dropout > 0.0:
         attention = F.dropout(attention, p=dropout)
 
     # Apply attention matrix to the value Tensor.
-    out = einsum(attention, value, "b h n s, b h s d -> b h n d")
+    out = einsum(attention, value, "b g h n s, b h s d -> b g h n d")
     # Move head dimension back to axis 2
-    out = rearrange(out, "b h n d -> b n h d")
+    out = rearrange(out, "b g h n d -> b n (h g) d")
 
     attn_weights: Optional[Tensor] = None
     if need_weights:
         # Move the sequence dimensions back to positions 1, 2.  Move the head dimension
         # to position 3.  This more closely matches the return shape of the attention
         # output: (b, n, h, d).
-        attn_weights = rearrange(attention, "b h n s -> b n s h")
+        attn_weights = rearrange(attention, "b g h n s -> b n s (h g)")
         if average_attn_weights:
             attn_weights = attn_weights.mean(dim=1)
 
     return out, attn_weights
 
 
 class MultiheadGQA(nn.Module):
@@ -218,21 +206,21 @@
         )
         self.v_proj = nn.Linear(
             embed_dim, kv_embed_dim, bias=bias, device=device, dtype=dtype
         )
         self.norm: Optional[nn.LayerNorm] = None
         if layer_norm:
             self.norm = nn.LayerNorm(
-                kv_embed_dim, eps=layer_norm_eps, device=device, dtype=dtype
+                embed_dim, eps=layer_norm_eps, device=device, dtype=dtype
             )
         # Grouped attention output will have the same embedding dimension as the
         # key/value Tensors.  So the output projection layer needs to accept the
         # same dimension (kv_embed_dim).
         self.out_proj = nn.Linear(
-            kv_embed_dim, embed_dim, bias=bias, device=device, dtype=dtype
+            embed_dim, embed_dim, bias=bias, device=device, dtype=dtype
         )
 
         self._reset_parameters()
 
     def _reset_parameters(self):
         nn.init.xavier_normal_(self.q_proj.weight)
         if self.q_proj.bias is not None:
```

### Comparing `grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/t5.py` & `grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/transformer.py` & `grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch/transformer.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch/utils/benchmark.py` & `grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/PKG-INFO` & `grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 Metadata-Version: 2.1
-Name: grouped-query-attention-pytorch
-Version: 0.2.0
+Name: grouped_query_attention_pytorch
+Version: 0.3.0
 Summary: grouped-query-attention-pytorch
 Author-email: Frank Odom <frank.odom.iii@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: einops~=0.6.0
+Requires-Dist: torch>=1.8.0
+Requires-Dist: torchscale~=0.2.0
 Provides-Extra: test
+Requires-Dist: black; extra == "test"
+Requires-Dist: kaleido; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: plotly; extra == "test"
+Requires-Dist: pre-commit; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: ruff; extra == "test"
+Requires-Dist: xformers==0.0.20; extra == "test"
 Provides-Extra: t5
-License-File: LICENSE
+Requires-Dist: sentencepiece; extra == "t5"
+Requires-Dist: transformers<4.32,>=4.5.0; extra == "t5"
 
 # grouped-query-attention-pytorch
 
 (Unofficial) PyTorch implementation of grouped-query attention (GQA) from [GQA: Training Generalized Multi-Query Transformer Models from Multi-Head Checkpoints](https://arxiv.org/pdf/2305.13245.pdf)
 
 <img src="doc/attention.png" alt="compare-attention-mechanisms" width="600"/>
```

### Comparing `grouped_query_attention_pytorch-0.2.0/grouped_query_attention_pytorch.egg-info/SOURCES.txt` & `grouped_query_attention_pytorch-0.3.0/grouped_query_attention_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/pyproject.toml` & `grouped_query_attention_pytorch-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     "pytest",
     "pytest-cov",
     "ruff",
     "xformers==0.0.20",
 ]
 t5 = [
     "sentencepiece",
-    "transformers>=4.5.0",
+    "transformers>=4.5.0,<4.32",
 ]
 
 [project.scripts]
 # Entrypoint scripts
 
 
 # ----- Linting, Formatting, and Typing -----
```

### Comparing `grouped_query_attention_pytorch-0.2.0/scripts/README.md` & `grouped_query_attention_pytorch-0.3.0/scripts/README.md`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/scripts/benchmark_attention.py` & `grouped_query_attention_pytorch-0.3.0/scripts/benchmark_attention.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/scripts/benchmark_t5.py` & `grouped_query_attention_pytorch-0.3.0/scripts/benchmark_t5.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/tests/conftest.py` & `grouped_query_attention_pytorch-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/tests/test_t5.py` & `grouped_query_attention_pytorch-0.3.0/tests/test_t5.py`

 * *Files identical despite different names*

### Comparing `grouped_query_attention_pytorch-0.2.0/tests/test_transformer.py` & `grouped_query_attention_pytorch-0.3.0/tests/test_transformer.py`

 * *Files identical despite different names*

