# Comparing `tmp/agentic_security-0.1.4.tar.gz` & `tmp/agentic_security-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentic_security-0.1.4.tar", max compression
+gzip compressed data, was "agentic_security-0.1.5.tar", max compression
```

## Comparing `agentic_security-0.1.4.tar` & `agentic_security-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0    11367 2024-05-04 09:49:34.419064 agentic_security-0.1.4/LICENSE
--rw-r--r--   0        0        0     9128 2024-05-04 09:49:34.419064 agentic_security-0.1.4/Readme.md
--rw-r--r--   0        0        0       64 2024-05-04 09:49:34.419064 agentic_security-0.1.4/agentic_security/__init__.py
--rw-r--r--   0        0        0      595 2024-05-04 09:49:34.419064 agentic_security-0.1.4/agentic_security/__main__.py
--rw-r--r--   0        0        0     8903 2024-05-04 09:49:34.419064 agentic_security-0.1.4/agentic_security/agent.py
--rw-r--r--   0        0        0     5365 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/app.py
--rw-r--r--   0        0        0     2900 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/http_spec.py
--rw-r--r--   0        0        0     2265 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/lib.py
--rw-r--r--   0        0        0        0 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_actor/__init__.py
--rw-r--r--   0        0        0        0 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_actor/__main__.py
--rw-r--r--   0        0        0     3720 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_actor/fuzzer.py
--rw-r--r--   0        0        0     1209 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_actor/refusal.py
--rw-r--r--   0        0        0      458 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_actor/test_refusal.py
--rw-r--r--   0        0        0     4325 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/__init__.py
--rw-r--r--   0        0        0     9314 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/data.py
--rw-r--r--   0        0        0        0 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/modules/__init__.py
--rw-r--r--   0        0        0     6593 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/modules/adaptive_attacks.py
--rw-r--r--   0        0        0     1910 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/modules/garak_tool.py
--rw-r--r--   0        0        0     2446 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/modules/test_adaptive_attacks.py
--rw-r--r--   0        0        0     2645 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/stenography_fn.py
--rw-r--r--   0        0        0      725 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/probe_data/test_data.py
--rw-r--r--   0        0        0     2365 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/report_chart.py
--rw-r--r--   0        0        0    27290 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/static/index.html
--rw-r--r--   0        0        0      657 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/test_lib.py
--rw-r--r--   0        0        0     1961 2024-05-04 09:49:34.423064 agentic_security-0.1.4/agentic_security/test_spec.py
--rw-r--r--   0        0        0     1349 2024-05-04 09:49:34.423064 agentic_security-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    10514 1970-01-01 00:00:00.000000 agentic_security-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11367 2024-05-09 07:19:59.173263 agentic_security-0.1.5/LICENSE
+-rw-r--r--   0        0        0    10009 2024-05-09 07:19:59.177263 agentic_security-0.1.5/Readme.md
+-rw-r--r--   0        0        0       64 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/__init__.py
+-rw-r--r--   0        0        0      595 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/__main__.py
+-rw-r--r--   0        0        0     8903 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/agent.py
+-rw-r--r--   0        0        0     6489 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/app.py
+-rw-r--r--   0        0        0     2900 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/http_spec.py
+-rw-r--r--   0        0        0     2265 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/lib.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_actor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_actor/__main__.py
+-rw-r--r--   0        0        0     3720 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_actor/fuzzer.py
+-rw-r--r--   0        0        0     1209 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_actor/refusal.py
+-rw-r--r--   0        0        0      458 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_actor/test_refusal.py
+-rw-r--r--   0        0        0     4643 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_data/__init__.py
+-rw-r--r--   0        0        0     9535 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_data/data.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_data/modules/__init__.py
+-rw-r--r--   0        0        0     6593 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_data/modules/adaptive_attacks.py
+-rw-r--r--   0        0        0     1909 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_data/modules/garak_tool.py
+-rw-r--r--   0        0        0      411 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_data/modules/inspect_ai_task.py
+-rw-r--r--   0        0        0     2238 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_data/modules/inspect_ai_tool.py
+-rw-r--r--   0        0        0     2446 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_data/modules/test_adaptive_attacks.py
+-rw-r--r--   0        0        0     2645 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_data/stenography_fn.py
+-rw-r--r--   0        0        0      725 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/probe_data/test_data.py
+-rw-r--r--   0        0        0     2365 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/report_chart.py
+-rw-r--r--   0        0        0    27290 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/static/index.html
+-rw-r--r--   0        0        0      657 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/test_lib.py
+-rw-r--r--   0        0        0     1961 2024-05-09 07:19:59.177263 agentic_security-0.1.5/agentic_security/test_spec.py
+-rw-r--r--   0        0        0     1358 2024-05-09 07:19:59.177263 agentic_security-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    11391 1970-01-01 00:00:00.000000 agentic_security-0.1.5/PKG-INFO
```

### Comparing `agentic_security-0.1.4/LICENSE` & `agentic_security-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/Readme.md` & `agentic_security-0.1.5/Readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,19 +22,27 @@
 ## Features
 
 - Customizable Rule Sets or Agent based attacks🛠️
 - Comprehensive fuzzing for any LLMs 🧪
 - LLM API integration and stress testing 🛠️
 - Wide range of fuzzing and attack techniques 🌀
 
