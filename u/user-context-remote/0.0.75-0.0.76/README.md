# Comparing `tmp/user_context_remote-0.0.75.tar.gz` & `tmp/user_context_remote-0.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_context_remote-0.0.75.tar", last modified: Sat Apr 20 12:29:34 2024, max compression
+gzip compressed data, was "user_context_remote-0.0.76.tar", last modified: Thu May  9 11:29:18 2024, max compression
```

## Comparing `user_context_remote-0.0.75.tar` & `user_context_remote-0.0.76.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:29:34.411569 user_context_remote-0.0.75/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-20 12:29:34.411569 user_context_remote-0.0.75/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-20 12:29:13.000000 user_context_remote-0.0.75/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 12:29:13.000000 user_context_remote-0.0.75/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 12:29:34.411569 user_context_remote-0.0.75/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-20 12:29:13.000000 user_context_remote-0.0.75/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:29:34.407569 user_context_remote-0.0.75/user_context_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:29:34.411569 user_context_remote-0.0.75/user_context_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:29:13.000000 user_context_remote-0.0.75/user_context_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-04-20 12:29:13.000000 user_context_remote-0.0.75/user_context_remote/src/user_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:29:34.411569 user_context_remote-0.0.75/user_context_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-20 12:29:34.000000 user_context_remote-0.0.75/user_context_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-20 12:29:34.000000 user_context_remote-0.0.75/user_context_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:29:34.000000 user_context_remote-0.0.75/user_context_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-20 12:29:34.000000 user_context_remote-0.0.75/user_context_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-20 12:29:34.000000 user_context_remote-0.0.75/user_context_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:18.561052 user_context_remote-0.0.76/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-09 11:29:18.561052 user_context_remote-0.0.76/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-09 11:29:00.000000 user_context_remote-0.0.76/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 11:29:00.000000 user_context_remote-0.0.76/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:29:18.561052 user_context_remote-0.0.76/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-09 11:29:00.000000 user_context_remote-0.0.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:18.561052 user_context_remote-0.0.76/user_context_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:18.561052 user_context_remote-0.0.76/user_context_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:00.000000 user_context_remote-0.0.76/user_context_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-05-09 11:29:00.000000 user_context_remote-0.0.76/user_context_remote/src/user_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:18.561052 user_context_remote-0.0.76/user_context_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-09 11:29:18.000000 user_context_remote-0.0.76/user_context_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-09 11:29:18.000000 user_context_remote-0.0.76/user_context_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:29:18.000000 user_context_remote-0.0.76/user_context_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-09 11:29:18.000000 user_context_remote-0.0.76/user_context_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-09 11:29:18.000000 user_context_remote-0.0.76/user_context_remote.egg-info/top_level.txt
```

### Comparing `user_context_remote-0.0.75/PKG-INFO` & `user_context_remote-0.0.76/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.75
+Version: 0.0.76
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `user_context_remote-0.0.75/README.md` & `user_context_remote-0.0.76/README.md`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.75/pyproject.toml` & `user_context_remote-0.0.76/pyproject.toml`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.75/setup.py` & `user_context_remote-0.0.76/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-context-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name='user-context-remote',
-    version='0.0.75',  # https://pypi.org/project/user-context-remote/
+    version='0.0.76',  # https://pypi.org/project/user-context-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles User Context Local/Remote Python",
     long_description="This is a package for sharing common user-context-remote functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

### Comparing `user_context_remote-0.0.75/user_context_remote/src/user_context.py` & `user_context_remote-0.0.76/user_context_remote/src/user_context.py`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.75/user_context_remote.egg-info/PKG-INFO` & `user_context_remote-0.0.76/user_context_remote.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.75
+Version: 0.0.76
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

