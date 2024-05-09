# Comparing `tmp/scrapwithgpt-0.0.2.tar.gz` & `tmp/scrapwithgpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapwithgpt-0.0.2.tar", last modified: Thu May  9 12:32:38 2024, max compression
+gzip compressed data, was "scrapwithgpt-0.0.3.tar", last modified: Thu May  9 12:38:57 2024, max compression
```

## Comparing `scrapwithgpt-0.0.2.tar` & `scrapwithgpt-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:32:38.706328 scrapwithgpt-0.0.2/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:32:38.706094 scrapwithgpt-0.0.2/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.0.2/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:32:38.705121 scrapwithgpt-0.0.2/scrapwithgpt/
--rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.0.2/scrapwithgpt/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)     3421 2024-05-09 11:06:44.000000 scrapwithgpt-0.0.2/scrapwithgpt/config.py
--rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.2/scrapwithgpt/oai.py
--rw-r--r--   0 henry      (501) staff       (20)     4042 2024-05-09 11:41:45.000000 scrapwithgpt-0.0.2/scrapwithgpt/prompts.py
--rw-r--r--   0 henry      (501) staff       (20)     4445 2024-05-09 12:32:25.000000 scrapwithgpt-0.0.2/scrapwithgpt/scrap.py
--rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.2/scrapwithgpt/utils.py
--rw-r--r--   0 henry      (501) staff       (20)    13377 2024-05-09 06:39:55.000000 scrapwithgpt-0.0.2/scrapwithgpt/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:32:38.705882 scrapwithgpt-0.0.2/scrapwithgpt.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:32:38.000000 scrapwithgpt-0.0.2/scrapwithgpt.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 12:32:38.000000 scrapwithgpt-0.0.2/scrapwithgpt.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 12:32:38.000000 scrapwithgpt-0.0.2/scrapwithgpt.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 12:32:38.000000 scrapwithgpt-0.0.2/scrapwithgpt.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 12:32:38.000000 scrapwithgpt-0.0.2/scrapwithgpt.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 12:32:38.706369 scrapwithgpt-0.0.2/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 12:30:13.000000 scrapwithgpt-0.0.2/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:38:57.509075 scrapwithgpt-0.0.3/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:38:57.508856 scrapwithgpt-0.0.3/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.0.3/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:38:57.507892 scrapwithgpt-0.0.3/scrapwithgpt/
+-rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.0.3/scrapwithgpt/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)     3421 2024-05-09 11:06:44.000000 scrapwithgpt-0.0.3/scrapwithgpt/config.py
+-rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.3/scrapwithgpt/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)     4245 2024-05-09 12:38:48.000000 scrapwithgpt-0.0.3/scrapwithgpt/prompts.py
+-rw-r--r--   0 henry      (501) staff       (20)     4445 2024-05-09 12:32:25.000000 scrapwithgpt-0.0.3/scrapwithgpt/scrap.py
+-rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.3/scrapwithgpt/utils.py
+-rw-r--r--   0 henry      (501) staff       (20)    13377 2024-05-09 06:39:55.000000 scrapwithgpt-0.0.3/scrapwithgpt/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:38:57.508643 scrapwithgpt-0.0.3/scrapwithgpt.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:38:57.000000 scrapwithgpt-0.0.3/scrapwithgpt.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 12:38:57.000000 scrapwithgpt-0.0.3/scrapwithgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 12:38:57.000000 scrapwithgpt-0.0.3/scrapwithgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 12:38:57.000000 scrapwithgpt-0.0.3/scrapwithgpt.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 12:38:57.000000 scrapwithgpt-0.0.3/scrapwithgpt.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 12:38:57.509120 scrapwithgpt-0.0.3/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 12:38:55.000000 scrapwithgpt-0.0.3/setup.py
```

### Comparing `scrapwithgpt-0.0.2/PKG-INFO` & `scrapwithgpt-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.0.2/scrapwithgpt/config.py` & `scrapwithgpt-0.0.3/scrapwithgpt/config.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.2/scrapwithgpt/oai.py` & `scrapwithgpt-0.0.3/scrapwithgpt/oai.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.2/scrapwithgpt/prompts.py` & `scrapwithgpt-0.0.3/scrapwithgpt/prompts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # To generate prompts
 
 from .config import DEFAULT_FILTERING_CRITERIA
 from .utils import remove_excess
 
 
-
 def gen_prompt_filter(criteria:str=DEFAULT_FILTERING_CRITERIA) -> str:
     """
     Generates the system prompt / role to filter content based on a list of criteria.
     """
     return remove_excess(f"""
         You are a rigorous analyst. 
-        The user will provide you with content extracted from a website. You must analyze this content and return a clean content IF and ONLY IF the Criteria are met.
-        ONLY use the content available and follow strictly the below Instructions:
+        The user will provide you with content extracted from a website. You must analyze this content and return a clean content if the majority of the Criteria are met.
+        ONLY use the content provided and follow strictly the below Instructions:
 
         ### Instructions: 
         1. Take your time and think step by step.
-        2. Ensure that the below Criteria are met: {criteria}
-        3. If the Criteria are mostly respected, clean and return the content from the website. To clean it: remove redundant sentences, generic verbose and incoherent text BUT make sure not to KEEP ALL descriptive information. If you don't know, keep the information. Return ONLY the clean content and nothing else.
+        2. Carefully go through the below Criteria: {criteria}
+        3. If the majority of the Criteria are respected, clean and return the content from the website. To clean the content: remove redundant sentences, generic verbose and incoherent text BUT make sure not to KEEP ALL descriptive information. If you don't know, keep the information. Return ONLY the clean content and nothing else.
         4. If the Criteria are NOT met at ALL, return the word False followed with a justification where you explain WHY the Criteria are not met at all. Be specific and say which criteria are not met and why.
 
 
         ### Important considerations
         - Follow strictly the Instructions. 
-        - Return the clean content as text if the Criteria are met in general. In this case, do not provide any justification. Just return the clean content.
-        - If the Criteria are NOT met at ALL, return the word False followed with the explanation. In this case, you MUST explain which Criteria are not met and WHY.
+        - Return the clean content as text if the majority of the Criteria are respected. In this case, do not provide any justification. Just return the clean content.
+        - If a large majority of the Criteria are STRICTLY NOT met, return the word False followed with the explanation. In this case, you MUST explain which Criteria are not met and WHY.
+        - Remember that it is ONLY if a large majority of the Criteria are NOT respected than you return False. Otherwise, return the clean content.
         - Do not preface your answer by anything.
         """)
 
 def gen_prompt_result(json_output:str, json_example=None) -> str:
     """
     Provide a list of criteria
     """
```

### Comparing `scrapwithgpt-0.0.2/scrapwithgpt/scrap.py` & `scrapwithgpt-0.0.3/scrapwithgpt/scrap.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.2/scrapwithgpt/utils.py` & `scrapwithgpt-0.0.3/scrapwithgpt/utils.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.2/scrapwithgpt/web.py` & `scrapwithgpt-0.0.3/scrapwithgpt/web.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.2/scrapwithgpt.egg-info/PKG-INFO` & `scrapwithgpt-0.0.3/scrapwithgpt.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.0.2/setup.py` & `scrapwithgpt-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapwithgpt",
-    version="0.0.2", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.0.3", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/scrapwithgpt',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

