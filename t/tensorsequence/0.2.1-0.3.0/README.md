# Comparing `tmp/tensorsequence-0.2.1.tar.gz` & `tmp/tensorsequence-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorsequence-0.2.1.tar", last modified: Sun Apr 21 18:31:04 2024, max compression
+gzip compressed data, was "tensorsequence-0.3.0.tar", last modified: Thu May  9 19:54:11 2024, max compression
```

## Comparing `tensorsequence-0.2.1.tar` & `tensorsequence-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:31:04.169699 tensorsequence-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-21 18:31:04.169699 tensorsequence-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-21 18:31:00.000000 tensorsequence-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:31:04.169699 tensorsequence-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-21 18:31:00.000000 tensorsequence-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:31:04.165699 tensorsequence-0.2.1/tensorsequence/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 18:31:00.000000 tensorsequence-0.2.1/tensorsequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-21 18:31:00.000000 tensorsequence-0.2.1/tensorsequence/tensorsequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:31:04.169699 tensorsequence-0.2.1/tensorsequence/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:31:00.000000 tensorsequence-0.2.1/tensorsequence/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-21 18:31:00.000000 tensorsequence-0.2.1/tensorsequence/tests/test_tensorsequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:31:04.169699 tensorsequence-0.2.1/tensorsequence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-21 18:31:04.000000 tensorsequence-0.2.1/tensorsequence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-21 18:31:04.000000 tensorsequence-0.2.1/tensorsequence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:31:04.000000 tensorsequence-0.2.1/tensorsequence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 18:31:04.000000 tensorsequence-0.2.1/tensorsequence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-21 18:31:04.000000 tensorsequence-0.2.1/tensorsequence.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:54:11.632343 tensorsequence-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-09 19:54:11.632343 tensorsequence-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-09 19:54:08.000000 tensorsequence-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 19:54:11.632343 tensorsequence-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-09 19:54:08.000000 tensorsequence-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:54:11.628343 tensorsequence-0.3.0/tensorsequence/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-09 19:54:08.000000 tensorsequence-0.3.0/tensorsequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-09 19:54:08.000000 tensorsequence-0.3.0/tensorsequence/tensorsequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:54:11.628343 tensorsequence-0.3.0/tensorsequence/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 19:54:08.000000 tensorsequence-0.3.0/tensorsequence/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-09 19:54:08.000000 tensorsequence-0.3.0/tensorsequence/tests/test_tensorsequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 19:54:11.628343 tensorsequence-0.3.0/tensorsequence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-09 19:54:11.000000 tensorsequence-0.3.0/tensorsequence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-09 19:54:11.000000 tensorsequence-0.3.0/tensorsequence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 19:54:11.000000 tensorsequence-0.3.0/tensorsequence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 19:54:11.000000 tensorsequence-0.3.0/tensorsequence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 19:54:11.000000 tensorsequence-0.3.0/tensorsequence.egg-info/top_level.txt
```

### Comparing `tensorsequence-0.2.1/PKG-INFO` & `tensorsequence-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: tensorsequence
-Version: 0.2.1
-Summary: manipulate sequences of tensors
-Home-page: https://github.com/theAdamColton/tensorsequence
-Author: Adam Colton
-Description-Content-Type: text/markdown
-Requires-Dist: torch>=2.0.1
-
 # tensorsequence
 
 tensorsequence is a pytorch library that lets you perform operations on related sequences using a unified `TensorSequence` object.
 
 It aims to reduce the complexity of using multiple related sequences. Sequences like these are very commonly used as inputs to a transformer model:
 ```python
 import torch
@@ -23,70 +14,90 @@
 pad_id = 255
 
 token_embeddings = nn.Embedding(vocab_size, hidden_size)
 
 input_ids = torch.randint(0, vocab_size, (batch_size, sequence_length))
 input_embeds = token_embeddings(input_ids) # Shape: batch_size, sequence_length, hidden_size
 key_pad_mask = input_ids == pad_id # Shape: batch_size, sequence_length 
-is_token_whitespace_mask = (input_ids == 0) | (input_ids == 1)# Shape: batch_size, sequence_length 
+is_whitespace_mask = (input_ids == 0) | (input_ids == 1)# Shape: batch_size, sequence_length 
 
 # These tensors would be used like this:
-# logits = transformer_model(input_embeds, key_pad_mask, is_token_whitespace_mask)
+# logits = transformer_model(input_embeds, key_pad_mask, is_whitespace_mask)
 ```
 
