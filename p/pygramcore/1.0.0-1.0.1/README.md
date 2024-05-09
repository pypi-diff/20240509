# Comparing `tmp/pygramcore-1.0.0.tar.gz` & `tmp/pygramcore-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygramcore-1.0.0.tar", last modified: Thu May  9 17:16:44 2024, max compression
+gzip compressed data, was "pygramcore-1.0.1.tar", last modified: Thu May  9 18:28:23 2024, max compression
```

## Comparing `pygramcore-1.0.0.tar` & `pygramcore-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 17:16:44.877349 pygramcore-1.0.0/
--rw-rw-rw-   0        0        0     1089 2024-05-05 17:27:36.000000 pygramcore-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3725 2024-05-09 17:16:44.876849 pygramcore-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 17:16:44.875848 pygramcore-1.0.0/PyGramCore.egg-info/
--rw-rw-rw-   0        0        0     3725 2024-05-09 17:16:44.000000 pygramcore-1.0.0/PyGramCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2024-05-09 17:16:44.000000 pygramcore-1.0.0/PyGramCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 17:16:44.000000 pygramcore-1.0.0/PyGramCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-09 17:16:44.000000 pygramcore-1.0.0/PyGramCore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 17:16:44.000000 pygramcore-1.0.0/PyGramCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3009 2024-05-09 15:17:25.000000 pygramcore-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 17:16:44.858845 pygramcore-1.0.0/pygramcore/
--rw-rw-rw-   0        0        0       54 2024-05-09 13:07:12.000000 pygramcore-1.0.0/pygramcore/__init__.py
--rw-rw-rw-   0        0        0      266 2024-05-09 13:07:12.000000 pygramcore-1.0.0/pygramcore/constants.py
-drwxrwxrwx   0        0        0        0 2024-05-09 17:16:44.867350 pygramcore-1.0.0/pygramcore/elements/
--rw-rw-rw-   0        0        0       48 2024-05-09 13:07:12.000000 pygramcore-1.0.0/pygramcore/elements/__init__.py
--rw-rw-rw-   0        0        0     9663 2024-05-09 16:17:22.000000 pygramcore-1.0.0/pygramcore/elements/post.py
--rw-rw-rw-   0        0        0    14390 2024-05-09 16:20:10.000000 pygramcore-1.0.0/pygramcore/elements/user.py
-drwxrwxrwx   0        0        0        0 2024-05-09 17:16:44.872347 pygramcore-1.0.0/pygramcore/exceptions/
--rw-rw-rw-   0        0        0        0 2024-05-09 12:49:58.000000 pygramcore-1.0.0/pygramcore/exceptions/__init__.py
--rw-rw-rw-   0        0        0      148 2024-05-09 17:13:14.000000 pygramcore-1.0.0/pygramcore/exceptions/auth.py
--rw-rw-rw-   0        0        0      238 2024-05-09 17:07:39.000000 pygramcore-1.0.0/pygramcore/exceptions/format.py
--rw-rw-rw-   0        0        0      494 2024-05-09 13:07:12.000000 pygramcore-1.0.0/pygramcore/exceptions/post.py
--rw-rw-rw-   0        0        0      638 2024-05-09 13:07:12.000000 pygramcore-1.0.0/pygramcore/exceptions/user.py
--rw-rw-rw-   0        0        0     8945 2024-05-09 17:16:12.000000 pygramcore-1.0.0/pygramcore/pygram.py
-drwxrwxrwx   0        0        0        0 2024-05-09 17:16:44.874848 pygramcore-1.0.0/pygramcore/utils/
--rw-rw-rw-   0        0        0       21 2024-05-09 13:07:12.000000 pygramcore-1.0.0/pygramcore/utils/__init__.py
--rw-rw-rw-   0        0        0      977 2024-05-09 13:07:12.000000 pygramcore-1.0.0/pygramcore/utils/misc.py
--rw-rw-rw-   0        0        0       42 2024-05-09 17:16:44.877846 pygramcore-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1174 2024-05-09 17:05:22.000000 pygramcore-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:28:23.547564 pygramcore-1.0.1/
+-rw-rw-rw-   0        0        0     1089 2024-05-05 17:27:36.000000 pygramcore-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3888 2024-05-09 18:28:23.546564 pygramcore-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3172 2024-05-09 18:21:40.000000 pygramcore-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 18:28:23.515995 pygramcore-1.0.1/pygramcore/
+-rw-rw-rw-   0        0        0       54 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:28:23.538066 pygramcore-1.0.1/pygramcore/elements/
+-rw-rw-rw-   0        0        0       48 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/elements/__init__.py
+-rw-rw-rw-   0        0        0     9663 2024-05-09 16:17:22.000000 pygramcore-1.0.1/pygramcore/elements/post.py
+-rw-rw-rw-   0        0        0    14390 2024-05-09 16:20:10.000000 pygramcore-1.0.1/pygramcore/elements/user.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:28:23.543065 pygramcore-1.0.1/pygramcore/exceptions/
+-rw-rw-rw-   0        0        0        0 2024-05-09 12:49:58.000000 pygramcore-1.0.1/pygramcore/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      148 2024-05-09 17:13:14.000000 pygramcore-1.0.1/pygramcore/exceptions/auth.py
+-rw-rw-rw-   0        0        0      238 2024-05-09 17:07:39.000000 pygramcore-1.0.1/pygramcore/exceptions/format.py
+-rw-rw-rw-   0        0        0      494 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/exceptions/post.py
+-rw-rw-rw-   0        0        0      638 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/exceptions/user.py
+-rw-rw-rw-   0        0        0     8945 2024-05-09 17:16:12.000000 pygramcore-1.0.1/pygramcore/pygram.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:28:23.545064 pygramcore-1.0.1/pygramcore/utils/
+-rw-rw-rw-   0        0        0       21 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/utils/__init__.py
+-rw-rw-rw-   0        0        0      977 2024-05-09 13:07:12.000000 pygramcore-1.0.1/pygramcore/utils/misc.py
+drwxrwxrwx   0        0        0        0 2024-05-09 18:28:23.546064 pygramcore-1.0.1/pygramcore.egg-info/
+-rw-rw-rw-   0        0        0     3888 2024-05-09 18:28:23.000000 pygramcore-1.0.1/pygramcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      561 2024-05-09 18:28:23.000000 pygramcore-1.0.1/pygramcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 18:28:23.000000 pygramcore-1.0.1/pygramcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-09 18:28:23.000000 pygramcore-1.0.1/pygramcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 18:28:23.000000 pygramcore-1.0.1/pygramcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 18:28:23.548064 pygramcore-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1174 2024-05-09 18:27:01.000000 pygramcore-1.0.1/setup.py
```

### Comparing `pygramcore-1.0.0/LICENSE` & `pygramcore-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.0/PKG-INFO` & `pygramcore-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygramcore
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple-to-use Instagram Python interface using Selenium.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: instagram,instagram bot,selenium,automation,bot
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,36 +13,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium
 Requires-Dist: selenium-stealth
 
 <h1 align="center">
   <br>
