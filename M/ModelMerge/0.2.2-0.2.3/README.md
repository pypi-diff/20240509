# Comparing `tmp/modelmerge-0.2.2.tar.gz` & `tmp/modelmerge-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.2.2.tar", last modified: Wed May  8 20:17:48 2024, max compression
+gzip compressed data, was "modelmerge-0.2.3.tar", last modified: Thu May  9 15:28:08 2024, max compression
```

## Comparing `modelmerge-0.2.2.tar` & `modelmerge-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.244330 modelmerge-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 20:17:35.000000 modelmerge-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-08 20:17:48.244330 modelmerge-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 20:17:35.000000 modelmerge-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:17:48.244330 modelmerge-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 20:17:35.000000 modelmerge-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.236330 modelmerge-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.240330 modelmerge-0.2.2/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.240330 modelmerge-0.2.2/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28569 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.240330 modelmerge-0.2.2/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.244330 modelmerge-0.2.2/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18726 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/utils/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/utils/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.244330 modelmerge-0.2.2/src/ModelMerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-08 20:17:48.000000 modelmerge-0.2.2/src/ModelMerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-08 20:17:48.000000 modelmerge-0.2.2/src/ModelMerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:17:48.000000 modelmerge-0.2.2/src/ModelMerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-08 20:17:48.000000 modelmerge-0.2.2/src/ModelMerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 20:17:48.000000 modelmerge-0.2.2/src/ModelMerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.394852 modelmerge-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 15:27:56.000000 modelmerge-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 15:28:08.394852 modelmerge-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 15:27:56.000000 modelmerge-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:28:08.394852 modelmerge-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 15:27:56.000000 modelmerge-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.386851 modelmerge-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.390852 modelmerge-0.2.3/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.390852 modelmerge-0.2.3/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28358 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.394852 modelmerge-0.2.3/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/plugins/travel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.394852 modelmerge-0.2.3/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.394852 modelmerge-0.2.3/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-09 15:27:56.000000 modelmerge-0.2.3/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:28:08.394852 modelmerge-0.2.3/src/ModelMerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 15:28:08.000000 modelmerge-0.2.3/src/ModelMerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-09 15:28:08.000000 modelmerge-0.2.3/src/ModelMerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:28:08.000000 modelmerge-0.2.3/src/ModelMerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 15:28:08.000000 modelmerge-0.2.3/src/ModelMerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 15:28:08.000000 modelmerge-0.2.3/src/ModelMerge.egg-info/top_level.txt
```

### Comparing `modelmerge-0.2.2/LICENSE` & `modelmerge-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.2/src/ModelMerge/config.py` & `modelmerge-0.2.3/src/ModelMerge/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 
 WEB_HOOK = os.environ.get('WEB_HOOK', None)
 BOT_TOKEN = os.environ.get('BOT_TOKEN', None)
 PORT = int(os.environ.get('PORT', '8080'))
 NICK = os.environ.get('NICK', None)
 API = os.environ.get('API', None)
 PASS_HISTORY = (os.environ.get('PASS_HISTORY', "False") == "False") == False
-USE_GOOGLE = (os.environ.get('USE_GOOGLE', "True") == "False") == False
-if os.environ.get('GOOGLE_API_KEY', None) == None and os.environ.get('GOOGLE_CSE_ID', None) == None:
-    USE_GOOGLE = False
+
 temperature = float(os.environ.get('temperature', '0.5'))
 GPT_ENGINE = os.environ.get('GPT_ENGINE', 'gpt-4-turbo-2024-04-09')
 # DEFAULT_SEARCH_MODEL = os.environ.get('DEFAULT_SEARCH_MODEL', 'gpt-3.5-turbo-1106') gpt-3.5-turbo-16k
 API_URL = os.environ.get('API_URL', 'https://api.openai.com/v1/chat/completions')
 # PDF_EMBEDDING = (os.environ.get('PDF_EMBEDDING', "True") == "False") == False
 LANGUAGE = os.environ.get('LANGUAGE', 'Simplified Chinese')
 GROQ_API_KEY = os.environ.get('GROQ_API_KEY', None)
