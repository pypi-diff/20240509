# Comparing `tmp/llmprototyping-0.1.0.dev3.tar.gz` & `tmp/llmprototyping-0.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmprototyping-0.1.0.dev3.tar", last modified: Wed May  8 00:04:44 2024, max compression
+gzip compressed data, was "llmprototyping-0.1.0.dev4.tar", last modified: Thu May  9 11:09:13 2024, max compression
```

## Comparing `llmprototyping-0.1.0.dev3.tar` & `llmprototyping-0.1.0.dev4.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-08 00:04:44.514251 llmprototyping-0.1.0.dev3/
--rw-r--r--   0 alejandro   (501) staff       (20)    11357 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev3/LICENSE
--rw-r--r--   0 alejandro   (501) staff       (20)     4298 2024-05-08 00:04:44.514170 llmprototyping-0.1.0.dev3/PKG-INFO
--rw-r--r--   0 alejandro   (501) staff       (20)     3633 2024-05-08 00:03:45.000000 llmprototyping-0.1.0.dev3/README.md
--rw-r--r--   0 alejandro   (501) staff       (20)       74 2024-05-08 00:04:44.514649 llmprototyping-0.1.0.dev3/setup.cfg
--rw-r--r--   0 alejandro   (501) staff       (20)     1119 2024-05-08 00:04:28.000000 llmprototyping-0.1.0.dev3/setup.py
-drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-08 00:04:44.508994 llmprototyping-0.1.0.dev3/src/
-drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-08 00:04:44.512465 llmprototyping-0.1.0.dev3/src/llmprototyping/
--rw-r--r--   0 alejandro   (501) staff       (20)      543 2024-05-07 22:50:14.000000 llmprototyping-0.1.0.dev3/src/llmprototyping/__init__.py
--rw-r--r--   0 alejandro   (501) staff       (20)     1919 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev3/src/llmprototyping/embeddings_interface.py
--rw-r--r--   0 alejandro   (501) staff       (20)     3150 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev3/src/llmprototyping/embeddings_openai.py
--rw-r--r--   0 alejandro   (501) staff       (20)     1163 2024-05-07 22:50:21.000000 llmprototyping-0.1.0.dev3/src/llmprototyping/error.py
--rw-r--r--   0 alejandro   (501) staff       (20)     1348 2024-05-07 22:50:24.000000 llmprototyping-0.1.0.dev3/src/llmprototyping/factory.py
--rw-r--r--   0 alejandro   (501) staff       (20)     3256 2024-05-07 23:44:54.000000 llmprototyping-0.1.0.dev3/src/llmprototyping/llm_groq.py
--rw-r--r--   0 alejandro   (501) staff       (20)     2834 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev3/src/llmprototyping/llm_interface.py
--rw-r--r--   0 alejandro   (501) staff       (20)     3634 2024-05-07 22:50:31.000000 llmprototyping-0.1.0.dev3/src/llmprototyping/llm_openai.py
--rw-r--r--   0 alejandro   (501) staff       (20)      434 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev3/src/llmprototyping/serializable.py
--rw-r--r--   0 alejandro   (501) staff       (20)     1930 2024-05-07 22:50:32.000000 llmprototyping-0.1.0.dev3/src/llmprototyping/vectordb.py
-drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-08 00:04:44.513891 llmprototyping-0.1.0.dev3/src/llmprototyping.egg-info/
--rw-r--r--   0 alejandro   (501) staff       (20)     4298 2024-05-08 00:04:44.000000 llmprototyping-0.1.0.dev3/src/llmprototyping.egg-info/PKG-INFO
--rw-r--r--   0 alejandro   (501) staff       (20)      583 2024-05-08 00:04:44.000000 llmprototyping-0.1.0.dev3/src/llmprototyping.egg-info/SOURCES.txt
--rw-r--r--   0 alejandro   (501) staff       (20)        1 2024-05-08 00:04:44.000000 llmprototyping-0.1.0.dev3/src/llmprototyping.egg-info/dependency_links.txt
--rw-r--r--   0 alejandro   (501) staff       (20)       41 2024-05-08 00:04:44.000000 llmprototyping-0.1.0.dev3/src/llmprototyping.egg-info/requires.txt
--rw-r--r--   0 alejandro   (501) staff       (20)       15 2024-05-08 00:04:44.000000 llmprototyping-0.1.0.dev3/src/llmprototyping.egg-info/top_level.txt
+drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-09 11:09:13.027473 llmprototyping-0.1.0.dev4/
+-rw-r--r--   0 alejandro   (501) staff       (20)    11357 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev4/LICENSE
+-rw-r--r--   0 alejandro   (501) staff       (20)     8044 2024-05-09 11:09:13.027415 llmprototyping-0.1.0.dev4/PKG-INFO
+-rw-r--r--   0 alejandro   (501) staff       (20)     7326 2024-05-08 23:49:15.000000 llmprototyping-0.1.0.dev4/README.md
+-rw-r--r--   0 alejandro   (501) staff       (20)       74 2024-05-09 11:09:13.027665 llmprototyping-0.1.0.dev4/setup.cfg
+-rw-r--r--   0 alejandro   (501) staff       (20)     1152 2024-05-09 11:06:40.000000 llmprototyping-0.1.0.dev4/setup.py
+drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-09 11:09:13.024452 llmprototyping-0.1.0.dev4/src/
+drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-09 11:09:13.026377 llmprototyping-0.1.0.dev4/src/llmprototyping/
+-rw-r--r--   0 alejandro   (501) staff       (20)      777 2024-05-09 10:01:17.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/__init__.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1919 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/embeddings_interface.py
+-rw-r--r--   0 alejandro   (501) staff       (20)        0 2024-05-09 09:48:40.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/embeddings_ollama.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     3148 2024-05-09 10:49:51.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/embeddings_openai.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1159 2024-05-09 10:06:53.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/error.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1570 2024-05-09 10:44:25.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/factory.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     6457 2024-05-09 10:58:15.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/llm_em_ollama.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     3260 2024-05-08 23:25:51.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/llm_groq.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     2909 2024-05-08 23:38:17.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/llm_interface.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     3573 2024-05-08 23:28:38.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/llm_openai.py
+-rw-r--r--   0 alejandro   (501) staff       (20)      434 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/serializable.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1930 2024-05-07 22:50:32.000000 llmprototyping-0.1.0.dev4/src/llmprototyping/vectordb.py
+drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-09 11:09:13.027200 llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/
+-rw-r--r--   0 alejandro   (501) staff       (20)     8044 2024-05-09 11:09:12.000000 llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/PKG-INFO
+-rw-r--r--   0 alejandro   (501) staff       (20)      659 2024-05-09 11:09:13.000000 llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/SOURCES.txt
+-rw-r--r--   0 alejandro   (501) staff       (20)        1 2024-05-09 11:09:13.000000 llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/dependency_links.txt
+-rw-r--r--   0 alejandro   (501) staff       (20)       48 2024-05-09 11:09:13.000000 llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/requires.txt
+-rw-r--r--   0 alejandro   (501) staff       (20)       15 2024-05-09 11:09:13.000000 llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/top_level.txt
```

### Comparing `llmprototyping-0.1.0.dev3/LICENSE` & `llmprototyping-0.1.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev3/setup.py` & `llmprototyping-0.1.0.dev4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="llmprototyping",
     # https://packaging.python.org/en/latest/discussions/versioning/
