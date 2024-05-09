# Comparing `tmp/prompt_learner-0.2.0.tar.gz` & `tmp/prompt_learner-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_learner-0.2.0.tar", max compression
+gzip compressed data, was "prompt_learner-0.2.1.tar", max compression
```

## Comparing `prompt_learner-0.2.0.tar` & `prompt_learner-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0     2140 2024-04-16 15:23:30.960382 prompt_learner-0.2.0/README.md
--rw-r--r--   0        0        0     6148 2024-04-12 21:48:53.225544 prompt_learner-0.2.0/prompt_learner/.DS_Store
--rw-r--r--   0        0        0       28 2024-04-11 03:24:46.950449 prompt_learner-0.2.0/prompt_learner/adapters/__init__.py
--rw-r--r--   0        0        0      394 2024-03-30 07:34:49.479472 prompt_learner-0.2.0/prompt_learner/adapters/adapter.py
--rw-r--r--   0        0        0     1291 2024-04-19 04:22:30.029307 prompt_learner-0.2.0/prompt_learner/adapters/anthropic.py
--rw-r--r--   0        0        0      720 2024-04-19 04:23:36.748602 prompt_learner-0.2.0/prompt_learner/adapters/llama.py
--rw-r--r--   0        0        0      662 2024-04-19 04:26:50.738576 prompt_learner-0.2.0/prompt_learner/adapters/openai.py
--rw-r--r--   0        0        0     1295 2024-04-12 22:29:26.768011 prompt_learner-0.2.0/prompt_learner/evals/metrics/accuracy.py
--rw-r--r--   0        0        0       29 2024-04-11 03:23:09.786151 prompt_learner-0.2.0/prompt_learner/examples/__init__.py
--rw-r--r--   0        0        0      316 2024-04-18 07:01:26.041471 prompt_learner-0.2.0/prompt_learner/examples/example.py
--rw-r--r--   0        0        0        0 2024-03-30 04:43:35.605009 prompt_learner-0.2.0/prompt_learner/examples/manipulation/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 06:22:23.812645 prompt_learner-0.2.0/prompt_learner/inference/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 06:22:57.915297 prompt_learner-0.2.0/prompt_learner/inference/predict.py
--rw-r--r--   0        0        0        0 2024-04-03 00:44:07.604053 prompt_learner-0.2.0/prompt_learner/optimizers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 03:24:34.521211 prompt_learner-0.2.0/prompt_learner/optimizers/descriptors/__init__.py
--rw-r--r--   0        0        0      165 2024-04-03 13:24:51.204583 prompt_learner-0.2.0/prompt_learner/optimizers/descriptors/descriptor.py
--rw-r--r--   0        0        0       34 2024-03-30 05:23:18.250890 prompt_learner-0.2.0/prompt_learner/optimizers/optimizer.py
--rw-r--r--   0        0        0       30 2024-04-11 03:24:14.614552 prompt_learner-0.2.0/prompt_learner/optimizers/selectors/__init__.py
--rw-r--r--   0        0        0     1537 2024-04-12 21:34:12.452345 prompt_learner-0.2.0/prompt_learner/optimizers/selectors/diverse_sampler.py
--rw-r--r--   0        0        0      624 2024-04-12 23:18:56.744204 prompt_learner-0.2.0/prompt_learner/optimizers/selectors/random_sampler.py
--rw-r--r--   0        0        0      873 2024-04-12 23:12:29.480864 prompt_learner-0.2.0/prompt_learner/optimizers/selectors/selector.py
--rw-r--r--   0        0        0      888 2024-04-11 07:42:16.046290 prompt_learner-0.2.0/prompt_learner/optimizers/selectors/stratified_sampler.py
--rw-r--r--   0        0        0       26 2024-04-11 03:24:06.645622 prompt_learner-0.2.0/prompt_learner/prompts/__init__.py
--rw-r--r--   0        0        0      597 2024-05-02 04:09:00.049153 prompt_learner-0.2.0/prompt_learner/prompts/cot.py
--rw-r--r--   0        0        0     1136 2024-05-02 04:10:24.786688 prompt_learner-0.2.0/prompt_learner/prompts/prompt.py
--rw-r--r--   0        0        0       22 2024-04-11 03:23:46.852998 prompt_learner-0.2.0/prompt_learner/tasks/__init__.py
--rw-r--r--   0        0        0      625 2024-05-02 04:33:01.819102 prompt_learner-0.2.0/prompt_learner/tasks/classification.py
--rw-r--r--   0        0        0      400 2024-04-18 06:38:05.061557 prompt_learner-0.2.0/prompt_learner/tasks/sql_generation.py
--rw-r--r--   0        0        0      529 2024-04-11 03:43:06.447386 prompt_learner-0.2.0/prompt_learner/tasks/tagging.py
--rw-r--r--   0        0        0     1589 2024-04-18 07:03:05.419391 prompt_learner-0.2.0/prompt_learner/tasks/task.py
--rw-r--r--   0        0        0       30 2024-04-11 03:23:57.503062 prompt_learner-0.2.0/prompt_learner/templates/__init__.py
--rw-r--r--   0        0        0     2819 2024-05-03 22:21:49.890118 prompt_learner-0.2.0/prompt_learner/templates/claude_template.py
--rw-r--r--   0        0        0     2610 2024-05-03 22:22:14.955790 prompt_learner-0.2.0/prompt_learner/templates/gpt_template.py
--rw-r--r--   0        0        0     2824 2024-05-03 22:21:49.889834 prompt_learner-0.2.0/prompt_learner/templates/llama_template.py
--rw-r--r--   0        0        0     1570 2024-04-18 06:49:29.458366 prompt_learner-0.2.0/prompt_learner/templates/template.py
--rw-r--r--   0        0        0     3373 2024-05-03 05:36:59.720092 prompt_learner-0.2.0/prompt_learner/translator/translate.py
--rw-r--r--   0        0        0      459 2024-05-03 22:31:16.739118 prompt_learner-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2817 1970-01-01 00:00:00.000000 prompt_learner-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2140 2024-05-07 04:41:30.281248 prompt_learner-0.2.1/README.md
+-rw-r--r--   0        0        0     6148 2024-05-07 04:41:30.293507 prompt_learner-0.2.1/prompt_learner/.DS_Store
+-rw-r--r--   0        0        0       28 2024-05-07 04:41:30.293626 prompt_learner-0.2.1/prompt_learner/adapters/__init__.py
+-rw-r--r--   0        0        0      394 2024-05-07 04:41:30.293694 prompt_learner-0.2.1/prompt_learner/adapters/adapter.py
+-rw-r--r--   0        0        0     1291 2024-05-07 04:41:30.293764 prompt_learner-0.2.1/prompt_learner/adapters/anthropic.py
+-rw-r--r--   0        0        0      659 2024-05-07 04:52:50.363858 prompt_learner-0.2.1/prompt_learner/adapters/llama.py
+-rw-r--r--   0        0        0      662 2024-05-07 04:41:30.293913 prompt_learner-0.2.1/prompt_learner/adapters/openai.py
+-rw-r--r--   0        0        0     1295 2024-05-07 04:41:30.294069 prompt_learner-0.2.1/prompt_learner/evals/metrics/accuracy.py
+-rw-r--r--   0        0        0       29 2024-05-07 04:41:30.294168 prompt_learner-0.2.1/prompt_learner/examples/__init__.py
+-rw-r--r--   0        0        0      316 2024-05-07 04:41:30.294240 prompt_learner-0.2.1/prompt_learner/examples/example.py
+-rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294327 prompt_learner-0.2.1/prompt_learner/examples/manipulation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294404 prompt_learner-0.2.1/prompt_learner/inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294446 prompt_learner-0.2.1/prompt_learner/inference/predict.py
+-rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294532 prompt_learner-0.2.1/prompt_learner/optimizers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294619 prompt_learner-0.2.1/prompt_learner/optimizers/descriptors/__init__.py
+-rw-r--r--   0        0        0      165 2024-05-07 04:41:30.294703 prompt_learner-0.2.1/prompt_learner/optimizers/descriptors/descriptor.py
+-rw-r--r--   0        0        0       34 2024-05-07 04:41:30.294768 prompt_learner-0.2.1/prompt_learner/optimizers/optimizer.py
+-rw-r--r--   0        0        0       30 2024-05-07 04:41:30.294865 prompt_learner-0.2.1/prompt_learner/optimizers/selectors/__init__.py
+-rw-r--r--   0        0        0     1537 2024-05-07 04:41:30.294949 prompt_learner-0.2.1/prompt_learner/optimizers/selectors/diverse_sampler.py
+-rw-r--r--   0        0        0      624 2024-05-07 04:41:30.295030 prompt_learner-0.2.1/prompt_learner/optimizers/selectors/random_sampler.py
+-rw-r--r--   0        0        0      873 2024-05-07 04:41:30.295104 prompt_learner-0.2.1/prompt_learner/optimizers/selectors/selector.py
+-rw-r--r--   0        0        0      888 2024-05-07 04:41:30.295186 prompt_learner-0.2.1/prompt_learner/optimizers/selectors/stratified_sampler.py
+-rw-r--r--   0        0        0       26 2024-05-07 04:41:30.295292 prompt_learner-0.2.1/prompt_learner/prompts/__init__.py
+-rw-r--r--   0        0        0      597 2024-05-07 04:41:30.295363 prompt_learner-0.2.1/prompt_learner/prompts/cot.py
+-rw-r--r--   0        0        0     1136 2024-05-07 04:41:30.295433 prompt_learner-0.2.1/prompt_learner/prompts/prompt.py
+-rw-r--r--   0        0        0       22 2024-05-07 04:41:30.295534 prompt_learner-0.2.1/prompt_learner/tasks/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-07 04:41:30.295599 prompt_learner-0.2.1/prompt_learner/tasks/classification.py
+-rw-r--r--   0        0        0      400 2024-05-07 04:41:30.295663 prompt_learner-0.2.1/prompt_learner/tasks/sql_generation.py
+-rw-r--r--   0        0        0      529 2024-05-07 04:41:30.295736 prompt_learner-0.2.1/prompt_learner/tasks/tagging.py
+-rw-r--r--   0        0        0     1589 2024-05-07 04:41:30.295807 prompt_learner-0.2.1/prompt_learner/tasks/task.py
+-rw-r--r--   0        0        0       30 2024-05-07 04:41:30.295907 prompt_learner-0.2.1/prompt_learner/templates/__init__.py
+-rw-r--r--   0        0        0     2819 2024-05-07 04:41:30.295990 prompt_learner-0.2.1/prompt_learner/templates/claude_template.py
+-rw-r--r--   0        0        0     2610 2024-05-07 04:41:30.296049 prompt_learner-0.2.1/prompt_learner/templates/gpt_template.py
+-rw-r--r--   0        0        0     1570 2024-05-07 04:41:30.296119 prompt_learner-0.2.1/prompt_learner/templates/template.py
+-rw-r--r--   0        0        0     3373 2024-05-07 04:41:30.296253 prompt_learner-0.2.1/prompt_learner/translator/translate.py
+-rw-r--r--   0        0        0      485 2024-05-09 03:55:53.413600 prompt_learner-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 prompt_learner-0.2.1/PKG-INFO
```

### Comparing `prompt_learner-0.2.0/README.md` & `prompt_learner-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/.DS_Store` & `prompt_learner-0.2.1/prompt_learner/.DS_Store`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/adapters/anthropic.py` & `prompt_learner-0.2.1/prompt_learner/adapters/anthropic.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/adapters/llama.py` & `prompt_learner-0.2.1/prompt_learner/adapters/openai.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""This module contains the Llama class
-which is used to interact with the Fireworks API."""
+"""This module contains the OpenAI class
+which is used to interact with the OpenAI API."""
 
 import os
-from langchain_fireworks import ChatFireworks
+from langchain_openai import ChatOpenAI
 from dotenv import load_dotenv
 from .adapter import Adapter
 
 
-class Llama(Adapter):
-    """An adapter for a llama model call using fireworks"""
-    def __init__(self, temperature: float = 0.0, max_tokens: int = 1024, model_name: str = "llama-v3-70b-instruct"):
+class OpenAI(Adapter):
+    """An adapter for an OpenAI language model call"""
+    def __init__(self, temperature: float = 0.0, max_tokens: int = 1024, model_name: str = "gpt-3.5-turbo"):
         super().__init__(temperature, max_tokens)
         load_dotenv()
-        self.llm = ChatFireworks(
-            model='accounts/fireworks/models/'+model_name,
-            fireworks_api_key=os.getenv('FIREWORKS_API_KEY'),
+        self.llm = ChatOpenAI(
+            openai_api_key=os.getenv('OPENAI_API_KEY'),
+            model=model_name,
             temperature=self.temperature,
             max_tokens=self.max_tokens)
```

