# Comparing `tmp/hierarchy_transformers-0.0.1.tar.gz` & `tmp/hierarchy_transformers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hierarchy_transformers-0.0.1.tar", last modified: Sun Jan 21 13:32:56 2024, max compression
+gzip compressed data, was "hierarchy_transformers-0.0.3.tar", last modified: Thu May  9 09:58:35 2024, max compression
```

## Comparing `hierarchy_transformers-0.0.1.tar` & `hierarchy_transformers-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:32:56.657176 hierarchy_transformers-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-01-21 13:32:56.657176 hierarchy_transformers-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-01-21 13:32:56.657176 hierarchy_transformers-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:32:56.653176 hierarchy_transformers-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:32:56.653176 hierarchy_transformers-0.0.1/src/hierarchy_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:32:56.657176 hierarchy_transformers-0.0.1/src/hierarchy_transformers/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/evaluation/hierarchy_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/evaluation/hit_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/evaluation/pretrained_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/evaluation/static_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:32:56.657176 hierarchy_transformers-0.0.1/src/hierarchy_transformers/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/losses/centri_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/losses/cluster_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/losses/cone_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/losses/hyper_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:32:56.657176 hierarchy_transformers-0.0.1/src/hierarchy_transformers/models/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/models/hit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/models/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:32:56.657176 hierarchy_transformers-0.0.1/src/hierarchy_transformers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/utils/construct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-01-21 13:32:48.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers/utils/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:32:56.657176 hierarchy_transformers-0.0.1/src/hierarchy_transformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-01-21 13:32:56.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-01-21 13:32:56.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 13:32:56.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-21 13:32:56.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-21 13:32:56.000000 hierarchy_transformers-0.0.1/src/hierarchy_transformers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:58:35.485235 hierarchy_transformers-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-09 09:58:35.485235 hierarchy_transformers-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-09 09:58:35.485235 hierarchy_transformers-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:58:35.481235 hierarchy_transformers-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:58:35.481235 hierarchy_transformers-0.0.3/src/hierarchy_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:58:35.481235 hierarchy_transformers-0.0.3/src/hierarchy_transformers/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/evaluation/hierarchy_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/evaluation/hit_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/evaluation/pretrained_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/evaluation/static_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:58:35.485235 hierarchy_transformers-0.0.3/src/hierarchy_transformers/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/losses/centri_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/losses/cluster_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/losses/cone_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/losses/hyper_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:58:35.485235 hierarchy_transformers-0.0.3/src/hierarchy_transformers/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/models/hit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/models/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:58:35.485235 hierarchy_transformers-0.0.3/src/hierarchy_transformers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/utils/construct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-09 09:58:29.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers/utils/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:58:35.485235 hierarchy_transformers-0.0.3/src/hierarchy_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-09 09:58:35.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-09 09:58:35.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:58:35.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 09:58:35.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 09:58:35.000000 hierarchy_transformers-0.0.3/src/hierarchy_transformers.egg-info/top_level.txt
```

### Comparing `hierarchy_transformers-0.0.1/LICENSE` & `hierarchy_transformers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hierarchy_transformers-0.0.1/setup.cfg` & `hierarchy_transformers-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hierarchy_transformers
-version = 0.0.1
+version = 0.0.3
 author = Yuan He (KRR-Oxford)
 author_email = yuan.he@cs.ox.ac.uk
 license = Apache License 2.0
 license_files = LICENSE
 description = Language models as hierarchy encoders.
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `hierarchy_transformers-0.0.1/src/hierarchy_transformers/evaluation/hit_eval.py` & `hierarchy_transformers-0.0.3/src/hierarchy_transformers/evaluation/hit_eval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 Yuan He
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from geoopt.manifolds import PoincareBall
 import torch
 from deeponto.utils import save_file
 from pathlib import Path
 from typing import Optional
 import logging
 
@@ -12,15 +26,15 @@
 
 
 class HierarchyTransformerEvaluator(HierarchyEvaluator):
     """Evaluator hierarchy re-trained language models (HiT).
 
     Hierarchy encoding is evaluated based on the hyperbolic distances between entity
     embeddings and hyperbolic norms of entity embeddings in the Poincare ball of
-    radius 1/sqrt(N) where N is the embedding dimension.
+    radius 1/sqrt(d) where d is the embedding dimension.
     """
 
     def __init__(
         self,
         device: torch.device,
         eval_batch_size: int,
         val_examples: list,
@@ -43,14 +57,20 @@
         dists = model.manifold.dist(child_embeds, parent_embeds)
         child_norms = model.manifold.dist0(child_embeds)
         parent_norms = model.manifold.dist0(parent_embeds)
         return torch.stack([labels, dists, child_norms, parent_norms]).T
 
     @classmethod
     def score(cls, result_mat: torch.Tensor, centri_score_weight: float):
+        """The empirical scoring function for using HiT embeddings to predict subsumptions.
+
+        The scores are "lower-the-better".
+
+        NOTE: In the paper, the `-` operator is appended to this function to make it "higher-the-better".
+        """
         scores = result_mat[:, 1] + centri_score_weight * (result_mat[:, 3] - result_mat[:, 2])
         labels = result_mat[:, 0]
         return scores, labels
 
     @classmethod
     def search_best_threshold(cls, result_mat: torch.Tensor, threshold_granularity: int = 100):
         best_f1 = -1.0
@@ -89,15 +109,18 @@
     ):
         result_mat = self.encode(model, examples, self.eval_batch_size)
         if not best_val_threshold or not best_val_centri_score_weight:
             eval_results = self.search_best_threshold(result_mat, 100)
         else:
             eval_scores, eval_labels = self.score(result_mat, best_val_centri_score_weight)
             eval_results = self.evaluate_by_threshold(eval_scores, eval_labels, best_val_threshold)
-            eval_results = {"centri_score_weight": best_val_centri_score_weight, **eval_results}
+            eval_results = {
+                "centri_score_weight": best_val_centri_score_weight,
+                **eval_results,
+            }
 
         return result_mat, eval_results
 
     def __call__(self, model, output_path: str = None, epoch: int = -1, steps: int = -1) -> float:
         """This is called during training to evaluate the model.
         It returns a score for the evaluation with a higher score indicating a better result.
         """
@@ -105,27 +128,42 @@
         # set to eval mode
         Path(f"{output_path}/epoch={epoch}.step={steps}").mkdir(parents=True, exist_ok=True)
         # model.save(f"{output_path}/epoch={epoch}.step={steps}")
 
         if self.train_examples:
             logger.info("Evaluate on train examples...")
             train_result_mat, train_results = self.inference(model, self.train_examples)
-            torch.save(train_result_mat, f"{output_path}/epoch={epoch}.step={steps}/train_result_mat.pt")
-            save_file(train_results, f"{output_path}/epoch={epoch}.step={steps}/train_results.json")
+            torch.save(
+                train_result_mat,
+                f"{output_path}/epoch={epoch}.step={steps}/train_result_mat.pt",
+            )
+            save_file(
+                train_results,
+                f"{output_path}/epoch={epoch}.step={steps}/train_results.json",
+            )
 
         logger.info("Evaluate on val examples...")
         val_result_mat, val_results = self.inference(model, self.val_examples)
-        torch.save(val_result_mat, f"{output_path}/epoch={epoch}.step={steps}/val_result_mat.pt")
+        torch.save(
+            val_result_mat,
+            f"{output_path}/epoch={epoch}.step={steps}/val_result_mat.pt",
+        )
         save_file(val_results, f"{output_path}/epoch={epoch}.step={steps}/val_results.json")
 
         if self.test_examples:
             logger.info("Evaluate on test examples using best val threshold...")
             test_result_mat, test_results = self.inference(
                 model,
                 self.test_examples,
                 val_results["centri_score_weight"],
                 val_results["threshold"],
             )
-            torch.save(test_result_mat, f"{output_path}/epoch={epoch}.step={steps}/test_result_mat.pt")
-            save_file(test_results, f"{output_path}/epoch={epoch}.step={steps}/test_results.json")
+            torch.save(
+                test_result_mat,
+                f"{output_path}/epoch={epoch}.step={steps}/test_result_mat.pt",
+            )
+            save_file(
+                test_results,
+                f"{output_path}/epoch={epoch}.step={steps}/test_results.json",
+            )
 
         return val_results["F1"]
```