-Note: Please be aware that Agentic Security is designed as a safety scanner tool and not a foolproof solution. It cannot guarantee complete protection against all possible threats.
 
-## About the Project 🧙
+| Tool                    | Source                                                                        | Integrated |
+|-------------------------|-------------------------------------------------------------------------------|------------|
+| Garak                   | [leondz/garak](https://github.com/leondz/garak2)                              | ✅          |
+| InspectAI               | [UKGovernmentBEIS/inspect_ai](https://github.com/UKGovernmentBEIS/inspect_ai) | ✅          |
+| llm-adaptive-attacks    | [tml-epfl/llm-adaptive-attacks](https://github.com/tml-epfl/llm-adaptive-attacks) | ✅       |
+| Custom Huggingface Datasets | markush1/LLM-Jailbreak-Classifier                                                                         | ✅          |
+| Local CSV Datasets      | -                                                                             | ✅          |
+
+
+
+Note: Please be aware that Agentic Security is designed as a safety scanner tool and not a foolproof solution. It cannot guarantee complete protection against all possible threats.
 
-<img width="100%" alt="booking-screen" src="https://res.cloudinary.com/do9qa2bqr/image/upload/v1713002396/1-ezgif.com-video-to-gif-converter_s2hsro.gif">
 
 ## 📦 Installation
 
 To get started with Agentic Security, simply install the package using pip:
 
 ```shell
 pip install agentic_security
@@ -59,14 +67,19 @@
 agentic_security --help
 
 
 agentic_security --port=PORT --host=HOST
 
 ```
 
+## UI 🧙
+
+
+<img width="100%" alt="booking-screen" src="https://res.cloudinary.com/do9qa2bqr/image/upload/v1713002396/1-ezgif.com-video-to-gif-converter_s2hsro.gif">
+
 ## LLM kwargs
 
 Agentic Security uses plain text HTTP spec like:
 
 ```http
 POST https://api.openai.com/v1/chat/completions
 Authorization: Bearer sk-xxxxxxxxx
```

### Comparing `agentic_security-0.1.4/agentic_security/__main__.py` & `agentic_security-0.1.5/agentic_security/__main__.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/agent.py` & `agentic_security-0.1.5/agentic_security/agent.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/http_spec.py` & `agentic_security-0.1.5/agentic_security/http_spec.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/lib.py` & `agentic_security-0.1.5/agentic_security/lib.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/probe_actor/fuzzer.py` & `agentic_security-0.1.5/agentic_security/probe_actor/fuzzer.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/probe_actor/refusal.py` & `agentic_security-0.1.5/agentic_security/probe_actor/refusal.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/probe_data/__init__.py` & `agentic_security-0.1.5/agentic_security/probe_data/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,14 +138,24 @@
         "approx_cost": 0.0,
         "source": "Github: https://github.com/leondz/garak#v0.9.0.1",
         "selected": False,
         "url": "https://github.com/leondz/garak2",
         "dynamic": True,
     },
     {
+        "dataset_name": "InspectAI",
+        "num_prompts": 0,
+        "tokens": 0,
+        "approx_cost": 0.0,
+        "source": "Github: https://github.com/UKGovernmentBEIS/inspect_ai",
+        "selected": False,
+        "url": "https://github.com/UKGovernmentBEIS/inspect_ai",
+        "dynamic": True,
+    },
+    {
         "dataset_name": "Custom CSV",
         "num_prompts": len(load_local_csv().prompts),
         "tokens": load_local_csv().tokens,
         "approx_cost": 0.0,
         "source": f"Local file dataset: {load_local_csv().metadata['src']}",
         "selected": len(load_local_csv().prompts),
         "url": "",
```

### Comparing `agentic_security-0.1.4/agentic_security/probe_data/data.py` & `agentic_security-0.1.5/agentic_security/probe_data/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from dataclasses import dataclass
 from functools import lru_cache
 
 import pandas as pd
 from loguru import logger
 
 from agentic_security.probe_data import stenography_fn
-from agentic_security.probe_data.modules import adaptive_attacks, garak_tool
+from agentic_security.probe_data.modules import (
+    adaptive_attacks,
+    garak_tool,
+    inspect_ai_tool,
+)
 
 IS_VERCEL = os.getenv("IS_VERCEL", "f") == "t"
 
 if not IS_VERCEL:
     from cache_to_disk import cache_to_disk
 else:
     # Read only fs in vercel, just mock no-op decorator
@@ -202,14 +206,19 @@
             "llm-adaptive-attacks", adaptive_attacks.Module(group).apply()
         ),
         "Garak": lambda: dataset_from_iterator(
             "Garak",
             garak_tool.Module(group, tools_inbox=tools_inbox).apply(),
             lazy=True,
         ),
+        "InspectAI": lambda: dataset_from_iterator(
+            "InspectAI",
+            inspect_ai_tool.Module(group, tools_inbox=tools_inbox).apply(),
+            lazy=True,
+        ),
         "GPT fuzzer": lambda: [],
     }
 
     dynamic_groups = []
     for dataset_name in dataset_names:
         if dataset_name in dynamic_datasets:
             logger.info(f"Loading {dataset_name}")
```

### Comparing `agentic_security-0.1.4/agentic_security/probe_data/modules/adaptive_attacks.py` & `agentic_security-0.1.5/agentic_security/probe_data/modules/adaptive_attacks.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/probe_data/modules/garak_tool.py` & `agentic_security-0.1.5/agentic_security/probe_data/modules/garak_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from loguru import logger
 
 # TODO: add probes modules
 
 
 class Module:
-
     def __init__(self, prompt_groups: [], tools_inbox: asyncio.Queue):
         self.tools_inbox = tools_inbox
         if not self.is_garak_installed():
             logger.error(
                 "Garak module is not installed. Please install it using 'pip install garak'"
             )
```

### Comparing `agentic_security-0.1.4/agentic_security/probe_data/modules/test_adaptive_attacks.py` & `agentic_security-0.1.5/agentic_security/probe_data/modules/test_adaptive_attacks.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/probe_data/stenography_fn.py` & `agentic_security-0.1.5/agentic_security/probe_data/stenography_fn.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/probe_data/test_data.py` & `agentic_security-0.1.5/agentic_security/probe_data/test_data.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/report_chart.py` & `agentic_security-0.1.5/agentic_security/report_chart.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/static/index.html` & `agentic_security-0.1.5/agentic_security/static/index.html`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/test_lib.py` & `agentic_security-0.1.5/agentic_security/test_lib.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/agentic_security/test_spec.py` & `agentic_security-0.1.5/agentic_security/test_spec.py`

 * *Files identical despite different names*

### Comparing `agentic_security-0.1.4/pyproject.toml` & `agentic_security-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentic_security"
-version = "0.1.4"
+version = "0.1.5"
 description = "Agentic LLM vulnerability scanner"
 authors = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 maintainers = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 repository = "https://github.com/msoedov/agentic_security"
 license = "MIT"
 readme = "Readme.md"
 keywords = [
@@ -24,15 +24,15 @@
 [tool.poetry.scripts]
 agentic_security = "agentic_security.__main__:entrypoint"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fastapi = ">=0.109.1,<0.112.0"
 uvicorn = ">=0.23.2,<0.30.0"
-fire = "^0.5.0"
+fire = ">=0.5,<0.7"
 loguru = "^0.7.2"
 httpx = ">=0.25.1,<0.28.0"
 cache-to-disk = "^2.0.0"
 pandas = ">=1.4,<3.0"
 datasets = "^1.14.0"
 tabulate = ">=0.8.9,<0.10.0"
 colorama = "^0.4.4"
@@ -40,15 +40,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.10.1,<25.0.0"
 mypy = "^1.6.1"
 httpx = ">=0.25.1,<0.28.0"
 pytest = ">=7.4.3,<9.0.0"
 pre-commit = "^3.5.0"
-inline-snapshot = "^0.8.0"
+inline-snapshot = ">=0.8,<0.10"
 langchain-groq = "^0.1.3"
 
 [tool.ruff]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `agentic_security-0.1.4/PKG-INFO` & `agentic_security-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentic_security
-Version: 0.1.4
+Version: 0.1.5
 Summary: Agentic LLM vulnerability scanner
 Home-page: https://github.com/msoedov/agentic_security
 License: MIT
 Keywords: LLM vulnerability scanner,llm security,llm adversarial attacks,prompt injection,prompt leakage,prompt injection attacks,prompt leakage prevention,llm vulnerabilities,owasp-llm-top-10
 Author: Alexander Miasoiedov
 Author-email: msoedov@gmail.com
 Maintainer: Alexander Miasoiedov
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cache-to-disk (>=2.0.0,<3.0.0)
 Requires-Dist: colorama (>=0.4.4,<0.5.0)
 Requires-Dist: datasets (>=1.14.0,<2.0.0)
 Requires-Dist: fastapi (>=0.109.1,<0.112.0)
-Requires-Dist: fire (>=0.5.0,<0.6.0)
+Requires-Dist: fire (>=0.5,<0.7)
 Requires-Dist: httpx (>=0.25.1,<0.28.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
 Requires-Dist: pandas (>=1.4,<3.0)
 Requires-Dist: tabulate (>=0.8.9,<0.10.0)
 Requires-Dist: uvicorn (>=0.23.2,<0.30.0)
 Project-URL: Repository, https://github.com/msoedov/agentic_security
@@ -54,19 +54,27 @@
 ## Features
 
 - Customizable Rule Sets or Agent based attacks🛠️
 - Comprehensive fuzzing for any LLMs 🧪
 - LLM API integration and stress testing 🛠️
 - Wide range of fuzzing and attack techniques 🌀
 
-Note: Please be aware that Agentic Security is designed as a safety scanner tool and not a foolproof solution. It cannot guarantee complete protection against all possible threats.
 
-## About the Project 🧙
+| Tool                    | Source                                                                        | Integrated |
+|-------------------------|-------------------------------------------------------------------------------|------------|
+| Garak                   | [leondz/garak](https://github.com/leondz/garak2)                              | ✅          |
+| InspectAI               | [UKGovernmentBEIS/inspect_ai](https://github.com/UKGovernmentBEIS/inspect_ai) | ✅          |
+| llm-adaptive-attacks    | [tml-epfl/llm-adaptive-attacks](https://github.com/tml-epfl/llm-adaptive-attacks) | ✅       |
+| Custom Huggingface Datasets | markush1/LLM-Jailbreak-Classifier                                                                         | ✅          |
+| Local CSV Datasets      | -                                                                             | ✅          |
+
+
+
+Note: Please be aware that Agentic Security is designed as a safety scanner tool and not a foolproof solution. It cannot guarantee complete protection against all possible threats.
 
-<img width="100%" alt="booking-screen" src="https://res.cloudinary.com/do9qa2bqr/image/upload/v1713002396/1-ezgif.com-video-to-gif-converter_s2hsro.gif">
 
 ## 📦 Installation
 
 To get started with Agentic Security, simply install the package using pip:
 
 ```shell
 pip install agentic_security
@@ -91,14 +99,19 @@
 agentic_security --help
 
 
 agentic_security --port=PORT --host=HOST
 
 ```
 
+## UI 🧙
+
+
+<img width="100%" alt="booking-screen" src="https://res.cloudinary.com/do9qa2bqr/image/upload/v1713002396/1-ezgif.com-video-to-gif-converter_s2hsro.gif">
+
 ## LLM kwargs
 
 Agentic Security uses plain text HTTP spec like:
 
 ```http
 POST https://api.openai.com/v1/chat/completions
 Authorization: Bearer sk-xxxxxxxxx
```

