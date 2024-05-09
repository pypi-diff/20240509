# Comparing `tmp/scrapwithgpt-0.0.5.tar.gz` & `tmp/scrapwithgpt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapwithgpt-0.0.5.tar", last modified: Thu May  9 12:53:08 2024, max compression
+gzip compressed data, was "scrapwithgpt-0.0.6.tar", last modified: Thu May  9 12:58:56 2024, max compression
```

## Comparing `scrapwithgpt-0.0.5.tar` & `scrapwithgpt-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:53:08.611301 scrapwithgpt-0.0.5/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:53:08.611048 scrapwithgpt-0.0.5/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.0.5/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:53:08.608670 scrapwithgpt-0.0.5/scrapwithgpt/
--rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.0.5/scrapwithgpt/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)     3449 2024-05-09 12:44:16.000000 scrapwithgpt-0.0.5/scrapwithgpt/config.py
--rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.5/scrapwithgpt/oai.py
--rw-r--r--   0 henry      (501) staff       (20)     3928 2024-05-09 12:52:49.000000 scrapwithgpt-0.0.5/scrapwithgpt/prompts.py
--rw-r--r--   0 henry      (501) staff       (20)     4495 2024-05-09 12:51:34.000000 scrapwithgpt-0.0.5/scrapwithgpt/scrap.py
--rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.5/scrapwithgpt/utils.py
--rw-r--r--   0 henry      (501) staff       (20)    13377 2024-05-09 06:39:55.000000 scrapwithgpt-0.0.5/scrapwithgpt/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:53:08.610788 scrapwithgpt-0.0.5/scrapwithgpt.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:53:08.000000 scrapwithgpt-0.0.5/scrapwithgpt.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 12:53:08.000000 scrapwithgpt-0.0.5/scrapwithgpt.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 12:53:08.000000 scrapwithgpt-0.0.5/scrapwithgpt.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 12:53:08.000000 scrapwithgpt-0.0.5/scrapwithgpt.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 12:53:08.000000 scrapwithgpt-0.0.5/scrapwithgpt.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 12:53:08.611349 scrapwithgpt-0.0.5/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 12:52:55.000000 scrapwithgpt-0.0.5/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:58:56.775518 scrapwithgpt-0.0.6/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:58:56.775305 scrapwithgpt-0.0.6/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.0.6/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:58:56.774245 scrapwithgpt-0.0.6/scrapwithgpt/
+-rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.0.6/scrapwithgpt/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)     3449 2024-05-09 12:44:16.000000 scrapwithgpt-0.0.6/scrapwithgpt/config.py
+-rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.6/scrapwithgpt/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)     3925 2024-05-09 12:58:51.000000 scrapwithgpt-0.0.6/scrapwithgpt/prompts.py
+-rw-r--r--   0 henry      (501) staff       (20)     4604 2024-05-09 12:58:16.000000 scrapwithgpt-0.0.6/scrapwithgpt/scrap.py
+-rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.6/scrapwithgpt/utils.py
+-rw-r--r--   0 henry      (501) staff       (20)    13377 2024-05-09 06:39:55.000000 scrapwithgpt-0.0.6/scrapwithgpt/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:58:56.775038 scrapwithgpt-0.0.6/scrapwithgpt.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:58:56.000000 scrapwithgpt-0.0.6/scrapwithgpt.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 12:58:56.000000 scrapwithgpt-0.0.6/scrapwithgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 12:58:56.000000 scrapwithgpt-0.0.6/scrapwithgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 12:58:56.000000 scrapwithgpt-0.0.6/scrapwithgpt.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 12:58:56.000000 scrapwithgpt-0.0.6/scrapwithgpt.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 12:58:56.775571 scrapwithgpt-0.0.6/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 12:54:20.000000 scrapwithgpt-0.0.6/setup.py
```

### Comparing `scrapwithgpt-0.0.5/PKG-INFO` & `scrapwithgpt-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.0.5/scrapwithgpt/config.py` & `scrapwithgpt-0.0.6/scrapwithgpt/config.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.5/scrapwithgpt/oai.py` & `scrapwithgpt-0.0.6/scrapwithgpt/oai.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.5/scrapwithgpt/prompts.py` & `scrapwithgpt-0.0.6/scrapwithgpt/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,20 @@
         The user will provide you with content extracted from a website. You must analyze this content and return True if the majority of the Criteria are met.
         ONLY use the content provided and follow strictly the below Instructions:
 
         ### Instructions: 
         1. Take your time and think step by step.
         2. Carefully go through the below Criteria: {criteria}
         3. If the majority of the Criteria are respected, return the word True and nothing else.