-  <img src="/images/icon.png" alt="PyGramCore" width="200">
+  <img src="https://github.com/jtayped/pygramcore/blob/40436d7b57e247742b1697a88e52f06821e2f9f8/images/icon.png" alt="PyGramCore" width="200">
   <br>
   📷 pygramcore
   <br>
 </h1>
 
 <h4 align="center">An easy-to-use Instagram SDK using <a href="https://www.selenium.dev/" target="_blank">Selenium</a>.</h4>
 
-<p align="center">
+<div align="center">
   <a href="https://pypi.org/project/PyGramCore/">
     <img src="https://img.shields.io/pypi/v/pygramcore?style=for-the-badge">
   </a>
-  <a href="/LICENSE">
-      <img src="https://img.shields.io/github/license/jtayped/pygramcore?style=for-the-badge" alt="License">
+  <a href="https://github.com/jtayped/pygramcore/blob/main/LICENSE">
+    <img src="https://img.shields.io/github/license/jtayped/pygramcore?style=for-the-badge" alt="License">
   </a>
-    <a href="/issues">
-      <img src="https://img.shields.io/github/issues/jtayped/pygramcore?style=for-the-badge" alt="License">
+  <a href="https://github.com/jtayped/pygramcore/issues">
+    <img src="https://img.shields.io/github/issues/jtayped/pygramcore?style=for-the-badge" alt="License">
   </a>
   <a href="https://www.linkedin.com/in/jtayped/">
-      <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
+    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
   </a>
-</p>
+</div>
 
 <p align="center">
   <a href="#key-features">Key Features</a> •
   <a href="#how-to-use">How To Use</a> •
   <a href="#related">Related</a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygramcore Version: 1.0.0 Summary: A simple-to-use
+Metadata-Version: 2.1 Name: pygramcore Version: 1.0.1 Summary: A simple-to-use
 Instagram Python interface using Selenium. Author: Joel Taylor Author-email:
 contact@joeltaylor.business License: MIT Keywords: instagram,instagram
 bot,selenium,automation,bot Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
 CPython Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: selenium Requires-Dist: selenium-stealth
```

### Comparing `pygramcore-1.0.0/PyGramCore.egg-info/PKG-INFO` & `pygramcore-1.0.1/pygramcore.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygramcore
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple-to-use Instagram Python interface using Selenium.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: instagram,instagram bot,selenium,automation,bot
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,36 +13,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium
 Requires-Dist: selenium-stealth
 
 <h1 align="center">
   <br>
-  <img src="/images/icon.png" alt="PyGramCore" width="200">
+  <img src="https://github.com/jtayped/pygramcore/blob/40436d7b57e247742b1697a88e52f06821e2f9f8/images/icon.png" alt="PyGramCore" width="200">
   <br>
   📷 pygramcore
   <br>
 </h1>
 
 <h4 align="center">An easy-to-use Instagram SDK using <a href="https://www.selenium.dev/" target="_blank">Selenium</a>.</h4>
 
