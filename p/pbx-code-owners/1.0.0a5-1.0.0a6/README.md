# Comparing `tmp/pbx_code_owners-1.0.0a5.tar.gz` & `tmp/pbx_code_owners-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbx_code_owners-1.0.0a5.tar", last modified: Wed May  8 10:22:12 2024, max compression
+gzip compressed data, was "pbx_code_owners-1.0.0a6.tar", last modified: Thu May  9 13:04:48 2024, max compression
```

## Comparing `pbx_code_owners-1.0.0a5.tar` & `pbx_code_owners-1.0.0a6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-08 10:22:12.125073 pbx_code_owners-1.0.0a5/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1063 2024-05-08 10:22:12.125073 pbx_code_owners-1.0.0a5/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      796 2024-05-08 10:00:04.000000 pbx_code_owners-1.0.0a5/README.md
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-08 10:22:12.124073 pbx_code_owners-1.0.0a5/code_owners/
--rw-r--r--   0 pawel     (1000) pawel     (1000)       39 2024-05-08 09:11:46.000000 pbx_code_owners-1.0.0a5/code_owners/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      490 2024-05-08 09:27:11.000000 pbx_code_owners-1.0.0a5/code_owners/config.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2225 2024-05-07 14:02:56.000000 pbx_code_owners-1.0.0a5/code_owners/parser.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-08 10:22:12.125073 pbx_code_owners-1.0.0a5/pbx_code_owners.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1063 2024-05-08 10:22:12.000000 pbx_code_owners-1.0.0a5/pbx_code_owners.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      347 2024-05-08 10:22:12.000000 pbx_code_owners-1.0.0a5/pbx_code_owners.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-05-08 10:22:12.000000 pbx_code_owners-1.0.0a5/pbx_code_owners.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       53 2024-05-08 10:22:12.000000 pbx_code_owners-1.0.0a5/pbx_code_owners.egg-info/entry_points.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       16 2024-05-08 10:22:12.000000 pbx_code_owners-1.0.0a5/pbx_code_owners.egg-info/requires.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       12 2024-05-08 10:22:12.000000 pbx_code_owners-1.0.0a5/pbx_code_owners.egg-info/top_level.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)      403 2024-05-08 10:22:12.125073 pbx_code_owners-1.0.0a5/setup.cfg
--rw-r--r--   0 pawel     (1000) pawel     (1000)      680 2024-05-08 10:00:31.000000 pbx_code_owners-1.0.0a5/setup.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-08 10:22:12.125073 pbx_code_owners-1.0.0a5/tests/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3357 2024-05-08 08:57:15.000000 pbx_code_owners-1.0.0a5/tests/tests.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-09 13:04:48.408701 pbx_code_owners-1.0.0a6/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1070 2024-05-09 13:04:48.408701 pbx_code_owners-1.0.0a6/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      803 2024-05-09 12:49:22.000000 pbx_code_owners-1.0.0a6/README.md
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-09 13:04:48.407701 pbx_code_owners-1.0.0a6/code_owners/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       50 2024-05-09 12:59:35.000000 pbx_code_owners-1.0.0a6/code_owners/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      497 2024-05-09 12:42:22.000000 pbx_code_owners-1.0.0a6/code_owners/config.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2225 2024-05-07 14:02:56.000000 pbx_code_owners-1.0.0a6/code_owners/parser.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-09 13:04:48.408701 pbx_code_owners-1.0.0a6/pbx_code_owners.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1070 2024-05-09 13:04:48.000000 pbx_code_owners-1.0.0a6/pbx_code_owners.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      358 2024-05-09 13:04:48.000000 pbx_code_owners-1.0.0a6/pbx_code_owners.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-05-09 13:04:48.000000 pbx_code_owners-1.0.0a6/pbx_code_owners.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       53 2024-05-09 13:04:48.000000 pbx_code_owners-1.0.0a6/pbx_code_owners.egg-info/entry_points.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       16 2024-05-09 13:04:48.000000 pbx_code_owners-1.0.0a6/pbx_code_owners.egg-info/requires.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       12 2024-05-09 13:04:48.000000 pbx_code_owners-1.0.0a6/pbx_code_owners.egg-info/top_level.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      403 2024-05-09 13:04:48.408701 pbx_code_owners-1.0.0a6/setup.cfg
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      680 2024-05-09 13:04:24.000000 pbx_code_owners-1.0.0a6/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-09 13:04:48.408701 pbx_code_owners-1.0.0a6/tests/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3357 2024-05-08 12:03:18.000000 pbx_code_owners-1.0.0a6/tests/test_code_owners.py
```

### Comparing `pbx_code_owners-1.0.0a5/PKG-INFO` & `pbx_code_owners-1.0.0a6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbx-code-owners
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Code Owners implementation
 Home-page: https://getprintbox.com/
 Author: 
 Author-email: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
@@ -38,8 +38,8 @@
 
 Download package with pip, and execute script with command `pbx-code-owners`. 
 
 Make sure you have all necessary environmental variables in scope:
 * CI_SERVER_URL (eg. https://yourcompany.gitlab.com)
 * CI_PROJECT_ID (can be found in project settings)
 * CI_MERGE_REQUEST_IID (merge request ID)
-* MR_QA_GUARD_TOKEN (access token necessary for creating threads)
+* CODE_OWNERS_GITLAB_TOKEN (access token necessary for creating threads)
```

### Comparing `pbx_code_owners-1.0.0a5/README.md` & `pbx_code_owners-1.0.0a6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 
 Download package with pip, and execute script with command `pbx-code-owners`. 
 
 Make sure you have all necessary environmental variables in scope:
 * CI_SERVER_URL (eg. https://yourcompany.gitlab.com)
 * CI_PROJECT_ID (can be found in project settings)
 * CI_MERGE_REQUEST_IID (merge request ID)
-* MR_QA_GUARD_TOKEN (access token necessary for creating threads)
+* CODE_OWNERS_GITLAB_TOKEN (access token necessary for creating threads)
```

### Comparing `pbx_code_owners-1.0.0a5/code_owners/parser.py` & `pbx_code_owners-1.0.0a6/code_owners/parser.py`

 * *Files identical despite different names*

### Comparing `pbx_code_owners-1.0.0a5/pbx_code_owners.egg-info/PKG-INFO` & `pbx_code_owners-1.0.0a6/pbx_code_owners.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbx-code-owners
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Code Owners implementation
 Home-page: https://getprintbox.com/
 Author: 
 Author-email: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
@@ -38,8 +38,8 @@
 
 Download package with pip, and execute script with command `pbx-code-owners`. 
 
 Make sure you have all necessary environmental variables in scope:
 * CI_SERVER_URL (eg. https://yourcompany.gitlab.com)
 * CI_PROJECT_ID (can be found in project settings)
 * CI_MERGE_REQUEST_IID (merge request ID)
-* MR_QA_GUARD_TOKEN (access token necessary for creating threads)
+* CODE_OWNERS_GITLAB_TOKEN (access token necessary for creating threads)
```

### Comparing `pbx_code_owners-1.0.0a5/setup.py` & `pbx_code_owners-1.0.0a6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pbx-code-owners",
-    version="1.0.0a5",
+    version="1.0.0a6",
     packages=find_packages(exclude=["tests*"]),
     url="https://getprintbox.com/",
     license="",
     author="",
     author_email="",
     description="Code Owners implementation",
     install_requires=[
```

### Comparing `pbx_code_owners-1.0.0a5/tests/tests.py` & `pbx_code_owners-1.0.0a6/tests/test_code_owners.py`

 * *Files identical despite different names*

