# Comparing `tmp/pytool-directory-0.0.1.tar.gz` & `tmp/pytool_directory-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytool-directory-0.0.1.tar", last modified: Wed Sep 13 03:01:32 2023, max compression
+gzip compressed data, was "pytool_directory-0.0.2.tar", last modified: Thu May  9 02:37:34 2024, max compression
```

## Comparing `pytool-directory-0.0.1.tar` & `pytool_directory-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 centos    (1000) centos    (1000)        0 2023-09-13 03:01:32.717048 pytool-directory-0.0.1/
--rw-r--r--   0 centos    (1000) centos    (1000)     1067 2023-08-25 01:03:59.000000 pytool-directory-0.0.1/LICENSE
--rw-r--r--   0 centos    (1000) centos    (1000)     2771 2023-09-13 03:01:32.716048 pytool-directory-0.0.1/PKG-INFO
--rw-r--r--   0 centos    (1000) centos    (1000)     1739 2023-09-12 09:06:10.000000 pytool-directory-0.0.1/README.md
--rw-r--r--   0 centos    (1000) centos    (1000)     1221 2023-09-13 02:58:37.000000 pytool-directory-0.0.1/pyproject.toml
--rw-r--r--   0 centos    (1000) centos    (1000)       38 2023-09-13 03:01:32.717048 pytool-directory-0.0.1/setup.cfg
-drwxr-xr-x   0 centos    (1000) centos    (1000)        0 2023-09-13 03:01:32.710048 pytool-directory-0.0.1/src/
-drwxr-xr-x   0 centos    (1000) centos    (1000)        0 2023-09-13 03:01:32.712048 pytool-directory-0.0.1/src/pytool_directory.egg-info/
--rw-r--r--   0 centos    (1000) centos    (1000)     2771 2023-09-13 03:01:32.000000 pytool-directory-0.0.1/src/pytool_directory.egg-info/PKG-INFO
--rw-r--r--   0 centos    (1000) centos    (1000)      429 2023-09-13 03:01:32.000000 pytool-directory-0.0.1/src/pytool_directory.egg-info/SOURCES.txt
--rw-r--r--   0 centos    (1000) centos    (1000)        1 2023-09-13 03:01:32.000000 pytool-directory-0.0.1/src/pytool_directory.egg-info/dependency_links.txt
--rw-r--r--   0 centos    (1000) centos    (1000)      150 2023-09-13 03:01:32.000000 pytool-directory-0.0.1/src/pytool_directory.egg-info/requires.txt
--rw-r--r--   0 centos    (1000) centos    (1000)       15 2023-09-13 03:01:32.000000 pytool-directory-0.0.1/src/pytool_directory.egg-info/top_level.txt
-drwxr-xr-x   0 centos    (1000) centos    (1000)        0 2023-09-13 03:01:32.714048 pytool-directory-0.0.1/src/tool_directory/
--rw-r--r--   0 centos    (1000) centos    (1000)      103 2023-09-12 01:22:43.000000 pytool-directory-0.0.1/src/tool_directory/__init__.py
--rw-r--r--   0 centos    (1000) centos    (1000)       49 2023-09-11 07:36:38.000000 pytool-directory-0.0.1/src/tool_directory/exceptions.py
--rw-r--r--   0 centos    (1000) centos    (1000)     4748 2023-09-12 08:11:27.000000 pytool-directory-0.0.1/src/tool_directory/loader.py
--rw-r--r--   0 centos    (1000) centos    (1000)     2169 2023-09-12 08:11:27.000000 pytool-directory-0.0.1/src/tool_directory/model.py
--rw-r--r--   0 centos    (1000) centos    (1000)       73 2023-09-11 07:36:38.000000 pytool-directory-0.0.1/src/tool_directory/prompt.py
--rw-r--r--   0 centos    (1000) centos    (1000)       93 2023-09-11 07:36:38.000000 pytool-directory-0.0.1/src/tool_directory/utils.py
+drwxr-xr-x   0 centos    (1000) centos    (1000)        0 2024-05-09 02:37:34.583597 pytool_directory-0.0.2/
+-rw-r--r--   0 centos    (1000) centos    (1000)     1067 2023-08-25 01:03:59.000000 pytool_directory-0.0.2/LICENSE
+-rw-r--r--   0 centos    (1000) centos    (1000)     3143 2024-05-09 02:37:34.582597 pytool_directory-0.0.2/PKG-INFO
+-rw-r--r--   0 centos    (1000) centos    (1000)     2001 2023-09-20 00:26:58.000000 pytool_directory-0.0.2/README.md
+-rw-r--r--   0 centos    (1000) centos    (1000)     1413 2024-05-09 00:18:32.000000 pytool_directory-0.0.2/pyproject.toml
+-rw-r--r--   0 centos    (1000) centos    (1000)       38 2024-05-09 02:37:34.583597 pytool_directory-0.0.2/setup.cfg
+drwxr-xr-x   0 centos    (1000) centos    (1000)        0 2024-05-09 02:37:34.574597 pytool_directory-0.0.2/src/
+drwxr-xr-x   0 centos    (1000) centos    (1000)        0 2024-05-09 02:37:34.579597 pytool_directory-0.0.2/src/pytool_directory.egg-info/
+-rw-r--r--   0 centos    (1000) centos    (1000)     3143 2024-05-09 02:37:34.000000 pytool_directory-0.0.2/src/pytool_directory.egg-info/PKG-INFO
+-rw-r--r--   0 centos    (1000) centos    (1000)      429 2024-05-09 02:37:34.000000 pytool_directory-0.0.2/src/pytool_directory.egg-info/SOURCES.txt
+-rw-r--r--   0 centos    (1000) centos    (1000)        1 2024-05-09 02:37:34.000000 pytool_directory-0.0.2/src/pytool_directory.egg-info/dependency_links.txt
+-rw-r--r--   0 centos    (1000) centos    (1000)      161 2024-05-09 02:37:34.000000 pytool_directory-0.0.2/src/pytool_directory.egg-info/requires.txt
+-rw-r--r--   0 centos    (1000) centos    (1000)       15 2024-05-09 02:37:34.000000 pytool_directory-0.0.2/src/pytool_directory.egg-info/top_level.txt
+drwxr-xr-x   0 centos    (1000) centos    (1000)        0 2024-05-09 02:37:34.578596 pytool_directory-0.0.2/src/tool_directory/
+-rw-r--r--   0 centos    (1000) centos    (1000)      103 2023-09-20 00:26:58.000000 pytool_directory-0.0.2/src/tool_directory/__init__.py
+-rw-r--r--   0 centos    (1000) centos    (1000)       49 2023-09-20 00:26:58.000000 pytool_directory-0.0.2/src/tool_directory/exceptions.py
+-rw-r--r--   0 centos    (1000) centos    (1000)     5525 2024-05-09 00:18:32.000000 pytool_directory-0.0.2/src/tool_directory/loader.py
+-rw-r--r--   0 centos    (1000) centos    (1000)     2483 2024-05-09 00:18:32.000000 pytool_directory-0.0.2/src/tool_directory/model.py
+-rw-r--r--   0 centos    (1000) centos    (1000)       73 2023-09-20 00:26:58.000000 pytool_directory-0.0.2/src/tool_directory/prompt.py
+-rw-r--r--   0 centos    (1000) centos    (1000)       93 2023-09-20 00:26:58.000000 pytool_directory-0.0.2/src/tool_directory/utils.py
```

### Comparing `pytool-directory-0.0.1/LICENSE` & `pytool_directory-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytool-directory-0.0.1/PKG-INFO` & `pytool_directory-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pytool-directory
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package to create langchain tool from the Tool Directory For LangChain.
 Author: Sheile
 License: MIT
 Project-URL: Homepage, https://github.com/dialogplay/pytool-directory
 Project-URL: Bug Tracker, https://github.com/dialogplay/pytool-directory/issues
