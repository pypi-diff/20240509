# Comparing `tmp/osc_llm-0.1.2.tar.gz` & `tmp/osc_llm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc_llm-0.1.2.tar", max compression
+gzip compressed data, was "osc_llm-0.1.3.tar", max compression
```

## Comparing `osc_llm-0.1.2.tar` & `osc_llm-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      560 2024-04-29 01:55:20.518111 osc_llm-0.1.2/README.md
--rw-r--r--   0        0        0      253 2024-04-30 00:21:10.635963 osc_llm-0.1.2/osc_llm/__init__.py
--rw-r--r--   0        0        0       51 2024-04-27 15:22:11.337904 osc_llm-0.1.2/osc_llm/architectures/__init__.py
--rw-r--r--   0        0        0     8089 2024-04-27 15:21:42.709990 osc_llm-0.1.2/osc_llm/architectures/transformer_decoder.py
--rw-r--r--   0        0        0     4697 2024-05-06 06:38:02.866868 osc_llm-0.1.2/osc_llm/chat.py
--rw-r--r--   0        0        0      136 2024-04-29 08:59:09.247275 osc_llm-0.1.2/osc_llm/chat_templates/__init__.py
--rw-r--r--   0        0        0     1509 2024-04-30 01:49:42.527398 osc_llm-0.1.2/osc_llm/chat_templates/base.py
--rw-r--r--   0        0        0      891 2024-04-27 15:20:32.266209 osc_llm-0.1.2/osc_llm/chat_templates/chatml.py
--rw-r--r--   0        0        0     2751 2024-04-30 12:29:13.554688 osc_llm-0.1.2/osc_llm/chat_templates/llama.py
--rw-r--r--   0        0        0     6733 2024-05-06 11:48:20.141468 osc_llm-0.1.2/osc_llm/cli.py
--rw-r--r--   0        0        0     1314 2024-04-29 23:11:24.182541 osc_llm-0.1.2/osc_llm/config.py
--rw-r--r--   0        0        0       48 2024-04-27 15:57:52.529093 osc_llm-0.1.2/osc_llm/demos/__init__.py
--rw-r--r--   0        0        0     5517 2024-04-27 16:06:43.049671 osc_llm-0.1.2/osc_llm/demos/language_model.py
--rw-r--r--   0        0        0       83 2024-04-29 23:43:54.288202 osc_llm-0.1.2/osc_llm/engines/__init__.py
--rw-r--r--   0        0        0     2084 2024-05-06 06:50:35.853043 osc_llm-0.1.2/osc_llm/engines/base.py
--rw-r--r--   0        0        0     4207 2024-05-07 01:00:24.504971 osc_llm-0.1.2/osc_llm/engines/v1.py
--rw-r--r--   0        0        0     4916 2024-04-30 14:10:25.104449 osc_llm-0.1.2/osc_llm/engines/v2.py
--rw-r--r--   0        0        0      725 2024-04-27 15:10:30.684848 osc_llm-0.1.2/osc_llm/layers/__init__.py
--rw-r--r--   0        0        0      650 2024-04-27 15:10:30.656849 osc_llm-0.1.2/osc_llm/layers/activation.py
--rw-r--r--   0        0        0     6224 2024-04-27 15:10:30.680848 osc_llm-0.1.2/osc_llm/layers/attention.py
--rw-r--r--   0        0        0      186 2024-04-27 15:17:53.918752 osc_llm-0.1.2/osc_llm/layers/dropout.py
--rw-r--r--   0        0        0     2238 2024-04-27 15:10:30.684848 osc_llm-0.1.2/osc_llm/layers/embedding.py
--rw-r--r--   0        0        0     3371 2024-04-27 15:10:30.684848 osc_llm-0.1.2/osc_llm/layers/feedforward.py
--rw-r--r--   0        0        0      336 2024-04-27 15:10:30.684848 osc_llm-0.1.2/osc_llm/layers/head.py
--rw-r--r--   0        0        0     2745 2024-04-27 15:10:30.684848 osc_llm-0.1.2/osc_llm/layers/kv_cache.py
--rw-r--r--   0        0        0     5657 2024-04-27 15:10:30.688848 osc_llm-0.1.2/osc_llm/layers/linear.py
--rw-r--r--   0        0        0      823 2024-04-27 15:10:30.688848 osc_llm-0.1.2/osc_llm/layers/normalization.py
--rw-r--r--   0        0        0      416 2024-04-27 15:17:28.926844 osc_llm-0.1.2/osc_llm/model_helpers/__init__.py
--rw-r--r--   0        0        0     6262 2024-04-27 15:44:58.586217 osc_llm-0.1.2/osc_llm/model_helpers/base.py
--rw-r--r--   0        0        0     3054 2024-04-27 15:16:30.027073 osc_llm-0.1.2/osc_llm/model_helpers/llama.py
--rw-r--r--   0        0        0     3203 2024-04-27 15:34:51.665212 osc_llm-0.1.2/osc_llm/model_helpers/qwen.py
--rw-r--r--   0        0        0       46 2024-04-27 15:00:44.802617 osc_llm-0.1.2/osc_llm/optimizers/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-27 15:00:44.802617 osc_llm-0.1.2/osc_llm/optimizers/scheduler.py
--rw-r--r--   0        0        0      159 2024-04-27 15:10:37.236808 osc_llm-0.1.2/osc_llm/quantizers/__init__.py
--rw-r--r--   0        0        0      717 2024-04-27 15:10:37.244808 osc_llm-0.1.2/osc_llm/quantizers/base.py
--rw-r--r--   0        0        0     8861 2024-04-27 15:33:29.096094 osc_llm-0.1.2/osc_llm/quantizers/int4.py
--rw-r--r--   0        0        0     3347 2024-04-27 15:33:57.584497 osc_llm-0.1.2/osc_llm/quantizers/int8.py
--rw-r--r--   0        0        0       74 2024-04-27 15:04:12.071947 osc_llm-0.1.2/osc_llm/samplers/__init__.py
--rw-r--r--   0        0        0      903 2024-04-27 15:04:12.079947 osc_llm-0.1.2/osc_llm/samplers/base.py
--rw-r--r--   0        0        0     1134 2024-04-27 15:04:12.083947 osc_llm-0.1.2/osc_llm/samplers/top_k.py
--rw-r--r--   0        0        0     1121 2024-04-27 15:04:12.083947 osc_llm-0.1.2/osc_llm/samplers/top_p.py
--rw-r--r--   0        0        0        0 2024-05-06 11:34:05.202914 osc_llm-0.1.2/osc_llm/servers/__init__.py
--rw-r--r--   0        0        0     7635 2024-05-07 01:03:41.381436 osc_llm-0.1.2/osc_llm/servers/openai.py
--rw-r--r--   0        0        0     8774 2024-05-07 02:27:53.539430 osc_llm-0.1.2/osc_llm/tokenizer.py
--rw-r--r--   0        0        0     6405 2024-05-06 10:35:40.498735 osc_llm-0.1.2/osc_llm/utils.py
--rw-r--r--   0        0        0      546 2024-05-07 02:47:55.169520 osc_llm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 osc_llm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      765 2024-05-09 08:34:18.837586 osc_llm-0.1.3/README.md
+-rw-r--r--   0        0        0      253 2024-04-30 00:21:10.635963 osc_llm-0.1.3/osc_llm/__init__.py
+-rw-r--r--   0        0        0     6755 2024-05-09 10:15:03.646846 osc_llm-0.1.3/osc_llm/__main__.py
+-rw-r--r--   0        0        0       51 2024-04-27 15:22:11.337904 osc_llm-0.1.3/osc_llm/architectures/__init__.py
+-rw-r--r--   0        0        0     8089 2024-04-27 15:21:42.709990 osc_llm-0.1.3/osc_llm/architectures/transformer_decoder.py
+-rw-r--r--   0        0        0     4697 2024-05-08 23:04:00.078814 osc_llm-0.1.3/osc_llm/chat.py
+-rw-r--r--   0        0        0      136 2024-04-29 08:59:09.247275 osc_llm-0.1.3/osc_llm/chat_templates/__init__.py
+-rw-r--r--   0        0        0     1663 2024-05-09 08:19:44.319893 osc_llm-0.1.3/osc_llm/chat_templates/base.py
+-rw-r--r--   0        0        0     1058 2024-05-09 08:43:14.223105 osc_llm-0.1.3/osc_llm/chat_templates/chatml.py
+-rw-r--r--   0        0        0     2933 2024-05-09 08:19:52.915836 osc_llm-0.1.3/osc_llm/chat_templates/llama.py
+-rw-r--r--   0        0        0     1314 2024-04-29 23:11:24.182541 osc_llm-0.1.3/osc_llm/config.py
+-rw-r--r--   0        0        0       48 2024-04-27 15:57:52.529093 osc_llm-0.1.3/osc_llm/demos/__init__.py
+-rw-r--r--   0        0        0     5517 2024-04-27 16:06:43.049671 osc_llm-0.1.3/osc_llm/demos/language_model.py
+-rw-r--r--   0        0        0       83 2024-04-29 23:43:54.288202 osc_llm-0.1.3/osc_llm/engines/__init__.py
+-rw-r--r--   0        0        0     1951 2024-05-09 00:43:57.688337 osc_llm-0.1.3/osc_llm/engines/base.py
+-rw-r--r--   0        0        0     4207 2024-05-07 01:00:24.504971 osc_llm-0.1.3/osc_llm/engines/v1.py
+-rw-r--r--   0        0        0     4916 2024-04-30 14:10:25.104449 osc_llm-0.1.3/osc_llm/engines/v2.py
+-rw-r--r--   0        0        0      705 2024-05-09 10:13:55.630489 osc_llm-0.1.3/osc_llm/layers/__init__.py
+-rw-r--r--   0        0        0      650 2024-04-27 15:10:30.656849 osc_llm-0.1.3/osc_llm/layers/activation.py
+-rw-r--r--   0        0        0     6224 2024-04-27 15:10:30.680848 osc_llm-0.1.3/osc_llm/layers/attention.py
+-rw-r--r--   0        0        0      186 2024-04-27 15:17:53.918752 osc_llm-0.1.3/osc_llm/layers/dropout.py
+-rw-r--r--   0        0        0     2238 2024-04-27 15:10:30.684848 osc_llm-0.1.3/osc_llm/layers/embedding.py
+-rw-r--r--   0        0        0     3371 2024-04-27 15:10:30.684848 osc_llm-0.1.3/osc_llm/layers/feedforward.py
+-rw-r--r--   0        0        0      336 2024-04-27 15:10:30.684848 osc_llm-0.1.3/osc_llm/layers/head.py
+-rw-r--r--   0        0        0     2745 2024-04-27 15:10:30.684848 osc_llm-0.1.3/osc_llm/layers/kv_cache.py
+-rw-r--r--   0        0        0     6023 2024-05-09 10:13:37.142379 osc_llm-0.1.3/osc_llm/layers/linear.py
+-rw-r--r--   0        0        0      823 2024-04-27 15:10:30.688848 osc_llm-0.1.3/osc_llm/layers/normalization.py
+-rw-r--r--   0        0        0      416 2024-04-27 15:17:28.926844 osc_llm-0.1.3/osc_llm/model_helpers/__init__.py
+-rw-r--r--   0        0        0     4350 2024-05-09 10:16:01.331095 osc_llm-0.1.3/osc_llm/model_helpers/base.py
+-rw-r--r--   0        0        0     3054 2024-04-27 15:16:30.027073 osc_llm-0.1.3/osc_llm/model_helpers/llama.py
+-rw-r--r--   0        0        0     3285 2024-05-09 07:37:31.990997 osc_llm-0.1.3/osc_llm/model_helpers/qwen.py
+-rw-r--r--   0        0        0       46 2024-04-27 15:00:44.802617 osc_llm-0.1.3/osc_llm/optimizers/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-27 15:00:44.802617 osc_llm-0.1.3/osc_llm/optimizers/scheduler.py
+-rw-r--r--   0        0        0      139 2024-05-09 10:14:52.802794 osc_llm-0.1.3/osc_llm/quantizers/__init__.py
+-rw-r--r--   0        0        0      717 2024-04-27 15:10:37.244808 osc_llm-0.1.3/osc_llm/quantizers/base.py
+-rw-r--r--   0        0        0     8861 2024-04-27 15:33:29.096094 osc_llm-0.1.3/osc_llm/quantizers/int4.py
+-rw-r--r--   0        0        0     3912 2024-05-09 10:18:30.539547 osc_llm-0.1.3/osc_llm/quantizers/int8.py
+-rw-r--r--   0        0        0       74 2024-04-27 15:04:12.071947 osc_llm-0.1.3/osc_llm/samplers/__init__.py
+-rw-r--r--   0        0        0      903 2024-04-27 15:04:12.079947 osc_llm-0.1.3/osc_llm/samplers/base.py
+-rw-r--r--   0        0        0     1122 2024-05-09 11:29:40.084349 osc_llm-0.1.3/osc_llm/samplers/top_k.py
+-rw-r--r--   0        0        0     1121 2024-04-27 15:04:12.083947 osc_llm-0.1.3/osc_llm/samplers/top_p.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:34:05.202914 osc_llm-0.1.3/osc_llm/servers/__init__.py
+-rw-r--r--   0        0        0     7453 2024-05-09 11:17:44.753636 osc_llm-0.1.3/osc_llm/servers/openai.py
+-rw-r--r--   0        0        0     8873 2024-05-09 08:14:53.581992 osc_llm-0.1.3/osc_llm/tokenizer.py
+-rw-r--r--   0        0        0     6405 2024-05-06 10:35:40.498735 osc_llm-0.1.3/osc_llm/utils.py
+-rw-r--r--   0        0        0      547 2024-05-08 23:00:15.836746 osc_llm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1626 1970-01-01 00:00:00.000000 osc_llm-0.1.3/PKG-INFO
```

### Comparing `osc_llm-0.1.2/osc_llm/architectures/transformer_decoder.py` & `osc_llm-0.1.3/osc_llm/architectures/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/chat.py` & `osc_llm-0.1.3/osc_llm/chat.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/chat_templates/chatml.py` & `osc_llm-0.1.3/osc_llm/chat_templates/chatml.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 @registry.chat_templates.register("Yi")
 @registry.chat_templates.register("Qwen")
 @registry.chat_templates.register("ChatML")
 class ChatMLChatTemplate(ChatTemplate):
     
     default_system: str = "You are a helpful assistant."
     stop_texts: List[str] = ["<|im_end|>"]