-Notice that any place where these tensors are truncated or stacked or concatenated there will be tedious repetitive code like this:
+Notice wherever these tensors are truncated or stacked or concatenated there will be tedious repetitive code like this:
 
 ```python
-def truncate_inputs(hidden_states, key_pad_mask, is_token_whitespace_mask, length):
+def truncate_inputs(hidden_states, key_pad_mask, is_whitespace_mask, length):
   hidden_states = hidden_states[:, :length]
   key_pad_mask= key_pad_mask[:, :length]
-  is_token_whitespace_mask= is_token_whitespace_mask[:, :length, :length]
-  return hidden_states, key_pad_mask, attention_mask
+  is_whitespace_mask= is_whitespace_mask[:, :length, :length]
+  return hidden_states, key_pad_mask, is_whitespace_mask
 
-truncated_inputs = truncate_inputs(hidden_states, key_pad_mask, is_token_whitespace_mask, length)
+truncated_inputs = truncate_inputs(hidden_states, key_pad_mask, is_whitespace_mask, length=10)
 ```
 
-`input_ids`, `input_embeds`, `key_pad_mask`, and `is_whitespace_mask` are all related.
+This repetitive code can be avoided. `input_ids`, `input_embeds`, `key_pad_mask`, and `is_whitespace_mask` are all related.
 They all have matching leading dimensions for batch_size and sequence length. 
-TensorSequence is a container for these related multi-dimensional sequences. 
-TensorSequence makes this kind of manipulation very easy and ergonomic.
+
+TensorSequence is a container for these related multi-dimensional sequences, making this kind of manipulation very easy and ergonomic.
 
 ```python
-from tensorsequence import TensorSequence
-inputs = TensorSequence((input_ids, input_embeds, key_pad_mask, is_whitespace_mask), sequence_dim=1)
+import tensorsequence as ts
+length = 10
+inputs = ts.TensorSequence(
+                input_ids=input_ids,
+                input_embeds=input_embeds,
+                key_pad_mask=key_pad_mask,
+                is_whitespace_mask=is_whitespace_mask,
+                sequence_dim=1
+         )
 truncated_inputs = inputs.iloc[:, :length]
+print(truncated_inputs)
+```
+
+prints:
+```
+TensorSet(
+  named_columns:
+    name: input_ids, shape: torch.Size([8, 10]), dtype: torch.int64
+    name: input_embeds, shape: torch.Size([8, 10, 768]), dtype: torch.float32
+    name: key_pad_mask, shape: torch.Size([8, 10]), dtype: torch.bool
+    name: is_whitespace_mask, shape: torch.Size([8, 10]), dtype: torch.bool
+)
 ```
 
 
 # Features
 
-Stack related TensorSets to create larger batches
+Stack related TensorSequences to create larger batches
 
 ```python
 sequence_length = 20
-sequence_1 = TensorSequence(
-                (torch.randn(sequence_length, 512),
-                torch.randn(sequence_length, 1024)),
+sequence_1 = ts.TensorSequence(
+                torch.randn(sequence_length, 512),
+                torch.randn(sequence_length, 1024),
                 sequence_dim=0
             )
-sequence_2 = TensorSequence(
-                (torch.randn(sequence_length, 512),
-                 torch.randn(sequence_length, 1024)),
-                 sequence_dim=0)
-batch = TensorSequence.stack(sequence_1, sequence_2)
+sequence_2 = ts.TensorSequence(
+                torch.randn(sequence_length, 512),
+                torch.randn(sequence_length, 1024),
+                sequence_dim=0)
+batch = ts.stack((sequence_1, sequence_2))
 
 print(batch.sequence_length) # Prints 20
 print(batch.leading_shape[0]) # This is the batch size, Prints 2
 ```
 
