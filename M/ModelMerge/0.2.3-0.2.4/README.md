# Comparing `tmp/modelmerge-0.2.3.tar.gz` & `tmp/modelmerge-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.2.3.tar", last modified: Thu May  9 15:28:08 2024, max compression
+gzip compressed data, was "modelmerge-0.2.4.tar", last modified: Thu May  9 16:41:33 2024, max compression
```

## Comparing `modelmerge-0.2.3.tar` & `modelmerge-0.2.4.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.394852 modelmerge-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 15:27:56.000000 modelmerge-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 15:28:08.394852 modelmerge-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 15:27:56.000000 modelmerge-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:28:08.394852 modelmerge-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 15:27:56.000000 modelmerge-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.386851 modelmerge-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.390852 modelmerge-0.2.3/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.390852 modelmerge-0.2.3/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28358 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.394852 modelmerge-0.2.3/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/plugins/travel.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.394852 modelmerge-0.2.3/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.394852 modelmerge-0.2.3/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.394852 modelmerge-0.2.3/src/ModelMerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 15:28:08.000000 modelmerge-0.2.3/src/ModelMerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-09 15:28:08.000000 modelmerge-0.2.3/src/ModelMerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:28:08.000000 modelmerge-0.2.3/src/ModelMerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 15:28:08.000000 modelmerge-0.2.3/src/ModelMerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 15:28:08.000000 modelmerge-0.2.3/src/ModelMerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.959859 modelmerge-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 16:41:24.000000 modelmerge-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 16:41:33.959859 modelmerge-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 16:41:24.000000 modelmerge-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 16:41:33.959859 modelmerge-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 16:41:24.000000 modelmerge-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.955859 modelmerge-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.955859 modelmerge-0.2.4/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.959859 modelmerge-0.2.4/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30068 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.959859 modelmerge-0.2.4/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/plugins/travel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.959859 modelmerge-0.2.4/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.959859 modelmerge-0.2.4/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-09 16:41:24.000000 modelmerge-0.2.4/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:41:33.959859 modelmerge-0.2.4/src/ModelMerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 16:41:33.000000 modelmerge-0.2.4/src/ModelMerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 16:41:33.000000 modelmerge-0.2.4/src/ModelMerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:41:33.000000 modelmerge-0.2.4/src/ModelMerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 16:41:33.000000 modelmerge-0.2.4/src/ModelMerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 16:41:33.000000 modelmerge-0.2.4/src/ModelMerge.egg-info/top_level.txt
```

### Comparing `modelmerge-0.2.3/LICENSE` & `modelmerge-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.3/src/ModelMerge/config.py` & `modelmerge-0.2.4/src/ModelMerge/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.3/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.2.4/src/ModelMerge/models/chatgpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -410,14 +410,15 @@
             if self.function_calls_counter[function_call_name] <= self.function_call_max_loop:
                 function_call_max_tokens = self.truncate_limit - message_token["total"] - 1000
                 if function_call_max_tokens <= 0:
                     function_call_max_tokens = int(self.truncate_limit / 2)
                 print("\033[32m function_call", function_call_name, "max token:", function_call_max_tokens, "\033[0m")
                 if function_call_name == "get_search_results":
                     prompt = json.loads(function_full_response)["prompt"]
+                    yield "🌐 正在搜索您的问题，提取关键词..."
                     llm = BaseLLM(api_key=self.api_key, api_url=self.api_url.source_api_url , engine=self.engine, system_prompt=self.system_prompt)
                     keywords = llm.ask(search_key_word_prompt.format(source=prompt)).split("\n")
                     function_response = yield from eval(function_call_name)(prompt, keywords)
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                     function_response = (
                         f"You need to response the following question: {prompt}. Search results is provided inside <Search_results></Search_results> XML tags. Your task is to think about the question step by step and then answer the above question in {LANGUAGE} based on the Search results provided. Please response in {LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive. Directly response markdown format, without using markdown code blocks"
                         "Here is the Search results, inside <Search_results></Search_results> XML tags:"
@@ -652,8 +653,57 @@
                     cookies=self.session.cookies,
                     headers=self.session.headers,
                 )
             if "session" in keys:
                 keys.remove("session")
             if "aclient" in keys:
                 keys.remove("aclient")
