# Comparing `tmp/scrapwithgpt-0.0.7.tar.gz` & `tmp/scrapwithgpt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapwithgpt-0.0.7.tar", last modified: Thu May  9 13:15:45 2024, max compression
+gzip compressed data, was "scrapwithgpt-0.1.0.tar", last modified: Thu May  9 13:31:30 2024, max compression
```

## Comparing `scrapwithgpt-0.0.7.tar` & `scrapwithgpt-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:15:45.231959 scrapwithgpt-0.0.7/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:15:45.231733 scrapwithgpt-0.0.7/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.0.7/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:15:45.230705 scrapwithgpt-0.0.7/scrapwithgpt/
--rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.0.7/scrapwithgpt/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)     3548 2024-05-09 13:11:16.000000 scrapwithgpt-0.0.7/scrapwithgpt/config.py
--rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.7/scrapwithgpt/oai.py
--rw-r--r--   0 henry      (501) staff       (20)     4185 2024-05-09 13:06:31.000000 scrapwithgpt-0.0.7/scrapwithgpt/prompts.py
--rw-r--r--   0 henry      (501) staff       (20)     4815 2024-05-09 13:08:30.000000 scrapwithgpt-0.0.7/scrapwithgpt/scrap.py
--rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.7/scrapwithgpt/utils.py
--rw-r--r--   0 henry      (501) staff       (20)    13519 2024-05-09 13:15:30.000000 scrapwithgpt-0.0.7/scrapwithgpt/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:15:45.231481 scrapwithgpt-0.0.7/scrapwithgpt.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:15:45.000000 scrapwithgpt-0.0.7/scrapwithgpt.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 13:15:45.000000 scrapwithgpt-0.0.7/scrapwithgpt.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 13:15:45.000000 scrapwithgpt-0.0.7/scrapwithgpt.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 13:15:45.000000 scrapwithgpt-0.0.7/scrapwithgpt.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 13:15:45.000000 scrapwithgpt-0.0.7/scrapwithgpt.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 13:15:45.232004 scrapwithgpt-0.0.7/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 13:15:35.000000 scrapwithgpt-0.0.7/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:31:30.878681 scrapwithgpt-0.1.0/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:31:30.878448 scrapwithgpt-0.1.0/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.1.0/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:31:30.876926 scrapwithgpt-0.1.0/scrapwithgpt/
+-rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.1.0/scrapwithgpt/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)     3639 2024-05-09 13:30:00.000000 scrapwithgpt-0.1.0/scrapwithgpt/config.py
+-rw-r--r--   0 henry      (501) staff       (20)     7885 2024-05-09 13:31:23.000000 scrapwithgpt-0.1.0/scrapwithgpt/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)     4283 2024-05-09 13:30:52.000000 scrapwithgpt-0.1.0/scrapwithgpt/prompts.py
+-rw-r--r--   0 henry      (501) staff       (20)     4902 2024-05-09 13:27:58.000000 scrapwithgpt-0.1.0/scrapwithgpt/scrap.py
+-rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.1.0/scrapwithgpt/utils.py
+-rw-r--r--   0 henry      (501) staff       (20)    13519 2024-05-09 13:15:30.000000 scrapwithgpt-0.1.0/scrapwithgpt/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:31:30.878202 scrapwithgpt-0.1.0/scrapwithgpt.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:31:30.000000 scrapwithgpt-0.1.0/scrapwithgpt.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 13:31:30.000000 scrapwithgpt-0.1.0/scrapwithgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 13:31:30.000000 scrapwithgpt-0.1.0/scrapwithgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 13:31:30.000000 scrapwithgpt-0.1.0/scrapwithgpt.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 13:31:30.000000 scrapwithgpt-0.1.0/scrapwithgpt.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 13:31:30.878731 scrapwithgpt-0.1.0/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 13:26:49.000000 scrapwithgpt-0.1.0/setup.py
```

### Comparing `scrapwithgpt-0.0.7/PKG-INFO` & `scrapwithgpt-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.0.7
+Version: 0.1.0
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.0.7/scrapwithgpt/config.py` & `scrapwithgpt-0.1.0/scrapwithgpt/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 """
 
 JSON_OUTPUT_VC = """{
   "Name of the fund": "string",
   "Country": "string",
   "Number of investments": "integer",
   "Size of the fund": "string",
-  "One relevant investment and why": "string",
+  "One relevant investment to us and why": "string",
   "Who to contact": {
     "Name": "string",
     "Position": "string",
     "Email": "string",
     "Linkedin page": "string"
   },
   "Good reasons to contact them": "string",
@@ -73,15 +73,15 @@
 }"""
 
 JSON_EXAMPLE_VC = """{
   "Name of the fund": "Innovate Ventures",
   "Country": "USA",
   "Number of investments": "12",
   "Size of the fund": "$50M",
-  "One relevant investment and why": "EduTech Innovators - Innovate Ventures invested $200K in 2019. EduTech is relevant because X,Y,Z",
+  "One relevant investment to us and why": "EduTech Innovators - Innovate Ventures invested $200K in 2019. EduTech is relevant because your company does X and EduTech does Y which has synergy with your company on A/B/C.",
   "Who to contact": {
     "Name": "Jane Doe",
     "Position": "Investment Director",
     "Email": "jdoe@innovatevc.com",
     "Linkedin page": "https://www.linkedin.com/in/janedoe"
   },
   "Good reasons to contact them": "Innovate Ventures has a strong focus on Edtech, which aligns with our product. They also have a track record of supporting early-stage startups and can provide valuable mentorship and networks in the US market.",
```

### Comparing `scrapwithgpt-0.0.7/scrapwithgpt/oai.py` & `scrapwithgpt-0.1.0/scrapwithgpt/oai.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,22 +110,21 @@
                 max_tokens=max_tokens,
                 top_p=top_p,
                 frequency_penalty=0,
                 presence_penalty=0,
                 stop=stop,
                 model=model,
             )
