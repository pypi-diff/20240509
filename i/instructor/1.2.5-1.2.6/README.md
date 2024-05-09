# Comparing `tmp/instructor-1.2.5.tar.gz` & `tmp/instructor-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructor-1.2.5.tar", max compression
+gzip compressed data, was "instructor-1.2.6.tar", max compression
```

## Comparing `instructor-1.2.5.tar` & `instructor-1.2.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2024-05-01 22:11:43.174889 instructor-1.2.5/LICENSE
--rw-r--r--   0        0        0     9716 2024-05-01 22:11:43.174889 instructor-1.2.5/README.md
--rw-r--r--   0        0        0     1450 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/_types/__init__.py
--rw-r--r--   0        0        0      654 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/_types/_alias.py
--rw-r--r--   0        0        0        0 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/cli/cli.py
--rw-r--r--   0        0        0     3865 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/cli/files.py
--rw-r--r--   0        0        0     5441 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/cli/hub.py
--rw-r--r--   0        0        0     8314 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/cli/jobs.py
--rw-r--r--   0        0        0     6441 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/cli/usage.py
--rw-r--r--   0        0        0    13256 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/client.py
--rw-r--r--   0        0        0     2573 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/client_anthropic.py
--rw-r--r--   0        0        0     2419 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/client_cohere.py
--rw-r--r--   0        0        0     1391 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/client_groq.py
--rw-r--r--   0        0        0     1727 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/client_mistral.py
--rw-r--r--   0        0        0     9579 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/distil.py
--rw-r--r--   0        0        0      424 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/__init__.py
--rw-r--r--   0        0        0     2927 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/citation.py
--rw-r--r--   0        0        0     8079 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/iterable.py
--rw-r--r--   0        0        0     2169 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/maybe.py
--rw-r--r--   0        0        0     2562 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/parallel.py
--rw-r--r--   0        0        0    10922 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/partial.py
--rw-r--r--   0        0        0     1879 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/simple_type.py
--rw-r--r--   0        0        0     4360 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/validators.py
--rw-r--r--   0        0        0      346 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/exceptions.py
--rw-r--r--   0        0        0     8724 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/function_calls.py
--rw-r--r--   0        0        0      852 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/mode.py
--rw-r--r--   0        0        0     4969 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/patch.py
--rw-r--r--   0        0        0    13501 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/process_response.py
--rw-r--r--   0        0        0        1 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/py.typed
--rw-r--r--   0        0        0     9502 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/retry.py
--rw-r--r--   0        0        0     6668 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/utils.py
--rw-r--r--   0        0        0     2799 2024-05-01 22:11:43.246888 instructor-1.2.5/pyproject.toml
--rw-r--r--   0        0        0    11713 1970-01-01 00:00:00.000000 instructor-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-09 04:29:33.847049 instructor-1.2.6/LICENSE
+-rw-r--r--   0        0        0     9716 2024-05-09 04:29:33.847049 instructor-1.2.6/README.md
+-rw-r--r--   0        0        0     1450 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/_types/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/_types/_alias.py
+-rw-r--r--   0        0        0        0 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/cli/cli.py
+-rw-r--r--   0        0        0     3865 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/cli/files.py
+-rw-r--r--   0        0        0     5441 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/cli/hub.py
+-rw-r--r--   0        0        0     8314 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/cli/jobs.py
+-rw-r--r--   0        0        0     6441 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/cli/usage.py
+-rw-r--r--   0        0        0    13256 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/client.py
+-rw-r--r--   0        0        0     2573 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/client_anthropic.py
+-rw-r--r--   0        0        0     2419 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/client_cohere.py
+-rw-r--r--   0        0        0     1391 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/client_groq.py
+-rw-r--r--   0        0        0     1727 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/client_mistral.py
+-rw-r--r--   0        0        0     9579 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/distil.py
+-rw-r--r--   0        0        0      424 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/__init__.py
+-rw-r--r--   0        0        0     2927 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/citation.py
+-rw-r--r--   0        0        0     8079 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/iterable.py
+-rw-r--r--   0        0        0     2169 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/maybe.py
+-rw-r--r--   0        0        0     2562 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/parallel.py
+-rw-r--r--   0        0        0    10922 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/partial.py
+-rw-r--r--   0        0        0     1879 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/simple_type.py
+-rw-r--r--   0        0        0     4360 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/validators.py
+-rw-r--r--   0        0        0      346 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/exceptions.py
+-rw-r--r--   0        0        0     8724 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/function_calls.py
+-rw-r--r--   0        0        0      852 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/mode.py
+-rw-r--r--   0        0        0     4969 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/patch.py
+-rw-r--r--   0        0        0    13501 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/process_response.py
+-rw-r--r--   0        0        0        1 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/py.typed
+-rw-r--r--   0        0        0     9502 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/retry.py
+-rw-r--r--   0        0        0     6507 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/utils.py
+-rw-r--r--   0        0        0     2799 2024-05-09 04:29:33.923049 instructor-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0    11713 1970-01-01 00:00:00.000000 instructor-1.2.6/PKG-INFO
```

### Comparing `instructor-1.2.5/LICENSE` & `instructor-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/README.md` & `instructor-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/__init__.py` & `instructor-1.2.6/instructor/__init__.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/_types/_alias.py` & `instructor-1.2.6/instructor/_types/_alias.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/cli/cli.py` & `instructor-1.2.6/instructor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/cli/files.py` & `instructor-1.2.6/instructor/cli/files.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/cli/hub.py` & `instructor-1.2.6/instructor/cli/hub.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/cli/jobs.py` & `instructor-1.2.6/instructor/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/cli/usage.py` & `instructor-1.2.6/instructor/cli/usage.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/client.py` & `instructor-1.2.6/instructor/client.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/client_anthropic.py` & `instructor-1.2.6/instructor/client_anthropic.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/client_cohere.py` & `instructor-1.2.6/instructor/client_cohere.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/client_groq.py` & `instructor-1.2.6/instructor/client_groq.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/client_mistral.py` & `instructor-1.2.6/instructor/client_mistral.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/distil.py` & `instructor-1.2.6/instructor/distil.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/dsl/citation.py` & `instructor-1.2.6/instructor/dsl/citation.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/dsl/iterable.py` & `instructor-1.2.6/instructor/dsl/iterable.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/dsl/maybe.py` & `instructor-1.2.6/instructor/dsl/maybe.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/dsl/parallel.py` & `instructor-1.2.6/instructor/dsl/parallel.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/dsl/partial.py` & `instructor-1.2.6/instructor/dsl/partial.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/dsl/simple_type.py` & `instructor-1.2.6/instructor/dsl/simple_type.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/dsl/validators.py` & `instructor-1.2.6/instructor/dsl/validators.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/function_calls.py` & `instructor-1.2.6/instructor/function_calls.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/mode.py` & `instructor-1.2.6/instructor/mode.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/patch.py` & `instructor-1.2.6/instructor/patch.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/process_response.py` & `instructor-1.2.6/instructor/process_response.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/retry.py` & `instructor-1.2.6/instructor/retry.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.5/instructor/utils.py` & `instructor-1.2.6/instructor/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from __future__ import annotations
 
 import inspect
 import json
 import logging
