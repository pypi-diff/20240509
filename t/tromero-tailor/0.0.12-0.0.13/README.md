# Comparing `tmp/tromero_tailor-0.0.12.tar.gz` & `tmp/tromero_tailor-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tromero_tailor-0.0.12.tar", last modified: Wed Apr 24 09:58:06 2024, max compression
+gzip compressed data, was "tromero_tailor-0.0.13.tar", last modified: Thu May  9 14:34:54 2024, max compression
```

## Comparing `tromero_tailor-0.0.12.tar` & `tromero_tailor-0.0.13.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-04-24 09:58:06.218749 tromero_tailor-0.0.12/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-04-24 09:58:06.218533 tromero_tailor-0.0.12/PKG-INFO
--rw-r--r--   0 tadhgamin   (501) staff       (20)      942 2024-04-08 16:49:32.000000 tromero_tailor-0.0.12/README.md
--rw-r--r--   0 tadhgamin   (501) staff       (20)       38 2024-04-24 09:58:06.218792 tromero_tailor-0.0.12/setup.cfg
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1633 2024-04-24 09:57:55.000000 tromero_tailor-0.0.12/setup.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-04-24 09:58:06.216502 tromero_tailor-0.0.12/tests/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     3672 2024-04-17 14:55:07.000000 tromero_tailor-0.0.12/tests/test.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-04-24 09:58:06.217317 tromero_tailor-0.0.12/tromero_tailor/
--rw-r--r--   0 tadhgamin   (501) staff       (20)       30 2024-04-08 15:07:54.000000 tromero_tailor-0.0.12/tromero_tailor/__init__.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1337 2024-04-24 09:57:47.000000 tromero_tailor-0.0.12/tromero_tailor/tromero_requests.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)      446 2024-04-12 11:06:15.000000 tromero_tailor-0.0.12/tromero_tailor/tromero_utils.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)     2828 2024-04-23 11:05:42.000000 tromero_tailor-0.0.12/tromero_tailor/wrapper.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-04-24 09:58:06.218182 tromero_tailor-0.0.12/tromero_tailor.egg-info/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-04-24 09:58:06.000000 tromero_tailor-0.0.12/tromero_tailor.egg-info/PKG-INFO
--rw-r--r--   0 tadhgamin   (501) staff       (20)      341 2024-04-24 09:58:06.000000 tromero_tailor-0.0.12/tromero_tailor.egg-info/SOURCES.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)        1 2024-04-24 09:58:06.000000 tromero_tailor-0.0.12/tromero_tailor.egg-info/dependency_links.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)      304 2024-04-24 09:58:06.000000 tromero_tailor-0.0.12/tromero_tailor.egg-info/requires.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)       15 2024-04-24 09:58:06.000000 tromero_tailor-0.0.12/tromero_tailor.egg-info/top_level.txt
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-09 14:34:54.322718 tromero_tailor-0.0.13/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-09 14:34:54.322509 tromero_tailor-0.0.13/PKG-INFO
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      942 2024-04-08 16:49:32.000000 tromero_tailor-0.0.13/README.md
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       38 2024-05-09 14:34:54.322758 tromero_tailor-0.0.13/setup.cfg
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1633 2024-05-09 14:34:42.000000 tromero_tailor-0.0.13/setup.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-09 14:34:54.320394 tromero_tailor-0.0.13/tests/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     3672 2024-04-17 14:55:07.000000 tromero_tailor-0.0.13/tests/test.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-09 14:34:54.321341 tromero_tailor-0.0.13/tromero_tailor/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       30 2024-04-08 15:07:54.000000 tromero_tailor-0.0.13/tromero_tailor/__init__.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1336 2024-05-09 14:32:30.000000 tromero_tailor-0.0.13/tromero_tailor/tromero_requests.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      446 2024-04-12 11:06:15.000000 tromero_tailor-0.0.13/tromero_tailor/tromero_utils.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     2828 2024-04-23 11:05:42.000000 tromero_tailor-0.0.13/tromero_tailor/wrapper.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-09 14:34:54.322215 tromero_tailor-0.0.13/tromero_tailor.egg-info/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-09 14:34:54.000000 tromero_tailor-0.0.13/tromero_tailor.egg-info/PKG-INFO
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      341 2024-05-09 14:34:54.000000 tromero_tailor-0.0.13/tromero_tailor.egg-info/SOURCES.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)        1 2024-05-09 14:34:54.000000 tromero_tailor-0.0.13/tromero_tailor.egg-info/dependency_links.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      304 2024-05-09 14:34:54.000000 tromero_tailor-0.0.13/tromero_tailor.egg-info/requires.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       15 2024-05-09 14:34:54.000000 tromero_tailor-0.0.13/tromero_tailor.egg-info/top_level.txt
```

### Comparing `tromero_tailor-0.0.12/PKG-INFO` & `tromero_tailor-0.0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tromero_tailor
-Version: 0.0.12
+Version: 0.0.13
 Summary: A short description of your package
 Home-page: http://yourpackagehomepage.com
 Author: Tromero
 Author-email: tadhg.amin@tromero.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tromero_tailor-0.0.12/README.md` & `tromero_tailor-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.12/setup.py` & `tromero_tailor-0.0.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tromero_tailor",  # Replace with your package name
-    version="0.0.12",  # Replace with your package's version
+    version="0.0.13",  # Replace with your package's version
     author="Tromero",  # Replace with your name
     author_email="tadhg.amin@tromero.ai",  # Replace with your email address
     description="A short description of your package",  # Provide a short description
     long_description=open('README.md').read(),  # This will read your long description from README.md
     long_description_content_type='text/markdown',  # Indicates that the long description is in Markdown
     url="http://yourpackagehomepage.com",  # Replace with the URL to your package's homepage
     license="MIT",  # Replace with your chosen license
```

### Comparing `tromero_tailor-0.0.12/tests/test.py` & `tromero_tailor-0.0.13/tests/test.py`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.12/tromero_tailor/tromero_requests.py` & `tromero_tailor-0.0.13/tromero_tailor/tromero_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
 data_url = "https://midyear-grid-402910.lm.r.appspot.com/tailor/v1/data"
-models_url = "http://87.120.209.240:5000/generate"
+models_url = "http://35.246.163.71:5000/generate"
 
 def post_data(data, auth_token):
     headers = {
         'X-API-KEY': auth_token,
         'Content-Type': 'application/json'
     }
     try:
```

### Comparing `tromero_tailor-0.0.12/tromero_tailor/wrapper.py` & `tromero_tailor-0.0.13/tromero_tailor/wrapper.py`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.12/tromero_tailor.egg-info/PKG-INFO` & `tromero_tailor-0.0.13/tromero_tailor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tromero_tailor
-Version: 0.0.12
+Version: 0.0.13
 Summary: A short description of your package
 Home-page: http://yourpackagehomepage.com
 Author: Tromero
 Author-email: tadhg.amin@tromero.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

