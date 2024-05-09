# Comparing `tmp/kal_middleware-0.0.1.tar.gz` & `tmp/kal_middleware-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kal_middleware-0.0.1.tar", last modified: Thu May  9 07:27:03 2024, max compression
+gzip compressed data, was "kal_middleware-0.0.2.tar", last modified: Thu May  9 11:08:55 2024, max compression
```

## Comparing `kal_middleware-0.0.1.tar` & `kal_middleware-0.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:27:03.708458 kal_middleware-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:27:03.700458 kal_middleware-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:27:03.704458 kal_middleware-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:27:03.704458 kal_middleware-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-09 07:27:03.708458 kal_middleware-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:27:03.704458 kal_middleware-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:27:03.704458 kal_middleware-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/docs/jwt.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/docs/kal_middleware.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:27:03.704458 kal_middleware-0.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/docs/sts.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:27:03.708458 kal_middleware-0.0.1/kal_middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/kal_middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/kal_middleware/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/kal_middleware/kal_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/kal_middleware/sts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:27:03.708458 kal_middleware-0.0.1/kal_middleware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-09 07:27:03.000000 kal_middleware-0.0.1/kal_middleware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-09 07:27:03.000000 kal_middleware-0.0.1/kal_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:27:03.000000 kal_middleware-0.0.1/kal_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 07:27:03.000000 kal_middleware-0.0.1/kal_middleware.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-09 07:27:03.000000 kal_middleware-0.0.1/kal_middleware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 07:27:03.000000 kal_middleware-0.0.1/kal_middleware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 07:27:03.708458 kal_middleware-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:27:03.708458 kal_middleware-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-09 07:26:52.000000 kal_middleware-0.0.1/tests/test_kal_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:08:55.408950 kal_middleware-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:08:55.400950 kal_middleware-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:08:55.404950 kal_middleware-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:08:55.404950 kal_middleware-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-09 11:08:55.408950 kal_middleware-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:08:55.404950 kal_middleware-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:08:55.404950 kal_middleware-0.0.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/docs/jwt.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/docs/kal_middleware.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:08:55.404950 kal_middleware-0.0.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/docs/sts.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:08:55.408950 kal_middleware-0.0.2/kal_middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/kal_middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/kal_middleware/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/kal_middleware/kal_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/kal_middleware/sts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:08:55.408950 kal_middleware-0.0.2/kal_middleware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-09 11:08:55.000000 kal_middleware-0.0.2/kal_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-09 11:08:55.000000 kal_middleware-0.0.2/kal_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:08:55.000000 kal_middleware-0.0.2/kal_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 11:08:55.000000 kal_middleware-0.0.2/kal_middleware.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-09 11:08:55.000000 kal_middleware-0.0.2/kal_middleware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 11:08:55.000000 kal_middleware-0.0.2/kal_middleware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:08:55.408950 kal_middleware-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:08:55.408950 kal_middleware-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-09 11:08:44.000000 kal_middleware-0.0.2/tests/test_kal_middleware.py
```

### Comparing `kal_middleware-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `kal_middleware-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/.github/ISSUE_TEMPLATE/config.yml` & `kal_middleware-0.0.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/.github/workflows/docs-build.yml` & `kal_middleware-0.0.2/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/.github/workflows/docs.yml` & `kal_middleware-0.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/.github/workflows/installation.yml` & `kal_middleware-0.0.2/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/.github/workflows/macos.yml` & `kal_middleware-0.0.2/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/.github/workflows/pypi.yml` & `kal_middleware-0.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/.github/workflows/ubuntu.yml` & `kal_middleware-0.0.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/.github/workflows/windows.yml` & `kal_middleware-0.0.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/.gitignore` & `kal_middleware-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/LICENSE` & `kal_middleware-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/PKG-INFO` & `kal_middleware-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kal-middleware
-Version: 0.0.1
+Version: 0.0.2
 Summary: Kaleidoo middleware package
 Author-email: Bar Lander <barh@kaleidoo.ai>
 License: MIT License
 Project-URL: Homepage, https://github.com/BarLanderK/kal-middleware
 Keywords: kal-middleware
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -63,16 +63,19 @@
     # Implement your logic to retrieve the user's role
     # If the user not found, return "".
     return "user_role"
 
 # Define a configuration map specifying services, actions, and required permissions
 config_map = {
     "service": {
-        "action": {
-            "permissions": ["user_role", "admin_role"]
+        "url": "service_url",
+        "actions": {
+            "example": {
+                "permissions": ["user_role", "admin_role"]
+            }
         }
     }
 }
 
 # if there is specific variable in the body that needed checks of who access its data only
 def check_access(firebase_uid, body):
     # check in the db the user and his parameters
```

