# Comparing `tmp/modelmerge-0.2.4.tar.gz` & `tmp/modelmerge-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.2.4.tar", last modified: Thu May  9 16:41:33 2024, max compression
+gzip compressed data, was "modelmerge-0.2.5.tar", last modified: Thu May  9 17:08:31 2024, max compression
```

## Comparing `modelmerge-0.2.4.tar` & `modelmerge-0.2.5.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.959859 modelmerge-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 16:41:24.000000 modelmerge-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 16:41:33.959859 modelmerge-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 16:41:24.000000 modelmerge-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 16:41:33.959859 modelmerge-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 16:41:24.000000 modelmerge-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.955859 modelmerge-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.955859 modelmerge-0.2.4/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.959859 modelmerge-0.2.4/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30068 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.959859 modelmerge-0.2.4/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/plugins/travel.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.959859 modelmerge-0.2.4/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.959859 modelmerge-0.2.4/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.959859 modelmerge-0.2.4/src/ModelMerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 16:41:33.000000 modelmerge-0.2.4/src/ModelMerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 16:41:33.000000 modelmerge-0.2.4/src/ModelMerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:41:33.000000 modelmerge-0.2.4/src/ModelMerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 16:41:33.000000 modelmerge-0.2.4/src/ModelMerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 16:41:33.000000 modelmerge-0.2.4/src/ModelMerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.546149 modelmerge-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 17:08:23.000000 modelmerge-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 17:08:31.546149 modelmerge-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 17:08:23.000000 modelmerge-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:08:31.546149 modelmerge-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 17:08:23.000000 modelmerge-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.542149 modelmerge-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.542149 modelmerge-0.2.5/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.546149 modelmerge-0.2.5/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29814 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.546149 modelmerge-0.2.5/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/plugins/travel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.546149 modelmerge-0.2.5/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.546149 modelmerge-0.2.5/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.546149 modelmerge-0.2.5/src/ModelMerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 17:08:31.000000 modelmerge-0.2.5/src/ModelMerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 17:08:31.000000 modelmerge-0.2.5/src/ModelMerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:08:31.000000 modelmerge-0.2.5/src/ModelMerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 17:08:31.000000 modelmerge-0.2.5/src/ModelMerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 17:08:31.000000 modelmerge-0.2.5/src/ModelMerge.egg-info/top_level.txt
```

### Comparing `modelmerge-0.2.4/LICENSE` & `modelmerge-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.4/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.2.5/src/ModelMerge/models/chatgpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 import json
 import copy
 from pathlib import Path
 from typing import AsyncGenerator, Set
-from .config import BaseLLM, ENGINES, CUSTOM_MODELS, PLUGINS, LANGUAGE
+from .config import BaseLLM, PLUGINS, LANGUAGE
 
 import httpx
 import requests
 import tiktoken
 
 # import config
 from ..utils.scripts import check_json, cut_message
@@ -152,20 +152,20 @@
     ) -> None:
         """
         Truncate the conversation
         """
         while True:
             json_post = self.get_post_body(prompt, role, convo_id, model, pass_history, **kwargs)
             url = self.api_url.chat_url
-            if "gpt-4" in self.engine or "claude" in self.engine or (CUSTOM_MODELS and self.engine in CUSTOM_MODELS):
-                message_token = {
-                    "total": self.get_token_count(convo_id),
-                }
-            else:
-                message_token = self.get_message_token(url, json_post)
+            # if "gpt-4" in self.engine or "claude" in self.engine or (CUSTOM_MODELS and self.engine in CUSTOM_MODELS):
+            message_token = {
+                "total": self.get_token_count(convo_id),
+            }
+            # else:
+            #     message_token = self.get_message_token(url, json_post)
             print("message_token", message_token, "truncate_limit", self.truncate_limit)
             if (
                 message_token["total"] > self.truncate_limit
                 and len(self.conversation[convo_id]) > 1
             ):
                 # Don't remove the first message
                 mess = self.conversation[convo_id].pop(1)
