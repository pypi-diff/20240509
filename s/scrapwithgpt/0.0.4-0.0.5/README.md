# Comparing `tmp/scrapwithgpt-0.0.4.tar.gz` & `tmp/scrapwithgpt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapwithgpt-0.0.4.tar", last modified: Thu May  9 12:44:33 2024, max compression
+gzip compressed data, was "scrapwithgpt-0.0.5.tar", last modified: Thu May  9 12:53:08 2024, max compression
```

## Comparing `scrapwithgpt-0.0.4.tar` & `scrapwithgpt-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:44:33.916159 scrapwithgpt-0.0.4/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:44:33.915925 scrapwithgpt-0.0.4/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.0.4/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:44:33.914898 scrapwithgpt-0.0.4/scrapwithgpt/
--rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.0.4/scrapwithgpt/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)     3449 2024-05-09 12:44:16.000000 scrapwithgpt-0.0.4/scrapwithgpt/config.py
--rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.4/scrapwithgpt/oai.py
--rw-r--r--   0 henry      (501) staff       (20)     4332 2024-05-09 12:42:05.000000 scrapwithgpt-0.0.4/scrapwithgpt/prompts.py
--rw-r--r--   0 henry      (501) staff       (20)     4428 2024-05-09 12:44:25.000000 scrapwithgpt-0.0.4/scrapwithgpt/scrap.py
--rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.4/scrapwithgpt/utils.py
--rw-r--r--   0 henry      (501) staff       (20)    13377 2024-05-09 06:39:55.000000 scrapwithgpt-0.0.4/scrapwithgpt/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:44:33.915695 scrapwithgpt-0.0.4/scrapwithgpt.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:44:33.000000 scrapwithgpt-0.0.4/scrapwithgpt.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 12:44:33.000000 scrapwithgpt-0.0.4/scrapwithgpt.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 12:44:33.000000 scrapwithgpt-0.0.4/scrapwithgpt.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 12:44:33.000000 scrapwithgpt-0.0.4/scrapwithgpt.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 12:44:33.000000 scrapwithgpt-0.0.4/scrapwithgpt.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 12:44:33.916202 scrapwithgpt-0.0.4/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 12:41:08.000000 scrapwithgpt-0.0.4/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:53:08.611301 scrapwithgpt-0.0.5/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:53:08.611048 scrapwithgpt-0.0.5/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.0.5/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:53:08.608670 scrapwithgpt-0.0.5/scrapwithgpt/
+-rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.0.5/scrapwithgpt/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)     3449 2024-05-09 12:44:16.000000 scrapwithgpt-0.0.5/scrapwithgpt/config.py
+-rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.5/scrapwithgpt/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)     3928 2024-05-09 12:52:49.000000 scrapwithgpt-0.0.5/scrapwithgpt/prompts.py
+-rw-r--r--   0 henry      (501) staff       (20)     4495 2024-05-09 12:51:34.000000 scrapwithgpt-0.0.5/scrapwithgpt/scrap.py
+-rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.5/scrapwithgpt/utils.py
+-rw-r--r--   0 henry      (501) staff       (20)    13377 2024-05-09 06:39:55.000000 scrapwithgpt-0.0.5/scrapwithgpt/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:53:08.610788 scrapwithgpt-0.0.5/scrapwithgpt.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:53:08.000000 scrapwithgpt-0.0.5/scrapwithgpt.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 12:53:08.000000 scrapwithgpt-0.0.5/scrapwithgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 12:53:08.000000 scrapwithgpt-0.0.5/scrapwithgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 12:53:08.000000 scrapwithgpt-0.0.5/scrapwithgpt.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 12:53:08.000000 scrapwithgpt-0.0.5/scrapwithgpt.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 12:53:08.611349 scrapwithgpt-0.0.5/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 12:52:55.000000 scrapwithgpt-0.0.5/setup.py
```

### Comparing `scrapwithgpt-0.0.4/PKG-INFO` & `scrapwithgpt-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.0.4/scrapwithgpt/config.py` & `scrapwithgpt-0.0.5/scrapwithgpt/config.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.4/scrapwithgpt/oai.py` & `scrapwithgpt-0.0.5/scrapwithgpt/oai.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.4/scrapwithgpt/prompts.py` & `scrapwithgpt-0.0.5/scrapwithgpt/prompts.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 
 def gen_prompt_filter(criteria:str=DEFAULT_FILTERING_CRITERIA) -> str:
     """
     Generates the system prompt / role to filter content based on a list of criteria.
     """
     return remove_excess(f"""
         You are a rigorous analyst. 
-        The user will provide you with content extracted from a website. You must analyze this content and return a clean content if the majority of the Criteria are met.
+        The user will provide you with content extracted from a website. You must analyze this content and return True if the majority of the Criteria are met.
         ONLY use the content provided and follow strictly the below Instructions:
 
         ### Instructions: 
         1. Take your time and think step by step.
         2. Carefully go through the below Criteria: {criteria}
-        3. If the majority of the Criteria are respected, clean and return the content from the website. To clean the content: remove redundant sentences, generic verbose and incoherent text BUT make sure not to KEEP ALL descriptive information. If you don't know, keep the information. Return ONLY the clean content and nothing else.
+        3. If the majority of the Criteria are respected, return the word True and nothing else.
         4. If the Criteria are NOT met at ALL, return the word False followed with a justification where you explain WHY the Criteria are not met at all. Be specific and say which criteria are not met and why.
 
 
         ### Important considerations
         - Follow strictly the Instructions. 
-        - Return the clean content as text if the majority of the Criteria are respected. In this case, do not provide any justification. Just return the clean content.
+        - Return True if the majority of the Criteria are respected. In this case, do not provide any justification. Just return True.
         - If a large majority of the Criteria are STRICTLY NOT met, return the word False followed with the explanation. In this case, you MUST explain which Criteria are not met and WHY.
-        - Remember that it is ONLY if a large majority of the Criteria are NOT respected than you return False. Otherwise, return the clean content.
         - Do not preface your answer by anything.
         """)
 
 def gen_prompt_result(json_output:str, json_example=None) -> str:
     """
     Provide a list of criteria
     """
