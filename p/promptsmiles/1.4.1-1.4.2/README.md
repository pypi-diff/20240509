# Comparing `tmp/promptsmiles-1.4.1.tar.gz` & `tmp/promptsmiles-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptsmiles-1.4.1.tar", last modified: Fri Mar  8 11:39:42 2024, max compression
+gzip compressed data, was "promptsmiles-1.4.2.tar", last modified: Thu May  9 09:43:23 2024, max compression
```

## Comparing `promptsmiles-1.4.1.tar` & `promptsmiles-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 morgan    (3088) lab       (3000)        0 2024-03-08 11:39:42.327989 promptsmiles-1.4.1/
--rw-r--r--   0 morgan    (3088) lab       (3000)    11357 2024-01-23 15:43:24.000000 promptsmiles-1.4.1/LICENSE
--rw-r--r--   0 morgan    (3088) lab       (3000)    16474 2024-03-08 11:39:42.324989 promptsmiles-1.4.1/PKG-INFO
--rw-r--r--   0 morgan    (3088) lab       (3000)     2869 2024-02-29 15:43:11.000000 promptsmiles-1.4.1/README.md
-drwxr-xr-x   0 morgan    (3088) lab       (3000)        0 2024-03-08 11:39:42.257989 promptsmiles-1.4.1/promptsmiles/
--rw-r--r--   0 morgan    (3088) lab       (3000)      291 2024-02-13 10:21:29.000000 promptsmiles-1.4.1/promptsmiles/__init__.py
--rw-r--r--   0 morgan    (3088) lab       (3000)    32394 2024-02-29 14:21:50.000000 promptsmiles-1.4.1/promptsmiles/samplers.py
--rw-r--r--   0 morgan    (3088) lab       (3000)    23147 2024-03-08 11:36:43.000000 promptsmiles-1.4.1/promptsmiles/utils.py
-drwxr-xr-x   0 morgan    (3088) lab       (3000)        0 2024-03-08 11:39:42.321989 promptsmiles-1.4.1/promptsmiles.egg-info/
--rw-r--r--   0 morgan    (3088) lab       (3000)    16474 2024-03-08 11:39:42.000000 promptsmiles-1.4.1/promptsmiles.egg-info/PKG-INFO
--rw-r--r--   0 morgan    (3088) lab       (3000)      350 2024-03-08 11:39:42.000000 promptsmiles-1.4.1/promptsmiles.egg-info/SOURCES.txt
--rw-r--r--   0 morgan    (3088) lab       (3000)        1 2024-03-08 11:39:42.000000 promptsmiles-1.4.1/promptsmiles.egg-info/dependency_links.txt
--rw-r--r--   0 morgan    (3088) lab       (3000)       12 2024-03-08 11:39:42.000000 promptsmiles-1.4.1/promptsmiles.egg-info/requires.txt
--rw-r--r--   0 morgan    (3088) lab       (3000)       24 2024-03-08 11:39:42.000000 promptsmiles-1.4.1/promptsmiles.egg-info/top_level.txt
--rw-r--r--   0 morgan    (3088) lab       (3000)     1073 2024-03-08 11:38:29.000000 promptsmiles-1.4.1/pyproject.toml
--rw-r--r--   0 morgan    (3088) lab       (3000)       38 2024-03-08 11:39:42.327989 promptsmiles-1.4.1/setup.cfg
-drwxr-xr-x   0 morgan    (3088) lab       (3000)        0 2024-03-08 11:39:42.304989 promptsmiles-1.4.1/tests/
--rw-r--r--   0 morgan    (3088) lab       (3000)    10324 2024-02-29 14:20:01.000000 promptsmiles-1.4.1/tests/test_samplers.py
--rw-r--r--   0 morgan    (3088) lab       (3000)     8973 2024-02-29 14:19:35.000000 promptsmiles-1.4.1/tests/test_samplers2.py
--rw-r--r--   0 morgan    (3088) lab       (3000)     8344 2024-02-19 22:22:01.000000 promptsmiles-1.4.1/tests/test_utils.py
+drwxr-xr-x   0 morgan    (3088) lab       (3000)        0 2024-05-09 09:43:23.488841 promptsmiles-1.4.2/
+-rw-r--r--   0 morgan    (3088) lab       (3000)    11357 2024-01-23 15:43:24.000000 promptsmiles-1.4.2/LICENSE
+-rw-r--r--   0 morgan    (3088) lab       (3000)    16473 2024-05-09 09:43:23.487841 promptsmiles-1.4.2/PKG-INFO
+-rw-r--r--   0 morgan    (3088) lab       (3000)     2868 2024-05-09 09:17:50.000000 promptsmiles-1.4.2/README.md
+drwxr-xr-x   0 morgan    (3088) lab       (3000)        0 2024-05-09 09:43:23.471841 promptsmiles-1.4.2/promptsmiles/
+-rw-r--r--   0 morgan    (3088) lab       (3000)      353 2024-05-09 09:18:48.000000 promptsmiles-1.4.2/promptsmiles/__init__.py
+-rw-r--r--   0 morgan    (3088) lab       (3000)    35338 2024-05-09 09:19:39.000000 promptsmiles-1.4.2/promptsmiles/samplers.py
+-rw-r--r--   0 morgan    (3088) lab       (3000)    24158 2024-05-09 09:22:55.000000 promptsmiles-1.4.2/promptsmiles/utils.py
+drwxr-xr-x   0 morgan    (3088) lab       (3000)        0 2024-05-09 09:43:23.485841 promptsmiles-1.4.2/promptsmiles.egg-info/
+-rw-r--r--   0 morgan    (3088) lab       (3000)    16473 2024-05-09 09:43:23.000000 promptsmiles-1.4.2/promptsmiles.egg-info/PKG-INFO
+-rw-r--r--   0 morgan    (3088) lab       (3000)      350 2024-05-09 09:43:23.000000 promptsmiles-1.4.2/promptsmiles.egg-info/SOURCES.txt
+-rw-r--r--   0 morgan    (3088) lab       (3000)        1 2024-05-09 09:43:23.000000 promptsmiles-1.4.2/promptsmiles.egg-info/dependency_links.txt
+-rw-r--r--   0 morgan    (3088) lab       (3000)       12 2024-05-09 09:43:23.000000 promptsmiles-1.4.2/promptsmiles.egg-info/requires.txt
+-rw-r--r--   0 morgan    (3088) lab       (3000)       24 2024-05-09 09:43:23.000000 promptsmiles-1.4.2/promptsmiles.egg-info/top_level.txt
+-rw-r--r--   0 morgan    (3088) lab       (3000)     1074 2024-05-09 09:37:53.000000 promptsmiles-1.4.2/pyproject.toml
+-rw-r--r--   0 morgan    (3088) lab       (3000)       38 2024-05-09 09:43:23.488841 promptsmiles-1.4.2/setup.cfg
+drwxr-xr-x   0 morgan    (3088) lab       (3000)        0 2024-05-09 09:43:23.483842 promptsmiles-1.4.2/tests/
+-rw-r--r--   0 morgan    (3088) lab       (3000)    10381 2024-05-09 09:24:24.000000 promptsmiles-1.4.2/tests/test_samplers.py
+-rw-r--r--   0 morgan    (3088) lab       (3000)     9400 2024-05-09 09:36:36.000000 promptsmiles-1.4.2/tests/test_samplers2.py
+-rw-r--r--   0 morgan    (3088) lab       (3000)     9257 2024-05-09 09:25:54.000000 promptsmiles-1.4.2/tests/test_utils.py
```

### Comparing `promptsmiles-1.4.1/LICENSE` & `promptsmiles-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptsmiles-1.4.1/PKG-INFO` & `promptsmiles-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptsmiles
-Version: 1.4.1
+Version: 1.4.2
 Summary: A conveniant package to manipulate SMILES strings for iterative prompting with chemical language models.
 Author-email: Morgan Thomas <morganthomas263@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -257,15 +257,15 @@
 FL = FragmentLinker(
     fragments=["N1(*)CCNCC1", "C1CC1(*)"],
     batch_size=64,
     sample_fn=CLM.sampler,
     evaluate_fn=CLM.evaluater,
     batch_prompts=False,
     optimize_prompts=True,
-    shuffle=True, 
+    shuffle=True,
     scan=False, # Optional when combining 2 fragments, otherwise is set to true
     return_all=False,
 )
 smiles = FL.sample(batch_size=3)
 ```
 ![alt text](https://github.com/MorganCThomas/PromptSMILES/blob/main/images/frag_link_example.png)
 ## Required chemical language model functions
```

### Comparing `promptsmiles-1.4.1/README.md` & `promptsmiles-1.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 FL = FragmentLinker(
     fragments=["N1(*)CCNCC1", "C1CC1(*)"],
     batch_size=64,
     sample_fn=CLM.sampler,
     evaluate_fn=CLM.evaluater,
     batch_prompts=False,
     optimize_prompts=True,
-    shuffle=True, 
+    shuffle=True,
     scan=False, # Optional when combining 2 fragments, otherwise is set to true
     return_all=False,
 )
 smiles = FL.sample(batch_size=3)
 ```
 ![alt text](https://github.com/MorganCThomas/PromptSMILES/blob/main/images/frag_link_example.png)
 ## Required chemical language model functions
```

### Comparing `promptsmiles-1.4.1/promptsmiles/samplers.py` & `promptsmiles-1.4.2/promptsmiles/samplers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,81 @@
 # Copyright Universitat Pompeu Fabra 2020-2023  https://www.compscience.org
 # Distributed under the Apache 2.0 License.
 # (See accompanying file README.md file or copy at https://opensource.org/license/apache-2-0/)
 
-import random
 import logging
+import random
+
 logger = logging.getLogger("promptsmiles")
+from collections import namedtuple
 from copy import deepcopy
 from typing import Callable
-from collections import namedtuple
 
 from promptsmiles import utils
 
+
 class BaseSampler:
-    def __init__(self, sample_fn: Callable, evaluate_fn: Callable, optimize_prompts: bool, **kwargs):
+    def __init__(
+        self,
+        sample_fn: Callable,
+        evaluate_fn: Callable,
+        optimize_prompts: bool,
+        **kwargs,
+    ):
         self.sample_fn = sample_fn
         self.evaluate_fn = evaluate_fn
         self.optimize_prompts = optimize_prompts
         self.tokenizer = utils.SMILESTokenizer()
 
-    def rearrange_prompt(self, smiles: str, at_idx: int, reverse: bool, n_rand: int = 10, **kwargs):
+    def rearrange_prompt(
+        self, smiles: str, at_idx: int, reverse: bool, n_rand: int = 10, **kwargs
+    ):
         # ---- Randomize ----
-        at_idx = utils.correct_attachment_point(smiles, at_idx) # NOTE correcting attachment index to atom index
+        at_idx = utils.correct_attachment_point(
+            smiles, at_idx
+        )  # NOTE correcting attachment index to atom index
         if self.optimize_prompts:
-            rand_smiles = utils.randomize_smiles(smiles, n_rand=n_rand, random_type='restricted', rootAtom=at_idx, reverse=reverse)
+            rand_smiles = utils.randomize_smiles(
+                smiles,
+                n_rand=n_rand,
+                random_type="restricted",
+                rootAtom=at_idx,
+                reverse=reverse,
+            )
             if rand_smiles:
                 # ---- Evaluate ----
                 try:
-                    nlls = self.evaluate_fn([utils.strip_attachment_points(smi)[0] for smi in rand_smiles])
+                    nlls = self.evaluate_fn(
+                        [utils.strip_attachment_points(smi)[0] for smi in rand_smiles]
+                    )
                     # ---- Sort ----
-                    opt_smi, opt_nll = sorted(zip(rand_smiles, nlls), key=lambda x: x[1])[0]
+                    opt_smi, opt_nll = sorted(
+                        zip(rand_smiles, nlls), key=lambda x: x[1]
+                    )[0]
                     return opt_smi, opt_nll
 
                 except KeyError:
                     # NOTE RDKit sometimes inserts a token that may not have been present in the vocabulary
-                    logger.debug(f"SMILES evaluation failed for {smiles} at {at_idx}, rearranging instead...")
-                    
+                    logger.debug(
+                        f"SMILES evaluation failed for {smiles} at {at_idx}, rearranging instead..."
+                    )
+
             else:
                 # NOTE RDKit sometimes creates duplicate ring indexes for different rings causing an error upon reversal
-                logger.debug(f"SMILES randomization failed for {smiles} at {at_idx}, rearranging instead...")
+                logger.debug(
+                    f"SMILES randomization failed for {smiles} at {at_idx}, rearranging instead..."
+                )
 
         return utils.root_smiles(smiles, at_idx, reverse=reverse), None
 
 
 class DeNovo:
     def __init__(
-        self,
-        batch_size: int,
-        sample_fn: Callable,
-        sample_fn_kwargs={},
-        **kwargs
-        ):
+        self, batch_size: int, sample_fn: Callable, sample_fn_kwargs={}, **kwargs
+    ):
         """
         A de novo sampling class to generate molecules from scratch i.e., dummy wrap that just calls the sample_fn.
 
         Parameters
         ----------
         batch_size : int
             The number of samples to generate. Passed to sample_fn.
@@ -67,37 +89,39 @@
         self.sample_fn_kwargs = sample_fn_kwargs
 
     def sample(self, batch_size: int = None, **kwargs):
         """
         Sample de novo molecules, see init docstring for more details.
         """
         # Set parameters
-        if not batch_size: batch_size = self.batch_size
-        
+        if not batch_size:
+            batch_size = self.batch_size
+
         # Sample
         results = self.sample_fn(batch_size=batch_size, **self.sample_fn_kwargs)
-        
+
         return results
 
 
 class ScaffoldDecorator(BaseSampler):
     def __init__(
         self,
         scaffold: str,
         batch_size: int,
         sample_fn: Callable,
         evaluate_fn: Callable,
         sample_fn_kwargs: dict = {},
         batch_prompts: bool = False,
         optimize_prompts: bool = True,
-        shuffle = True,
+        shuffle=True,
         return_all: bool = False,
-        random_seed = 123,
+        random_seed=123,
         force_first: bool = False,
-        rdkit_logging=False):
+        rdkit_logging=False,
+    ):
         """
         A scaffold decorator class to sample from a scaffold constraint via iterative prompting.
 
         Parameters
         ----------
         scaffold : str
             The scaffold SMILES to decorate.
