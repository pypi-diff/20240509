# Comparing `tmp/scrapwithgpt-0.0.3.tar.gz` & `tmp/scrapwithgpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapwithgpt-0.0.3.tar", last modified: Thu May  9 12:38:57 2024, max compression
+gzip compressed data, was "scrapwithgpt-0.0.4.tar", last modified: Thu May  9 12:44:33 2024, max compression
```

## Comparing `scrapwithgpt-0.0.3.tar` & `scrapwithgpt-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:38:57.509075 scrapwithgpt-0.0.3/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:38:57.508856 scrapwithgpt-0.0.3/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.0.3/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:38:57.507892 scrapwithgpt-0.0.3/scrapwithgpt/
--rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.0.3/scrapwithgpt/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)     3421 2024-05-09 11:06:44.000000 scrapwithgpt-0.0.3/scrapwithgpt/config.py
--rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.3/scrapwithgpt/oai.py
--rw-r--r--   0 henry      (501) staff       (20)     4245 2024-05-09 12:38:48.000000 scrapwithgpt-0.0.3/scrapwithgpt/prompts.py
--rw-r--r--   0 henry      (501) staff       (20)     4445 2024-05-09 12:32:25.000000 scrapwithgpt-0.0.3/scrapwithgpt/scrap.py
--rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.3/scrapwithgpt/utils.py
--rw-r--r--   0 henry      (501) staff       (20)    13377 2024-05-09 06:39:55.000000 scrapwithgpt-0.0.3/scrapwithgpt/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:38:57.508643 scrapwithgpt-0.0.3/scrapwithgpt.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:38:57.000000 scrapwithgpt-0.0.3/scrapwithgpt.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 12:38:57.000000 scrapwithgpt-0.0.3/scrapwithgpt.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 12:38:57.000000 scrapwithgpt-0.0.3/scrapwithgpt.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 12:38:57.000000 scrapwithgpt-0.0.3/scrapwithgpt.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 12:38:57.000000 scrapwithgpt-0.0.3/scrapwithgpt.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 12:38:57.509120 scrapwithgpt-0.0.3/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 12:38:55.000000 scrapwithgpt-0.0.3/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:44:33.916159 scrapwithgpt-0.0.4/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:44:33.915925 scrapwithgpt-0.0.4/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.0.4/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:44:33.914898 scrapwithgpt-0.0.4/scrapwithgpt/
+-rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.0.4/scrapwithgpt/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)     3449 2024-05-09 12:44:16.000000 scrapwithgpt-0.0.4/scrapwithgpt/config.py
+-rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.4/scrapwithgpt/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)     4332 2024-05-09 12:42:05.000000 scrapwithgpt-0.0.4/scrapwithgpt/prompts.py
+-rw-r--r--   0 henry      (501) staff       (20)     4428 2024-05-09 12:44:25.000000 scrapwithgpt-0.0.4/scrapwithgpt/scrap.py
+-rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.4/scrapwithgpt/utils.py
+-rw-r--r--   0 henry      (501) staff       (20)    13377 2024-05-09 06:39:55.000000 scrapwithgpt-0.0.4/scrapwithgpt/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:44:33.915695 scrapwithgpt-0.0.4/scrapwithgpt.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:44:33.000000 scrapwithgpt-0.0.4/scrapwithgpt.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 12:44:33.000000 scrapwithgpt-0.0.4/scrapwithgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 12:44:33.000000 scrapwithgpt-0.0.4/scrapwithgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 12:44:33.000000 scrapwithgpt-0.0.4/scrapwithgpt.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 12:44:33.000000 scrapwithgpt-0.0.4/scrapwithgpt.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 12:44:33.916202 scrapwithgpt-0.0.4/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 12:41:08.000000 scrapwithgpt-0.0.4/setup.py
```

### Comparing `scrapwithgpt-0.0.3/PKG-INFO` & `scrapwithgpt-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.0.3/scrapwithgpt/config.py` & `scrapwithgpt-0.0.4/scrapwithgpt/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 )
 MODEL_GPT4_STABLE = r"gpt-4"  # 8K context window and 4,096 output
 
 MODEL_EMB_LARGE = r"text-embedding-3-large"
 MODEL_EMB_SMALL = r"text-embedding-3-small"
 
 MAX_TOKEN_OUTPUT_DEFAULT = 300
+MAX_TOKEN_GPT4_RESULT = 500
 MAX_TOKEN_OUTPUT_DEFAULT_HUGE = 3000
 MAX_TOKEN_OUTPUT_FILTER = 10000
 
 MAX_TOKEN_WINDOW_GPT4_TURBO = 128000
 MAX_TOKEN_WINDOW_GPT35_TURBO = 16385
 MAX_TOKEN_WINDOW_GPT4 = 8192
 MAX_TOKEN_OUTPUT_GPT3 = 4096