+    generate_prompt: str = "<|im_start|>assistant\n"
     
     @classmethod
-    def apply_messages(cls, messages: List[Message]) -> str:
+    def apply_messages(cls, messages: List[Message], add_generate_prompt: bool = True) -> str:
         prompt = ""
         for message in messages:
             if message.role == "user":
-                prompt += f"<|im_start|>user\n{message.content}<|im_end|>\n"
+                prompt += f"<|im_start|>user\n{message.content}\n<|im_end|>\n"
             elif message.role == "assistant":
-                prompt += f"<|im_start|>assistant\n{message.content}<|im_end|>\n"
+                prompt += f"<|im_start|>assistant\n{message.content}\n<|im_end|>\n"
             elif message.role == "system":
-                prompt += f"<|im_start|>system\n{message.content}<|im_end|>\n"
+                prompt += f"<|im_start|>system\n{message.content}\n<|im_end|>\n"
+        if add_generate_prompt:
+            prompt += cls.generate_prompt
         return prompt
```

### Comparing `osc_llm-0.1.2/osc_llm/chat_templates/llama.py` & `osc_llm-0.1.3/osc_llm/chat_templates/llama.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 
 
 @registry.chat_templates.register("Llama3-8B-Chinese-Chat")
 @registry.chat_templates.register("Llama-3")
 class Llama3ChatTemplate(ChatTemplate):
     
     stop_texts: List[str] = ["<|end_of_text|>", "<|eot_id|>"]