+Project-URL: Source, https://github.com/dialogplay/pytool-directory
 Keywords: langchain,gpt,dialogplay
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
@@ -19,64 +20,67 @@
 Requires-Dist: PyYAML
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pyproject-flake8; extra == "dev"
 Requires-Dist: flake8-quotes; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-describe; extra == "dev"
 Requires-Dist: pytest-watcher; extra == "dev"
 Requires-Dist: requests-mock; extra == "dev"
 
 pytool-directory
 =========================
-Python package to create langchain tool from the [Tool Directory For LangChain](https://github.com/dialogplay/tool-directory/).
+[![Unittest](https://github.com/dialogplay/pytool-directory/actions/workflows/unittest.yaml/badge.svg)](https://github.com/dialogplay/pytool-directory/actions/workflows/unittest.yaml)
 
-Can create langchain tool from definition in the Tool Directory.
+Python package to create the [LangChain](https://github.com/langchain-ai/langchain) tool from the [Tool Directory For LangChain](https://github.com/dialogplay/tool-directory/).
+
+Can create LangChain tool from definition in the Tool Directory.
 
 Installation
 -------------------------
-```
+```bash
 pip install pytool-directory
 ```
 
 Usage
 -------------------------
 1. Search tools for your destination from [Tool Directory For LangChain](https://github.com/dialogplay/tool-directory).
 2. Load tools from the name of integration.
-```
+```python
 from tool_directory import ToolLoader
 tools = ToolLoader('openweather').get_tools(parameters={'appid': 'YOUR_APP_ID_FOR_OPENWEATHER'})
 ```
 3. Ask question to LLM with tools.
-```
+```python
 llm = ChatOpenAI(temperature=0, model_name='gpt-4')
 agent = initialize_agent(tools, llm, agent=AgentType.STRUCTURED_CHAT_ZERO_SHOT_REACT_DESCRIPTION, verbose=True)
 answer = agent('Please tell me about the temperature in tokyo.')
 ```
 
 Examples
 -------------------------
 ### [langchain_with_tools.py](https://github.com/dialogplay/pytool-directory/blob/main/examples/langchain_with_tools.py)
 Use a tool for the OpenWeather API to get the weather information on specified location.
 
 This example execute following conversation via ChatGPT.
 
-```
+```text
 User: Please tell me about the temperature in tokyo.
 Bot: The current temperature in Tokyo is 29.54°C, but it feels like 32.72°C. The minimum and maximum temperatures today are 27.74°C and 30.45°C respectively. The humidity is 64%.
 ```
 
 Contribution
 -------------------------
 1. Fork and clone repository.
 2. Install development dependencies.
+```bash
+pip install '.[dev]'
 ```
-pip install '.[dev]
-'```
 
 3. Install pre-commit hook for linter and formatter.
-```
+```bash
 pre-commit install
 ```
 
 4. Commit your changes and send pull request.
```

### Comparing `pytool-directory-0.0.1/README.md` & `pytool_directory-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 pytool-directory
 =========================
-Python package to create langchain tool from the [Tool Directory For LangChain](https://github.com/dialogplay/tool-directory/).
+[![Unittest](https://github.com/dialogplay/pytool-directory/actions/workflows/unittest.yaml/badge.svg)](https://github.com/dialogplay/pytool-directory/actions/workflows/unittest.yaml)
 
-Can create langchain tool from definition in the Tool Directory.
+Python package to create the [LangChain](https://github.com/langchain-ai/langchain) tool from the [Tool Directory For LangChain](https://github.com/dialogplay/tool-directory/).
+
+Can create LangChain tool from definition in the Tool Directory.
 
 Installation
 -------------------------
-```
+```bash
 pip install pytool-directory
 ```
 
 Usage
 -------------------------
 1. Search tools for your destination from [Tool Directory For LangChain](https://github.com/dialogplay/tool-directory).
 2. Load tools from the name of integration.
-```
+```python
 from tool_directory import ToolLoader
 tools = ToolLoader('openweather').get_tools(parameters={'appid': 'YOUR_APP_ID_FOR_OPENWEATHER'})
 ```
 3. Ask question to LLM with tools.
-```
+```python
 llm = ChatOpenAI(temperature=0, model_name='gpt-4')
 agent = initialize_agent(tools, llm, agent=AgentType.STRUCTURED_CHAT_ZERO_SHOT_REACT_DESCRIPTION, verbose=True)
 answer = agent('Please tell me about the temperature in tokyo.')
 ```
 
 Examples
 -------------------------
 ### [langchain_with_tools.py](https://github.com/dialogplay/pytool-directory/blob/main/examples/langchain_with_tools.py)
 Use a tool for the OpenWeather API to get the weather information on specified location.
 
 This example execute following conversation via ChatGPT.
 
-```
+```text
 User: Please tell me about the temperature in tokyo.
 Bot: The current temperature in Tokyo is 29.54°C, but it feels like 32.72°C. The minimum and maximum temperatures today are 27.74°C and 30.45°C respectively. The humidity is 64%.
 ```
 
 Contribution
 -------------------------
 1. Fork and clone repository.
 2. Install development dependencies.
+```bash
+pip install '.[dev]'
 ```
-pip install '.[dev]
-'```
 
 3. Install pre-commit hook for linter and formatter.
-```
+```bash
 pre-commit install
 ```
 
 4. Commit your changes and send pull request.
```

### Comparing `pytool-directory-0.0.1/pyproject.toml` & `pytool_directory-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytool-directory"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Sheile"},
 ]
 description = "Python package to create langchain tool from the Tool Directory For LangChain."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["langchain", "gpt", "dialogplay"]
@@ -24,22 +24,24 @@
   "langchain",
   "PyYAML",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dialogplay/pytool-directory"
 "Bug Tracker" = "https://github.com/dialogplay/pytool-directory/issues"
+"Source" = "https://github.com/dialogplay/pytool-directory"
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "flake8",
     "pyproject-flake8",
     "flake8-quotes",
     "pytest",
+    "pytest-cov",
     "pytest-describe",
     "pytest-watcher",
     "requests-mock",
 ]
 
 [tool.black]
 line-length = 120
@@ -54,7 +56,15 @@
 inline-quotes = "single"
 multiline-quotes = "single"
 docstring-quotes = "single"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 testpaths = ["tests"]
+addopts = "--cov"
+
+[tool.coverage.run]
+branch = true
+source = ["src"]
+
+[tool.coverage.report]
+show_missing = true
```

### Comparing `pytool-directory-0.0.1/src/pytool_directory.egg-info/PKG-INFO` & `pytool_directory-0.0.2/src/pytool_directory.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pytool-directory
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package to create langchain tool from the Tool Directory For LangChain.
 Author: Sheile
 License: MIT
 Project-URL: Homepage, https://github.com/dialogplay/pytool-directory
 Project-URL: Bug Tracker, https://github.com/dialogplay/pytool-directory/issues
+Project-URL: Source, https://github.com/dialogplay/pytool-directory
 Keywords: langchain,gpt,dialogplay
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
@@ -19,64 +20,67 @@
 Requires-Dist: PyYAML
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pyproject-flake8; extra == "dev"
 Requires-Dist: flake8-quotes; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-describe; extra == "dev"
 Requires-Dist: pytest-watcher; extra == "dev"
 Requires-Dist: requests-mock; extra == "dev"
 
 pytool-directory
 =========================
-Python package to create langchain tool from the [Tool Directory For LangChain](https://github.com/dialogplay/tool-directory/).
+[![Unittest](https://github.com/dialogplay/pytool-directory/actions/workflows/unittest.yaml/badge.svg)](https://github.com/dialogplay/pytool-directory/actions/workflows/unittest.yaml)
 
-Can create langchain tool from definition in the Tool Directory.
+Python package to create the [LangChain](https://github.com/langchain-ai/langchain) tool from the [Tool Directory For LangChain](https://github.com/dialogplay/tool-directory/).
+
+Can create LangChain tool from definition in the Tool Directory.
 
 Installation
 -------------------------
-```
+```bash
 pip install pytool-directory
 ```
 
 Usage
 -------------------------
 1. Search tools for your destination from [Tool Directory For LangChain](https://github.com/dialogplay/tool-directory).
 2. Load tools from the name of integration.
-```
+```python
 from tool_directory import ToolLoader
 tools = ToolLoader('openweather').get_tools(parameters={'appid': 'YOUR_APP_ID_FOR_OPENWEATHER'})
 ```
 3. Ask question to LLM with tools.
-```
+```python
 llm = ChatOpenAI(temperature=0, model_name='gpt-4')
 agent = initialize_agent(tools, llm, agent=AgentType.STRUCTURED_CHAT_ZERO_SHOT_REACT_DESCRIPTION, verbose=True)
 answer = agent('Please tell me about the temperature in tokyo.')
 ```
 
 Examples
 -------------------------
 ### [langchain_with_tools.py](https://github.com/dialogplay/pytool-directory/blob/main/examples/langchain_with_tools.py)
 Use a tool for the OpenWeather API to get the weather information on specified location.
 
 This example execute following conversation via ChatGPT.
 
-```
+```text
 User: Please tell me about the temperature in tokyo.
 Bot: The current temperature in Tokyo is 29.54°C, but it feels like 32.72°C. The minimum and maximum temperatures today are 27.74°C and 30.45°C respectively. The humidity is 64%.
 ```
 
 Contribution
 -------------------------
 1. Fork and clone repository.
 2. Install development dependencies.
+```bash
+pip install '.[dev]'
 ```
-pip install '.[dev]
-'```
 
 3. Install pre-commit hook for linter and formatter.
-```
+```bash
 pre-commit install
 ```
 
 4. Commit your changes and send pull request.
```

### Comparing `pytool-directory-0.0.1/src/tool_directory/loader.py` & `pytool_directory-0.0.2/src/tool_directory/loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import copy
+import itertools
 import logging
 from typing import Any, Dict, List, Union
 from urllib.parse import urljoin
 
 import requests
 import yaml
 from pydantic.v1 import BaseModel, Field, create_model
@@ -51,28 +53,28 @@
     def _fetch_openapi_spec(self, url: str):
         response = requests.get(url)
         response.raise_for_status()
 
         return yaml.load(response.content, Loader=yaml.SafeLoader)
 
     def _override(self, spec: Dict[str, Any], integration: Dict[str, Any], language: str) -> Dict[str, Any]:
-        for path, detail in integration.get('paths', []).items():
+        for path, detail in integration.get('paths', {}).items():
             for method, endpoint in detail.items():
                 try:
                     if endpoint.get('description'):
                         spec['paths'][path][method]['description'] = self._translate(endpoint['description'], language)
                     for parameter in endpoint.get('parameters', []):
                         if parameter.get('description'):
                             self._override_parameter(
                                 spec['paths'][path][method]['parameters'],
                                 _in=parameter['in'],
                                 name=parameter['name'],
                                 description=self._translate(parameter['description'], language),
                             )
-                except Exception:
+                except KeyError:
                     logging.warning('Failed to override OpenAPI spec', exc_info=True)
 
         return spec
 
     def _override_parameter(self, parameters: List[Dict[str, Any]], _in: str, name: str, description: str):
         for parameter in parameters:
             if parameter['in'] == _in and parameter['name'] == name:
@@ -102,18 +104,37 @@
 
         return endpoints
 
     def _create_args_schema(self, endpoint: Dict[str, Any]) -> BaseModel:
         # Check required flag and default value
         parameters = {
             x.get('name'): (str, Field()) if x.get('required') else (str, Field(None))
-            for x in endpoint.get('parameters', [])
+            for x in self._get_parameters(endpoint)
         }
 
         return create_model('ArgumentsSchema', **parameters)
 
     def _create_args_source(self, endpoint: Dict[str, Any]) -> Dict[str, str]:
         args_source = {}
-        for parameter in endpoint.get('parameters', []):
+        for parameter in self._get_parameters(endpoint):
             args_source[parameter.get('name')] = parameter.get('in')
 
         return args_source
+
+    def _get_parameters(self, endpoint: Dict[str, Any]):
+        parameters = copy.deepcopy(endpoint.get('parameters', []))
+        security_keys = list(itertools.chain.from_iterable([x.keys() for x in endpoint.get('security', [])]))
+        if not security_keys:
+            return parameters
+
+        security_schemes = self.spec.get('components', {}).get('securitySchemes', {})
+        for key in security_keys:
+            security_scheme = security_schemes.get(key)
+            parameters.append(
+                {
+                    'name': security_scheme['name'],
+                    'in': security_scheme['in'],
+                    'description': security_scheme['description'],
+                }
+            )
+
+        return parameters
```

### Comparing `pytool-directory-0.0.1/src/tool_directory/model.py` & `pytool_directory-0.0.2/src/tool_directory/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     def path_args(self):
         return [k for k, v in self.args_source.items() if v == 'path']
 
     @cached_property
     def query_args(self):
         return [k for k, v in self.args_source.items() if v == 'query']
 
+    @cached_property
+    def header_args(self):
+        return [k for k, v in self.args_source.items() if v == 'header']
+
 
 class OpenApiTool(StructuredTool):
     server: str
     endpoint: Endpoint
     parameters: Dict[str, str]
 
     def __init__(self, description: str, server: str, endpoint: Endpoint, parameters: Dict[str, str]):
@@ -47,20 +51,24 @@
             endpoint=endpoint,
             args_schema=endpoint.args_schema,
             func=self.request_by_spec,
             parameters=parameters,
         )
 
     def request_by_spec(self, **kwargs):
-        path_args = {k: v for k, v in kwargs.items() if k in self.endpoint.path_args}
-        query_args = {k: v for k, v in kwargs.items() if k in self.endpoint.query_args}
+        parameters = kwargs | self.parameters
+        path_args = {k: v for k, v in parameters.items() if k in self.endpoint.path_args}
+        query_args = {k: v for k, v in parameters.items() if k in self.endpoint.query_args}
+        header_args = {k: v for k, v in parameters.items() if k in self.endpoint.header_args}
         url = (self.server + self.endpoint.path).format(**path_args)
         if self.endpoint.method == 'get':
-            response = requests.get(url, params=query_args | self.parameters)
+            response = requests.get(url, headers=header_args, params=query_args)
         elif self.endpoint.method == 'post':
-            response = requests.post(url, data=query_args | self.parameters)
+            response = requests.post(url, headers=header_args, data=query_args)
+        else:
+            return None
 
         response.raise_for_status()
         try:
             return response.json()
         except Exception:
             return response.text
```