-            print(response)
             rep = response.choices[0].message.content
             rep = rep.strip()
             valid = True
         except Exception as e:
             attempts += 1
     if not rep:
-        print("We didn't get a reply")
+        print(f"We didn't get a reply despite {attempts} attempts")
     return rep
 
 
 def ask_question_gpt4(question: str, role: str, model=MODEL_GPT4_TURBO, max_tokens=MAX_TOKEN_OUTPUT_DEFAULT_HUGE, verbose=False, temperature=0, top_p=1, json_on=False,) -> str:
     """
     Queries Chat GPT 4 with a specific question if too lazy to change the param in ask_question_gpt)
     """
```

### Comparing `scrapwithgpt-0.0.7/scrapwithgpt/prompts.py` & `scrapwithgpt-0.1.0/scrapwithgpt/prompts.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     return remove_excess("""
     You are an expert at making summarizations that preserve ALL useful information.
     You take the text submitted by the user and return a detailed summary.
     You MUST ensure that you keep ALL relevant information about the main topic of the content.
                         
     ### Important Considerations: 
     - Do not include anything that is not in the provided text. ALWAYS be truthfull.
-    - Avoid puting recommendations like 'Subscribe to their newsletter for more information and updates'.
+    - Avoid puting recommendations like 'Subscribe to their newsletter for more information and updates'. REMOVE ALL reference to user action like 'individuals can subscribe to their monthly newsletter'.
     - Do not preface the summary with anything. Do not put a title. Only return the summary and nothing else.
     - Ensure you keep ALL contact details (email or phone number). Do not consider a website URL as a contact information.
     - Ensure you keep ALL numbers and factual informations.           
     """)
 
 # *************************************************************
 if __name__ == "__main__":
```

### Comparing `scrapwithgpt-0.0.7/scrapwithgpt/scrap.py` & `scrapwithgpt-0.1.0/scrapwithgpt/scrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .prompts import gen_prompt_filter, gen_prompt_result, gen_role_summarizer
 from .web import crawl_website, fetch_content_url, clean_url_to_filename
 from .oai import ask_question_gpt, calculate_token, ask_question_gpt4
 from .utils import get_now, log_issue
 
 
 from typing import Optional
-import json
+import time
 import os
 
 def smartscrap(url:str, desired_output:str=None, example_output:str=None, filtering_criteria:str=None, summarization:bool=True, full_website:bool=True, additional_consideration:str=None, verbose:bool=None) -> Optional[str]:
     """
     Main function to scrap a website.
 
     Args:
@@ -25,14 +25,15 @@
     Returns:
         - The content or None if issue. The content will also be put in a file named "gptscrapper_url.txt" in the current dir. 
 
     Note:    
     full_website is True by default. We scrap the full website up to 30 pages by default. Put it to False if you want to scrap ONLY the page.
     Change the crawl_website params to scrap more (or less) pages
     """
+    start = time.time()
     try:
         final_content, summary = "", ""
         if full_website:
             if verbose: print(f"👷‍♂️ Crawling the full website {url}. Please be patient...")
             content = str(crawl_website(url))
             
         else:
@@ -65,15 +66,15 @@
             if os.path.exists(title):
                 title = f"scrapwithgpt_{clean_url_to_filename(url)}_{get_now(True)}.txt" # To avoid overwriting
             if summary:
                 final_content = f"### SUMMARY of {url}:\n" + summary.replace(".", ".\n") + "\n\n" 
             final_content += f"### RESULT for {url}:\n" + result
             with open(title, "w") as file:
                 file.write(final_content)
-            if verbose: print(f"✅ Done - The content is in {title}")
+            if verbose: print(f"✅ Done - The content is in {title} and was obtained in {round(time.time()-start, 1)} seconds 👌")
         else:
             print("Failed to get the result data - END")
         return final_content
     except Exception as e:
         log_issue(e, smartscrap, f"TBD - add the params here")
 
 # *************************************************************
```

### Comparing `scrapwithgpt-0.0.7/scrapwithgpt/utils.py` & `scrapwithgpt-0.1.0/scrapwithgpt/utils.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.7/scrapwithgpt/web.py` & `scrapwithgpt-0.1.0/scrapwithgpt/web.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.7/scrapwithgpt.egg-info/PKG-INFO` & `scrapwithgpt-0.1.0/scrapwithgpt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.0.7
+Version: 0.1.0
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.0.7/setup.py` & `scrapwithgpt-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapwithgpt",
-    version="0.0.7", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.1.0", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/scrapwithgpt',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