### Comparing `hierarchy_transformers-0.0.1/src/hierarchy_transformers/evaluation/pretrained_eval.py` & `hierarchy_transformers-0.0.3/src/hierarchy_transformers/evaluation/pretrained_eval.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 Yuan He
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from typing import Optional
 import torch
 from deeponto.utils import save_file
 from tqdm.auto import tqdm
 from transformers import pipeline
 from .hierarchy_eval import HierarchyEvaluator
 from ..models import HierarchyTransformer
@@ -33,15 +47,16 @@
 
     def inference(self, examples: list):
         labels = [example.label for example in examples]
         labels = torch.tensor(labels)
 
         scores = []
         for result in tqdm(
-            self.pipeline(self.pipeline_data(examples), batch_size=self.eval_batch_size, top_k=10), total=len(examples)
+            self.pipeline(self.pipeline_data(examples), batch_size=self.eval_batch_size, top_k=10),
+            total=len(examples),
         ):
             pos_score = 0.0
             neg_score = 0.0
             for pred in result:
                 if pred["token_str"].strip().lower() == "yes":
                     pos_score += pred["score"]
                 elif pred["token_str"].strip().lower() == "no":
```

### Comparing `hierarchy_transformers-0.0.1/src/hierarchy_transformers/evaluation/static_eval.py` & `hierarchy_transformers-0.0.3/src/hierarchy_transformers/evaluation/static_eval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,28 @@
+# Copyright 2023 Yuan He
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from typing import Optional
 import torch
 from torch.utils.data import DataLoader
 from deeponto.utils import save_file
 
 from .hierarchy_eval import HierarchyEvaluator
