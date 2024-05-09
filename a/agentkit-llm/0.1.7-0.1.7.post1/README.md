# Comparing `tmp/agentkit-llm-0.1.7.tar.gz` & `tmp/agentkit-llm-0.1.7.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentkit-llm-0.1.7.tar", last modified: Mon May  6 21:48:06 2024, max compression
+gzip compressed data, was "agentkit-llm-0.1.7.post1.tar", last modified: Thu May  9 00:26:26 2024, max compression
```

## Comparing `agentkit-llm-0.1.7.tar` & `agentkit-llm-0.1.7.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-06 21:48:06.241146 agentkit-llm-0.1.7/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.7/LICENSE
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     9016 2024-05-06 21:48:06.241146 agentkit-llm-0.1.7/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     8505 2024-05-06 21:46:13.000000 agentkit-llm-0.1.7/README.md
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-05-06 21:48:06.241146 agentkit-llm-0.1.7/setup.cfg
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1068 2024-05-06 21:33:58.000000 agentkit-llm-0.1.7/setup.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-06 21:48:06.237146 agentkit-llm-0.1.7/src/
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-06 21:48:06.241146 agentkit-llm-0.1.7/src/agentkit/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.7/src/agentkit/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2951 2024-04-29 05:28:17.000000 agentkit-llm-0.1.7/src/agentkit/after_query.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-05-06 21:44:02.000000 agentkit-llm-0.1.7/src/agentkit/base_node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.7/src/agentkit/compose_prompt.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.7/src/agentkit/exceptions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.7/src/agentkit/graph.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-06 21:48:06.241146 agentkit-llm-0.1.7/src/agentkit/llm_api/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4799 2024-05-06 21:41:05.000000 agentkit-llm-0.1.7/src/agentkit/llm_api/GPT.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1726 2024-05-06 21:26:12.000000 agentkit-llm-0.1.7/src/agentkit/llm_api/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4226 2024-05-06 21:20:24.000000 agentkit-llm-0.1.7/src/agentkit/llm_api/base.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4615 2024-04-24 17:43:52.000000 agentkit-llm-0.1.7/src/agentkit/llm_api/claude.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     3782 2024-05-06 21:32:28.000000 agentkit-llm-0.1.7/src/agentkit/llm_api/ollama.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1613 2024-05-06 21:24:37.000000 agentkit-llm-0.1.7/src/agentkit/llm_api/utils.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.7/src/agentkit/node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.7/src/agentkit/node_functions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.7/src/agentkit/utils.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-06 21:48:06.241146 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/
--rw-r--r--   0 holmes    (1000) holmes    (1000)     9016 2024-05-06 21:48:06.000000 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      683 2024-05-06 21:48:06.000000 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/SOURCES.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-05-06 21:48:06.000000 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/dependency_links.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-05-06 21:48:06.000000 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/entry_points.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      124 2024-05-06 21:48:06.000000 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/requires.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-05-06 21:48:06.000000 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/top_level.txt
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-09 00:26:26.311713 agentkit-llm-0.1.7.post1/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.7.post1/LICENSE
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     9022 2024-05-09 00:26:26.311713 agentkit-llm-0.1.7.post1/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     8505 2024-05-06 21:46:13.000000 agentkit-llm-0.1.7.post1/README.md
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-05-09 00:26:26.311713 agentkit-llm-0.1.7.post1/setup.cfg
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1074 2024-05-09 00:26:10.000000 agentkit-llm-0.1.7.post1/setup.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-09 00:26:26.307713 agentkit-llm-0.1.7.post1/src/
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-09 00:26:26.307713 agentkit-llm-0.1.7.post1/src/agentkit/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.7.post1/src/agentkit/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2951 2024-04-29 05:28:17.000000 agentkit-llm-0.1.7.post1/src/agentkit/after_query.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-05-06 21:44:02.000000 agentkit-llm-0.1.7.post1/src/agentkit/base_node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.7.post1/src/agentkit/compose_prompt.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.7.post1/src/agentkit/exceptions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.7.post1/src/agentkit/graph.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-09 00:26:26.311713 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4799 2024-05-06 21:41:05.000000 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/GPT.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1635 2024-05-09 00:25:51.000000 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4226 2024-05-06 21:20:24.000000 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/base.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4615 2024-04-24 17:43:52.000000 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/claude.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     3783 2024-05-09 00:25:51.000000 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/ollama.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1681 2024-05-09 00:25:51.000000 agentkit-llm-0.1.7.post1/src/agentkit/llm_api/utils.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.7.post1/src/agentkit/node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.7.post1/src/agentkit/node_functions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.7.post1/src/agentkit/utils.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-09 00:26:26.311713 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/
+-rw-r--r--   0 holmes    (1000) holmes    (1000)     9022 2024-05-09 00:26:26.000000 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      683 2024-05-09 00:26:26.000000 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/SOURCES.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-05-09 00:26:26.000000 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/dependency_links.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-05-09 00:26:26.000000 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/entry_points.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      124 2024-05-09 00:26:26.000000 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/requires.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-05-09 00:26:26.000000 agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/top_level.txt
```

### Comparing `agentkit-llm-0.1.7/LICENSE` & `agentkit-llm-0.1.7.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7/PKG-INFO` & `agentkit-llm-0.1.7.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.7
+Version: 0.1.7.post1
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/rhyswynn/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `agentkit-llm-0.1.7/README.md` & `agentkit-llm-0.1.7.post1/README.md`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7/setup.py` & `agentkit-llm-0.1.7.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import pkg_resources
 import pathlib
 
 PKG_NAME = "agentkit-llm"