-Pad TensorSets with a specific amount of padding along the sequence dimension
+Pad TensorSequences with a specific amount of padding along the sequence dimension
 ```python
 sequence_length = 20
-sequence = TensorSequence(
-                (torch.randn(sequence_length, 512), torch.randn(sequence_length, 1024)),
+sequence = ts.TensorSequence(
+                torch.randn(sequence_length, 512),
+                torch.randn(sequence_length, 1024),
                 sequence_dim=0
             )
 pad_value = -200
 padded_sequence = sequence.pad(44, pad_value)
 print(padded_sequence.sequence_length) # prints 64
 ```
```

### Comparing `tensorsequence-0.2.1/README.md` & `tensorsequence-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: tensorsequence
+Version: 0.3.0
+Summary: manipulate sequences of tensors
+Home-page: https://github.com/theAdamColton/tensorsequence
+Author: Adam Colton
+Description-Content-Type: text/markdown
+Requires-Dist: torch>=2.0.1
+
 # tensorsequence
 
 tensorsequence is a pytorch library that lets you perform operations on related sequences using a unified `TensorSequence` object.
 
 It aims to reduce the complexity of using multiple related sequences. Sequences like these are very commonly used as inputs to a transformer model:
 ```python
 import torch
@@ -14,70 +23,90 @@
 pad_id = 255
 
 token_embeddings = nn.Embedding(vocab_size, hidden_size)
 
 input_ids = torch.randint(0, vocab_size, (batch_size, sequence_length))
 input_embeds = token_embeddings(input_ids) # Shape: batch_size, sequence_length, hidden_size
 key_pad_mask = input_ids == pad_id # Shape: batch_size, sequence_length 
-is_token_whitespace_mask = (input_ids == 0) | (input_ids == 1)# Shape: batch_size, sequence_length 
+is_whitespace_mask = (input_ids == 0) | (input_ids == 1)# Shape: batch_size, sequence_length 
 
 # These tensors would be used like this:
-# logits = transformer_model(input_embeds, key_pad_mask, is_token_whitespace_mask)
+# logits = transformer_model(input_embeds, key_pad_mask, is_whitespace_mask)
 ```
 
-Notice that any place where these tensors are truncated or stacked or concatenated there will be tedious repetitive code like this:
+Notice wherever these tensors are truncated or stacked or concatenated there will be tedious repetitive code like this:
 
 ```python
-def truncate_inputs(hidden_states, key_pad_mask, is_token_whitespace_mask, length):
+def truncate_inputs(hidden_states, key_pad_mask, is_whitespace_mask, length):
   hidden_states = hidden_states[:, :length]
   key_pad_mask= key_pad_mask[:, :length]
-  is_token_whitespace_mask= is_token_whitespace_mask[:, :length, :length]
-  return hidden_states, key_pad_mask, attention_mask
+  is_whitespace_mask= is_whitespace_mask[:, :length, :length]
+  return hidden_states, key_pad_mask, is_whitespace_mask
 
-truncated_inputs = truncate_inputs(hidden_states, key_pad_mask, is_token_whitespace_mask, length)
+truncated_inputs = truncate_inputs(hidden_states, key_pad_mask, is_whitespace_mask, length=10)
 ```
 
-`input_ids`, `input_embeds`, `key_pad_mask`, and `is_whitespace_mask` are all related.
+This repetitive code can be avoided. `input_ids`, `input_embeds`, `key_pad_mask`, and `is_whitespace_mask` are all related.
 They all have matching leading dimensions for batch_size and sequence length. 
