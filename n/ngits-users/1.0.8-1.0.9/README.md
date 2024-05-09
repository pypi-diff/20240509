# Comparing `tmp/ngits-users-1.0.8.tar.gz` & `tmp/ngits-users-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngits-users-1.0.8.tar", last modified: Fri Apr 21 10:50:58 2023, max compression
+gzip compressed data, was "ngits-users-1.0.9.tar", last modified: Thu May  9 15:18:15 2024, max compression
```

## Comparing `ngits-users-1.0.8.tar` & `ngits-users-1.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:58.954570 ngits-users-1.0.8/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      136 2023-04-21 06:52:22.000000 ngits-users-1.0.8/MANIFEST.in
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    10028 2023-04-21 10:50:58.954570 ngits-users-1.0.8/PKG-INFO
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     6888 2023-04-21 08:22:27.000000 ngits-users-1.0.8/README.rst
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      736 2023-04-21 06:52:22.000000 ngits-users-1.0.8/pyproject.toml
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      803 2023-04-21 10:50:58.954570 ngits-users-1.0.8/setup.cfg
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       38 2023-04-21 06:52:22.000000 ngits-users-1.0.8/setup.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:58.946570 ngits-users-1.0.8/src/
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:58.950570 ngits-users-1.0.8/src/ngits_users.egg-info/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    10028 2023-04-21 10:50:58.000000 ngits-users-1.0.8/src/ngits_users.egg-info/PKG-INFO
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1078 2023-04-21 10:50:58.000000 ngits-users-1.0.8/src/ngits_users.egg-info/SOURCES.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        1 2023-04-21 10:50:58.000000 ngits-users-1.0.8/src/ngits_users.egg-info/dependency_links.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       98 2023-04-21 10:50:58.000000 ngits-users-1.0.8/src/ngits_users.egg-info/requires.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        6 2023-04-21 10:50:58.000000 ngits-users-1.0.8/src/ngits_users.egg-info/top_level.txt
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:58.950570 ngits-users-1.0.8/src/users/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/__init__.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      368 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/admin.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      193 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/apps.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1997 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/forms.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:58.950570 ngits-users-1.0.8/src/users/migrations/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3021 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/migrations/0001_initial.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/migrations/__init__.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      344 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/models.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3657 2023-04-21 08:17:08.000000 ngits-users-1.0.8/src/users/schemas.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3122 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/serializers.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      357 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/signals.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:58.946570 ngits-users-1.0.8/src/users/static/
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:58.946570 ngits-users-1.0.8/src/users/static/users/
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:58.950570 ngits-users-1.0.8/src/users/static/users/css/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     2333 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/static/users/css/style.css
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:58.954570 ngits-users-1.0.8/src/users/static/users/img/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    11327 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/static/users/img/fail.svg
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    20062 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/static/users/img/success.svg
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      603 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/tasks.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:58.954570 ngits-users-1.0.8/src/users/templates/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      538 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/templates/change_password.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      118 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/templates/change_password_email.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       71 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/templates/change_password_email.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      602 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/templates/form_site.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      575 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/templates/info_site.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      395 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/templates/password_changed.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      117 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/templates/registration_email.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       70 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/templates/registration_email.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      384 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/templates/verify_error.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      389 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/templates/verify_ok.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1302 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/urls.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3047 2023-04-21 06:52:22.000000 ngits-users-1.0.8/src/users/utils.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    12257 2023-04-21 08:22:27.000000 ngits-users-1.0.8/src/users/views.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-05-09 15:18:15.268447 ngits-users-1.0.9/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      136 2024-05-09 15:04:14.000000 ngits-users-1.0.9/MANIFEST.in
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    10140 2024-05-09 15:18:15.268447 ngits-users-1.0.9/PKG-INFO
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     6984 2024-05-09 15:04:14.000000 ngits-users-1.0.9/README.rst
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      736 2024-05-09 15:04:14.000000 ngits-users-1.0.9/pyproject.toml
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      803 2024-05-09 15:18:15.268447 ngits-users-1.0.9/setup.cfg
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       38 2024-05-09 15:04:14.000000 ngits-users-1.0.9/setup.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-05-09 15:18:15.264447 ngits-users-1.0.9/src/
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-05-09 15:18:15.264447 ngits-users-1.0.9/src/ngits_users.egg-info/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    10140 2024-05-09 15:18:15.000000 ngits-users-1.0.9/src/ngits_users.egg-info/PKG-INFO
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1078 2024-05-09 15:18:15.000000 ngits-users-1.0.9/src/ngits_users.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        1 2024-05-09 15:18:15.000000 ngits-users-1.0.9/src/ngits_users.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       98 2024-05-09 15:18:15.000000 ngits-users-1.0.9/src/ngits_users.egg-info/requires.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        6 2024-05-09 15:18:15.000000 ngits-users-1.0.9/src/ngits_users.egg-info/top_level.txt
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-05-09 15:18:15.268447 ngits-users-1.0.9/src/users/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/__init__.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      368 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/admin.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      193 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/apps.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1997 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/forms.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-05-09 15:18:15.268447 ngits-users-1.0.9/src/users/migrations/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3021 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/migrations/0001_initial.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/migrations/__init__.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      344 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/models.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3657 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/schemas.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3122 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/serializers.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      357 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/signals.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-05-09 15:18:15.264447 ngits-users-1.0.9/src/users/static/
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-05-09 15:18:15.264447 ngits-users-1.0.9/src/users/static/users/
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-05-09 15:18:15.268447 ngits-users-1.0.9/src/users/static/users/css/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     2333 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/static/users/css/style.css
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-05-09 15:18:15.268447 ngits-users-1.0.9/src/users/static/users/img/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    11327 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/static/users/img/fail.svg
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    20062 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/static/users/img/success.svg
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      603 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/tasks.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2024-05-09 15:18:15.268447 ngits-users-1.0.9/src/users/templates/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      538 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/templates/change_password.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      118 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/templates/change_password_email.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       71 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/templates/change_password_email.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      602 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/templates/form_site.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      575 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/templates/info_site.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      395 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/templates/password_changed.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      117 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/templates/registration_email.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       70 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/templates/registration_email.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      384 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/templates/verify_error.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      389 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/templates/verify_ok.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1302 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/urls.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3068 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/utils.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    12257 2024-05-09 15:04:14.000000 ngits-users-1.0.9/src/users/views.py
```

### Comparing `ngits-users-1.0.8/PKG-INFO` & `ngits-users-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ngits-users
-Version: 1.0.8
+Version: 1.0.9
 Summary: Base users application for Django projects
 Home-page: https://ngits.dev
 Author: NGITs
 License: BSD-3-Clause
 Description: ngits-users
         ============
         