+    generate_prompt: str = "<|start_header_id|>assistant<|end_header_id|>\n\n"
     
     @classmethod
-    def apply_messages(cls, messages: List[Message]) -> str:
+    def apply_messages(cls, messages: List[Message], add_generate_prompt: bool = False) -> str:
         assert messages[-1].role == "user", "Last message must be user"
         prompt = "<|begin_of_text|>"
         for message in messages:
             prompt += _apply_message_llama3(message)
-        prompt += "<|start_header_id|>assistant<|end_header_id|>\n\n"
+        if add_generate_prompt:
+            prompt += cls.generate_prompt
         return prompt
     
 def _apply_message_llama3(message: Message) -> str:
     template = "<|start_header_id|>{role}<|end_header_id|>\n\n{content}<|eot_id|>"
     return template.format(role=message.role, content=message.content)
 
 
@@ -29,17 +31,18 @@
     default_system: str = ("You are a helpful, respectful and honest assistant. Always answer as helpfully as"
             " possible, while being safe.  Your answers should not include any harmful, unethical, racist, sexist,"
             " toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and"
             " positive in nature.\n\nIf a question does not make any sense, or is not factually coherent, explain why"
             " instead of answering something not correct. If you don't know the answer to a question, please don't"
             " share false information.")
     stop_texts: List[str] = []