@@ -52,22 +51,22 @@
         """)
 
 def gen_role_summarizer() -> str:
     """
     Quick prompt for summarization. 
     """
     return remove_excess("""
-    You are an expert at making summarizations.
-    You take the text submitted by the user and return a summary that is well formatted.
-    Ensure that you keep ALL relevant information about the main topic of the content.
+    You are an expert at making summarizations that preserve ALL useful information.
+    You take the text submitted by the user and return a detailed summary.
+    You MUST ensure that you keep ALL relevant information about the main topic of the content.
                         
     ### Important Considerations: 
     - Do not include anything that is not in the provided text. ALWAYS be truthfull.
-    - Avoid puting recommendations like 'Subscribe to their newsletter for more information and updates'
+    - Avoid puting recommendations like 'Subscribe to their newsletter for more information and updates'.
     - Do not preface the summary with anything. Do not put a title. Only return the summary and nothing else.
     - Ensure you keep ALL contact details (email or phone number). Do not consider a website URL as a contact information.
-    - Ensure you keep ALL numbers and factual informations.                
+    - Ensure you keep ALL numbers and factual informations.           
     """)
 
 # *************************************************************
 if __name__ == "__main__":
     pass
```

### Comparing `scrapwithgpt-0.0.4/scrapwithgpt/scrap.py` & `scrapwithgpt-0.0.5/scrapwithgpt/scrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,30 +38,31 @@
             if verbose: print(f"👷‍♂️ Crawling the page {url}.")    
             content = fetch_content_url(url)
         if filtering_criteria:
             if verbose: print(f"👷‍♂️ Checking if content matches criteria")
             role_filter = gen_prompt_filter(filtering_criteria)
             buffer_tok = 16000 - calculate_token(json.dumps(role_filter)) - calculate_token(json.dumps(content))
             if buffer_tok < 4000:
-                print("The website content is too large for a single prompt - TBD chunking strat")
+                print("The website content is too large for a single prompt - TBD // TODO for Henry next version - chunking strat - END")
+                return ""
             else:
                 buffer_tok = max(min(buffer_tok, MAX_TOKEN_OUTPUT_GPT3), MAX_TOKEN_OUTPUT_DEFAULT_HUGE) # basically between 3K and 4K
-            filtered_content = ask_question_gpt(content, role_filter, max_tokens= buffer_tok, verbose=False)
-            if not filtered_content:
+            answer_from_filtergpt = ask_question_gpt(content, role_filter, max_tokens= buffer_tok, verbose=False)
+            if not answer_from_filtergpt:
                 if verbose: print("Couldn't check the Criteria - END")
                 return
-            elif "false" in filtered_content[:10].lower(): 
-                if verbose: print(f"The website is NOT relevant according to the Criteria. Response: {filtered_content} - END")
+            elif "false" in answer_from_filtergpt[:10].lower(): 
+                if verbose: print(f"The website is NOT relevant according to the Criteria. Response: {answer_from_filtergpt} - END")
                 return
         if summarization:
             if verbose: print(f"👷‍♂️ Generating a summary")   
-            summary = ask_question_gpt(filtered_content, gen_role_summarizer(), max_tokens=MAX_TOKEN_OUTPUT_DEFAULT_HUGE,  verbose=False)
+            summary = ask_question_gpt(content, gen_role_summarizer(), max_tokens=MAX_TOKEN_OUTPUT_DEFAULT_HUGE,  verbose=False)
         
         if verbose: print(f"👷‍♂️ Using GPT 4 to  the requested data")  
-        result = ask_question_gpt4(filtered_content, gen_prompt_result(desired_output, example_output), max_tokens=MAX_TOKEN_GPT4_RESULT,  verbose=False)
+        result = ask_question_gpt4(content, gen_prompt_result(desired_output, example_output), max_tokens=MAX_TOKEN_GPT4_RESULT,  verbose=False)
         if result:
             title = f"scrapwithgpt_{clean_url_to_filename(url)}.txt"
             if os.path.exists(title):
                 title = f"scrapwithgpt_{clean_url_to_filename(url)}_{get_now(True)}.txt" # To avoid overwriting
             if summary:
                 final_content = f"### SUMMARY of {url}:\n" + summary.replace(".", ".\n") + "\n\n" 
             final_content += f"### RESULT for {url}:\n" + result
```

### Comparing `scrapwithgpt-0.0.4/scrapwithgpt/utils.py` & `scrapwithgpt-0.0.5/scrapwithgpt/utils.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.4/scrapwithgpt/web.py` & `scrapwithgpt-0.0.5/scrapwithgpt/web.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.4/scrapwithgpt.egg-info/PKG-INFO` & `scrapwithgpt-0.0.5/scrapwithgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.0.4/setup.py` & `scrapwithgpt-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapwithgpt",
-    version="0.0.4", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.0.5", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/scrapwithgpt',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

