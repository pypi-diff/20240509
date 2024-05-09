# Comparing `tmp/partenaire-qualif-0.0.4.tar.gz` & `tmp/partenaire-qualif-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partenaire-qualif-0.0.4.tar", last modified: Thu May  9 04:15:26 2024, max compression
+gzip compressed data, was "partenaire-qualif-0.0.5.tar", last modified: Thu May  9 04:41:15 2024, max compression
```

## Comparing `partenaire-qualif-0.0.4.tar` & `partenaire-qualif-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 04:15:26.258614 partenaire-qualif-0.0.4/
--rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3256 2024-05-09 04:15:26.258614 partenaire-qualif-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2733 2024-05-09 03:25:03.000000 partenaire-qualif-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 04:15:26.242877 partenaire-qualif-0.0.4/partenaire_qualif.egg-info/
--rw-rw-rw-   0        0        0     3256 2024-05-09 04:15:26.000000 partenaire-qualif-0.0.4/partenaire_qualif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-05-09 04:15:26.000000 partenaire-qualif-0.0.4/partenaire_qualif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 04:15:26.000000 partenaire-qualif-0.0.4/partenaire_qualif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2024-05-09 04:15:26.000000 partenaire-qualif-0.0.4/partenaire_qualif.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-09 04:15:26.000000 partenaire-qualif-0.0.4/partenaire_qualif.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 04:15:26.258614 partenaire-qualif-0.0.4/qualif/
--rw-rw-rw-   0        0        0      101 2024-05-09 04:06:13.000000 partenaire-qualif-0.0.4/qualif/__init__.py
--rw-rw-rw-   0        0        0     7589 2024-05-09 03:11:33.000000 partenaire-qualif-0.0.4/qualif/qualif.py
--rw-rw-rw-   0        0        0       42 2024-05-09 04:15:26.258614 partenaire-qualif-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      919 2024-05-09 04:15:14.000000 partenaire-qualif-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 04:41:15.638443 partenaire-qualif-0.0.5/
+-rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3256 2024-05-09 04:41:15.638443 partenaire-qualif-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2733 2024-05-09 03:25:03.000000 partenaire-qualif-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 04:41:15.634363 partenaire-qualif-0.0.5/partenaire_qualif.egg-info/
+-rw-rw-rw-   0        0        0     3256 2024-05-09 04:41:15.000000 partenaire-qualif-0.0.5/partenaire_qualif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-05-09 04:41:15.000000 partenaire-qualif-0.0.5/partenaire_qualif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 04:41:15.000000 partenaire-qualif-0.0.5/partenaire_qualif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-09 04:41:15.000000 partenaire-qualif-0.0.5/partenaire_qualif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-09 04:41:15.000000 partenaire-qualif-0.0.5/partenaire_qualif.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 04:41:15.636446 partenaire-qualif-0.0.5/qualif/
+-rw-rw-rw-   0        0        0      101 2024-05-09 04:06:13.000000 partenaire-qualif-0.0.5/qualif/__init__.py
+-rw-rw-rw-   0        0        0     7992 2024-05-09 04:32:27.000000 partenaire-qualif-0.0.5/qualif/qualif.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 04:41:15.639415 partenaire-qualif-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      911 2024-05-09 04:38:46.000000 partenaire-qualif-0.0.5/setup.py
```

### Comparing `partenaire-qualif-0.0.4/LICENSE` & `partenaire-qualif-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.4/PKG-INFO` & `partenaire-qualif-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire-qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `partenaire-qualif-0.0.4/README.md` & `partenaire-qualif-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.4/partenaire_qualif.egg-info/PKG-INFO` & `partenaire-qualif-0.0.5/partenaire_qualif.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire-qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `partenaire-qualif-0.0.4/qualif/qualif.py` & `partenaire-qualif-0.0.5/qualif/qualif.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import tqdm
 import time
 import pandas as pd
 import json
 import logging
 import httpx
 import validators
+import importlib_resources
 
 logger = logging.getLogger(__name__)
 handler = logging.StreamHandler()
 logger.addHandler(handler)
 logger.setLevel(logging.INFO)
 
 
@@ -40,19 +41,27 @@
             return contents
 
         except Exception as e:
             raise e
 
 
 class CompanyQualificationTool:
-    def __init__(self, client: AzureOpenAI | OpenAI, prompt_qualification_template_path: str, model: str, temperature=0,
+    def __init__(self, client: AzureOpenAI | OpenAI, model: str, temperature=0, prompt_qualification_template_path= None,
                  browsing=False, browsing_key=None, prompt_find_website_template=None):
-        self.prompt_qualification = open(prompt_qualification_template_path).read()
-        if prompt_find_website_template is not None:
+
+        my_templates = importlib_resources.files("qualif") / "templates"
+        if prompt_qualification_template_path is None:
+            self.prompt_find_website = (my_templates / "prompt_find_website_template.txt").read_text()
+        else:
+            self.prompt_qualification = open(prompt_qualification_template_path).read()
+        if prompt_find_website_template is None:
+            self.prompt_qualification = (my_templates / "prompt_qualification_template.txt").read_text()
+        else:
             self.prompt_find_website = open(prompt_find_website_template).read()
+
         self.model = model
         self.client = client
         self.browsing = browsing
         self.browsing_key = browsing_key
         self.time_sleep = 0.1
         self.temperature = temperature
```

### Comparing `partenaire-qualif-0.0.4/setup.py` & `partenaire-qualif-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="partenaire-qualif",
-    version="0.0.4",
+    version="0.0.5",
     author="Yanchao MURONG",
     author_email="yanchao.murong@gmail.com",
     description="A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ymurong/partenaire-qualif.git",
     packages=setuptools.find_packages(),
     install_requires=[
-        'openai>=1.26.0',
-        'pandas>=2.2.2',
-        'httpx>=0.27.0',
-        'validators>=0.28.1',
-        'beautifulsoup4>=4.12.3',
+        'openai',
+        'pandas',
+        'httpx',
+        'validators',
+        'beautifulsoup4',
+        'importlib_resources'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
 )
```

