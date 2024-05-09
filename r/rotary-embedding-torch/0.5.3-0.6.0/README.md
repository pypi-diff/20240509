# Comparing `tmp/rotary-embedding-torch-0.5.3.tar.gz` & `tmp/rotary_embedding_torch-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotary-embedding-torch-0.5.3.tar", last modified: Tue Dec 26 02:00:03 2023, max compression
+gzip compressed data, was "rotary_embedding_torch-0.6.0.tar", last modified: Thu May  9 14:26:52 2024, max compression
```

## Comparing `rotary-embedding-torch-0.5.3.tar` & `rotary_embedding_torch-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 02:00:03.825788 rotary-embedding-torch-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-26 01:59:52.000000 rotary-embedding-torch-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-26 02:00:03.825788 rotary-embedding-torch-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2023-12-26 01:59:52.000000 rotary-embedding-torch-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 02:00:03.821788 rotary-embedding-torch-0.5.3/rotary_embedding_torch/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-26 01:59:52.000000 rotary-embedding-torch-0.5.3/rotary_embedding_torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2023-12-26 01:59:52.000000 rotary-embedding-torch-0.5.3/rotary_embedding_torch/rotary_embedding_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 02:00:03.821788 rotary-embedding-torch-0.5.3/rotary_embedding_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-26 02:00:03.000000 rotary-embedding-torch-0.5.3/rotary_embedding_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2023-12-26 02:00:03.000000 rotary-embedding-torch-0.5.3/rotary_embedding_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 02:00:03.000000 rotary-embedding-torch-0.5.3/rotary_embedding_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-26 02:00:03.000000 rotary-embedding-torch-0.5.3/rotary_embedding_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-26 02:00:03.000000 rotary-embedding-torch-0.5.3/rotary_embedding_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-26 02:00:03.825788 rotary-embedding-torch-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-26 01:59:52.000000 rotary-embedding-torch-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:26:52.161379 rotary_embedding_torch-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 14:26:45.000000 rotary_embedding_torch-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-09 14:26:52.161379 rotary_embedding_torch-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-05-09 14:26:45.000000 rotary_embedding_torch-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:26:52.161379 rotary_embedding_torch-0.6.0/rotary_embedding_torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 14:26:45.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-05-09 14:26:45.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch/rotary_embedding_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:26:52.161379 rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-09 14:26:52.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-09 14:26:52.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:26:52.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 14:26:52.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 14:26:52.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:26:52.161379 rotary_embedding_torch-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-09 14:26:45.000000 rotary_embedding_torch-0.6.0/setup.py
```

### Comparing `rotary-embedding-torch-0.5.3/LICENSE` & `rotary_embedding_torch-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rotary-embedding-torch-0.5.3/PKG-INFO` & `rotary_embedding_torch-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.5.3
+Version: 0.6.0
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary-embedding-torch-0.5.3/README.md` & `rotary_embedding_torch-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `rotary-embedding-torch-0.5.3/rotary_embedding_torch/rotary_embedding_torch.py` & `rotary_embedding_torch-0.6.0/rotary_embedding_torch/rotary_embedding_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,48 +129,49 @@
             self.tmp_store('scale', None)
             return
 
         scale = (torch.arange(0, dim, 2) + 0.4 * dim) / (1.4 * dim)
         self.scale_base = xpos_scale_base
         self.tmp_store('scale', scale)
 
+        # add apply_rotary_emb as static method
+
+        self.apply_rotary_emb = staticmethod(apply_rotary_emb)
+
     @property
     def device(self):
         return self.dummy.device
 
     def tmp_store(self, key, value):
         self.register_buffer(key, value, persistent = False)
 
     def get_seq_pos(self, seq_len, device, dtype, offset = 0):
         return (torch.arange(seq_len, device = device, dtype = dtype) + offset) / self.interpolate_factor
 
-    def rotate_queries_or_keys(self, t, seq_dim = None, offset = 0, freq_seq_len = None):
+    def rotate_queries_or_keys(self, t, seq_dim = None, offset = 0):
         seq_dim = default(seq_dim, self.default_seq_dim)
 
         assert not self.use_xpos, 'you must use `.rotate_queries_and_keys` method instead and pass in both queries and keys, for length extrapolatable rotary embeddings'
 
         device, dtype, seq_len = t.device, t.dtype, t.shape[seq_dim]
 
-        if exists(freq_seq_len):
-            assert freq_seq_len >= seq_len
-            seq_len = freq_seq_len
-
         freqs = self.forward(self.get_seq_pos(seq_len, device = device, dtype = dtype, offset = offset), seq_len = seq_len, offset = offset)
 
         if seq_dim == -3:
             freqs = rearrange(freqs, 'n d -> n 1 d')
 
         return apply_rotary_emb(freqs, t, seq_dim = seq_dim)
 
     def rotate_queries_with_cached_keys(self, q, k, seq_dim = None, offset = 0):
         seq_dim = default(seq_dim, self.default_seq_dim)
 
         q_len, k_len = q.shape[seq_dim], k.shape[seq_dim]
         assert q_len <= k_len
-        rotated_q = self.rotate_queries_or_keys(q, seq_dim = seq_dim, freq_seq_len = k_len)
+
+        rotated_q = self.rotate_queries_or_keys(q, seq_dim = seq_dim, offset = k_len - q_len)
         rotated_k = self.rotate_queries_or_keys(k, seq_dim = seq_dim)
 
         rotated_q = rotated_q.type(q.dtype)
         rotated_k = rotated_k.type(k.dtype)
 
         return rotated_q, rotated_k
```

### Comparing `rotary-embedding-torch-0.5.3/rotary_embedding_torch.egg-info/PKG-INFO` & `rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.5.3
+Version: 0.6.0
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary-embedding-torch-0.5.3/setup.py` & `rotary_embedding_torch-0.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'rotary-embedding-torch',
   packages = find_packages(),
-  version = '0.5.3',
+  version = '0.6.0',
   license='MIT',
   description = 'Rotary Embedding - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/rotary-embedding-torch',
   keywords = [
```