+from ..losses import EntailmentConeConstrastiveLoss
 
 
 class StaticPoincareEvaluator(HierarchyEvaluator):
     """Evaluator for the static Poincare embedding model.
 
     Hierarchy encoding is evaluated based on hyperbolic distances between
     entity embeddings in the unit Poincare ball.
@@ -17,59 +32,73 @@
         self,
         model_path: str,
         device: torch.device,
         val_examples: list,
         eval_batch_size: int,
         test_examples: Optional[list] = None,
         train_examples: Optional[list] = None,
+        apply_entailment_cone: bool = False,
     ):
         super().__init__()
 
         self.model = torch.load(model_path)
         self.device = device
         self.model.to(self.device)
 
         self.eval_batch_size = eval_batch_size
         self.val_examples = val_examples
         self.test_examples = test_examples
         self.train_examples = train_examples
 
-    def score(self, subject: torch.Tensor, objects: torch.Tensor, norm_score_weight: float = 1000.0):
+        self.score = self.dist_score
+        self.apply_entailment_cone = apply_entailment_cone
+        if self.apply_entailment_cone:
+            self.eloss = EntailmentConeConstrastiveLoss(self.model.manifold)
+            self.score = self.cone_score
+
+    def dist_score(self, subject: torch.Tensor, objects: torch.Tensor, norm_score_weight: float = 1000.0):
         dists = self.model.manifold.dist(subject, objects)
         subject_norms = subject.norm(dim=-1)
         objects_norms = objects.norm(dim=-1)
         return (1 + norm_score_weight * (objects_norms - subject_norms)) * dists
 
+    def cone_score(self, subject: torch.Tensor, objects: torch.Tensor):
+        return self.eloss.energy(objects, subject)
+
     def inference(self, examples: list):
         """WARNING: this function is highly customised to our hierarchy datasets
         where 1 positive sample corresponds to 10 negatives."""
         self.model.eval()
         num_negatives = len(examples[0]) - 2  # each example is formatted as [child, parent, *negatives]
         eval_scores = []
-        dataloader = DataLoader(torch.tensor(examples).to(self.device), shuffle=False, batch_size=self.eval_batch_size)
+        dataloader = DataLoader(
+            torch.tensor(examples).to(self.device),
+            shuffle=False,
+            batch_size=self.eval_batch_size,
+        )
         with torch.no_grad():
             for batch in dataloader:
                 subject, objects = self.model(batch)
                 cur_scores = self.score(subject, objects)
                 eval_scores.append(cur_scores.reshape((-1,)))
             eval_scores = torch.concat(eval_scores, dim=0)
             eval_labels = torch.tensor(([1] + [0] * num_negatives) * (int(len(eval_scores) / (1 + num_negatives)))).to(
                 self.device
             )
         assert len(eval_labels) == len(eval_scores)
         return eval_scores, eval_labels
 
-    def __call__(self, output_path: str):
+    def __call__(self, output_path: str, threshold_granularity: int = 1):
+
         if self.train_examples:
             train_scores, train_labels = self.inference(self.train_examples)
-            best_train_results = self.search_best_threshold(train_scores, train_labels, threshold_granularity=1)
+            best_train_results = self.search_best_threshold(train_scores, train_labels, threshold_granularity=threshold_granularity)
             save_file(best_train_results, f"{output_path}/train_results.json")
-        
+
         val_scores, val_labels = self.inference(self.val_examples)
-        best_val_results = self.search_best_threshold(val_scores, val_labels, threshold_granularity=1)
+        best_val_results = self.search_best_threshold(val_scores, val_labels, threshold_granularity=threshold_granularity)
         save_file(best_val_results, f"{output_path}/val_results.json")
 
         if self.test_examples:
             test_scores, test_labels = self.inference(self.test_examples)
             test_results = self.evaluate_by_threshold(test_scores, test_labels, best_val_results["threshold"])
             save_file(test_results, f"{output_path}/test_results.json")
-
```

### Comparing `hierarchy_transformers-0.0.1/src/hierarchy_transformers/losses/centri_loss.py` & `hierarchy_transformers-0.0.3/src/hierarchy_transformers/losses/centri_loss.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,29 @@
+# Copyright 2023 Yuan He
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import torch
 import torch.nn.functional as F
 from geoopt.manifolds import PoincareBall
 
 
 class CentripetalTripletLoss(torch.nn.Module):
     r"""Hyperbolic loss that regulates the norms of child and parent entities.
