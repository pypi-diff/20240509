# Comparing `tmp/athena_starship-0.0.4.tar.gz` & `tmp/athena_starship-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_starship-0.0.4.tar", max compression
+gzip compressed data, was "athena_starship-0.0.5.tar", max compression
```

## Comparing `athena_starship-0.0.4.tar` & `athena_starship-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        1 2024-05-08 23:20:52.861407 athena_starship-0.0.4/LICENSE
--rw-r--r--   0        0        0     1290 2024-05-08 23:56:29.101861 athena_starship-0.0.4/README.md
--rw-r--r--   0        0        0      118 2024-05-09 00:10:01.147469 athena_starship-0.0.4/athena_starship/__init__.py
--rw-r--r--   0        0        0     2375 2024-05-08 23:34:28.241612 athena_starship-0.0.4/athena_starship/data_connectors.py
--rw-r--r--   0        0        0     1010 2024-05-08 23:20:52.885141 athena_starship-0.0.4/athena_starship/ghost_datasource_urls.py
--rw-r--r--   0        0        0     3073 2024-05-09 00:09:42.918424 athena_starship-0.0.4/athena_starship/llama.py
--rw-r--r--   0        0        0     5403 2024-05-08 23:39:54.739467 athena_starship-0.0.4/athena_starship/memory.py
--rw-r--r--   0        0        0     1822 2024-05-08 23:20:52.886160 athena_starship-0.0.4/athena_starship/tool_schemas.py
--rw-r--r--   0        0        0        0 2024-05-08 23:27:03.908694 athena_starship-0.0.4/athena_starship/tools/__init__.py
--rw-r--r--   0        0        0     2932 2024-05-08 23:33:29.346598 athena_starship-0.0.4/athena_starship/tools/google_calendar.py
--rw-r--r--   0        0        0     2478 2024-05-08 23:20:52.886402 athena_starship-0.0.4/athena_starship/youtube_utils.py
--rw-r--r--   0        0        0     1345 2024-05-09 00:10:17.391836 athena_starship-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2021 1970-01-01 00:00:00.000000 athena_starship-0.0.4/setup.py
--rw-r--r--   0        0        0     2217 1970-01-01 00:00:00.000000 athena_starship-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        1 2024-05-08 23:20:52.861407 athena_starship-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1292 2024-05-09 00:27:53.965621 athena_starship-0.0.5/README.md
+-rw-r--r--   0        0        0      119 2024-05-09 00:41:37.630435 athena_starship-0.0.5/athena_starship/__init__.py
+-rw-r--r--   0        0        0     2375 2024-05-08 23:34:28.241612 athena_starship-0.0.5/athena_starship/data_connectors.py
+-rw-r--r--   0        0        0     1010 2024-05-08 23:20:52.885141 athena_starship-0.0.5/athena_starship/ghost_datasource_urls.py
+-rw-r--r--   0        0        0     3079 2024-05-09 00:55:43.715183 athena_starship-0.0.5/athena_starship/llama.py
+-rw-r--r--   0        0        0     5403 2024-05-08 23:39:54.739467 athena_starship-0.0.5/athena_starship/memory.py
+-rw-r--r--   0        0        0     1822 2024-05-08 23:20:52.886160 athena_starship-0.0.5/athena_starship/tool_schemas.py
+-rw-r--r--   0        0        0        0 2024-05-08 23:27:03.908694 athena_starship-0.0.5/athena_starship/tools/__init__.py
+-rw-r--r--   0        0        0     2932 2024-05-08 23:33:29.346598 athena_starship-0.0.5/athena_starship/tools/google_calendar.py
+-rw-r--r--   0        0        0     2478 2024-05-08 23:20:52.886402 athena_starship-0.0.5/athena_starship/youtube_utils.py
+-rw-r--r--   0        0        0     1345 2024-05-09 00:55:57.765868 athena_starship-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 athena_starship-0.0.5/setup.py
+-rw-r--r--   0        0        0     2219 1970-01-01 00:00:00.000000 athena_starship-0.0.5/PKG-INFO
```

### Comparing `athena_starship-0.0.4/README.md` & `athena_starship-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     max_loops="auto",
     interactive=True,
     autosave=True,
     dashboard=True,
     long_term_memory=chromadb,
     stopping_token="<DONE>",
     verbose=True,
-    tools=[calendar],
+    # tools=[calendar],
 )
 
 # Run the workflow on a task
 agent.run(
     "What are the 3 traits you look for before investing in a seed"
     " stage startup?"
 )
```

### Comparing `athena_starship-0.0.4/athena_starship/data_connectors.py` & `athena_starship-0.0.5/athena_starship/data_connectors.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.4/athena_starship/ghost_datasource_urls.py` & `athena_starship-0.0.5/athena_starship/ghost_datasource_urls.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.4/athena_starship/llama.py` & `athena_starship-0.0.5/athena_starship/llama.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from transformers import AutoTokenizer, AutoModelForCausalLM
 import torch
 from swarms.models.base_llm import BaseLLM
 