-        4. If the Criteria are NOT met at ALL, return the word False followed with a justification where you explain WHY the Criteria are not met at all. Be specific and say which criteria are not met and why.
-
+        4. If the Criteria are NOT met at ALL, return the word False followed with a justification where you explain WHY the Criteria are not met at all. Be specific and say which criteria is not met and why.
 
         ### Important considerations
         - Follow strictly the Instructions. 
         - Return True if the majority of the Criteria are respected. In this case, do not provide any justification. Just return True.
-        - If a large majority of the Criteria are STRICTLY NOT met, return the word False followed with the explanation. In this case, you MUST explain which Criteria are not met and WHY.
+        - If a large majority of the Criteria are STRICTLY NOT met, return the word False followed with the explanation. In this case, you MUST explain which Criteria is not met and WHY.
         - Do not preface your answer by anything.
         """)
 
 def gen_prompt_result(json_output:str, json_example=None) -> str:
     """
     Provide a list of criteria
     """
```

### Comparing `scrapwithgpt-0.0.5/scrapwithgpt/scrap.py` & `scrapwithgpt-0.0.6/scrapwithgpt/scrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #   Main function to scrap the page according to the criteria specified.
 
+from .config import MAX_TOKEN_OUTPUT_DEFAULT_HUGE, MAX_TOKEN_OUTPUT_GPT3, MAX_TOKEN_GPT4_RESULT, MAX_TOKEN_WINDOW_GPT35_TURBO
 from .prompts import gen_prompt_filter, gen_prompt_result, gen_role_summarizer
-from .config import MAX_TOKEN_OUTPUT_DEFAULT_HUGE, MAX_TOKEN_OUTPUT_GPT3, MAX_TOKEN_GPT4_RESULT
 from .web import crawl_website, fetch_content_url, clean_url_to_filename
 from .oai import ask_question_gpt, calculate_token, ask_question_gpt4
 from .utils import get_now, log_issue
 
 
 from typing import Optional
 import json
@@ -36,20 +36,20 @@
             
         else:
             if verbose: print(f"👷‍♂️ Crawling the page {url}.")    
             content = fetch_content_url(url)
         if filtering_criteria:
             if verbose: print(f"👷‍♂️ Checking if content matches criteria")
             role_filter = gen_prompt_filter(filtering_criteria)
-            buffer_tok = 16000 - calculate_token(json.dumps(role_filter)) - calculate_token(json.dumps(content))
-            if buffer_tok < 4000:
-                print("The website content is too large for a single prompt - TBD // TODO for Henry next version - chunking strat - END")
+            buffer_tok = MAX_TOKEN_WINDOW_GPT35_TURBO - calculate_token(role_filter) - calculate_token(content)
+            if buffer_tok < MAX_TOKEN_OUTPUT_GPT3-100: # Adding -100 as security
+                print(f"The website content is too large for a single prompt - remains only {buffer_tok} - TBD // TODO for Henry next version - chunking strat - END")
                 return ""
             else:
-                buffer_tok = max(min(buffer_tok, MAX_TOKEN_OUTPUT_GPT3), MAX_TOKEN_OUTPUT_DEFAULT_HUGE) # basically between 3K and 4K
+                buffer_tok = max(min(buffer_tok, MAX_TOKEN_OUTPUT_GPT3-100), MAX_TOKEN_OUTPUT_DEFAULT_HUGE) # basically between 3K and 4K
             answer_from_filtergpt = ask_question_gpt(content, role_filter, max_tokens= buffer_tok, verbose=False)
             if not answer_from_filtergpt:
                 if verbose: print("Couldn't check the Criteria - END")
                 return
             elif "false" in answer_from_filtergpt[:10].lower(): 
                 if verbose: print(f"The website is NOT relevant according to the Criteria. Response: {answer_from_filtergpt} - END")
                 return
```

### Comparing `scrapwithgpt-0.0.5/scrapwithgpt/utils.py` & `scrapwithgpt-0.0.6/scrapwithgpt/utils.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.5/scrapwithgpt/web.py` & `scrapwithgpt-0.0.6/scrapwithgpt/web.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.5/scrapwithgpt.egg-info/PKG-INFO` & `scrapwithgpt-0.0.6/scrapwithgpt.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.0.5/setup.py` & `scrapwithgpt-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapwithgpt",
-    version="0.0.5", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.0.6", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/scrapwithgpt',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