@@ -192,18 +192,14 @@
     #             self.conversation[convo_id].remove(function_call_items[i])
 
     # https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     def get_token_count(self, convo_id: str = "default") -> int:
         """
         Get token count
         """
-        if self.engine not in ENGINES:
-            raise NotImplementedError(
-                f"Engine {self.engine} is not supported. Select from {ENGINES}",
-            )
         encoding = tiktoken.get_encoding("cl100k_base")
 
         num_tokens = 0
         for message in self.conversation[convo_id]:
             # every message follows <im_start>{role/name}\n{content}<im_end>\n
             num_tokens += 5
             for key, value in message.items():
@@ -285,15 +281,15 @@
             "frequency_penalty": kwargs.get(
                 "frequency_penalty",
                 self.frequency_penalty,
             ),
             "n": kwargs.get("n", self.reply_count),
             "user": role,
         }
-        if CUSTOM_MODELS and self.engine in CUSTOM_MODELS and "gpt-" not in self.engine and "claude-3" not in self.engine:
+        if "gpt-" not in self.engine and "claude-3" not in self.engine:
             return json_post_body
         json_post_body.update(copy.deepcopy(body))
         json_post_body.update(copy.deepcopy(function_call_list["base"]))
         for item in PLUGINS.keys():
             try:
                 if PLUGINS[item]:
                     json_post_body["functions"].append(function_call_list[item])
```

### Comparing `modelmerge-0.2.4/src/ModelMerge/models/claude.py` & `modelmerge-0.2.5/src/ModelMerge/models/claude.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ..tools.function_call import claude_tools_list
 import os
 import json
 import tiktoken
 import requests
 
-from .config import BaseLLM, ENGINES
+from .config import BaseLLM
 
 class claudeConversation(dict):
     def Conversation(self, index):
         conversation_list = super().__getitem__(index)
         return "\n\n" + "\n\n".join([f"{item['role']}:{item['content']}" for item in conversation_list]) + "\n\nAssistant:"
 
 class claude(BaseLLM):
@@ -61,18 +61,14 @@
             else:
                 break
 
     def get_token_count(self, convo_id: str = "default") -> int:
         """
         Get token count
         """
-        if self.engine not in ENGINES:
-            raise NotImplementedError(
-                f"Engine {self.engine} is not supported. Select from {ENGINES}",
-            )
         tiktoken.model.MODEL_TO_ENCODING["claude-2.1"] = "cl100k_base"
         encoding = tiktoken.encoding_for_model(self.engine)
 
         num_tokens = 0
         for message in self.conversation[convo_id]:
             # every message follows <im_start>{role/name}\n{content}<im_end>\n
             num_tokens += 5
@@ -209,18 +205,14 @@
             else:
                 break
 
     def get_token_count(self, convo_id: str = "default") -> int:
         """
         Get token count
         """
-        if self.engine not in ENGINES:
-            raise NotImplementedError(
-                f"Engine {self.engine} is not supported. Select from {ENGINES}",
-            )
         tiktoken.model.MODEL_TO_ENCODING["claude-2.1"] = "cl100k_base"
         encoding = tiktoken.encoding_for_model(self.engine)
 
         num_tokens = 0
         for message in self.conversation[convo_id]:
             # every message follows <im_start>{role/name}\n{content}<im_end>\n
             num_tokens += 5
```

### Comparing `modelmerge-0.2.4/src/ModelMerge/models/config.py` & `modelmerge-0.2.5/src/ModelMerge/models/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,54 +2,19 @@
 import json
 import httpx
 import requests
 from pathlib import Path
 
 from ..utils import prompt
 
