# Comparing `tmp/scrapwithgpt-0.0.1.tar.gz` & `tmp/scrapwithgpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapwithgpt-0.0.1.tar", last modified: Thu May  9 12:00:33 2024, max compression
+gzip compressed data, was "scrapwithgpt-0.0.2.tar", last modified: Thu May  9 12:32:38 2024, max compression
```

## Comparing `scrapwithgpt-0.0.1.tar` & `scrapwithgpt-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:00:33.087891 scrapwithgpt-0.0.1/
--rw-r--r--   0 henry      (501) staff       (20)      373 2024-05-09 12:00:33.087678 scrapwithgpt-0.0.1/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      113 2024-05-09 11:54:19.000000 scrapwithgpt-0.0.1/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:00:33.086700 scrapwithgpt-0.0.1/scrapwithgpt/
--rw-r--r--   0 henry      (501) staff       (20)       79 2024-05-09 11:58:44.000000 scrapwithgpt-0.0.1/scrapwithgpt/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)     3421 2024-05-09 11:06:44.000000 scrapwithgpt-0.0.1/scrapwithgpt/config.py
--rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.1/scrapwithgpt/oai.py
--rw-r--r--   0 henry      (501) staff       (20)     4042 2024-05-09 11:41:45.000000 scrapwithgpt-0.0.1/scrapwithgpt/prompts.py
--rw-r--r--   0 henry      (501) staff       (20)     4412 2024-05-09 11:58:41.000000 scrapwithgpt-0.0.1/scrapwithgpt/scrap.py
--rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.1/scrapwithgpt/utils.py
--rw-r--r--   0 henry      (501) staff       (20)    13377 2024-05-09 06:39:55.000000 scrapwithgpt-0.0.1/scrapwithgpt/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:00:33.087469 scrapwithgpt-0.0.1/scrapwithgpt.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)      373 2024-05-09 12:00:33.000000 scrapwithgpt-0.0.1/scrapwithgpt.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 12:00:33.000000 scrapwithgpt-0.0.1/scrapwithgpt.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 12:00:33.000000 scrapwithgpt-0.0.1/scrapwithgpt.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 12:00:33.000000 scrapwithgpt-0.0.1/scrapwithgpt.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 12:00:33.000000 scrapwithgpt-0.0.1/scrapwithgpt.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 12:00:33.087935 scrapwithgpt-0.0.1/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 11:54:24.000000 scrapwithgpt-0.0.1/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:32:38.706328 scrapwithgpt-0.0.2/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:32:38.706094 scrapwithgpt-0.0.2/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.0.2/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:32:38.705121 scrapwithgpt-0.0.2/scrapwithgpt/
+-rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.0.2/scrapwithgpt/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)     3421 2024-05-09 11:06:44.000000 scrapwithgpt-0.0.2/scrapwithgpt/config.py
+-rw-r--r--   0 henry      (501) staff       (20)     7884 2024-05-09 11:07:59.000000 scrapwithgpt-0.0.2/scrapwithgpt/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)     4042 2024-05-09 11:41:45.000000 scrapwithgpt-0.0.2/scrapwithgpt/prompts.py
+-rw-r--r--   0 henry      (501) staff       (20)     4445 2024-05-09 12:32:25.000000 scrapwithgpt-0.0.2/scrapwithgpt/scrap.py
+-rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.0.2/scrapwithgpt/utils.py
+-rw-r--r--   0 henry      (501) staff       (20)    13377 2024-05-09 06:39:55.000000 scrapwithgpt-0.0.2/scrapwithgpt/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 12:32:38.705882 scrapwithgpt-0.0.2/scrapwithgpt.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 12:32:38.000000 scrapwithgpt-0.0.2/scrapwithgpt.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 12:32:38.000000 scrapwithgpt-0.0.2/scrapwithgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 12:32:38.000000 scrapwithgpt-0.0.2/scrapwithgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 12:32:38.000000 scrapwithgpt-0.0.2/scrapwithgpt.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 12:32:38.000000 scrapwithgpt-0.0.2/scrapwithgpt.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 12:32:38.706369 scrapwithgpt-0.0.2/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 12:30:13.000000 scrapwithgpt-0.0.2/setup.py
```

### Comparing `scrapwithgpt-0.0.1/scrapwithgpt/config.py` & `scrapwithgpt-0.0.2/scrapwithgpt/config.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.1/scrapwithgpt/oai.py` & `scrapwithgpt-0.0.2/scrapwithgpt/oai.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.1/scrapwithgpt/prompts.py` & `scrapwithgpt-0.0.2/scrapwithgpt/prompts.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.1/scrapwithgpt/scrap.py` & `scrapwithgpt-0.0.2/scrapwithgpt/scrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,11 +70,13 @@
         else:
             print("Failed to get the result data - END")
         return final_content
     except Exception as e:
         log_issue(e, smartscrap, f"TBD - add the params here")
 
 # *************************************************************
-test_url = "https://www.27v.vc"
 
 if __name__ == "__main__":
-    smartscrap(test_url, desired_output=JSON_OUTPUT_VC, example_output=JSON_EXAMPLE_VC, filtering_criteria=DEFAULT_FILTERING_CRITERIA, verbose=True)
+    pass
+    # How to use
+    # test_url = "https://www.27v.vc"
+    #smartscrap(test_url, desired_output=JSON_OUTPUT_VC, example_output=JSON_EXAMPLE_VC, filtering_criteria=DEFAULT_FILTERING_CRITERIA, verbose=True)
```

### Comparing `scrapwithgpt-0.0.1/scrapwithgpt/utils.py` & `scrapwithgpt-0.0.2/scrapwithgpt/utils.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.1/scrapwithgpt/web.py` & `scrapwithgpt-0.0.2/scrapwithgpt/web.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.0.1/setup.py` & `scrapwithgpt-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapwithgpt",
-    version="0.0.1", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.0.2", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/scrapwithgpt',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

