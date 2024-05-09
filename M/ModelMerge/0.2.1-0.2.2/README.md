# Comparing `tmp/modelmerge-0.2.1.tar.gz` & `tmp/modelmerge-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.2.1.tar", last modified: Wed May  8 19:12:13 2024, max compression
+gzip compressed data, was "modelmerge-0.2.2.tar", last modified: Wed May  8 20:17:48 2024, max compression
```

## Comparing `modelmerge-0.2.1.tar` & `modelmerge-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.303237 modelmerge-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 19:12:04.000000 modelmerge-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 19:12:13.303237 modelmerge-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 19:12:04.000000 modelmerge-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:12:13.303237 modelmerge-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 19:12:04.000000 modelmerge-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.299237 modelmerge-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.299237 modelmerge-0.2.1/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.303237 modelmerge-0.2.1/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28525 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.303237 modelmerge-0.2.1/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.303237 modelmerge-0.2.1/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18685 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/utils/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/utils/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.303237 modelmerge-0.2.1/src/ModelMerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 19:12:13.000000 modelmerge-0.2.1/src/ModelMerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-08 19:12:13.000000 modelmerge-0.2.1/src/ModelMerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:12:13.000000 modelmerge-0.2.1/src/ModelMerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 19:12:13.000000 modelmerge-0.2.1/src/ModelMerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 19:12:13.000000 modelmerge-0.2.1/src/ModelMerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.244330 modelmerge-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 20:17:35.000000 modelmerge-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-08 20:17:48.244330 modelmerge-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 20:17:35.000000 modelmerge-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:17:48.244330 modelmerge-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 20:17:35.000000 modelmerge-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.236330 modelmerge-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.240330 modelmerge-0.2.2/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.240330 modelmerge-0.2.2/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28569 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.240330 modelmerge-0.2.2/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.244330 modelmerge-0.2.2/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18726 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/utils/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-08 20:17:35.000000 modelmerge-0.2.2/src/ModelMerge/utils/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:48.244330 modelmerge-0.2.2/src/ModelMerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-08 20:17:48.000000 modelmerge-0.2.2/src/ModelMerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-08 20:17:48.000000 modelmerge-0.2.2/src/ModelMerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:17:48.000000 modelmerge-0.2.2/src/ModelMerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-08 20:17:48.000000 modelmerge-0.2.2/src/ModelMerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 20:17:48.000000 modelmerge-0.2.2/src/ModelMerge.egg-info/top_level.txt
```

### Comparing `modelmerge-0.2.1/LICENSE` & `modelmerge-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.1/src/ModelMerge/config.py` & `modelmerge-0.2.2/src/ModelMerge/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.1/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.2.2/src/ModelMerge/models/chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .config import BaseLLM, ENGINES, CUSTOM_MODELS, PLUGINS, LANGUAGE
 
 import httpx
 import requests
 import tiktoken
 
 # import config
-from ..utils.plugins import check_json, Web_crawler, cut_message
+from ..utils.plugins import check_json, Web_crawler, cut_message, get_search_results
 from ..tools.function_call import function_call_list
 
 def get_filtered_keys_from_object(obj: object, *keys: str) -> Set[str]:
     """
     Get filtered list of object variable names.
     :param keys: List of keys to include. If the first key is "not", the remaining keys will be removed from the class keys.
     :return: List of class keys.
@@ -424,15 +424,15 @@
             if self.function_calls_counter[function_call_name] <= self.function_call_max_loop:
                 function_call_max_tokens = self.truncate_limit - message_token["total"] - 1000
                 if function_call_max_tokens <= 0:
                     function_call_max_tokens = int(self.truncate_limit / 2)
                 print("\033[32m function_call", function_call_name, "max token:", function_call_max_tokens, "\033[0m")
                 if function_call_name == "get_search_results":
                     prompt = json.loads(function_full_response)["prompt"]
-                    function_response = yield from eval(function_call_name)(prompt)
+                    function_response = yield from eval(function_call_name)(prompt, chatgpt_api_url.v1_url)
                     function_response, text_len = cut_message(function_response, function_call_max_tokens)
                     function_response = (
                         f"You need to response the following question: {prompt}. Search results is provided inside <Search_results></Search_results> XML tags. Your task is to think about the question step by step and then answer the above question in {LANGUAGE} based on the Search results provided. Please response in {LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive. Directly response markdown format, without using markdown code blocks"
                         "Here is the Search results, inside <Search_results></Search_results> XML tags:"
                         "<Search_results>"
                         "{}"
                         "</Search_results>"
```

### Comparing `modelmerge-0.2.1/src/ModelMerge/models/claude.py` & `modelmerge-0.2.2/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.1/src/ModelMerge/models/config.py` & `modelmerge-0.2.2/src/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.1/src/ModelMerge/models/dalle.py` & `modelmerge-0.2.2/src/ModelMerge/models/dalle.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.1/src/ModelMerge/models/genimi.py` & `modelmerge-0.2.2/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.1/src/ModelMerge/models/groq.py` & `modelmerge-0.2.2/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.1/src/ModelMerge/tools/function_call.py` & `modelmerge-0.2.2/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.1/src/ModelMerge/utils/plugins.py` & `modelmerge-0.2.2/src/ModelMerge/utils/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,23 +266,23 @@
     encode_text = encoding.encode(message)
     if len(encode_text) > max_tokens:
         encode_text = encode_text[:max_tokens]
         message = encoding.decode(encode_text)
     encode_text = encoding.encode(message)
     return message, len(encode_text)
 
-def get_url_text_list(prompt):
+def get_url_text_list(prompt, chatgpt_api_url):
     start_time = record_time.time()
     yield "🌐 正在搜索您的问题，提取关键词..."
 
     # if config.PLUGINS["USE_G4F"]:
     #     chainllm = EducationalLLM()
     # else:
     #     chainllm = ChatOpenAI(temperature=config.temperature, openai_api_base=config.bot_api_url.v1_url, model_name=config.GPT_ENGINE, openai_api_key=config.API)
-    chainllm = ChatOpenAI(temperature=config.temperature, openai_api_base=config.bot_api_url.v1_url, model_name=config.GPT_ENGINE, openai_api_key=config.API)
+    chainllm = ChatOpenAI(temperature=config.temperature, openai_api_base=chatgpt_api_url, model_name=config.GPT_ENGINE, openai_api_key=config.API)
 
     # url_set_list, url_pdf_set_list = get_search_url(prompt, chainllm)
     url_set_list, url_pdf_set_list = yield from get_search_url(prompt, chainllm)
 
     yield "🌐 已找到一些有用的链接，正在获取详细内容..."
     threads = []
     for url in url_set_list:
@@ -300,17 +300,17 @@
     run_time = end_time - start_time
     print("urls", url_set_list)
     print(f"搜索用时：{run_time}秒")
 
     return url_text_list
 
 # Plugins 搜索
-def get_search_results(prompt: str):
+def get_search_results(prompt: str, chatgpt_api_url):
 
-    url_text_list = yield from get_url_text_list(prompt)
+    url_text_list = yield from get_url_text_list(prompt, chatgpt_api_url)
     useful_source_text = "\n\n".join(url_text_list)
 
     # useful_source_text, search_tokens_len = cut_message(useful_source_text, context_max_tokens)
     # print("search tokens len", search_tokens_len, "\n\n")
 
     return useful_source_text
```

### Comparing `modelmerge-0.2.1/src/ModelMerge/utils/prompt.py` & `modelmerge-0.2.2/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.1/src/ModelMerge.egg-info/SOURCES.txt` & `modelmerge-0.2.2/src/ModelMerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

