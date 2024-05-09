# Comparing `tmp/openlit-1.1.3.tar.gz` & `tmp/openlit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlit-1.1.3.tar", max compression
+gzip compressed data, was "openlit-1.2.0.tar", max compression
```

## Comparing `openlit-1.1.3.tar` & `openlit-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0    11357 2024-05-02 08:18:53.598146 openlit-1.1.3/LICENSE
--rw-r--r--   0        0        0     9235 2024-05-02 08:18:53.598146 openlit-1.1.3/README.md
--rw-r--r--   0        0        0      966 2024-05-02 08:18:53.598146 openlit-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     4651 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/__helpers.py
--rw-r--r--   0        0        0     8932 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/__init__.py
--rw-r--r--   0        0        0     1955 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0    15993 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/anthropic/anthropic.py
--rw-r--r--   0        0        0    16035 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/anthropic/async_anthropic.py
--rw-r--r--   0        0        0     1540 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0    22278 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/bedrock/bedrock.py
--rw-r--r--   0        0        0     3253 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0    10374 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/chroma/chroma.py
--rw-r--r--   0        0        0     1920 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0    20348 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/cohere/cohere.py
--rw-r--r--   0        0        0     2531 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     7609 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/langchain/langchain.py
--rw-r--r--   0        0        0     3156 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/mistral/__init__.py
--rw-r--r--   0        0        0    21328 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/mistral/async_mistral.py
--rw-r--r--   0        0        0    21179 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/mistral/mistral.py
--rw-r--r--   0        0        0    16265 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0    46297 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/openai/async_azure_openai.py
--rw-r--r--   0        0        0    45841 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/openai/async_openai.py
--rw-r--r--   0        0        0    46091 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/openai/azure_openai.py
--rw-r--r--   0        0        0    46522 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/openai/openai.py
--rw-r--r--   0        0        0     2526 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     8732 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/pinecone/pinecone.py
--rw-r--r--   0        0        0     1478 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/transformers/__init__.py
--rw-r--r--   0        0        0     7592 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/instrumentation/transformers/transformers.py
--rw-r--r--   0        0        0     4291 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/otel/metrics.py
--rw-r--r--   0        0        0     3612 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/otel/tracing.py
--rw-r--r--   0        0        0     5724 2024-05-02 08:18:53.598146 openlit-1.1.3/src/openlit/semcov/__init__.py
--rw-r--r--   0        0        0    10535 1970-01-01 00:00:00.000000 openlit-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-09 06:25:35.217594 openlit-1.2.0/LICENSE
+-rw-r--r--   0        0        0     9235 2024-05-09 06:25:35.217594 openlit-1.2.0/README.md
+-rw-r--r--   0        0        0      966 2024-05-09 06:25:35.217594 openlit-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4651 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/__helpers.py
+-rw-r--r--   0        0        0     9077 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/__init__.py
+-rw-r--r--   0        0        0     1955 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0    15993 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/instrumentation/anthropic/anthropic.py
+-rw-r--r--   0        0        0    16035 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/instrumentation/anthropic/async_anthropic.py
+-rw-r--r--   0        0        0     1540 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0    22278 2024-05-09 06:25:35.217594 openlit-1.2.0/src/openlit/instrumentation/bedrock/bedrock.py
+-rw-r--r--   0        0        0     3253 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0    10374 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/chroma/chroma.py
+-rw-r--r--   0        0        0     1920 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0    20348 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/cohere/cohere.py
+-rw-r--r--   0        0        0     2531 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     7609 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/langchain/langchain.py
+-rw-r--r--   0        0        0     3156 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/mistral/__init__.py
+-rw-r--r--   0        0        0    21328 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/mistral/async_mistral.py
+-rw-r--r--   0        0        0    21179 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/mistral/mistral.py
+-rw-r--r--   0        0        0    16265 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0    46297 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/openai/async_azure_openai.py
+-rw-r--r--   0        0        0    45841 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/openai/async_openai.py
+-rw-r--r--   0        0        0    46091 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/openai/azure_openai.py
+-rw-r--r--   0        0        0    46522 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/openai/openai.py
+-rw-r--r--   0        0        0     2526 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     8732 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/pinecone/pinecone.py
+-rw-r--r--   0        0        0     1478 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/transformers/__init__.py
+-rw-r--r--   0        0        0     7592 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/transformers/transformers.py
+-rw-r--r--   0        0        0     6079 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/vertexai/__init__.py
+-rw-r--r--   0        0        0    52372 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/vertexai/async_vertexai.py
+-rw-r--r--   0        0        0    52125 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/instrumentation/vertexai/vertexai.py
+-rw-r--r--   0        0        0     4291 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/otel/metrics.py
+-rw-r--r--   0        0        0     3612 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/otel/tracing.py
+-rw-r--r--   0        0        0     5764 2024-05-09 06:25:35.221594 openlit-1.2.0/src/openlit/semcov/__init__.py
+-rw-r--r--   0        0        0    10535 1970-01-01 00:00:00.000000 openlit-1.2.0/PKG-INFO
```

### Comparing `openlit-1.1.3/LICENSE` & `openlit-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/README.md` & `openlit-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/pyproject.toml` & `openlit-1.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openlit"
-version = "1.1.3"
+version = "1.2.0"
 description = "OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects"
 authors = ["OpenLIT"]
 repository = "https://github.com/openlit/openlit/tree/main/openlit/python"
 readme = "README.md"
 homepage = "https://github.com/openlit/openlit/tree/main/openlit/python"
 keywords = ["OpenTelemetry", "otel", "otlp","llm", "tracing", "openai", "anthropic", "claude", "cohere", "llm monitoring", "observability", "monitoring", "gpt", "Generative AI", "chatGPT"]
