# Comparing `tmp/llama_index_tools_multion-0.1.3.tar.gz` & `tmp/llama_index_tools_multion-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_tools_multion-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_tools_multion-0.2.0.tar", max compression
```

## Comparing `llama_index_tools_multion-0.1.3.tar` & `llama_index_tools_multion-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1121 2024-02-20 18:45:10.334617 llama_index_tools_multion-0.1.3/README.md
--rw-r--r--   0        0        0       90 2024-02-13 13:53:01.947845 llama_index_tools_multion-0.1.3/llama_index/tools/multion/__init__.py
--rw-r--r--   0        0        0     1935 2024-02-13 13:53:01.947908 llama_index_tools_multion-0.1.3/llama_index/tools/multion/base.py
--rw-r--r--   0        0        0     1525 2024-02-21 22:21:01.354254 llama_index_tools_multion-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 llama_index_tools_multion-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1128 2024-05-08 23:49:40.646813 llama_index_tools_multion-0.2.0/README.md
+-rw-r--r--   0        0        0       90 2024-05-08 23:49:40.646813 llama_index_tools_multion-0.2.0/llama_index/tools/multion/__init__.py
+-rw-r--r--   0        0        0      956 2024-05-08 23:49:40.646813 llama_index_tools_multion-0.2.0/llama_index/tools/multion/base.py
+-rw-r--r--   0        0        0     1525 2024-05-08 23:49:40.646813 llama_index_tools_multion-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 llama_index_tools_multion-0.2.0/PKG-INFO
```

### Comparing `llama_index_tools_multion-0.1.3/README.md` & `llama_index_tools_multion-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # MultiOn Tool
 
+```bash
+pip install llama-index-tools-multion
+```
+
 This tool connects to [MultiOn](https://www.multion.ai/) to enable your agent to easily
 connect to the internet through your Chrome Web browser and act on your behalf
 
 You will need to have the MultiOn chrome extension installed and a MultiOn account
 to use this integration
 
 ## Usage
 
 This tool has more a extensive example usage documented in a Jupyter notebook [here](https://github.com/emptycrown/llama-hub/tree/main/llama_hub/tools/notebooks/multion.ipynb)
 
 Here's an example usage of the MultionToolSpec.
 
 ```python
-from llama_index.tools.metaphor import MultionToolSpec
-from llama_index.agent import OpenAIAgent
+from llama_index.tools.multion import MultionToolSpec
+from llama_index.agent.openai import OpenAIAgent
 
-multion_tool = MultionToolSpec()
+multion_tool = MultionToolSpec(api_key="your-multion-key")
 
 agent = OpenAIAgent.from_tools(multion_tool.to_tool_list())
 
 agent.chat("Can you read the latest tweets from my followers")
 agent.chat("What's the next thing on my google calendar?")
 ```
 
 `browse`: The core function that takes natural language instructions to pass to the web browser to execute
 
-This loader is designed to be used as a way to load data as a Tool in a Agent. See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
+This loader is designed to be used as a way to load data as a Tool in a Agent.
```

### Comparing `llama_index_tools_multion-0.1.3/pyproject.toml` & `llama_index_tools_multion-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index tools multion integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["ajhofmann"]
 name = "llama-index-tools-multion"
 readme = "README.md"
-version = "0.1.3"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 multion = "^0.3.11"
 pytesseract = "^0.3.10"
 pillow = "^10.2.0"
```

### Comparing `llama_index_tools_multion-0.1.3/PKG-INFO` & `llama_index_tools_multion-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 Metadata-Version: 2.1
 Name: llama-index-tools-multion
-Version: 0.1.3
+Version: 0.2.0
 Summary: llama-index tools multion integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Maintainer: ajhofmann
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: multion (>=0.3.11,<0.4.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Description-Content-Type: text/markdown
 
 # MultiOn Tool
 
+```bash
+pip install llama-index-tools-multion
+```
+
 This tool connects to [MultiOn](https://www.multion.ai/) to enable your agent to easily
 connect to the internet through your Chrome Web browser and act on your behalf
 
 You will need to have the MultiOn chrome extension installed and a MultiOn account
 to use this integration
 
 ## Usage
 
 This tool has more a extensive example usage documented in a Jupyter notebook [here](https://github.com/emptycrown/llama-hub/tree/main/llama_hub/tools/notebooks/multion.ipynb)
 
 Here's an example usage of the MultionToolSpec.
 
 ```python
-from llama_index.tools.metaphor import MultionToolSpec
-from llama_index.agent import OpenAIAgent
+from llama_index.tools.multion import MultionToolSpec
+from llama_index.agent.openai import OpenAIAgent
 
-multion_tool = MultionToolSpec()
+multion_tool = MultionToolSpec(api_key="your-multion-key")
 
 agent = OpenAIAgent.from_tools(multion_tool.to_tool_list())
 
 agent.chat("Can you read the latest tweets from my followers")
 agent.chat("What's the next thing on my google calendar?")
 ```
 
 `browse`: The core function that takes natural language instructions to pass to the web browser to execute
 
-This loader is designed to be used as a way to load data as a Tool in a Agent. See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
+This loader is designed to be used as a way to load data as a Tool in a Agent.
```