-    version="0.1.0.dev3",
-    description="A simple set of tools to access llm apis",
+    version="0.1.0.dev4",
+    description="A lightweight set of tools to use several llm and embeddings apis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alejandrolc/llmprototyping",
     author="Alejandro López Correa",
     #author_email="...",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: Apache Software License",
     ],
-    keywords="llm, rag, openai, groq",
+    keywords="llm, rag, openai, groq, ollama",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.9, <4",
     install_requires=required,
 )
```

### Comparing `llmprototyping-0.1.0.dev3/src/llmprototyping/__init__.py` & `llmprototyping-0.1.0.dev4/src/llmprototyping/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,7 +16,16 @@
     pass
 
 try:
     from .embeddings_openai import init as openai_emb_init
     openai_emb_init()
 except ImportError:
     pass
+
+
+try:
+    from .llm_em_ollama import init as ollama_llm_init
+    from .llm_em_ollama import pull_model as ollama_pull_model
+    ollama_llm_init()
+    from .llm_em_ollama import discover as ollama_discover
+except ImportError:
+    pass
```

### Comparing `llmprototyping-0.1.0.dev3/src/llmprototyping/embeddings_interface.py` & `llmprototyping-0.1.0.dev4/src/llmprototyping/embeddings_interface.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev3/src/llmprototyping/embeddings_openai.py` & `llmprototyping-0.1.0.dev4/src/llmprototyping/embeddings_openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     @staticmethod
     def get_computer_name(model_name):
         return f"openai/{model_name}"
 
     def get_embedding(self, text):
         text = text.replace("\n", " ").strip()
