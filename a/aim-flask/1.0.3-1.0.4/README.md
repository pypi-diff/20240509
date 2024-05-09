# Comparing `tmp/aim_flask-1.0.3.tar.gz` & `tmp/aim_flask-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aim_flask-1.0.3.tar", max compression
+gzip compressed data, was "aim_flask-1.0.4.tar", max compression
```

## Comparing `aim_flask-1.0.3.tar` & `aim_flask-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       91 2024-05-09 18:42:35.660138 aim_flask-1.0.3/aim_flask/__init__.py
--rw-r--r--   0        0        0     8823 2024-05-09 18:43:59.155387 aim_flask-1.0.3/aim_flask/main.py
--rw-r--r--   0        0        0     1087 2024-05-08 23:37:10.837307 aim_flask-1.0.3/LICENSE
--rw-r--r--   0        0        0      408 2024-05-09 18:35:58.663153 aim_flask-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 aim_flask-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-05-09 18:42:35.660138 aim_flask-1.0.4/aim_flask/__init__.py
+-rw-r--r--   0        0        0     8823 2024-05-09 19:25:11.895554 aim_flask-1.0.4/aim_flask/main.py
+-rw-r--r--   0        0        0     1087 2024-05-08 23:37:10.837307 aim_flask-1.0.4/LICENSE
+-rw-r--r--   0        0        0      413 2024-05-09 19:30:13.058311 aim_flask-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 aim_flask-1.0.4/PKG-INFO
```

### Comparing `aim_flask-1.0.3/aim_flask/main.py` & `aim_flask-1.0.4/aim_flask/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import subprocess
 import platform
 import logging
 
 # aim_flask.py
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 # Configure logging
 logging.basicConfig(filename='../setup.log', level=logging.INFO, format='%(asctime)s - %(levelname)s: %(message)s')
 logger = logging.getLogger(__name__)
 
 # GitHub repository URL for feedback and logs
 GITHUB_REPO_URL = "https://github.com/MrMayami/AIM.git"
```

### Comparing `aim_flask-1.0.3/LICENSE` & `aim_flask-1.0.4/LICENSE`

 * *Files identical despite different names*

