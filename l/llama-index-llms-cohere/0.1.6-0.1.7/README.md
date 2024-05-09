# Comparing `tmp/llama_index_llms_cohere-0.1.6.tar.gz` & `tmp/llama_index_llms_cohere-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_cohere-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_llms_cohere-0.1.7.tar", max compression
```

## Comparing `llama_index_llms_cohere-0.1.6.tar` & `llama_index_llms_cohere-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       38 2024-04-04 14:59:01.166962 llama_index_llms_cohere-0.1.6/README.md
--rw-r--r--   0        0        0       70 2024-04-04 14:59:01.166962 llama_index_llms_cohere-0.1.6/llama_index/llms/cohere/__init__.py
--rw-r--r--   0        0        0    11689 2024-04-04 14:59:01.166962 llama_index_llms_cohere-0.1.6/llama_index/llms/cohere/base.py
--rw-r--r--   0        0        0     3985 2024-04-04 14:59:01.166962 llama_index_llms_cohere-0.1.6/llama_index/llms/cohere/utils.py
--rw-r--r--   0        0        0     1439 2024-04-04 14:59:01.166962 llama_index_llms_cohere-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 llama_index_llms_cohere-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       38 2024-05-09 16:04:34.265789 llama_index_llms_cohere-0.1.7/README.md
+-rw-r--r--   0        0        0      475 2024-05-09 16:04:34.265789 llama_index_llms_cohere-0.1.7/llama_index/llms/cohere/__init__.py
+-rw-r--r--   0        0        0    11991 2024-05-09 16:04:34.265789 llama_index_llms_cohere-0.1.7/llama_index/llms/cohere/base.py
+-rw-r--r--   0        0        0    11021 2024-05-09 16:04:34.265789 llama_index_llms_cohere-0.1.7/llama_index/llms/cohere/utils.py
+-rw-r--r--   0        0        0     1439 2024-05-09 16:04:34.265789 llama_index_llms_cohere-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 llama_index_llms_cohere-0.1.7/PKG-INFO
```

### Comparing `llama_index_llms_cohere-0.1.6/llama_index/llms/cohere/base.py` & `llama_index_llms_cohere-0.1.7/llama_index/llms/cohere/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from llama_index.core.types import BaseOutputParser, PydanticProgramMode
 from llama_index.llms.cohere.utils import (
     CHAT_MODELS,
     acompletion_with_retry,
     cohere_modelname_to_contextsize,
     completion_with_retry,
     messages_to_cohere_history,
+    remove_documents_from_messages,
 )
 
 import cohere
 
 
 class Cohere(LLM):
     """Cohere LLM.
@@ -43,31 +44,33 @@
         llm = Cohere(model="command", api_key=api_key)
         resp = llm.complete("Paul Graham is ")
         print(resp)
         ```
     """
 
     model: str = Field(description="The cohere model to use.")
-    temperature: float = Field(description="The temperature to use for sampling.")
+    temperature: float = Field(
+        description="The temperature to use for sampling.", default=None
+    )
     max_retries: int = Field(
         default=10, description="The maximum number of API retries."
     )
     additional_kwargs: Dict[str, Any] = Field(
         default_factory=dict, description="Additional kwargs for the Cohere API."
     )
     max_tokens: int = Field(description="The maximum number of tokens to generate.")
 
     _client: Any = PrivateAttr()
     _aclient: Any = PrivateAttr()
 
     def __init__(
         self,
-        model: str = "command",
-        temperature: float = 0.5,
-        max_tokens: int = 512,
+        model: str = "command-r",
+        temperature: Optional[float] = None,
+        max_tokens: Optional[int] = 8192,
         timeout: Optional[float] = None,
         max_retries: int = 10,
         api_key: Optional[str] = None,
         additional_kwargs: Optional[Dict[str, Any]] = None,
         callback_manager: Optional[CallbackManager] = None,
         system_prompt: Optional[str] = None,
         messages_to_prompt: Optional[Callable[[Sequence[ChatMessage]], str]] = None,
@@ -126,16 +129,18 @@
         return {
             **self._model_kwargs,
             **kwargs,
         }
 
     @llm_chat_callback()
     def chat(self, messages: Sequence[ChatMessage], **kwargs: Any) -> ChatResponse:
-        history = messages_to_cohere_history(messages[:-1])
         prompt = messages[-1].content
+        remaining, documents = remove_documents_from_messages(messages[:-1])
+        history = messages_to_cohere_history(remaining)
+
         all_kwargs = self._get_all_kwargs(**kwargs)
         if all_kwargs["model"] not in CHAT_MODELS:
             raise ValueError(f"{all_kwargs['model']} not supported for chat")
 
         if "stream" in all_kwargs:
             warnings.warn(
                 "Parameter `stream` is not supported by the `chat` method."
@@ -143,14 +148,15 @@
             )
         response = completion_with_retry(
             client=self._client,
             max_retries=self.max_retries,
             chat=True,
             message=prompt,
             chat_history=history,
+            documents=documents,
             **all_kwargs,
         )
         return ChatResponse(
             message=ChatMessage(role=MessageRole.ASSISTANT, content=response.text),
             raw=response.__dict__,
         )
 
@@ -178,26 +184,29 @@
             raw=response.__dict__,
         )
 
     @llm_chat_callback()
     def stream_chat(
         self, messages: Sequence[ChatMessage], **kwargs: Any
     ) -> ChatResponseGen:
-        history = messages_to_cohere_history(messages[:-1])
         prompt = messages[-1].content
+        remaining, documents = remove_documents_from_messages(messages[:-1])
+        history = messages_to_cohere_history(remaining)
+
         all_kwargs = self._get_all_kwargs(**kwargs)
         all_kwargs["stream"] = True
         if all_kwargs["model"] not in CHAT_MODELS:
             raise ValueError(f"{all_kwargs['model']} not supported for chat")
         response = completion_with_retry(
             client=self._client,
             max_retries=self.max_retries,
             chat=True,
             message=prompt,
             chat_history=history,
+            documents=documents,
             **all_kwargs,
         )
 
         def gen() -> ChatResponseGen:
             content = ""
             role = MessageRole.ASSISTANT
             for r in response:
```

### Comparing `llama_index_llms_cohere-0.1.6/pyproject.toml` & `llama_index_llms_cohere-0.1.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms cohere integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-cohere"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 cohere = "^5.1.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_llms_cohere-0.1.6/PKG-INFO` & `llama_index_llms_cohere-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-cohere
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index llms cohere integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

