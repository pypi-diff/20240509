# Comparing `tmp/scrapwithgpt-0.1.1.tar.gz` & `tmp/scrapwithgpt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapwithgpt-0.1.1.tar", last modified: Thu May  9 13:33:37 2024, max compression
+gzip compressed data, was "scrapwithgpt-0.1.2.tar", last modified: Thu May  9 13:43:23 2024, max compression
```

## Comparing `scrapwithgpt-0.1.1.tar` & `scrapwithgpt-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:33:37.254192 scrapwithgpt-0.1.1/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:33:37.253935 scrapwithgpt-0.1.1/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.1.1/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:33:37.252859 scrapwithgpt-0.1.1/scrapwithgpt/
--rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.1.1/scrapwithgpt/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)     3639 2024-05-09 13:30:00.000000 scrapwithgpt-0.1.1/scrapwithgpt/config.py
--rw-r--r--   0 henry      (501) staff       (20)     7885 2024-05-09 13:31:23.000000 scrapwithgpt-0.1.1/scrapwithgpt/oai.py
--rw-r--r--   0 henry      (501) staff       (20)     4283 2024-05-09 13:30:52.000000 scrapwithgpt-0.1.1/scrapwithgpt/prompts.py
--rw-r--r--   0 henry      (501) staff       (20)     4902 2024-05-09 13:27:58.000000 scrapwithgpt-0.1.1/scrapwithgpt/scrap.py
--rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.1.1/scrapwithgpt/utils.py
--rw-r--r--   0 henry      (501) staff       (20)    13604 2024-05-09 13:33:33.000000 scrapwithgpt-0.1.1/scrapwithgpt/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:33:37.253690 scrapwithgpt-0.1.1/scrapwithgpt.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:33:37.000000 scrapwithgpt-0.1.1/scrapwithgpt.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 13:33:37.000000 scrapwithgpt-0.1.1/scrapwithgpt.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 13:33:37.000000 scrapwithgpt-0.1.1/scrapwithgpt.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 13:33:37.000000 scrapwithgpt-0.1.1/scrapwithgpt.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 13:33:37.000000 scrapwithgpt-0.1.1/scrapwithgpt.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 13:33:37.254236 scrapwithgpt-0.1.1/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 13:32:36.000000 scrapwithgpt-0.1.1/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:43:23.113040 scrapwithgpt-0.1.2/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:43:23.112812 scrapwithgpt-0.1.2/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.1.2/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:43:23.111760 scrapwithgpt-0.1.2/scrapwithgpt/
+-rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.1.2/scrapwithgpt/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)     3639 2024-05-09 13:30:00.000000 scrapwithgpt-0.1.2/scrapwithgpt/config.py
+-rw-r--r--   0 henry      (501) staff       (20)     7885 2024-05-09 13:31:23.000000 scrapwithgpt-0.1.2/scrapwithgpt/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)     4283 2024-05-09 13:30:52.000000 scrapwithgpt-0.1.2/scrapwithgpt/prompts.py
+-rw-r--r--   0 henry      (501) staff       (20)     5096 2024-05-09 13:43:16.000000 scrapwithgpt-0.1.2/scrapwithgpt/scrap.py
+-rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.1.2/scrapwithgpt/utils.py
+-rw-r--r--   0 henry      (501) staff       (20)    13604 2024-05-09 13:33:33.000000 scrapwithgpt-0.1.2/scrapwithgpt/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:43:23.112591 scrapwithgpt-0.1.2/scrapwithgpt.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:43:23.000000 scrapwithgpt-0.1.2/scrapwithgpt.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 13:43:23.000000 scrapwithgpt-0.1.2/scrapwithgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 13:43:23.000000 scrapwithgpt-0.1.2/scrapwithgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 13:43:23.000000 scrapwithgpt-0.1.2/scrapwithgpt.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 13:43:23.000000 scrapwithgpt-0.1.2/scrapwithgpt.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 13:43:23.113087 scrapwithgpt-0.1.2/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 13:34:50.000000 scrapwithgpt-0.1.2/setup.py
```

### Comparing `scrapwithgpt-0.1.1/PKG-INFO` & `scrapwithgpt-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.1.1/scrapwithgpt/config.py` & `scrapwithgpt-0.1.2/scrapwithgpt/config.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.1/scrapwithgpt/oai.py` & `scrapwithgpt-0.1.2/scrapwithgpt/oai.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.1/scrapwithgpt/prompts.py` & `scrapwithgpt-0.1.2/scrapwithgpt/prompts.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.1/scrapwithgpt/scrap.py` & `scrapwithgpt-0.1.2/scrapwithgpt/scrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,17 @@
             if verbose: print(f"👷‍♂️ Crawling the page {url}.")    
             content = fetch_content_url(url)
         if filtering_criteria:
             if verbose: print(f"👷‍♂️ Checking if content matches criteria")
             role_filter = gen_prompt_filter(filtering_criteria)
             buffer_tok = MAX_TOKEN_WINDOW_GPT35_TURBO - calculate_token(role_filter) - calculate_token(content)
             if buffer_tok < MAX_TOKEN_OUTPUT_GPT3-100: # Adding -100 as security
-                print(f"The website content is too large for a single prompt - remains only {buffer_tok} - TBD // TODO for Henry next version - chunking strat - END")
-                return ""
+                print(f"The website content is too large for a single prompt - remains only {buffer_tok}\nTBD // TODO for Henry next version\nFor now we will take a subset of the content\n🔴 Information might be missing!")
+                safe_removal = int((MAX_TOKEN_OUTPUT_GPT3 - buffer_tok) * 4) * 1.362 # Adding 36% buffer on top
+                content = content[:-safe_removal]
             else:
                 buffer_tok = max(min(buffer_tok, MAX_TOKEN_OUTPUT_GPT3-100), MAX_TOKEN_OUTPUT_DEFAULT_HUGE) # basically between 3K and 4K
             answer_from_filtergpt = ask_question_gpt(content, role_filter, max_tokens= buffer_tok, verbose=False)
             if not answer_from_filtergpt:
                 if verbose: print("Couldn't check the Criteria - END")
                 return
             elif "false" in answer_from_filtergpt[:10].lower():
```

### Comparing `scrapwithgpt-0.1.1/scrapwithgpt/utils.py` & `scrapwithgpt-0.1.2/scrapwithgpt/utils.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.1/scrapwithgpt/web.py` & `scrapwithgpt-0.1.2/scrapwithgpt/web.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.1/scrapwithgpt.egg-info/PKG-INFO` & `scrapwithgpt-0.1.2/scrapwithgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.1.1/setup.py` & `scrapwithgpt-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapwithgpt",
-    version="0.1.1", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.1.2", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/scrapwithgpt',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