### Comparing `prompt_learner-0.2.0/prompt_learner/evals/metrics/accuracy.py` & `prompt_learner-0.2.1/prompt_learner/evals/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/optimizers/selectors/diverse_sampler.py` & `prompt_learner-0.2.1/prompt_learner/optimizers/selectors/diverse_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/optimizers/selectors/random_sampler.py` & `prompt_learner-0.2.1/prompt_learner/optimizers/selectors/random_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/optimizers/selectors/selector.py` & `prompt_learner-0.2.1/prompt_learner/optimizers/selectors/selector.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/optimizers/selectors/stratified_sampler.py` & `prompt_learner-0.2.1/prompt_learner/optimizers/selectors/stratified_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/prompts/cot.py` & `prompt_learner-0.2.1/prompt_learner/prompts/cot.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/prompts/prompt.py` & `prompt_learner-0.2.1/prompt_learner/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/tasks/classification.py` & `prompt_learner-0.2.1/prompt_learner/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/tasks/tagging.py` & `prompt_learner-0.2.1/prompt_learner/tasks/tagging.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/tasks/task.py` & `prompt_learner-0.2.1/prompt_learner/tasks/task.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/templates/claude_template.py` & `prompt_learner-0.2.1/prompt_learner/templates/claude_template.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/templates/gpt_template.py` & `prompt_learner-0.2.1/prompt_learner/templates/gpt_template.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/templates/template.py` & `prompt_learner-0.2.1/prompt_learner/templates/template.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/prompt_learner/translator/translate.py` & `prompt_learner-0.2.1/prompt_learner/translator/translate.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.0/PKG-INFO` & `prompt_learner-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: prompt-learner
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Aditya Lahiri
 Author-email: adityalahiri13@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: black (>=24.3.0,<25.0.0)
 Requires-Dist: langchain (>=0.1.13,<0.2.0)
 Requires-Dist: langchain-anthropic (>=0.1.4,<0.2.0)
 Requires-Dist: langchain-fireworks (>=0.1.2,<0.2.0)
+Requires-Dist: langchain-groq (>=0.1.3,<0.2.0)
 Requires-Dist: langchain-openai (>=0.1.5,<0.2.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Prompt Learner
```