```

### Comparing `modelmerge-0.2.2/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.2.3/src/ModelMerge/models/chatgpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 from .config import BaseLLM, ENGINES, CUSTOM_MODELS, PLUGINS, LANGUAGE
 
 import httpx
 import requests
 import tiktoken
 
 # import config
-from ..utils.plugins import check_json, Web_crawler, cut_message, get_search_results
+from ..utils.scripts import check_json, cut_message
+from ..utils.prompt import search_key_word_prompt
 from ..tools.function_call import function_call_list
+from ..plugins.websearch import Web_crawler, get_search_results
 
 def get_filtered_keys_from_object(obj: object, *keys: str) -> Set[str]:
     """
     Get filtered list of object variable names.
     :param keys: List of keys to include. If the first key is "not", the remaining keys will be removed from the class keys.
     :return: List of class keys.
     """
@@ -31,53 +33,39 @@
     if invalid_keys := set(keys) - class_keys:
         raise ValueError(
             f"Invalid keys: {invalid_keys}",
         )
     # Only return specified keys that are in class_keys
     return {key for key in keys if key in class_keys}
 
-class openaiAPI:
-    def __init__(
-        self,
-        api_url: str = (os.environ.get("API_URL") or "https://api.openai.com/v1/chat/completions"),
-    ):
-        from urllib.parse import urlparse, urlunparse
-        self.source_api_url: str = api_url
-        parsed_url = urlparse(self.source_api_url)
-        self.base_url: str = urlunparse(parsed_url[:2] + ("",) * 4)
-        self.v1_url: str = urlunparse(parsed_url[:2] + ("/v1",) + ("",) * 3)
-        self.chat_url: str = urlunparse(parsed_url[:2] + ("/v1/chat/completions",) + ("",) * 3)
-        self.image_url: str = urlunparse(parsed_url[:2] + ("/v1/images/generations",) + ("",) * 3)
-
-chatgpt_api_url = openaiAPI()
-
 class chatgpt(BaseLLM):
     """
     Official ChatGPT API
     """
 
     def __init__(
         self,
         api_key: str,
         engine: str = os.environ.get("GPT_ENGINE") or "gpt-3.5-turbo",
+        api_url: str = (os.environ.get("API_URL") or "https://api.openai.com/v1/chat/completions"),
+        system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
         proxy: str = None,
         timeout: float = 600,
         max_tokens: int = None,
         temperature: float = 0.5,
         top_p: float = 1.0,
         presence_penalty: float = 0.0,
         frequency_penalty: float = 0.0,
         reply_count: int = 1,
         truncate_limit: int = None,
-        system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
     ) -> None:
         """
         Initialize Chatbot with API key (from https://platform.openai.com/account/api-keys)
         """
-        super().__init__(api_key, engine, proxy, timeout, max_tokens, temperature, top_p, presence_penalty, frequency_penalty, reply_count, truncate_limit, system_prompt)
+        super().__init__(api_key, engine, api_url, system_prompt, proxy, timeout, max_tokens, temperature, top_p, presence_penalty, frequency_penalty, reply_count, truncate_limit)
         self.max_tokens: int = max_tokens or (
             4096
             if "gpt-4-1106-preview" in engine or "gpt-4-0125-preview" in engine or "gpt-4-turbo" in engine or "gpt-3.5-turbo-1106" in engine or "claude" in engine
             else 31000
             if "gpt-4-32k" in engine
             else 7000
             if "gpt-4" in engine
@@ -106,15 +94,15 @@
                 {
                     "role": "system",
                     "content": system_prompt,
                 },
             ],
         }
         self.function_calls_counter = {}