+    generate_prompt: str = ''
     
     @classmethod
-    def apply_messages(cls, messages: List[Message]) -> str:
+    def apply_messages(cls, messages: List[Message], add_generate_prompt: bool = True) -> str:
         if messages[0].role == 'system':
             assert len(messages) >= 2, "must have a user input"
             assert messages[1].role == "user", "must have a user input"
             prompt = f"[INST] <<SYS>>\n{messages[0].content}\n<</SYS>>\n\n{messages[1].content} [/INST]"
             for message in messages[2:]:
                 prompt += _apply_message_llama2(message)
         else:
```

### Comparing `osc_llm-0.1.2/osc_llm/cli.py` & `osc_llm-0.1.3/osc_llm/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from jsonargparse import CLI 
 from .chat import main as chat_main
 from .servers.openai import main as openai_main
 from .model_helpers import get_supported_architectures
 from .model_helpers.base import HFModelHelper
-from .quantizers import WeightOnlyInt8Quantizer, WeightOnlyInt4Quantizer
+from .quantizers import Int8Quantizer, WeightOnlyInt4Quantizer
 from .tokenizer import Tokenizer
 from .config import registry
 from .utils import build_from_checkpoint
 from pathlib import Path
 from wasabi import msg
 from typing import Literal, Optional
 import json
@@ -17,22 +17,22 @@
 
 
 
 _SAFETENSORS_AVAILABLE = RequirementCache("safetensors")
 
 def download_huggingface_model(repo_id: str, 
                                save_dir: str = "./checkpoints",
-                               force_download: bool = False,
+                               force_download: bool = True,
                                access_token: Optional[str] = os.getenv("HF_TOKEN"),
                                from_safetensors: bool = False):
     
     directory = Path(save_dir, repo_id)
     if directory.exists():
         if not force_download:
-            msg.fail(f"Directory {directory} already exists. Use --force-download to re-download.", exits=1)
+            msg.fail(f"Directory {directory} already exists. Use --force_download to re-download.", exits=1)
         else:
             msg.info(f"Directory {directory} already exists. Re-downloading.")
             import shutil
             shutil.rmtree(directory)
     if not directory.exists():
         directory.mkdir(parents=True)      
     from huggingface_hub import snapshot_download