-            self.__dict__.update({key: loaded_config[key] for key in keys})
+            self.__dict__.update({key: loaded_config[key] for key in keys})
+
+class Imagebot(BaseLLM):
+    def __init__(
+        self,
+        api_key: str,
+        api_url: str = (os.environ.get("API_URL") or "https://api.openai.com/v1/chat/completions"),
+        timeout: float = 20,
+    ):
+        super().__init__(api_key, api_url=api_url, timeout=timeout)
+        self.engine: str = "dall-e-3"
+
+    def dall_e_3(
+        self,
+        prompt: str,
+        model: str = None,
+        **kwargs,
+    ):
+        url = self.api_url.image_url
+        headers = {"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"}
+
+        json_post = {
+                "model": os.environ.get("IMAGE_MODEL_NAME") or model or self.engine,
+                "prompt": prompt,
+                "n": 1,
+                "size": "1024x1024",
+        }
+        try:
+            response = self.session.post(
+                url,
+                headers=headers,
+                json=json_post,
+                timeout=kwargs.get("timeout", self.timeout),
+                stream=True,
+            )
+        except ConnectionError:
+            print("连接错误，请检查服务器状态或网络连接。")
+            return
+        except requests.exceptions.ReadTimeout:
+            print("请求超时，请检查网络连接或增加超时时间。{e}")
+            return
+        except Exception as e:
+            print(f"发生了未预料的错误: {e}")
+            return
+
+        if response.status_code != 200:
+            raise Exception(f"{response.status_code} {response.reason} {response.text}")
+        json_data = json.loads(response.text)
+        url = json_data["data"][0]["url"]
+        yield url
```

### Comparing `modelmerge-0.2.3/src/ModelMerge/models/claude.py` & `modelmerge-0.2.4/src/ModelMerge/models/claude.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-from tools import claude_tools_list
+from ..tools.function_call import claude_tools_list
+import os
+import json
+import tiktoken
+import requests
+
+from .config import BaseLLM, ENGINES
 
 class claudeConversation(dict):
     def Conversation(self, index):
         conversation_list = super().__getitem__(index)
         return "\n\n" + "\n\n".join([f"{item['role']}:{item['content']}" for item in conversation_list]) + "\n\nAssistant:"
 
