# Comparing `tmp/chaseinvest_api-0.1.2.tar.gz` & `tmp/chaseinvest_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaseinvest_api-0.1.2.tar", last modified: Thu May  9 10:44:42 2024, max compression
+gzip compressed data, was "chaseinvest_api-0.1.3.tar", last modified: Thu May  9 11:02:41 2024, max compression
```

## Comparing `chaseinvest_api-0.1.2.tar` & `chaseinvest_api-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:44:42.175531 chaseinvest_api-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-09 10:44:42.175531 chaseinvest_api-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:44:42.171531 chaseinvest_api-0.1.2/chase/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/chase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/chase/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/chase/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/chase/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/chase/symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/chase/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:44:42.171531 chaseinvest_api-0.1.2/chaseinvest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-09 10:44:42.000000 chaseinvest_api-0.1.2/chaseinvest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-09 10:44:42.000000 chaseinvest_api-0.1.2/chaseinvest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:44:42.000000 chaseinvest_api-0.1.2/chaseinvest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-09 10:44:42.000000 chaseinvest_api-0.1.2/chaseinvest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 10:44:42.000000 chaseinvest_api-0.1.2/chaseinvest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:44:42.175531 chaseinvest_api-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:44:42.171531 chaseinvest_api-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:02:41.675894 chaseinvest_api-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-09 11:02:37.000000 chaseinvest_api-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-09 11:02:41.675894 chaseinvest_api-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-09 11:02:37.000000 chaseinvest_api-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:02:41.675894 chaseinvest_api-0.1.3/chase/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 11:02:37.000000 chaseinvest_api-0.1.3/chase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-09 11:02:37.000000 chaseinvest_api-0.1.3/chase/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-05-09 11:02:37.000000 chaseinvest_api-0.1.3/chase/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-05-09 11:02:37.000000 chaseinvest_api-0.1.3/chase/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-09 11:02:37.000000 chaseinvest_api-0.1.3/chase/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-09 11:02:37.000000 chaseinvest_api-0.1.3/chase/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:02:41.675894 chaseinvest_api-0.1.3/chaseinvest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-09 11:02:41.000000 chaseinvest_api-0.1.3/chaseinvest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-09 11:02:41.000000 chaseinvest_api-0.1.3/chaseinvest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:02:41.000000 chaseinvest_api-0.1.3/chaseinvest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-09 11:02:41.000000 chaseinvest_api-0.1.3/chaseinvest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 11:02:41.000000 chaseinvest_api-0.1.3/chaseinvest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:02:41.675894 chaseinvest_api-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-09 11:02:37.000000 chaseinvest_api-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:02:41.675894 chaseinvest_api-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-09 11:02:37.000000 chaseinvest_api-0.1.3/tests/test.py
```

### Comparing `chaseinvest_api-0.1.2/LICENSE` & `chaseinvest_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chaseinvest_api-0.1.2/PKG-INFO` & `chaseinvest_api-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chaseinvest-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: An unofficial API for Chase Invest
 Home-page: https://github.com/MaxxRK/chaseinvest-api
-Download-URL: https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.3.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: CHASE,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
@@ -56,16 +56,16 @@
 import sys
 
 from chase import account as acc
 from chase import order as och
 from chase import session
 from chase import symbols as sym
 
-# create Session
-cs = session.ChaseSession(title="Title of your profile here", headless=True, profile_path='your/profile/path')
+# create Session Headless does not work at the moment it must be set to false.
+cs = session.ChaseSession(title="Title of your profile here", headless=False, profile_path='your/profile/path')
 
 # Login to Chase.com
 login_one = cs.login("your_username", "your_password", "last_four_of_your_cell_phone")
 
 # Check if login succeeded without needing 2fa if not then prompt for 2fa code
 if login_one == False:
     print('Login succeeded without needing 2fa...')
```

### Comparing `chaseinvest_api-0.1.2/README.md` & `chaseinvest_api-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 import sys
 
 from chase import account as acc
 from chase import order as och
 from chase import session
 from chase import symbols as sym
 
