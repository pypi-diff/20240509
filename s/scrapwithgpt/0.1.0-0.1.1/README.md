# Comparing `tmp/scrapwithgpt-0.1.0.tar.gz` & `tmp/scrapwithgpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapwithgpt-0.1.0.tar", last modified: Thu May  9 13:31:30 2024, max compression
+gzip compressed data, was "scrapwithgpt-0.1.1.tar", last modified: Thu May  9 13:33:37 2024, max compression
```

## Comparing `scrapwithgpt-0.1.0.tar` & `scrapwithgpt-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:31:30.878681 scrapwithgpt-0.1.0/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:31:30.878448 scrapwithgpt-0.1.0/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.1.0/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:31:30.876926 scrapwithgpt-0.1.0/scrapwithgpt/
--rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.1.0/scrapwithgpt/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)     3639 2024-05-09 13:30:00.000000 scrapwithgpt-0.1.0/scrapwithgpt/config.py
--rw-r--r--   0 henry      (501) staff       (20)     7885 2024-05-09 13:31:23.000000 scrapwithgpt-0.1.0/scrapwithgpt/oai.py
--rw-r--r--   0 henry      (501) staff       (20)     4283 2024-05-09 13:30:52.000000 scrapwithgpt-0.1.0/scrapwithgpt/prompts.py
--rw-r--r--   0 henry      (501) staff       (20)     4902 2024-05-09 13:27:58.000000 scrapwithgpt-0.1.0/scrapwithgpt/scrap.py
--rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.1.0/scrapwithgpt/utils.py
--rw-r--r--   0 henry      (501) staff       (20)    13519 2024-05-09 13:15:30.000000 scrapwithgpt-0.1.0/scrapwithgpt/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:31:30.878202 scrapwithgpt-0.1.0/scrapwithgpt.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:31:30.000000 scrapwithgpt-0.1.0/scrapwithgpt.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 13:31:30.000000 scrapwithgpt-0.1.0/scrapwithgpt.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 13:31:30.000000 scrapwithgpt-0.1.0/scrapwithgpt.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 13:31:30.000000 scrapwithgpt-0.1.0/scrapwithgpt.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 13:31:30.000000 scrapwithgpt-0.1.0/scrapwithgpt.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 13:31:30.878731 scrapwithgpt-0.1.0/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 13:26:49.000000 scrapwithgpt-0.1.0/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:33:37.254192 scrapwithgpt-0.1.1/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:33:37.253935 scrapwithgpt-0.1.1/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.1.1/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:33:37.252859 scrapwithgpt-0.1.1/scrapwithgpt/
+-rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.1.1/scrapwithgpt/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)     3639 2024-05-09 13:30:00.000000 scrapwithgpt-0.1.1/scrapwithgpt/config.py
+-rw-r--r--   0 henry      (501) staff       (20)     7885 2024-05-09 13:31:23.000000 scrapwithgpt-0.1.1/scrapwithgpt/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)     4283 2024-05-09 13:30:52.000000 scrapwithgpt-0.1.1/scrapwithgpt/prompts.py
+-rw-r--r--   0 henry      (501) staff       (20)     4902 2024-05-09 13:27:58.000000 scrapwithgpt-0.1.1/scrapwithgpt/scrap.py
+-rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.1.1/scrapwithgpt/utils.py
+-rw-r--r--   0 henry      (501) staff       (20)    13604 2024-05-09 13:33:33.000000 scrapwithgpt-0.1.1/scrapwithgpt/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:33:37.253690 scrapwithgpt-0.1.1/scrapwithgpt.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:33:37.000000 scrapwithgpt-0.1.1/scrapwithgpt.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 13:33:37.000000 scrapwithgpt-0.1.1/scrapwithgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 13:33:37.000000 scrapwithgpt-0.1.1/scrapwithgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 13:33:37.000000 scrapwithgpt-0.1.1/scrapwithgpt.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 13:33:37.000000 scrapwithgpt-0.1.1/scrapwithgpt.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 13:33:37.254236 scrapwithgpt-0.1.1/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 13:32:36.000000 scrapwithgpt-0.1.1/setup.py
```

### Comparing `scrapwithgpt-0.1.0/PKG-INFO` & `scrapwithgpt-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.1.0/scrapwithgpt/config.py` & `scrapwithgpt-0.1.1/scrapwithgpt/config.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.0/scrapwithgpt/oai.py` & `scrapwithgpt-0.1.1/scrapwithgpt/oai.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.0/scrapwithgpt/prompts.py` & `scrapwithgpt-0.1.1/scrapwithgpt/prompts.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.0/scrapwithgpt/scrap.py` & `scrapwithgpt-0.1.1/scrapwithgpt/scrap.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.0/scrapwithgpt/utils.py` & `scrapwithgpt-0.1.1/scrapwithgpt/utils.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.0/scrapwithgpt/web.py` & `scrapwithgpt-0.1.1/scrapwithgpt/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,20 @@
     return text
 
 def clean_url_to_filename(url: str) -> str:
     """
     Convert URL to a suitable filename.
     """
     file_name = urlparse(url).netloc
+    if file_name and "." in file_name:
+        file_name = file_name.split(".")[1]
     if file_name == "":
         file_name = url[url.find(".")+1: url.find(".",url.find(".")+1)]
         if not file_name: file_name = url.replace("wwww","").replace("https://","").replace(".","")
+ 
     file_name = file_name.replace("/","_")
     file_name = file_name.replace("-","_")
     if file_name.startswith("_"): file_name = file_name[1:]
     return file_name
 
 def clean_url_into_title(url: str) -> str:
     """
```

### Comparing `scrapwithgpt-0.1.0/scrapwithgpt.egg-info/PKG-INFO` & `scrapwithgpt-0.1.1/scrapwithgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.1.0/setup.py` & `scrapwithgpt-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapwithgpt",
-    version="0.1.0", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.1.1", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/scrapwithgpt',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