-<p align="center">
+<div align="center">
   <a href="https://pypi.org/project/PyGramCore/">
     <img src="https://img.shields.io/pypi/v/pygramcore?style=for-the-badge">
   </a>
-  <a href="/LICENSE">
-      <img src="https://img.shields.io/github/license/jtayped/pygramcore?style=for-the-badge" alt="License">
+  <a href="https://github.com/jtayped/pygramcore/blob/main/LICENSE">
+    <img src="https://img.shields.io/github/license/jtayped/pygramcore?style=for-the-badge" alt="License">
   </a>
-    <a href="/issues">
-      <img src="https://img.shields.io/github/issues/jtayped/pygramcore?style=for-the-badge" alt="License">
+  <a href="https://github.com/jtayped/pygramcore/issues">
+    <img src="https://img.shields.io/github/issues/jtayped/pygramcore?style=for-the-badge" alt="License">
   </a>
   <a href="https://www.linkedin.com/in/jtayped/">
-      <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
+    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
   </a>
-</p>
+</div>
 
 <p align="center">
   <a href="#key-features">Key Features</a> •
   <a href="#how-to-use">How To Use</a> •
   <a href="#related">Related</a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygramcore Version: 1.0.0 Summary: A simple-to-use
+Metadata-Version: 2.1 Name: pygramcore Version: 1.0.1 Summary: A simple-to-use
 Instagram Python interface using Selenium. Author: Joel Taylor Author-email:
 contact@joeltaylor.business License: MIT Keywords: instagram,instagram
 bot,selenium,automation,bot Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
 CPython Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: selenium Requires-Dist: selenium-stealth
```

### Comparing `pygramcore-1.0.0/PyGramCore.egg-info/SOURCES.txt` & `pygramcore-1.0.1/pygramcore.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 LICENSE
 README.md
 setup.py
-PyGramCore.egg-info/PKG-INFO
-PyGramCore.egg-info/SOURCES.txt
-PyGramCore.egg-info/dependency_links.txt
-PyGramCore.egg-info/requires.txt
-PyGramCore.egg-info/top_level.txt
 pygramcore/__init__.py
 pygramcore/constants.py
 pygramcore/pygram.py
 pygramcore.egg-info/PKG-INFO
 pygramcore.egg-info/SOURCES.txt
 pygramcore.egg-info/dependency_links.txt
 pygramcore.egg-info/requires.txt
```

### Comparing `pygramcore-1.0.0/README.md` & `pygramcore-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 <h1 align="center">
   <br>
-  <img src="/images/icon.png" alt="PyGramCore" width="200">
+  <img src="https://github.com/jtayped/pygramcore/blob/40436d7b57e247742b1697a88e52f06821e2f9f8/images/icon.png" alt="PyGramCore" width="200">
   <br>
   📷 pygramcore
   <br>
 </h1>
 
 <h4 align="center">An easy-to-use Instagram SDK using <a href="https://www.selenium.dev/" target="_blank">Selenium</a>.</h4>
 
-<p align="center">
+<div align="center">
   <a href="https://pypi.org/project/PyGramCore/">
     <img src="https://img.shields.io/pypi/v/pygramcore?style=for-the-badge">
   </a>
-  <a href="/LICENSE">
-      <img src="https://img.shields.io/github/license/jtayped/pygramcore?style=for-the-badge" alt="License">
+  <a href="https://github.com/jtayped/pygramcore/blob/main/LICENSE">
+    <img src="https://img.shields.io/github/license/jtayped/pygramcore?style=for-the-badge" alt="License">
   </a>
-    <a href="/issues">
-      <img src="https://img.shields.io/github/issues/jtayped/pygramcore?style=for-the-badge" alt="License">
+  <a href="https://github.com/jtayped/pygramcore/issues">
+    <img src="https://img.shields.io/github/issues/jtayped/pygramcore?style=for-the-badge" alt="License">
   </a>
   <a href="https://www.linkedin.com/in/jtayped/">
-      <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
+    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
   </a>
-</p>
+</div>
 
 <p align="center">
   <a href="#key-features">Key Features</a> •
   <a href="#how-to-use">How To Use</a> •
   <a href="#related">Related</a>
 </p>
```

### Comparing `pygramcore-1.0.0/pygramcore/elements/post.py` & `pygramcore-1.0.1/pygramcore/elements/post.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.0/pygramcore/elements/user.py` & `pygramcore-1.0.1/pygramcore/elements/user.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.0/pygramcore/exceptions/user.py` & `pygramcore-1.0.1/pygramcore/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.0/pygramcore/pygram.py` & `pygramcore-1.0.1/pygramcore/pygram.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.0/pygramcore/utils/misc.py` & `pygramcore-1.0.1/pygramcore/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.0/setup.py` & `pygramcore-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 # Read version from VERSION file
 here = path.abspath(path.dirname(__file__))
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 DESCRIPTION = "A simple-to-use Instagram Python interface using Selenium."
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