```

### Comparing `openlit-1.1.3/src/openlit/__helpers.py` & `openlit-1.2.0/src/openlit/__helpers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/__init__.py` & `openlit-1.2.0/src/openlit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 # Instrumentors for various large language models.
 from openlit.instrumentation.openai import OpenAIInstrumentor
 from openlit.instrumentation.anthropic import AnthropicInstrumentor
 from openlit.instrumentation.cohere import CohereInstrumentor
 from openlit.instrumentation.mistral import MistralInstrumentor
 from openlit.instrumentation.bedrock import BedrockInstrumentor
+from openlit.instrumentation.vertexai import VertexAIInstrumentor
 from openlit.instrumentation.langchain import LangChainInstrumentor
 from openlit.instrumentation.chroma import ChromaInstrumentor
 from openlit.instrumentation.pinecone import PineconeInstrumentor
 from openlit.instrumentation.transformers import TransformersInstrumentor
 
 # Set up logging for error and information messages.
 logger = logging.getLogger(__name__)
@@ -135,23 +136,23 @@
         otlp_headers (Dict[str, str]): OTLP headers for exporter (Optional).
         disable_batch (bool): Flag to disable batch span processing (Optional).
         trace_content (bool): Flag to trace content (Optional).
         disabled_instrumentors (List[str]): Optional. List of instrumentor names to disable.
         disable_metrics (bool): Flag to disable metrics (Optional)
     """
     disabled_instrumentors = disabled_instrumentors if disabled_instrumentors else []
-
     # Check for invalid instrumentor names
 
     module_name_map = {
         "openai": "openai",
         "anthropic": "anthropic",  
         "cohere": "cohere",  
         "mistral": "mistralai",
         "bedrock": "boto3",
+        "vertexai": "vertexai",
         "langchain": "langchain",
         "chroma": "chromadb",
         "pinecone": "pinecone",
         "transformers": "transformers"
     }
 
     invalid_instrumentors = [name for name in disabled_instrumentors if name not in module_name_map]
@@ -191,14 +192,15 @@
         # Map instrumentor names to their instances
         instrumentor_instances = {
             "openai": OpenAIInstrumentor(),
             "anthropic": AnthropicInstrumentor(),
             "cohere": CohereInstrumentor(),
             "mistral": MistralInstrumentor(),
             "bedrock": BedrockInstrumentor(),
+            "vertexai": VertexAIInstrumentor(),
             "langchain": LangChainInstrumentor(),
             "chroma": ChromaInstrumentor(),
             "pinecone": PineconeInstrumentor(),
             "transformers": TransformersInstrumentor()
         }
 
         # Initialize and instrument only the enabled instrumentors
```

### Comparing `openlit-1.1.3/src/openlit/instrumentation/anthropic/__init__.py` & `openlit-1.2.0/src/openlit/instrumentation/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/anthropic/anthropic.py` & `openlit-1.2.0/src/openlit/instrumentation/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/anthropic/async_anthropic.py` & `openlit-1.2.0/src/openlit/instrumentation/anthropic/async_anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/bedrock/__init__.py` & `openlit-1.2.0/src/openlit/instrumentation/bedrock/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/bedrock/bedrock.py` & `openlit-1.2.0/src/openlit/instrumentation/bedrock/bedrock.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/chroma/__init__.py` & `openlit-1.2.0/src/openlit/instrumentation/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/chroma/chroma.py` & `openlit-1.2.0/src/openlit/instrumentation/chroma/chroma.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/cohere/__init__.py` & `openlit-1.2.0/src/openlit/instrumentation/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/cohere/cohere.py` & `openlit-1.2.0/src/openlit/instrumentation/cohere/cohere.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/langchain/__init__.py` & `openlit-1.2.0/src/openlit/instrumentation/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/langchain/langchain.py` & `openlit-1.2.0/src/openlit/instrumentation/langchain/langchain.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/mistral/__init__.py` & `openlit-1.2.0/src/openlit/instrumentation/mistral/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/mistral/async_mistral.py` & `openlit-1.2.0/src/openlit/instrumentation/mistral/async_mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/mistral/mistral.py` & `openlit-1.2.0/src/openlit/instrumentation/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/openai/__init__.py` & `openlit-1.2.0/src/openlit/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/openai/async_azure_openai.py` & `openlit-1.2.0/src/openlit/instrumentation/openai/async_azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/openai/async_openai.py` & `openlit-1.2.0/src/openlit/instrumentation/openai/async_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/openai/azure_openai.py` & `openlit-1.2.0/src/openlit/instrumentation/openai/azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/openai/openai.py` & `openlit-1.2.0/src/openlit/instrumentation/openai/openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/pinecone/__init__.py` & `openlit-1.2.0/src/openlit/instrumentation/pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/pinecone/pinecone.py` & `openlit-1.2.0/src/openlit/instrumentation/pinecone/pinecone.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/transformers/__init__.py` & `openlit-1.2.0/src/openlit/instrumentation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/instrumentation/transformers/transformers.py` & `openlit-1.2.0/src/openlit/instrumentation/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/otel/metrics.py` & `openlit-1.2.0/src/openlit/otel/metrics.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/otel/tracing.py` & `openlit-1.2.0/src/openlit/otel/tracing.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.3/src/openlit/semcov/__init__.py` & `openlit-1.2.0/src/openlit/semcov/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     GEN_AI_SYSTEM_HUGGING_FACE = "huggingface"
     GEN_AI_SYSTEM_OPENAI = "openai"
     GEN_AI_SYSTEM_AZURE_OPENAI = "azure_openai"
     GEN_AI_SYSTEM_ANTHROPIC = "anthropic"
     GEN_AI_SYSTEM_COHERE = "cohere"
     GEN_AI_SYSTEM_MISTRAL = "mistral"
     GEN_AI_SYSTEM_BEDROCK = "bedrock"
+    GEN_AI_SYSTEM_VERTEXAI = "vertexai"
     GEN_AI_SYSTEM_LANGCHAIN = "langchain"
 
     # Vector DB
     DB_REQUESTS = "db.total.requests"
     DB_SYSTEM = "db.system"
     DB_SYSTEM_CHROMA = "chroma"
     DB_SYSTEM_PINECONE = "pinecone"
```

### Comparing `openlit-1.1.3/PKG-INFO` & `openlit-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlit
-Version: 1.1.3
+Version: 1.2.0
 Summary: OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects
 Home-page: https://github.com/openlit/openlit/tree/main/openlit/python
 Keywords: OpenTelemetry,otel,otlp,llm,tracing,openai,anthropic,claude,cohere,llm monitoring,observability,monitoring,gpt,Generative AI,chatGPT
 Author: OpenLIT
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