@@ -110,15 +110,15 @@
     save_dir= Path(save_dir)
     if save_dir == checkpoint_dir:
         msg.warn("The quantized model will replace the original model.")
     if not save_dir.exists():
         save_dir.mkdir(parents=True)
     tokenizer = Tokenizer(checkpoint_dir=checkpoint_dir)
     model, config = build_from_checkpoint(checkpoint_dir=checkpoint_dir, return_config=True)
-    quantizer = WeightOnlyInt8Quantizer()
+    quantizer = Int8Quantizer()
     model = quantizer.quantize(model)
     config = config.merge(quantizer.quantizer_config)
     torch.save(model.state_dict(), Path(save_dir) / "osc_model.pth")
     config.to_disk(Path(save_dir) / "config.cfg")
     tokenizer.save(save_dir)
     
     
@@ -169,9 +169,13 @@
         "int4": quantize_int4
     },
     "serve": openai_main
 }
 
 
 
-def run_cli():
-    CLI(components=commands, as_positional=False)
+def run():
+    CLI(components=commands, as_positional=False)
+    
+    
+if __name__ == "__main__":
+    run()
```

### Comparing `osc_llm-0.1.2/osc_llm/config.py` & `osc_llm-0.1.3/osc_llm/config.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/demos/language_model.py` & `osc_llm-0.1.3/osc_llm/demos/language_model.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/engines/base.py` & `osc_llm-0.1.3/osc_llm/engines/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,16 +49,14 @@
         raise NotImplementedError
     
     def setup(self) -> None:
         t = perf_counter()
         self.load_model()
         self.fabric.print(f"load model in {perf_counter() - t:.02f} seconds", file=sys.stderr)
         if self.compile:
-            t = perf_counter()
             self.compile_model()
-            self.fabric.print(f"compile model in {perf_counter() - t:.02f} seconds", file=sys.stderr)
         t = perf_counter()
         self.setup_model()
         self.fabric.print(f"setup model in {perf_counter() - t:.02f} seconds", file=sys.stderr)
             
     def reset_sampler(self, sampler: Sampler) -> None:
         self.sampler = sampler
```

### Comparing `osc_llm-0.1.2/osc_llm/engines/v1.py` & `osc_llm-0.1.3/osc_llm/engines/v1.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/engines/v2.py` & `osc_llm-0.1.3/osc_llm/engines/v2.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/layers/activation.py` & `osc_llm-0.1.3/osc_llm/layers/activation.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/layers/attention.py` & `osc_llm-0.1.3/osc_llm/layers/attention.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/layers/embedding.py` & `osc_llm-0.1.3/osc_llm/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/layers/feedforward.py` & `osc_llm-0.1.3/osc_llm/layers/feedforward.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/layers/kv_cache.py` & `osc_llm-0.1.3/osc_llm/layers/kv_cache.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/layers/linear.py` & `osc_llm-0.1.3/osc_llm/layers/linear.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,38 +8,48 @@
 
 
 @registry.layers.register("Linear")
 def Linear(n_in: int, n_out: int, bias: bool = True):
     return nn.Linear(in_features=n_in, out_features=n_out, bias=bias)
 
 
-@registry.layers.register("WeightOnlyInt8Linear")
-class WeightOnlyInt8Linear(nn.Module):
+@registry.layers.register("Int8Linear")
+class Int8Linear(nn.Module):
     """用于量化的Linear层，只包含weight和scales两个参数"""
     __contains__ = ["in_features", "out_features"]
     in_features: int
     out_features: int
     weight: torch.Tensor
     
     def __init__(
         self,
         in_features: int,
         out_features: int,
+        bias: bool = False
     ):
         super().__init__()
         
         self.in_features = in_features
         self.out_features = out_features
         self.register_buffer("weight", torch.empty((out_features, in_features), dtype=torch.int8))
         self.register_buffer("scales", torch.ones(out_features, dtype=torch.bfloat16))
+        if bias:
+            self.register_buffer("bias", torch.zeros(out_features, dtype=torch.bfloat16))
+        else:
+            self.bias = None
         
     def forward(self, input: torch.Tensor) -> torch.Tensor:
-        return F.linear(input, self.weight.to(dtype=input.dtype)) * self.scales
+        
+        if self.bias is not None:
+            logits = F.linear(input, self.weight.to(dtype=input.dtype)) * self.scales + self.bias.to(dtype=input.dtype)
+        else:
+            logits = F.linear(input, self.weight.to(dtype=input.dtype)) * self.scales
+        return logits
+    
     
-
 @registry.layers.register("WeightOnlyInt4Linear")
 class WeightOnlyInt4Linear(torch.nn.Module):
     __constants__ = ['in_features', 'out_features']
     in_features: int
     out_features: int
     weight: torch.Tensor
```

### Comparing `osc_llm-0.1.2/osc_llm/layers/normalization.py` & `osc_llm-0.1.3/osc_llm/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/model_helpers/base.py` & `osc_llm-0.1.3/osc_llm/model_helpers/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import json 
 from pathlib import Path
 from typing import Dict
 import torch