-VERSION = "0.1.7"
+VERSION = "0.1.7.post1"
 EXTRAS = {
     "logging": ["wandb"],
     "proprietary": ["wandb", "openai", "anthropic", "tiktoken"],
     "all": ["wandb", "openai", "anthropic", "tiktoken", "llama"],
 }
 
 setuptools.setup(
```

### Comparing `agentkit-llm-0.1.7/src/agentkit/after_query.py` & `agentkit-llm-0.1.7.post1/src/agentkit/after_query.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7/src/agentkit/base_node.py` & `agentkit-llm-0.1.7.post1/src/agentkit/base_node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7/src/agentkit/compose_prompt.py` & `agentkit-llm-0.1.7.post1/src/agentkit/compose_prompt.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7/src/agentkit/exceptions.py` & `agentkit-llm-0.1.7.post1/src/agentkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7/src/agentkit/graph.py` & `agentkit-llm-0.1.7.post1/src/agentkit/graph.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7/src/agentkit/llm_api/GPT.py` & `agentkit-llm-0.1.7.post1/src/agentkit/llm_api/GPT.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7/src/agentkit/llm_api/__init__.py` & `agentkit-llm-0.1.7.post1/src/agentkit/llm_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     global token_counter
     query_model = Claude_chat(model, token_counter)
     return query_model
 
 def query_ollama_chat(model):
     from .ollama import Ollama_chat
     global token_counter
-    model = model.replace('ollama:','')
+    #model = model.replace('ollama-','')
     query_model = Ollama_chat(model, token_counter)
     return query_model
 
-def get_query(LLM_name, ollama_url=None, tokenmodel_path=None):
+def get_query(LLM_name):
     """Get the query model for the specified LLM_name.
 
     Currently supported LLMs:
 
     - GPT-4
 
     - GPT-3.5
@@ -49,10 +49,10 @@
     """
     print("Warning: The built-in LLM API is only for testing, and will not be actively maintained. Please write your own API for production use.")
     if LLM_name.lower().startswith("gpt-4") or LLM_name.lower().startswith("gpt-3.5"):
         return query_gpt_chat(model=LLM_name)
     elif LLM_name.lower().startswith("claude"):
         return query_claude_chat(model=LLM_name)
     elif LLM_name.lower().startswith("ollama-"):
-        return query_ollama_chat(model=LLM_name,ollama_url=ollama_url,tokenmodel_path=tokenmodel_path)
+        return query_ollama_chat(model=LLM_name)
     else:
-        raise NotImplementedError("LLM {} not implemented".format(LLM_name))
+        raise NotImplementedError("LLM {} not implemented".format(LLM_name))
```

### Comparing `agentkit-llm-0.1.7/src/agentkit/llm_api/base.py` & `agentkit-llm-0.1.7.post1/src/agentkit/llm_api/base.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7/src/agentkit/llm_api/claude.py` & `agentkit-llm-0.1.7.post1/src/agentkit/llm_api/claude.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7/src/agentkit/llm_api/ollama.py` & `agentkit-llm-0.1.7.post1/src/agentkit/llm_api/ollama.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 class Ollama_chat(BaseModel):
 
     def __init__(self, model_name, global_counter=None):
 
         tokenmodel_path, ollama_url = initialize_client()
         model_max, enc_fn = match_model(model_name)
-        model_name = model_name.replace('ollama:','')
+        model_name = model_name.replace('ollama-','')
         self.model_name = model_name
         self.name = model_name
         self.sp_model = Tokenizer(tokenmodel_path)
         self.url = f'{ollama_url}/api/chat'
         self.model_max = model_max
         super().__init__(model_name, global_counter, "chat")
     
@@ -79,8 +79,8 @@
                     import re
                     val = int(re.findall(r'\d+', e[index + len("your messages resulted in ") : ])[0])
                     index2 = e.find("maximum context length is ")
                     model_max = int(re.findall(r'\d+', e[index2 + len("maximum context length is "):])[0])
                     messages = self.shrink_msg_by(messages, shrink_idx, val-model_max)
                 else:
                     time.sleep(5)
-                    print(e)
+                    print(e)
```

### Comparing `agentkit-llm-0.1.7/src/agentkit/llm_api/utils.py` & `agentkit-llm-0.1.7.post1/src/agentkit/llm_api/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,18 +31,20 @@
     "ollama":8192,
 }
 
 def match_model(model_name):
 
     # match model name to the closest string in enc_fns.keys()
     model_name = model_name.lower()
+    if model_name.startswith('ollama'):
+    	model_name = 'ollama'
     matches = difflib.get_close_matches(model_name, enc_fns.keys())
     matches += [model for model in model_maxes.keys() if model_name.startswith(model)]
     if len(matches) == 0:
         raise ValueError("Model name {} not found!".format(model_name))
     else:
         model = matches[0]
     print("Matched model_name {} to: {}. If this match is not accurate, then the token counter will not function properly.".format(model_name, model))
 
     model_max = model_maxes[model]
     enc_fn = enc_fns[model]
-    return model_max, enc_fn
+    return model_max, enc_fn
```

### Comparing `agentkit-llm-0.1.7/src/agentkit/node.py` & `agentkit-llm-0.1.7.post1/src/agentkit/node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7/src/agentkit/utils.py` & `agentkit-llm-0.1.7.post1/src/agentkit/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.7/src/agentkit_llm.egg-info/PKG-INFO` & `agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.7
+Version: 0.1.7.post1
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/rhyswynn/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `agentkit-llm-0.1.7/src/agentkit_llm.egg-info/SOURCES.txt` & `agentkit-llm-0.1.7.post1/src/agentkit_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