-class claudebot:
+class claude(BaseLLM):
     def __init__(
         self,
         api_key: str,
         engine: str = os.environ.get("GPT_ENGINE") or "claude-2.1",
+        api_url: str = "https://api.anthropic.com/v1/complete",
+        system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
         temperature: float = 0.5,
         top_p: float = 0.7,
-        chat_url: str = "https://api.anthropic.com/v1/complete",
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
+        super().__init__(api_key, engine, api_url, system_prompt, timeout=timeout, temperature=temperature, top_p=top_p)
+        self.api_url = api_url
         self.conversation = claudeConversation()
-        self.system_prompt = system_prompt
 
     def add_to_conversation(
         self,
         message: str,
         role: str,
         convo_id: str = "default",
         pass_history: bool = True,
@@ -42,15 +41,15 @@
             self.reset(convo_id=convo_id)
         self.conversation[convo_id].append({"role": role, "content": message})
 
     def reset(self, convo_id: str = "default", system_prompt: str = None) -> None:
         """
         Reset the conversation
         """
-        self.conversation[convo_id] = list()
+        self.conversation[convo_id] = claudeConversation()
 
     def __truncate_conversation(self, convo_id: str = "default") -> None:
         """
         Truncate the conversation
         """
         while True:
             if (
@@ -98,15 +97,15 @@
         pass_history = True
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
         self.add_to_conversation(prompt, role, convo_id=convo_id)
         # self.__truncate_conversation(convo_id=convo_id)
         # print(self.conversation[convo_id])
 
-        url = self.chat_url
+        url = self.api_url
         headers = {
             "accept": "application/json",
             "anthropic-version": "2023-06-01",
             "content-type": "application/json",
             "x-api-key": f"{kwargs.get('api_key', self.api_key)}",
         }
 
@@ -149,55 +148,45 @@
             # print(line)
             resp: dict = json.loads(line)
             content = resp.get("completion")
             if content:
                 full_response += content
                 yield content
         self.add_to_conversation(full_response, response_role, convo_id=convo_id)
-        # print(repr(self.conversation.Conversation(convo_id)))
-        # print("total tokens:", self.get_token_count(convo_id))
 
-class claude3bot:
+class claude3(BaseLLM):
     def __init__(
         self,
         api_key: str,
         engine: str = os.environ.get("GPT_ENGINE") or "claude-3-opus-20240229",
+        api_url: str = "https://api.anthropic.com/v1/messages",
+        system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
         temperature: float = 0.5,
-        top_p: float = 0.7,
-        chat_url: str = "https://api.anthropic.com/v1/messages",
         timeout: float = 20,
-        system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
-        **kwargs,
+        top_p: float = 0.7,
     ):
-        self.api_key: str = api_key
-        self.engine: str = engine
-        self.temperature = temperature
-        self.top_p = top_p
-        self.chat_url = chat_url
-        self.timeout = timeout
-        self.session = requests.Session()
+        super().__init__(api_key, engine, api_url, system_prompt, timeout=timeout, temperature=temperature, top_p=top_p)
+        self.api_url = api_url
         self.conversation: dict[str, list[dict]] = {
             "default": [],
         }
-        self.system_prompt = system_prompt
 
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
 
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
-        # print("message", message)
         self.conversation[convo_id].append({"role": role, "content": message})
         index = len(self.conversation[convo_id]) - 2
         if index >= 0 and self.conversation[convo_id][index]["role"] == self.conversation[convo_id][index + 1]["role"]:
             self.conversation[convo_id][index]["content"] += self.conversation[convo_id][index + 1]["content"]
             self.conversation[convo_id].pop(index + 1)
 
     def reset(self, convo_id: str = "default", system_prompt: str = None) -> None:
@@ -256,15 +245,15 @@
         pass_history = True
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
         self.add_to_conversation(prompt, role, convo_id=convo_id)
         # self.__truncate_conversation(convo_id=convo_id)
         # print(self.conversation[convo_id])
 
-        url = self.chat_url
+        url = self.api_url
         headers = {
             "x-api-key": f"{kwargs.get('api_key', self.api_key)}",
             "anthropic-version": "2023-06-01",
             "content-type": "application/json",
             # "anthropic-beta": "tools-2024-04-04"
         }
 
@@ -321,10 +310,8 @@
             delta = resp.get("delta")
             if not delta:
                 continue
             if "text" in delta:
                 content = delta["text"]
                 full_response += content
                 yield content
-        self.add_to_conversation(full_response, response_role, convo_id=convo_id)
-        # print(repr(self.conversation.Conversation(convo_id)))
-        # print("total tokens:", self.get_token_count(convo_id))
+        self.add_to_conversation(full_response, response_role, convo_id=convo_id)
```

### Comparing `modelmerge-0.2.3/src/ModelMerge/models/config.py` & `modelmerge-0.2.4/src/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.3/src/ModelMerge/models/genimi.py` & `modelmerge-0.2.4/src/ModelMerge/models/groq.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-class gemini_bot:
+class groqbot:
     def __init__(
         self,
         api_key: str,
-        engine: str = os.environ.get("GPT_ENGINE") or "gemini-1.5-pro-latest",
+        engine: str = os.environ.get("GPT_ENGINE") or "llama3-70b-8192",
         temperature: float = 0.5,
-        top_p: float = 0.7,
-        chat_url: str = "https://generativelanguage.googleapis.com/v1beta/models/{model}:{stream}?key={api_key}",
+        top_p: float = 1,
+        chat_url: str = "https://api.groq.com/openai/v1/chat/completions",
         timeout: float = 20,
         system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
         **kwargs,
     ):
         self.api_key: str = api_key
         self.engine: str = engine
         self.temperature = temperature
         self.top_p = top_p
         self.chat_url = chat_url
         self.timeout = timeout
         self.session = requests.Session()
         self.conversation: dict[str, list[dict]] = {
-            "default": [],
+            "default": [
+                {
+                    "role": "system",
+                    "content": system_prompt,
+                },
+            ],
         }
         self.system_prompt = system_prompt
 
     def add_to_conversation(
         self,
         message: str,
         role: str,
@@ -31,20 +36,15 @@
     ) -> None:
         """
         Add a message to the conversation
         """
 
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
-        # print("message", message)
-        self.conversation[convo_id].append({"role": role, "parts": [{"text": message}]})
-        # index = len(self.conversation[convo_id]) - 2
-        # if index >= 0 and self.conversation[convo_id][index]["role"] == self.conversation[convo_id][index + 1]["role"]:
-        #     self.conversation[convo_id][index]["content"] += self.conversation[convo_id][index + 1]["content"]
-        #     self.conversation[convo_id].pop(index + 1)
+        self.conversation[convo_id].append({"role": role, "content": message})
 
     def reset(self, convo_id: str = "default", system_prompt: str = None) -> None:
         """
         Reset the conversation
         """
         self.conversation[convo_id] = list()
 
@@ -66,14 +66,15 @@
         """
         Get token count
         """
         if self.engine not in ENGINES:
             raise NotImplementedError(
                 f"Engine {self.engine} is not supported. Select from {ENGINES}",
             )
+        # tiktoken.model.MODEL_TO_ENCODING["mixtral-8x7b-32768"] = "cl100k_base"
         encoding = tiktoken.get_encoding("cl100k_base")
 
         num_tokens = 0
         for message in self.conversation[convo_id]:
             # every message follows <im_start>{role/name}\n{content}<im_end>\n
             num_tokens += 5
             for key, value in message.items():
@@ -87,55 +88,44 @@
     def ask_stream(
         self,
         prompt: str,
         role: str = "user",
         convo_id: str = "default",
         model: str = None,
         pass_history: bool = True,
-        model_max_tokens: int = 4096,
+        model_max_tokens: int = 1024,
         **kwargs,
     ):
         pass_history = True
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
         self.add_to_conversation(prompt, role, convo_id=convo_id)
         # self.__truncate_conversation(convo_id=convo_id)
         # print(self.conversation[convo_id])
 
+        url = self.chat_url
         headers = {
+            "Authorization": f"Bearer {kwargs.get('GROQ_API_KEY', self.api_key)}",
             "Content-Type": "application/json",
         }
 
         json_post = {
-            "contents": self.conversation[convo_id] if pass_history else [{
+            "messages": self.conversation[convo_id] if pass_history else [{
                 "role": "user",
                 "content": prompt
             }],
-            "safetySettings": [
-                {
-                    "category": "HARM_CATEGORY_HARASSMENT",
-                    "threshold": "BLOCK_NONE"
-                },
-                {
-                    "category": "HARM_CATEGORY_HATE_SPEECH",
-                    "threshold": "BLOCK_NONE"
-                },
-                {
-                    "category": "HARM_CATEGORY_SEXUALLY_EXPLICIT",
-                    "threshold": "BLOCK_NONE"
-                },
-                {
-                    "category": "HARM_CATEGORY_DANGEROUS_CONTENT",
-                    "threshold": "BLOCK_NONE"
-                }
-            ],
+            "model": model or self.engine,
+            "temperature": kwargs.get("temperature", self.temperature),
+            "max_tokens": model_max_tokens,
+            "top_p": kwargs.get("top_p", self.top_p),
+            "stop": None,
+            "stream": True,
         }
-        print(json.dumps(json_post, indent=4, ensure_ascii=False))
-
-        url = self.chat_url.format(model=model or self.engine, stream="streamGenerateContent", api_key=self.api_key)
+        # print("json_post", json_post)
+        # print(os.environ.get("GPT_ENGINE"), model, self.engine)
 
         try:
             response = self.session.post(
                 url,
                 headers=headers,
                 json=json_post,
                 timeout=kwargs.get("timeout", self.timeout),
@@ -150,25 +140,40 @@
         except Exception as e:
             print(f"发生了未预料的错误: {e}")
             return
 
         if response.status_code != 200:
             print(response.text)
             raise BaseException(f"{response.status_code} {response.reason} {response.text}")
-        response_role: str = "model"
+        response_role: str = "assistant"
         full_response: str = ""
-        try:
-            for line in response.iter_lines():
-                if not line:
-                    continue
-                line = line.decode("utf-8")
-                if line and '\"text\": \"' in line:
-                    content = line.split('\"text\": \"')[1][:-1]
-                    content = "\n".join(content.split("\\n"))
-                    full_response += content
-                    yield content
-        except requests.exceptions.ChunkedEncodingError as e:
-            print("Chunked Encoding Error occurred:", e)
-        except Exception as e:
-            print("An error occurred:", e)
-
-        self.add_to_conversation(full_response, response_role, convo_id=convo_id)
+        for line in response.iter_lines():
+            if not line:
+                continue
+            # Remove "data: "
+            # print(line.decode("utf-8"))
+            if line.decode("utf-8")[:6] == "data: ":
+                line = line.decode("utf-8")[6:]
+            else:
+                print(line.decode("utf-8"))
+                full_response = json.loads(line.decode("utf-8"))["choices"][0]["message"]["content"]
+                yield full_response
+                break
+            if line == "[DONE]":
+                break
+            resp: dict = json.loads(line)
+            # print("resp", resp)
+            choices = resp.get("choices")
+            if not choices:
+                continue
+            delta = choices[0].get("delta")
+            if not delta:
+                continue
+            if "role" in delta:
+                response_role = delta["role"]
+            if "content" in delta and delta["content"]:
+                content = delta["content"]
+                full_response += content
+                yield content
+        self.add_to_conversation(full_response, response_role, convo_id=convo_id)
+        # print(repr(self.conversation.Conversation(convo_id)))
+        # print("total tokens:", self.get_token_count(convo_id))
```

### Comparing `modelmerge-0.2.3/src/ModelMerge/models/groq.py` & `modelmerge-0.2.4/src/ModelMerge/models/genimi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,46 @@
-class groqbot:
+import os
+import json
+import requests
+import tiktoken
+
+from .config import BaseLLM, ENGINES
+
+class gemini(BaseLLM):
     def __init__(
         self,
         api_key: str,
-        engine: str = os.environ.get("GPT_ENGINE") or "llama3-70b-8192",
+        engine: str = os.environ.get("GPT_ENGINE") or "gemini-1.5-pro-latest",
+        api_url: str = "https://generativelanguage.googleapis.com/v1beta/models/{model}:{stream}?key={api_key}",
+        system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
         temperature: float = 0.5,
-        top_p: float = 1,
-        chat_url: str = "https://api.groq.com/openai/v1/chat/completions",
+        top_p: float = 0.7,
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
+        super().__init__(api_key, engine, system_prompt=system_prompt, timeout=timeout, temperature=temperature, top_p=top_p)
+        self.api_url = api_url
         self.conversation: dict[str, list[dict]] = {
-            "default": [
-                {
-                    "role": "system",
-                    "content": system_prompt,
-                },
-            ],
+            "default": [],
         }
-        self.system_prompt = system_prompt
 
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
 
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
-        self.conversation[convo_id].append({"role": role, "content": message})
+        # print("message", message)
+        self.conversation[convo_id].append({"role": role, "parts": [{"text": message}]})
 
     def reset(self, convo_id: str = "default", system_prompt: str = None) -> None:
         """
         Reset the conversation
         """
         self.conversation[convo_id] = list()
 
@@ -66,15 +62,14 @@
         """
         Get token count
         """
         if self.engine not in ENGINES:
             raise NotImplementedError(
                 f"Engine {self.engine} is not supported. Select from {ENGINES}",
             )
-        # tiktoken.model.MODEL_TO_ENCODING["mixtral-8x7b-32768"] = "cl100k_base"
         encoding = tiktoken.get_encoding("cl100k_base")
 
         num_tokens = 0
         for message in self.conversation[convo_id]:
             # every message follows <im_start>{role/name}\n{content}<im_end>\n
             num_tokens += 5
             for key, value in message.items():
@@ -88,44 +83,55 @@
     def ask_stream(
         self,
         prompt: str,
         role: str = "user",
         convo_id: str = "default",
         model: str = None,
         pass_history: bool = True,
-        model_max_tokens: int = 1024,
+        model_max_tokens: int = 4096,
         **kwargs,
     ):
         pass_history = True
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
         self.add_to_conversation(prompt, role, convo_id=convo_id)
         # self.__truncate_conversation(convo_id=convo_id)
         # print(self.conversation[convo_id])
 
-        url = self.chat_url
         headers = {
-            "Authorization": f"Bearer {kwargs.get('GROQ_API_KEY', self.api_key)}",
             "Content-Type": "application/json",
         }
 
         json_post = {
-            "messages": self.conversation[convo_id] if pass_history else [{
+            "contents": self.conversation[convo_id] if pass_history else [{
                 "role": "user",
                 "content": prompt
             }],
-            "model": model or self.engine,
-            "temperature": kwargs.get("temperature", self.temperature),
-            "max_tokens": model_max_tokens,
-            "top_p": kwargs.get("top_p", self.top_p),
-            "stop": None,
-            "stream": True,
+            "safetySettings": [
+                {
+                    "category": "HARM_CATEGORY_HARASSMENT",
+                    "threshold": "BLOCK_NONE"
+                },
+                {
+                    "category": "HARM_CATEGORY_HATE_SPEECH",
+                    "threshold": "BLOCK_NONE"
+                },
+                {
+                    "category": "HARM_CATEGORY_SEXUALLY_EXPLICIT",
+                    "threshold": "BLOCK_NONE"
+                },
+                {
+                    "category": "HARM_CATEGORY_DANGEROUS_CONTENT",
+                    "threshold": "BLOCK_NONE"
+                }
+            ],
         }
-        # print("json_post", json_post)
-        # print(os.environ.get("GPT_ENGINE"), model, self.engine)
+        print(json.dumps(json_post, indent=4, ensure_ascii=False))
+
+        url = self.api_url.format(model=model or self.engine, stream="streamGenerateContent", api_key=self.api_key)
 
         try:
             response = self.session.post(
                 url,
                 headers=headers,
                 json=json_post,
                 timeout=kwargs.get("timeout", self.timeout),
@@ -140,40 +146,25 @@
         except Exception as e:
             print(f"发生了未预料的错误: {e}")
             return
 
         if response.status_code != 200:
             print(response.text)
             raise BaseException(f"{response.status_code} {response.reason} {response.text}")
-        response_role: str = "assistant"
+        response_role: str = "model"
         full_response: str = ""
-        for line in response.iter_lines():
-            if not line:
-                continue
-            # Remove "data: "
-            # print(line.decode("utf-8"))
-            if line.decode("utf-8")[:6] == "data: ":
-                line = line.decode("utf-8")[6:]
-            else:
-                print(line.decode("utf-8"))
-                full_response = json.loads(line.decode("utf-8"))["choices"][0]["message"]["content"]
-                yield full_response
-                break
-            if line == "[DONE]":
-                break
-            resp: dict = json.loads(line)
-            # print("resp", resp)
-            choices = resp.get("choices")
-            if not choices:
-                continue
-            delta = choices[0].get("delta")
-            if not delta:
-                continue
-            if "role" in delta:
-                response_role = delta["role"]
-            if "content" in delta and delta["content"]:
-                content = delta["content"]
-                full_response += content
-                yield content
-        self.add_to_conversation(full_response, response_role, convo_id=convo_id)
-        # print(repr(self.conversation.Conversation(convo_id)))
-        # print("total tokens:", self.get_token_count(convo_id))
+        try:
+            for line in response.iter_lines():
+                if not line:
+                    continue
+                line = line.decode("utf-8")
+                if line and '\"text\": \"' in line:
+                    content = line.split('\"text\": \"')[1][:-1]
+                    content = "\n".join(content.split("\\n"))
+                    full_response += content
+                    yield content
+        except requests.exceptions.ChunkedEncodingError as e:
+            print("Chunked Encoding Error occurred:", e)
+        except Exception as e:
+            print("An error occurred:", e)
+
+        self.add_to_conversation(full_response, response_role, convo_id=convo_id)
```

### Comparing `modelmerge-0.2.3/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.2.4/src/ModelMerge/plugins/websearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,30 +188,26 @@
         tmp = t.join()
         if tmp:
             url_result.append(tmp)
     return url_result
 
 def get_url_text_list(keywords, search_url_num):
     start_time = record_time.time()
-    yield "🌐 正在搜索您的问题，提取关键词..."
 
-    # url_set_list, url_pdf_set_list = get_search_url(prompt, chainllm)
     url_set_list, url_pdf_set_list = yield from get_search_url(keywords, search_url_num)
 
     yield "🌐 已找到一些有用的链接，正在获取详细内容..."
     threads = []
     for url in url_set_list:
         # url_search_thread = ThreadWithReturnValue(target=jina_ai_Web_crawler, args=(url,True,))
         url_search_thread = ThreadWithReturnValue(target=Web_crawler, args=(url,True,))
         url_search_thread.start()
         threads.append(url_search_thread)
 
     url_text_list = concat_url(threads)
-    # print("url_text_list", url_text_list)
-
 
     yield "🌐 快完成了✅，正在为您整理搜索结果..."
     end_time = record_time.time()
     run_time = end_time - start_time
     print("urls", url_set_list)
     print(f"搜索用时：{run_time}秒")
```

### Comparing `modelmerge-0.2.3/src/ModelMerge/tools/function_call.py` & `modelmerge-0.2.4/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.3/src/ModelMerge/utils/prompt.py` & `modelmerge-0.2.4/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.3/src/ModelMerge/utils/scripts.py` & `modelmerge-0.2.4/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.3/src/ModelMerge.egg-info/SOURCES.txt` & `modelmerge-0.2.4/src/ModelMerge.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 src/ModelMerge.egg-info/dependency_links.txt
 src/ModelMerge.egg-info/requires.txt
 src/ModelMerge.egg-info/top_level.txt
 src/ModelMerge/models/__init__.py
 src/ModelMerge/models/chatgpt.py
 src/ModelMerge/models/claude.py
 src/ModelMerge/models/config.py
-src/ModelMerge/models/dalle.py
 src/ModelMerge/models/genimi.py
 src/ModelMerge/models/groq.py
 src/ModelMerge/plugins/__init__.py
 src/ModelMerge/plugins/today.py
 src/ModelMerge/plugins/travel.py
 src/ModelMerge/plugins/version.py
 src/ModelMerge/plugins/websearch.py
```