-        v = self._client.embeddings.create(input=[text], model=self.model_name).data[0].embedding
+        v = self._client.embeddings.create(input=text, model=self.model_name).data[0].embedding
         if len(v) != self.vector_size:
             raise Exception(f"vector size mismatch; expected:{self.vector_size} got:{len(v)}")
         return EmbeddingVector(v, self.get_computer_name(self.model_name))
 
     def __init__(self, api_key, model_name, max_digest_size, vector_size, comparison_method):
         self._model_name = model_name
         self._client = OpenAI(api_key=api_key)
```

### Comparing `llmprototyping-0.1.0.dev3/src/llmprototyping/error.py` & `llmprototyping-0.1.0.dev4/src/llmprototyping/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
         self.error_type = error_type
         self.info = info
         self.retryable = retryable
         self.extra_data = extra_data
 
     def __str__(self) -> str:
-        return f"AIAgentException {self.error_type} ({'retryable' if self.retryable else 'final'}) {self.info}"
+        return f"LLMException {self.error_type} ({'retryable' if self.retryable else 'final'}) {self.info}"
 
     @staticmethod
     def not_available(info):
         return LLMException("not available", info, True)
     @staticmethod
     def unknown_backend(info):
         return LLMException("unknown backend", info, False)
```

### Comparing `llmprototyping-0.1.0.dev3/src/llmprototyping/factory.py` & `llmprototyping-0.1.0.dev4/src/llmprototyping/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,29 @@
     @classmethod
     @property
     def available_models(cls):
         registry = cls.__get_registry()
         return [x for x in registry.keys()]
 
     @classmethod
-    def register(cls, name, class_obj):
+    def model_registered(cls, name):
+        registry = cls.__get_registry()
+        return name in registry
+
+    @classmethod
+    def register(cls, name, class_obj, alias = None):
         if issubclass(class_obj, cls._class):
             registry = cls.__get_registry()
             registry[name] = class_obj
+            if alias is not None:
+                registry[alias] = class_obj
         else:
             raise LLMException.param_error(f"error registering {class_obj}: type mismatch; expected {cls._class}")
 
     @classmethod
-    def build(cls, name, data):
+    def build(cls, name, data={}):
         registry = cls.__get_registry()
         obj_cls = registry.get(name)
         if obj_cls:
             return obj_cls.from_dict(data)
         else:
             raise LLMException.not_found(f"No model registered with name '{name}'")