-TensorSequence is a container for these related multi-dimensional sequences. 
-TensorSequence makes this kind of manipulation very easy and ergonomic.
+
+TensorSequence is a container for these related multi-dimensional sequences, making this kind of manipulation very easy and ergonomic.
 
 ```python
-from tensorsequence import TensorSequence
-inputs = TensorSequence((input_ids, input_embeds, key_pad_mask, is_whitespace_mask), sequence_dim=1)
+import tensorsequence as ts
+length = 10
+inputs = ts.TensorSequence(
+                input_ids=input_ids,
+                input_embeds=input_embeds,
+                key_pad_mask=key_pad_mask,
+                is_whitespace_mask=is_whitespace_mask,
+                sequence_dim=1
+         )
 truncated_inputs = inputs.iloc[:, :length]
+print(truncated_inputs)
+```
+
+prints:
+```
+TensorSet(
+  named_columns:
+    name: input_ids, shape: torch.Size([8, 10]), dtype: torch.int64
+    name: input_embeds, shape: torch.Size([8, 10, 768]), dtype: torch.float32
+    name: key_pad_mask, shape: torch.Size([8, 10]), dtype: torch.bool
+    name: is_whitespace_mask, shape: torch.Size([8, 10]), dtype: torch.bool
+)
 ```
 
 
 # Features
 
-Stack related TensorSets to create larger batches
+Stack related TensorSequences to create larger batches
 
 ```python
 sequence_length = 20
-sequence_1 = TensorSequence(
-                (torch.randn(sequence_length, 512),
-                torch.randn(sequence_length, 1024)),
+sequence_1 = ts.TensorSequence(
+                torch.randn(sequence_length, 512),
+                torch.randn(sequence_length, 1024),
                 sequence_dim=0
             )
-sequence_2 = TensorSequence(
-                (torch.randn(sequence_length, 512),
-                 torch.randn(sequence_length, 1024)),
-                 sequence_dim=0)
-batch = TensorSequence.stack(sequence_1, sequence_2)
+sequence_2 = ts.TensorSequence(
+                torch.randn(sequence_length, 512),
+                torch.randn(sequence_length, 1024),
+                sequence_dim=0)
+batch = ts.stack((sequence_1, sequence_2))
 
 print(batch.sequence_length) # Prints 20
 print(batch.leading_shape[0]) # This is the batch size, Prints 2
 ```
 
-Pad TensorSets with a specific amount of padding along the sequence dimension
+Pad TensorSequences with a specific amount of padding along the sequence dimension
 ```python
 sequence_length = 20
-sequence = TensorSequence(
-                (torch.randn(sequence_length, 512), torch.randn(sequence_length, 1024)),
+sequence = ts.TensorSequence(
+                torch.randn(sequence_length, 512),
+                torch.randn(sequence_length, 1024),
                 sequence_dim=0
             )
 pad_value = -200
 padded_sequence = sequence.pad(44, pad_value)
 print(padded_sequence.sequence_length) # prints 64
 ```
```

### Comparing `tensorsequence-0.2.1/tensorsequence.egg-info/PKG-INFO` & `tensorsequence-0.3.0/tensorsequence.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorsequence
-Version: 0.2.1
+Version: 0.3.0
 Summary: manipulate sequences of tensors
 Home-page: https://github.com/theAdamColton/tensorsequence
 Author: Adam Colton
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.0.1
 
 # tensorsequence
@@ -23,70 +23,90 @@
 pad_id = 255
 
 token_embeddings = nn.Embedding(vocab_size, hidden_size)
 
 input_ids = torch.randint(0, vocab_size, (batch_size, sequence_length))
 input_embeds = token_embeddings(input_ids) # Shape: batch_size, sequence_length, hidden_size
 key_pad_mask = input_ids == pad_id # Shape: batch_size, sequence_length 
-is_token_whitespace_mask = (input_ids == 0) | (input_ids == 1)# Shape: batch_size, sequence_length 
+is_whitespace_mask = (input_ids == 0) | (input_ids == 1)# Shape: batch_size, sequence_length 
 
 # These tensors would be used like this:
-# logits = transformer_model(input_embeds, key_pad_mask, is_token_whitespace_mask)
+# logits = transformer_model(input_embeds, key_pad_mask, is_whitespace_mask)
 ```
 
-Notice that any place where these tensors are truncated or stacked or concatenated there will be tedious repetitive code like this:
+Notice wherever these tensors are truncated or stacked or concatenated there will be tedious repetitive code like this:
 
 ```python
