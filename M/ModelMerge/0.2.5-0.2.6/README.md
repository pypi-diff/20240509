# Comparing `tmp/modelmerge-0.2.5.tar.gz` & `tmp/modelmerge-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.2.5.tar", last modified: Thu May  9 17:08:31 2024, max compression
+gzip compressed data, was "modelmerge-0.2.6.tar", last modified: Thu May  9 18:10:59 2024, max compression
```

## Comparing `modelmerge-0.2.5.tar` & `modelmerge-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.546149 modelmerge-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 17:08:23.000000 modelmerge-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 17:08:31.546149 modelmerge-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 17:08:23.000000 modelmerge-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:08:31.546149 modelmerge-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 17:08:23.000000 modelmerge-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.542149 modelmerge-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.542149 modelmerge-0.2.5/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.546149 modelmerge-0.2.5/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29814 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.546149 modelmerge-0.2.5/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/plugins/travel.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.546149 modelmerge-0.2.5/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.546149 modelmerge-0.2.5/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-09 17:08:23.000000 modelmerge-0.2.5/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:08:31.546149 modelmerge-0.2.5/src/ModelMerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 17:08:31.000000 modelmerge-0.2.5/src/ModelMerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 17:08:31.000000 modelmerge-0.2.5/src/ModelMerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:08:31.000000 modelmerge-0.2.5/src/ModelMerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 17:08:31.000000 modelmerge-0.2.5/src/ModelMerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 17:08:31.000000 modelmerge-0.2.5/src/ModelMerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:59.061267 modelmerge-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 18:10:45.000000 modelmerge-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 18:10:59.061267 modelmerge-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 18:10:45.000000 modelmerge-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:10:59.061267 modelmerge-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 18:10:45.000000 modelmerge-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:59.053266 modelmerge-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:59.057266 modelmerge-0.2.6/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:59.057266 modelmerge-0.2.6/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29813 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:59.057266 modelmerge-0.2.6/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/plugins/travel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:59.057266 modelmerge-0.2.6/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:59.061267 modelmerge-0.2.6/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-09 18:10:45.000000 modelmerge-0.2.6/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:59.061267 modelmerge-0.2.6/src/ModelMerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 18:10:59.000000 modelmerge-0.2.6/src/ModelMerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-09 18:10:59.000000 modelmerge-0.2.6/src/ModelMerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:10:59.000000 modelmerge-0.2.6/src/ModelMerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 18:10:59.000000 modelmerge-0.2.6/src/ModelMerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 18:10:59.000000 modelmerge-0.2.6/src/ModelMerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:10:59.061267 modelmerge-0.2.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-09 18:10:45.000000 modelmerge-0.2.6/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 18:10:45.000000 modelmerge-0.2.6/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-09 18:10:45.000000 modelmerge-0.2.6/test/test_google_search.py
```

### Comparing `modelmerge-0.2.5/LICENSE` & `modelmerge-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.5/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.2.6/src/ModelMerge/models/chatgpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,14 @@
             model_max_tokens = kwargs.get("max_tokens", self.max_tokens)
         elif self.engine == "gpt-3.5-turbo-1106":
             model_max_tokens = min(kwargs.get("max_tokens", self.max_tokens), 16385 - message_token["total"])
         else:
             model_max_tokens = min(kwargs.get("max_tokens", self.max_tokens), self.max_tokens - message_token["total"])
         print("model_max_tokens", model_max_tokens)
         json_post["max_tokens"] = model_max_tokens
-
         try:
             response = self.session.post(
                 self.api_url.chat_url,
                 headers={"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"},
                 json=json_post,
                 timeout=kwargs.get("timeout", self.timeout),
                 stream=True,
```

### Comparing `modelmerge-0.2.5/src/ModelMerge/models/claude.py` & `modelmerge-0.2.6/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.5/src/ModelMerge/models/config.py` & `modelmerge-0.2.6/src/ModelMerge/models/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,19 @@
     def __init__(
         self,
         api_url: str = (os.environ.get("API_URL") or "https://api.openai.com/v1/chat/completions"),
     ):
         from urllib.parse import urlparse, urlunparse
         self.source_api_url: str = api_url
         parsed_url = urlparse(self.source_api_url)
-        self.base_url: str = urlunparse(parsed_url[:2] + ("",) * 4)
-        self.v1_url: str = urlunparse(parsed_url[:2] + ("/v1",) + ("",) * 3)
-        self.chat_url: str = urlunparse(parsed_url[:2] + ("/v1/chat/completions",) + ("",) * 3)
-        self.image_url: str = urlunparse(parsed_url[:2] + ("/v1/images/generations",) + ("",) * 3)
+        before_v1 = parsed_url.path.split("/v1")[0]
+        self.base_url: str = urlunparse(parsed_url[:2] + (before_v1,) + ("",) * 3)
+        self.v1_url: str = urlunparse(parsed_url[:2]+ (before_v1 + "/v1",) + ("",) * 3)
+        self.chat_url: str = urlunparse(parsed_url[:2] + (before_v1 + "/v1/chat/completions",) + ("",) * 3)
+        self.image_url: str = urlunparse(parsed_url[:2] + (before_v1 + "/v1/images/generations",) + ("",) * 3)
 
 class BaseLLM:
     def __init__(
         self,
         api_key: str,
         engine: str = os.environ.get("GPT_ENGINE") or "gpt-3.5-turbo",
         api_url: str = (os.environ.get("API_URL") or "https://api.openai.com/v1/chat/completions"),
```

### Comparing `modelmerge-0.2.5/src/ModelMerge/models/genimi.py` & `modelmerge-0.2.6/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.5/src/ModelMerge/models/groq.py` & `modelmerge-0.2.6/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.5/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.2.6/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.5/src/ModelMerge/tools/function_call.py` & `modelmerge-0.2.6/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.5/src/ModelMerge/utils/prompt.py` & `modelmerge-0.2.6/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.5/src/ModelMerge/utils/scripts.py` & `modelmerge-0.2.6/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.5/src/ModelMerge.egg-info/SOURCES.txt` & `modelmerge-0.2.6/src/ModelMerge.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -18,8 +18,11 @@
 src/ModelMerge/plugins/travel.py
 src/ModelMerge/plugins/version.py
 src/ModelMerge/plugins/websearch.py
 src/ModelMerge/tools/__init__.py
 src/ModelMerge/tools/function_call.py
 src/ModelMerge/utils/__init__.py
 src/ModelMerge/utils/prompt.py
-src/ModelMerge/utils/scripts.py
+src/ModelMerge/utils/scripts.py
+test/test.py
+test/test_ddg_search.py
+test/test_google_search.py
```

