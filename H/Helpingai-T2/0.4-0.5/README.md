# Comparing `tmp/Helpingai_T2-0.4.tar.gz` & `tmp/Helpingai_T2-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Helpingai_T2-0.4.tar", last modified: Fri May  3 05:00:51 2024, max compression
+gzip compressed data, was "Helpingai_T2-0.5.tar", last modified: Thu May  9 15:54:47 2024, max compression
```

## Comparing `Helpingai_T2-0.4.tar` & `Helpingai_T2-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 05:00:51.749431 Helpingai_T2-0.4/
-drwxrwxrwx   0        0        0        0 2024-05-03 05:00:51.645093 Helpingai_T2-0.4/Helpingai_T2/
--rw-rw-rw-   0        0        0     4597 2024-05-03 04:58:45.000000 Helpingai_T2-0.4/Helpingai_T2/Labs.py
--rw-rw-rw-   0        0        0     4431 2024-05-03 04:58:45.000000 Helpingai_T2-0.4/Helpingai_T2/Search.py
--rw-rw-rw-   0        0        0      104 2024-05-03 05:00:37.000000 Helpingai_T2-0.4/Helpingai_T2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 05:00:51.729663 Helpingai_T2-0.4/Helpingai_T2.egg-info/
--rw-rw-rw-   0        0        0     3120 2024-05-03 05:00:50.000000 Helpingai_T2-0.4/Helpingai_T2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-03 05:00:51.000000 Helpingai_T2-0.4/Helpingai_T2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 05:00:50.000000 Helpingai_T2-0.4/Helpingai_T2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-03 05:00:50.000000 Helpingai_T2-0.4/Helpingai_T2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-03 05:00:50.000000 Helpingai_T2-0.4/Helpingai_T2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2024-05-03 04:58:45.000000 Helpingai_T2-0.4/LICENSE
--rw-rw-rw-   0        0        0     3120 2024-05-03 05:00:51.743436 Helpingai_T2-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1954 2024-05-03 04:58:45.000000 Helpingai_T2-0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 05:00:51.750441 Helpingai_T2-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1532 2024-05-03 05:00:42.000000 Helpingai_T2-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 15:54:47.319412 Helpingai_T2-0.5/
+drwxrwxrwx   0        0        0        0 2024-05-09 15:54:46.984934 Helpingai_T2-0.5/Helpingai_T2/
+-rw-rw-rw-   0        0        0     4597 2024-05-03 04:58:45.000000 Helpingai_T2-0.5/Helpingai_T2/Labs.py
+-rw-rw-rw-   0        0        0     4341 2024-05-09 15:50:06.000000 Helpingai_T2-0.5/Helpingai_T2/Search.py
+-rw-rw-rw-   0        0        0      104 2024-05-03 05:00:37.000000 Helpingai_T2-0.5/Helpingai_T2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 15:54:47.290417 Helpingai_T2-0.5/Helpingai_T2.egg-info/
+-rw-rw-rw-   0        0        0     3120 2024-05-09 15:54:45.000000 Helpingai_T2-0.5/Helpingai_T2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-09 15:54:45.000000 Helpingai_T2-0.5/Helpingai_T2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 15:54:45.000000 Helpingai_T2-0.5/Helpingai_T2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-09 15:54:45.000000 Helpingai_T2-0.5/Helpingai_T2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-09 15:54:45.000000 Helpingai_T2-0.5/Helpingai_T2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2024-05-03 04:58:45.000000 Helpingai_T2-0.5/LICENSE
+-rw-rw-rw-   0        0        0     3120 2024-05-09 15:54:47.308417 Helpingai_T2-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1954 2024-05-03 04:58:45.000000 Helpingai_T2-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-09 15:54:47.326422 Helpingai_T2-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1532 2024-05-09 15:50:12.000000 Helpingai_T2-0.5/setup.py
```

### Comparing `Helpingai_T2-0.4/Helpingai_T2/Labs.py` & `Helpingai_T2-0.5/Helpingai_T2/Labs.py`

 * *Files identical despite different names*

### Comparing `Helpingai_T2-0.4/Helpingai_T2/Search.py` & `Helpingai_T2-0.5/Helpingai_T2/Search.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,18 @@
 from requests import Session
 
 
 class Perplexity:
     def __init__(self):
         self.session = Session()
         self.request_headers = {
-            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:124.0) Gecko/20100101 Firefox/124.0",
-            "Referer" : "https://www.perplexity.ai/",
-            "Accept" : "*/*",
-            "Accept-Encoding": 	"gzip, deflate",
-            "Accept-Language" :"en-US,en;q=0.5",
-        }
+    "Sec-Fetch-User": "?1",
+    "Upgrade-Insecure-Requests": "1",
+    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36"
+    }
         self.session.headers.update(self.request_headers)
         self.t = format(getrandbits(32), "08x")
         self.sid = loads(
             self.session.get(
                 url=f"https://www.perplexity.ai/socket.io/?EIO=4&transport=polling&t={self.t}"
             ).text[1:]
         )["sid"]
```

### Comparing `Helpingai_T2-0.4/Helpingai_T2.egg-info/PKG-INFO` & `Helpingai_T2-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Helpingai-T2
-Version: 0.4
+Name: Helpingai_T2
+Version: 0.5
 Summary: A simple module to use Perplexity AI in Python.
 Home-page: https://github.com/HelpingAI/Helpingai_T2.git
 Author: OEvortex
 License: GPLv3
 Project-URL: Source, https://github.com/HelpingAI/Helpingai_T2.git
 Keywords: artificial-intelligence,perplexityai,perplexity,python,api,ai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Helpingai_T2-0.4/LICENSE` & `Helpingai_T2-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Helpingai_T2-0.4/PKG-INFO` & `Helpingai_T2-0.5/Helpingai_T2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Helpingai_T2
-Version: 0.4
+Name: Helpingai-T2
+Version: 0.5
 Summary: A simple module to use Perplexity AI in Python.
 Home-page: https://github.com/HelpingAI/Helpingai_T2.git
 Author: OEvortex
 License: GPLv3
 Project-URL: Source, https://github.com/HelpingAI/Helpingai_T2.git
 Keywords: artificial-intelligence,perplexityai,perplexity,python,api,ai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Helpingai_T2-0.4/README.md` & `Helpingai_T2-0.5/README.md`

 * *Files identical despite different names*

### Comparing `Helpingai_T2-0.4/setup.py` & `Helpingai_T2-0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="Helpingai_T2",
-    version="0.4",
+    version="0.5",
     description="A simple module to use Perplexity AI in Python.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/HelpingAI/Helpingai_T2.git",
     author="OEvortex",
     license="GPLv3",
     keywords=[
```

