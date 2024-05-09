# Comparing `tmp/st_paywall-0.1.7.tar.gz` & `tmp/st_paywall-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_paywall-0.1.7.tar", last modified: Tue May  7 17:31:44 2024, max compression
+gzip compressed data, was "st_paywall-0.1.8.tar", last modified: Thu May  9 15:16:24 2024, max compression
```

## Comparing `st_paywall-0.1.7.tar` & `st_paywall-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2024-05-07 17:31:44.780587 st_paywall-0.1.7/
--rw-r--r--   0 trichards   (501) staff       (20)     1068 2024-03-24 02:06:46.000000 st_paywall-0.1.7/LICENSE
--rw-r--r--   0 trichards   (501) staff       (20)     3547 2024-05-07 17:31:44.780159 st_paywall-0.1.7/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)     3166 2023-09-24 19:23:05.000000 st_paywall-0.1.7/README.md
--rw-r--r--   0 trichards   (501) staff       (20)      417 2024-05-07 17:30:19.000000 st_paywall-0.1.7/pyproject.toml
--rw-r--r--   0 trichards   (501) staff       (20)       38 2024-05-07 17:31:44.780639 st_paywall-0.1.7/setup.cfg
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2024-05-07 17:31:44.773295 st_paywall-0.1.7/src/
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2024-05-07 17:31:44.776184 st_paywall-0.1.7/src/st_paywall/
--rw-r--r--   0 trichards   (501) staff       (20)       45 2023-09-24 19:23:05.000000 st_paywall-0.1.7/src/st_paywall/__init__.py
--rw-r--r--   0 trichards   (501) staff       (20)     3149 2024-03-24 02:06:49.000000 st_paywall-0.1.7/src/st_paywall/aggregate_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     1414 2023-09-24 19:23:05.000000 st_paywall-0.1.7/src/st_paywall/buymeacoffee_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     3112 2024-05-07 17:30:19.000000 st_paywall-0.1.7/src/st_paywall/google_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     1746 2024-03-24 02:06:49.000000 st_paywall-0.1.7/src/st_paywall/stripe_auth.py
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2024-05-07 17:31:44.779658 st_paywall-0.1.7/src/st_paywall.egg-info/
--rw-r--r--   0 trichards   (501) staff       (20)     3547 2024-05-07 17:31:44.000000 st_paywall-0.1.7/src/st_paywall.egg-info/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)      377 2024-05-07 17:31:44.000000 st_paywall-0.1.7/src/st_paywall.egg-info/SOURCES.txt
--rw-r--r--   0 trichards   (501) staff       (20)        1 2024-05-07 17:31:44.000000 st_paywall-0.1.7/src/st_paywall.egg-info/dependency_links.txt
--rw-r--r--   0 trichards   (501) staff       (20)       43 2024-05-07 17:31:44.000000 st_paywall-0.1.7/src/st_paywall.egg-info/requires.txt
--rw-r--r--   0 trichards   (501) staff       (20)       11 2024-05-07 17:31:44.000000 st_paywall-0.1.7/src/st_paywall.egg-info/top_level.txt
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2024-05-09 15:16:24.644585 st_paywall-0.1.8/
+-rw-r--r--   0 trichards   (501) staff       (20)     1068 2024-03-24 02:06:46.000000 st_paywall-0.1.8/LICENSE
+-rw-r--r--   0 trichards   (501) staff       (20)     3547 2024-05-09 15:16:24.644166 st_paywall-0.1.8/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)     3166 2023-09-24 19:23:05.000000 st_paywall-0.1.8/README.md
+-rw-r--r--   0 trichards   (501) staff       (20)      417 2024-05-09 15:15:53.000000 st_paywall-0.1.8/pyproject.toml
+-rw-r--r--   0 trichards   (501) staff       (20)       38 2024-05-09 15:16:24.644648 st_paywall-0.1.8/setup.cfg
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2024-05-09 15:16:24.637235 st_paywall-0.1.8/src/
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2024-05-09 15:16:24.640529 st_paywall-0.1.8/src/st_paywall/
+-rw-r--r--   0 trichards   (501) staff       (20)       45 2023-09-24 19:23:05.000000 st_paywall-0.1.8/src/st_paywall/__init__.py
+-rw-r--r--   0 trichards   (501) staff       (20)     3149 2024-03-24 02:06:49.000000 st_paywall-0.1.8/src/st_paywall/aggregate_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1414 2023-09-24 19:23:05.000000 st_paywall-0.1.8/src/st_paywall/buymeacoffee_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     3067 2024-05-09 15:15:53.000000 st_paywall-0.1.8/src/st_paywall/google_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1746 2024-03-24 02:06:49.000000 st_paywall-0.1.8/src/st_paywall/stripe_auth.py
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2024-05-09 15:16:24.643629 st_paywall-0.1.8/src/st_paywall.egg-info/
+-rw-r--r--   0 trichards   (501) staff       (20)     3547 2024-05-09 15:16:24.000000 st_paywall-0.1.8/src/st_paywall.egg-info/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)      377 2024-05-09 15:16:24.000000 st_paywall-0.1.8/src/st_paywall.egg-info/SOURCES.txt
+-rw-r--r--   0 trichards   (501) staff       (20)        1 2024-05-09 15:16:24.000000 st_paywall-0.1.8/src/st_paywall.egg-info/dependency_links.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       43 2024-05-09 15:16:24.000000 st_paywall-0.1.8/src/st_paywall.egg-info/requires.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       11 2024-05-09 15:16:24.000000 st_paywall-0.1.8/src/st_paywall.egg-info/top_level.txt
```

### Comparing `st_paywall-0.1.7/LICENSE` & `st_paywall-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `st_paywall-0.1.7/PKG-INFO` & `st_paywall-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-paywall
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package for creating subscription Streamlit apps
 Author-email: Tyler Richards <tylerjrichards@gmail.com>
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: stripe
```

### Comparing `st_paywall-0.1.7/README.md` & `st_paywall-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `st_paywall-0.1.7/src/st_paywall/aggregate_auth.py` & `st_paywall-0.1.8/src/st_paywall/aggregate_auth.py`

 * *Files identical despite different names*

### Comparing `st_paywall-0.1.7/src/st_paywall/buymeacoffee_auth.py` & `st_paywall-0.1.8/src/st_paywall/buymeacoffee_auth.py`

 * *Files identical despite different names*

### Comparing `st_paywall-0.1.7/src/st_paywall/google_auth.py` & `st_paywall-0.1.8/src/st_paywall/google_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,16 +77,15 @@
     token = await client.get_access_token(code, redirect_url)
     return token
 
 
 def get_access_token_from_query_params(
     client: GoogleOAuth2, redirect_url: str
 ) -> OAuth2Token:
-    query_params = st.query_params.get_all()
-    code = query_params["code"][0]
+    code = st.query_params["code"]
     token = asyncio.run(
         get_access_token(client=client, redirect_url=redirect_url, code=code)
     )
     # Clear query params
     st.query_params.clear()
     return token
```

### Comparing `st_paywall-0.1.7/src/st_paywall/stripe_auth.py` & `st_paywall-0.1.8/src/st_paywall/stripe_auth.py`

 * *Files identical despite different names*

### Comparing `st_paywall-0.1.7/src/st_paywall.egg-info/PKG-INFO` & `st_paywall-0.1.8/src/st_paywall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-paywall
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package for creating subscription Streamlit apps
 Author-email: Tyler Richards <tylerjrichards@gmail.com>
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: stripe
```