```

### Comparing `scrapwithgpt-0.0.3/scrapwithgpt/oai.py` & `scrapwithgpt-0.0.4/scrapwithgpt/oai.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.3/scrapwithgpt/prompts.py` & `scrapwithgpt-0.0.4/scrapwithgpt/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,21 +37,22 @@
         You are a rigorous analyst. 
         The user will provide you with content extracted from a website. You must analyze this content and return a JSON object with the information filled when available.
         ONLY use the content available, NEVER INVENT anything and follow strictly the below Instructions:
 
         ### Instructions: 
         1. Take your time and think step by step.
         2. Review and keep in mind ALL the fields of the below json structure: {json_output}
-        3. Go through the content provided by the user and fill the json accordingly. 
+        3. Go through the content provided by the user and try your best to fill the json accordingly. 
         4. If the information is NOT in the content AT ALL, put NA.
         {example}
         ### Important considerations:
         - Follow strictly the Instructions. 
         - Remember that you must construct a JSON object with the provided keys, populated with the relevant information. If an information is not available at ALL or does not apply, use 'NA' for those fields.
         - Return the JSON and the JSON only. Do not preface by anything not even ```json before. 
+        - Do your best, my job depends on the quality of your output.
         """)
 
 def gen_role_summarizer() -> str:
     """
     Quick prompt for summarization. 
     """
     return remove_excess("""
```

### Comparing `scrapwithgpt-0.0.3/scrapwithgpt/scrap.py` & `scrapwithgpt-0.0.4/scrapwithgpt/scrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #   Main function to scrap the page according to the criteria specified.
 
 from .prompts import gen_prompt_filter, gen_prompt_result, gen_role_summarizer
-from .config import MAX_TOKEN_OUTPUT_DEFAULT_HUGE, JSON_EXAMPLE_VC, JSON_OUTPUT_VC, DEFAULT_FILTERING_CRITERIA, MAX_TOKEN_OUTPUT_GPT3
+from .config import MAX_TOKEN_OUTPUT_DEFAULT_HUGE, MAX_TOKEN_OUTPUT_GPT3, MAX_TOKEN_GPT4_RESULT
 from .web import crawl_website, fetch_content_url, clean_url_to_filename
+from .oai import ask_question_gpt, calculate_token, ask_question_gpt4
 from .utils import get_now, log_issue
-from .oai import ask_question_gpt, calculate_token
+
 
 from typing import Optional
 import json
 import os
 
 def smartscrap(url:str, desired_output:str=None, example_output:str=None, filtering_criteria:str=None, summarization:bool=True, full_website:bool=True, verbose:bool=None) -> Optional[str]:
     """
@@ -51,16 +52,16 @@
             elif "false" in filtered_content[:10].lower(): 
                 if verbose: print(f"The website is NOT relevant according to the Criteria. Response: {filtered_content} - END")
                 return
         if summarization:
             if verbose: print(f"👷‍♂️ Generating a summary")   
             summary = ask_question_gpt(filtered_content, gen_role_summarizer(), max_tokens=MAX_TOKEN_OUTPUT_DEFAULT_HUGE,  verbose=False)
         
-        if verbose: print(f"👷‍♂️ Getting the requested data")  
-        result = ask_question_gpt(filtered_content, gen_prompt_result(desired_output, example_output), max_tokens=MAX_TOKEN_OUTPUT_DEFAULT_HUGE,  verbose=False)
+        if verbose: print(f"👷‍♂️ Using GPT 4 to  the requested data")  
+        result = ask_question_gpt4(filtered_content, gen_prompt_result(desired_output, example_output), max_tokens=MAX_TOKEN_GPT4_RESULT,  verbose=False)
         if result:
             title = f"scrapwithgpt_{clean_url_to_filename(url)}.txt"
             if os.path.exists(title):
                 title = f"scrapwithgpt_{clean_url_to_filename(url)}_{get_now(True)}.txt" # To avoid overwriting
             if summary:
                 final_content = f"### SUMMARY of {url}:\n" + summary.replace(".", ".\n") + "\n\n" 
             final_content += f"### RESULT for {url}:\n" + result
```

### Comparing `scrapwithgpt-0.0.3/scrapwithgpt/utils.py` & `scrapwithgpt-0.0.4/scrapwithgpt/utils.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.3/scrapwithgpt/web.py` & `scrapwithgpt-0.0.4/scrapwithgpt/web.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.3/scrapwithgpt.egg-info/PKG-INFO` & `scrapwithgpt-0.0.4/scrapwithgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.0.3/setup.py` & `scrapwithgpt-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapwithgpt",
-    version="0.0.3", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.0.4", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/scrapwithgpt',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