-    
+
     Essentially, this loss is expected to achieve:
     $$
         d(child, origin) > d(parent, origin)
     $$
 
     Inputs are presented in `(rep_anchor, rep_positive, rep_negative)` but only `(rep_anchor, rep_positive)` pairs are involved in this loss.
     """
@@ -17,28 +31,31 @@
     def __init__(self, manifold: PoincareBall, embed_dim: int, margin: float):
         super().__init__()
         self.manifold = manifold
         self.margin = margin
         # self.manifold_origin = self.manifold.origin(embed_dim)
 
     def get_config_dict(self):
-        config = {"distance_metric": f"PoincareBall(c={self.manifold.c}).dist(_, origin)", "margin": self.margin}
+        config = {
+            "distance_metric": f"PoincareBall(c={self.manifold.c}).dist(_, origin)",
+            "margin": self.margin,
+        }
         return config
 
     def forward(self, rep_anchor: torch.Tensor, rep_positive: torch.Tensor, rep_negative: torch.Tensor):
         rep_anchor_hyper_norms = self.manifold.dist0(rep_anchor)
         rep_positive_hyper_norms = self.manifold.dist0(rep_positive)
         # child further than parent w.r.t. origin
         centri_triplet_loss = F.relu(self.margin + rep_positive_hyper_norms - rep_anchor_hyper_norms)
         return centri_triplet_loss.mean()
 
 
 class CentripetalContrastiveLoss(torch.nn.Module):
     r"""Hyperbolic loss that regulates the norms of child and parent entities.