@@ -119,15 +143,15 @@
             Whether to shuffle the attachment points, by default True
         return_all : bool, optional
             Whether to return all intermediate samples, by default False
         random_seed : int, optional
             The random seed to use, by default 123, only for the wrapper and not e.g., torch.
         force_first : bool, optional
             Whether to force the first attachment point to be the first prompt, by default False
-        
+
         Returns
         -------
         smiles : list
             A list of generated SMILES with a scaffold decorated.
         """
         super().__init__(sample_fn, evaluate_fn, optimize_prompts)
         self.batch_size = batch_size
@@ -135,15 +159,17 @@
         self.shuffle = shuffle
         self.sample_fn = sample_fn
         self.sample_fn_kwargs = sample_fn_kwargs
         self.evaluate_fn = evaluate_fn
         self.return_all = return_all
         self.scaffold = scaffold
         self.force_first = force_first
-        self.variant = namedtuple('variant', ['orig_smiles', 'opt_smiles', 'strip_smiles', 'at_pts', 'nll'])
+        self.variant = namedtuple(
+            "variant", ["orig_smiles", "opt_smiles", "strip_smiles", "at_pts", "nll"]
+        )
         self.seed = random_seed
         random.seed(self.seed)
         if not rdkit_logging:
             utils.disable_rdkit_logging()
 
         # Prepare scaffold SMILES
         self.at_pts = utils.get_attachment_points(self.scaffold)
@@ -151,217 +177,270 @@
         self.variants = []
         # Optionally force initial configuration as the first prompt
         if self.force_first:
             opt_smi = self.scaffold
             opt_nll = self.evaluate_fn([opt_smi])[0]
             strip_smi, rem_pts = utils.strip_attachment_points(opt_smi)
             rem_pts.pop(-1)
-            self.at_pts.pop(-1) # remove last one
+            self.at_pts.pop(-1)  # remove last one
             self.variants.append(
                 self.variant(
                     orig_smiles=self.scaffold,
                     opt_smiles=opt_smi,
                     strip_smiles=strip_smi,
                     at_pts=rem_pts,
-                    nll=opt_nll
-                    )
+                    nll=opt_nll,
                 )
+            )
         # Optimize all other attachment points
         variants = []
         for aidx in self.at_pts:
             opt_smi, opt_nll = self.rearrange_prompt(self.scaffold, aidx, reverse=True)
             strip_smi, rem_pts = utils.strip_attachment_points(opt_smi)
             rem_pts.pop(-1)
             variants.append(
                 self.variant(
                     orig_smiles=self.scaffold,
                     opt_smiles=opt_smi,
                     strip_smiles=strip_smi,
                     at_pts=rem_pts,
-                    nll=opt_nll
-                    )
+                    nll=opt_nll,
                 )
+            )
         if self.optimize_prompts:
             variants.sort(key=lambda x: x.nll)
         self.variants.extend(variants)
 
     def _single_sample(self, shuffle: bool = None, return_all: bool = None):
         # Set parameters
-        if not shuffle: shuffle = self.shuffle
-        if not return_all: return_all = self.return_all
+        if not shuffle:
+            shuffle = self.shuffle
+        if not return_all:
+            return_all = self.return_all
 
         # Select initial attachment point
-        if shuffle: i = random.randint(0, self.n_pts-1)
-        else: i = 0
-        if self.force_first: i = 0
+        if shuffle:
+            i = random.randint(0, self.n_pts - 1)
+        else:
+            i = 0
+        if self.force_first:
+            i = 0
         variant = deepcopy(self.variants[i])
 
         # Sample
         n_rem = self.n_pts
         batch_smiles = []
         while n_rem:
             prompt = variant.strip_smiles
-            smiles = self.sample_fn(prompt=prompt, batch_size=1, **self.sample_fn_kwargs)
+            smiles = self.sample_fn(
+                prompt=prompt, batch_size=1, **self.sample_fn_kwargs
+            )
             smiles = smiles[0]
             if not smiles.startswith(prompt):
-                logger.error(f"Sampled SMILES {smiles} does not start with prompt {prompt}, why not?")
+                logger.error(
+                    f"Sampled SMILES {smiles} does not start with prompt {prompt}, why not?"
+                )
             batch_smiles.append(smiles)
             n_rem -= 1
 
             if n_rem:
                 # Insert remaining attachment points
                 smi_w_at = utils.insert_attachment_points(smiles, variant.at_pts)
                 # Select another
-                if shuffle: i = random.randint(0, n_rem-1)
-                else: i = 0
+                if shuffle:
+                    i = random.randint(0, n_rem - 1)
+                else:
+                    i = 0
                 sel_pt = variant.at_pts[i]
                 # Optimize & strip
                 opt_smi, opt_nll = self.rearrange_prompt(smi_w_at, sel_pt, reverse=True)
                 if opt_smi:
                     strip_smi, rem_pts = utils.strip_attachment_points(opt_smi)
-                    rem_pts.pop(-1) # remove the last one
+                    rem_pts.pop(-1)  # remove the last one
                     variant = self.variant(
                         orig_smiles=smi_w_at,
                         opt_smiles=opt_smi,
                         strip_smiles=strip_smi,
                         at_pts=rem_pts,
-                        nll=opt_nll
-                        )
+                        nll=opt_nll,
+                    )
                 else:
-                    logger.debug(f"SMILES optimization failed for {smiles}, reverting to previous prompt.")
+                    logger.debug(
+                        f"SMILES optimization failed for {smiles}, reverting to previous prompt."
+                    )
                     # Skip position
                     smi_w_at = utils.insert_attachment_points(prompt, variant.at_pts)
-                    opt_smi, opt_nll = self.rearrange_prompt(smi_w_at, sel_pt, reverse=True)
+                    opt_smi, opt_nll = self.rearrange_prompt(
+                        smi_w_at, sel_pt, reverse=True
+                    )
                     if opt_smi:
                         strip_smi, rem_pts = utils.strip_attachment_points(opt_smi)
                         rem_pts.pop(-1)
                         variant = self.variant(
                             orig_smiles=smi_w_at,
                             opt_smiles=opt_smi,
                             strip_smiles=strip_smi,
                             at_pts=rem_pts,
-                            nll=opt_nll
-                            )
+                            nll=opt_nll,
+                        )
                     else:
-                        logger.debug(f"SMILES optimization failed for {smiles}, stopping here.")
+                        logger.debug(
+                            f"SMILES optimization failed for {smiles}, stopping here."
+                        )
                         # Stop here
                         variant = self.variant(
                             orig_smiles=smi_w_at,
                             opt_smiles=smiles,
                             strip_smiles=smiles,
                             at_pts=deepcopy(variant.at_pts),
-                            nll=None
-                            )
+                            nll=None,
+                        )
 
         if return_all:
             return batch_smiles
         else:
             return batch_smiles[-1]
-    
-    def _batch_sample(self, batch_size: int = None, shuffle: bool = None, return_all: bool = None):
+
+    def _batch_sample(
+        self, batch_size: int = None, shuffle: bool = None, return_all: bool = None
+    ):
         """More efficient sampling assuming the sample_fn can accept a batch of prompts"""
         # Set parameters
-        if not batch_size: batch_size = self.batch_size
-        if not shuffle: shuffle = self.shuffle
-        if not return_all: return_all = self.return_all
+        if not batch_size:
+            batch_size = self.batch_size
+        if not shuffle:
+            shuffle = self.shuffle
+        if not return_all:
+            return_all = self.return_all
 
         # Select initial attachment points
         batch_variants = []
         for _ in range(batch_size):
-            if shuffle: i = random.randint(0, self.n_pts-1)
-            else: i = 0
-            if self.force_first: i = 0
+            if shuffle:
+                i = random.randint(0, self.n_pts - 1)
+            else:
+                i = 0
+            if self.force_first:
+                i = 0
             batch_variants.append(deepcopy(self.variants[i]))
 
         # Sample
         n_rem = self.n_pts
         batch_smiles = []
         while n_rem:
             # Sample based on initial prompt
             prompts = [v.strip_smiles for v in batch_variants]
-            smiles = self.sample_fn(prompt=prompts, batch_size=batch_size, **self.sample_fn_kwargs)
+            smiles = self.sample_fn(
+                prompt=prompts, batch_size=batch_size, **self.sample_fn_kwargs
+            )
             batch_smiles.append(smiles)
             n_rem -= 1
 
             if n_rem:
                 new_variants = []
                 for smi, variant in zip(smiles, batch_variants):
                     if not smi.startswith(variant.strip_smiles):
-                        logger.error(f"Sampled SMILES {smi} does not start with prompt {variant.strip_smiles}, why not?")
-                    
+                        logger.error(
+                            f"Sampled SMILES {smi} does not start with prompt {variant.strip_smiles}, why not?"
+                        )
+
                     # Insert remaining attachment points
                     smi_w_at = utils.insert_attachment_points(smi, variant.at_pts)
                     # Select another
-                    if shuffle: i = random.randint(0, n_rem-1)
-                    else: i = 0
+                    if shuffle:
+                        i = random.randint(0, n_rem - 1)
+                    else:
+                        i = 0
                     sel_pt = variant.at_pts[i]
                     # Optimize & strip
-                    opt_smi, opt_nll = self.rearrange_prompt(smi_w_at, sel_pt, reverse=True)
+                    opt_smi, opt_nll = self.rearrange_prompt(
+                        smi_w_at, sel_pt, reverse=True
+                    )
                     if opt_smi:
                         strip_smi, rem_pts = utils.strip_attachment_points(opt_smi)
-                        rem_pts.pop(-1) # remove the last one
+                        rem_pts.pop(-1)  # remove the last one
                         # Create new batch_variants?
                         new_variants.append(
                             self.variant(
                                 orig_smiles=smi_w_at,
                                 opt_smiles=opt_smi,
                                 strip_smiles=strip_smi,
                                 at_pts=rem_pts,
-                                nll=opt_nll
-                                )
+                                nll=opt_nll,
                             )
+                        )
                     else:
-                        logger.debug(f"SMILES optimization failed for {smi}, reverting to previous prompt.")
+                        logger.debug(
+                            f"SMILES optimization failed for {smi}, reverting to previous prompt."
+                        )
                         # Skip position (variant.strip_smiles = previous_)
-                        smi_w_at = utils.insert_attachment_points(variant.strip_smiles, variant.at_pts)
-                        opt_smi, opt_nll = self.rearrange_prompt(smi_w_at, sel_pt, reverse=True)
+                        smi_w_at = utils.insert_attachment_points(
+                            variant.strip_smiles, variant.at_pts
+                        )
+                        opt_smi, opt_nll = self.rearrange_prompt(
+                            smi_w_at, sel_pt, reverse=True
+                        )
                         if opt_smi:
                             strip_smi, rem_pts = utils.strip_attachment_points(opt_smi)
                             rem_pts.pop(-1)
                             new_variants.append(
                                 self.variant(
                                     orig_smiles=smi_w_at,
                                     opt_smiles=opt_smi,
                                     strip_smiles=strip_smi,
                                     at_pts=rem_pts,
-                                    nll=opt_nll
+                                    nll=opt_nll,
                                 )
                             )
                         else:
-                            logger.debug(f"SMILES optimization failed for {smi}, stopping here.")
+                            logger.debug(
+                                f"SMILES optimization failed for {smi}, stopping here."
+                            )
                             # Stop here
                             new_variants.append(
                                 self.variant(
                                     orig_smiles=smi_w_at,
                                     opt_smiles=smi,
                                     strip_smiles=smi,
                                     at_pts=deepcopy(variant.at_pts),
-                                    nll=None
-                                    )
+                                    nll=None,
                                 )
+                            )
                 batch_variants = new_variants
 
         if return_all:
             return batch_smiles
         else:
             return batch_smiles[-1]
 
-    def sample(self, batch_size: int = None, batch_prompts: bool = None, return_all: bool = None, shuffle: bool = None):
+    def sample(
+        self,
+        batch_size: int = None,
+        batch_prompts: bool = None,
+        return_all: bool = None,
+        shuffle: bool = None,
+    ):
         """
         Sample de novo molecules, see init docstring for more details.
         """
         # Set parameters
-        if not batch_size: batch_size = self.batch_size
-        if not batch_prompts: batch_prompts = self.batch_prompts
-        if not shuffle: shuffle = self.shuffle
-        if not return_all: return_all = self.return_all
+        if not batch_size:
+            batch_size = self.batch_size
+        if not batch_prompts:
+            batch_prompts = self.batch_prompts
+        if not shuffle:
+            shuffle = self.shuffle
+        if not return_all:
+            return_all = self.return_all
 
         # Choose _single_sample, iterative _single_sample, or _batch_sample
         if batch_prompts:
-            return self._batch_sample(batch_size=batch_size, shuffle=shuffle, return_all=return_all)
+            return self._batch_sample(
+                batch_size=batch_size, shuffle=shuffle, return_all=return_all
+            )
         else:
             batch_smiles = []
             for i in range(batch_size):
                 smiles = self._single_sample(shuffle=shuffle, return_all=return_all)
                 batch_smiles.append(smiles)
             # Reformat to be the same as batch_prompts
             if return_all:
@@ -379,16 +458,17 @@
         sample_fn_kwargs: dict = {},
         batch_prompts: bool = False,
         optimize_prompts: bool = True,
         shuffle: bool = True,
         scan: bool = False,
         detect_existing: bool = True,
         return_all: bool = False,
-        random_seed = 123,
-        rdkit_logging=False):
+        random_seed=123,
+        rdkit_logging=False,
+    ):
         """
         A Fragment linker class to combine different fragments together via iterative prompting.
 
         Parameters
         ----------
         fragments : list
             The fragmnet SMILES to link together with one specified attachment point each.
@@ -405,20 +485,20 @@
         batch_prompts : bool, optional
             Whether the sample_fn can accept a list of prompts equal to batch_size, by default False
         optimize_prompts : bool, optional
             Whether to optimize the SMILES string for the attachment point, by default True
         shuffle : bool, optional
             Whether to shuffle the attachment points, by default True
         scan : bool, optional