-from typing import Literal
 from ..config import Config
 from ..utils import build_model
-from ..quantizers import WeightOnlyInt4Quantizer, WeightOnlyInt8Quantizer
 from ..tokenizer import Tokenizer
 from wasabi import msg
 
 
 
 class HFModelHelper:
     
@@ -100,45 +98,8 @@
                     sd[wmap[key]] = f.get_tensor(key)
         return sd
         
     def load_checkpoint(self, checkpoint_name: str = 'osc_model.pth', device: str = 'cpu'):
         model = build_model(config=self.osc_config)
         model.load_state_dict(torch.load(str(self.checkpoint_dir / checkpoint_name), mmap=True, weights_only=True), assign=True)
         model.to(device)
-        return model.eval()
-        
-    def quantize_int8(self, save_dir: str):
-        model = self.load_checkpoint()
-        helper = WeightOnlyInt8Quantizer()
-        quantized_model = helper.quantize(model)
-        merged_config: Config = self.osc_config.merge(helper.quantizer_config)
-        save_dir = Path(save_dir)
-        if not save_dir.exists():
-            save_dir.mkdir(parents=True)
-        checkpoint_path = Path(save_dir) / 'osc_model.pth'
-        merged_config_path = Path(save_dir) / "config.cfg"
-        torch.save(quantized_model.state_dict(), checkpoint_path)
-        merged_config.to_disk(merged_config_path)
-        if self.tokenizer:
-            self.tokenizer.save(save_dir)
-        
-    def quantize_int4(self,
-                      save_dir: str, 
-                      groupsize: Literal[32, 64, 128, 256] = 32, 
-                      k: Literal[2, 4, 8] = 8, 
-                      padding: bool = True, 
-                      device: str = 'cuda'):
-        assert torch.cuda.is_available(), 'Only support cuda device for int4 quantization'
-        assert 'cuda' in device, 'Only support cuda device for int4 quantization'
-        model = self.load_checkpoint(device=device)
-        helper = WeightOnlyInt4Quantizer(groupsize=groupsize, inner_k_tiles=k, padding_allowed=padding)
-        quantized_model = helper.quantize(model)
-        merged_config: Config = self.osc_config.merge(helper.quantizer_config)
-        save_dir = Path(save_dir)
-        if not save_dir.exists():
-            save_dir.mkdir(parents=True)
-        checkpoint_path = save_dir / 'osc_model.pth'
-        merged_config_path = save_dir / "config.cfg"
-        torch.save(quantized_model.state_dict(), checkpoint_path)
-        merged_config.to_disk(merged_config_path)
-        if self.tokenizer:
-            self.tokenizer.save(save_dir)
+        return model.eval()
```

### Comparing `osc_llm-0.1.2/osc_llm/model_helpers/llama.py` & `osc_llm-0.1.3/osc_llm/model_helpers/llama.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/model_helpers/qwen.py` & `osc_llm-0.1.3/osc_llm/model_helpers/qwen.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,17 @@
         n_embeddings = {vocab_size}
         embedding_size = {hidden_size}
 
         [model.feedforward]
         @layers = "SwiGLU"
         n_in = {hidden_size}
         n_hidden = {intermediate_size}
+        up_bias = "False"
+        gate_bias = "False"
+        down_bias = "False"
 
         [model.head]
         @layers = "Linear"
         n_in = {hidden_size}
         n_out = {vocab_size}
         bias = "False"
```

### Comparing `osc_llm-0.1.2/osc_llm/optimizers/scheduler.py` & `osc_llm-0.1.3/osc_llm/optimizers/scheduler.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/quantizers/base.py` & `osc_llm-0.1.3/osc_llm/quantizers/base.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/quantizers/int4.py` & `osc_llm-0.1.3/osc_llm/quantizers/int4.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/quantizers/int8.py` & `osc_llm-0.1.3/osc_llm/quantizers/int8.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,72 @@
 from .base import Quantizer
-from ..layers import WeightOnlyInt8Linear
+from ..layers import Int8Linear
 from ..config import registry
 from confection import Config
 import torch.nn as nn
 import torch
 
 
 
-@registry.quantizers.register("WeightOnlyInt8Quantizer")
-class WeightOnlyInt8Quantizer(Quantizer):
-    
+@registry.quantizers.register("Int8Quantizer")
+class Int8Quantizer(Quantizer):
     def quantize(self, model: nn.Module) -> nn.Module:
         for name, children in model.named_children():
             if isinstance(children, torch.nn.Linear):
                 int8_weight, scales, _ = self._dynamically_quantize_per_channel(children.weight.float(), -128, 127, torch.int8)