+
 class Llama3(BaseLLM):
     """
     Llama3 class represents a Llama model for natural language generation.
 
     Args:
         model_id (str): The ID of the Llama model to use.
         system_prompt (str): The system prompt to use for generating responses.
@@ -31,15 +32,15 @@
     def __init__(
         self,
         model_id="meta-llama/Meta-Llama-3-8B-Instruct",
         system_prompt: str = None,
         temperature: float = 0.6,
         top_p: float = 0.9,
         max_tokens: int = 4000,
-        **kwargs
+        **kwargs,
     ):
         self.model_id = model_id
         self.system_prompt = system_prompt
         self.temperature = temperature
         self.top_p = top_p
         self.max_tokens = max_tokens
         self.tokenizer = AutoTokenizer.from_pretrained(model_id)
@@ -62,27 +63,27 @@
         """
         messages = [
             {"role": "system", "content": self.system_prompt},
             {"role": "user", "content": task},
         ]
 
         input_ids = self.tokenizer.apply_chat_template(
-            messages,
-            add_generation_prompt=True,
-            return_tensors="pt"
+            messages, add_generation_prompt=True, return_tensors="pt"
         ).to(self.model.device)
 
         terminators = [
             self.tokenizer.eos_token_id,
-            self.tokenizer.convert_tokens_to_ids("<|eot_id|>")
+            self.tokenizer.convert_tokens_to_ids("<|eot_id|>"),
         ]
 
-        outputs = self.generate(
+        outputs = self.model.generate(
             input_ids,
             max_new_tokens=self.max_tokens,
             eos_token_id=terminators,
             do_sample=True,
             temperature=self.temperature,
             top_p=self.top_p,
         )
-        response = outputs[0][input_ids.shape[-1]:]
-        return (self.tokenizer.decode(response, skip_special_tokens=True))
+        response = outputs[0][input_ids.shape[-1] :]
+        return self.tokenizer.decode(
+            response, skip_special_tokens=True
+        )
```

### Comparing `athena_starship-0.0.4/athena_starship/memory.py` & `athena_starship-0.0.5/athena_starship/memory.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.4/athena_starship/tool_schemas.py` & `athena_starship-0.0.5/athena_starship/tool_schemas.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.4/athena_starship/tools/google_calendar.py` & `athena_starship-0.0.5/athena_starship/tools/google_calendar.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.4/athena_starship/youtube_utils.py` & `athena_starship-0.0.5/athena_starship/youtube_utils.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.4/pyproject.toml` & `athena_starship-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "athena-starship"
-version = "0.0.4"
+version = "0.0.5"
 description = "Paper - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/Starship-Ventures/Athena"
 documentation = "https://github.com/Starship-Ventures/Athena"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/Starship-Ventures/Athena"
```

### Comparing `athena_starship-0.0.4/setup.py` & `athena_starship-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['swarms==4.9.3']
 
 setup_kwargs = {
     'name': 'athena-starship',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Paper - Pytorch',
-    'long_description': '# Athena\n\n## Install\n`$ pip install athena-starship`\n\n## Usage\n```bash\npython3 sam_altman.py\n```\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent\nfrom athena_starship.llama import llama\nfrom athena_starship.memory import ChromaDB\nfrom athena_starship.tools.google_calendar import calendar\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initilaize the chromadb client\nchromadb = ChromaDB(\n    metric="cosine",\n    verbose=True,\n    n_results=3,\n)\n\n## Initialize the workflow\nagent = Agent(\n    llm=llama,\n    agent_name="Sam Altman",\n    agent_description="Sam Altman Agent, CEO of OpenAI.",\n    system_prompt="You\'re Sam Altman, CEO of OpenAI.",\n    max_loops="auto",\n    interactive=True,\n    autosave=True,\n    dashboard=True,\n    long_term_memory=chromadb,\n    stopping_token="<DONE>",\n    verbose=True,\n    tools=[calendar],\n)\n\n# Run the workflow on a task\nagent.run(\n    "What are the 3 traits you look for before investing in a seed"\n    " stage startup?"\n)\n\n```\n\n# License\nMIT\n\n\n# Todo\n- [ ] Make csv of few shot prompt examples for various tool usages\n- [ ] Make tools for airtable, google calendar, notion, gmail\n',
+    'long_description': '# Athena\n\n## Install\n`$ pip install athena-starship`\n\n## Usage\n```bash\npython3 sam_altman.py\n```\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent\nfrom athena_starship.llama import llama\nfrom athena_starship.memory import ChromaDB\nfrom athena_starship.tools.google_calendar import calendar\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initilaize the chromadb client\nchromadb = ChromaDB(\n    metric="cosine",\n    verbose=True,\n    n_results=3,\n)\n\n## Initialize the workflow\nagent = Agent(\n    llm=llama,\n    agent_name="Sam Altman",\n    agent_description="Sam Altman Agent, CEO of OpenAI.",\n    system_prompt="You\'re Sam Altman, CEO of OpenAI.",\n    max_loops="auto",\n    interactive=True,\n    autosave=True,\n    dashboard=True,\n    long_term_memory=chromadb,\n    stopping_token="<DONE>",\n    verbose=True,\n    # tools=[calendar],\n)\n\n# Run the workflow on a task\nagent.run(\n    "What are the 3 traits you look for before investing in a seed"\n    " stage startup?"\n)\n\n```\n\n# License\nMIT\n\n\n# Todo\n- [ ] Make csv of few shot prompt examples for various tool usages\n- [ ] Make tools for airtable, google calendar, notion, gmail\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Starship-Ventures/Athena',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `athena_starship-0.0.4/PKG-INFO` & `athena_starship-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-starship
-Version: 0.0.4
+Version: 0.0.5
 Summary: Paper - Pytorch
 Home-page: https://github.com/Starship-Ventures/Athena
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
@@ -64,15 +64,15 @@
     max_loops="auto",
     interactive=True,
     autosave=True,
     dashboard=True,
     long_term_memory=chromadb,
     stopping_token="<DONE>",
     verbose=True,
-    tools=[calendar],
+    # tools=[calendar],
 )
 
 # Run the workflow on a task
 agent.run(
     "What are the 3 traits you look for before investing in a seed"
     " stage startup?"
 )
```