-        self.function_call_max_loop = 10
+        self.function_call_max_loop = 3
         # self.encode_web_text_list = []
 
         if self.get_token_count("default") > self.max_tokens:
             raise Exception("System prompt is too long")
 
     def add_to_conversation(
         self,
@@ -163,15 +151,15 @@
         **kwargs,
     ) -> None:
         """
         Truncate the conversation
         """
         while True:
             json_post = self.get_post_body(prompt, role, convo_id, model, pass_history, **kwargs)
-            url = chatgpt_api_url.chat_url
+            url = self.api_url.chat_url
             if "gpt-4" in self.engine or "claude" in self.engine or (CUSTOM_MODELS and self.engine in CUSTOM_MODELS):
                 message_token = {
                     "total": self.get_token_count(convo_id),
                 }
             else:
                 message_token = self.get_message_token(url, json_post)
             print("message_token", message_token, "truncate_limit", self.truncate_limit)
@@ -347,20 +335,18 @@
         elif self.engine == "gpt-3.5-turbo-1106":
             model_max_tokens = min(kwargs.get("max_tokens", self.max_tokens), 16385 - message_token["total"])
         else:
             model_max_tokens = min(kwargs.get("max_tokens", self.max_tokens), self.max_tokens - message_token["total"])
         print("model_max_tokens", model_max_tokens)
         json_post["max_tokens"] = model_max_tokens
 
-        url = chatgpt_api_url.chat_url
-        headers = {"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"}
         try:
             response = self.session.post(
-                url,
-                headers=headers,
+                self.api_url.chat_url,
+                headers={"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"},
                 json=json_post,
                 timeout=kwargs.get("timeout", self.timeout),
                 stream=True,
             )
         except ConnectionError:
             print("连接错误，请检查服务器状态或网络连接。")
             return
@@ -376,15 +362,15 @@
         full_response: str = ""
         function_full_response: str = ""
         function_call_name: str = ""
         need_function_call: bool = False
         for line in response.iter_lines():
             if not line:
                 continue
-            # Remove "data: "
+            # print("line", line.decode("utf-8"))
             if line.decode("utf-8")[:6] == "data: ":
                 line = line.decode("utf-8")[6:]
             else:
                 print(line.decode("utf-8"))
                 full_response = json.loads(line.decode("utf-8"))["choices"][0]["message"]["content"]
                 yield full_response
                 break
@@ -394,15 +380,15 @@
             # print("resp", resp)
             choices = resp.get("choices")
             if not choices:
                 continue
             delta = choices[0].get("delta")
             if not delta:
                 continue
-            if "role" in delta:
+            if "role" in delta and response_role == None:
                 response_role = delta["role"]
             if "content" in delta and delta["content"]:
                 need_function_call = False
                 content = delta["content"]
                 full_response += content
                 yield content
             if "function_call" in delta:
@@ -424,43 +410,45 @@
             if self.function_calls_counter[function_call_name] <= self.function_call_max_loop:
                 function_call_max_tokens = self.truncate_limit - message_token["total"] - 1000
                 if function_call_max_tokens <= 0:
                     function_call_max_tokens = int(self.truncate_limit / 2)
                 print("\033[32m function_call", function_call_name, "max token:", function_call_max_tokens, "\033[0m")
                 if function_call_name == "get_search_results":
                     prompt = json.loads(function_full_response)["prompt"]
-                    function_response = yield from eval(function_call_name)(prompt, chatgpt_api_url.v1_url)
-                    function_response, text_len = cut_message(function_response, function_call_max_tokens)
+                    llm = BaseLLM(api_key=self.api_key, api_url=self.api_url.source_api_url , engine=self.engine, system_prompt=self.system_prompt)
+                    keywords = llm.ask(search_key_word_prompt.format(source=prompt)).split("\n")
+                    function_response = yield from eval(function_call_name)(prompt, keywords)
+                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                     function_response = (
                         f"You need to response the following question: {prompt}. Search results is provided inside <Search_results></Search_results> XML tags. Your task is to think about the question step by step and then answer the above question in {LANGUAGE} based on the Search results provided. Please response in {LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive. Directly response markdown format, without using markdown code blocks"
                         "Here is the Search results, inside <Search_results></Search_results> XML tags:"
                         "<Search_results>"
                         "{}"
                         "</Search_results>"
                     ).format(function_response)
                     # user_prompt = f"You need to response the following question: {prompt}. Search results is provided inside <Search_results></Search_results> XML tags. Your task is to think about the question step by step and then answer the above question in {config.LANGUAGE} based on the Search results provided. Please response in {config.LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive. Directly response markdown format, without using markdown code blocks"
                     # self.add_to_conversation(user_prompt, "user", convo_id=convo_id)
                 if function_call_name == "get_url_content":
                     url = json.loads(function_full_response)["url"]
                     print("\n\nurl", url)
                     # function_response = jina_ai_Web_crawler(url)
                     function_response = Web_crawler(url)
