# Comparing `tmp/scrapwithgpt-0.0.6.tar.gz` & `tmp/scrapwithgpt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapwithgpt-0.0.6.tar", last modified: Thu May  9 12:58:56 2024, max compression
+gzip compressed data, was "scrapwithgpt-0.0.7.tar", last modified: Thu May  9 13:15:45 2024, max compression
```

## Comparing `scrapwithgpt-0.0.6.tar` & `scrapwithgpt-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:58:56.775518 scrapwithgpt-0.0.6/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:58:56.775305 scrapwithgpt-0.0.6/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.0.6/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:58:56.774245 scrapwithgpt-0.0.6/scrapwithgpt/
--rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.0.6/scrapwithgpt/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)     3449 2024-05-09 12:44:16.000000 scrapwithgpt-0.0.6/scrapwithgpt/config.py
--rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.6/scrapwithgpt/oai.py
--rw-r--r--   0 henry      (501) staff       (20)     3925 2024-05-09 12:58:51.000000 scrapwithgpt-0.0.6/scrapwithgpt/prompts.py
--rw-r--r--   0 henry      (501) staff       (20)     4604 2024-05-09 12:58:16.000000 scrapwithgpt-0.0.6/scrapwithgpt/scrap.py
--rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.6/scrapwithgpt/utils.py
--rw-r--r--   0 henry      (501) staff       (20)    13377 2024-05-09 06:39:55.000000 scrapwithgpt-0.0.6/scrapwithgpt/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:58:56.775038 scrapwithgpt-0.0.6/scrapwithgpt.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:58:56.000000 scrapwithgpt-0.0.6/scrapwithgpt.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 12:58:56.000000 scrapwithgpt-0.0.6/scrapwithgpt.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 12:58:56.000000 scrapwithgpt-0.0.6/scrapwithgpt.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 12:58:56.000000 scrapwithgpt-0.0.6/scrapwithgpt.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 12:58:56.000000 scrapwithgpt-0.0.6/scrapwithgpt.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 12:58:56.775571 scrapwithgpt-0.0.6/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 12:54:20.000000 scrapwithgpt-0.0.6/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:15:45.231959 scrapwithgpt-0.0.7/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:15:45.231733 scrapwithgpt-0.0.7/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.0.7/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:15:45.230705 scrapwithgpt-0.0.7/scrapwithgpt/
+-rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.0.7/scrapwithgpt/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)     3548 2024-05-09 13:11:16.000000 scrapwithgpt-0.0.7/scrapwithgpt/config.py
+-rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.7/scrapwithgpt/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)     4185 2024-05-09 13:06:31.000000 scrapwithgpt-0.0.7/scrapwithgpt/prompts.py
+-rw-r--r--   0 henry      (501) staff       (20)     4815 2024-05-09 13:08:30.000000 scrapwithgpt-0.0.7/scrapwithgpt/scrap.py
+-rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.7/scrapwithgpt/utils.py
+-rw-r--r--   0 henry      (501) staff       (20)    13519 2024-05-09 13:15:30.000000 scrapwithgpt-0.0.7/scrapwithgpt/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:15:45.231481 scrapwithgpt-0.0.7/scrapwithgpt.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:15:45.000000 scrapwithgpt-0.0.7/scrapwithgpt.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 13:15:45.000000 scrapwithgpt-0.0.7/scrapwithgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 13:15:45.000000 scrapwithgpt-0.0.7/scrapwithgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 13:15:45.000000 scrapwithgpt-0.0.7/scrapwithgpt.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 13:15:45.000000 scrapwithgpt-0.0.7/scrapwithgpt.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 13:15:45.232004 scrapwithgpt-0.0.7/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 13:15:35.000000 scrapwithgpt-0.0.7/setup.py
```

### Comparing `scrapwithgpt-0.0.6/PKG-INFO` & `scrapwithgpt-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.0.6/scrapwithgpt/config.py` & `scrapwithgpt-0.0.7/scrapwithgpt/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 """
 
 JSON_OUTPUT_VC = """{
   "Name of the fund": "string",
   "Country": "string",
   "Number of investments": "integer",
   "Size of the fund": "string",
-  "One relevant company they invest in": "string",
+  "One relevant investment and why": "string",
   "Who to contact": {
     "Name": "string",
     "Position": "string",
     "Email": "string",
     "Linkedin page": "string"
   },
   "Good reasons to contact them": "string",
@@ -73,18 +73,18 @@
 }"""
 
 JSON_EXAMPLE_VC = """{
   "Name of the fund": "Innovate Ventures",
   "Country": "USA",
   "Number of investments": "12",
   "Size of the fund": "$50M",
-  "Edtech info": "yes",
-  "One relevant company they invest in": "EduTech Innovators",
+  "One relevant investment and why": "EduTech Innovators - Innovate Ventures invested $200K in 2019. EduTech is relevant because X,Y,Z",
   "Who to contact": {
     "Name": "Jane Doe",
     "Position": "Investment Director",
     "Email": "jdoe@innovatevc.com",
     "Linkedin page": "https://www.linkedin.com/in/janedoe"
   },
   "Good reasons to contact them": "Innovate Ventures has a strong focus on Edtech, which aligns with our product. They also have a track record of supporting early-stage startups and can provide valuable mentorship and networks in the US market.",
-  "Useful Infos": "The fund recently increased its investment cap for Edtech startups and is actively seeking new innovative projects to finance."
+  "Useful Infos": "The fund recently increased its investment cap for Edtech startups and is actively seeking new innovative projects to finance. It mentioned that X and Y. It is noteworthy that Z."
 }"""
+
```

### Comparing `scrapwithgpt-0.0.6/scrapwithgpt/oai.py` & `scrapwithgpt-0.0.7/scrapwithgpt/oai.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.6/scrapwithgpt/prompts.py` & `scrapwithgpt-0.0.7/scrapwithgpt/prompts.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,19 @@
         ### Important considerations
         - Follow strictly the Instructions. 
         - Return True if the majority of the Criteria are respected. In this case, do not provide any justification. Just return True.
         - If a large majority of the Criteria are STRICTLY NOT met, return the word False followed with the explanation. In this case, you MUST explain which Criteria is not met and WHY.
         - Do not preface your answer by anything.
         """)
 