-# create Session
-cs = session.ChaseSession(title="Title of your profile here", headless=True, profile_path='your/profile/path')
+# create Session Headless does not work at the moment it must be set to false.
+cs = session.ChaseSession(title="Title of your profile here", headless=False, profile_path='your/profile/path')
 
 # Login to Chase.com
 login_one = cs.login("your_username", "your_password", "last_four_of_your_cell_phone")
 
 # Check if login succeeded without needing 2fa if not then prompt for 2fa code
 if login_one == False:
     print('Login succeeded without needing 2fa...')
```

### Comparing `chaseinvest_api-0.1.2/chase/account.py` & `chaseinvest_api-0.1.3/chase/account.py`

 * *Files identical despite different names*

### Comparing `chaseinvest_api-0.1.2/chase/order.py` & `chaseinvest_api-0.1.3/chase/order.py`

 * *Files identical despite different names*

### Comparing `chaseinvest_api-0.1.2/chase/session.py` & `chaseinvest_api-0.1.3/chase/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,17 @@
         with open(self.profile_path, "w") as f:
             json.dump(storage_state, f)
 
     def close_browser(self):
         """Closes the browser."""
         self.save_storage_state()
         if self.debug:
-            self.context.tracing.stop(path="./chase_trace.zip")
+            self.context.tracing.stop(
+                path=f'./chase_trace{self.title if self.title is not None else ""}.zip'
+            )
         self.browser.close()
         self.playwright.stop()
 
     def login(self, username, password, last_four):
         """
         Logs into the website with the provided username and password.
```

### Comparing `chaseinvest_api-0.1.2/chase/symbols.py` & `chaseinvest_api-0.1.3/chase/symbols.py`

 * *Files identical despite different names*

### Comparing `chaseinvest_api-0.1.2/chase/urls.py` & `chaseinvest_api-0.1.3/chase/urls.py`

 * *Files identical despite different names*

### Comparing `chaseinvest_api-0.1.2/chaseinvest_api.egg-info/PKG-INFO` & `chaseinvest_api-0.1.3/chaseinvest_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chaseinvest-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: An unofficial API for Chase Invest
 Home-page: https://github.com/MaxxRK/chaseinvest-api
-Download-URL: https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.3.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: CHASE,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
@@ -56,16 +56,16 @@
 import sys
 
 from chase import account as acc
 from chase import order as och
 from chase import session
 from chase import symbols as sym
 
-# create Session
-cs = session.ChaseSession(title="Title of your profile here", headless=True, profile_path='your/profile/path')
+# create Session Headless does not work at the moment it must be set to false.
+cs = session.ChaseSession(title="Title of your profile here", headless=False, profile_path='your/profile/path')
 
 # Login to Chase.com
 login_one = cs.login("your_username", "your_password", "last_four_of_your_cell_phone")
 
 # Check if login succeeded without needing 2fa if not then prompt for 2fa code
 if login_one == False:
     print('Login succeeded without needing 2fa...')
```

### Comparing `chaseinvest_api-0.1.2/setup.py` & `chaseinvest_api-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="chaseinvest-api",
-    version="0.1.2",
+    version="0.1.3",
     author="MaxxRK",
     author_email="maxxrk@pm.me",
     description="An unofficial API for Chase Invest",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/MaxxRK/chaseinvest-api",
-    download_url="https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.2.tar.gz",
+    download_url="https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.3.tar.gz",
     keywords=["CHASE", "API"],
     install_requires=["playwright", "playwright-stealth"],
     packages=["chase"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP :: Session",
```

### Comparing `chaseinvest_api-0.1.2/tests/test.py` & `chaseinvest_api-0.1.3/tests/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import sys
 
 from chase import account as acc
 from chase import order as och
 from chase import session
 from chase import symbols as sym
 
-# create Session
+# create Session Headless does not work at the moment it must be set to false.
 cs = session.ChaseSession(
-    title="Title of your profile here", headless=True, profile_path="your/profile/path"
+    title="Title of your profile here", headless=False, profile_path="your/profile/path"
 )
 
 # Login to Chase.com
 login_one = cs.login("your_username", "your_password", "last_four_of_your_cell_phone")
 
 # Check if login succeeded without needing 2fa if not then prompt for 2fa code
 if login_one is False:
```

