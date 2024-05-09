# Comparing `tmp/totokenizers-1.2.3.tar.gz` & `tmp/totokenizers-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totokenizers-1.2.3.tar", last modified: Thu May  9 16:45:42 2024, max compression
+gzip compressed data, was "totokenizers-1.2.4.tar", last modified: Thu May  9 17:22:48 2024, max compression
```

## Comparing `totokenizers-1.2.3.tar` & `totokenizers-1.2.4.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:45:42.075300 totokenizers-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-09 16:45:42.075300 totokenizers-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-09 16:45:28.000000 totokenizers-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 16:45:42.075300 totokenizers-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-09 16:45:28.000000 totokenizers-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:45:42.067299 totokenizers-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-09 16:45:28.000000 totokenizers-1.2.3/tests/test_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-09 16:45:28.000000 totokenizers-1.2.3/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-09 16:45:28.000000 totokenizers-1.2.3/tests/test_jsonschema_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:45:42.071299 totokenizers-1.2.3/totokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:45:42.071299 totokenizers-1.2.3/totokenizers/anthropic/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/anthropic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/anthropic/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/anthropic/info.py
--rw-r--r--   0 runner    (1001) docker     (127)  1774213 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/anthropic/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/jsonschema_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:45:42.075300 totokenizers-1.2.3/totokenizers/mockai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/mockai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/mockai/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/mockai/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/model_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/openai_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-09 16:45:28.000000 totokenizers-1.2.3/totokenizers/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:45:42.075300 totokenizers-1.2.3/totokenizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-09 16:45:42.000000 totokenizers-1.2.3/totokenizers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-09 16:45:42.000000 totokenizers-1.2.3/totokenizers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:45:42.000000 totokenizers-1.2.3/totokenizers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 16:45:42.000000 totokenizers-1.2.3/totokenizers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 16:45:42.000000 totokenizers-1.2.3/totokenizers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:45:41.000000 totokenizers-1.2.3/totokenizers.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:48.099187 totokenizers-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-09 17:22:48.099187 totokenizers-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-09 17:22:31.000000 totokenizers-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:22:48.099187 totokenizers-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-09 17:22:31.000000 totokenizers-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:48.091187 totokenizers-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-09 17:22:31.000000 totokenizers-1.2.4/tests/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-09 17:22:31.000000 totokenizers-1.2.4/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-09 17:22:31.000000 totokenizers-1.2.4/tests/test_jsonschema_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:48.095187 totokenizers-1.2.4/totokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:48.095187 totokenizers-1.2.4/totokenizers/anthropic/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/anthropic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/anthropic/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/anthropic/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1774213 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/anthropic/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:48.099187 totokenizers-1.2.4/totokenizers/google/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/google/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/jsonschema_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:48.099187 totokenizers-1.2.4/totokenizers/mockai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/mockai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/mockai/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/mockai/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/model_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/openai_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-09 17:22:31.000000 totokenizers-1.2.4/totokenizers/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:48.099187 totokenizers-1.2.4/totokenizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-09 17:22:48.000000 totokenizers-1.2.4/totokenizers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-09 17:22:48.000000 totokenizers-1.2.4/totokenizers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:22:48.000000 totokenizers-1.2.4/totokenizers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 17:22:48.000000 totokenizers-1.2.4/totokenizers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 17:22:48.000000 totokenizers-1.2.4/totokenizers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:22:47.000000 totokenizers-1.2.4/totokenizers.egg-info/zip-safe
```

### Comparing `totokenizers-1.2.3/PKG-INFO` & `totokenizers-1.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: totokenizers
-Version: 1.2.3
+Version: 1.2.4
 Summary: Text tokenizers.
 Home-page: https://github.com/TeiaLabs/totokenizers
 Author: TeiaLabs
 Author-email: contato@teialabs.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Requires-Dist: google-cloud-aiplatform
 Requires-Dist: tiktoken
 Requires-Dist: tokenizers
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # totokenizers
```

### Comparing `totokenizers-1.2.3/README.md` & `totokenizers-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/setup.py` & `totokenizers-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/tests/test_anthropic.py` & `totokenizers-1.2.4/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/tests/test_code.py` & `totokenizers-1.2.4/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/tests/test_jsonschema_formatter.py` & `totokenizers-1.2.4/tests/test_jsonschema_formatter.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/totokenizers/anthropic/anthropic.py` & `totokenizers-1.2.4/totokenizers/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/totokenizers/anthropic/info.py` & `totokenizers-1.2.4/totokenizers/anthropic/info.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,33 +5,35 @@
 Model knowledge cutoff (Anthropic only mentions "early 2023"):
 https://support.anthropic.com/en/articles/8114494-how-up-to-date-is-claude-s-training-data
 
 Context and generation token limits:
 https://docs.anthropic.com/claude/reference/input-and-output-sizes
 """
 
-from ..model_info import ChatModelInfo, EmbeddingModelInfo, TextModelInfo
+from ..model_info import ChatModelInfo
 
 ANTHROPIC_CHAT_MODELS = {
     info.name: info
     for info in [
         ChatModelInfo(
             completion_token_cost=0.024,
             cutoff="2023-01-01",
             max_tokens=204_096,
             name="claude-2.1",
             prompt_token_cost=0.008,
             feature_flags=False,
+            max_output_tokens=4096,
         ),
         ChatModelInfo(
             completion_token_cost=0.0024,
             cutoff="2023-01-01",
             max_tokens=104_096,
             name="claude-instant-1.2",
             prompt_token_cost=0.0008,
             feature_flags=False,
+            max_output_tokens=4096,
         ),
     ]
 }
 
 
 ANTHROPIC_MODELS: dict[str, ChatModelInfo] = {**ANTHROPIC_CHAT_MODELS}
```

### Comparing `totokenizers-1.2.3/totokenizers/anthropic/tokenizer.json` & `totokenizers-1.2.4/totokenizers/anthropic/tokenizer.json`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/totokenizers/errors.py` & `totokenizers-1.2.4/totokenizers/errors.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/totokenizers/factories.py` & `totokenizers-1.2.4/totokenizers/factories.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/totokenizers/jsonschema_formatter.py` & `totokenizers-1.2.4/totokenizers/jsonschema_formatter.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/totokenizers/mockai/info.py` & `totokenizers-1.2.4/totokenizers/mockai/info.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,22 @@
     for info in [
         ChatModelInfo(
             completion_token_cost=0,
             cutoff="1997-01-01",
             max_tokens=4096,
             name="always-func",
             prompt_token_cost=0,
+            max_output_tokens=-1,
         ),
         ChatModelInfo(
             completion_token_cost=0,
             cutoff="1997-01-01",
             max_tokens=4096,
             name="always-chat",
             prompt_token_cost=0,
             feature_flags=True,
+            max_output_tokens=-1,
         ),
     ]
 }
 
 MODELS: dict[str, ChatModelInfo] = {**CHAT_MODELS}
```

### Comparing `totokenizers-1.2.3/totokenizers/mockai/tokenizer.py` & `totokenizers-1.2.4/totokenizers/mockai/tokenizer.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/totokenizers/model_info.py` & `totokenizers-1.2.4/totokenizers/model_info.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/totokenizers/openai.py` & `totokenizers-1.2.4/totokenizers/openai.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/totokenizers/openai_info.py` & `totokenizers-1.2.4/totokenizers/openai_info.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/totokenizers/protocols.py` & `totokenizers-1.2.4/totokenizers/protocols.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/totokenizers/schemas.py` & `totokenizers-1.2.4/totokenizers/schemas.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.3/totokenizers.egg-info/PKG-INFO` & `totokenizers-1.2.4/totokenizers.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: totokenizers
-Version: 1.2.3
+Version: 1.2.4
 Summary: Text tokenizers.
 Home-page: https://github.com/TeiaLabs/totokenizers
 Author: TeiaLabs
 Author-email: contato@teialabs.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Requires-Dist: google-cloud-aiplatform
 Requires-Dist: tiktoken
 Requires-Dist: tokenizers
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # totokenizers
```

### Comparing `totokenizers-1.2.3/totokenizers.egg-info/SOURCES.txt` & `totokenizers-1.2.4/totokenizers.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,10 +18,12 @@
 totokenizers.egg-info/requires.txt
 totokenizers.egg-info/top_level.txt
 totokenizers.egg-info/zip-safe
 totokenizers/anthropic/__init__.py
 totokenizers/anthropic/anthropic.py
 totokenizers/anthropic/info.py
 totokenizers/anthropic/tokenizer.json
+totokenizers/google/__init__.py
+totokenizers/google/google.py
 totokenizers/mockai/__init__.py
 totokenizers/mockai/info.py
 totokenizers/mockai/tokenizer.py
```