### Comparing `kal_middleware-0.0.1/README.md` & `kal_middleware-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -35,16 +35,19 @@
     # Implement your logic to retrieve the user's role
     # If the user not found, return "".
     return "user_role"
 
 # Define a configuration map specifying services, actions, and required permissions
 config_map = {
     "service": {
-        "action": {
-            "permissions": ["user_role", "admin_role"]
+        "url": "service_url",
+        "actions": {
+            "example": {
+                "permissions": ["user_role", "admin_role"]
+            }
         }
     }
 }
 
 # if there is specific variable in the body that needed checks of who access its data only
 def check_access(firebase_uid, body):
     # check in the db the user and his parameters
```

### Comparing `kal_middleware-0.0.1/docs/contributing.md` & `kal_middleware-0.0.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/docs/installation.md` & `kal_middleware-0.0.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/kal_middleware/jwt.py` & `kal_middleware-0.0.2/kal_middleware/jwt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from functools import wraps
 from fastapi import Request, status
 from starlette.responses import Response
 import firebase_admin
 from firebase_admin import auth
-from typing import Callable, Optional, Dict, Any
+from typing import Callable, Optional, Dict, Any, List, Union
 
 default_app = firebase_admin.initialize_app()
 
 def jwt_authenticated(
     get_user_role_function: Callable[[str], Any],
-    config_map: Dict[str, Dict[str, Dict[str, list]]],
+    config_map: Dict[str, Dict[str, Union[str, Dict[str, Dict[str, List[str]]]]]],
     check_access: Optional[Callable[[str, Any], bool]] = None,
 ):
     def decorator(func: Callable) -> Callable:
         @wraps(func)
         async def decorated_function(request: Request, *args, **kwargs):
             # verify the token exists and validate with firebase
             header = request.headers.get("Authorization", None)
@@ -31,23 +31,23 @@
             # verify that the service and action exists in the config map
             service = request.path_params.get("service")
             action = request.path_params.get("action")
             if service not in config_map:
                 return Response(
                     status_code=status.HTTP_404_NOT_FOUND, content=f"Service {service} not found."
                 )
-            if action not in config_map[service]:
+            if action not in config_map[service]["actions"]:
                 return Response(
                     status_code=status.HTTP_404_NOT_FOUND,
                     content=f"Action {action} not found in service {service}.",
                 )
 
             # verify that the user has the permission to execute the request
             user_uid = decoded_token["uid"]
-            permissions = config_map[service][action]["permissions"]
+            permissions = config_map[service]["actions"][action]["permissions"]
             user_role = await get_user_role_function(user_uid)
 
             if not user_role:
                 return Response(
                     status_code=status.HTTP_404_NOT_FOUND,
                     content=f"User not exist.",
                 )
```

### Comparing `kal_middleware-0.0.1/kal_middleware/sts.py` & `kal_middleware-0.0.2/kal_middleware/sts.py`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/kal_middleware.egg-info/PKG-INFO` & `kal_middleware-0.0.2/kal_middleware.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kal-middleware
-Version: 0.0.1
+Version: 0.0.2
 Summary: Kaleidoo middleware package
 Author-email: Bar Lander <barh@kaleidoo.ai>
 License: MIT License
 Project-URL: Homepage, https://github.com/BarLanderK/kal-middleware
 Keywords: kal-middleware
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -63,16 +63,19 @@
     # Implement your logic to retrieve the user's role
     # If the user not found, return "".
     return "user_role"
 
 # Define a configuration map specifying services, actions, and required permissions
 config_map = {
     "service": {
-        "action": {
-            "permissions": ["user_role", "admin_role"]
+        "url": "service_url",
+        "actions": {
+            "example": {
+                "permissions": ["user_role", "admin_role"]
+            }
         }
     }
 }
 
 # if there is specific variable in the body that needed checks of who access its data only
 def check_access(firebase_uid, body):
     # check in the db the user and his parameters
```

### Comparing `kal_middleware-0.0.1/kal_middleware.egg-info/SOURCES.txt` & `kal_middleware-0.0.2/kal_middleware.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/mkdocs.yml` & `kal_middleware-0.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.1/pyproject.toml` & `kal_middleware-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kal-middleware"
-version = "0.0.1"
+version = "0.0.2"
 dynamic = [
     "dependencies",
 ]
 description = "Kaleidoo middleware package"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
@@ -75,8 +75,8 @@
 
 
 [project.urls]
 Homepage = "https://github.com/BarLanderK/kal-middleware"
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm>=8"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
```