-                int8_linear = WeightOnlyInt8Linear(in_features=children.in_features, out_features=children.out_features)
-                int8_linear.weight = int8_weight
-                int8_linear.scales = scales
+                if hasattr(children, "bias") and children.bias is not None:
+                    int8_linear = Int8Linear(in_features=children.in_features, out_features=children.out_features, bias=True)
+                    int8_linear.bias = children.bias
+                    int8_linear.weight = int8_weight
+                    int8_linear.scales = scales
+                else:
+                    int8_linear = Int8Linear(in_features=children.in_features, out_features=children.out_features)
+                    int8_linear.weight = int8_weight
+                    int8_linear.scales = scales
                 setattr(model, name, int8_linear)
             else:
                 self.quantize(model=children)
         return model
         
     def convert_for_runtime(self, model: nn.Module) -> nn.Module:
         model = self._replace_linear_weight_only_int8_per_channel(model)
         return model
     
     @property
     def quantizer_config(self):
         config_str = """
         [quantizer]
-        @quantizers = "WeightOnlyInt8Quantizer"
+        @quantizers = "Int8Quantizer"
         """
         config = Config().from_str(config_str)
         return config
         
     def _replace_linear_weight_only_int8_per_channel(self, module: nn.Module) -> nn.Module:
         """递归替换module中的所有nn.Linear为WeightOnlyInt8Linear"""
         for name, child in module.named_children():
             if isinstance(child, nn.Linear):
-                setattr(module, name, WeightOnlyInt8Linear(child.in_features, child.out_features))
+                if hasattr(child, "bias") and child.bias is not None:
+                    setattr(module, name, Int8Linear(child.in_features, child.out_features, bias=True))
+                else:
+                    setattr(module, name, Int8Linear(child.in_features, child.out_features))
             else:
                 self._replace_linear_weight_only_int8_per_channel(child)
         return module
                 
-    def _dynamically_quantize_per_channel(self, x, quant_min, quant_max, target_dtype):
+    def _dynamically_quantize_per_channel(self, x, quant_min = -128, quant_max = 127, target_dtype: torch.dtype = torch.int8):
         # assumes symmetric quantization
         # assumes axis == 0
         # assumes dense memory format
         # TODO(future): relax ^ as needed
 
         # default setup for affine quantization of activations
         eps = torch.finfo(torch.float32).eps
 
         # get min and max
-        min_val, max_val = torch.aminmax(x, dim=1)
+        min_val, max_val = torch.aminmax(x, dim=-1)
 
         # calculate scales and zero_points based on min and max
         # reference: https://fburl.com/code/srbiybme
         min_val_neg = torch.min(min_val, torch.zeros_like(min_val))
         max_val_pos = torch.max(max_val, torch.zeros_like(max_val))
         device = min_val_neg.device
```

### Comparing `osc_llm-0.1.2/osc_llm/samplers/base.py` & `osc_llm-0.1.3/osc_llm/samplers/base.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/samplers/top_k.py` & `osc_llm-0.1.3/osc_llm/samplers/top_k.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 class TopK(Sampler):
     def __init__(
         self, 
         k: int = 10,
         temperature: float = 1.0,
         ) -> None:
         super().__init__()
-        assert temperature > 0
-        self.temperature = temperature
+        self.temperature = 0.001 if temperature <=0 else temperature
         self.k = k 
         
     def logits_to_probs(self, logits: torch.Tensor) -> torch.Tensor:
-        logits = logits / min(self.temperature, 1e-5)
+        logits = logits / self.temperature
         values, indices = torch.topk(logits, min(self.k, logits.shape[-1]), dim=-1)
         logits = torch.full_like(logits, float("-inf")).scatter_(-1, indices, values)
         probs = torch.softmax(logits, dim=-1)
         return probs
     
     def probs_to_ids(self, probs: torch.Tensor) -> torch.Tensor:
         ids = self.multinomial_sample_one(probs=probs)
```

### Comparing `osc_llm-0.1.2/osc_llm/samplers/top_p.py` & `osc_llm-0.1.3/osc_llm/samplers/top_p.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/osc_llm/servers/openai.py` & `osc_llm-0.1.3/osc_llm/servers/openai.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..engines import LLMEngineV2, LLMEngineV1
+from ..engines import LLMEngineV2, LLMEngineV1, LLMEngine
 from ..tokenizer import Tokenizer
 from ..chat_templates import Message
 from ..utils import random_uuid
 from ..samplers import TopK
 from typing import List, Optional, Dict, Union, Literal
 from fastapi import FastAPI
 from fastapi.responses import StreamingResponse, JSONResponse
@@ -118,24 +118,26 @@
     
     
 def main(checkpoint_dir: str,
          engine: Literal['v1', 'v2'] = 'v1',
          accelerator: Literal['cuda', 'cpu', 'gpu', 'auto'] = 'cuda',
          devices: Union[int, List[int]] = 1,
          host: str = '0.0.0.0',
-         port: int = 8000):
+         port: int = 8000,
+         compile: bool = True):
     """openai接口服务
 
     Args:
         checkpoint_dir (str): checkpoint目录
-        engine (Literal[&#39;v1&#39;, &#39;v2&#39;], optional): LLMEngine版本. Defaults to 'v2'.
+        engine (Literal[&#39;v1&#39;, &#39;v2&#39;], optional): LLMEngine版本. Defaults to 'v1'.
         accelerator (Literal[&#39;cuda&#39;, &#39;cpu&#39;, &#39;gpu&#39;, &#39;auto&#39;], optional): 推理硬件. Defaults to 'cuda'.
         devices (Union[int, List[int]], optional): 设备数量或者设备的ID. Defaults to 1.
         host (str, optional): 主机地址. Defaults to '0.0.0.0'.
         port (int, optional): 端口号. Defaults to 8000.
+        compile (bool, optional): 是否编译模型. Defaults to True.
     """
     
     app = FastAPI()
     
     @app.post("/v1/chat/completions")
     def create_chat_completion(request: ChatCompletionRequest):
         with engine.fabric.init_tensor():
