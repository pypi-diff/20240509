# Comparing `tmp/athena_starship-0.0.2.tar.gz` & `tmp/athena_starship-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_starship-0.0.2.tar", max compression
+gzip compressed data, was "athena_starship-0.0.3.tar", max compression
```

## Comparing `athena_starship-0.0.2.tar` & `athena_starship-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        1 2024-05-08 23:20:52.861407 athena_starship-0.0.2/LICENSE
--rw-r--r--   0        0        0     1290 2024-05-08 23:56:29.101861 athena_starship-0.0.2/README.md
--rw-r--r--   0        0        0      116 2024-05-08 23:58:01.824713 athena_starship-0.0.2/athena_starship/__init__.py
--rw-r--r--   0        0        0     2375 2024-05-08 23:34:28.241612 athena_starship-0.0.2/athena_starship/data_connectors.py
--rw-r--r--   0        0        0     1010 2024-05-08 23:20:52.885141 athena_starship-0.0.2/athena_starship/ghost_datasource_urls.py
--rw-r--r--   0        0        0      158 2024-05-08 23:42:10.513806 athena_starship-0.0.2/athena_starship/llama.py
--rw-r--r--   0        0        0     5403 2024-05-08 23:39:54.739467 athena_starship-0.0.2/athena_starship/memory.py
--rw-r--r--   0        0        0     1822 2024-05-08 23:20:52.886160 athena_starship-0.0.2/athena_starship/tool_schemas.py
--rw-r--r--   0        0        0        0 2024-05-08 23:27:03.908694 athena_starship-0.0.2/athena_starship/tools/__init__.py
--rw-r--r--   0        0        0     2932 2024-05-08 23:33:29.346598 athena_starship-0.0.2/athena_starship/tools/google_calendar.py
--rw-r--r--   0        0        0     2478 2024-05-08 23:20:52.886402 athena_starship-0.0.2/athena_starship/youtube_utils.py
--rw-r--r--   0        0        0     1341 2024-05-08 23:58:08.022029 athena_starship-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2014 1970-01-01 00:00:00.000000 athena_starship-0.0.2/setup.py
--rw-r--r--   0        0        0     2207 1970-01-01 00:00:00.000000 athena_starship-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        1 2024-05-08 23:20:52.861407 athena_starship-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1290 2024-05-08 23:56:29.101861 athena_starship-0.0.3/README.md
+-rw-r--r--   0        0        0      116 2024-05-08 23:58:01.824713 athena_starship-0.0.3/athena_starship/__init__.py
+-rw-r--r--   0        0        0     2375 2024-05-08 23:34:28.241612 athena_starship-0.0.3/athena_starship/data_connectors.py
+-rw-r--r--   0        0        0     1010 2024-05-08 23:20:52.885141 athena_starship-0.0.3/athena_starship/ghost_datasource_urls.py
+-rw-r--r--   0        0        0      158 2024-05-08 23:42:10.513806 athena_starship-0.0.3/athena_starship/llama.py
+-rw-r--r--   0        0        0     5403 2024-05-08 23:39:54.739467 athena_starship-0.0.3/athena_starship/memory.py
+-rw-r--r--   0        0        0     1822 2024-05-08 23:20:52.886160 athena_starship-0.0.3/athena_starship/tool_schemas.py
+-rw-r--r--   0        0        0        0 2024-05-08 23:27:03.908694 athena_starship-0.0.3/athena_starship/tools/__init__.py
+-rw-r--r--   0        0        0     2932 2024-05-08 23:33:29.346598 athena_starship-0.0.3/athena_starship/tools/google_calendar.py
+-rw-r--r--   0        0        0     2478 2024-05-08 23:20:52.886402 athena_starship-0.0.3/athena_starship/youtube_utils.py
+-rw-r--r--   0        0        0     1345 2024-05-09 00:01:28.203687 athena_starship-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2021 1970-01-01 00:00:00.000000 athena_starship-0.0.3/setup.py
+-rw-r--r--   0        0        0     2217 1970-01-01 00:00:00.000000 athena_starship-0.0.3/PKG-INFO
```

### Comparing `athena_starship-0.0.2/README.md` & `athena_starship-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.2/athena_starship/data_connectors.py` & `athena_starship-0.0.3/athena_starship/data_connectors.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.2/athena_starship/ghost_datasource_urls.py` & `athena_starship-0.0.3/athena_starship/ghost_datasource_urls.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.2/athena_starship/memory.py` & `athena_starship-0.0.3/athena_starship/memory.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.2/athena_starship/tool_schemas.py` & `athena_starship-0.0.3/athena_starship/tool_schemas.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.2/athena_starship/tools/google_calendar.py` & `athena_starship-0.0.3/athena_starship/tools/google_calendar.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.2/athena_starship/youtube_utils.py` & `athena_starship-0.0.3/athena_starship/youtube_utils.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.2/pyproject.toml` & `athena_starship-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "athena-starship"
-version = "0.0.2"
+version = "0.0.3"
 description = "Paper - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/Starship-Ventures/Athena"
 documentation = "https://github.com/Starship-Ventures/Athena"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/Starship-Ventures/Athena"
@@ -19,15 +19,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-swarms = "*"
+swarms = "4.9.3"
 
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.6"
 types-toml = "^0.10.8.1"
 types-redis = "^4.3.21.6"
 types-pytz = "^2023.3.0.0"
```

### Comparing `athena_starship-0.0.2/setup.py` & `athena_starship-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['athena_starship', 'athena_starship.tools']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['swarms']
+['swarms==4.9.3']
 
 setup_kwargs = {
     'name': 'athena-starship',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Paper - Pytorch',
     'long_description': '# Athena\n\n## Install\n`$ pip install athena-starship`\n\n## Usage\n```bash\npython3 sam_altman.py\n```\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent\nfrom athena_starship.llama import llama\nfrom athena_starship.memory import ChromaDB\nfrom athena_starship.tools.google_calendar import calendar\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initilaize the chromadb client\nchromadb = ChromaDB(\n    metric="cosine",\n    verbose=True,\n    n_results=3,\n)\n\n## Initialize the workflow\nagent = Agent(\n    llm=llama,\n    agent_name="Sam Altman",\n    agent_description="Sam Altman Agent, CEO of OpenAI.",\n    system_prompt="You\'re Sam Altman, CEO of OpenAI.",\n    max_loops="auto",\n    interactive=True,\n    autosave=True,\n    dashboard=True,\n    long_term_memory=chromadb,\n    stopping_token="<DONE>",\n    verbose=True,\n    tools=[calendar],\n)\n\n# Run the workflow on a task\nagent.run(\n    "What are the 3 traits you look for before investing in a seed"\n    " stage startup?"\n)\n\n```\n\n# License\nMIT\n\n\n# Todo\n- [ ] Make csv of few shot prompt examples for various tool usages\n- [ ] Make tools for airtable, google calendar, notion, gmail\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Starship-Ventures/Athena',
```

### Comparing `athena_starship-0.0.2/PKG-INFO` & `athena_starship-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-starship
-Version: 0.0.2
+Version: 0.0.3
 Summary: Paper - Pytorch
 Home-page: https://github.com/Starship-Ventures/Athena
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Dist: swarms
+Requires-Dist: swarms (==4.9.3)
 Project-URL: Documentation, https://github.com/Starship-Ventures/Athena
 Project-URL: Repository, https://github.com/Starship-Ventures/Athena
 Description-Content-Type: text/markdown
 
 # Athena
 
 ## Install
```