+from collections.abc import AsyncGenerator, Generator, Iterable
 from typing import (
+    TYPE_CHECKING,
+    Any,
     Callable,
     Generic,
     Protocol,
     TypeVar,
 )
-from collections.abc import Generator, Iterable, AsyncGenerator
-from typing import Callable, Protocol, TypeVar
-from collections.abc import Generator, Iterable, AsyncGenerator
-from openai.types.completion_usage import CompletionUsage
-from anthropic.types import Usage as AnthropicUsage
-from typing import Any
+
 from openai.types import CompletionUsage as OpenAIUsage
 from openai.types.chat import (
     ChatCompletion,
     ChatCompletionMessage,
     ChatCompletionMessageParam,
 )
 
+if TYPE_CHECKING:
+    from anthropic.types import Usage as AnthropicUsage
+
+
 logger = logging.getLogger("instructor")
 R_co = TypeVar("R_co", covariant=True)
 T_Model = TypeVar("T_Model", bound="Response")
 
 from enum import Enum
 
 
@@ -106,20 +108,18 @@
                     break  # Cease yielding upon closing the current JSON object
             elif capturing:
                 yield char
 
 
 def update_total_usage(
     response: T_Model,
-    total_usage: CompletionUsage | AnthropicUsage,
+    total_usage: OpenAIUsage | AnthropicUsage,
 ) -> T_Model | ChatCompletion:
     response_usage = getattr(response, "usage", None)
-    if isinstance(response_usage, OpenAIUsage) and isinstance(
-        total_usage, CompletionUsage
-    ):
+    if isinstance(response_usage, OpenAIUsage) and isinstance(total_usage, OpenAIUsage):
         total_usage.completion_tokens += response_usage.completion_tokens or 0
         total_usage.prompt_tokens += response_usage.prompt_tokens or 0
         total_usage.total_tokens += response_usage.total_tokens or 0
         response.usage = total_usage  # Replace each response usage with the total usage
         return response
 
     # Anthropic usage.
```

### Comparing `instructor-1.2.5/pyproject.toml` & `instructor-1.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "instructor"
-version = "1.2.5"
+version = "1.2.6"
 description = "structured outputs for llm"
 authors = ["Jason Liu <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "instructor"}]
 repository = "https://github.com/jxnl/instructor"
```

### Comparing `instructor-1.2.5/PKG-INFO` & `instructor-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructor
-Version: 1.2.5
+Version: 1.2.6
 Summary: structured outputs for llm
 Home-page: https://github.com/jxnl/instructor
 License: MIT
 Author: Jason Liu
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