```

### Comparing `llmprototyping-0.1.0.dev3/src/llmprototyping/llm_groq.py` & `llmprototyping-0.1.0.dev4/src/llmprototyping/llm_groq.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
             raise LLMException.param_error("temperature must be a float in range [0.0,2.0]")
 
         try:
             rformat = {"type": "json_object"} if json_response else None
             r = self._client.chat.completions.create(
                 messages = [m.to_dict() for m in messages],
                 model = self.model_name,
-                response_format=rformat,
-                temperature=temperature
+                response_format = rformat,
+                temperature = temperature
             )
             rcontent = r.choices[0].message.content
             rrole = r.choices[0].message.role
             msg = Message(content=rcontent, role=rrole)
             input_tokens = r.usage.prompt_tokens
             output_tokens = r.usage.completion_tokens
             response = Response(message=msg, input_token_count=input_tokens, output_token_count=output_tokens)
```

### Comparing `llmprototyping-0.1.0.dev3/src/llmprototyping/llm_interface.py` & `llmprototyping-0.1.0.dev4/src/llmprototyping/llm_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,19 +47,23 @@
     @property
     def status_code(self):
         return self._status_code
     @property
     def error(self):
         return self._error
 
-    def show(self):
+    def show_header(self):
         if not self.is_success:
             print(f"Response failure; status:{self.status_code} error:{self.error}")
         else:
-            print(f"Response successful tokens: i:{self.input_token_count} o:{self.output_token_count} message:")
+            print(f"Response successful; tokens: i:{self.input_token_count} o:{self.output_token_count}")
+
+    def show(self):
+        self.show_header()
+        if self.is_success:
             self.message.show()
 
     @staticmethod
     def error_response(status_code, error):
         return Response(status_code = status_code, error = error, is_success=False)
 
     def __init__(self,
```

### Comparing `llmprototyping-0.1.0.dev3/src/llmprototyping/llm_openai.py` & `llmprototyping-0.1.0.dev4/src/llmprototyping/llm_openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from typing import List
 import inspect
 import openai
 from .llm_interface import LLMChatCompletion, LLMChatCompletionFactory, Message, Response
 from .error import LLMException
 
-@property
-def context_size(self):
-    return self._context_size
-
 class LLMOpenAIChatCompletion(LLMChatCompletion):
     def __init__(self, api_key, model_name, context_size):
         self.model_name = model_name
         self._client = openai.OpenAI(api_key=api_key)
         self._context_size = context_size
 
     @property
@@ -25,16 +21,16 @@
             raise LLMException.param_error("temperature must be a float in range [0.0,2.0]")
 
         try:
             rformat = {"type": "json_object"} if json_response else None
             r = self._client.chat.completions.create(
                 messages = [m.to_dict() for m in messages],
                 model = self.model_name,
-                response_format=rformat,
-                temperature=temperature
+                response_format = rformat,
+                temperature = temperature
             )
             rcontent = r.choices[0].message.content
             rrole = r.choices[0].message.role
             msg = Message(content=rcontent, role=rrole)
             input_tokens = r.usage.prompt_tokens
             output_tokens = r.usage.completion_tokens
             response = Response(message=msg, input_token_count=input_tokens, output_token_count=output_tokens)
```

### Comparing `llmprototyping-0.1.0.dev3/src/llmprototyping/vectordb.py` & `llmprototyping-0.1.0.dev4/src/llmprototyping/vectordb.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev3/src/llmprototyping.egg-info/SOURCES.txt` & `llmprototyping-0.1.0.dev4/src/llmprototyping.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/llmprototyping/__init__.py
 src/llmprototyping/embeddings_interface.py
+src/llmprototyping/embeddings_ollama.py
 src/llmprototyping/embeddings_openai.py
 src/llmprototyping/error.py
 src/llmprototyping/factory.py
+src/llmprototyping/llm_em_ollama.py
 src/llmprototyping/llm_groq.py
 src/llmprototyping/llm_interface.py
 src/llmprototyping/llm_openai.py
 src/llmprototyping/serializable.py
 src/llmprototyping/vectordb.py
 src/llmprototyping.egg-info/PKG-INFO
 src/llmprototyping.egg-info/SOURCES.txt
```