@@ -163,28 +165,21 @@
                 completion_tokens += 1
             prompt_tokens = len(input_ids)
             total_tokens = prompt_tokens + completion_tokens
             response = ChatCompletionResponse(id=f"chatcmpl-{random_uuid()}",
                                                   model=request.model,
                                                   choices=[ChatCompletionResponseChoice(index=0, message=ChatMessage(role='assistant', content=content))],
                                                   usage=UsageInfo(prompt_tokens=prompt_tokens, total_tokens=total_tokens, completion_tokens=completion_tokens))
-            return JSONResponse(content=response.model_dump_json(exclude_unset=True))
+            return JSONResponse(content=response.model_dump(exclude_unset=True))
     
     if engine == 'v1':
-        engine = LLMEngineV1(checkpoint_dir, devices=devices, accelerator=accelerator)
+        engine: LLMEngine = LLMEngineV1(checkpoint_dir, devices=devices, accelerator=accelerator, compile=compile)
     else:
-        engine = LLMEngineV2(checkpoint_dir, devices=devices, accelerator=accelerator)
+        engine: LLMEngine = LLMEngineV2(checkpoint_dir, devices=devices, accelerator=accelerator, compile=compile)
     engine.setup()
-    tokenizer = Tokenizer(checkpoint_dir)
-    
-    warmup_messages = [[Message(role='user', content="你好")], [Message(role='user', content="介绍一下你自己")]]
-    engine.fabric.print("Warming up engine that may take one or two minutes...")
-    start_time = time.perf_counter()
-    for messages in warmup_messages:
-        input_ids = tokenizer.encode_messages(messages)
-        stream = engine.run(input_ids=input_ids, stop_ids=tokenizer.stop_ids)
-        stream_tokens = tokenizer.decode_stream(stream=stream)
-        for token in stream_tokens:
-            pass
-    engine.fabric.print(f"Engine warmup finished in {time.perf_counter() - start_time:.2f}s")
+    tokenizer = Tokenizer(checkpoint_dir=checkpoint_dir)
     
+    # Todo: 在启动模型编译的情况下第一次运行需要耗费很多时间(几分钟),如何在启动的时候预热模型?
+    if compile:
+        from wasabi import msg
+        msg.warn("you are using compile mode, the first run may take a long time")
     uvicorn.run(app=app, host=host, port=port)
```

### Comparing `osc_llm-0.1.2/osc_llm/tokenizer.py` & `osc_llm-0.1.3/osc_llm/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,21 +108,22 @@
             tokens = tokens + [self.eos_id]
         if max_length > 0:
             tokens = tokens[:max_length]
         return torch.tensor(tokens, dtype=torch.int, device=device)
     
     def encode_messages(self, 
                         messages: List[Message], 
+                        add_generate_prompt: bool = True,
                         device: Optional[torch.device] = None,
                         bos: Optional[bool] = None,
                         eos: bool = False,
                         max_length: int = -1,
                         ) -> torch.Tensor:
         assert self.chat_template, "Chat template is required for encoding messages"
-        string = self.chat_template.apply_messages(messages)
+        string = self.chat_template.apply_messages(messages, add_generate_prompt=add_generate_prompt)
         return self.encode(string, device, bos, eos, max_length)
 
     def decode(self, tensor: torch.Tensor) -> str:
         tokens = [tensor.item()] if tensor.ndim == 0 else tensor.tolist()
         return self.processor.decode(tokens)
     
     def decode_stream(
```

### Comparing `osc_llm-0.1.2/osc_llm/utils.py` & `osc_llm-0.1.3/osc_llm/utils.py`

 * *Files identical despite different names*

### Comparing `osc_llm-0.1.2/pyproject.toml` & `osc_llm-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "osc-llm"
-version = "0.1.2"
+version = "0.1.3"
 description = "大模型训练,推理,部署工具"
 authors = ["wangmengdi <790990241@qq.com>"]
 license = "mit"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
@@ -15,13 +15,13 @@
 confection = ">=0.1.4"
 catalogue = ">=2.0.10"
 sentencepiece = ">=0.2.0"
 tokenizers  = ">=0.19.1"
 
 
 [tool.poetry.scripts]
-llm = "osc_llm.cli:run_cli"
+llm = "osc_llm.__main__:run"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

