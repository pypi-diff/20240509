# Comparing `tmp/name_that_fucking_film-0.1.1.tar.gz` & `tmp/name_that_fucking_film-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "name_that_fucking_film-0.1.1.tar", max compression
+gzip compressed data, was "name_that_fucking_film-0.1.2.tar", max compression
```

## Comparing `name_that_fucking_film-0.1.1.tar` & `name_that_fucking_film-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1359 2024-05-09 19:08:20.531696 name_that_fucking_film-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-06 17:14:37.807976 name_that_fucking_film-0.1.1/name_that_fucking_film/__init__.py
--rw-r--r--   0        0        0     6745 2024-05-09 19:08:46.419175 name_that_fucking_film-0.1.1/name_that_fucking_film/main.py
--rw-r--r--   0        0        0      397 2024-05-09 19:09:30.021043 name_that_fucking_film-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 name_that_fucking_film-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1359 2024-05-09 19:08:20.531696 name_that_fucking_film-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 17:14:37.807976 name_that_fucking_film-0.1.2/name_that_fucking_film/__init__.py
+-rw-r--r--   0        0        0     6785 2024-05-09 19:14:00.966696 name_that_fucking_film-0.1.2/name_that_fucking_film/main.py
+-rw-r--r--   0        0        0      397 2024-05-09 19:16:57.267313 name_that_fucking_film-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 name_that_fucking_film-0.1.2/PKG-INFO
```

### Comparing `name_that_fucking_film-0.1.1/README.md` & `name_that_fucking_film-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `name_that_fucking_film-0.1.1/name_that_fucking_film/main.py` & `name_that_fucking_film-0.1.2/name_that_fucking_film/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import pathlib
 import re
+import sys
 from random import choice
 
 import pandas as pd
 from rich.console import Console
 
 console = Console(highlight=False)
+resources_path = sys.argv[1]
 
 
 def levenshtein(s1, s2):
     if len(s1) > len(s2):
         s1, s2 = s2, s1
     distances = range(len(s1) + 1)
     for i2, c2 in enumerate(s2):
```

### Comparing `name_that_fucking_film-0.1.1/PKG-INFO` & `name_that_fucking_film-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: name-that-fucking-film
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: jkarenko
 Author-email: juho.karenko@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