-def gen_prompt_result(json_output:str, json_example=None) -> str:
+def gen_prompt_result(json_output:str, json_example:str=None, additional_consideration:str=None) -> str:
     """
     Provide a list of criteria
     """
+    additional_consideration = "" if not additional_consideration else "Very important: You MUST the below considerations in mind when performing the task:\n" + additional_consideration
     example = "" if not json_example else f"""\n### Example of output:\n{json_example}\n"""
     return remove_excess(f"""
         You are a rigorous analyst. 
         The user will provide you with content extracted from a website. You must analyze this content and return a JSON object with the information filled when available.
         ONLY use the content available, NEVER INVENT anything and follow strictly the below Instructions:
 
         ### Instructions: 
@@ -43,14 +44,15 @@
         4. If the information is NOT in the content AT ALL, put NA.
         {example}
         ### Important considerations:
         - Follow strictly the Instructions. 
         - Remember that you must construct a JSON object with the provided keys, populated with the relevant information. If an information is not available at ALL or does not apply, use 'NA' for those fields.
         - Return the JSON and the JSON only. Do not preface by anything not even ```json before. 
         - Do your best, my job depends on the quality of your output.
+        {additional_consideration}
         """)
 
 def gen_role_summarizer() -> str:
     """
     Quick prompt for summarization. 
     """
     return remove_excess("""
```

### Comparing `scrapwithgpt-0.0.6/scrapwithgpt/scrap.py` & `scrapwithgpt-0.0.7/scrapwithgpt/scrap.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 from .utils import get_now, log_issue
 
 
 from typing import Optional
 import json
 import os
 
-def smartscrap(url:str, desired_output:str=None, example_output:str=None, filtering_criteria:str=None, summarization:bool=True, full_website:bool=True, verbose:bool=None) -> Optional[str]:
+def smartscrap(url:str, desired_output:str=None, example_output:str=None, filtering_criteria:str=None, summarization:bool=True, full_website:bool=True, additional_consideration:str=None, verbose:bool=None) -> Optional[str]:
     """
     Main function to scrap a website.
 
     Args:
         - url (str): The website to scrap
         - desired_output (str): A json like structure with the keys representing the information you want to find
         - filtering_criteria (str): A set of criteria the content must respect for the program to continue
         - summarization (bool): If you want also to output the summary of the website. True by default.
+        - additional_consideration (str): If you want to provide additional info to consider when generating the result. Ex: Info about your company.
 
     Returns:
         - The content or None if issue. The content will also be put in a file named "gptscrapper_url.txt" in the current dir. 
 
     Note:    
     full_website is True by default. We scrap the full website up to 30 pages by default. Put it to False if you want to scrap ONLY the page.
     Change the crawl_website params to scrap more (or less) pages
@@ -54,15 +55,15 @@
                 if verbose: print(f"The website is NOT relevant according to the Criteria. Response: {answer_from_filtergpt} - END")
                 return
         if summarization:
             if verbose: print(f"👷‍♂️ Generating a summary")   
             summary = ask_question_gpt(content, gen_role_summarizer(), max_tokens=MAX_TOKEN_OUTPUT_DEFAULT_HUGE,  verbose=False)
         
         if verbose: print(f"👷‍♂️ Using GPT 4 to  the requested data")  
-        result = ask_question_gpt4(content, gen_prompt_result(desired_output, example_output), max_tokens=MAX_TOKEN_GPT4_RESULT,  verbose=False)
+        result = ask_question_gpt4(content, gen_prompt_result(desired_output, example_output, additional_consideration), max_tokens=MAX_TOKEN_GPT4_RESULT,  verbose=False)
         if result:
             title = f"scrapwithgpt_{clean_url_to_filename(url)}.txt"
             if os.path.exists(title):
                 title = f"scrapwithgpt_{clean_url_to_filename(url)}_{get_now(True)}.txt" # To avoid overwriting
             if summary:
                 final_content = f"### SUMMARY of {url}:\n" + summary.replace(".", ".\n") + "\n\n" 
             final_content += f"### RESULT for {url}:\n" + result
```

### Comparing `scrapwithgpt-0.0.6/scrapwithgpt/utils.py` & `scrapwithgpt-0.0.7/scrapwithgpt/utils.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.6/scrapwithgpt/web.py` & `scrapwithgpt-0.0.7/scrapwithgpt/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,18 @@
 
     return text
 
 def clean_url_to_filename(url: str) -> str:
     """
     Convert URL to a suitable filename.
     """
-    file_name = urlparse(url).path
-    if file_name == "": file_name = "home_landing_none"
+    file_name = urlparse(url).netloc
+    if file_name == "":
+        file_name = url[url.find(".")+1: url.find(".",url.find(".")+1)]
+        if not file_name: file_name = url.replace("wwww","").replace("https://","").replace(".","")
     file_name = file_name.replace("/","_")
     file_name = file_name.replace("-","_")
     if file_name.startswith("_"): file_name = file_name[1:]
     return file_name
 
 def clean_url_into_title(url: str) -> str:
     """
```

### Comparing `scrapwithgpt-0.0.6/scrapwithgpt.egg-info/PKG-INFO` & `scrapwithgpt-0.0.7/scrapwithgpt.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.0.6/setup.py` & `scrapwithgpt-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapwithgpt",
-    version="0.0.6", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.0.7", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/scrapwithgpt',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