@@ -229,14 +229,16 @@
                 - ``registration_email.html``
                 - ``registration_email.txt``
             - View templates:
                 - ``change_password.html`` - **this have to contain {{ form }} !**
                 - ``verify_ok.html``
                 - ``verify_error.html``
         
+        There's also additional :code:`{{ email }}` context param you can use in your email templates.
+        
         e.g.:
         
         ::
         
             /repo
                 /manage.py
                 /templates
```

### Comparing `ngits-users-1.0.8/README.rst` & `ngits-users-1.0.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,16 @@
         - ``registration_email.html``
         - ``registration_email.txt``
     - View templates:
         - ``change_password.html`` - **this have to contain {{ form }} !**
         - ``verify_ok.html``
         - ``verify_error.html``
 
+There's also additional :code:`{{ email }}` context param you can use in your email templates.
+
 e.g.:
 
 ::
 
     /repo
         /manage.py
         /templates
```

### Comparing `ngits-users-1.0.8/pyproject.toml` & `ngits-users-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/setup.cfg` & `ngits-users-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ngits-users
-version = 1.0.8
+version = 1.0.9
 description = Base users application for Django projects
 long_description = file: README.rst
 url = https://ngits.dev
 author = NGITs
 license = BSD-3-Clause
 classifiers = 
 	Environment :: Web Environment
```

### Comparing `ngits-users-1.0.8/src/ngits_users.egg-info/PKG-INFO` & `ngits-users-1.0.9/src/ngits_users.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ngits-users
-Version: 1.0.8
+Version: 1.0.9
 Summary: Base users application for Django projects
 Home-page: https://ngits.dev
 Author: NGITs
 License: BSD-3-Clause
 Description: ngits-users
         ============
         
@@ -229,14 +229,16 @@
                 - ``registration_email.html``
                 - ``registration_email.txt``
             - View templates:
                 - ``change_password.html`` - **this have to contain {{ form }} !**
                 - ``verify_ok.html``
                 - ``verify_error.html``
         
+        There's also additional :code:`{{ email }}` context param you can use in your email templates.
+        
         e.g.:
         
         ::
         
             /repo
                 /manage.py
                 /templates
```

### Comparing `ngits-users-1.0.8/src/ngits_users.egg-info/SOURCES.txt` & `ngits-users-1.0.9/src/ngits_users.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/forms.py` & `ngits-users-1.0.9/src/users/forms.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/migrations/0001_initial.py` & `ngits-users-1.0.9/src/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/schemas.py` & `ngits-users-1.0.9/src/users/schemas.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/serializers.py` & `ngits-users-1.0.9/src/users/serializers.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/static/users/css/style.css` & `ngits-users-1.0.9/src/users/static/users/css/style.css`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/static/users/img/fail.svg` & `ngits-users-1.0.9/src/users/static/users/img/fail.svg`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/static/users/img/success.svg` & `ngits-users-1.0.9/src/users/static/users/img/success.svg`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/tasks.py` & `ngits-users-1.0.9/src/users/tasks.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/templates/change_password.html` & `ngits-users-1.0.9/src/users/templates/change_password.html`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/templates/form_site.html` & `ngits-users-1.0.9/src/users/templates/form_site.html`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/templates/info_site.html` & `ngits-users-1.0.9/src/users/templates/info_site.html`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/urls.py` & `ngits-users-1.0.9/src/users/urls.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.8/src/users/utils.py` & `ngits-users-1.0.9/src/users/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         URL = "{}://{}{}?user={}&key={}".format(
             protocol,
             host,
             reverse(self.EMAIL_TEMPLATES[self.template]["url"]),
             user.pk,
             hash,
         )
-        context = {"url": URL}
+        context = {"url": URL, "email": user.email}
         text_template = get_template(
             self.EMAIL_TEMPLATES[self.template]["text_template"]
         )
         html_template = get_template(
             self.EMAIL_TEMPLATES[self.template]["html_template"]
         )
```

### Comparing `ngits-users-1.0.8/src/users/views.py` & `ngits-users-1.0.9/src/users/views.py`

 * *Files identical despite different names*