-    
+
     Essentially, this loss is expected to achieve:
     $$
         d(child, origin) > d(parent, origin)
     $$
 
     Inputs are presented in `(rep_anchor, rep_other, label)` but only `label==1` ones are involved in this loss.
     """
@@ -46,15 +63,18 @@
     def __init__(self, manifold: PoincareBall, embed_dim: int, margin: float):
         super().__init__()
         self.manifold = manifold
         self.margin = margin
         # self.manifold_origin = self.manifold.origin(embed_dim)
 
     def get_config_dict(self):
-        config = {"distance_metric": f"PoincareBall(c={self.manifold.c}).dist(_, origin)", "margin": self.margin}
+        config = {
+            "distance_metric": f"PoincareBall(c={self.manifold.c}).dist(_, origin)",
+            "margin": self.margin,
+        }
         return config
 
     def forward(self, rep_anchor: torch.Tensor, rep_other: torch.Tensor, labels: torch.Tensor):
         rep_anchor_hyper_norms = self.manifold.dist0(rep_anchor)
         rep_other_hyper_norms = self.manifold.dist0(rep_other)
         # child further than parent w.r.t. origin
         centri_loss = labels.float() * F.relu(self.margin + rep_other_hyper_norms - rep_anchor_hyper_norms)
```

### Comparing `hierarchy_transformers-0.0.1/src/hierarchy_transformers/losses/cluster_loss.py` & `hierarchy_transformers-0.0.3/src/hierarchy_transformers/losses/cluster_loss.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,29 @@
+# Copyright 2023 Yuan He
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import torch
 import torch.nn.functional as F
 from geoopt.manifolds import PoincareBall
 
 
 class ClusteringTripletLoss(torch.nn.Module):
     """Hyperbolic loss that clusters entities in subsumptions.
-    
+
     Essentially, this loss is expected to achieve:
     $$
         d(child, parent) < d(child, non-parent)
     $$
 
     Inputs are presented in `(rep_anchor, rep_positive, rep_negative)`.
     """
@@ -31,15 +45,15 @@
         distances_negative = self.manifold.dist(rep_anchor, rep_negative)
         cluster_triplet_loss = F.relu(distances_positive - distances_negative + self.margin)
         return cluster_triplet_loss.mean()
 
 
 class ClusteringConstrastiveLoss(torch.nn.Module):
     """Hyperbolic loss that clusters entities in subsumptions.
-    
+
     Essentially, this loss is expected to achieve:
     $$
         d(child, parent) < d(child, non-parent)
     $$
 
     Inputs are presented in `(rep_anchor, rep_other, label)`.
     """
```

### Comparing `hierarchy_transformers-0.0.1/src/hierarchy_transformers/losses/cone_loss.py` & `hierarchy_transformers-0.0.3/src/hierarchy_transformers/losses/cone_loss.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,78 @@
+# Copyright 2023 Yuan He
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import torch
 import torch.nn.functional as F
 from geoopt.manifolds import PoincareBall
 
 
 class EntailmentConeTripletLoss(torch.nn.Module):
     """Hyperbolic loss that construct entailment cones for entities.