-                    function_response, text_len = cut_message(function_response, function_call_max_tokens)
+                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                     function_response = (
                         "Here is the documentation, inside <document></document> XML tags:"
                         "<document>"
                         "{}"
                         "</document>"
                     ).format(function_response)
                 if function_call_name == "get_date_time_weekday":
                     function_response = eval(function_call_name)()
-                    function_response, text_len = cut_message(function_response, function_call_max_tokens)
+                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                 if function_call_name == "get_version_info":
                     function_response = eval(function_call_name)()
-                    function_response, text_len = cut_message(function_response, function_call_max_tokens)
+                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
             else:
                 function_response = "抱歉，直接告诉用户，无法找到相关信息"
             response_role = "function"
             # print(self.conversation[convo_id][-1])
             if self.conversation[convo_id][-1]["role"] == "function" and self.conversation[convo_id][-1]["name"] == "get_search_results":
                 mess = self.conversation[convo_id].pop(-1)
                 # print("Truncate message:", mess)
@@ -494,15 +482,15 @@
         if self.engine == "gpt-4-1106-preview" or "gpt-4-0125-preview" in self.engine or "gpt-4-turbo" in self.engine:
             model_max_tokens = kwargs.get("max_tokens", self.max_tokens)
         else:
             model_max_tokens = min(self.get_max_tokens(convo_id=convo_id) - 500, kwargs.get("max_tokens", self.max_tokens))
         # Get response
         async with self.aclient.stream(
             "post",
-            chatgpt_api_url.chat_url,
+            self.api_url.chat_url,
             headers={"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"},
             json={
                 "model": model or self.engine,
                 "messages": self.conversation[convo_id] if pass_history else [{"role": "system","content": self.system_prompt},{"role": role, "content": prompt}],
                 "stream": True,
                 # kwargs
                 "temperature": kwargs.get("temperature", self.temperature),
```

### Comparing `modelmerge-0.2.2/src/ModelMerge/models/claude.py` & `modelmerge-0.2.3/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.2/src/ModelMerge/models/dalle.py` & `modelmerge-0.2.3/src/ModelMerge/models/dalle.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.2/src/ModelMerge/models/genimi.py` & `modelmerge-0.2.3/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.2/src/ModelMerge/models/groq.py` & `modelmerge-0.2.3/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.2/src/ModelMerge/tools/function_call.py` & `modelmerge-0.2.3/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.2/src/ModelMerge/utils/plugins.py` & `modelmerge-0.2.3/src/ModelMerge/plugins/websearch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,19 @@
 import os
 import re
-import json
-import base64
 import datetime
-
-import sys
-sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-import config
-from utils.prompt import search_key_word_prompt
-# import jieba
-
-import asyncio
-import tiktoken
 import requests
 import threading
-
-import urllib.parse
 import time as record_time
 from bs4 import BeautifulSoup
+from duckduckgo_search import DDGS
+from googleapiclient.discovery import build
 
+from ..models import chatgpt
 
-from langchain.prompts import PromptTemplate
-from langchain.chat_models import ChatOpenAI
-from langchain.tools import DuckDuckGoSearchResults
-from langchain.chains import LLMChain
-
-# from typing import Optional, List
-# from langchain.llms.base import LLM
-# import g4f
-# class EducationalLLM(LLM):
-
-#     @property
-#     def _llm_type(self) -> str:
-#         return "custom"
-
-#     def _call(self, prompt: str, stop: Optional[List[str]] = None) -> str:
-#         out = g4f.ChatCompletion.create(
-#             model=config.GPT_ENGINE,
-#             messages=[{"role": "user", "content": prompt}],
-#         )  #
-#         if stop:
-#             stop_indexes = (out.find(s) for s in stop if s in out)
-#             min_stop = min(stop_indexes, default=-1)
-#             if min_stop > -1:
-#                 out = out[:min_stop]
-#         return out
 
 class ThreadWithReturnValue(threading.Thread):
     def run(self):
         if self._target is not None:
             self._return = self._target(*self._args, **self._kwargs)
 
     def join(self):
@@ -127,45 +92,43 @@
         print('\033[31m')
         print("error url", url)
         print("error", e)
         print('\033[0m')
     # print(result + "\n\n")
     return result
 
-def getddgsearchurl(result, numresults=4):
+def getddgsearchurl(query, max_results=4):
     try:
-        search = DuckDuckGoSearchResults(num_results=numresults)
-        webresult = search.run(result)
-        # print("ddgwebresult", webresult)
+        webresult = DDGS().text(query, max_results=max_results)
         if webresult == None:
             return []
-        urls = re.findall(r"(https?://\S+)\]", webresult, re.MULTILINE)
+        urls = [result['href'] for result in webresult]
     except Exception as e:
         print('\033[31m')
         print("duckduckgo error", e)
         print('\033[0m')
         urls = []
     # print("ddg urls", urls)
     return urls
 
-from googleapiclient.discovery import build
 def getgooglesearchurl(result, numresults=3):
     urls = []
+    if os.environ.get('GOOGLE_API_KEY', None) == None and os.environ.get('GOOGLE_CSE_ID', None) == None:
+        return urls
     try:
         service = build("customsearch", "v1", developerKey=os.environ.get('GOOGLE_API_KEY', None))
         res = service.cse().list(q=result, cx=os.environ.get('GOOGLE_CSE_ID', None)).execute()
         link_list = [item['link'] for item in res['items']]
         urls = link_list[:numresults]
     except Exception as e:
         print('\033[31m')
         print("error", e)
         print('\033[0m')
         if "rateLimitExceeded" in str(e):
             print("Google API 每日调用频率已达上限，请明日再试！")
-            config.USE_GOOGLE = False
     # print("google urls", urls)
     return urls
 
 def sort_by_time(urls):
     def extract_date(url):
         match = re.search(r'[12]\d{3}.\d{1,2}.\d{1,2}', url)
         if match is not None:
@@ -188,62 +151,29 @@
     date_url_pairs.sort(key=lambda x: x[0], reverse=True)
 
     # 获取排序后的URL列表
     sorted_urls = [url for _, url in date_url_pairs]
 
     return sorted_urls
 
-def get_search_url(prompt, chainllm):
-    urls_set = []
-
-    keyword_prompt = PromptTemplate(
-        input_variables=["source"],
-        template=search_key_word_prompt,
-    )
-    key_chain = LLMChain(llm=chainllm, prompt=keyword_prompt)
-    keyword_google_search_thread = ThreadWithReturnValue(target=key_chain.run, args=({"source": prompt},))
-    keyword_google_search_thread.start()
-    keywords = keyword_google_search_thread.join().split('\n')[-3:]
-    print("keywords", keywords)
-    keywords = [item.replace("三行关键词是：", "") for item in keywords if "\\x" not in item if item != ""]
-
-    keywords = [prompt] + keywords
-    keywords = keywords[:3]
-    # if len(keywords) == 1:
-    #     keywords = keywords * 3
-    print("select keywords", keywords)
-
-    # # seg_list = jieba.cut_for_search(prompt)  # 搜索引擎模式
-    # seg_list = jieba.cut(prompt, cut_all=True)
-    # result = " ".join(seg_list)
-    # keywords = [result] * 3
-    # print("keywords", keywords)
+def get_search_url(keywords, search_url_num):
+    yield "🌐 正在网上挑选最相关的信息源，请稍候..."
 
     search_threads = []
-    urls_set = []
-    if len(keywords) == 3:
-        search_url_num = 4
-    if len(keywords) == 2:
-        search_url_num = 6
-    if len(keywords) == 1:
-        search_url_num = 12
-    # print(keywords)
-    yield "🌐 正在网上挑选最相关的信息源，请稍候..."
-    if config.USE_GOOGLE:
-        search_thread = ThreadWithReturnValue(target=getgooglesearchurl, args=(keywords[0],search_url_num,))
-        search_thread.start()
-        search_threads.append(search_thread)
-        keywords.pop(0)
-    # print(keywords)
+    search_thread = ThreadWithReturnValue(target=getgooglesearchurl, args=(keywords[0],search_url_num,))
+    search_thread.start()
+    search_threads.append(search_thread)
+    keywords.pop(0)
+
     for keyword in keywords:
         search_thread = ThreadWithReturnValue(target=getddgsearchurl, args=(keyword,search_url_num,))
         search_thread.start()
         search_threads.append(search_thread)
-    # exit(0)
 
+    urls_set = []
     for t in search_threads:
         tmp = t.join()
         urls_set += tmp
     url_set_list = sorted(set(urls_set), key=lambda x: urls_set.index(x))
     url_set_list = sort_by_time(url_set_list)
 
     url_pdf_set_list = [item for item in url_set_list if item.endswith(".pdf")]
@@ -256,36 +186,20 @@
     url_result = []
     for t in threads:
         tmp = t.join()
         if tmp:
             url_result.append(tmp)
     return url_result
 
-def cut_message(message: str, max_tokens: int):
-    tiktoken.get_encoding("cl100k_base")
-    encoding = tiktoken.encoding_for_model(config.GPT_ENGINE)
-    encode_text = encoding.encode(message)
-    if len(encode_text) > max_tokens:
-        encode_text = encode_text[:max_tokens]
-        message = encoding.decode(encode_text)
-    encode_text = encoding.encode(message)
-    return message, len(encode_text)
-
-def get_url_text_list(prompt, chatgpt_api_url):
+def get_url_text_list(keywords, search_url_num):
     start_time = record_time.time()
     yield "🌐 正在搜索您的问题，提取关键词..."
 
-    # if config.PLUGINS["USE_G4F"]:
-    #     chainllm = EducationalLLM()
-    # else:
-    #     chainllm = ChatOpenAI(temperature=config.temperature, openai_api_base=config.bot_api_url.v1_url, model_name=config.GPT_ENGINE, openai_api_key=config.API)
-    chainllm = ChatOpenAI(temperature=config.temperature, openai_api_base=chatgpt_api_url, model_name=config.GPT_ENGINE, openai_api_key=config.API)
-
     # url_set_list, url_pdf_set_list = get_search_url(prompt, chainllm)
-    url_set_list, url_pdf_set_list = yield from get_search_url(prompt, chainllm)
+    url_set_list, url_pdf_set_list = yield from get_search_url(keywords, search_url_num)
 
     yield "🌐 已找到一些有用的链接，正在获取详细内容..."
     threads = []
     for url in url_set_list:
         # url_search_thread = ThreadWithReturnValue(target=jina_ai_Web_crawler, args=(url,True,))
         url_search_thread = ThreadWithReturnValue(target=Web_crawler, args=(url,True,))
         url_search_thread.start()
@@ -299,136 +213,37 @@
     end_time = record_time.time()
     run_time = end_time - start_time
     print("urls", url_set_list)
     print(f"搜索用时：{run_time}秒")
 
     return url_text_list
 
-# Plugins 搜索
-def get_search_results(prompt: str, chatgpt_api_url):
-
-    url_text_list = yield from get_url_text_list(prompt, chatgpt_api_url)
-    useful_source_text = "\n\n".join(url_text_list)
+# Plugins 搜索入口
+def get_search_results(prompt: str, keywords):
+    print("keywords", keywords)
+    keywords = [item.replace("三行关键词是：", "") for item in keywords if "\\x" not in item if item != ""]
+    keywords = [prompt] + keywords
+    keywords = keywords[:3]
+    print("select keywords", keywords)
 
-    # useful_source_text, search_tokens_len = cut_message(useful_source_text, context_max_tokens)
-    # print("search tokens len", search_tokens_len, "\n\n")
+    if len(keywords) == 3:
+        search_url_num = 4
+    if len(keywords) == 2:
+        search_url_num = 6
+    if len(keywords) == 1:
+        search_url_num = 12
 
+    url_text_list = yield from get_url_text_list(keywords, search_url_num)
+    useful_source_text = "\n\n".join(url_text_list)
     return useful_source_text
 
-# Plugins 获取日期时间
-def get_date_time_weekday():
-    import datetime
-    import pytz
-    tz = pytz.timezone('Asia/Shanghai')  # 为东八区设置时区
-    now = datetime.datetime.now(tz)  # 获取东八区当前时间
-    weekday = now.weekday()
-    weekday_str = ['星期一', '星期二', '星期三', '星期四', '星期五', '星期六', '星期日'][weekday]
-    return "今天是：" + str(now.date()) + "，现在的时间是：" + str(now.time())[:-7] + "，" + weekday_str
-
-# Plugins 使用函数
-def get_version_info():
-    import subprocess
-    current_directory = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-    result = subprocess.run(['git', '-C', current_directory, 'log', '-1'], stdout=subprocess.PIPE)
-    output = result.stdout.decode()
-    return output
-
-
-
-# 公用函数
-def encode_image(image_path):
-  with open(image_path, "rb") as image_file:
-    return base64.b64encode(image_file.read()).decode('utf-8')
-
-def get_doc_from_url(url):
-    filename = urllib.parse.unquote(url.split("/")[-1])
-    response = requests.get(url, stream=True)
-    with open(filename, 'wb') as f:
-        for chunk in response.iter_content(chunk_size=1024):
-            f.write(chunk)
-    return filename
-
-def get_encode_image(image_url):
-    filename = get_doc_from_url(image_url)
-    image_path = os.getcwd() + "/" + filename
-    base64_image = encode_image(image_path)
-    prompt = f"data:image/jpeg;base64,{base64_image}"
-    os.remove(image_path)
-    return prompt
-
-def get_text_token_len(text):
-    tiktoken.get_encoding("cl100k_base")
-    encoding = tiktoken.encoding_for_model(config.GPT_ENGINE)
-    encode_text = encoding.encode(text)
-    return len(encode_text)
-
-def Document_extract(docurl):
-    filename = get_doc_from_url(docurl)
-    docpath = os.getcwd() + "/" + filename
-    if filename[-3:] == "pdf":
-        from pdfminer.high_level import extract_text
-        text = extract_text(docpath)
-    if filename[-3:] == "txt":
-        with open(docpath, 'r') as f:
-            text = f.read()
-    prompt = (
-        "Here is the document, inside <document></document> XML tags:"
-        "<document>"
-        "{}"
-        "</document>"
-    ).format(text)
-    os.remove(docpath)
-    return prompt
-
-def check_json(json_data):
-    while True:
-        try:
-            json.loads(json_data)
-            break
-        except json.decoder.JSONDecodeError as e:
-            print("JSON error：", e)
-            print("JSON body", repr(json_data))
-            if "Invalid control character" in str(e):
-                json_data = json_data.replace("\n", "\\n")
-            if "Unterminated string starting" in str(e):
-                json_data += '"}'
-            if "Expecting ',' delimiter" in str(e):
-                json_data += '}'
-            if "Expecting value: line 1 column 1" in str(e):
-                json_data = '{"prompt": ' + json.dumps(json_data) + '}'
-    return json_data
-
-def is_surrounded_by_chinese(text, index):
-    left_char = text[index - 1]
-    if 0 < index < len(text) - 1:
-        right_char = text[index + 1]
-        return '\u4e00' <= left_char <= '\u9fff' or '\u4e00' <= right_char <= '\u9fff'
-    if index == len(text) - 1:
-        return '\u4e00' <= left_char <= '\u9fff'
-    return False
-
-def replace_char(string, index, new_char):
-    return string[:index] + new_char + string[index+1:]
-
-def claude_replace(text):
-    Punctuation_mapping = {",": "，", ":": "：", "!": "！", "?": "？", ";": "；"}
-    key_list = list(Punctuation_mapping.keys())
-    for i in range(len(text)):
-        if is_surrounded_by_chinese(text, i) and (text[i] in key_list):
-            text = replace_char(text, i, Punctuation_mapping[text[i]])
-    return text
-
 if __name__ == "__main__":
     os.system("clear")
-    print(get_date_time_weekday())
-    # print(get_version_info())
-    print(get_search_results("今天的微博热搜有哪些？", 1000))
-
-    # from langchain.agents import get_all_tool_names
-    # print(get_all_tool_names())
+    from ModelMerge.models import chatgpt
+    print(get_search_results("今天的微博热搜有哪些？", chatgpt.chatgpt_api_url.v1_url))
 
     # # 搜索
 
     # for i in search_web_and_summary("今天的微博热搜有哪些？"):
     # for i in search_web_and_summary("给出清华铊中毒案时间线，并作出你的评论。"):
     # for i in search_web_and_summary("红警hbk08是谁"):
     # for i in search_web_and_summary("国务院 2024 放假安排"):
```

### Comparing `modelmerge-0.2.2/src/ModelMerge/utils/prompt.py` & `modelmerge-0.2.3/src/ModelMerge/utils/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "意译\n\n"
     "{意译结果}"
     "现在请按照上面的要求翻译以下内容为简体中文："
 )
 
 search_key_word_prompt = (
     "根据我的问题，总结关键词概括问题，输出要求如下："
-    "1. 给出三行不同的关键词组合，每行的关键词用空格连接。每行关键词可以是一个或者多个。"
+    "1. 给出三行不同的关键词组合，每行的关键词用空格连接。每行关键词可以是一个或者多个。三行关键词用换行分开。"
     "2. 至少有一行关键词里面有中文，至少有一行关键词里面有英文。"
     "3. 只要直接给出这三行关键词，不需要其他任何解释，不要出现其他符号和内容。"
     "4. 如果问题有关于日漫，至少有一行关键词里面有日文。"
     "下面是一些根据问题提取关键词的示例："
     "问题 1：How much does the 'zeabur' software service cost per month? Is it free to use? Any limitations?"
     "三行关键词是："
     "zeabur price"
```

### Comparing `modelmerge-0.2.2/src/ModelMerge.egg-info/SOURCES.txt` & `modelmerge-0.2.3/src/ModelMerge.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -11,12 +11,17 @@
 src/ModelMerge/models/__init__.py
 src/ModelMerge/models/chatgpt.py
 src/ModelMerge/models/claude.py
 src/ModelMerge/models/config.py
 src/ModelMerge/models/dalle.py
 src/ModelMerge/models/genimi.py
 src/ModelMerge/models/groq.py
+src/ModelMerge/plugins/__init__.py
+src/ModelMerge/plugins/today.py
+src/ModelMerge/plugins/travel.py
+src/ModelMerge/plugins/version.py
+src/ModelMerge/plugins/websearch.py
 src/ModelMerge/tools/__init__.py
 src/ModelMerge/tools/function_call.py
 src/ModelMerge/utils/__init__.py
-src/ModelMerge/utils/plugins.py
-src/ModelMerge/utils/prompt.py
+src/ModelMerge/utils/prompt.py
+src/ModelMerge/utils/scripts.py
```