-def truncate_inputs(hidden_states, key_pad_mask, is_token_whitespace_mask, length):
+def truncate_inputs(hidden_states, key_pad_mask, is_whitespace_mask, length):
   hidden_states = hidden_states[:, :length]
   key_pad_mask= key_pad_mask[:, :length]
-  is_token_whitespace_mask= is_token_whitespace_mask[:, :length, :length]
-  return hidden_states, key_pad_mask, attention_mask
+  is_whitespace_mask= is_whitespace_mask[:, :length, :length]
+  return hidden_states, key_pad_mask, is_whitespace_mask
 
-truncated_inputs = truncate_inputs(hidden_states, key_pad_mask, is_token_whitespace_mask, length)
+truncated_inputs = truncate_inputs(hidden_states, key_pad_mask, is_whitespace_mask, length=10)
 ```
 
-`input_ids`, `input_embeds`, `key_pad_mask`, and `is_whitespace_mask` are all related.
+This repetitive code can be avoided. `input_ids`, `input_embeds`, `key_pad_mask`, and `is_whitespace_mask` are all related.
 They all have matching leading dimensions for batch_size and sequence length. 
-TensorSequence is a container for these related multi-dimensional sequences. 
-TensorSequence makes this kind of manipulation very easy and ergonomic.
+
+TensorSequence is a container for these related multi-dimensional sequences, making this kind of manipulation very easy and ergonomic.
 
 ```python
-from tensorsequence import TensorSequence
-inputs = TensorSequence((input_ids, input_embeds, key_pad_mask, is_whitespace_mask), sequence_dim=1)
+import tensorsequence as ts
+length = 10
+inputs = ts.TensorSequence(
+                input_ids=input_ids,
+                input_embeds=input_embeds,
+                key_pad_mask=key_pad_mask,
+                is_whitespace_mask=is_whitespace_mask,
+                sequence_dim=1
+         )
 truncated_inputs = inputs.iloc[:, :length]
+print(truncated_inputs)
+```
+
+prints:
+```
+TensorSet(
+  named_columns:
+    name: input_ids, shape: torch.Size([8, 10]), dtype: torch.int64
+    name: input_embeds, shape: torch.Size([8, 10, 768]), dtype: torch.float32
+    name: key_pad_mask, shape: torch.Size([8, 10]), dtype: torch.bool
+    name: is_whitespace_mask, shape: torch.Size([8, 10]), dtype: torch.bool
+)
 ```
 
 
 # Features
 
-Stack related TensorSets to create larger batches
+Stack related TensorSequences to create larger batches
 
 ```python
 sequence_length = 20
-sequence_1 = TensorSequence(
-                (torch.randn(sequence_length, 512),
-                torch.randn(sequence_length, 1024)),
+sequence_1 = ts.TensorSequence(
+                torch.randn(sequence_length, 512),
+                torch.randn(sequence_length, 1024),
                 sequence_dim=0
             )
-sequence_2 = TensorSequence(
-                (torch.randn(sequence_length, 512),
-                 torch.randn(sequence_length, 1024)),
-                 sequence_dim=0)
-batch = TensorSequence.stack(sequence_1, sequence_2)
+sequence_2 = ts.TensorSequence(
+                torch.randn(sequence_length, 512),
+                torch.randn(sequence_length, 1024),
+                sequence_dim=0)
+batch = ts.stack((sequence_1, sequence_2))
 
 print(batch.sequence_length) # Prints 20
 print(batch.leading_shape[0]) # This is the batch size, Prints 2
 ```
 
-Pad TensorSets with a specific amount of padding along the sequence dimension
+Pad TensorSequences with a specific amount of padding along the sequence dimension
 ```python
 sequence_length = 20
-sequence = TensorSequence(
-                (torch.randn(sequence_length, 512), torch.randn(sequence_length, 1024)),
+sequence = ts.TensorSequence(
+                torch.randn(sequence_length, 512),
+                torch.randn(sequence_length, 1024),
                 sequence_dim=0
             )
 pad_value = -200
 padded_sequence = sequence.pad(44, pad_value)
 print(padded_sequence.sequence_length) # prints 64
 ```
```