-ENGINES = [
-    "gpt-3.5-turbo",
-    "gpt-3.5-turbo-16k",
-    "gpt-3.5-turbo-0301",
-    "gpt-3.5-turbo-0613",
-    "gpt-3.5-turbo-1106",
-    "gpt-3.5-turbo-16k-0613",
-    "gpt-4",
-    "gpt-4-0314",
-    "gpt-4-32k",
-    "gpt-4-32k-0314",
-    "gpt-4-0613",
-    "gpt-4-32k-0613",
-    "gpt-4-1106-preview",
-    "gpt-4-0125-preview",
-    "gpt-4-turbo-preview",
-    "gpt-4-turbo-2024-04-09",
-    "mixtral-8x7b-32768",
-    "llama2-70b-4096",
-    "llama3-70b-8192",
-    "claude-2.1",
-    "claude-3-sonnet-20240229",
-    "claude-3-haiku-20240307",
-    "claude-3-opus-20240229",
-    "gemini-1.5-pro-latest",
-]
-
-CUSTOM_MODELS = os.environ.get('CUSTOM_MODELS', None)
-if CUSTOM_MODELS:
-    CUSTOM_MODELS_LIST = [id for id in CUSTOM_MODELS.split(",")]
-    ENGINES.extend(CUSTOM_MODELS_LIST)
-else:
-    CUSTOM_MODELS_LIST = None
-
 PLUGINS = {
-    "SEARCH_USE_GPT": (os.environ.get('SEARCH_USE_GPT', "True") == "False") == False,
-    # "USE_G4F": (os.environ.get('USE_G4F', "False") == "False") == False,
-    "DATE": True,
+    "SEARCH": (os.environ.get('SEARCH', "True") == "False") == False,
     "URL": True,
-    "VERSION": True,
+    "DATE": False,
+    "VERSION": False,
 }
 
 LANGUAGE = os.environ.get('LANGUAGE', 'Simplified Chinese')
 
 class BaseAPI:
     def __init__(
         self,
```

### Comparing `modelmerge-0.2.4/src/ModelMerge/models/genimi.py` & `modelmerge-0.2.5/src/ModelMerge/models/genimi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 import requests
 import tiktoken
 
-from .config import BaseLLM, ENGINES
+from .config import BaseLLM
 
 class gemini(BaseLLM):
     def __init__(
         self,
         api_key: str,
         engine: str = os.environ.get("GPT_ENGINE") or "gemini-1.5-pro-latest",
         api_url: str = "https://generativelanguage.googleapis.com/v1beta/models/{model}:{stream}?key={api_key}",
@@ -58,18 +58,14 @@
             else:
                 break
 
     def get_token_count(self, convo_id: str = "default") -> int:
         """
         Get token count
         """
-        if self.engine not in ENGINES:
-            raise NotImplementedError(
-                f"Engine {self.engine} is not supported. Select from {ENGINES}",
-            )
         encoding = tiktoken.get_encoding("cl100k_base")
 
         num_tokens = 0
         for message in self.conversation[convo_id]:
             # every message follows <im_start>{role/name}\n{content}<im_end>\n
             num_tokens += 5
             for key, value in message.items():
```

### Comparing `modelmerge-0.2.4/src/ModelMerge/models/groq.py` & `modelmerge-0.2.5/src/ModelMerge/models/groq.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,38 @@
-class groqbot:
+import os
+import json
+import requests
+import tiktoken
+
+from .config import BaseLLM
+
+class groq(BaseLLM):
     def __init__(
         self,
         api_key: str,
         engine: str = os.environ.get("GPT_ENGINE") or "llama3-70b-8192",
+        api_url: str = "https://api.groq.com/openai/v1/chat/completions",
+        system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
         temperature: float = 0.5,
         top_p: float = 1,
-        chat_url: str = "https://api.groq.com/openai/v1/chat/completions",
         timeout: float = 20,
-        system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
-        **kwargs,
     ):
-        self.api_key: str = api_key
-        self.engine: str = engine
-        self.temperature = temperature
-        self.top_p = top_p
-        self.chat_url = chat_url
-        self.timeout = timeout
-        self.session = requests.Session()
-        self.conversation: dict[str, list[dict]] = {
-            "default": [
-                {
-                    "role": "system",
-                    "content": system_prompt,
-                },
-            ],
-        }
-        self.system_prompt = system_prompt
+        super().__init__(api_key, engine, api_url, system_prompt, timeout=timeout, temperature=temperature, top_p=top_p)
+        self.api_url = api_url
 
     def add_to_conversation(
         self,
         message: str,
         role: str,
         convo_id: str = "default",
         pass_history: bool = True,
     ) -> None:
         """
         Add a message to the conversation
         """
-
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
         self.conversation[convo_id].append({"role": role, "content": message})
 
     def reset(self, convo_id: str = "default", system_prompt: str = None) -> None:
         """
         Reset the conversation
@@ -62,18 +53,14 @@
             else:
                 break
 
     def get_token_count(self, convo_id: str = "default") -> int:
         """
         Get token count
         """
-        if self.engine not in ENGINES:
-            raise NotImplementedError(
-                f"Engine {self.engine} is not supported. Select from {ENGINES}",
-            )
         # tiktoken.model.MODEL_TO_ENCODING["mixtral-8x7b-32768"] = "cl100k_base"
         encoding = tiktoken.get_encoding("cl100k_base")
 
         num_tokens = 0
         for message in self.conversation[convo_id]:
             # every message follows <im_start>{role/name}\n{content}<im_end>\n
             num_tokens += 5
@@ -98,15 +85,15 @@
         pass_history = True
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
         self.add_to_conversation(prompt, role, convo_id=convo_id)
         # self.__truncate_conversation(convo_id=convo_id)
         # print(self.conversation[convo_id])
 
-        url = self.chat_url
+        url = self.api_url
         headers = {
             "Authorization": f"Bearer {kwargs.get('GROQ_API_KEY', self.api_key)}",
             "Content-Type": "application/json",
         }
 
         json_post = {
             "messages": self.conversation[convo_id] if pass_history else [{
@@ -170,10 +157,8 @@
                 continue
             if "role" in delta:
                 response_role = delta["role"]
             if "content" in delta and delta["content"]:
                 content = delta["content"]
                 full_response += content
                 yield content
-        self.add_to_conversation(full_response, response_role, convo_id=convo_id)
-        # print(repr(self.conversation.Conversation(convo_id)))
-        # print("total tokens:", self.get_token_count(convo_id))
+        self.add_to_conversation(full_response, response_role, convo_id=convo_id)
```

### Comparing `modelmerge-0.2.4/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.2.5/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.4/src/ModelMerge/tools/function_call.py` & `modelmerge-0.2.5/src/ModelMerge/tools/function_call.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 }
             },
             "required": [
                 "location"
             ]
         }
     },
-    "SEARCH_USE_GPT": {
+    "SEARCH": {
         "name": "get_search_results",
         "description": "Search Google to enhance knowledge.",
         "parameters": {
             "type": "object",
             "properties": {
                 "prompt": {
                     "type": "string",
```

### Comparing `modelmerge-0.2.4/src/ModelMerge/utils/prompt.py` & `modelmerge-0.2.5/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.4/src/ModelMerge/utils/scripts.py` & `modelmerge-0.2.5/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.4/src/ModelMerge.egg-info/SOURCES.txt` & `modelmerge-0.2.5/src/ModelMerge.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 setup.py
 src/ModelMerge/__init__.py
-src/ModelMerge/config.py
 src/ModelMerge.egg-info/PKG-INFO
 src/ModelMerge.egg-info/SOURCES.txt
 src/ModelMerge.egg-info/dependency_links.txt
 src/ModelMerge.egg-info/requires.txt
 src/ModelMerge.egg-info/top_level.txt
 src/ModelMerge/models/__init__.py
 src/ModelMerge/models/chatgpt.py
```