-    
+
     Essentially, this loss is expected to achieve:
     $$
         angle(child, parent_cone_axis) < angle(parent_cone)
     $$
 
     Inputs are presented in `(rep_anchor, rep_positive, rep_negative)`.
     """
 
-    def __init__(self, manifold: PoincareBall, min_euclidean_norm: float, margin: float):
+    def __init__(self, manifold: PoincareBall, min_euclidean_norm: float = 0.1, margin: float = 0.1, eps: float = 1e-5):
         super().__init__()
         self.manifold = manifold
         assert self.manifold.c == 1.0, f"Entailment cone loss is not defined for curvature: {manifold.c}."
         self.min_euclidean_norm = min_euclidean_norm
         self.margin = margin
+        self.eps = eps
 
     def get_config_dict(self):
         config = {"distance_metric": "PoincareBall(c=1.0).cone_angle", "margin": self.margin}
         return config
 
     def half_cone_aperture(self, cone_tip: torch.Tensor):
         """Angle between the axis [0, x] (line through 0 and x) and the boundary of the cone at x,
         where x is the cone tip.
         """
         # cone tip means the point x is the tip of the hyperbolic cone
-        norm_tip = cone_tip.norm(dim=-1).clamp(min=self.min_euclidean_norm)  # to prevent undefined aperture
-        return torch.arcsin(self.min_euclidean_norm * (1 - (norm_tip**2)) / norm_tip)
+        # norm_tip = cone_tip.norm(dim=-1).clamp(min=self.min_euclidean_norm)  # to prevent undefined aperture
+        sq_norm_tip = cone_tip.pow(2).sum(dim=-1).clamp(min=self.min_euclidean_norm+self.eps, max=1-self.eps)
+        return torch.arcsin(self.min_euclidean_norm * (1 - sq_norm_tip) / torch.sqrt(sq_norm_tip)).clamp(min=-1 + self.eps, max=1 - self.eps)
 
     def cone_angle_at_u(self, cone_tip: torch.Tensor, u: torch.Tensor):
         """Angle between the axis [0, x] and the line [x, u]. This angle should be smaller than the
         half cone aperture at x for real children.
         """
         # parent point is treated as the cone tip
-        norm_tip = cone_tip.norm(dim=-1)
-        norm_child = u.norm(dim=-1)
+        norm_tip = cone_tip.norm(2, dim=-1)
+        norm_child = u.norm(2, dim=-1)
         dot_prod = (cone_tip * u).sum(dim=-1)
-        edist = (cone_tip - u).norm(dim=-1)  # euclidean distance
+        edist = (cone_tip - u).norm(2, dim=-1)  # euclidean distance
         numerator = dot_prod * (1 + norm_tip**2) - norm_tip**2 * (1 + norm_child**2)
-        denomenator = norm_tip * edist * torch.sqrt(1 + (norm_child**2) * (norm_tip**2) - 2 * dot_prod)
-        return torch.arccos(numerator / denomenator)
+        denominator = norm_tip * edist * torch.sqrt(1 + (norm_child**2) * (norm_tip**2) - 2 * dot_prod)
+            
+        angle = torch.arccos((numerator / denominator.clamp(min=self.eps)).clamp(min=-1 + self.eps, max=1 - self.eps))
+        # Debugging step
+        if torch.isnan(angle).any():
+            print("Numerator:", numerator)
+            print("Denominator:", denominator)
+            print("Angle calculation resulted in NaNs")
+        
+        return angle
 
     def energy(self, cone_tip: torch.Tensor, u: torch.Tensor):
         """Enery function defined as: max(0, cone_angle(u) - half_cone_aperture) given a cone tip."""
         return F.relu(self.cone_angle_at_u(cone_tip, u) - self.half_cone_aperture(cone_tip))
 
     def forward(self, rep_anchor: torch.Tensor, rep_positive: torch.Tensor, rep_negative: torch.Tensor):
         # anchors are children
@@ -56,54 +80,64 @@
         energies_negative = self.energy(cone_tip=rep_negative, u=rep_anchor)
         cone_triplet_loss = F.relu(energies_positive - energies_negative + self.margin)
         return cone_triplet_loss.mean()
 
 
 class EntailmentConeConstrastiveLoss(torch.nn.Module):
     """Hyperbolic loss that construct entailment cones for entities.