-            Whether to evaluate fragment attachment through the whole linker as oppose to simple concatenation, by default False, automatically enabled for more than two fragments 
+            Whether to evaluate fragment attachment through the whole linker as oppose to simple concatenation, by default False, automatically enabled for more than two fragments
         return_all : bool, optional
             Whether to return all intermediate samples, by default False
         random_seed : int, optional
             The random seed to use, by default 123, only for the wrapper and not e.g., torch.
-        
+
         Returns
         -------
         smiles : list
             A list of generated SMILES with a fragments linked.
         """
         super().__init__(sample_fn, evaluate_fn, optimize_prompts)
         self.batch_size = batch_size
@@ -426,84 +506,108 @@
         self.shuffle = shuffle
         self.scan = scan
         self.detect_existing = detect_existing
         self.sample_fn = sample_fn
         self.sample_fn_kwargs = sample_fn_kwargs
         self.evaluate_fn = evaluate_fn
         self.return_all = return_all
-        self.fragment = namedtuple('fragment', ['for_smiles', 'for_nll', 'rev_smiles', 'rev_nll'])
+        self.fragment = namedtuple(
+            "fragment", ["for_smiles", "for_nll", "rev_smiles", "rev_nll"]
+        )
         self.seed = random_seed
         random.seed(self.seed)
         if not rdkit_logging:
             utils.disable_rdkit_logging()
 
         # Correct scan
         if len(fragments) > 2 and not self.scan:
-            logger.warn(f"Scan must be used for more than two fragments, Scan will be enabled.")
+            logger.warn(
+                "Scan must be used for more than two fragments, Scan will be enabled."
+            )
             self.scan = True
 
         # Prepare fragments
         self.n_fgs = len(fragments)
         self.fragments = []
         for frag in fragments:
             # Get attachment index
             aidx = utils.get_attachment_points(frag)
-            assert len(aidx) == 1, f"Fragment {frag} should only have one attachment point"
+            assert (
+                len(aidx) == 1
+            ), f"Fragment {frag} should only have one attachment point"
             # Optimize forward direction
             for_smi, for_nll = self.rearrange_prompt(frag, aidx[0], reverse=False)
             # Optimize reverse direction
             rev_smi, rev_nll = self.rearrange_prompt(frag, aidx[0], reverse=True)
             # Append
             self.fragments.append(
                 self.fragment(
                     for_smiles=utils.strip_attachment_points(for_smi)[0],
                     for_nll=for_nll,
                     rev_smiles=utils.strip_attachment_points(rev_smi)[0],
-                    rev_nll=rev_nll
-                    )
+                    rev_nll=rev_nll,
+                )
             )
         if self.optimize_prompts:
             self.fragments.sort(key=lambda x: x.for_nll)
 
-    def _single_sample(self, shuffle: bool = None, scan: bool = None, detect_existing: bool = None, return_all: bool = None):
+    def _single_sample(
+        self,
+        shuffle: bool = None,
+        scan: bool = None,
+        detect_existing: bool = None,
+        return_all: bool = None,
+    ):
         # Set parameters
-        if not shuffle: shuffle = self.shuffle
-        if not scan: scan = self.scan
-        if not detect_existing: detect_existing = self.detect_existing
-        if not return_all: return_all = self.return_all
+        if not shuffle:
+            shuffle = self.shuffle
+        if not scan:
+            scan = self.scan
+        if not detect_existing:
+            detect_existing = self.detect_existing
+        if not return_all:
+            return_all = self.return_all
         fragments = deepcopy(self.fragments)
 
         # Randomly select starting attachment points
-        if shuffle: i = random.randint(0, self.n_fgs-1)
-        else: i = 0
+        if shuffle:
+            i = random.randint(0, self.n_fgs - 1)
+        else:
+            i = 0
         f0 = fragments.pop(i)
 
         # Sample
         n_rem = self.n_fgs
         batch_smiles = []
         prompt = f0.rev_smiles
         prompt_tokens = self.tokenizer.tokenize(prompt, with_begin_and_end=False)
         frag_indexes = list(range(len(prompt_tokens)))
         smiles = self.sample_fn(prompt=prompt, batch_size=1, **self.sample_fn_kwargs)
         smiles = smiles[0]
-        assert smiles.startswith(prompt), f"Sampled SMILES {smiles} does not start with prompt {prompt}, why not?"
+        assert smiles.startswith(
+            prompt
+        ), f"Sampled SMILES {smiles} does not start with prompt {prompt}, why not?"
         smiles_tokens = self.tokenizer.tokenize(smiles, with_begin_and_end=False)
         batch_smiles.append(smiles)
         n_rem -= 1
-        
+
         if self.scan:
             while n_rem:
                 # Select another fragment
-                if shuffle: i = random.randint(0, n_rem-1)
-                else: i = 0
+                if shuffle:
+                    i = random.randint(0, n_rem - 1)
+                else:
+                    i = 0
                 fi = fragments.pop(i)
                 # Detect existing fragments
                 if detect_existing:
                     exists = False
-                    existing_atoms = utils.detect_existing_fragment(smiles, fi.for_smiles)
+                    existing_atoms = utils.detect_existing_fragment(
+                        smiles, fi.for_smiles
+                    )
                     # Get an atom map between atoms and tokens
                     atom_map = self.tokenizer._token2atom_map(smiles_tokens)
                     # Check it's not generated linker
                     for match in existing_atoms:
                         if not any([atom_map[aidx] in frag_indexes for aidx in match]):
                             # If so, insert fragment indexes, append etc.
                             frag_indexes.extend([atom_map[aidx] for aidx in match])
@@ -513,27 +617,37 @@
                             break
                     if exists:
                         continue
                 # Correct rings
                 fi_smi = utils.correct_fragment_ring_numbers(smiles, fi.for_smiles)
                 # Insert fragment at different positions
                 temp_smiles = []
-                for i in range(len(prompt_tokens)-1, len(smiles_tokens)):
-                    if i in frag_indexes: 
-                        continue 
-                    else: 
+                for i in range(len(prompt_tokens) - 1, len(smiles_tokens)):
+                    if i in frag_indexes:
+                        continue
+                    else:
                         # NOTE operate in token space to reduce errors
-                        tsmi = "".join(smiles_tokens[:i+1] + ["("] + [fi_smi] + [")"] + smiles_tokens[i+1:])
-                        tidx = list(range(i+1, i+len(fi_smi)+2))
+                        tsmi = "".join(
+                            smiles_tokens[: i + 1]
+                            + ["("]
+                            + [fi_smi]
+                            + [")"]
+                            + smiles_tokens[i + 1 :]
+                        )
+                        tidx = list(range(i + 1, i + len(fi_smi) + 2))
                         temp_smiles.append((tsmi, tidx))
                 if temp_smiles:
                     # Select best position
                     temp_nlls = self.evaluate_fn([smi for smi, _ in temp_smiles])
-                    (smiles, fidxs), nll = sorted(zip(temp_smiles, temp_nlls), key=lambda x: x[1])[0]
-                    smiles_tokens = self.tokenizer.tokenize(smiles, with_begin_and_end=False)
+                    (smiles, fidxs), nll = sorted(
+                        zip(temp_smiles, temp_nlls), key=lambda x: x[1]
+                    )[0]
+                    smiles_tokens = self.tokenizer.tokenize(
+                        smiles, with_begin_and_end=False
+                    )
                     batch_smiles.append(smiles)
                     frag_indexes.extend(fidxs)
                 else:
                     # Don't add fragment
                     batch_smiles.append(smiles)
                 n_rem -= 1
         else:
@@ -542,129 +656,179 @@
             exists = False
             if detect_existing:
                 existing_atoms = utils.detect_existing_fragment(smiles, fi.for_smiles)
                 # Get an atom map between atoms and tokens
                 atom_map = self.tokenizer._token2atom_map(smiles_tokens)
                 for match in existing_atoms:
                     # Check it's not generated linker
-                    if (not any([atom_map[aidx] in frag_indexes for aidx in match])):
+                    if not any([atom_map[aidx] in frag_indexes for aidx in match]):
                         # If so, insert fragment indexes, append etc.
                         batch_smiles.append(smiles)
                         n_rem -= 1
                         exists = True
                         break
             if not exists:
                 # Correct rings
                 fi_smi = utils.correct_fragment_ring_numbers(smiles, fi.for_smiles)
                 # Append fragment
                 smiles = smiles + fi_smi
                 # Evaluate
-                nll = self.evaluate_fn([smiles])[0]
                 batch_smiles.append(smiles)
                 n_rem -= 1
 
         if return_all:
             return batch_smiles
         else:
             return batch_smiles[-1]
 
-    def _batch_sample(self, batch_size: int = None, shuffle: bool = None, scan: bool = None, detect_existing: bool = None, return_all: bool = None):
+    def _batch_sample(
+        self,
+        batch_size: int = None,
+        shuffle: bool = None,
+        scan: bool = None,
+        detect_existing: bool = None,
+        return_all: bool = None,
+    ):
         """More efficient sampling assuming the sample_fn can accept a batch of prompts"""
         # Set parameters
-        if not batch_size: batch_size = self.batch_size
-        if not shuffle: shuffle = self.shuffle
-        if not scan: scan = self.scan
-        if not detect_existing: detect_existing = self.detect_existing
-        if not return_all: return_all = self.return_all
-        batch_fragments = [deepcopy(self.fragments) for _ in range(batch_size)] # NOTE repeating with itertools or by *x leads to abberant behaviour with pop removing element from all sublists
+        if not batch_size:
+            batch_size = self.batch_size
+        if not shuffle:
+            shuffle = self.shuffle
+        if not scan:
+            scan = self.scan
+        if not detect_existing:
+            detect_existing = self.detect_existing
+        if not return_all:
+            return_all = self.return_all
+        batch_fragments = [
+            deepcopy(self.fragments) for _ in range(batch_size)
+        ]  # NOTE repeating with itertools or by *x leads to abberant behaviour with pop removing element from all sublists
 
         # Select initial fragments
         prompts = []
         frag_indexes = []
         for bi in range(batch_size):
-            if shuffle: i = random.randint(0, self.n_fgs-1)
-            else: i = 0
+            if shuffle:
+                i = random.randint(0, self.n_fgs - 1)
+            else:
+                i = 0
             f0 = batch_fragments[bi].pop(i)
             f0_tokens = self.tokenizer.tokenize(f0.rev_smiles, with_begin_and_end=False)
             prompts.append(f0.rev_smiles)
             frag_indexes.append(list(range(len(f0_tokens))))
 
         # Sample
         n_rem = self.n_fgs
         batch_smiles = []
-        smiles = self.sample_fn(prompt=prompts, batch_size=batch_size, **self.sample_fn_kwargs)
+        smiles = self.sample_fn(
+            prompt=prompts, batch_size=batch_size, **self.sample_fn_kwargs
+        )
         batch_smiles.append(smiles)
         n_rem -= 1
 
         if self.scan:
             while n_rem:
                 n_smiles = []
-                n_idxs = []
-                for bi, (smiles, fragments, existing_indexes) in enumerate(zip(batch_smiles[-1], batch_fragments, frag_indexes)):
-                    assert smiles.startswith(prompts[bi]), f"Sampled SMILES {smiles} does not start with prompt {prompts[bi]}, why not?"
+                for bi, (smiles, fragments, existing_indexes) in enumerate(
+                    zip(batch_smiles[-1], batch_fragments, frag_indexes)
+                ):
+                    assert smiles.startswith(
+                        prompts[bi]
+                    ), f"Sampled SMILES {smiles} does not start with prompt {prompts[bi]}, why not?"
                     # Select another fragment
-                    if shuffle: i = random.randint(0, n_rem-1)
-                    else: i = 0
+                    if shuffle:
+                        i = random.randint(0, n_rem - 1)
+                    else:
+                        i = 0
                     fi = fragments.pop(i)
                     # Detect existing fragments
                     if detect_existing:
                         exists = False
-                        smiles_tokens = self.tokenizer.tokenize(smiles, with_begin_and_end=False)
-                        existing_atoms = utils.detect_existing_fragment(smiles, fi.for_smiles)
+                        smiles_tokens = self.tokenizer.tokenize(
+                            smiles, with_begin_and_end=False
+                        )
+                        existing_atoms = utils.detect_existing_fragment(
+                            smiles, fi.for_smiles
+                        )
                         # Get an atom map between atoms and tokens
                         atom_map = self.tokenizer._token2atom_map(smiles_tokens)
                         # Check it's not generated linker
                         for match in existing_atoms:
-                            if not any([atom_map[aidx] in frag_indexes for aidx in match]):
+                            if not any(
+                                [atom_map[aidx] in frag_indexes for aidx in match]
+                            ):
                                 # If so, insert fragment indexes, append etc.
-                                frag_indexes[bi].extend([atom_map[aidx] for aidx in match])
+                                frag_indexes[bi].extend(
+                                    [atom_map[aidx] for aidx in match]
+                                )
                                 n_smiles.append(smiles)
                                 exists = True
                                 break
                         if exists:
                             continue
                     # Correct rings
                     fi_smi = utils.correct_fragment_ring_numbers(smiles, fi.for_smiles)
                     # Insert fragment at different positions
-                    smiles_tokens = self.tokenizer.tokenize(smiles, with_begin_and_end=False)
-                    prompt_tokens = self.tokenizer.tokenize(prompts[bi], with_begin_and_end=False)
+                    smiles_tokens = self.tokenizer.tokenize(
+                        smiles, with_begin_and_end=False
+                    )
+                    prompt_tokens = self.tokenizer.tokenize(
+                        prompts[bi], with_begin_and_end=False
+                    )
                     temp_smiles = []
-                    for i in range(len(prompt_tokens)-1, len(smiles_tokens)):
-                        if i in existing_indexes: 
-                            continue 
-                        else: 
-                            tsmi = "".join(smiles_tokens[:i+1] + ["("] + [fi_smi] + [")"] + smiles_tokens[i+1:])
-                            tidx = list(range(i+1, i+len(fi_smi)+2))
+                    for i in range(len(prompt_tokens) - 1, len(smiles_tokens)):
+                        if i in existing_indexes:
+                            continue
+                        else:
+                            tsmi = "".join(
+                                smiles_tokens[: i + 1]
+                                + ["("]
+                                + [fi_smi]
+                                + [")"]
+                                + smiles_tokens[i + 1 :]
+                            )
+                            tidx = list(range(i + 1, i + len(fi_smi) + 2))
                             temp_smiles.append((tsmi, tidx))
                     if temp_smiles:
                         # Select best position
                         temp_nlls = self.evaluate_fn([smi for smi, _ in temp_smiles])
-                        (smiles, fidxs), nll = sorted(zip(temp_smiles, temp_nlls), key=lambda x: x[1])[0]
+                        (smiles, fidxs), nll = sorted(
+                            zip(temp_smiles, temp_nlls), key=lambda x: x[1]
+                        )[0]
                         n_smiles.append(smiles)
                         frag_indexes[bi].extend(fidxs)
                     else:
                         # Don't add fragment
                         n_smiles.append(smiles)
                 batch_smiles.append(n_smiles)
                 n_rem -= 1
         else:
             concat_smiles = []
-            for bi, (smiles, fragments) in enumerate(zip(batch_smiles[0], batch_fragments)):
-                assert smiles.startswith(prompts[bi]), f"Sampled SMILES {smiles} does not start with prompt {prompts[bi]}, why not?"
+            for bi, (smiles, fragments) in enumerate(
+                zip(batch_smiles[0], batch_fragments)
+            ):
+                assert smiles.startswith(
+                    prompts[bi]
+                ), f"Sampled SMILES {smiles} does not start with prompt {prompts[bi]}, why not?"
                 fi = fragments.pop(0)
                 # Detect existing fragments
                 exists = False
                 if detect_existing:
-                    smiles_tokens = self.tokenizer.tokenize(smiles, with_begin_and_end=False)
-                    existing_atoms = utils.detect_existing_fragment(smiles, fi.for_smiles)
+                    smiles_tokens = self.tokenizer.tokenize(
+                        smiles, with_begin_and_end=False
+                    )
+                    existing_atoms = utils.detect_existing_fragment(
+                        smiles, fi.for_smiles
+                    )
                     # Get an atom map between atoms and tokens
                     atom_map = self.tokenizer._token2atom_map(smiles_tokens)
                     for match in existing_atoms:
                         # Check it's not generated linker
-                        if (not any([atom_map[aidx] in frag_indexes for aidx in match])):
+                        if not any([atom_map[aidx] in frag_indexes for aidx in match]):
                             # If so, insert fragment indexes, append etc.
                             concat_smiles.append(smiles)
                             exists = True
                             break
                 if not exists:
                     # Correct rings
                     fi_smi = utils.correct_fragment_ring_numbers(smiles, fi.for_smiles)
@@ -676,34 +840,51 @@
             n_rem -= 1
 
         if return_all:
             return batch_smiles
         else:
             return batch_smiles[-1]
 
-    def sample(self, batch_size: int = None, batch_prompts: bool = None, return_all: bool = None, shuffle: bool = None, scan: bool = None, **kwargs):
+    def sample(
+        self,
+        batch_size: int = None,
+        batch_prompts: bool = None,
+        return_all: bool = None,
+        shuffle: bool = None,
+        scan: bool = None,
+        **kwargs,
+    ):
         """
         Sample de novo molecules, see init docstring for more details.
         """
         # Set parameters
-        if not batch_size: batch_size = self.batch_size
-        if not batch_prompts: batch_prompts = self.batch_prompts
-        if not shuffle: shuffle = self.shuffle
-        if not scan: scan = self.scan
-        if not return_all: return_all = self.return_all
+        if not batch_size:
+            batch_size = self.batch_size
+        if not batch_prompts:
+            batch_prompts = self.batch_prompts
+        if not shuffle:
+            shuffle = self.shuffle
+        if not scan:
+            scan = self.scan
+        if not return_all:
+            return_all = self.return_all
         # Correct scan
         if self.n_fgs > 2 and not self.scan:
-            logger.warn(f"Scan must be used for more than two fragments, Scan will be enabled.")
+            logger.warn(
+                "Scan must be used for more than two fragments, Scan will be enabled."
+            )
             self.scan = True
 
         # Choose _single_sample, iterative _single_sample, or _batch_sample
         if batch_prompts:
-            return self._batch_sample(batch_size=batch_size, shuffle=shuffle, return_all=return_all)
+            return self._batch_sample(
+                batch_size=batch_size, shuffle=shuffle, return_all=return_all
+            )
         else:
             batch_smiles = []
             for i in range(batch_size):
                 smiles = self._single_sample(shuffle=shuffle, return_all=return_all)
                 batch_smiles.append(smiles)
             # Reformat to be the same as batch_prompts
             if return_all:
                 batch_smiles = list(map(list, zip(*batch_smiles)))
-            return batch_smiles
+            return batch_smiles
```

### Comparing `promptsmiles-1.4.1/promptsmiles/utils.py` & `promptsmiles-1.4.2/promptsmiles/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,86 +1,110 @@
 # Copyright Universitat Pompeu Fabra 2020-2023  https://www.compscience.org
 # Distributed under the Apache 2.0 License.
 # (See accompanying file README.md file or copy at https://opensource.org/license/apache-2-0/)
 
-import re
 import copy
-import random
 import logging
+import random
+import re
+
 logger = logging.getLogger("promptsmiles")
-from collections import defaultdict
 
 from rdkit import Chem, RDLogger
-from rdkit.Chem import Descriptors, rdqueries
-import rdkit.Chem.Draw as Draw
+from rdkit.Chem import rdqueries
 
 # TODO Canonicalize to ensure ring atoms have the ring number afterwards (before any branches or )
 
 # REGEX
 SQUARE_BRACKET = re.compile(r"(\[[^\]]*\])")
 SQUARE_BRACKET_noH = re.compile(r"(\[(?:(?!H)[^\]]*)\])")
 BRCL = re.compile(r"(Br|Cl)")
 ATOM = re.compile(r"([a-zA-Z])")
 # ---- RING_ATOM needs some explaining ----
 # An atom followed by ring connections (0-9) or double ring connections (%0-9)
 # The atom may also have an explicit bond to the ring connection -/=/#
 # The atom may also be wrapped in square brackets []
 # The atom should not be *within* square brackets, e.g., "[NH2+]2" is a ring atom but not the "H2" inside it
-RING_ATOM = re.compile(r"([a-zA-Z][%0-9]+(?![^[]*\])|[a-zA-Z][-=#:][%0-9]+(?![^[]*\])|\[[^\]]*\][%0-9]+(?![^[]*\])|\[[^\]]*\][-=#:][%0-9]+(?![^[]*\]))")
+RING_ATOM = re.compile(
+    r"([a-zA-Z][%0-9]+(?![^[]*\])|[a-zA-Z][-=#:][%0-9]+(?![^[]*\])|\[[^\]]*\][%0-9]+(?![^[]*\])|\[[^\]]*\][-=#:][%0-9]+(?![^[]*\]))"
+)
 # The following regex identifies ring numbers seperated by an explicit bond e.g., C2-3, whereas above only recognizes C-2
-RING_ATOM_2 = re.compile(r"([a-zA-Z][%0-9][-=#][%0-9]+(?![^[]*\])|[a-zA-Z][%0-9]+(?![^[]*\])|[a-zA-Z][-=#][%0-9]+(?![^[]*\])|\[[^\]]*\][%0-9][-=#][%0-9]+(?![^[]*\])|\[[^\]]*\][%0-9]+(?![^[]*\])|\[[^\]]*\][-=#][%0-9]+(?![^[]*\]))")
+RING_ATOM_2 = re.compile(
+    r"([a-zA-Z][%0-9][-=#][%0-9]+(?![^[]*\])|[a-zA-Z][%0-9]+(?![^[]*\])|[a-zA-Z][-=#][%0-9]+(?![^[]*\])|\[[^\]]*\][%0-9][-=#][%0-9]+(?![^[]*\])|\[[^\]]*\][%0-9]+(?![^[]*\])|\[[^\]]*\][-=#][%0-9]+(?![^[]*\]))"
+)
 SINGLE_RING = re.compile(r"([0-9]{1})")
 DOUBLE_RING = re.compile(r"(%[0-9]{2})")
 BR_ATTCH = re.compile(r"(\(\*\))")
 ATTCH = re.compile(r"(\*)")
 BR_OPEN = re.compile(r"(\()")
 BR_CLOSE = re.compile(r"(\))")
 BR = re.compile(r"(\(|\))")
 
+
 def disable_rdkit_logging():
-    RDLogger.DisableLog('rdApp.*')
+    RDLogger.DisableLog("rdApp.*")
+
 
 def disable_rdkit_logging_dec(func):
-    def wrapper(*args,  **kwargs):
-        RDLogger.DisableLog('rdApp.*')
+    def wrapper(*args, **kwargs):
+        RDLogger.DisableLog("rdApp.*")
         out = func(*args, **kwargs)
-        RDLogger.EnableLog('rdApp.*')
+        RDLogger.EnableLog("rdApp.*")
         return out
+
     return wrapper
 
+
 class SMILESTokenizer:
     """Deals with the tokenization and untokenization of SMILES."""
 
-    GRAMMAR = 'SMILES'
+    GRAMMAR = "SMILES"
     REGEXPS = {
         "brackets": re.compile(r"(\[[^\]]*\])"),
         "2_ring_nums": re.compile(r"(%\d{2})"),
         "brcl": re.compile(r"(Br|Cl)"),
         "atom": re.compile(r"[a-zA-Z]"),
-        "ring_atom": re.compile(r"([a-zA-Z][%0-9]+(?![^[]*\])|[a-zA-Z][-=#][%0-9]+(?![^[]*\])|\[[^\]]*\][%0-9]+(?![^[]*\])|\[[^\]]*\][-=#][%0-9]+(?![^[]*\]))"),
+        "ring_atom": re.compile(
+            r"([a-zA-Z][%0-9]+(?![^[]*\])|[a-zA-Z][-=#][%0-9]+(?![^[]*\])|\[[^\]]*\][%0-9]+(?![^[]*\])|\[[^\]]*\][-=#][%0-9]+(?![^[]*\]))"
+        ),
     }
-    REGEXP_ORDER = ["ring_atom", "brackets", "brcl"] #["brackets", "2_ring_nums", "brcl"]
+    REGEXP_ORDER = [
+        "ring_atom",
+        "brackets",
+        "brcl",
+    ]  # ["brackets", "2_ring_nums", "brcl"]
 
     def __init__(self):
         self.GRAMMAR = copy.deepcopy(self.GRAMMAR)
         self.REGEXPS = copy.deepcopy(self.REGEXPS)
         self.REGEXP_ORDER = copy.deepcopy(self.REGEXP_ORDER)
 
     def _token2atom_map(self, tokens):
         """Given a list of tokens that tokenizes at least by atom e.g., Br / Cl / [NH2+]"""
         atom_map = {}
         atom_counter = 0
         for i, t in enumerate(tokens):
-            if any([regex.fullmatch(t) for regex in [self.REGEXPS["ring_atom"], self.REGEXPS["brackets"], self.REGEXPS["brcl"], self.REGEXPS["atom"]]]):
+            if any(
+                [
+                    regex.fullmatch(t)
+                    for regex in [
+                        self.REGEXPS["ring_atom"],
+                        self.REGEXPS["brackets"],
+                        self.REGEXPS["brcl"],
+                        self.REGEXPS["atom"],
+                    ]
+                ]
+            ):
                 atom_map[atom_counter] = i
                 atom_counter += 1
         return atom_map
 
     def tokenize(self, data, with_begin_and_end=True):
         """Tokenizes a SMILES string."""
+
         def split_by(data, regexps):
             if not regexps:
                 return list(data)
             regexp = self.REGEXPS[regexps[0]]
             splitted = regexp.split(data)
             tokens = []
             for i, split in enumerate(splitted):
@@ -101,165 +125,204 @@
         for token in tokens:
             if token == "$":
                 break
             if token != "^":
                 smi += token
         return smi
 
+
 def split_by_regex(data: str, regexes: list):
     if not regexes:
         return list(data)
     regexp = regexes[0]
     splitted = regexp.split(data)
     tokens = []
     for i, split in enumerate(splitted):
         if i % 2 == 0:
             tokens += split_by_regex(split, regexes[1:])
         else:
             tokens.append(split)
     return tokens
 
+
 def int2ring_number(x):
-    if x < 10: 
+    if x < 10:
         return str(x)
-    else: 
-        return "%"+str(x)
+    else:
+        return "%" + str(x)
+
 
 def root_smiles(smi, rootAtom=None, reverse=False):
     """Rearrange SMILES to start at rootAtom"""
     # Convert leading wildcard out of parenthesis if presented that way
-    if smi.startswith('(*)'):
-        smi = re.sub(r'\(\*\)', '*', smi, count=1)
+    if smi.startswith("(*)"):
+        smi = re.sub(r"\(\*\)", "*", smi, count=1)
 
     mol = Chem.MolFromSmiles(smi)
     new_smi = None
     if mol:
         new_smi = Chem.MolToSmiles(mol, rootedAtAtom=rootAtom)
         if reverse:
             # NOTE sometimes RDKit assigns the same ring index to different rings, causing an error upon reversing, so let's re-index if necessary
-            try: new_smi = _check_ring_numbers(new_smi)
-            except Exception as e: logger.error(e); pass
+            try:
+                new_smi = _check_ring_numbers(new_smi)
+            except Exception as e:
+                logger.error(e)
+                pass
             new_smi = reverse_smiles(new_smi)
         # Convert back to (*)
         new_smi = bracket_attachments(new_smi)
     return new_smi
 
-def randomize_smiles(smi, n_rand=10, random_type="restricted", rootAtom=None, reverse=False):
+
+def randomize_smiles(
+    smi, n_rand=10, random_type="restricted", rootAtom=None, reverse=False
+):
     """
     Returns a random SMILES given a SMILES of a molecule.
     :param smi: A SMILES string
     :param n_rand: Number of randomized smiles per molecule
     :param random_type: The type (unrestricted, restricted) of randomization performed.
     :param rootAtom: Root smiles generation to begin with this atom, -1 denotes the last atom)
     :return : A random SMILES string of the same molecule or None if the molecule is invalid.
     """
-    assert random_type in ['restricted', 'unrestricted'], f"Type {random_type} is not valid"
-    
+    assert random_type in [
+        "restricted",
+        "unrestricted",
+    ], f"Type {random_type} is not valid"
+
     # Convert leading wildcard out of parenthesis if presented that way
-    if smi.startswith('(*)'):
-        smi = re.sub(r'\(\*\)', '*', smi, count=1)
+    if smi.startswith("(*)"):
+        smi = re.sub(r"\(\*\)", "*", smi, count=1)
 
     mol = Chem.MolFromSmiles(smi)
-    if not mol: return None
+    if not mol:
+        return None
 
     if random_type == "unrestricted":
         rand_smiles = []
         for i in range(n_rand):
             if rootAtom is not None:
                 if rootAtom == -1:
-                    rootAtom = mol.GetNumAtoms()-1
-                random_smiles = Chem.MolToSmiles(mol, canonical=False, doRandom=True, isomericSmiles=False, rootedAtAtom=rootAtom)
+                    rootAtom = mol.GetNumAtoms() - 1
+                random_smiles = Chem.MolToSmiles(
+                    mol,
+                    canonical=False,
+                    doRandom=True,
+                    isomericSmiles=False,
+                    rootedAtAtom=rootAtom,
+                )
             else:
-                random_smiles = Chem.MolToSmiles(mol, canonical=False, doRandom=True, isomericSmiles=False)
-            
+                random_smiles = Chem.MolToSmiles(
+                    mol, canonical=False, doRandom=True, isomericSmiles=False
+                )
+
             if reverse:
-                assert "*" not in smi, "Unexpected behaviour when smiles contain a wildcard character (*), please use restricted randomization"
+                assert (
+                    "*" not in smi
+                ), "Unexpected behaviour when smiles contain a wildcard character (*), please use restricted randomization"
                 random_smiles = reverse_smiles(random_smiles)
 
             # Convert back to (*)
             random_smiles = bracket_attachments(random_smiles)
-            
+
             rand_smiles.append(random_smiles)
-                
+
         return list(set(rand_smiles))
 
     if random_type == "restricted":
         rand_smiles = []
         i = 0
         attempts = 0
         while (i < n_rand) and (attempts < 50):
             attempts += 1
             if rootAtom is not None:
                 new_atom_order = list(range(mol.GetNumAtoms()))
-                root_atom = new_atom_order.pop(rootAtom) # -1
+                root_atom = new_atom_order.pop(rootAtom)  # -1
                 random.shuffle(new_atom_order)
                 new_atom_order = [root_atom] + new_atom_order
                 random_mol = Chem.RenumberAtoms(mol, newOrder=new_atom_order)
-                random_smiles = Chem.MolToSmiles(random_mol, canonical=False, isomericSmiles=True)
+                random_smiles = Chem.MolToSmiles(
+                    random_mol, canonical=False, isomericSmiles=True
+                )
             else:
                 new_atom_order = list(range(mol.GetNumAtoms()))
                 random.shuffle(new_atom_order)
                 random_mol = Chem.RenumberAtoms(mol, newOrder=new_atom_order)
-                random_smiles = Chem.MolToSmiles(random_mol, canonical=False, isomericSmiles=True)
+                random_smiles = Chem.MolToSmiles(
+                    random_mol, canonical=False, isomericSmiles=True
+                )
 
             if reverse:
                 # NOTE sometimes RDKit assigns the same ring index to different rings, causing an error upon reversing, so let's re-index if necessary
-                try: random_smiles = _check_ring_numbers(random_smiles)
-                except Exception as e: logger.error(e); pass
+                try:
+                    random_smiles = _check_ring_numbers(random_smiles)
+                except Exception as e:
+                    logger.error(e)
+                    pass
                 random_smiles = reverse_smiles(random_smiles)
 
             # Convert back to (*)
             random_smiles = bracket_attachments(random_smiles)
-                
+
             rand_smiles.append(random_smiles)
             i += 1
 
         return list(set(rand_smiles))
 
+
 def reverse_smiles(smiles, renumber_rings=True, v=False):
     """
     Reverse a SMILES string
     """
-    if v: print(f'Reversing: {smiles}')
+    if v:
+        print(f"Reversing: {smiles}")
 
     # Tokenize
     tokens = split_by_regex(smiles, [RING_ATOM_2, SQUARE_BRACKET, BRCL, ATTCH, ATOM])
-    if v: print(f'Tokenized:\n\t{tokens}')
+    if v:
+        print(f"Tokenized:\n\t{tokens}")
 
     # Find parenthesis
     branching_idxs = _seek_parenthesis(tokens)
-    if v: print(f'Branches identified:\n\t{branching_idxs}')
+    if v:
+        print(f"Branches identified:\n\t{branching_idxs}")
 
     # Merge branches with source atom
     new_tokens = []
     i = 0
     while i < len(tokens):
         # Check if we need to combine branches into one token
-        if i+1 in branching_idxs:
-            t = "".join(tokens[i:branching_idxs[i+1]+1])
+        if i + 1 in branching_idxs:
+            t = "".join(tokens[i : branching_idxs[i + 1] + 1])
             new_tokens.append(t)
-            i = branching_idxs[i+1] + 1
+            i = branching_idxs[i + 1] + 1
         else:
             new_tokens.append(tokens[i])
             i += 1
-    if v: print(f'Tokens corrected by branch:\n\t{new_tokens}')
+    if v:
+        print(f"Tokens corrected by branch:\n\t{new_tokens}")
 
     # Reverse
     rev_tokens = list(reversed(new_tokens))
     rsmiles = "".join(rev_tokens)
-    if v: print(f'Tokens reversed:\n\t{rev_tokens}')
-    if v: print(f'SMILES reversed: {rsmiles}')
+    if v:
+        print(f"Tokens reversed:\n\t{rev_tokens}")
+    if v:
+        print(f"SMILES reversed: {rsmiles}")
 
     # Re-number rings
     if renumber_rings:
         rsmiles = _reverse_ring_numbers(rsmiles)
-        if v: print(f'Rings reindexed:\n\t {rsmiles}')
+        if v:
+            print(f"Rings reindexed:\n\t {rsmiles}")
 
     return rsmiles
 
+
 def _reverse_ring_numbers(smi: str) -> str:
     """Given ring numbers in smi, reindex the rings in smi from left to right"""
     ring_map = {}
     ring_count = 1
     new_smiles = []
     for c in split_by_regex(smi, [SQUARE_BRACKET, BRCL, DOUBLE_RING, SINGLE_RING]):
         if SINGLE_RING.fullmatch(c) or DOUBLE_RING.fullmatch(c):
@@ -270,201 +333,240 @@
             # Update ring close
             c = ring_map[c]
         # Add token
         new_smiles.append(c)
     smiles = "".join(new_smiles)
     return smiles
 
+
 def _check_ring_numbers(smiles, debug=False, v=False):
     """Check and re-index ring numbers sequentially if needed"""
     mol = Chem.MolFromSmiles(smiles)
     ringinfo = mol.GetRingInfo()
     N_rings = ringinfo.NumRings()
-    L_rings = [int(t.strip("%")) for t in DOUBLE_RING.findall(smiles) + SINGLE_RING.findall(smiles)]
+    L_rings = [
+        int(t.strip("%"))
+        for t in DOUBLE_RING.findall(smiles) + SINGLE_RING.findall(smiles)
+    ]
     if L_rings:
         L_rings = max(L_rings)
 
     # ---- Check rings
     if (not L_rings) or (L_rings == N_rings):
         # Assume they're labelled correctly
         return smiles
 
     # ---- Otherwise let's re-index
     rings = list(ringinfo.AtomRings())
-    if v: print(rings)
+    if v:
+        print(rings)
     tokens = split_by_regex(smiles, [SQUARE_BRACKET, DOUBLE_RING, BRCL])
 
     ring_count = 0
-    atom_count = -1 # Counting what the last atom was
-    ring_map = {} # {old_ring -> new_ring}
+    atom_count = -1  # Counting what the last atom was
+    ring_map = {}  # {old_ring -> new_ring}
     new_tokens = []
     for i, t in enumerate(tokens):
         # If it's a ring token -> update
         if any([regex.fullmatch(t) for regex in [DOUBLE_RING, SINGLE_RING]]):
-            if debug: import pdb; pdb.set_trace()
-            mapped = False
+            if debug:
+                import pdb
+
+                pdb.set_trace()
             # Check to see if it's already mapped
             if t in ring_map.keys():
                 new_tokens.append(ring_map[t])
-                if v: print(f"Relabelled {t} -> {ring_map[t]} at atom {atom_count}")
+                if v:
+                    print(f"Relabelled {t} -> {ring_map[t]} at atom {atom_count}")
                 ring_map.pop(t)
             else:
                 # Add it
                 ring_count += 1
                 new_ring_id = int2ring_number(ring_count)
                 ring_map[t] = new_ring_id
                 new_tokens.append(new_ring_id)
-                if v: print(f"Relabelled {t} -> {new_ring_id} at atom {atom_count}")
+                if v:
+                    print(f"Relabelled {t} -> {new_ring_id} at atom {atom_count}")
         # If it's an atom -> count
-        elif any([regex.fullmatch(t) for regex in [SQUARE_BRACKET_noH, BRCL, ATOM, BR_ATTCH, ATTCH]]):
+        elif any(
+            [
+                regex.fullmatch(t)
+                for regex in [SQUARE_BRACKET_noH, BRCL, ATOM, BR_ATTCH, ATTCH]
+            ]
+        ):
             atom_count += 1
             new_tokens.append(t)
         else:
             new_tokens.append(t)
-    if v: print(ring_map)
+    if v:
+        print(ring_map)
     new_smiles = "".join(new_tokens)
     logger.debug(f"Re-indexed SMILES rings from {smiles} -> {new_smiles}")
     return new_smiles
 
+
 def _seek_parenthesis(smiles_or_tokens):
     """
     Return the indices of top level parenthesis only as a dict map
     """
     br_open = 0
     multiple = False
-    open_close_idxs = {} # {idx1: idx2}
+    open_close_idxs = {}  # {idx1: idx2}
     for i, t in enumerate(smiles_or_tokens):
         # Open
         if BR_OPEN.fullmatch(t):
             # If first open, save index
             if (br_open == 0) and not multiple:
-                br_open_idx = i  
+                br_open_idx = i
             br_open += 1
             multiple = False
         # Close
         if BR_CLOSE.fullmatch(t):
             br_open -= 1
             # If last close, save index
             if br_open == 0:
                 # Check to see we aren't immediately branching afterwards
-                if (i < len(smiles_or_tokens)-1) and BR_OPEN.fullmatch(smiles_or_tokens[i+1]):
+                if (i < len(smiles_or_tokens) - 1) and BR_OPEN.fullmatch(
+                    smiles_or_tokens[i + 1]
+                ):
                     multiple = True
                 else:
                     br_close_idx = i
                     open_close_idxs[br_open_idx] = br_close_idx
     return open_close_idxs
 
+
 def _seek_source_atom(smiles_or_tokens, idx):
     found = False
     br_open = 0
     while not found:
-        idx = idx-1
+        idx = idx - 1
         t = smiles_or_tokens[idx]
         # NOTE opposite because in reverse
         if BR_CLOSE.fullmatch(t):
             br_open += 1
         if BR_OPEN.fullmatch(t):
             br_open += -1
         # If there's no branches open and we're not opening another
         if (br_open == 0) and not BR.fullmatch(t):
             found = True
     return idx
 
+
 def get_attachment_points(smi: str, return_map: bool = False) -> list:
-    tokens = split_by_regex(smi, [RING_ATOM, SQUARE_BRACKET, BRCL, BR_ATTCH, ATTCH, ATOM])
+    tokens = split_by_regex(
+        smi, [RING_ATOM, SQUARE_BRACKET, BRCL, BR_ATTCH, ATTCH, ATOM]
+    )
     atom_counter = 0
     all_counter = 0
     token2atom_map = {}
     attch2dummy_map = {}
     for ti, t in enumerate(tokens):
-        
         if ATTCH.fullmatch(t) or BR_ATTCH.fullmatch(t):
             # If it's the first atom
             if ti == 0:
                 # Seek next atom...
                 attch2dummy_map[atom_counter] = all_counter
             # NOTE correcting for preceeding branches i.e., see previous atom...
-            elif (ti > 0) and BR_CLOSE.fullmatch(tokens[ti-1]):
+            elif (ti > 0) and BR_CLOSE.fullmatch(tokens[ti - 1]):
                 source_ti = _seek_source_atom(tokens, ti)
                 attch2dummy_map[token2atom_map[source_ti]] = all_counter
             # Otherwise it's the previous atom
             else:
-                attch2dummy_map[atom_counter-1] = all_counter
+                attch2dummy_map[atom_counter - 1] = all_counter
             all_counter += 1
 
-        if any([regex.fullmatch(t) for regex in [RING_ATOM, SQUARE_BRACKET_noH, BRCL, ATOM]]):
+        if any(
+            [
+                regex.fullmatch(t)
+                for regex in [RING_ATOM, SQUARE_BRACKET_noH, BRCL, ATOM]
+            ]
+        ):
             token2atom_map[ti] = atom_counter
             atom_counter += 1
             all_counter += 1
 
     if return_map:
         return attch2dummy_map
     else:
         return list(attch2dummy_map.keys())
 
+
 def insert_attachment_points(smi: str, at_pts: list):
-    tokens = split_by_regex(smi, [RING_ATOM, SQUARE_BRACKET, BRCL, BR_ATTCH, ATTCH, ATOM])
+    tokens = split_by_regex(
+        smi, [RING_ATOM, SQUARE_BRACKET, BRCL, BR_ATTCH, ATTCH, ATOM]
+    )
     atom_counter = 0
     new_tokens = []
     for t in tokens:
         new_tokens.append(t)
-        if any([regex.fullmatch(t) for regex in [RING_ATOM, SQUARE_BRACKET_noH, BRCL, ATOM]]):
+        if any(
+            [
+                regex.fullmatch(t)
+                for regex in [RING_ATOM, SQUARE_BRACKET_noH, BRCL, ATOM]
+            ]
+        ):
             if atom_counter in at_pts:
                 new_tokens.append("(*)")
             atom_counter += 1
-    smi = ''.join(new_tokens)
+    smi = "".join(new_tokens)
     return smi
 
+
 def correct_attachment_point(smi: str, at_pt: int) -> int:
     """Switch attachment point index to wildcard index in atom"""
     attch2dummy_map = get_attachment_points(smi, return_map=True)
     return attch2dummy_map[at_pt]
 
+
 def strip_attachment_points(smi: str):
     """
     Remove * and provide canonical SMILES
     :param smi: SMILES with (*)
     :return: SMILES without (*), Atom index of attachment points
     """
     at_pts = get_attachment_points(smi)
     smi = smi.replace("(*)", "").replace("*", "")
     return smi, at_pts
 
+
 def bracket_attachments(smi):
     """
     Convert all * to ensure they are branching points (*)
     """
     # Replace start
     nsmi = re.sub(r"^(\*)([a-zA-Z][0-9]?)", "\\2(\\1)", smi)
     # Replace end
     nsmi = re.sub(r"(\*)$", "(\\1)", nsmi)
     # Replace un-isolated
     nsmi = re.sub(r"([^(])(\*)", "\\1(\\2)", nsmi)
     nsmi = re.sub(r"(\*)([^)])", "(\\1)\\2", nsmi)
     return nsmi
 
+
 # ----- Useful functions for fragment linking specifically -----
 
+
 def extract_linker(smiles, fragments=[], return_all=False):
     mol = Chem.MolFromSmiles(smiles)
-    
+
     if not mol:
         return None
 
     # Sort frags by largest SMILES first
     fragments = sorted(fragments, key=lambda x: len(x), reverse=True)
 
     for frag in fragments:
         # Get frag
-        sfrag, _ = strip_attachment_points(frag) ###
+        sfrag, _ = strip_attachment_points(frag)  ###
         # Remove explicit Hs as no substructure match otherwise (RDKit seems to have a bug, doesn't work)
         sfrag = re.sub(r"\[([a-zA-Z])H\]", "\\1", sfrag)
         fmol = Chem.MolFromSmiles(sfrag)
         # Get attachment point
-        for match in mol.GetSubstructMatches(fmol): 
+        for match in mol.GetSubstructMatches(fmol):
             fragment_point = set()
             attachment_points = set()
             for idx in match:
                 atom = mol.GetAtomWithIdx(idx)
                 neighbour_atoms = atom.GetNeighbors()
                 for natom in neighbour_atoms:
                     nidx = natom.GetIdx()
@@ -474,90 +576,98 @@
             if len(fragment_point) == 1:
                 break
 
         # An end fragment should have exactly one fragment atom attached
         # This may cause an error if the RNN has added the exact same fragment in the middle of the linker
         if not mol.HasSubstructMatch(fmol) or (len(fragment_point) != 1):
             return None
-        
+
         # Add attachment points
         mol = Chem.RWMol(mol)
         fp = fragment_point.pop()
         mol.AddAtom(Chem.AtomFromSmiles("*"))
         for ap in attachment_points:
             # Get bond type first
             fatom_bonds = mol.GetAtomWithIdx(fp).GetBonds()
-            fl_bond_type = [bond.GetBondType() for bond in fatom_bonds if (bond.GetBeginAtomIdx() == ap) or (bond.GetEndAtomIdx() == ap)][0]
+            fl_bond_type = [
+                bond.GetBondType()
+                for bond in fatom_bonds
+                if (bond.GetBeginAtomIdx() == ap) or (bond.GetEndAtomIdx() == ap)
+            ][0]
             # Add bond
-            mol.AddBond(ap, mol.GetNumAtoms()-1, fl_bond_type)
+            mol.AddBond(ap, mol.GetNumAtoms() - 1, fl_bond_type)
         # Delete substructure match
         mol.BeginBatchEdit()
         for aid in match:
             mol.RemoveAtom(aid)
         mol.CommitBatchEdit()
         try:
             Chem.SanitizeMol(mol)
-        except:
+        except Exception:
             return None
 
     linker = Chem.MolToSmiles(mol)
     if "." in linker:
-        links = [f.count("*") for i, f in enumerate(linker.split("."))]
-        linker = sorted(linker.split("."), key=lambda x: f.count("*"))[-1]
+        linker = sorted(linker.split("."), key=lambda x: x.count("*"))[-1]
 
     return linker
 
+
 def _smiles2smarts(smiles):
     """Convert a SMILES sequence to a more specific SMARTS query including degree, aromaticity and ring membership"""
     smiles = smiles.replace("(*)", "*")
     mol = Chem.MolFromSmiles(smiles)
     mol2 = Chem.RWMol(mol)
     for i, at in enumerate(mol.GetAtoms()):
         if at.GetSymbol() == "*":
             continue
         num = at.GetAtomicNum()
         degree = at.GetDegree()
         aromatic = at.GetIsAromatic()
         ring = at.IsInRing()
         q = rdqueries.AtomNumEqualsQueryAtom(num)
         q.ExpandQuery(rdqueries.ExplicitDegreeEqualsQueryAtom(degree))
-        if aromatic: q.ExpandQuery(rdqueries.IsAromaticQueryAtom())
-        if ring: q.ExpandQuery(rdqueries.IsInRingQueryAtom())
+        if aromatic:
+            q.ExpandQuery(rdqueries.IsAromaticQueryAtom())
+        if ring:
+            q.ExpandQuery(rdqueries.IsInRingQueryAtom())
         mol2.ReplaceAtom(i, q)
     smarts = Chem.MolToSmarts(mol2)
     smarts = smarts.replace("[#0]", "[*]")
     return smarts
 
+
 def correct_fragment_ring_numbers(smi1: str, smi2: str) -> str:
     """Given the rings in smi1, reindex the rings in smi2"""
     # Count rings in smi1
     ring_count = 0
     for c in split_by_regex(smi1, [SQUARE_BRACKET, BRCL, DOUBLE_RING, SINGLE_RING]):
         # Check for number
         if SINGLE_RING.fullmatch(c) or DOUBLE_RING.fullmatch(c):
             # Count max ring index
             ring_count = max(ring_count, int(c.strip("%")))
-    
+
     # Reindex smi2
     ring_map = {}
-    ring_count += 1 # Start from next index
+    ring_count += 1  # Start from next index
     new_smi2 = []
     for c in split_by_regex(smi2, [SQUARE_BRACKET, BRCL, DOUBLE_RING, SINGLE_RING]):
         # Check for number
         if SINGLE_RING.fullmatch(c) or DOUBLE_RING.fullmatch(c):
             # Add new ring to map
             if c not in ring_map.keys():
                 ring_map[c] = int2ring_number(ring_count)
                 ring_count += 1
             # Update c
             c = ring_map[c]
         # Add token
         new_smi2.append(c)
     return "".join(new_smi2)
 
+
 def detect_existing_fragment(smiles, frag_smiles):
     """Get substructure match for frag smiles (with attachment index first)"""
     frag_indexes = []
     mol = Chem.MolFromSmiles(smiles)
     # Fragment must start with attachment point
     if not frag_smiles.startswith("(*)"):
         frag_smiles = "(*)" + frag_smiles
@@ -567,47 +677,49 @@
         if mol.HasSubstructMatch(frag_patt):
             frag_indexes = list(mol.GetSubstructMatches(frag_patt))
     # NOTE that now we ignore the first atom i.e., the attachment point
     if frag_indexes:
         frag_indexes = [list(match)[1:] for match in frag_indexes]
     return frag_indexes
 
+
 # ----- Useful functions for testing -----
 def smiles_eq(smi1, smi2):
     mol1 = Chem.MolFromSmiles(smi1)
     mol2 = Chem.MolFromSmiles(smi2)
     # Parse them
     if not mol1:
-        return False, f'Parsing error: {smi1}'
+        return False, f"Parsing error: {smi1}"
     if not mol2:
-        return False, f'Parsing error: {smi2}'
+        return False, f"Parsing error: {smi2}"
     # Remove atom map
     for mol in [mol1, mol2]:
         for atom in mol.GetAtoms():
             atom.SetAtomMapNum(0)
     # Check smiles are the same
     nsmi1 = Chem.MolToSmiles(mol1)
     nsmi2 = Chem.MolToSmiles(mol2)
     if nsmi1 != nsmi2:
-        return False, f'Inequivalent SMILES: {nsmi1} vs {nsmi2}'
+        return False, f"Inequivalent SMILES: {nsmi1} vs {nsmi2}"
     # Check InChi
     inchi1 = Chem.MolToInchi(mol1)
     inchi2 = Chem.MolToInchi(mol2)
     if inchi1 != inchi2:
-        return False, f'Inequivalent InChi\'s'
+        return False, "Inequivalent InChi's"
     return True, ""
 
+
 def mol_eq(mol1, mol2):
     mols = []
     # Remove atom map
     for mol in [mol1, mol2]:
         if isinstance(mol, str):
             mol = Chem.MolFromSmiles(mol)
         for atom in mol.GetAtoms():
             atom.SetAtomMapNum(0)
         mols.append(mol)
     # Check InChi
     inchi1 = Chem.MolToInchi(mols[0])
     inchi2 = Chem.MolToInchi(mols[1])
     if inchi1 != inchi2:
-        return False, f'Inequivalent InChi\'s'
+        return False, "Inequivalent InChi's"
     return True, ""
```

### Comparing `promptsmiles-1.4.1/promptsmiles.egg-info/PKG-INFO` & `promptsmiles-1.4.2/promptsmiles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptsmiles
-Version: 1.4.1
+Version: 1.4.2
 Summary: A conveniant package to manipulate SMILES strings for iterative prompting with chemical language models.
 Author-email: Morgan Thomas <morganthomas263@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -257,15 +257,15 @@
 FL = FragmentLinker(
     fragments=["N1(*)CCNCC1", "C1CC1(*)"],
     batch_size=64,
     sample_fn=CLM.sampler,
     evaluate_fn=CLM.evaluater,
     batch_prompts=False,
     optimize_prompts=True,
-    shuffle=True, 
+    shuffle=True,
     scan=False, # Optional when combining 2 fragments, otherwise is set to true
     return_all=False,
 )
 smiles = FL.sample(batch_size=3)
 ```
 ![alt text](https://github.com/MorganCThomas/PromptSMILES/blob/main/images/frag_link_example.png)
 ## Required chemical language model functions
```

### Comparing `promptsmiles-1.4.1/pyproject.toml` & `promptsmiles-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 exclude = ["images*", "tests*"]
 
 [project]
 name = "promptsmiles"
-version = "1.4.1"
+version = "1.4.2"
 authors = [
   { name="Morgan Thomas", email="morganthomas263@gmail.com" },
 ]
 description = "A conveniant package to manipulate SMILES strings for iterative prompting with chemical language models."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
@@ -26,8 +26,8 @@
 ]
 dependencies = [
   "rdkit>=2022" # Let's just take a relatively recent cut-off for RDKit
 ]
 
 [project.urls]
 Homepage = "https://github.com/compsciencelab/PromptSMILES"
-Issues = "https://github.com/compsciencelab/PromptSMILES/issues"
+Issues = "https://github.com/compsciencelab/PromptSMILES/issues"
```

### Comparing `promptsmiles-1.4.1/tests/test_samplers.py` & `promptsmiles-1.4.2/tests/test_samplers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,297 +1,321 @@
 # Copyright Universitat Pompeu Fabra 2020-2023  https://www.compscience.org
 # Distributed under the Apache 2.0 License.
 # (See accompanying file README.md file or copy at https://opensource.org/license/apache-2-0/)
 
 import random
+
 import pytest
-from promptsmiles import utils, samplers
+
+from promptsmiles import samplers, utils
+
 
 def evaluate_fn(smiles: list):
     return [random.randint(0, 40) for i in range(len(smiles))]
 
+
 def sample_scaffold_fn(prompt, batch_size):
     """Dummy sampler that adds a F"""
     if isinstance(prompt, list):
-        assert len(prompt) == batch_size, "Prompts provided is not the same as batch size requested"
+        assert (
+            len(prompt) == batch_size
+        ), "Prompts provided is not the same as batch size requested"
         return [prompt[i] + "F" for i in range(batch_size)]
     else:
         return [prompt + "F" for _ in range(batch_size)]
 
+
 def sample_scaffold_fn2(prompt, batch_size):
     """Dummy sampler that adds nothing"""
     if isinstance(prompt, list):
-        assert len(prompt) == batch_size, "Prompts provided is not the same as batch size requested"
+        assert (
+            len(prompt) == batch_size
+        ), "Prompts provided is not the same as batch size requested"
         return [prompt[i] for i in range(batch_size)]
     else:
         return [prompt for _ in range(batch_size)]
 
+
 def sample_linker_fn(prompt, batch_size):
     """Dummy sampler that adds a PEG monomer"""
     if isinstance(prompt, list):
-        assert len(prompt) == batch_size, "Prompts provided is not the same as batch size requested"
+        assert (
+            len(prompt) == batch_size
+        ), "Prompts provided is not the same as batch size requested"
         return [prompt[i] + "CCOCC" for i in range(batch_size)]
     else:
         return [prompt + "CCOCC" for _ in range(batch_size)]
 
+
 def sample_linker_fn2(prompt, batch_size):
     """Dummy sampler that adds nothing"""
     if isinstance(prompt, list):
-        assert len(prompt) == batch_size, "Prompts provided is not the same as batch size requested"
+        assert (
+            len(prompt) == batch_size
+        ), "Prompts provided is not the same as batch size requested"
         return [prompt[i] for i in range(batch_size)]
     else:
         return [prompt for _ in range(batch_size)]
 
+
 # --------------------- Scaffold decoration ---------------------
 scaffold_params = [
-    (
-        "c1c(Cl)c(*)c(*)cc1",
-        "c1c(Cl)c(F)c(F)cc1"
-    ),
-    (
-        "C(*)C1=C(*)C(*)N=C(c2nccs2)N1",
-        "C(F)C1=C(F)C(F)N=C(c2nccs2)N1"
-    ),
+    ("c1c(Cl)c(*)c(*)cc1", "c1c(Cl)c(F)c(F)cc1"),
+    ("C(*)C1=C(*)C(*)N=C(c2nccs2)N1", "C(F)C1=C(F)C(F)N=C(c2nccs2)N1"),
     (
         "C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12",
-        "C(F)c1nc(F)n2[nH]c(-c3c(F)c(F)c(F)c(S(=O)(=O)N4C(F)C(F)N(F)C(F)C4(F))c3(F))nc(=O)c12"
+        "C(F)c1nc(F)n2[nH]c(-c3c(F)c(F)c(F)c(S(=O)(=O)N4C(F)C(F)N(F)C(F)C4(F))c3(F))nc(=O)c12",
     ),
     (
         "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
-        "C(F)Oc1c(F)nc(F)c(F)c1-c1c(F)c(F)c(F)c(NC(=O)C(F)c2c(F)c(F)n(C(F))n2)c1(F)"
+        "C(F)Oc1c(F)nc(F)c(F)c1-c1c(F)c(F)c(F)c(NC(=O)C(F)c2c(F)c(F)n(C(F))n2)c1(F)",
     ),
     (
         "C(*)C(*)c1c(*)nc(-c2c(*)c(*)c(*)c(*)c2(*))c(C(*)(C(*)c2c(*)c(*)c(*)c(*)c2(*))NC(=O)C(*)n2nc(C(*)(F))c3c2C(C(*))(F)C2(*)C(*)C32(*))n1",
-        "C(F)C(F)c1c(F)nc(-c2c(F)c(F)c(F)c(F)c2(F))c(C(F)(C(F)c2c(F)c(F)c(F)c(F)c2(F))NC(=O)C(F)n2nc(C(F)(F))c3c2C(C(F))(F)C2(F)C(F)C32(F))n1"
+        "C(F)C(F)c1c(F)nc(-c2c(F)c(F)c(F)c(F)c2(F))c(C(F)(C(F)c2c(F)c(F)c(F)c(F)c2(F))NC(=O)C(F)n2nc(C(F)(F))c3c2C(C(F))(F)C2(F)C(F)C32(F))n1",
     ),
     (
         "C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O",
-        "C(F)C(F)N(C(F)=O)c1c(F)c(F)c(F)c(F)c1(F)N1C(F)C(F)C(F)C(F)C1=O"
+        "C(F)C(F)N(C(F)=O)c1c(F)c(F)c(F)c(F)c1(F)N1C(F)C(F)C(F)C(F)C1=O",
     ),
     (
         "N(*)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O",
-        "N(F)c1c(F)c(F)c(F)c(F)c1(F)N1C(F)C(F)C(F)C(F)C1=O"
-    )  
+        "N(F)c1c(F)c(F)c(F)c(F)c1(F)N1C(F)C(F)C(F)C(F)C1=O",
+    ),
 ]
 
+
 @pytest.mark.parametrize("scaffold,expected", scaffold_params)
 def test_decoration_canonical(scaffold, expected):
     SD = samplers.ScaffoldDecorator(
         scaffold=scaffold,
         batch_size=10,
         sample_fn=sample_scaffold_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=False,
         shuffle=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("scaffold,expected", scaffold_params)
 def test_decoration_shuffle(scaffold, expected):
     SD = samplers.ScaffoldDecorator(
         scaffold=scaffold,
         batch_size=10,
         sample_fn=sample_scaffold_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=False,
         shuffle=True,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("scaffold,expected", scaffold_params)
 def test_decoration_batch_canonical(scaffold, expected):
     SD = samplers.ScaffoldDecorator(
         scaffold=scaffold,
         batch_size=10,
         sample_fn=sample_scaffold_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=True,
         shuffle=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("scaffold,expected", scaffold_params)
 def test_decoration_batch_shuffle(scaffold, expected):
     SD = samplers.ScaffoldDecorator(
         scaffold=scaffold,
         batch_size=10,
         sample_fn=sample_scaffold_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=True,
         shuffle=True,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
 
 # --------------------- Fragment linking ---------------------
-fragment_params1 = [ # frag1, frag2, expected
+fragment_params1 = [  # frag1, frag2, expected
     ("C1CC1(*)", "c1cc(*)cc(Cl)c1", "C1CC1CCOCCc1cc(Cl)ccc1")
 ]
 
+
 @pytest.mark.parametrize("frag1,frag2,expected", fragment_params1)
 def test_linking_canonical(frag1, frag2, expected):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=False,
         shuffle=False,
         scan=False,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("frag1,frag2,expected", fragment_params1)
 def test_linking_shuffle(frag1, frag2, expected):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=False,
         shuffle=True,
         scan=False,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("frag1,frag2,expected", fragment_params1)
 def test_linking_batch_canonical(frag1, frag2, expected):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=True,
         shuffle=False,
         scan=False,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("frag1,frag2,expected", fragment_params1)
 def test_linking_batch_shuffle(frag1, frag2, expected):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=True,
         shuffle=True,
         scan=False,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("frag1,frag2,expected", fragment_params1)
 def test_linking_scan(frag1, frag2, expected):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=False,
         shuffle=True,
         scan=True,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     # Extract linker, and check it's what we expect
     for smiles in denovo:
         linker = utils.extract_linker(smiles, [frag1, frag2])
         if linker:
             assert utils.strip_attachment_points(linker)[0] == "CCOCC"
 
+
 @pytest.mark.parametrize("frag1,frag2,expected", fragment_params1)
 def test_linking_batch_scan(frag1, frag2, expected):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=True,
         shuffle=True,
         scan=True,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     # Extract linker, and check it's what we expect
     for smiles in denovo:
         linker = utils.extract_linker(smiles, [frag1, frag2])
         if linker:
             assert utils.strip_attachment_points(linker)[0] == "CCOCC"
 
+
 # --------------------- Fragment linking more than two fragments -------------------
 
-fragment_params2 = [ # frag1, frag2, frag3
+fragment_params2 = [  # frag1, frag2, frag3
     ("C1CC1(*)", "c1cc(*)cc(Cl)c1", "N1(*)CCC1")
 ]
+
+
 @pytest.mark.parametrize("frag1,frag2,frag3", fragment_params2)
-def test_linking_scan(frag1, frag2, frag3):
+def test_linking_scan_multi(frag1, frag2, frag3):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2, frag3],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=False,
         shuffle=True,
         scan=True,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     # Extract linker, and check it's what we expect
     for smiles in denovo:
         linker = utils.extract_linker(smiles, [frag1, frag2, frag3])
         if linker:
             assert utils.smiles_eq(utils.strip_attachment_points(linker)[0], "CCOCC")[0]
 
+
 @pytest.mark.parametrize("frag1,frag2,frag3", fragment_params2)
-def test_linking_batch_scan(frag1, frag2, frag3):
+def test_linking_batch_scan_multi(frag1, frag2, frag3):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2, frag3],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=True,
         shuffle=True,
         scan=True,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     # Extract linker, and check it's what we expect
     for smiles in denovo:
         linker = utils.extract_linker(smiles, [frag1, frag2, frag3])
         if linker:
-            assert utils.smiles_eq(utils.strip_attachment_points(linker)[0], "CCOCC")[0]
+            assert utils.smiles_eq(utils.strip_attachment_points(linker)[0], "CCOCC")[0]
```

### Comparing `promptsmiles-1.4.1/tests/test_samplers2.py` & `promptsmiles-1.4.2/tests/test_samplers2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,267 +1,300 @@
 # Copyright Universitat Pompeu Fabra 2020-2023  https://www.compscience.org
 # Distributed under the Apache 2.0 License.
 # (See accompanying file README.md file or copy at https://opensource.org/license/apache-2-0/)
 
 import random
+
 import pytest
-from promptsmiles import utils, samplers
+
+from promptsmiles import samplers, utils
+
 
 def evaluate_fn(smiles: list):
     return [random.randint(0, 40) for i in range(len(smiles))]
 
+
 def sample_scaffold_fn(prompt, batch_size):
     """Dummy sampler that adds nothing"""
     if isinstance(prompt, list):
-        assert len(prompt) == batch_size, "Prompts provided is not the same as batch size requested"
+        assert (
+            len(prompt) == batch_size
+        ), "Prompts provided is not the same as batch size requested"
         return [prompt[i] for i in range(batch_size)]
     else:
         return [prompt for _ in range(batch_size)]
 
+
 def sample_linker_fn(prompt, batch_size):
     """Dummy sampler that adds nothing"""
     if isinstance(prompt, list):
-        assert len(prompt) == batch_size, "Prompts provided is not the same as batch size requested"
+        assert (
+            len(prompt) == batch_size
+        ), "Prompts provided is not the same as batch size requested"
         return [prompt[i] for i in range(batch_size)]
     else:
         return [prompt for _ in range(batch_size)]
 
+
 # --------------------- Scaffold decoration ---------------------
 scaffold_params = [
-    (
-        "c1c(Cl)c(*)c(*)cc1",
-        "c1c(Cl)cccc1"
-    ),
-    (
-        "C(*)C1=C(*)C(*)N=C(c2nccs2)N1",
-        "CC1=CCN=C(c2nccs2)N1"
-    ),
+    ("c1c(Cl)c(*)c(*)cc1", "c1c(Cl)cccc1"),
+    ("C(*)C1=C(*)C(*)N=C(c2nccs2)N1", "CC1=CCN=C(c2nccs2)N1"),
     (
         "C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12",
-        "Cc1ncn2[nH]c(-c3ccc(F)c(S(=O)(=O)N4CCNCC4)c3)nc(=O)c12"
+        "Cc1ncn2[nH]c(-c3ccc(F)c(S(=O)(=O)N4CCNCC4)c3)nc(=O)c12",
     ),
     (
         "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
-        "COc1cnccc1-c1cccc(NC(=O)Cc2ccn(C)n2)c1"
+        "COc1cnccc1-c1cccc(NC(=O)Cc2ccn(C)n2)c1",
     ),
     (
         "C(*)C(*)c1c(*)nc(-c2c(*)c(*)c(*)c(*)c2(*))c(C(*)(C(*)c2c(*)c(*)c(*)c(*)c2(*))NC(=O)C(*)n2nc(C(*)(F))c3c2C(C(*))(F)C2(*)C(*)C32(*))n1",
-        "CCc1cnc(-c2ccccc2)c(C(Cc2ccccc2)NC(=O)Cn2nc(C)c3c2C(C)C2CC32)n1"
+        "CCc1cnc(-c2ccccc2)c(C(Cc2ccccc2)NC(=O)Cn2nc(C)c3c2C(C)C2CC32)n1",
     ),
     (
         "C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O",
-        "CCN(C=O)c1ccccc1N1CCCCC1=O"
+        "CCN(C=O)c1ccccc1N1CCCCC1=O",
     ),
-    (
-        "N(*)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O",
-        "Nc1ccccc1N1CCCCC1=O"
-    )  
+    ("N(*)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O", "Nc1ccccc1N1CCCCC1=O"),
 ]
 
+
 @pytest.mark.parametrize("scaffold,expected", scaffold_params)
 def test_decoration_canonical(scaffold, expected):
     SD = samplers.ScaffoldDecorator(
         scaffold=scaffold,
         batch_size=10,
         sample_fn=sample_scaffold_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=False,
         shuffle=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("scaffold,expected", scaffold_params)
 def test_decoration_shuffle(scaffold, expected):
     SD = samplers.ScaffoldDecorator(
         scaffold=scaffold,
         batch_size=10,
         sample_fn=sample_scaffold_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=False,
         shuffle=True,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("scaffold,expected", scaffold_params)
 def test_decoration_batch_canonical(scaffold, expected):
     SD = samplers.ScaffoldDecorator(
         scaffold=scaffold,
         batch_size=10,
         sample_fn=sample_scaffold_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=True,
         shuffle=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("scaffold,expected", scaffold_params)
 def test_decoration_batch_shuffle(scaffold, expected):
     SD = samplers.ScaffoldDecorator(
         scaffold=scaffold,
         batch_size=10,
         sample_fn=sample_scaffold_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=True,
         shuffle=True,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
 
 # --------------------- Fragment linking ---------------------
-fragment_params1 = [ # frag1, frag2, expected
+fragment_params1 = [  # frag1, frag2, expected
     ("C1CC1(*)", "c1cc(*)cc(Cl)c1", "C1CC1-c1cc(Cl)ccc1")
 ]
 
+
 @pytest.mark.parametrize("frag1,frag2,expected", fragment_params1)
 def test_linking_canonical(frag1, frag2, expected):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=False,
         shuffle=False,
         scan=False,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("frag1,frag2,expected", fragment_params1)
 def test_linking_shuffle(frag1, frag2, expected):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=False,
         shuffle=True,
         scan=False,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("frag1,frag2,expected", fragment_params1)
 def test_linking_batch_canonical(frag1, frag2, expected):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=True,
         shuffle=False,
         scan=False,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("frag1,frag2,expected", fragment_params1)
 def test_linking_batch_shuffle(frag1, frag2, expected):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=True,
         shuffle=True,
         scan=False,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     assert len(denovo) == 10
     assert all([utils.smiles_eq(smiles, expected) for smiles in denovo])
 
+
 @pytest.mark.parametrize("frag1,frag2,expected", fragment_params1)
 def test_linking_scan(frag1, frag2, expected):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=False,
         shuffle=True,
         scan=True,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
+    frags = [utils.strip_attachment_points(frag)[0] for frag in [frag1, frag2]]
     assert len(denovo) == 10
-    assert all([smiles in [frag1, frag2] for smiles in denovo])
+    for smiles in denovo:
+        assert (
+            (utils.smiles_eq(smiles, frags[0]))[0]
+            or (utils.smiles_eq(smiles, frags[1]))[0]
+        )
+
 
 @pytest.mark.parametrize("frag1,frag2,expected", fragment_params1)
 def test_linking_batch_scan(frag1, frag2, expected):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=True,
         shuffle=True,
         scan=True,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
+    frags = [utils.strip_attachment_points(frag)[0] for frag in [frag1, frag2]]
     assert len(denovo) == 10
-    assert all([smiles in [frag1, frag2] for smiles in denovo])
+    for smiles in denovo:
+        assert (
+            (utils.smiles_eq(smiles, frags[0]))[0]
+            or (utils.smiles_eq(smiles, frags[1]))[0]
+        )
+
 
-fragment_params2 = [ # frag1, frag2, frag3
+fragment_params2 = [  # frag1, frag2, frag3
     ("C1CC1(*)", "c1cc(*)cc(Cl)c1", "N1(*)CCC1")
 ]
+
+
 @pytest.mark.parametrize("frag1,frag2,frag3", fragment_params2)
-def test_linking_scan(frag1, frag2, frag3):
+def test_linking_scan_multi(frag1, frag2, frag3):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2, frag3],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=False,
         shuffle=True,
         scan=True,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     frags = [utils.strip_attachment_points(frag)[0] for frag in [frag1, frag2, frag3]]
     assert len(denovo) == 10
     for smiles in denovo:
-        assert (utils.smiles_eq(smiles, frags[0]))[0] or (utils.smiles_eq(smiles, frags[1]))[0] or (utils.smiles_eq(smiles, frags[2]))[0]
+        assert (
+            (utils.smiles_eq(smiles, frags[0]))[0]
+            or (utils.smiles_eq(smiles, frags[1]))[0]
+            or (utils.smiles_eq(smiles, frags[2]))[0]
+        )
+
 
 @pytest.mark.parametrize("frag1,frag2,frag3", fragment_params2)
-def test_linking_batch_scan(frag1, frag2, frag3):
+def test_linking_batch_scan_multi(frag1, frag2, frag3):
     SD = samplers.FragmentLinker(
         fragments=[frag1, frag2, frag3],
         batch_size=10,
         sample_fn=sample_linker_fn,
         evaluate_fn=evaluate_fn,
         batch_prompts=True,
         shuffle=True,
         scan=True,
         detect_existing=False,
-        return_all=False
-        )
+        return_all=False,
+    )
     denovo = SD.sample()
     frags = [utils.strip_attachment_points(frag)[0] for frag in [frag1, frag2, frag3]]
     assert len(denovo) == 10
     for smiles in denovo:
-        assert (utils.smiles_eq(smiles, frags[0]))[0] or (utils.smiles_eq(smiles, frags[1]))[0] or (utils.smiles_eq(smiles, frags[2]))[0]
+        assert (
+            (utils.smiles_eq(smiles, frags[0]))[0]
+            or (utils.smiles_eq(smiles, frags[1]))[0]
+            or (utils.smiles_eq(smiles, frags[2]))[0]
+        )
```

### Comparing `promptsmiles-1.4.1/tests/test_utils.py` & `promptsmiles-1.4.2/tests/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright Universitat Pompeu Fabra 2020-2023  https://www.compscience.org
 # Distributed under the Apache 2.0 License.
 # (See accompanying file README.md file or copy at https://opensource.org/license/apache-2-0/)
 
+import gzip
 import os
 import sys
-import gzip
+
 import pytest
+
 from promptsmiles import utils
 
 # --------------------- Load test files ---------------------
 # PyTest was doing my head in so I've done it this way
 TEST_SMILES = []
 TEST_SCAFFOLD = []
 # Load supplied files
@@ -18,15 +20,15 @@
         with open(arg) as f:
             TEST_SMILES.extend([smi.strip() for smi in f.readlines()])
     if arg.endswith(".smi.gz"):
         with gzip.open(arg) as gf:
             TEST_SMILES.extend([smi.decode().strip() for smi in gf.readlines()])
     if arg.endswith(".scaff"):
         with open(arg) as f:
-            TEST_SCAFFOLDS.extend([smi.strip() for smi in f.readlines()])
+            TEST_SCAFFOLD.extend([smi.strip() for smi in f.readlines()])
 # Load defaults
 if not TEST_SMILES:
     with open(os.path.join(os.path.dirname(__file__), "test_smiles.smi")) as f:
         TEST_SMILES.extend([smi.strip() for smi in f.readlines()])
 if not TEST_SCAFFOLD:
     with open(os.path.join(os.path.dirname(__file__), "test_scaffolds.scaff")) as f:
         TEST_SCAFFOLD.extend([smi.strip() for smi in f.readlines()])
@@ -36,106 +38,222 @@
 @pytest.mark.parametrize("smiles", TEST_SMILES)
 def test_reverse(smiles):
     """Make an assumption that if we reverse a SMILES string twice, we get the same thing back."""
     rsmiles = utils.reverse_smiles(smiles, renumber_rings=False)
     eq, err = utils.smiles_eq(smiles, rsmiles)
     assert eq, "Reverse SMILES are not chemically equivalent"
     nsmiles = utils.reverse_smiles(rsmiles, renumber_rings=False)
-    assert utils.smiles_eq(smiles, nsmiles)[0], "Double reverse SMILES are not chemically equivalent"
+    assert utils.smiles_eq(smiles, nsmiles)[
+        0
+    ], "Double reverse SMILES are not chemically equivalent"
     assert nsmiles == smiles, "Double reverse SMILES are not exactly the same"
 
+
 @pytest.mark.parametrize("smiles", TEST_SMILES)
 def test_ring_numbers(smiles):
     """Check to see that we can safely reindex ring numbers by chronological opening order... this fixes an RDKit Error."""
     csmiles = utils._check_ring_numbers(smiles)
     eq, err = utils.smiles_eq(smiles, csmiles)
     assert eq, "SMILES with corrected ring numbers is not equivalent"
 
 
 # --------------------- Scaffold tests ----------------------
 @pytest.mark.parametrize("scaffold", TEST_SCAFFOLD)
 def test_attachment_points(scaffold):
     """If we get extract attachment points, and put them back in, we should get the same thing back."""
-    stripped, at_pts = utils.strip_attachment_points(scaffold) # This calls get_attachment_points
+    stripped, at_pts = utils.strip_attachment_points(
+        scaffold
+    )  # This calls get_attachment_points
     recycled_smiles = utils.insert_attachment_points(stripped, at_pts)
     eq, error = utils.smiles_eq(scaffold, recycled_smiles)
-    assert eq, error # Check if they are the same molecule
-    assert scaffold == recycled_smiles # Check if the are the exact same arrangement
+    assert eq, error  # Check if they are the same molecule
+    assert scaffold == recycled_smiles  # Check if the are the exact same arrangement
+
 
 @pytest.mark.parametrize("scaffold", TEST_SCAFFOLD)
 def test_root(scaffold):
     """If we pick every attachment point, randomize it and reverse it, we should get the same molecule back and an attachment point should be on the end."""
     at_pts = utils.get_attachment_points(scaffold)
     for at_pt in at_pts:
         c_pt = utils.correct_attachment_point(scaffold, at_pt)
         rev_rand_smi = utils.root_smiles(scaffold, rootAtom=c_pt, reverse=True)
-        eq, error = utils.smiles_eq(utils.strip_attachment_points(scaffold)[0], utils.strip_attachment_points(rev_rand_smi)[0])
+        eq, error = utils.smiles_eq(
+            utils.strip_attachment_points(scaffold)[0],
+            utils.strip_attachment_points(rev_rand_smi)[0],
+        )
         assert eq, error
-        assert rev_rand_smi.endswith("(*)"), f"Attachment point not at the end of the molecule: {rev_rand_smi}"
+        assert rev_rand_smi.endswith(
+            "(*)"
+        ), f"Attachment point not at the end of the molecule: {rev_rand_smi}"
+
 
 @pytest.mark.parametrize("scaffold", TEST_SCAFFOLD)
 def test_randomize(scaffold):
     """If we pick every attachment point, randomize it and reverse it, we should get the same molecule back and an attachment point should be on the end."""
     at_pts = utils.get_attachment_points(scaffold)
     for at_pt in at_pts:
         c_pt = utils.correct_attachment_point(scaffold, at_pt)
         rev_rand_smiles = utils.randomize_smiles(scaffold, rootAtom=c_pt, reverse=True)
         for rev_rand_smi in rev_rand_smiles:
-            eq, error = utils.smiles_eq(utils.strip_attachment_points(scaffold)[0], utils.strip_attachment_points(rev_rand_smi)[0])
+            eq, error = utils.smiles_eq(
+                utils.strip_attachment_points(scaffold)[0],
+                utils.strip_attachment_points(rev_rand_smi)[0],
+            )
             assert eq, error
-            assert rev_rand_smi.endswith("(*)"), f"Attachment point not at the end of the molecule: {rev_rand_smi}"
+            assert rev_rand_smi.endswith(
+                "(*)"
+            ), f"Attachment point not at the end of the molecule: {rev_rand_smi}"
 
 
 # --------------------- Specific tests ---------------------
 # smi, attachment_point, RDKit_atom_index
 scaffold_parameters = [
     ("c1(*)cc(*)ccc1", 0, 1),
     ("c1(*)cc(*)ccc1", 2, 4),
-    ("C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12", 0, 1),
-    ("C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12", 3, 5),
-    ("C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12", 8, 11),
-    ("C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12", 9, 13),
-    ("C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12", 17, 22),
-    ("C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12", 18, 24),
-    ("C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12", 19, 26),
-    ("C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12", 20, 28),
-    ("C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12", 21, 30),
-    ("C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12", 22, 32),
-    ('C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)', 0, 1),
-    ('C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)', 3, 5),
-    ('C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)', 5, 8),
-    ('C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)', 6, 10),
-    ('C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)', 9, 14),
-    ('C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)', 10, 16),
-    ('C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)', 11, 18),
-    ('C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)', 16, 24),
-    ('C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)', 18, 27),
-    ('C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)', 19, 29),
-    ('C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)', 21, 32),
-    ('C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)', 23, 35),
-    ('C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O', 0, 1),
-    ('C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O', 1, 3),
-    ('C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O', 3, 6),
-    ('C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O', 6, 10),
-    ('C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O', 7, 12),
-    ('C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O', 9, 15),
-    ('C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O', 10, 17),
-    ('C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O', 12, 20),
-    ('C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O', 13, 22),
-    ('C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O', 14, 24),
-    ('C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O', 15, 26),
-    ('c1(*)c(*)c(-c2c(OC(*))c(*)nc(*)c2(*))c(*)c(NC(C(c2c(*)c(*)n(C(*))n2)(*))=O)c1(*)', 15, 32),
-    ('c1(*)c(-c2c(OC(*))c(*)nc(*)c2(*))c(*)c(NC(=O)C(c2c(*)c(*)n(C(*))n2)(*))c(*)c1(*))', 15, 31)
-    ]
+    (
+        "C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12",
+        0,
+        1,
+    ),
+    (
+        "C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12",
+        3,
+        5,
+    ),
+    (
+        "C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12",
+        8,
+        11,
+    ),
+    (
+        "C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12",
+        9,
+        13,
+    ),
+    (
+        "C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12",
+        17,
+        22,
+    ),
+    (
+        "C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12",
+        18,
+        24,
+    ),
+    (
+        "C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12",
+        19,
+        26,
+    ),
+    (
+        "C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12",
+        20,
+        28,
+    ),
+    (
+        "C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12",
+        21,
+        30,
+    ),
+    (
+        "C(*)c1nc(*)n2[nH]c(-c3c(*)c(*)c(F)c(S(=O)(=O)N4C(*)C(*)N(*)C(*)C4(*))c3(*))nc(=O)c12",
+        22,
+        32,
+    ),
+    (
+        "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
+        0,
+        1,
+    ),
+    (
+        "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
+        3,
+        5,
+    ),
+    (
+        "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
+        5,
+        8,
+    ),
+    (
+        "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
+        6,
+        10,
+    ),
+    (
+        "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
+        9,
+        14,
+    ),
+    (
+        "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
+        10,
+        16,
+    ),
+    (
+        "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
+        11,
+        18,
+    ),
+    (
+        "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
+        16,
+        24,
+    ),
+    (
+        "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
+        18,
+        27,
+    ),
+    (
+        "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
+        19,
+        29,
+    ),
+    (
+        "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
+        21,
+        32,
+    ),
+    (
+        "C(*)Oc1c(*)nc(*)c(*)c1-c1c(*)c(*)c(*)c(NC(=O)C(*)c2c(*)c(*)n(C(*))n2)c1(*)",
+        23,
+        35,
+    ),
+    ("C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O", 0, 1),
+    ("C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O", 1, 3),
+    ("C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O", 3, 6),
+    ("C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O", 6, 10),
+    ("C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O", 7, 12),
+    ("C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O", 9, 15),
+    ("C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O", 10, 17),
+    ("C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O", 12, 20),
+    ("C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O", 13, 22),
+    ("C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O", 14, 24),
+    ("C(*)C(*)N(C(*)=O)c1c(*)c(*)c(c(*)c1(*))N1C(*)C(*)C(*)C(*)C1=O", 15, 26),
+    (
+        "c1(*)c(*)c(-c2c(OC(*))c(*)nc(*)c2(*))c(*)c(NC(C(c2c(*)c(*)n(C(*))n2)(*))=O)c1(*)",
+        15,
+        32,
+    ),
+    (
+        "c1(*)c(-c2c(OC(*))c(*)nc(*)c2(*))c(*)c(NC(=O)C(c2c(*)c(*)n(C(*))n2)(*))c(*)c1(*))",
+        15,
+        31,
+    ),
+]
+
 
 @pytest.mark.parametrize("smiles,at_pt,rd_pt", scaffold_parameters)
 def test_correct_attachment(smiles, at_pt, rd_pt):
     """Check if we can correct attachment points to the actual wildcard"""
     assert utils.correct_attachment_point(smiles, at_pt) == rd_pt
 
+
 @pytest.mark.parametrize("smiles,at_pt,rd_pt", scaffold_parameters)
 def test_get_attachment(smiles, at_pt, rd_pt):
     """Check if we can correct attachment points to the actual wildcard"""
     at_pts = utils.get_attachment_points(smiles)
     assert at_pt in at_pts
 
+
 # TODO test fragments utils
```