-    
+
     Essentially, this loss is expected to achieve:
     $$
         angle(child, parent_cone_axis) < angle(parent_cone)
     $$
 
     Inputs are presented in `(rep_anchor, rep_other, label)`.
     """
 
-    def __init__(self, manifold: PoincareBall, min_euclidean_norm: float, margin: float):
+    def __init__(self, manifold: PoincareBall, min_euclidean_norm: float = 0.1, margin: float = 0.1, eps: float = 1e-5):
         super().__init__()
         self.manifold = manifold
         assert self.manifold.c == 1.0, f"Entailment cone loss is not defined for curvature: {manifold.c}."
         self.min_euclidean_norm = min_euclidean_norm
         self.margin = margin
+        self.eps = eps
 
     def get_config_dict(self):
         config = {"distance_metric": "PoincareBall(c=1.0).cone_angle", "margin": self.margin}
         return config
 
     def half_cone_aperture(self, cone_tip: torch.Tensor):
         """Angle between the axis [0, x] (line through 0 and x) and the boundary of the cone at x,
         where x is the cone tip.
         """
         # cone tip means the point x is the tip of the hyperbolic cone
-        norm_tip = cone_tip.norm(dim=-1).clamp(min=self.min_euclidean_norm)  # to prevent undefined aperture
-        return torch.arcsin(self.min_euclidean_norm * (1 - (norm_tip**2)) / norm_tip)
+        # norm_tip = cone_tip.norm(dim=-1).clamp(min=self.min_euclidean_norm)  # to prevent undefined aperture
+        sq_norm_tip = cone_tip.pow(2).sum(dim=-1).clamp(min=self.min_euclidean_norm+self.eps, max=1-self.eps)
+        return torch.arcsin(self.min_euclidean_norm * (1 - sq_norm_tip) / torch.sqrt(sq_norm_tip)).clamp(min=-1 + self.eps, max=1 - self.eps)
 
     def cone_angle_at_u(self, cone_tip: torch.Tensor, u: torch.Tensor):
         """Angle between the axis [0, x] and the line [x, u]. This angle should be smaller than the
         half cone aperture at x for real children.
         """
         # parent point is treated as the cone tip
-        norm_tip = cone_tip.norm(dim=-1)
-        norm_child = u.norm(dim=-1)
+        norm_tip = cone_tip.norm(2, dim=-1)
+        norm_child = u.norm(2, dim=-1)
         dot_prod = (cone_tip * u).sum(dim=-1)
-        edist = (cone_tip - u).norm(dim=-1)  # euclidean distance
+        edist = (cone_tip - u).norm(2, dim=-1)  # euclidean distance
         numerator = dot_prod * (1 + norm_tip**2) - norm_tip**2 * (1 + norm_child**2)
-        denomenator = norm_tip * edist * torch.sqrt(1 + (norm_child**2) * (norm_tip**2) - 2 * dot_prod)
-        return torch.arccos(numerator / denomenator)
+        denominator = norm_tip * edist * torch.sqrt(1 + (norm_child**2) * (norm_tip**2) - 2 * dot_prod)
+            
+        angle = torch.arccos((numerator / denominator.clamp(min=self.eps)).clamp(min=-1 + self.eps, max=1 - self.eps))
+        # Debugging step
+        if torch.isnan(angle).any():
+            print("Numerator:", numerator)
+            print("Denominator:", denominator)
+            print("Angle calculation resulted in NaNs")
+        
+        return angle
 
     def energy(self, cone_tip: torch.Tensor, u: torch.Tensor):
         """Enery function defined as: max(0, cone_angle(u) - half_cone_aperture) given a cone tip."""
         return F.relu(self.cone_angle_at_u(cone_tip, u) - self.half_cone_aperture(cone_tip))
 
     def forward(self, rep_anchor: torch.Tensor, rep_other: torch.Tensor, labels: torch.Tensor):
         # anchors are children
```

### Comparing `hierarchy_transformers-0.0.1/src/hierarchy_transformers/losses/hyper_loss.py` & `hierarchy_transformers-0.0.3/src/hierarchy_transformers/losses/hyper_loss.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 Yuan He
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from typing import Iterable, Dict, Union, Tuple
 import torch
 import logging
 
 from .cluster_loss import *
 from .centri_loss import *
 from .cone_loss import *
```

### Comparing `hierarchy_transformers-0.0.1/src/hierarchy_transformers/models/hit.py` & `hierarchy_transformers-0.0.3/src/hierarchy_transformers/models/hit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,36 @@
+# Copyright 2023 Yuan He
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import torch
 from geoopt.manifolds import PoincareBall
 from sentence_transformers import SentenceTransformer
 from sentence_transformers.models import Pooling, Transformer
 import logging
 from typing import Union, Optional, Iterable
 
 logger = logging.getLogger(__name__)
 
 
 class HierarchyTransformer(SentenceTransformer):
+    r"""`HierarchyTransformer` is a subclass of `SentenceTransformer` that extends its functionality
+    to support hierarchy encoding using the Poincar\'eBall manifold.
+    """
+
     def __init__(
         self,
         model_name_or_path: Optional[str] = None,
         modules: Optional[Iterable[torch.nn.Module]] = None,
         device: Optional[str] = None,
         cache_folder: Optional[str] = None,
         use_auth_token: Union[bool, str, None] = None,
```

### Comparing `hierarchy_transformers-0.0.1/src/hierarchy_transformers/utils/construct.py` & `hierarchy_transformers-0.0.3/src/hierarchy_transformers/utils/construct.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 Yuan He
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from deeponto.onto import Taxonomy, TaxonomyNegativeSampler
 from deeponto.utils import save_file
 from sklearn.model_selection import train_test_split
 import json
 from pathlib import Path
 from tqdm.auto import tqdm
 
@@ -62,15 +76,15 @@
 
         trans_task_name = "multi"
         Path(f"{output_dir}/{trans_task_name}").mkdir(parents=True, exist_ok=True)
         self.save_dataset(base_examples, f"{output_dir}/{trans_task_name}/train.jsonl")
         # self.save_dataset(trans_train_examples, f"{output_dir}/transitivity/trans_train.jsonl")
         self.save_dataset(trans_val_examples, f"{output_dir}/{trans_task_name}/val.jsonl")
         self.save_dataset(trans_test_examples, f"{output_dir}/{trans_task_name}/test.jsonl")
-        
+
         base_train_examples, base_eval_examples = train_test_split(base_examples, test_size=eval_size)
         base_val_examples, base_test_examples = train_test_split(base_eval_examples, test_size=0.5)
         # base_train_edges = [(x["child"], x["parent"]) for x in base_train_examples]
         # trans_base_train_edges = self.get_transitive_edges(base_train_edges)
         # trans_base_train_examples = []
         # for child, parent in tqdm(trans_base_train_edges, desc="trans on base_train"):
         #     trans_base_train_examples.append(self.construct_example(child, parent, num_negative))
```

### Comparing `hierarchy_transformers-0.0.1/src/hierarchy_transformers/utils/data.py` & `hierarchy_transformers-0.0.3/src/hierarchy_transformers/utils/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 Yuan He
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import os
 from datasets import Dataset, load_dataset
 from sentence_transformers import InputExample
 from tqdm.auto import tqdm
 import json
 from typing import Optional
```

### Comparing `hierarchy_transformers-0.0.1/src/hierarchy_transformers.egg-info/SOURCES.txt` & `hierarchy_transformers-0.0.3/src/hierarchy_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

